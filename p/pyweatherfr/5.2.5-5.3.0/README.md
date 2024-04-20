# Comparing `tmp/pyweatherfr-5.2.5.tar.gz` & `tmp/pyweatherfr-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyweatherfr-5.2.5.tar", last modified: Wed Apr 17 10:04:50 2024, max compression
+gzip compressed data, was "pyweatherfr-5.3.0.tar", last modified: Sat Apr 20 16:52:21 2024, max compression
```

## Comparing `pyweatherfr-5.2.5.tar` & `pyweatherfr-5.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:04:50.055160 pyweatherfr-5.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-17 10:03:49.000000 pyweatherfr-5.2.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-17 10:04:50.055160 pyweatherfr-5.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-17 10:03:49.000000 pyweatherfr-5.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-17 10:03:49.000000 pyweatherfr-5.2.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:04:50.051160 pyweatherfr-5.2.5/pyweatherfr/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-17 10:03:49.000000 pyweatherfr-5.2.5/pyweatherfr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-04-17 10:03:49.000000 pyweatherfr-5.2.5/pyweatherfr/args.py
--rw-r--r--   0 runner    (1001) docker     (127)    45035 2024-04-17 10:03:49.000000 pyweatherfr-5.2.5/pyweatherfr/pyweatherfr.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-17 10:03:49.000000 pyweatherfr-5.2.5/pyweatherfr/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:04:50.055160 pyweatherfr-5.2.5/pyweatherfr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-17 10:04:50.000000 pyweatherfr-5.2.5/pyweatherfr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-17 10:04:50.000000 pyweatherfr-5.2.5/pyweatherfr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 10:04:50.000000 pyweatherfr-5.2.5/pyweatherfr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-17 10:04:50.000000 pyweatherfr-5.2.5/pyweatherfr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 10:03:58.000000 pyweatherfr-5.2.5/pyweatherfr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-17 10:04:50.000000 pyweatherfr-5.2.5/pyweatherfr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 10:04:50.000000 pyweatherfr-5.2.5/pyweatherfr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 10:04:50.055160 pyweatherfr-5.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-17 10:03:49.000000 pyweatherfr-5.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:52:21.385417 pyweatherfr-5.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-20 16:51:29.000000 pyweatherfr-5.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-20 16:52:21.381417 pyweatherfr-5.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-20 16:51:29.000000 pyweatherfr-5.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-20 16:51:29.000000 pyweatherfr-5.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:52:21.381417 pyweatherfr-5.3.0/pyweatherfr/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-20 16:51:29.000000 pyweatherfr-5.3.0/pyweatherfr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-20 16:51:29.000000 pyweatherfr-5.3.0/pyweatherfr/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50011 2024-04-20 16:51:29.000000 pyweatherfr-5.3.0/pyweatherfr/pyweatherfr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-20 16:51:29.000000 pyweatherfr-5.3.0/pyweatherfr/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 16:52:21.381417 pyweatherfr-5.3.0/pyweatherfr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-20 16:52:21.000000 pyweatherfr-5.3.0/pyweatherfr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-20 16:52:21.000000 pyweatherfr-5.3.0/pyweatherfr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 16:52:21.000000 pyweatherfr-5.3.0/pyweatherfr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-20 16:52:21.000000 pyweatherfr-5.3.0/pyweatherfr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 16:51:34.000000 pyweatherfr-5.3.0/pyweatherfr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-20 16:52:21.000000 pyweatherfr-5.3.0/pyweatherfr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-20 16:52:21.000000 pyweatherfr-5.3.0/pyweatherfr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 16:52:21.385417 pyweatherfr-5.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-20 16:51:29.000000 pyweatherfr-5.3.0/setup.py
```

### Comparing `pyweatherfr-5.2.5/LICENSE.txt` & `pyweatherfr-5.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyweatherfr-5.2.5/PKG-INFO` & `pyweatherfr-5.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 5.2.5
+Version: 5.3.0
 Summary: pyweatherfr displays weather forecast for a given town in world (with high accuracy for France)
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-5.2.5/README.md` & `pyweatherfr-5.3.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # :sunny: :umbrella: :cloud: pyweatherfr
 
