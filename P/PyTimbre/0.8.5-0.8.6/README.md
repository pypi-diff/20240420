# Comparing `tmp/pytimbre-0.8.5.tar.gz` & `tmp/pytimbre-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytimbre-0.8.5.tar", last modified: Fri Mar 15 18:54:38 2024, max compression
+gzip compressed data, was "pytimbre-0.8.6.tar", last modified: Thu Apr 18 18:48:20 2024, max compression
```

## Comparing `pytimbre-0.8.5.tar` & `pytimbre-0.8.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1106 2023-02-28 16:15:07.326899 pytimbre-0.8.5/LICENSE.txt
--rw-r--r--   0        0        0     6248 2023-08-27 21:56:46.707791 pytimbre-0.8.5/README.md
--rw-r--r--   0        0        0      853 2024-03-15 18:54:38.832295 pytimbre-0.8.5/pyproject.toml
--rw-r--r--   0        0        0       75 2023-04-13 00:23:16.156081 pytimbre-0.8.5/src/pytimbre/__init__.py
--rw-r--r--   0        0        0      108 2023-04-04 13:59:30.719773 pytimbre-0.8.5/src/pytimbre/audio_files/__init__.py
--rw-r--r--   0        0        0    24251 2023-06-26 00:38:01.172575 pytimbre-0.8.5/src/pytimbre/audio_files/ansi_standard_formatted_files.py
--rw-r--r--   0        0        0    15392 2023-04-14 23:28:06.150571 pytimbre-0.8.5/src/pytimbre/audio_files/calibrated_binary_files.py
--rw-r--r--   0        0        0    78477 2024-03-15 18:53:05.756568 pytimbre-0.8.5/src/pytimbre/audio_files/wavefile.py
--rw-r--r--   0        0        0     1711 2023-08-19 12:27:51.367618 pytimbre-0.8.5/src/pytimbre/audio_files/wavefile_structure.md
--rw-r--r--   0        0        0      123 2023-08-20 17:11:36.679376 pytimbre-0.8.5/src/pytimbre/spectral/__init__.py
--rw-r--r--   0        0        0    18327 2023-08-26 14:29:31.077914 pytimbre-0.8.5/src/pytimbre/spectral/acoustic_weights.py
--rw-r--r--   0        0        0    30285 2023-11-04 18:58:46.586298 pytimbre-0.8.5/src/pytimbre/spectral/fractional_octave_band.py
--rw-r--r--   0        0        0    16861 2023-08-27 21:56:46.709788 pytimbre-0.8.5/src/pytimbre/spectral/fundamental_frequency.py
--rw-r--r--   0        0        0    62219 2023-09-01 20:18:53.607021 pytimbre-0.8.5/src/pytimbre/spectral/spectra.py
--rw-r--r--   0        0        0    13865 2023-04-13 17:16:30.787476 pytimbre-0.8.5/src/pytimbre/spectral/swipe.py
--rw-r--r--   0        0        0        0 2023-08-20 17:11:36.683376 pytimbre-0.8.5/src/pytimbre/spectral/timbral_model/__init__.py
--rw-r--r--   0        0        0    48539 2023-08-27 22:01:28.080294 pytimbre-0.8.5/src/pytimbre/spectral/timbral_model/timbral_models.py
--rw-r--r--   0        0        0    71115 2023-08-26 14:29:31.080431 pytimbre-0.8.5/src/pytimbre/spectral/timbral_model/timbral_util.py
--rw-r--r--   0        0        0    38381 2024-02-15 23:11:07.368810 pytimbre-0.8.5/src/pytimbre/spectral/time_histories.py
--rw-r--r--   0        0        0        0 2023-08-19 12:27:51.368619 pytimbre-0.8.5/src/pytimbre/temporal/__init__.py
--rw-r--r--   0        0        0    19270 2023-08-26 14:29:31.081431 pytimbre-0.8.5/src/pytimbre/temporal/temporal_metrics.py
--rw-r--r--   0        0        0   140826 2024-02-15 22:14:06.045421 pytimbre-0.8.5/src/pytimbre/waveform.py
--rw-r--r--   0        0        0     7703 2023-04-13 01:31:15.026419 pytimbre-0.8.5/src/pytimbre/yin.py
--rw-r--r--   0        0        0     6756 1970-01-01 00:00:00.000000 pytimbre-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0     1106 2023-02-28 16:15:07.326899 pytimbre-0.8.6/LICENSE.txt
+-rw-r--r--   0        0        0     6248 2023-08-27 21:56:46.707791 pytimbre-0.8.6/README.md
+-rw-r--r--   0        0        0      873 2024-04-18 18:48:20.921915 pytimbre-0.8.6/pyproject.toml
+-rw-r--r--   0        0        0       75 2023-04-13 00:23:16.156081 pytimbre-0.8.6/src/pytimbre/__init__.py
+-rw-r--r--   0        0        0      108 2023-04-04 13:59:30.719773 pytimbre-0.8.6/src/pytimbre/audio_files/__init__.py
+-rw-r--r--   0        0        0    24251 2023-06-26 00:38:01.172575 pytimbre-0.8.6/src/pytimbre/audio_files/ansi_standard_formatted_files.py
+-rw-r--r--   0        0        0    15392 2023-04-14 23:28:06.150571 pytimbre-0.8.6/src/pytimbre/audio_files/calibrated_binary_files.py
+-rw-r--r--   0        0        0    83806 2024-04-18 18:48:08.033857 pytimbre-0.8.6/src/pytimbre/audio_files/wavefile.py
+-rw-r--r--   0        0        0     1711 2023-08-19 12:27:51.367618 pytimbre-0.8.6/src/pytimbre/audio_files/wavefile_structure.md
+-rw-r--r--   0        0        0      123 2023-08-20 17:11:36.679376 pytimbre-0.8.6/src/pytimbre/spectral/__init__.py
+-rw-r--r--   0        0        0    18327 2023-08-26 14:29:31.077914 pytimbre-0.8.6/src/pytimbre/spectral/acoustic_weights.py
+-rw-r--r--   0        0        0    30285 2023-11-04 18:58:46.586298 pytimbre-0.8.6/src/pytimbre/spectral/fractional_octave_band.py
+-rw-r--r--   0        0        0    16861 2023-08-27 21:56:46.709788 pytimbre-0.8.6/src/pytimbre/spectral/fundamental_frequency.py
+-rw-r--r--   0        0        0    62219 2023-09-01 20:18:53.607021 pytimbre-0.8.6/src/pytimbre/spectral/spectra.py
+-rw-r--r--   0        0        0    13865 2023-04-13 17:16:30.787476 pytimbre-0.8.6/src/pytimbre/spectral/swipe.py
+-rw-r--r--   0        0        0        0 2023-08-20 17:11:36.683376 pytimbre-0.8.6/src/pytimbre/spectral/timbral_model/__init__.py
+-rw-r--r--   0        0        0    48539 2023-08-27 22:01:28.080294 pytimbre-0.8.6/src/pytimbre/spectral/timbral_model/timbral_models.py
+-rw-r--r--   0        0        0    71115 2023-08-26 14:29:31.080431 pytimbre-0.8.6/src/pytimbre/spectral/timbral_model/timbral_util.py
+-rw-r--r--   0        0        0    38381 2024-02-15 23:11:07.368810 pytimbre-0.8.6/src/pytimbre/spectral/time_histories.py
+-rw-r--r--   0        0        0        0 2023-08-19 12:27:51.368619 pytimbre-0.8.6/src/pytimbre/temporal/__init__.py
+-rw-r--r--   0        0        0    19270 2023-08-26 14:29:31.081431 pytimbre-0.8.6/src/pytimbre/temporal/temporal_metrics.py
+-rw-r--r--   0        0        0   140826 2024-02-15 22:14:06.045421 pytimbre-0.8.6/src/pytimbre/waveform.py
+-rw-r--r--   0        0        0     7703 2023-04-13 01:31:15.026419 pytimbre-0.8.6/src/pytimbre/yin.py
+-rw-r--r--   0        0        0     6786 1970-01-01 00:00:00.000000 pytimbre-0.8.6/PKG-INFO
```

### Comparing `pytimbre-0.8.5/LICENSE.txt` & `pytimbre-0.8.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytimbre-0.8.5/README.md` & `pytimbre-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `pytimbre-0.8.5/pyproject.toml` & `pytimbre-0.8.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [project]
 name = "PyTimbre"
-version = "0.8.5"
+version = "0.8.6"
 description = "Python conversion of Timbre Toolbox"
 authors = [
     { name = "frankmobley", email = "mobssoft@gmail.com" },
     { name = "Dr. Frank Mobley", email = "frank.mobley.1@afrl.af.mil" },
 ]
 dependencies = [
     "colorednoise>=2.1.0",
     "numpy>=1.21.5",
     "pandas>=1.4.3",
     "python_speech_features~=0.6",
     "scipy>=1.9.1",
     "statsmodels>=0.13.2",
+    "json5>=0.9.0",
 ]
 requires-python = ">=3.9"
 readme = "README.md"
 keywords = [
     "machine learning",
     "feature extraction",
     "MATLAB",
```

