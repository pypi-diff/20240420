# Comparing `tmp/ds18b20_datalogger-0.0.2.tar.gz` & `tmp/ds18b20_datalogger-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ds18b20_datalogger-0.0.2.tar", last modified: Sun Apr 14 22:48:41 2024, max compression
+gzip compressed data, was "ds18b20_datalogger-0.0.3.tar", last modified: Fri Apr 19 23:52:51 2024, max compression
```

## Comparing `ds18b20_datalogger-0.0.2.tar` & `ds18b20_datalogger-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,28 @@
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-14 22:48:41.916338 ds18b20_datalogger-0.0.2/
--rw-r--r--   0 amo        (501) staff       (20)      177 2024-04-14 22:48:04.000000 ds18b20_datalogger-0.0.2/CHANGES.md
--rw-r--r--   0 amo        (501) staff       (20)    32473 2024-04-14 22:30:08.000000 ds18b20_datalogger-0.0.2/LICENSE
--rw-r--r--   0 amo        (501) staff       (20)      102 2024-04-14 22:30:08.000000 ds18b20_datalogger-0.0.2/MANIFEST.in
--rw-r--r--   0 amo        (501) staff       (20)    44833 2024-04-14 22:48:41.915837 ds18b20_datalogger-0.0.2/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)     5369 2024-04-14 22:47:03.000000 ds18b20_datalogger-0.0.2/README.md
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-14 22:48:41.907057 ds18b20_datalogger-0.0.2/docs/
--rw-r--r--   0 amo        (501) staff       (20)      214 2024-04-14 22:45:38.000000 ds18b20_datalogger-0.0.2/docs/backlog.md
--rw-r--r--   0 amo        (501) staff       (20)      357 2024-04-14 22:30:08.000000 ds18b20_datalogger-0.0.2/docs/sandbox.md
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-14 22:48:41.909598 ds18b20_datalogger-0.0.2/ds18b20_datalogger/
--rw-r--r--   0 amo        (501) staff       (20)        0 2024-04-14 22:30:08.000000 ds18b20_datalogger-0.0.2/ds18b20_datalogger/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)      299 2024-04-14 22:30:08.000000 ds18b20_datalogger-0.0.2/ds18b20_datalogger/cli.py
--rwxr-xr-x   0 amo        (501) staff       (20)     9180 2024-04-14 22:45:38.000000 ds18b20_datalogger-0.0.2/ds18b20_datalogger/core.py
--rw-r--r--   0 amo        (501) staff       (20)   144953 2024-04-14 22:45:38.000000 ds18b20_datalogger-0.0.2/ds18b20_datalogger/grafana-dashboard.json
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-14 22:48:41.913596 ds18b20_datalogger-0.0.2/ds18b20_datalogger.egg-info/
--rw-r--r--   0 amo        (501) staff       (20)    44833 2024-04-14 22:48:41.000000 ds18b20_datalogger-0.0.2/ds18b20_datalogger.egg-info/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)      467 2024-04-14 22:48:41.000000 ds18b20_datalogger-0.0.2/ds18b20_datalogger.egg-info/SOURCES.txt
--rw-r--r--   0 amo        (501) staff       (20)        1 2024-04-14 22:48:41.000000 ds18b20_datalogger-0.0.2/ds18b20_datalogger.egg-info/dependency_links.txt
--rw-r--r--   0 amo        (501) staff       (20)       67 2024-04-14 22:48:41.000000 ds18b20_datalogger-0.0.2/ds18b20_datalogger.egg-info/entry_points.txt
--rw-r--r--   0 amo        (501) staff       (20)      182 2024-04-14 22:48:41.000000 ds18b20_datalogger-0.0.2/ds18b20_datalogger.egg-info/requires.txt
--rw-r--r--   0 amo        (501) staff       (20)       19 2024-04-14 22:48:41.000000 ds18b20_datalogger-0.0.2/ds18b20_datalogger.egg-info/top_level.txt
--rw-r--r--   0 amo        (501) staff       (20)     4358 2024-04-14 22:30:08.000000 ds18b20_datalogger-0.0.2/pyproject.toml
--rw-r--r--   0 amo        (501) staff       (20)       38 2024-04-14 22:48:41.916436 ds18b20_datalogger-0.0.2/setup.cfg
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-19 23:52:51.456175 ds18b20_datalogger-0.0.3/
+-rw-r--r--   0 amo        (501) staff       (20)      711 2024-04-19 23:52:12.000000 ds18b20_datalogger-0.0.3/CHANGES.md
+-rw-r--r--   0 amo        (501) staff       (20)    32473 2024-04-14 22:30:08.000000 ds18b20_datalogger-0.0.3/LICENSE
+-rw-r--r--   0 amo        (501) staff       (20)      109 2024-04-19 23:50:25.000000 ds18b20_datalogger-0.0.3/MANIFEST.in
+-rw-r--r--   0 amo        (501) staff       (20)    46382 2024-04-19 23:52:51.455581 ds18b20_datalogger-0.0.3/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)     6792 2024-04-19 23:50:25.000000 ds18b20_datalogger-0.0.3/README.md
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-19 23:52:51.427332 ds18b20_datalogger-0.0.3/docs/
+-rw-r--r--   0 amo        (501) staff       (20)      521 2024-04-19 23:51:56.000000 ds18b20_datalogger-0.0.3/docs/backlog.md
+-rw-r--r--   0 amo        (501) staff       (20)      249 2024-04-19 23:50:25.000000 ds18b20_datalogger-0.0.3/docs/mois.md
+-rw-r--r--   0 amo        (501) staff       (20)     2152 2024-04-19 23:50:25.000000 ds18b20_datalogger-0.0.3/docs/production.md
+-rw-r--r--   0 amo        (501) staff       (20)      726 2024-04-19 23:50:25.000000 ds18b20_datalogger-0.0.3/docs/sandbox.md
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-19 23:52:51.447815 ds18b20_datalogger-0.0.3/ds18b20_datalogger/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2024-04-14 22:30:08.000000 ds18b20_datalogger-0.0.3/ds18b20_datalogger/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)     1542 2024-04-19 23:50:25.000000 ds18b20_datalogger-0.0.3/ds18b20_datalogger/cli.py
+-rwxr-xr-x   0 amo        (501) staff       (20)     2313 2024-04-19 23:50:25.000000 ds18b20_datalogger-0.0.3/ds18b20_datalogger/core.py
+-rw-r--r--   0 amo        (501) staff       (20)      877 2024-04-19 23:50:25.000000 ds18b20_datalogger-0.0.3/ds18b20_datalogger/datalogger.yaml
+-rw-r--r--   0 amo        (501) staff       (20)   144953 2024-04-14 22:45:38.000000 ds18b20_datalogger-0.0.3/ds18b20_datalogger/grafana-dashboard.json
+-rw-r--r--   0 amo        (501) staff       (20)     2683 2024-04-19 23:50:25.000000 ds18b20_datalogger-0.0.3/ds18b20_datalogger/model.py
+-rw-r--r--   0 amo        (501) staff       (20)      404 2024-04-19 23:50:25.000000 ds18b20_datalogger-0.0.3/ds18b20_datalogger/util.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-04-19 23:52:51.452915 ds18b20_datalogger-0.0.3/ds18b20_datalogger.egg-info/
+-rw-r--r--   0 amo        (501) staff       (20)    46382 2024-04-19 23:52:51.000000 ds18b20_datalogger-0.0.3/ds18b20_datalogger.egg-info/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)      589 2024-04-19 23:52:51.000000 ds18b20_datalogger-0.0.3/ds18b20_datalogger.egg-info/SOURCES.txt
+-rw-r--r--   0 amo        (501) staff       (20)        1 2024-04-19 23:52:51.000000 ds18b20_datalogger-0.0.3/ds18b20_datalogger.egg-info/dependency_links.txt
+-rw-r--r--   0 amo        (501) staff       (20)       67 2024-04-19 23:52:51.000000 ds18b20_datalogger-0.0.3/ds18b20_datalogger.egg-info/entry_points.txt
+-rw-r--r--   0 amo        (501) staff       (20)      249 2024-04-19 23:52:51.000000 ds18b20_datalogger-0.0.3/ds18b20_datalogger.egg-info/requires.txt
+-rw-r--r--   0 amo        (501) staff       (20)       25 2024-04-19 23:52:51.000000 ds18b20_datalogger-0.0.3/ds18b20_datalogger.egg-info/top_level.txt
+-rw-r--r--   0 amo        (501) staff       (20)     4451 2024-04-19 23:50:25.000000 ds18b20_datalogger-0.0.3/pyproject.toml
+-rw-r--r--   0 amo        (501) staff       (20)       38 2024-04-19 23:52:51.456293 ds18b20_datalogger-0.0.3/setup.cfg
```

### Comparing `ds18b20_datalogger-0.0.2/LICENSE` & `ds18b20_datalogger-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ds18b20_datalogger-0.0.2/PKG-INFO` & `ds18b20_datalogger-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ds18b20-datalogger
-Version: 0.0.2
+Version: 0.0.3
 Summary: A data logger specializing in reading an array of DS18B20 sensors.
 Author-email: The Hiveeyes Developers <hello@hiveeyes.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -643,37 +643,40 @@
 Classifier: Topic :: Education
 Classifier: Topic :: File Formats
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Text Processing
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: importlib-resources; python_version < "3.9"
 Requires-Dist: paho-mqtt<2
