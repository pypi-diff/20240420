# Comparing `tmp/weather_command-6.1.4.tar.gz` & `tmp/weather_command-6.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weather_command-6.1.4.tar", max compression
+gzip compressed data, was "weather_command-6.1.5.tar", max compression
```

## Comparing `weather_command-6.1.4.tar` & `weather_command-6.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1069 2023-10-02 18:39:14.770548 weather_command-6.1.4/LICENSE
--rw-r--r--   0        0        0     3392 2023-10-02 18:39:14.770548 weather_command-6.1.4/README.md
--rw-r--r--   0        0        0     1793 2023-10-02 18:39:14.774548 weather_command-6.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-10-02 18:39:14.774548 weather_command-6.1.4/weather_command/__init__.py
--rw-r--r--   0        0        0       95 2023-10-02 18:39:14.774548 weather_command-6.1.4/weather_command/__main__.py
--rw-r--r--   0        0        0    18650 2023-10-02 18:39:14.774548 weather_command-6.1.4/weather_command/_builder.py
--rw-r--r--   0        0        0     5382 2023-10-02 18:39:14.774548 weather_command-6.1.4/weather_command/_cache.py
--rw-r--r--   0        0        0     5262 2023-10-02 18:39:14.774548 weather_command-6.1.4/weather_command/_config.py
--rw-r--r--   0        0        0     2652 2023-10-02 18:39:14.774548 weather_command-6.1.4/weather_command/_location.py
--rw-r--r--   0        0        0      473 2023-10-02 18:39:14.774548 weather_command-6.1.4/weather_command/_utils.py
--rw-r--r--   0        0        0     2834 2023-10-02 18:39:14.774548 weather_command-6.1.4/weather_command/_weather.py
--rw-r--r--   0        0        0      459 2023-10-02 18:39:14.774548 weather_command-6.1.4/weather_command/errors.py
--rw-r--r--   0        0        0     9084 2023-10-02 18:39:14.774548 weather_command-6.1.4/weather_command/main.py
--rw-r--r--   0        0        0        0 2023-10-02 18:39:14.774548 weather_command-6.1.4/weather_command/models/__init__.py
--rw-r--r--   0        0        0      133 2023-10-02 18:39:14.774548 weather_command-6.1.4/weather_command/models/location.py
--rw-r--r--   0        0        0     3053 2023-10-02 18:39:14.774548 weather_command-6.1.4/weather_command/models/weather.py
--rw-r--r--   0        0        0        0 2023-10-02 18:39:14.774548 weather_command-6.1.4/weather_command/py.typed
--rw-r--r--   0        0        0     2816 2023-10-02 18:39:14.774548 weather_command-6.1.4/weather_command/settings_commands.py
--rw-r--r--   0        0        0     4390 1970-01-01 00:00:00.000000 weather_command-6.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-19 19:24:25.626369 weather_command-6.1.5/LICENSE
+-rw-r--r--   0        0        0     3392 2024-04-19 19:24:25.626369 weather_command-6.1.5/README.md
+-rw-r--r--   0        0        0     1765 2024-04-19 19:24:25.626369 weather_command-6.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-19 19:24:25.630369 weather_command-6.1.5/weather_command/__init__.py
+-rw-r--r--   0        0        0       95 2024-04-19 19:24:25.630369 weather_command-6.1.5/weather_command/__main__.py
+-rw-r--r--   0        0        0    18650 2024-04-19 19:24:25.630369 weather_command-6.1.5/weather_command/_builder.py
+-rw-r--r--   0        0        0     5382 2024-04-19 19:24:25.630369 weather_command-6.1.5/weather_command/_cache.py
+-rw-r--r--   0        0        0     5262 2024-04-19 19:24:25.630369 weather_command-6.1.5/weather_command/_config.py
+-rw-r--r--   0        0        0     2652 2024-04-19 19:24:25.630369 weather_command-6.1.5/weather_command/_location.py
+-rw-r--r--   0        0        0      473 2024-04-19 19:24:25.630369 weather_command-6.1.5/weather_command/_utils.py
+-rw-r--r--   0        0        0     2834 2024-04-19 19:24:25.630369 weather_command-6.1.5/weather_command/_weather.py
+-rw-r--r--   0        0        0      459 2024-04-19 19:24:25.630369 weather_command-6.1.5/weather_command/errors.py
+-rw-r--r--   0        0        0     9084 2024-04-19 19:24:25.630369 weather_command-6.1.5/weather_command/main.py
+-rw-r--r--   0        0        0        0 2024-04-19 19:24:25.630369 weather_command-6.1.5/weather_command/models/__init__.py
+-rw-r--r--   0        0        0      133 2024-04-19 19:24:25.630369 weather_command-6.1.5/weather_command/models/location.py
+-rw-r--r--   0        0        0     3053 2024-04-19 19:24:25.630369 weather_command-6.1.5/weather_command/models/weather.py
+-rw-r--r--   0        0        0        0 2024-04-19 19:24:25.630369 weather_command-6.1.5/weather_command/py.typed
+-rw-r--r--   0        0        0     2818 2024-04-19 19:24:25.630369 weather_command-6.1.5/weather_command/settings_commands.py
+-rw-r--r--   0        0        0     4442 1970-01-01 00:00:00.000000 weather_command-6.1.5/PKG-INFO
```

### Comparing `weather_command-6.1.4/LICENSE` & `weather_command-6.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `weather_command-6.1.4/README.md` & `weather_command-6.1.5/README.md`

 * *Files identical despite different names*