-pyweatherfr affiche les prévisions méteo pour les communes françaises (voire mondiales) dans votre terminal. Il utilise l'API de MéteoFrance
+pyweatherfr affiche les prévisions méteo pour les communes françaises (voire mondiales) dans votre terminal. Il utilise l'API de MéteoFrance et d'OpenStreetMap.
 
 
 # 🚀 Comment utiliser **pyweatherfr**
 
-pyweatherfr affiche les prévisions météo sur 4 jours en se basant sur l'ip
-
 pyweatherfr \[VILLE\]
 
+exemple : ``pyweatherfr`` affiche les prévisions météo pour la ville trouvée en se basant sur l'ip
+
 exemple : ``pyweatherfr Grenoble`` affiche les prévisions météo pour Grenoble sur 4 jours
 
 exemple : ``pyweatherfr 38700`` affiche les prévisions météo pour le code postal 38700
 
 pyweatherfr -n \[VILLE\]
 
 exemple : ``pyweatherfr -n Grenoble`` affiche les données météo pour Grenoble 
@@ -39,27 +39,32 @@
 
 
 ## Autres options
 
   - ``-w/--world``  recherche la ville en pramètre dans le monde et non seulement en France
   - ``-h/--help``    montrer l'aide
   - ``-u/--update``  update pyweatherfr
-  - ``-c/--condensate``  condense la sortie
   - ``--nocolor``  désactive les couleurs et les emojis en sortie
   - ``-v/--verbose``  mode verbeux
   - ``--nocache``  supprime le cache de l'api meteo france avant l'appel
   - ``--utc``    utilise l'heure utc dans les previsions au lieu de l'heure locale de la ville
   - ``--pc``    utilise l'heure du pc dans les previsions au lieu de l'heure locale de la ville
-  - ``-l/--lang` recherche (puis affiche) les villes avec leurs noms locaux
-  
+  - ``-l/--lang`` recherche (puis affiche) les villes avec leurs noms locaux
+  - ``-f/--fullwidth`` affiche toutes les données y compris si la largeur du terminal est trop petite  
+
 # Démo
 
-![image](./demo_01.png)
+![image](https://github.com/thib1984/pyweatherfr/assets/45128847/9b0c5353-8e1b-4dfa-86b5-e2d5472a6cf2)
+
+![image](https://github.com/thib1984/pyweatherfr/assets/45128847/e92ceca0-e542-4c15-8eea-6a6067d55af8)
+
+![image](https://github.com/thib1984/pyweatherfr/assets/45128847/2d938bcd-3ee9-432b-a02d-080147ccc974)
+
+![image](https://github.com/thib1984/pyweatherfr/assets/45128847/b75a6a03-74fa-42b4-8cf5-24b15f35fa21)
 
-![image](./demo_02.png)
 
 # ⚙️ Install
 
 See [this page](INSTALL.md)
 
 # :construction_worker: Contribution
```