### Comparing `pytimbre-0.8.5/src/pytimbre/audio_files/ansi_standard_formatted_files.py` & `pytimbre-0.8.6/src/pytimbre/audio_files/ansi_standard_formatted_files.py`

 * *Files identical despite different names*

### Comparing `pytimbre-0.8.5/src/pytimbre/audio_files/calibrated_binary_files.py` & `pytimbre-0.8.6/src/pytimbre/audio_files/calibrated_binary_files.py`

 * *Files identical despite different names*

### Comparing `pytimbre-0.8.5/src/pytimbre/audio_files/wavefile.py` & `pytimbre-0.8.6/src/pytimbre/audio_files/wavefile.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os, os.path
 from io import FileIO
+import dateutil.parser
 import numpy as np
 from datetime import datetime, timedelta
 from ..waveform import Waveform
 import struct
 import scipy.signal
 import warnings
 
@@ -648,14 +649,16 @@
         :param offset: int - the offset of the chunk's data
         :param name: str - the name of the chunk
 
         https://www.recordingblogs.com/wiki/list-chunk-of-a-wave-file#:~:text=List%20chunk%20%28of%20a%20RIFF%20file
         %29%20%20,%20Depends%20on%20the%20list%20type%20ID%20
         """
 
+        import json
+
         if reader is None:
             #   Create the dictionaries that will be used for the creation of the data
 
             self.time0 = datetime.fromtimestamp(0)
             self.meta_data = {
                 'creation_date': self.time0
             }
@@ -694,37 +697,73 @@
                         data = data[:-1]
                         if len(data) <= 0:
                             break
 
                 offset += 8 + size
 
                 #   Determine what the information represents
-
                 if cmd == "IARL":
                     self.meta_data["archival_location"] = data
                 elif cmd == "IART":
                     self.meta_data["artist"] = data
                 elif cmd == "ICMS":
                     self.meta_data["commissioned_organization"] = data
                 elif cmd == "ICMT":
                     self.meta_data["general_comments"] = data
 
                     # Now we understand that the majority of the header does not actually fall within the
                     # standard LIST elements.  So we created a comma delimited arrangement of header name and
                     # we can now separate apart.
-
                     if len(data) > 0:
                         if "|" in data:
                             sub_elements = data.split("|")
 
                             for header_element in sub_elements:
                                 cmd = header_element.split('=')[0]
                                 data = header_element.split('=')[1]
 
                                 self.header[cmd] = data
+                        if "{" in data and "}" in data:
+                            #   This is likely a JSON formatted string, so we will attempt to use the JSON decoder to
+                            #   actually read the data from the string
+                            self.header[cmd] = json.loads(data)
+                            for key in self.header[cmd].keys():
+                                if key == 'sens_l':
+                                    self.meta_data['left_channel_sensor_sensitivity'] = self.header[cmd][key]
+                                elif key == 'sens_r':
+                                    self.meta_data['right_channel_sensor_sensitivity'] = self.header[cmd][key]
+                                elif key == 'gain_l':
+                                    self.meta_data['left_channel_gain'] = self.header[cmd][key]
+                                elif key == 'gain_r':
+                                    self.meta_data['right_channel_gain'] = self.header[cmd][key]
+                                elif key == 'v_scale':
+                                    self.meta_data['vertical_scale'] = self.header[cmd][key]
+                                elif key == 'gps_lat':
+                                    self.meta_data['latitude'] = self.header[cmd][key]
+                                elif key == 'gps_lon':
+                                    self.meta_data['longitude'] = self.header[cmd][key]
+                                elif key == 'gpx_fix':
+                                    self.meta_data['gps_fix_quality'] = self.header[cmd][key]
+                                elif key == 'gps_sat':
+                                    self.meta_data['gps_satellite_count'] = self.header[cmd][key]
+                                elif key == 'gps_alt':
+                                    self.meta_data['gps_altitude'] = self.header[cmd][key]
+                                elif key == 'gps_spd':
+                                    self.meta_data['gps_ground_speed'] = self.header[cmd][key]
+                                elif key == 'gps_trk_ang':
+                                    self.meta_data['gps_track_heading_angle'] = self.header[cmd][key]
+                                elif key == 'gps_hor_dil':
+                                    self.meta_data['gps_horizontal_dilution'] = self.header[cmd][key]
+                                elif key == 'gps_ht_gd':
+                                    self.meta_data['gps_height_above_ground'] = self.header[cmd][key]
+                                elif key == 'gps_ts':
+                                    self.meta_data['gps_time_stamp'] = self.header[cmd][key]
+                                elif key == 'gps_ts_sub':
+                                    self.meta_data['gps_time_stamp'] = self.header[cmd][key]
+                                    self.time0 = dateutil.parser.parse(self.meta_data['gps_time_stamp'])
                 elif cmd == "ICOP":
                     self.meta_data['copyright'] = data
                 elif cmd == "ICRD":
                     self.meta_data['creation_date'] = data
                 elif cmd == "ICRP":
                     self.meta_data['cropping_information'] = data
                 elif cmd == "IDIM":
@@ -1226,19 +1265,23 @@
         :param path: str - the path to the audio file
         :returns: dict
 
         Remarks
         -------
         20230120 - FSM - changed from tuple to dictionary to provide some context for the values within the returned
             object.
+        20240417 - FSM - Updated this function to return values from the RAAS system developed by AFRL for acoustic
+            recordings
         """
 