### Comparing `weather_command-6.1.4/pyproject.toml` & `weather_command-6.1.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,46 @@
 [tool.poetry]
 name = "weather-command"
-version = "6.1.4"
+version = "6.1.5"
 description = "Command line weather app"
 authors = ["Paul Sanders <psanders1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sanders41/weather-command"
 homepage = "https://github.com/sanders41/weather-command"
 documentation = "https://github.com/sanders41/weather-command"
 keywords = ["weather", "cli"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-rich = "13.5.3"
-httpx = "0.25.0"
-pydantic = "2.4.2"
-camel-converter = {version = "3.0.2", extras = ["pydantic"]}
-typer = "0.9.0"
+rich = "13.7.1"
+httpx = "0.27.0"
+pydantic = "2.7.0"
+camel-converter = {version = "3.1.1", extras = ["pydantic"]}
+typer = "0.12.3"
 tenacity = "8.2.3"
 pyyaml = "6.0.1"
 
 [tool.poetry.group.dev.dependencies]
-black = "23.9.1"
-mypy = "1.5.1"
-pre-commit = "3.4.0"
-pytest = "7.4.2"
-pytest-cov = "4.1.0"
-ruff = "0.0.291"
+mypy = "1.9.0"
+pre-commit = "3.5.0"
+pytest = "8.1.1"
+pytest-cov = "5.0.0"
+ruff = "0.4.0"
 tomli = {version = "2.0.1", python = "<3.11"}
-types-pyyaml = "6.0.12.12"
-pytest-asyncio = "0.21.1"
+types-pyyaml = "6.0.12.20240311"
+pytest-asyncio = "0.23.6"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 weather = "weather_command.main:app"
 
-[tool.black]
-line-length = 100
-include = '\.pyi?$'
-exclude = '''
-/(
-    \.egg
-  | \.git
-  | \.hg
-  | \.mypy_cache
-  | \.nox
-  | \.tox
-  | \.venv
-  | \venv
-  | _build
-  | buck-out
-  | build
-  | dist
-  | setup.py
-)/
-'''
-
 [tool.mypy]
 check_untyped_defs = true
 disallow_untyped_defs = true
 
 [[tool.mypy.overrides]]
 module = ["tests.*"]
 disallow_untyped_defs = false
@@ -77,11 +55,28 @@
 asyncio_mode = "auto"
 
 [tool.coverage.report]
 exclude_lines = ["if __name__ == .__main__.:", "pragma: no cover"]
 
 [tool.ruff]
 select = ["E", "F", "UP", "I001", "T201", "T203"]
-ignore = ["E501"]
+ignore=[
+  # Recommened ignores by ruff when using formatter
+  "E501",
+  "W191",
+  "E111",
+  "E114",
+  "E117",
+  "D206",
+  "D300",
+  "Q000",
+  "Q001",
+  "Q002",
+  "Q003",
+  "COM812",
+  "COM819",
+  "ISC001",
+  "ISC002",
+]
 line-length = 100
 target-version = "py38"
 fix = true
```

### Comparing `weather_command-6.1.4/weather_command/_builder.py` & `weather_command-6.1.5/weather_command/_builder.py`

 * *Files identical despite different names*

### Comparing `weather_command-6.1.4/weather_command/_cache.py` & `weather_command-6.1.5/weather_command/_cache.py`

 * *Files identical despite different names*

### Comparing `weather_command-6.1.4/weather_command/_config.py` & `weather_command-6.1.5/weather_command/_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import yaml
 from rich.console import Console
 from rich.theme import Theme
 
 from weather_command.errors import MissingApiKey
 
-WEATHER_BASE_URL = "https://api.openweathermap.org/data/2.5"
+WEATHER_BASE_URL = "https://api.openweathermap.org/data/3.0"
 LOCATION_BASE_URL = "https://nominatim.openstreetmap.org/search?format=json&limit=1"
 
 custom_style = Theme({"error": "red", "date": "green"})
 console = Console(theme=custom_style)
 
 
 @lru_cache(maxsize=16)
```

### Comparing `weather_command-6.1.4/weather_command/_location.py` & `weather_command-6.1.5/weather_command/_location.py`

 * *Files identical despite different names*

### Comparing `weather_command-6.1.4/weather_command/_weather.py` & `weather_command-6.1.5/weather_command/_weather.py`

 * *Files identical despite different names*

### Comparing `weather_command-6.1.4/weather_command/main.py` & `weather_command-6.1.5/weather_command/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from weather_command._builder import show_current, show_daily, show_hourly
 from weather_command._cache import Cache
 from weather_command._config import console, load_settings
 from weather_command._location import build_location_url, get_location_details
 from weather_command._utils import build_weather_url
 from weather_command._weather import get_current_weather, get_one_call_weather
 
-__version__ = "6.1.4"
+__version__ = "6.1.5"
 
 app = Typer()
 app.add_typer(settings_commands.app, name="settings", help="Manage saved settings.")
 
 
 class ForecastType(str, Enum):
     CURRENT = "current"
```

### Comparing `weather_command-6.1.4/weather_command/models/weather.py` & `weather_command-6.1.5/weather_command/models/weather.py`

 * *Files identical despite different names*

### Comparing `weather_command-6.1.4/weather_command/settings_commands.py` & `weather_command-6.1.5/weather_command/settings_commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 @app.command()
 def api_key(
     api_key: Union[str, None] = Option(
         None,
         prompt=True,
         hide_input=True,
         help="OpenWeather API key",
-    )
+    ),
 ) -> None:
     """Save the OpenWeather API key. Can also be set by using the OPEN_WEATHER_API_KEY environment variable."""
     settings = load_settings()
     settings.api_key_file = api_key
     settings.save()
     console.print("API key successfully saved", style="green")
 
@@ -69,15 +69,15 @@
     settings.temp_only = temp_only
     settings.save()
     console.print("Temp only preference successfully saved", style="green")
 
 
 @app.command()
 def time_format(
-    time_format: TimeFormat = Option(..., prompt=True, help="Preferred time format")
+    time_format: TimeFormat = Option(..., prompt=True, help="Preferred time format"),
 ) -> None:
     """Save the preferred time format."""
     settings = load_settings()
     am_pm = time_format == TimeFormat.AMPM
     settings.am_pm = am_pm
     settings.save()
     console.print("Units preference successfully saved", style="green")
```

### Comparing `weather_command-6.1.4/PKG-INFO` & `weather_command-6.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: weather-command
-Version: 6.1.4
+Version: 6.1.5
 Summary: Command line weather app
 Home-page: https://github.com/sanders41/weather-command
 License: MIT
 Keywords: weather,cli
 Author: Paul Sanders
 Author-email: psanders1@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: camel-converter[pydantic] (==3.0.2)
-Requires-Dist: httpx (==0.25.0)
-Requires-Dist: pydantic (==2.4.2)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: camel-converter[pydantic] (==3.1.1)
+Requires-Dist: httpx (==0.27.0)
+Requires-Dist: pydantic (==2.7.0)
 Requires-Dist: pyyaml (==6.0.1)
-Requires-Dist: rich (==13.5.3)
+Requires-Dist: rich (==13.7.1)
 Requires-Dist: tenacity (==8.2.3)
-Requires-Dist: typer (==0.9.0)
+Requires-Dist: typer (==0.12.3)
 Project-URL: Documentation, https://github.com/sanders41/weather-command
 Project-URL: Repository, https://github.com/sanders41/weather-command
 Description-Content-Type: text/markdown
 
 # Weather Command
 
 [![Tests Status](https://github.com/sanders41/weather-command/workflows/Testing/badge.svg?branch=main&event=push)](https://github.com/sanders41/weather-command/actions?query=workflow%3ATesting+branch%3Amain+event%3Apush)
```

