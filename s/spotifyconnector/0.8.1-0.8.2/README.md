# Comparing `tmp/spotifyconnector-0.8.1.tar.gz` & `tmp/spotifyconnector-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotifyconnector-0.8.1.tar", last modified: Mon Nov 27 20:40:54 2023, max compression
+gzip compressed data, was "spotifyconnector-0.8.2.tar", last modified: Sat Apr 20 16:27:07 2024, max compression
```

## Comparing `spotifyconnector-0.8.1.tar` & `spotifyconnector-0.8.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mendler    (501) staff       (20)        0 2023-11-27 20:40:54.082094 spotifyconnector-0.8.1/
--rw-r--r--   0 mendler    (501) staff       (20)     1085 2022-11-02 14:26:49.000000 spotifyconnector-0.8.1/LICENSE
--rw-r--r--   0 mendler    (501) staff       (20)     3249 2023-11-27 20:40:54.081981 spotifyconnector-0.8.1/PKG-INFO
--rw-r--r--   0 mendler    (501) staff       (20)     3048 2023-11-27 20:39:02.000000 spotifyconnector-0.8.1/README.md
--rw-r--r--   0 mendler    (501) staff       (20)       38 2023-11-27 20:40:54.082128 spotifyconnector-0.8.1/setup.cfg
--rw-r--r--   0 mendler    (501) staff       (20)      833 2023-11-27 20:39:02.000000 spotifyconnector-0.8.1/setup.py
-drwxr-xr-x   0 mendler    (501) staff       (20)        0 2023-11-27 20:40:54.081162 spotifyconnector-0.8.1/spotifyconnector/
--rw-r--r--   0 mendler    (501) staff       (20)      236 2023-11-27 18:26:55.000000 spotifyconnector-0.8.1/spotifyconnector/__init__.py
--rw-r--r--   0 mendler    (501) staff       (20)     3494 2023-11-27 18:26:55.000000 spotifyconnector-0.8.1/spotifyconnector/__main__.py
--rw-r--r--   0 mendler    (501) staff       (20)    17288 2023-11-27 20:39:02.000000 spotifyconnector-0.8.1/spotifyconnector/connector.py
-drwxr-xr-x   0 mendler    (501) staff       (20)        0 2023-11-27 20:40:54.081833 spotifyconnector-0.8.1/spotifyconnector.egg-info/
--rw-r--r--   0 mendler    (501) staff       (20)     3249 2023-11-27 20:40:54.000000 spotifyconnector-0.8.1/spotifyconnector.egg-info/PKG-INFO
--rw-r--r--   0 mendler    (501) staff       (20)      356 2023-11-27 20:40:54.000000 spotifyconnector-0.8.1/spotifyconnector.egg-info/SOURCES.txt
--rw-r--r--   0 mendler    (501) staff       (20)        1 2023-11-27 20:40:54.000000 spotifyconnector-0.8.1/spotifyconnector.egg-info/dependency_links.txt
--rw-r--r--   0 mendler    (501) staff       (20)       68 2023-11-27 20:40:54.000000 spotifyconnector-0.8.1/spotifyconnector.egg-info/entry_points.txt
--rw-r--r--   0 mendler    (501) staff       (20)       32 2023-11-27 20:40:54.000000 spotifyconnector-0.8.1/spotifyconnector.egg-info/requires.txt
--rw-r--r--   0 mendler    (501) staff       (20)       17 2023-11-27 20:40:54.000000 spotifyconnector-0.8.1/spotifyconnector.egg-info/top_level.txt
+drwxr-xr-x   0 mendler    (501) staff       (20)        0 2024-04-20 16:27:07.646823 spotifyconnector-0.8.2/
+-rw-r--r--   0 mendler    (501) staff       (20)     1085 2024-04-20 16:24:50.000000 spotifyconnector-0.8.2/LICENSE
+-rw-r--r--   0 mendler    (501) staff       (20)     3508 2024-04-20 16:27:07.646696 spotifyconnector-0.8.2/PKG-INFO
+-rw-r--r--   0 mendler    (501) staff       (20)     3307 2024-04-20 16:20:37.000000 spotifyconnector-0.8.2/README.md
+-rw-r--r--   0 mendler    (501) staff       (20)       38 2024-04-20 16:27:07.646856 spotifyconnector-0.8.2/setup.cfg
+-rw-r--r--   0 mendler    (501) staff       (20)      854 2024-04-20 16:25:06.000000 spotifyconnector-0.8.2/setup.py
+drwxr-xr-x   0 mendler    (501) staff       (20)        0 2024-04-20 16:27:07.645654 spotifyconnector-0.8.2/spotifyconnector/
+-rw-r--r--   0 mendler    (501) staff       (20)      278 2024-04-20 16:26:35.000000 spotifyconnector-0.8.2/spotifyconnector/__init__.py
+-rw-r--r--   0 mendler    (501) staff       (20)     3235 2024-01-20 18:59:50.000000 spotifyconnector-0.8.2/spotifyconnector/__main__.py
+-rw-r--r--   0 mendler    (501) staff       (20)    19670 2024-01-20 19:00:12.000000 spotifyconnector-0.8.2/spotifyconnector/connector.py
+drwxr-xr-x   0 mendler    (501) staff       (20)        0 2024-04-20 16:27:07.646538 spotifyconnector-0.8.2/spotifyconnector.egg-info/
+-rw-r--r--   0 mendler    (501) staff       (20)     3508 2024-04-20 16:27:07.000000 spotifyconnector-0.8.2/spotifyconnector.egg-info/PKG-INFO
+-rw-r--r--   0 mendler    (501) staff       (20)      356 2024-04-20 16:27:07.000000 spotifyconnector-0.8.2/spotifyconnector.egg-info/SOURCES.txt
+-rw-r--r--   0 mendler    (501) staff       (20)        1 2024-04-20 16:27:07.000000 spotifyconnector-0.8.2/spotifyconnector.egg-info/dependency_links.txt
+-rw-r--r--   0 mendler    (501) staff       (20)       68 2024-04-20 16:27:07.000000 spotifyconnector-0.8.2/spotifyconnector.egg-info/entry_points.txt
+-rw-r--r--   0 mendler    (501) staff       (20)       50 2024-04-20 16:27:07.000000 spotifyconnector-0.8.2/spotifyconnector.egg-info/requires.txt
+-rw-r--r--   0 mendler    (501) staff       (20)       17 2024-04-20 16:27:07.000000 spotifyconnector-0.8.2/spotifyconnector.egg-info/top_level.txt
```

### Comparing `spotifyconnector-0.8.1/LICENSE` & `spotifyconnector-0.8.2/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 The Open Podcast maintainers
+Copyright (c) 2024 The Open Podcast maintainers
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `spotifyconnector-0.8.1/PKG-INFO` & `spotifyconnector-0.8.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: spotifyconnector
-Version: 0.8.1
+Version: 0.8.2
 Summary: Spotify Connector for Podcast Data
 Author: Open Podcast
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Spotify Connector
 
+[![Docs](https://readthedocs.org/projects/spotify-connector/badge?version=latest)](https://spotify-connector.readthedocs.io)
+
+[![OpenPodcast Banner](https://raw.githubusercontent.com/openpodcast/banner/main/openpodcast-banner.png)](https://openpodcast.app/)
+
 This is a simple library for connecting to the unofficial Spotify podcast API.  
 It can be used to export data from your dashboard at
 https://podcasters.spotify.com/home.
 
 ## Supported Data
 
 - List of episodes
@@ -25,15 +29,15 @@
 - Episode performance
 
 ## Credentials
 
 Before you can use the library, you must extract your Spotify credentials from the dashboard;
 they are **not** exposed through your Spotify settings.
 
-You can use our [web-extension](https://github.com/openpodcast/web-extension) for that
+You can use our [web extension](https://github.com/openpodcast/web-extension) for that
 or [take a look at the code](https://github.com/openpodcast/web-extension/blob/7ce0865d22bea34fcfc53eec06b25cd076aa8034/src/openpodcast.js)
 to see how to do it manually.
 
 ## Installation
 
 ```
 pip install spotifyconnector