### Comparing `pyweatherfr-5.2.5/pyweatherfr/args.py` & `pyweatherfr-5.3.0/pyweatherfr/args.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,14 +105,20 @@
     my_parser.add_argument(
         "-w",
         "--world",
         action="store_true",
         help="activer la recherche hors France",
     )
     my_parser.add_argument(
+        "-f",
+        "--fullwidth",
+        action="store_true",
+        help="force l'affichage de toutes les données",
+    )    
+    my_parser.add_argument(
         "-l",
         "--lang",
         action="store_true",
         help="recherche (puis affiche) les villes avec leurs noms locaux",
     )     
     group = my_parser.add_mutually_exclusive_group()
     group.add_argument(
@@ -122,20 +128,14 @@
     )
     group.add_argument(
         "--utc",
         action="store_true",
         help="utilise l'heure UTC",
     )          
     my_parser.add_argument(
-        "-c",
-        "--condensate",
-        action="store_true",
-        help="condenser la sortie",
-    )
-    my_parser.add_argument(
         "--nocache",
         action="store_true",
         help="supprime le cache de l'api meteo france",
     )    
     my_parser.add_argument(
         "-v",
         "--verbose",
```

### Comparing `pyweatherfr-5.2.5/pyweatherfr/pyweatherfr.py` & `pyweatherfr-5.3.0/pyweatherfr/pyweatherfr.py`

 * *Files 4% similar despite different names*

```diff
@@ -122,15 +122,14 @@
     try:
         datetime.datetime.strptime(chaine, '%Y-%m-%d')
         return True
     except ValueError:
         return False
 
 def find():
-
     if compute_args().town:
         ville, dpt, lat, long,country = obtain_city_data()
     elif compute_args().gps:
         ville, dpt, lat, long,country = obtain_city_data_from_gps()
     else:
         ville, dpt, lat, long,country = obtain_city_data_from_ip()
     tz=timezonefinder.TimezoneFinder().timezone_at(lng=float(long), lat=float(lat))
@@ -196,29 +195,34 @@
         warning = ""
         if (
             (datetime.datetime.now(tz=pytz.timezone(tz)) + datetime.timedelta(days=new_var)).strftime(
             "%Y-%m-%d") == datetime.datetime.now(tz=pytz.timezone(tz)).strftime("%Y-%m-%d")
             and 0 < h - int(datetime.datetime.now(tz=pytz.timezone(tz)).strftime("%H")) <= 1
         ):
             warning = warning + " " + CLOCK
-        temp = (
-            f"{hourly_temperature_2m[h]:.1f}°C ({hourly_apparent_temperature[h]:.1f}°C)"
-        )
+        if isFullWidth():    
+            temp = (
+                f"{hourly_temperature_2m[h]:.1f}°C ({hourly_apparent_temperature[h]:.1f}°C)"
+            )
+        else:
+            temp = (
+                f"{hourly_temperature_2m[h]:.0f}°C"
+            )               
         if hourly_temperature_2m[h] <= WARNING_FROID or hourly_apparent_temperature[h] <= WARNING_FROID:
             warning = warning + " " + COLD
         if hourly_temperature_2m[h] >= WARNING_WARM or hourly_apparent_temperature[h] >= WARNING_WARM:
             warning = warning + " " + WARM
         pluie = f"{hourly_precipitation[h]:.1f}mm"
         if snowfall[h] >= WARNING_SNOW:
             warning = warning + " " + SNOW
         elif hourly_precipitation[h] >= WARNING_RAIN:
             warning = warning + " " + RAIN
 
         vent = (
-            f"{hourly_wind_speed_10m[h]:.1f}km/h ({hourly_wind_gusts_10m[h]:.1f}km/h)"
+            f"{hourly_wind_speed_10m[h]:.0f}km/h ({hourly_wind_gusts_10m[h]:.0f}km/h)"
         )
         direction = calculer_direction(hourly_wind_direction_10m[h])
 
         vent = vent
         if hourly_wind_speed_10m[h] >= WARNING_WIND or hourly_wind_gusts_10m[h] >= WARNING_WIND_GUST:
             warning = warning + " " + WIND
 
@@ -230,90 +234,155 @@
         weather, emojiweather = traduction(current_weather_code[h],isday[h])
         humidity = f"{relative_humidity_2m[h]:.0f}%"
         duree_soleil = f"{sunshine_duration[h]/60:.0f}'"
         rayonnement = f" {shortwave_radiation[h]:.0f}W/m\u00B2" 
         if shortwave_radiation[h]>1000:
             warning = warning + " " + LUNETTES   
         if compute_args().nocolor:
-            data.append(
-                [
-                    datetime.datetime.strftime(
-                        datetime.datetime.now(tz=pytz.timezone(tz)).replace(
-                            hour=0, minute=0, second=0, microsecond=0
-                        )
-                        + datetime.timedelta(days=new_var)
-                        + datetime.timedelta(hours=h),
-                        "%Y-%m-%d %H:%M",
-                    ),
-                    weather,
-                    temp,
-                    pluie,
-                    vent,
-                    direction,
-                    pression,
-                    humidity,
-                    rayonnement,
-                ]
-            )
+            if isFullWidth():
+                data.append(
+                    [
+                        datetime.datetime.strftime(
+                            datetime.datetime.now(tz=pytz.timezone(tz)).replace(
+                                hour=0, minute=0, second=0, microsecond=0
+                            )
+                            + datetime.timedelta(days=new_var)
+                            + datetime.timedelta(hours=h),
+                            "%H:%M",
+                        ),
+                        weather,
+                        temp,
+                        pluie,
+                        vent,
+                        direction,
+                        pression,
+                        humidity,
+                        rayonnement,
+                    ]
+                )
+            else:
+                data.append(
+                    [
+                        datetime.datetime.strftime(
+                            datetime.datetime.now(tz=pytz.timezone(tz)).replace(
+                                hour=0, minute=0, second=0, microsecond=0
+                            )
+                            + datetime.timedelta(days=new_var)
+                            + datetime.timedelta(hours=h),
+                            "%H:%M",
+                        ),
+                        weather,
+                        temp,
+                        pluie,
+                        vent,
+                        direction
+                    ]
+                )                    
         else:
-            data.append(
-                [
-                    datetime.datetime.strftime(
-                        datetime.datetime.now(tz=pytz.timezone(tz)).replace(
-                            hour=0, minute=0, second=0, microsecond=0
-                        )
-                        + datetime.timedelta(days=new_var)
-                        + datetime.timedelta(hours=h),
-                        "%Y-%m-%d %H:%M",
-                    ),
-                    emojiweather + " " + weather,
-                    temp,
-                    pluie,
-                    vent,
-                    direction,
-                    pression,
-                    humidity,
-                    rayonnement,
-                    warning,
-                ]
-            )
+            if isFullWidth():
+                data.append(
+                    [
+                        datetime.datetime.strftime(
+                            datetime.datetime.now(tz=pytz.timezone(tz)).replace(
+                                hour=0, minute=0, second=0, microsecond=0
+                            )
+                            + datetime.timedelta(days=new_var)
+                            + datetime.timedelta(hours=h),
+                            "%H:%M",
+                        ),
+                        emojiweather + " " + weather,
+                        temp,
+                        pluie,
+                        vent,
+                        direction,
+                        pression,
+                        humidity,
+                        rayonnement,
+                        warning,
+                    ]
+                )
+            else:
+                data.append(
+                    [
+                        datetime.datetime.strftime(
+                            datetime.datetime.now(tz=pytz.timezone(tz)).replace(
+                                hour=0, minute=0, second=0, microsecond=0
+                            )
+                            + datetime.timedelta(days=new_var)
+                            + datetime.timedelta(hours=h),
+                            "%H:%M",
+                        ),
+                        emojiweather + " " + weather,
+                        temp,
+                        pluie,
+                        vent,
+                        direction,
+                        warning,
+                    ]
+                )                    
 
     if compute_args().nocolor:
-        headers = [
-            "date",
-            "temps",
-            "température (ressentie)",
-            "précipitations",
-            "vent (rafales)",
-            "direction vent",
-            "pression",
-            "humidité",
-            "rayonnement"            
-        ]
+        if isFullWidth():
+            headers = [
+                "heure",
+                "temps",
+                "température (ressentie)",
+                "pluie",
+                "vent (rafales)",
+                "dir.",
+                "pression",
+                "humidité",
+                "rayonnement"            
+            ]
+        else:
+            headers = [
+                "heure",
+                "temps",
+                "température",
+                "pluie",
+                "vent (rafales)",
+                "dir."         
+            ]                
     else:
-        headers = [
-            "date",
-            "temps",
-            "température (ressentie)",
-            "précipitations",
-            "vent (rafales)",
-            "direction vent",
-            "pression",
-            "humidité",
-            "rayonnement",            
-            "warnings",
-        ]
-
-    if data != []:
-        if compute_args().condensate:
-            table = columnar.columnar(data, headers, no_borders=True, wrap_max=0)
+        if isFullWidth():
+            headers = [
+                "heure",
+                "temps",
+                "température (ressentie)",
+                "pluie",
+                "vent (rafales)",
+                "dir.",
+                "pression",
+                "humidité",
+                "rayonnement",            
+                "/!\\",
+            ]
         else:
-            print("")
-            table = columnar.columnar(data, headers, no_borders=False, wrap_max=0)
+            headers = [
+                "heure",
+                "temps",
+                "température",
+                "pluie",
+                "vent (rafales)",
+                "dir.",          
+                "/!\\",
+            ]            
+    if data != []:
+        print("")
+        table = columnar.columnar(data, headers, no_borders=False, wrap_max=0)
         print(table)
+        if not isFullWidth():
+            print(my_colored("warning : pour + d'affichage, élargissez votre terminal", "yellow"))
+
+def isFullWidth():
+    try:
+        return os.get_terminal_size().columns > 140 or compute_args().fullwidth
+    except Exception:
+        print_debug("détection impossible de la largeur du terminal")
+        return True
 
 def calculer_direction(direction_vent_degres):
     if (
             direction_vent_degres <= 22.5
             or direction_vent_degres >= 360 - 22.5
         ):
         direction = "N  "
@@ -385,25 +454,25 @@
             return ["nuageux ", NIGHT_CLOUD]        
         return ["nuageux", CLOUD]
     if current_weather_code >= 13 and current_weather_code <= 19:
         return ["pluie proche", RAIN]
     if current_weather_code >= 20 and current_weather_code <= 29:
         return ["fin de pluie", RAIN]
     if current_weather_code >= 30 and current_weather_code <= 39:
-        return ["tempete de poussière, sable ou neige", FOG]
+        return ["tempete", FOG]
     if current_weather_code >= 40 and current_weather_code <= 49:
         return ["brouillard", FOG]
     if current_weather_code >= 50 and current_weather_code <= 59:
         return ["bruine", RAIN]
     if current_weather_code >= 60 and current_weather_code <= 69:
         return ["pluie", RAIN]
     if current_weather_code >= 70 and current_weather_code <= 79:
         return ["neige", SNOW]
     if current_weather_code >= 80 and current_weather_code <= 99:
-        return ["averse / orage", ORAGE_PLUIE]
+        return ["averse-orage", ORAGE_PLUIE]
     return ["", ""]
 
 def previsions_courantes(ville, dpt, lat, long, tz):
     
 
     (
         current_temperature_2m,
@@ -506,19 +575,16 @@
                 ]
             )
         if w_soleil>1000:
             data.append(["rayonnement", f"{w_soleil:.0f}W/m\u00B2",LUNETTES]) 
         else:      
             data.append(["rayonnement", f"{w_soleil:.0f}W/m\u00B2",""]) 
         data.append(["temps", emojiweather + " " + current_weather, ""])