+        #   Open the file and list the chunks that exist within the object
         scanner = ChunkScanner(path)
 
-        with open(path, 'rb') as file:
+        #   open the path to extract the information from the file without having to read all the contents of the file
+        with (open(path, 'rb') as file):
 
             #   The format chunk is required by all wav files
             format_chunk = FormatChunk(
                 file, scanner.format_chunk.chunk_offset, scanner.format_chunk.chunk_size,
                 scanner.format_chunk.chunk_name
             )
 
@@ -1255,40 +1298,67 @@
             #   If there is a list chunk, read it
 
             if scanner.list_chunk is not None:
                 list_chunk = ListChunk(
                     file, scanner.list_chunk.chunk_size, scanner.list_chunk.chunk_offset,
                     scanner.list_chunk.chunk_name
                 )
-                time0 = list_chunk.time0
+
                 if list_chunk.cropping_information is not None:
                     if list_chunk.cropping_information == "normalized":
                         normalized = True
                     else:
                         normlized = False
                 else:
                     normalized = False
+
+                if list_chunk.file_start_time is not None:
+                    time0 = list_chunk.file_start_time
             else:
                 list_chunk = None
                 time0 = 0
                 normalized = False
 
             samples_per_channel = scanner.data_chunk.chunk_size / ((format_chunk.bits_per_sample / 8) /
                                                                    format_chunk.channel_count)
             duration = samples_per_channel / format_chunk.sample_rate
 
             information = {'sample_rate': format_chunk.sample_rate,
                            "channel_count": format_chunk.channel_count,
                            'byte_size': format_chunk.bits_per_sample / 8,
                            'is_normalized': normalized,
                            'start_time': time0,
-                           'duration': duration,
                            'has_peak_chunk': scanner.peak_chunk is not None,
                            'has_list_chunk': scanner.list_chunk is not None,
-                           'has_xml_chunk': scanner.xml_chunk is not None}
+                           'has_xml_chunk': scanner.xml_chunk is not None,
+                           'data_chunk_size': scanner.data_chunk.chunk_size}
+            if list_chunk is not None:
+                for key in list_chunk.meta_data.keys():
+                    information[key] = list_chunk.meta_data[key]
+
+            if peak_chunk is not None:
+                information['peak_count'] = len(peak_chunk.peak_sample)
+                for i in range(len(peak_chunk.peak_sample)):
+                    information['peak {} sample'.format(i)] = peak_chunk.peak_sample[i]
+                    information['peak {} level'.format(i)] = peak_chunk.peak_amplitude[i]
+                    if list_chunk is not None:
+
+                        information['left_channel_gain (dB)'] = list_chunk.meta_data['left_channel_gain'],
+                        information['right_channel_gain (dB)'] = list_chunk.meta_data['right_channel_gain'],
+                        information['left_channel_sensor_sensitivity'] = list_chunk.meta_data[
+                            'left_channel_sensor_sensitivity'],
+                        information['right_channel_sensor_sensitivity'] = list_chunk.meta_data[
+                            'right_channel_sensor_sensitivity']
+
+                    else:
+                        information['left_channel_gain (dB)'] = None
+                        information['right_channel_gain (dB)'] = None
+                        information['left_channel_sensor_sensitivity'] = None
+                        information['right_channel_sensor_sensitivity'] = None
+                        information['peak {} level'.format(i)] = peak_chunk.peak_amplitude[i]
 
         return information
 
     def _read_format_chunk(self, file):
         """
         To further reduce the cognitive complexity of the functions, this will read the format chunk from the file
 
@@ -1339,14 +1409,17 @@
             if self.list_chunk.cropping_information is not None:
                 if self.list_chunk.cropping_information == "normalized":
                     self.normalized = True
                 else:
                     self.normalized = False
             else:
                 self.normalized = False
+
+            if 'gps_time' in self.list_chunk.meta_data.keys():
+                self.start_time = dateutil.parser.parse(self.list_chunk.meta_data['gps_time'])
         else:
             #   If there is no list chunk in the file, create one so that we can hold the start_time data for the
             #   waveform
             self.list_chunk = ListChunk()
             self.normalized = False
 
     def _read_xml_chunk(self, file):
@@ -1499,15 +1572,16 @@
             #   of the start time now to ensure that it is stored in the list chunk
             self.start_time = t0
 
         self.normalized = False
 
     def __init__(
             self, path=None, s0: int = None, s1: int = None, fs: int = None, samples=None, time=None,
-            get_peak: bool = True):
+            get_peak: bool = True
+    ):
         """
         This constructor reads the chunks from the wave file and then processes those that are canonical.
 
         :param path: str - the full path to the file that we want to read
         :param s0: int - the starting sample for the reading of the audio file
         :param s1: int - the ending sample for the reading of the audio file
         :param fs: int - the number of samples per second.  This facilitates calling the based class with the required