@@ -90,15 +94,15 @@
 ```
 
 ## Development
 
 We use [Pipenv] for virtualenv and dev dependency management. With Pipenv
 installed:
 
-1. Install your locally checked out code in [development mode], including its
+1. Install your locally checked-out code in [development mode], including its
    dependencies, and all dev dependencies into a virtual environment:
 
 ```sh
 pipenv sync --dev
 ```
 
 2. Create an environment file and fill in the required values:
```

### Comparing `spotifyconnector-0.8.1/README.md` & `spotifyconnector-0.8.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Spotify Connector
 
+[![Docs](https://readthedocs.org/projects/spotify-connector/badge?version=latest)](https://spotify-connector.readthedocs.io)
+
+[![OpenPodcast Banner](https://raw.githubusercontent.com/openpodcast/banner/main/openpodcast-banner.png)](https://openpodcast.app/)
+
 This is a simple library for connecting to the unofficial Spotify podcast API.  
 It can be used to export data from your dashboard at
 https://podcasters.spotify.com/home.
 
 ## Supported Data
 
 - List of episodes
@@ -16,15 +20,15 @@
 - Episode performance
 
 ## Credentials
 
 Before you can use the library, you must extract your Spotify credentials from the dashboard;
 they are **not** exposed through your Spotify settings.
 
-You can use our [web-extension](https://github.com/openpodcast/web-extension) for that
+You can use our [web extension](https://github.com/openpodcast/web-extension) for that
 or [take a look at the code](https://github.com/openpodcast/web-extension/blob/7ce0865d22bea34fcfc53eec06b25cd076aa8034/src/openpodcast.js)
 to see how to do it manually.
 
 ## Installation
 
 ```
 pip install spotifyconnector
@@ -81,15 +85,15 @@
 ```
 
 ## Development
 
 We use [Pipenv] for virtualenv and dev dependency management. With Pipenv
 installed:
 
-1. Install your locally checked out code in [development mode], including its
+1. Install your locally checked-out code in [development mode], including its
    dependencies, and all dev dependencies into a virtual environment:
 
 ```sh
 pipenv sync --dev
 ```
 
 2. Create an environment file and fill in the required values:
```

### Comparing `spotifyconnector-0.8.1/setup.py` & `spotifyconnector-0.8.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="spotifyconnector",
     packages=find_packages(include=["spotifyconnector"]),
-    version="0.8.1",
+    version="0.8.2",
     description="Spotify Connector for Podcast Data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Open Podcast",
     license="MIT",
     entry_points={
         "console_scripts": [
             "spotifyconnector = spotifyconnector.__main__:main",
         ]
     },
-    install_requires=["requests", "loguru", "PyYAML", "tenacity"],
+    install_requires=["requests", "loguru", "PyYAML", "tenacity", "myst_parser[docs]"],
 )
```

### Comparing `spotifyconnector-0.8.1/spotifyconnector/connector.py` & `spotifyconnector-0.8.2/spotifyconnector/connector.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,30 +22,29 @@
 from tenacity.stop import stop_after_attempt
 from tenacity.wait import wait_exponential
 from tenacity.retry import retry_if_exception_type
 import yaml
 
 DELAY_BASE = 2.0
 MAX_REQUEST_ATTEMPTS = 6
+# The Spotify API imposes exactly 29 days of data for "total" and "faceted" impressions
+IMPRESSIONS_DAYS_DIFF = 29
 
 
 class CredentialsExpired(Exception):
-    """
-    CredentialsExpired is raised when the Spotify API asks for a login
+    """CredentialsExpired is raised when the Spotify API asks for a login
     This is usually because the cookies have expired.
     """
 
 
-def random_string(
+def _random_string(
     length: int,
     chars: str = string.ascii_lowercase + string.ascii_uppercase + string.digits,
 ) -> str:
-    """
-    Simple helper function to generate random strings suitable for use with Spotify
-    """
+    """Simple helper function to generate random strings suitable for use with Spotify"""
     return "".join(random.choices(chars, k=length))
 
 
 class MaxRetriesException(Exception):
     """
     Raised when the maximum number of retries is reached
     """
@@ -94,16 +93,15 @@
 
     @retry(
         retry=retry_if_exception_type(HTTPError),
         wait=wait_exponential(),
         stop=stop_after_attempt(7),
     )
     def _authenticate(self):
-        """
-        Retrieves a Bearer token for the inofficial Spotify API, valid 1 hour.
+        """Retrieves a Bearer token for the inofficial Spotify API, valid 1 hour.
 
         Generally follows the steps outlined here:
         https://developer.spotify.com/documentation/general/guides/authorization/code-flow/
         (with a few exceptions)
         """
         if self._auth_poisoned:
             raise CredentialsExpired(
@@ -112,17 +110,17 @@
             )
 
         with self._auth_lock:
             logger.info("Retrieving Bearer")
 
             logger.debug("Generating secrets")
 
-            state = random_string(32)
+            state = _random_string(32)
 
-            code_verifier = random_string(64)
+            code_verifier = _random_string(64)
             code_challenge = base64.b64encode(
                 hashlib.sha256(code_verifier.encode("utf-8")).digest()
             ).decode("utf-8")
 
             # Fix up format of code_challenge for spotify
             code_challenge = re.sub(r"=+$", "", code_challenge)
             code_challenge = code_challenge.replace("/", "_")
@@ -400,14 +398,76 @@
         url = self._build_url(
             "shows",
             self.podcast_id,
             "followers",
         )
         return self._request(url, params=self._date_params(start, end))
 
+    def _set_impression_date_range(self, kind: str, start: dt.date, end: dt.date):
+        """
+        The following conditions must hold for impression data:
+        - If kind is "total" or "faceted", start and end must be exactly
+          IMPRESSIONS_DAYS_DIFF days apart.
+          We override the date range if this is not the case.
+        - Otherwise, end may not be before start.
+
+        Returns the new start and end dates.
+        Logs a warning if the dates were invalid.
+        """
+        if kind in ("total", "faceted"):
+            new_end = start + dt.timedelta(days=IMPRESSIONS_DAYS_DIFF)
+            if new_end != end:
+                logger.warning(
+                    f"kind is {kind}, overriding end date to be "
+                    f"{IMPRESSIONS_DAYS_DIFF} days after start date ({start}). "
+                    f"New end date: {new_end}"
+                )
+            return start, new_end
+
+        if end < start:
+            logger.warning(
+                f"End date {end} is before start date {start}, "
+                "setting end date to start date."
+            )
+            end = start
+        return start, end
+
+    def impressions(
+        self,
+        kind: str = "total",
+        start: Optional[dt.date] = None,
+        end: Optional[dt.date] = None,
+    ) -> dict:
+        """Loads podcast impression data.
+
+        Args:
+            kind (str): Range of data to request. Can be "total", "daily", or "faceted".
+            start (dt.date): Earliest date to request data for.
+            end (Optional[dt.date], optional): Most recent date to request data for.
+              Defaults to None. Will be set to `start` if None.
+
+        Returns:
+            dict: [description]
+        """
+
+        initial_start = start or dt.date.today() - dt.timedelta(
+            days=IMPRESSIONS_DAYS_DIFF
+        )
+        initial_end = end or start + dt.timedelta(days=IMPRESSIONS_DAYS_DIFF)
+        start, end = self._set_impression_date_range(kind, initial_start, initial_end)
+        logger.info(f"kind = {kind}, start = {start}, end = {end}")
+
+        url = self._build_url(
+            "shows",
+            self.podcast_id,
+            "impressions",
+            kind,
+        )
+        return self._request(url, params=self._date_params(start, end))
+
     def aggregate(
         self,
         start: dt.date,
         end: Optional[dt.date] = None,
         episode=None,
     ) -> dict:
         """Loads podcast aggregate data, which includes the number of
```

### Comparing `spotifyconnector-0.8.1/spotifyconnector.egg-info/PKG-INFO` & `spotifyconnector-0.8.2/spotifyconnector.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: spotifyconnector
-Version: 0.8.1
+Version: 0.8.2
 Summary: Spotify Connector for Podcast Data
 Author: Open Podcast
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Spotify Connector
 
+[![Docs](https://readthedocs.org/projects/spotify-connector/badge?version=latest)](https://spotify-connector.readthedocs.io)
+
+[![OpenPodcast Banner](https://raw.githubusercontent.com/openpodcast/banner/main/openpodcast-banner.png)](https://openpodcast.app/)
+
 This is a simple library for connecting to the unofficial Spotify podcast API.  
 It can be used to export data from your dashboard at
 https://podcasters.spotify.com/home.
 
 ## Supported Data
 
 - List of episodes
@@ -25,15 +29,15 @@
 - Episode performance
 
 ## Credentials
 
 Before you can use the library, you must extract your Spotify credentials from the dashboard;
 they are **not** exposed through your Spotify settings.
 
-You can use our [web-extension](https://github.com/openpodcast/web-extension) for that
+You can use our [web extension](https://github.com/openpodcast/web-extension) for that
 or [take a look at the code](https://github.com/openpodcast/web-extension/blob/7ce0865d22bea34fcfc53eec06b25cd076aa8034/src/openpodcast.js)
 to see how to do it manually.
 
 ## Installation
 
 ```
 pip install spotifyconnector
@@ -90,15 +94,15 @@
 ```
 
 ## Development
 
 We use [Pipenv] for virtualenv and dev dependency management. With Pipenv
 installed:
 
-1. Install your locally checked out code in [development mode], including its
+1. Install your locally checked-out code in [development mode], including its
    dependencies, and all dev dependencies into a virtual environment:
 
 ```sh
 pipenv sync --dev
 ```
 
 2. Create an environment file and fill in the required values:
```