-    if compute_args().condensate:
-        table = columnar.columnar(data, no_borders=True, wrap_max=0)
-    else:
-        print("")
-        table = columnar.columnar(data, no_borders=False, wrap_max=0)
+    print("")
+    table = columnar.columnar(data, no_borders=False, wrap_max=0)
     print(table)
 
 
 def previsions_generiques(ville, dpt, lat, long, tz):
 
     
     (
@@ -558,15 +624,18 @@
         if not numpy.isnan(daily_precipitation_sum[i]):
             warning = ""
             pluie = f"{daily_precipitation_sum[i]:.1f}mm"
             if snowfall[i] >= WARNING_SNOW:
                 warning = warning + " " + SNOW
             elif daily_precipitation_sum[i] >= WARNING_RAIN:
                 warning = warning + " " + RAIN
-            temp = f"{daily_temperature_2m_min[i]:.1f}°C ({daily_apparent_temperature_min[i]:.1f}°C) -> {daily_temperature_2m_max[i]:.1f}°C ({daily_apparent_temperature_max[i]:.1f}°C)"
+            if isFullWidth():    
+                temp = f"{daily_temperature_2m_min[i]:.1f}°C ({daily_apparent_temperature_min[i]:.1f}°C) -> {daily_temperature_2m_max[i]:.1f}°C ({daily_apparent_temperature_max[i]:.1f}°C)"
+            else:
+                temp = f"{daily_temperature_2m_min[i]:.0f}°C -> {daily_temperature_2m_max[i]:.0f}°C"
             if (
                 daily_temperature_2m_min[i] <= WARNING_FROID
                 or daily_apparent_temperature_min[i] <= WARNING_FROID
                 or daily_temperature_2m_max[i] <= WARNING_FROID
                 or daily_apparent_temperature_max[i] <= WARNING_FROID
             ):
                 warning = warning + " " + COLD
@@ -575,96 +644,159 @@
                 or daily_apparent_temperature_min[i] >= WARNING_WARM
                 or daily_temperature_2m_max[i] >= WARNING_WARM
                 or daily_apparent_temperature_max[i] >= WARNING_WARM
             ):
                 warning = warning + " " + WARM
             weather, emojiweather = traduction(weather_code[i],1)
 