@@ -1892,17 +1966,23 @@
         if 'creation_date' in self.list_chunk.meta_data.keys() and self.list_chunk.meta_data['creation_date'] is not \
                 None:
             if isinstance(self.list_chunk.meta_data['creation_date'], str):
                 if self.list_chunk.meta_data['creation_date'].isdigit():
                     return float(self.list_chunk.meta_data['creation_date'])
                 else:
                     try:
-                        return datetime.strptime(self.list_chunk.meta_data['creation_date'], "%Y-%m-%d %H:%M:%S.%f")
+                        return datetime.strptime(
+                            self.list_chunk.meta_data['creation_date'],
+                            "%Y-%m-%d %H:%M:%S.%f"
+                            )
                     except ValueError:
-                        return datetime.strptime(self.list_chunk.meta_data['creation_date'], "%Y-%m-%d %H:%M:%S")
+                        return datetime.strptime(
+                            self.list_chunk.meta_data['creation_date'],
+                            "%Y-%m-%d %H:%M:%S"
+                            )
             else:
                 return self.list_chunk.meta_data['creation_date']
         else:
             return 0
 
     @start_time.setter
     def start_time(self, value):
@@ -1913,24 +1993,27 @@
         """
         This property creates a set of Waveform objects that represent the individual channels within the audio file.
         """
 
         if self.channel_count > 1:
             array = np.empty((self.channel_count,), dtype=Waveform)
             for i in range(self.channel_count):