+Requires-Dist: pyyaml<7
 Provides-Extra: develop
 Requires-Dist: black<25; extra == "develop"
 Requires-Dist: mypy<1.10; extra == "develop"
 Requires-Dist: poethepoet<0.26; extra == "develop"
 Requires-Dist: pyproject-fmt<1.8; extra == "develop"
 Requires-Dist: ruff<0.4; extra == "develop"
 Requires-Dist: validate-pyproject<0.17; extra == "develop"
 Provides-Extra: docs
 Provides-Extra: release
 Requires-Dist: build<2; extra == "release"
 Requires-Dist: keyring; extra == "release"
 Requires-Dist: twine<6; extra == "release"
 Provides-Extra: test
+Requires-Dist: pyfakefs<6; extra == "test"
 Requires-Dist: pytest<9; extra == "test"
 Requires-Dist: pytest-cov<6; extra == "test"
 
 # ds18b20-datalogger
 
 A data logger specializing in reading an array of DS18B20 sensors.
 
 A temperature sensor matrix with heatmap visualization for bee hive monitoring,
-using Raspberry Pi, Python, DS18B20, MQTT, Kotori DAQ, and Grafana. 
+using Raspberry Pi, Linux, Python, DS18B20, MQTT, Kotori DAQ, and Grafana.
 
 
 | View from outside | View from inside (sensor tip details) |
 |:----:|:----:|
 | ![Außen](https://community.hiveeyes.org/uploads/default/optimized/2X/f/f59f0149306b811f793627ec956c3e43c3758e51_2_334x500.jpeg)  | ![Innen](https://community.hiveeyes.org/uploads/default/optimized/2X/1/10f98dd272bd95940b311e22ef756114bd4efa04_2_333x500.jpeg) |
 
 
@@ -699,94 +702,121 @@
 [![Status][badge-status]][project-pypi]
 [![Package version][badge-package-version]][project-pypi]
 
 
 ## What's Inside
 
 - The `ds18b20-datalogger` program, reading DS18B20 sensors and
-  publishing readings to MQTT.
-- JSON representation for a corresponding [Grafana Dashboard],
-  when acquired through [Kotori DAQ].
+  publishing readings to MQTT in JSON format.
+- Configuration file in YAML format, like [`datalogger.yaml`].
+- JSON representation for a corresponding Grafana Dashboard
+  [`grafana-dashboard.json`], when measurement data is submitted
+  and acquired through [Kotori DAQ].
 
 
-## Setup
-We recommend to install the program into a Python virtualenv.
+## Synopsis
+Acquire single reading, and echo it on STDOUT in JSON format.
 ```shell
-python3 -m venv .venv
-source .venv/bin/activate
-pip install 'ds18b20-datalogger @ git+https://github.com/hiveeyes/ds18b20-datalogger.git'
+ds18b20-datalogger read datalogger.yaml
 ```
 
-In this spirit, you keep the installation separate from your system Python, so
-you can easily nuke it and start from scratch in case anything goes south.
+Take a single reading, and publish it to the configured MQTT topic.
+```shell
+ds18b20-datalogger run datalogger.yaml
+```
+
+## Live
+In order to see a running system in action, please enjoy inspecting the
+[Live Grafana Dashboard].
+
+
+## Installation
+Install the `ds18b20-datalogger` package from PyPI using `pip`.
+```shell
+pip install --upgrade ds18b20-datalogger
+```
+See also alternative installation methods and hands-on walkthroughs at
+[development sandbox] and [production setup].
 
-Prerequisites: This program needs the `paho-mqtt` package.
-https://pypi.org/project/paho-mqtt/#installation
+## Configuration
+In order to operate the data logger successfully, you will need to configure
+two important details:
 
+- Sensors: Map one-wire sensor sysfs paths to self-assigned sensor names.
+- Telemetry: Adjust MQTT connection settings and MQTT topic.
 
-## Operations
+You can create a blueprint configuration file by using the `make-config`
+subcommand.
+```shell
+ds18b20-datalogger make-config > datalogger.yaml
+```
+
+### Appliance: Sensor Wiring and Sensor Mapping
 
-### Sensor Wiring
 Be aware that you might have to adjust your resistors size.
 With 30 sensors i had erratic sensor mapping using a 4.7k resistor.
 I am getting valid mapping using a 2.2k resistor.
 
-### Sensor Mapping
-https://community.hiveeyes.org/t/ds18b20-temperatur-sensoren-am-one-wire-bus-anordnen/1399
+Please read more about [sensor mapping] on our community forum. In practice,
+just edit the `one-wire` section within the configuration file according to
+your setup.
+
+### Backend: Telemetry and Visualization
+
+The data logger will publish measurements to an MQTT topic, where [Kotori DAQ]
+can pick it up, in order to converge into a timeseries database, and displays
+it on a Grafana Dashboard.
+
+The package includes a corresponding Grafana Dashboard, which can be created
+by invoking the `make-dashboard` subcommand.
 
-### Data Publishing
 ```shell
-ssh youruser@yourpi
-screen
-source /path/to/ds18b20-datalogger/.venv/bin/activate
-ds18b20-datalogger
+ds18b20-datalogger make-dashboard > dashboard.json
 ```
 
-### MQTT data upload to Hiveeyes
-https://community.hiveeyes.org/t/daten-per-mqtt-und-python-ans-backend-auf-swarm-hiveeyes-org-ubertragen/94/6
+On our community forum, you can find relevant discussions about this topic.
 
-### Format your array
-https://community.hiveeyes.org/t/how-to-visualize-2-dimensional-temperature-data-in-grafana/974/9
-```python
-matrix = [[temp_ir_1_1, temp_ir_1_2, temp_ir_1_3, temp_ir_1_4, temp_ir_1_5, temp_ir_1_6],
-          [temp_ir_2_1, temp_ir_2_2, temp_ir_2_3, temp_ir_2_4, temp_ir_2_5, temp_ir_2_6],
-          [temp_ir_3_1, temp_ir_3_2, temp_ir_3_3, temp_ir_3_4, temp_ir_3_5, temp_ir_3_6],
-          [temp_ir_4_1, temp_ir_4_2, temp_ir_4_3, temp_ir_4_4, temp_ir_4_5, temp_ir_4_6],
-          [temp_ir_5_1, temp_ir_5_2, temp_ir_5_3, temp_ir_5_4, temp_ir_5_5, temp_ir_5_6]]
-```
+- [MQTT data upload to Hiveeyes]
+- [Data visualization in Grafana]
+- [Sensor offsets] (optional)
 
-### Data visualization in Grafana
-https://swarm.hiveeyes.org/grafana/d/Y9PcgE4Sz/mois-ex-wtf-test-ir-sensor-svg-pixmap-copy
 
-### Bonus: Sensor offsets
-https://community.hiveeyes.org/t/temperatursensoren-justieren-kalibrieren/1744/2
+## Acknowledgements
 
-### Cron Configuration
-```
-*/5 * * * * cd /path/to/data-directory && /path/to/ds18b20-datalogger/.venv/bin/ds18b20-datalogger
-```
+The original code this implementation has been derived from has been discovered
+on the element14 community forum at [Multiple DS18B20 Temp sensors interfacing
+with Raspberry Pi], shared by [@laluha]. Thanks!
 
 
 ## Contributing
 
 In order to learn how to start hacking on this program, please have a look at the
-documentation about how to install a [development sandbox](./docs/sandbox.md).
+documentation about how to install a [development sandbox].
 
 Contributions of any kind are always welcome and appreciated. Thank you.
 
 
 
-[Grafana Dashboard]: https://swarm.hiveeyes.org/grafana/d/T49wHSaIk/mois-ex-wtf-test-ds18b20-5x6-temp-matrix-svg-pixmap?orgId=2&from=1712771622514&to=1712807415379
+[@laluha]: https://github.com/laluha
+[`datalogger.yaml`]: https://github.com/hiveeyes/ds18b20-datalogger/raw/main/ds18b20_datalogger/datalogger.yaml
+[Data visualization in Grafana]: https://swarm.hiveeyes.org/grafana/d/Y9PcgE4Sz/mois-ex-wtf-test-ir-sensor-svg-pixmap-copy
+[`grafana-dashboard.json`]: https://github.com/hiveeyes/ds18b20-datalogger/raw/main/ds18b20_datalogger/grafana-dashboard.json
 [Kotori DAQ]: https://kotori.readthedocs.io
+[Live Grafana Dashboard]: https://swarm.hiveeyes.org/grafana/d/T49wHSaIk/mois-ex-wtf-test-ds18b20-5x6-temp-matrix-svg-pixmap?orgId=2&from=1712771622514&to=1712807415379
+[MQTT data upload to Hiveeyes]: https://community.hiveeyes.org/t/daten-per-mqtt-und-python-ans-backend-auf-swarm-hiveeyes-org-ubertragen/94/6
+[Multiple DS18B20 Temp sensors interfacing with Raspberry Pi]: https://community.element14.com/products/raspberry-pi/raspberrypi_projects/b/blog/posts/multiple-ds18b20-temp-sensors-interfacing-with-raspberry-pi?CommentId=9470e4e9-b054-4dd3-9a3f-ac9d1fe38087
+[Sensor offsets]: https://community.hiveeyes.org/t/temperatursensoren-justieren-kalibrieren/1744/2
+[sensor mapping]: https://community.hiveeyes.org/t/ds18b20-temperatur-sensoren-am-one-wire-bus-anordnen/1399
 
 [Changelog]: https://github.com/hiveeyes/ds18b20-datalogger/blob/main/CHANGES.md
-[development documentation]: https://ds18b20-datalogger.readthedocs.io/en/latest/sandbox.html
+[development sandbox]: https://github.com/hiveeyes/ds18b20-datalogger/blob/main/docs/sandbox.md
 [Documentation]: https://ds18b20-datalogger.readthedocs.io/
 [Issues]: https://github.com/hiveeyes/ds18b20-datalogger/issues
 [License]: https://github.com/hiveeyes/ds18b20-datalogger/blob/main/LICENSE
+[production setup]: https://github.com/hiveeyes/ds18b20-datalogger/blob/main/docs/production.md
 [PyPI]: https://pypi.org/project/ds18b20-datalogger/
 [Source code]: https://github.com/hiveeyes/ds18b20-datalogger
 
 [badge-coverage]: https://codecov.io/gh/hiveeyes/ds18b20-datalogger/branch/main/graph/badge.svg
 [badge-downloads-per-month]: https://pepy.tech/badge/ds18b20-datalogger/month
 [badge-license]: https://img.shields.io/github/license/hiveeyes/ds18b20-datalogger.svg
 [badge-package-version]: https://img.shields.io/pypi/v/ds18b20-datalogger.svg
```

### Comparing `ds18b20_datalogger-0.0.2/ds18b20_datalogger/grafana-dashboard.json` & `ds18b20_datalogger-0.0.3/ds18b20_datalogger/grafana-dashboard.json`

 * *Files identical despite different names*

### Comparing `ds18b20_datalogger-0.0.2/ds18b20_datalogger.egg-info/PKG-INFO` & `ds18b20_datalogger-0.0.3/ds18b20_datalogger.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ds18b20-datalogger
-Version: 0.0.2
+Version: 0.0.3
 Summary: A data logger specializing in reading an array of DS18B20 sensors.
 Author-email: The Hiveeyes Developers <hello@hiveeyes.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -643,37 +643,40 @@
 Classifier: Topic :: Education
 Classifier: Topic :: File Formats
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Text Processing
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: importlib-resources; python_version < "3.9"
 Requires-Dist: paho-mqtt<2
+Requires-Dist: pyyaml<7
 Provides-Extra: develop
 Requires-Dist: black<25; extra == "develop"
 Requires-Dist: mypy<1.10; extra == "develop"
 Requires-Dist: poethepoet<0.26; extra == "develop"
 Requires-Dist: pyproject-fmt<1.8; extra == "develop"
 Requires-Dist: ruff<0.4; extra == "develop"
 Requires-Dist: validate-pyproject<0.17; extra == "develop"
 Provides-Extra: docs
 Provides-Extra: release
 Requires-Dist: build<2; extra == "release"
 Requires-Dist: keyring; extra == "release"
 Requires-Dist: twine<6; extra == "release"
 Provides-Extra: test
+Requires-Dist: pyfakefs<6; extra == "test"
 Requires-Dist: pytest<9; extra == "test"
 Requires-Dist: pytest-cov<6; extra == "test"
 
 # ds18b20-datalogger
 
 A data logger specializing in reading an array of DS18B20 sensors.
 
 A temperature sensor matrix with heatmap visualization for bee hive monitoring,
-using Raspberry Pi, Python, DS18B20, MQTT, Kotori DAQ, and Grafana. 
+using Raspberry Pi, Linux, Python, DS18B20, MQTT, Kotori DAQ, and Grafana.
 
 
 | View from outside | View from inside (sensor tip details) |
 |:----:|:----:|
 | ![Außen](https://community.hiveeyes.org/uploads/default/optimized/2X/f/f59f0149306b811f793627ec956c3e43c3758e51_2_334x500.jpeg)  | ![Innen](https://community.hiveeyes.org/uploads/default/optimized/2X/1/10f98dd272bd95940b311e22ef756114bd4efa04_2_333x500.jpeg) |
 
 
@@ -699,94 +702,121 @@
 [![Status][badge-status]][project-pypi]
 [![Package version][badge-package-version]][project-pypi]
 
 
 ## What's Inside
 
 - The `ds18b20-datalogger` program, reading DS18B20 sensors and
-  publishing readings to MQTT.
-- JSON representation for a corresponding [Grafana Dashboard],
-  when acquired through [Kotori DAQ].
+  publishing readings to MQTT in JSON format.
+- Configuration file in YAML format, like [`datalogger.yaml`].
+- JSON representation for a corresponding Grafana Dashboard
+  [`grafana-dashboard.json`], when measurement data is submitted
+  and acquired through [Kotori DAQ].
 
 
-## Setup
-We recommend to install the program into a Python virtualenv.
+## Synopsis
+Acquire single reading, and echo it on STDOUT in JSON format.
 ```shell
-python3 -m venv .venv
-source .venv/bin/activate
-pip install 'ds18b20-datalogger @ git+https://github.com/hiveeyes/ds18b20-datalogger.git'
+ds18b20-datalogger read datalogger.yaml
 ```
 
-In this spirit, you keep the installation separate from your system Python, so
-you can easily nuke it and start from scratch in case anything goes south.
+Take a single reading, and publish it to the configured MQTT topic.
+```shell
+ds18b20-datalogger run datalogger.yaml
+```
+
+## Live
+In order to see a running system in action, please enjoy inspecting the
+[Live Grafana Dashboard].
+
+
+## Installation
+Install the `ds18b20-datalogger` package from PyPI using `pip`.
+```shell
+pip install --upgrade ds18b20-datalogger
+```
+See also alternative installation methods and hands-on walkthroughs at
+[development sandbox] and [production setup].
 
-Prerequisites: This program needs the `paho-mqtt` package.
-https://pypi.org/project/paho-mqtt/#installation
+## Configuration
+In order to operate the data logger successfully, you will need to configure
+two important details:
 
+- Sensors: Map one-wire sensor sysfs paths to self-assigned sensor names.
+- Telemetry: Adjust MQTT connection settings and MQTT topic.
 
-## Operations
+You can create a blueprint configuration file by using the `make-config`
+subcommand.
+```shell
+ds18b20-datalogger make-config > datalogger.yaml
+```
+
+### Appliance: Sensor Wiring and Sensor Mapping
 
-### Sensor Wiring
 Be aware that you might have to adjust your resistors size.
 With 30 sensors i had erratic sensor mapping using a 4.7k resistor.
 I am getting valid mapping using a 2.2k resistor.
 
-### Sensor Mapping
-https://community.hiveeyes.org/t/ds18b20-temperatur-sensoren-am-one-wire-bus-anordnen/1399
+Please read more about [sensor mapping] on our community forum. In practice,
+just edit the `one-wire` section within the configuration file according to
+your setup.
+
+### Backend: Telemetry and Visualization
+
+The data logger will publish measurements to an MQTT topic, where [Kotori DAQ]
+can pick it up, in order to converge into a timeseries database, and displays
+it on a Grafana Dashboard.
+
+The package includes a corresponding Grafana Dashboard, which can be created
+by invoking the `make-dashboard` subcommand.
 
-### Data Publishing
 ```shell
-ssh youruser@yourpi
-screen
-source /path/to/ds18b20-datalogger/.venv/bin/activate
-ds18b20-datalogger
+ds18b20-datalogger make-dashboard > dashboard.json
 ```
 
-### MQTT data upload to Hiveeyes
-https://community.hiveeyes.org/t/daten-per-mqtt-und-python-ans-backend-auf-swarm-hiveeyes-org-ubertragen/94/6
+On our community forum, you can find relevant discussions about this topic.
 
-### Format your array
-https://community.hiveeyes.org/t/how-to-visualize-2-dimensional-temperature-data-in-grafana/974/9
-```python
-matrix = [[temp_ir_1_1, temp_ir_1_2, temp_ir_1_3, temp_ir_1_4, temp_ir_1_5, temp_ir_1_6],
-          [temp_ir_2_1, temp_ir_2_2, temp_ir_2_3, temp_ir_2_4, temp_ir_2_5, temp_ir_2_6],
-          [temp_ir_3_1, temp_ir_3_2, temp_ir_3_3, temp_ir_3_4, temp_ir_3_5, temp_ir_3_6],
-          [temp_ir_4_1, temp_ir_4_2, temp_ir_4_3, temp_ir_4_4, temp_ir_4_5, temp_ir_4_6],
-          [temp_ir_5_1, temp_ir_5_2, temp_ir_5_3, temp_ir_5_4, temp_ir_5_5, temp_ir_5_6]]
-```
+- [MQTT data upload to Hiveeyes]
+- [Data visualization in Grafana]
+- [Sensor offsets] (optional)
 
-### Data visualization in Grafana
-https://swarm.hiveeyes.org/grafana/d/Y9PcgE4Sz/mois-ex-wtf-test-ir-sensor-svg-pixmap-copy
 
-### Bonus: Sensor offsets
-https://community.hiveeyes.org/t/temperatursensoren-justieren-kalibrieren/1744/2
+## Acknowledgements
 
-### Cron Configuration
-```
-*/5 * * * * cd /path/to/data-directory && /path/to/ds18b20-datalogger/.venv/bin/ds18b20-datalogger
-```
+The original code this implementation has been derived from has been discovered
+on the element14 community forum at [Multiple DS18B20 Temp sensors interfacing
+with Raspberry Pi], shared by [@laluha]. Thanks!
 
 
 ## Contributing
 
 In order to learn how to start hacking on this program, please have a look at the
-documentation about how to install a [development sandbox](./docs/sandbox.md).
+documentation about how to install a [development sandbox].
 
 Contributions of any kind are always welcome and appreciated. Thank you.
 
 
 
-[Grafana Dashboard]: https://swarm.hiveeyes.org/grafana/d/T49wHSaIk/mois-ex-wtf-test-ds18b20-5x6-temp-matrix-svg-pixmap?orgId=2&from=1712771622514&to=1712807415379
+[@laluha]: https://github.com/laluha
+[`datalogger.yaml`]: https://github.com/hiveeyes/ds18b20-datalogger/raw/main/ds18b20_datalogger/datalogger.yaml
+[Data visualization in Grafana]: https://swarm.hiveeyes.org/grafana/d/Y9PcgE4Sz/mois-ex-wtf-test-ir-sensor-svg-pixmap-copy
+[`grafana-dashboard.json`]: https://github.com/hiveeyes/ds18b20-datalogger/raw/main/ds18b20_datalogger/grafana-dashboard.json
 [Kotori DAQ]: https://kotori.readthedocs.io
+[Live Grafana Dashboard]: https://swarm.hiveeyes.org/grafana/d/T49wHSaIk/mois-ex-wtf-test-ds18b20-5x6-temp-matrix-svg-pixmap?orgId=2&from=1712771622514&to=1712807415379
+[MQTT data upload to Hiveeyes]: https://community.hiveeyes.org/t/daten-per-mqtt-und-python-ans-backend-auf-swarm-hiveeyes-org-ubertragen/94/6
+[Multiple DS18B20 Temp sensors interfacing with Raspberry Pi]: https://community.element14.com/products/raspberry-pi/raspberrypi_projects/b/blog/posts/multiple-ds18b20-temp-sensors-interfacing-with-raspberry-pi?CommentId=9470e4e9-b054-4dd3-9a3f-ac9d1fe38087
+[Sensor offsets]: https://community.hiveeyes.org/t/temperatursensoren-justieren-kalibrieren/1744/2
+[sensor mapping]: https://community.hiveeyes.org/t/ds18b20-temperatur-sensoren-am-one-wire-bus-anordnen/1399
 
 [Changelog]: https://github.com/hiveeyes/ds18b20-datalogger/blob/main/CHANGES.md
-[development documentation]: https://ds18b20-datalogger.readthedocs.io/en/latest/sandbox.html
+[development sandbox]: https://github.com/hiveeyes/ds18b20-datalogger/blob/main/docs/sandbox.md
 [Documentation]: https://ds18b20-datalogger.readthedocs.io/
 [Issues]: https://github.com/hiveeyes/ds18b20-datalogger/issues
 [License]: https://github.com/hiveeyes/ds18b20-datalogger/blob/main/LICENSE
+[production setup]: https://github.com/hiveeyes/ds18b20-datalogger/blob/main/docs/production.md
 [PyPI]: https://pypi.org/project/ds18b20-datalogger/
 [Source code]: https://github.com/hiveeyes/ds18b20-datalogger
 
 [badge-coverage]: https://codecov.io/gh/hiveeyes/ds18b20-datalogger/branch/main/graph/badge.svg
 [badge-downloads-per-month]: https://pepy.tech/badge/ds18b20-datalogger/month
 [badge-license]: https://img.shields.io/github/license/hiveeyes/ds18b20-datalogger.svg
 [badge-package-version]: https://img.shields.io/pypi/v/ds18b20-datalogger.svg
```

### Comparing `ds18b20_datalogger-0.0.2/pyproject.toml` & `ds18b20_datalogger-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,17 @@
   "Topic :: Scientific/Engineering",
   "Topic :: Text Processing",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
+  "importlib-resources; python_version<'3.9'",
   "paho-mqtt<2",
+  "pyyaml<7",
 ]
 [project.optional-dependencies]
 develop = [
   "black<25",
   "mypy<1.10",
   "poethepoet<0.26",
   "pyproject-fmt<1.8",
@@ -63,14 +65,15 @@
 ]
 release = [
   "build<2",
   "keyring",
   "twine<6",
 ]
 test = [
+  "pyfakefs<6",
   "pytest<9",
   "pytest-cov<6",
 ]
 [project.urls]
 changelog = "https://github.com/hiveeyes/ds18b20-datalogger/blob/main/CHANGES.md"
 documentation = "https://ds18b20-datalogger.readthedocs.io/"
 homepage = "https://ds18b20-datalogger.readthedocs.io/"
@@ -89,15 +92,18 @@
 source = ["ds18b20_datalogger"]
 
 [tool.coverage.report]
 fail_under = 0
 show_missing = true
 
 [tool.mypy]
-packages = ["ds18b20_datalogger"]
+packages = [
+  "ds18b20_datalogger",
+  "tests",
+]
 exclude = [
 ]
 check_untyped_defs = true
 implicit_optional = true
 install_types = true
 no_implicit_optional = true
 non_interactive = true
```