-            vent = f"{daily_wind_speed_10m_max[i]:.1f}km/h ({daily_wind_gusts_10m_max[i]:.1f}km/h)"
+            vent = f"{daily_wind_speed_10m_max[i]:.0f}km/h ({daily_wind_gusts_10m_max[i]:.0f}km/h)"
             direction=calculer_direction(daily_wind_direction_10m_dominant[i])
 
 
             vent = vent
             if daily_wind_speed_10m_max[i] >= WARNING_WIND or daily_wind_gusts_10m_max[i] >= WARNING_WIND_GUST:
                 warning = warning + " " + WIND
             duree_pluie = f"{precipitation_hours[i]:.0f}h"
             duree_soleil = f"{sunshine_duration[i]/3600:.1f}h"
             if compute_args().nocolor:
-                data.append(
-                    [
-                        datetime.datetime.strftime(
-                            datetime.datetime.now(tz=pytz.timezone(tz)).replace(
-                                hour=0, minute=0, second=0, microsecond=0
-                            )
-                            + datetime.timedelta(hours=24 * i),
-                            "%Y-%m-%d",
-                        ),
-                        weather,
-                        temp,
-                        pluie,
-                        vent,
-                        direction,
-                        duree_pluie,
-                        duree_soleil
-                    ]
-                )
+                if isFullWidth():
+                    data.append(
+                        [
+                            datetime.datetime.strftime(
+                                datetime.datetime.now(tz=pytz.timezone(tz)).replace(
+                                    hour=0, minute=0, second=0, microsecond=0
+                                )
+                                + datetime.timedelta(hours=24 * i),
+                                "%Y-%m-%d",
+                            ),
+                            weather,
+                            temp,
+                            pluie,
+                            vent,
+                            direction,
+                            duree_pluie,
+                            duree_soleil
+                        ]
+                    )
+                else:
+                    data.append(
+                        [
+                            datetime.datetime.strftime(
+                                datetime.datetime.now(tz=pytz.timezone(tz)).replace(
+                                    hour=0, minute=0, second=0, microsecond=0
+                                )
+                                + datetime.timedelta(hours=24 * i),
+                                "%y-%m-%d",
+                            ),
+                            weather,
+                            temp,
+                            pluie,
+                            vent,
+                            direction
+                        ]
+                    )
             else:
-                data.append(
-                    [
-                        datetime.datetime.strftime(
-                            datetime.datetime.now(tz=pytz.timezone(tz)).replace(
-                                hour=0, minute=0, second=0, microsecond=0
-                            )
-                            + datetime.timedelta(hours=24 * i)
-                            + datetime.timedelta(days=-1*compute_args().past),
-                            "%Y-%m-%d",
-                        ),
-                        emojiweather + " " + weather,
-                        temp,
-                        pluie,
-                        vent,
-                        direction,
-                        duree_pluie,
-                        duree_soleil,
-                        warning,
-                    ]
-                )
+                if isFullWidth():
+
+                    data.append(
+                        [
+                            datetime.datetime.strftime(
+                                datetime.datetime.now(tz=pytz.timezone(tz)).replace(
+                                    hour=0, minute=0, second=0, microsecond=0
+                                )
+                                + datetime.timedelta(hours=24 * i)
+                                + datetime.timedelta(days=-1*compute_args().past),
+                                "%Y-%m-%d",
+                            ),
+                            emojiweather + " " + weather,
+                            temp,
+                            pluie,
+                            vent,
+                            direction,
+                            duree_pluie,
+                            duree_soleil,
+                            warning,
+                        ]
+                    )
+                else:
+                    data.append(
+                        [
+                            datetime.datetime.strftime(
+                                datetime.datetime.now(tz=pytz.timezone(tz)).replace(
+                                    hour=0, minute=0, second=0, microsecond=0
+                                )
+                                + datetime.timedelta(hours=24 * i)
+                                + datetime.timedelta(days=-1*compute_args().past),
+                                "%y-%m-%d",
+                            ),
+                            emojiweather + " " + weather,
+                            temp,
+                            pluie,
+                            vent,
+                            direction,
+                            warning,
+                        ]
+                    )
         else:
             tronque=True
     if data != []:
         if compute_args().nocolor:
-            headers = [
-                "date",
-                "temps",
-                "température (ressentie)",
-                "précipitations",
-                "vent (rafales)",
-                "direction",
-                "durée pluie",
-                "durée soleil"
-            ]
+            if isFullWidth():
+            
+                headers = [
+                    "date",
+                    "temps",
+                    "température (ressentie)",
+                    "pluie",
+                    "vent (rafales)",
+                    "direction",
+                    "tps pluie",
+                    "tps soleil"
+                ]
+            else:
+                headers = [
+                    "date",
+                    "temps",
+                    "température",
+                    "pluie",
+                    "vent (rafales)",
+                    "direction"
+                ]                
         else:
-            headers = [
-                "date",
-                "temps",
-                "température (ressentie)",
-                "précipitations",
-                "vent (rafales)",
-                "direction vent",
-                "durée pluie",
-                "durée soleil",
-                "warning",
-            ]
+            if isFullWidth():
 
-        if compute_args().condensate:
-            table = columnar.columnar(data, headers, no_borders=True, wrap_max=0)
-        else:
-            print("")
-            table = columnar.columnar(data, headers, no_borders=False, wrap_max=0)
+                headers = [
+                    "date",
+                    "temps",
+                    "température (ressentie)",
+                    "pluie",
+                    "vent (rafales)",
+                    "dir.",
+                    "tps pluie",
+                    "tps soleil",
+                    "",
+                ]
+            else:
+                                headers = [
+                    "date",
+                    "temps",
+                    "température",
+                    "pluie",
+                    "vent (rafales)",
+                    "dir.",
+                    "",
+                ]
+
+
+        print("")
+        table = columnar.columnar(data, headers, no_borders=False, wrap_max=0)
         print(table)
+        if not isFullWidth():
+            print(my_colored("warning : pour + d'affichage, élargissez votre terminal", "yellow"))
+
     if tronque:
         print(my_colored("warning : données tronquées", "yellow"))
 
 def print_generic_data_town(ville, dpt, lat, long, alt, recap):
     print("")
 
     data = []
@@ -682,18 +814,17 @@
             print_debug("pas de data pour ville/dpt/cp")
         elif dpt is None or dpt == "":
             data.append([HOME, ville])
         else:    
             data.append([HOME, ville + " (" + dpt + ")"])
         data.append([BOUSSOLE, f"lat.:  {float(lat):.4f}°  / long.: {float(long):.4f}° / alt.: {float(alt):.0f}m "])
         data.append([PC,recap])
-    if compute_args().condensate:
-        table = columnar.columnar(data, no_borders=True, wrap_max=0)
-    else:
-        table = columnar.columnar(data, no_borders=False, wrap_max=0)
+
+
+    table = columnar.columnar(data, no_borders=False, wrap_max=0)
 
     print(table)
 
 
 def display_error(r):
     print(my_colored("erreur : pas de données trouvées", "red"))
     print_debug(r.json().get("errors")[0].get("code"))
```

### Comparing `pyweatherfr-5.2.5/pyweatherfr.egg-info/PKG-INFO` & `pyweatherfr-5.3.0/pyweatherfr.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 5.2.5
+Version: 5.3.0
 Summary: pyweatherfr displays weather forecast for a given town in world (with high accuracy for France)
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-5.2.5/setup.py` & `pyweatherfr-5.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name="pyweatherfr",
-    version="5.2.5",
+    version="5.3.0",
     description="pyweatherfr displays weather forecast for a given town in world (with high accuracy for France)",
     long_description="The complete description/installation/use/FAQ is available at : https://github.com/thib1984/pyweatherfr#readme",
     url="https://github.com/thib1984/pyweatherfr",
     author="thib1984",
     author_email="thibault.garcon@gmail.com",
     license="MIT",
     packages=["pyweatherfr"],
```