-                array[i] = Waveform(pressures=self.samples[:, i],
-                                    sample_rate=self.sample_rate,
-                                    start_time=self.start_time)
+                array[i] = Waveform(
+                    pressures=self.samples[:, i],
+                    sample_rate=self.sample_rate,
+                    start_time=self.start_time
+                    )
 
             return array
         else:
-            return Waveform(pressures=self.samples,
-                                    sample_rate=self.sample_rate,
-                                    start_time=self.start_time)
-
+            return Waveform(
+                pressures=self.samples,
+                sample_rate=self.sample_rate,
+                start_time=self.start_time
+                )
 
     def save(self, path):
         """
         This function will save the data to a canonical wav formatted file with appropriate scaling to recover the
         actual Pascal values.
 
         :param path: str - the output path for the scaled canonical wav format
```

### Comparing `pytimbre-0.8.5/src/pytimbre/audio_files/wavefile_structure.md` & `pytimbre-0.8.6/src/pytimbre/audio_files/wavefile_structure.md`

 * *Files identical despite different names*

### Comparing `pytimbre-0.8.5/src/pytimbre/spectral/acoustic_weights.py` & `pytimbre-0.8.6/src/pytimbre/spectral/acoustic_weights.py`

 * *Files identical despite different names*

### Comparing `pytimbre-0.8.5/src/pytimbre/spectral/fractional_octave_band.py` & `pytimbre-0.8.6/src/pytimbre/spectral/fractional_octave_band.py`

 * *Files identical despite different names*

### Comparing `pytimbre-0.8.5/src/pytimbre/spectral/fundamental_frequency.py` & `pytimbre-0.8.6/src/pytimbre/spectral/fundamental_frequency.py`

 * *Files identical despite different names*

### Comparing `pytimbre-0.8.5/src/pytimbre/spectral/spectra.py` & `pytimbre-0.8.6/src/pytimbre/spectral/spectra.py`

 * *Files identical despite different names*

### Comparing `pytimbre-0.8.5/src/pytimbre/spectral/swipe.py` & `pytimbre-0.8.6/src/pytimbre/spectral/swipe.py`

 * *Files identical despite different names*

### Comparing `pytimbre-0.8.5/src/pytimbre/spectral/timbral_model/timbral_models.py` & `pytimbre-0.8.6/src/pytimbre/spectral/timbral_model/timbral_models.py`

 * *Files identical despite different names*

### Comparing `pytimbre-0.8.5/src/pytimbre/spectral/timbral_model/timbral_util.py` & `pytimbre-0.8.6/src/pytimbre/spectral/timbral_model/timbral_util.py`

 * *Files identical despite different names*

### Comparing `pytimbre-0.8.5/src/pytimbre/spectral/time_histories.py` & `pytimbre-0.8.6/src/pytimbre/spectral/time_histories.py`

 * *Files identical despite different names*

### Comparing `pytimbre-0.8.5/src/pytimbre/temporal/temporal_metrics.py` & `pytimbre-0.8.6/src/pytimbre/temporal/temporal_metrics.py`

 * *Files identical despite different names*

### Comparing `pytimbre-0.8.5/src/pytimbre/waveform.py` & `pytimbre-0.8.6/src/pytimbre/waveform.py`

 * *Files identical despite different names*

### Comparing `pytimbre-0.8.5/src/pytimbre/yin.py` & `pytimbre-0.8.6/src/pytimbre/yin.py`

 * *Files identical despite different names*

### Comparing `pytimbre-0.8.5/PKG-INFO` & `pytimbre-0.8.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: PyTimbre
-Version: 0.8.5
+Version: 0.8.6
 Summary: Python conversion of Timbre Toolbox
-Keywords: machine learning feature extraction MATLAB audio
-Author-Email: frankmobley <mobssoft@gmail.com>, Dr. Frank Mobley <frank.mobley.1@afrl.af.mil>
+Keywords: machine learning,feature extraction,MATLAB,audio
+Author-Email: frankmobley <mobssoft@gmail.com>, "Dr. Frank Mobley" <frank.mobley.1@afrl.af.mil>
 License: MIT
 Project-URL: Homepage, https://gitlab.com/python-audio-feature-extraction/pytimbre
 Requires-Python: >=3.9
 Requires-Dist: colorednoise>=2.1.0
 Requires-Dist: numpy>=1.21.5
 Requires-Dist: pandas>=1.4.3
 Requires-Dist: python_speech_features~=0.6
 Requires-Dist: scipy>=1.9.1
 Requires-Dist: statsmodels>=0.13.2
+Requires-Dist: json5>=0.9.0
 Description-Content-Type: text/markdown
 
 ![PyTimbre Logo](pytimbre_bing_gen_a.png " ") 
 
 # PyTimbre
 __PyTimbre is a Python conversion of the Matlab package Timbre Toolbox, found here:
 (https://github.com/VincentPerreault0/timbretoolbox).__
```

