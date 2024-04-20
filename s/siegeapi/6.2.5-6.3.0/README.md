# Comparing `tmp/siegeapi-6.2.5.tar.gz` & `tmp/siegeapi-6.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siegeapi-6.2.5.tar", last modified: Wed Mar 13 16:28:07 2024, max compression
+gzip compressed data, was "siegeapi-6.3.0.tar", last modified: Sat Apr 20 08:26:13 2024, max compression
```

## Comparing `siegeapi-6.2.5.tar` & `siegeapi-6.3.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:28:07.436809 siegeapi-6.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-13 16:28:02.000000 siegeapi-6.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-03-13 16:28:07.436809 siegeapi-6.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-03-13 16:28:02.000000 siegeapi-6.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-13 16:28:02.000000 siegeapi-6.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 16:28:07.436809 siegeapi-6.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-03-13 16:28:02.000000 siegeapi-6.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:28:07.436809 siegeapi-6.2.5/siegeapi/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-13 16:28:02.000000 siegeapi-6.2.5/siegeapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12617 2024-03-13 16:28:02.000000 siegeapi-6.2.5/siegeapi/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:28:07.436809 siegeapi-6.2.5/siegeapi/constants/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-13 16:28:02.000000 siegeapi-6.2.5/siegeapi/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33141 2024-03-13 16:28:02.000000 siegeapi-6.2.5/siegeapi/constants/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-03-13 16:28:02.000000 siegeapi-6.2.5/siegeapi/constants/ranks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-03-13 16:28:02.000000 siegeapi-6.2.5/siegeapi/constants/seasons.py
--rw-r--r--   0 runner    (1001) docker     (127)    22727 2024-03-13 16:28:02.000000 siegeapi-6.2.5/siegeapi/constants/weapons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-03-13 16:28:02.000000 siegeapi-6.2.5/siegeapi/default_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-13 16:28:02.000000 siegeapi-6.2.5/siegeapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-03-13 16:28:02.000000 siegeapi-6.2.5/siegeapi/linked_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-03-13 16:28:02.000000 siegeapi-6.2.5/siegeapi/maps.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-03-13 16:28:02.000000 siegeapi-6.2.5/siegeapi/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    11618 2024-03-13 16:28:02.000000 siegeapi-6.2.5/siegeapi/player.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-03-13 16:28:02.000000 siegeapi-6.2.5/siegeapi/rank_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-03-13 16:28:02.000000 siegeapi-6.2.5/siegeapi/ranks.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-13 16:28:02.000000 siegeapi-6.2.5/siegeapi/summaries.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-03-13 16:28:02.000000 siegeapi-6.2.5/siegeapi/trends.py
--rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-03-13 16:28:02.000000 siegeapi-6.2.5/siegeapi/url_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-03-13 16:28:02.000000 siegeapi-6.2.5/siegeapi/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-03-13 16:28:02.000000 siegeapi-6.2.5/siegeapi/weapons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:28:07.436809 siegeapi-6.2.5/siegeapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-03-13 16:28:07.000000 siegeapi-6.2.5/siegeapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-03-13 16:28:07.000000 siegeapi-6.2.5/siegeapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 16:28:07.000000 siegeapi-6.2.5/siegeapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-13 16:28:07.000000 siegeapi-6.2.5/siegeapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-13 16:28:07.000000 siegeapi-6.2.5/siegeapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:26:13.312725 siegeapi-6.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-20 08:26:05.000000 siegeapi-6.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-20 08:26:13.312725 siegeapi-6.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-20 08:26:05.000000 siegeapi-6.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-20 08:26:05.000000 siegeapi-6.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 08:26:13.312725 siegeapi-6.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-20 08:26:05.000000 siegeapi-6.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:26:13.312725 siegeapi-6.3.0/siegeapi/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-20 08:26:05.000000 siegeapi-6.3.0/siegeapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14194 2024-04-20 08:26:05.000000 siegeapi-6.3.0/siegeapi/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:26:13.312725 siegeapi-6.3.0/siegeapi/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-20 08:26:05.000000 siegeapi-6.3.0/siegeapi/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33141 2024-04-20 08:26:05.000000 siegeapi-6.3.0/siegeapi/constants/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-04-20 08:26:05.000000 siegeapi-6.3.0/siegeapi/constants/ranks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-04-20 08:26:05.000000 siegeapi-6.3.0/siegeapi/constants/seasons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22727 2024-04-20 08:26:05.000000 siegeapi-6.3.0/siegeapi/constants/weapons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-20 08:26:05.000000 siegeapi-6.3.0/siegeapi/default_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-20 08:26:05.000000 siegeapi-6.3.0/siegeapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-20 08:26:05.000000 siegeapi-6.3.0/siegeapi/linked_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-20 08:26:05.000000 siegeapi-6.3.0/siegeapi/maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-04-20 08:26:05.000000 siegeapi-6.3.0/siegeapi/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-20 08:26:05.000000 siegeapi-6.3.0/siegeapi/persona.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16291 2024-04-20 08:26:05.000000 siegeapi-6.3.0/siegeapi/player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-20 08:26:05.000000 siegeapi-6.3.0/siegeapi/rank_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-20 08:26:05.000000 siegeapi-6.3.0/siegeapi/ranks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-20 08:26:05.000000 siegeapi-6.3.0/siegeapi/summaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-04-20 08:26:05.000000 siegeapi-6.3.0/siegeapi/trends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-04-20 08:26:05.000000 siegeapi-6.3.0/siegeapi/url_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-20 08:26:05.000000 siegeapi-6.3.0/siegeapi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-20 08:26:05.000000 siegeapi-6.3.0/siegeapi/weapons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:26:13.312725 siegeapi-6.3.0/siegeapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-20 08:26:13.000000 siegeapi-6.3.0/siegeapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-20 08:26:13.000000 siegeapi-6.3.0/siegeapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 08:26:13.000000 siegeapi-6.3.0/siegeapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-20 08:26:13.000000 siegeapi-6.3.0/siegeapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-20 08:26:13.000000 siegeapi-6.3.0/siegeapi.egg-info/top_level.txt
```

### Comparing `siegeapi-6.2.5/LICENSE` & `siegeapi-6.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `siegeapi-6.2.5/PKG-INFO` & `siegeapi-6.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siegeapi
-Version: 6.2.5
+Version: 6.3.0
 Summary: Rainbow Six Siege API interface
 Home-page: https://github.com/CNDRD/siegeapi
 Author: CNDRD
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -18,15 +18,15 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aiohttp<3.8.0,>=3.6.0
+Requires-Dist: aiohttp>=3.6.0
 
 <div align="center">
     <img width="250" src="https://raw.githubusercontent.com/CNDRD/siegeapi/master/assets/siegeapi-banner.png" />
     <h1>siegeapi</h1>
     <a href="https://github.com/CNDRD/siegeapi/releases">
         <img src="https://img.shields.io/github/v/release/CNDRD/siegeapi?label=latest%20release&style=for-the-badge&logo=github&logoColor=white" />
     </a>
@@ -49,53 +49,58 @@
 
 ## Quick example  
 ```python
 from siegeapi import Auth
 import asyncio
 
 async def sample():
-    auth = Auth("UBI_EMAIL", "UBI_PASSWORD")
-    player = await auth.get_player(uid="7e0f63df-a39b-44c5-8de0-d39a05926e77")
+    auth = Auth(UBISOFT_EMAIL, UBISOFT_PASSW)
+    player = await auth.get_player(name="CNDRD")
 
     print(f"Name: {player.name}")
     print(f"Profile pic URL: {player.profile_pic_url}")
-    
+
+    await player.load_persona()
+    print(f"Streamer nickname: {player.persona.nickname}")
+    print(f"Nickname enabled: {player.persona.enabled}")
+
     await player.load_playtime()
-    print(f"Total Time Played: {player.total_time_played:,} seconds")
+    print(f"Total Time Played: {player.total_time_played:,} seconds / {player.total_time_played_hours:,} hours")
     print(f"Level: {player.level}")
 
     await player.load_ranked_v2()
     print(f"Ranked Points: {player.ranked_profile.rank_points}")
     print(f"Rank: {player.ranked_profile.rank}")
     print(f"Max Rank Points: {player.ranked_profile.max_rank_points}")
     print(f"Max Rank: {player.ranked_profile.max_rank}")
 
     await player.load_progress()
     print(f"XP: {player.xp:,}")
     print(f"Total XP: {player.total_xp:,}")
     print(f"XP to level up: {player.xp_to_level_up:,}")
-    
+
     await auth.close()
 
-asyncio.get_event_loop().run_until_complete(sample())
-# Or `asyncio.run(sample())`  
+asyncio.run(sample())
 ```
 ### Output  
 ```text
 Name: CNDRD
 Profile pic URL: https://ubisoft-avatars.akamaized.net/7e0f63df-a39b-44c5-8de0-d39a05926e77/default_256_256.png
-Total Time Played: 9,037,159 seconds
-Level: 305
-Ranked Points: 4188
-Rank: Diamond 4
-Max Rank Points: 4289
-Max Rank: Diamond 3
-XP: 11,858
-Total XP: 20,694,358
-XP to level up: 131,642
+Streamer nickname: d1kCheeze
+Nickname enabled: True
+Total Time Played: 9,265,890 seconds / 2,573 hours
+Level: 308
+Ranked Points: 3919
+Rank: Emerald 1
+Max Rank Points: 3933
+Max Rank: Emerald 1
+XP: 124,375
+Total XP: 21,238,875
+XP to level up: 20,625
 ```
 
 ---  
 
 ## Siege Inventory  
 If you want to see every skin, headgear, uniform and more, head over to **[skins.cndrd.xyz](https://skins.cndrd.xyz/)**
```

#### html2text {}

```diff
@@ -1,54 +1,57 @@
-Metadata-Version: 2.1 Name: siegeapi Version: 6.2.5 Summary: Rainbow Six Siege
+Metadata-Version: 2.1 Name: siegeapi Version: 6.3.0 Summary: Rainbow Six Siege
 API interface Home-page: https://github.com/CNDRD/siegeapi Author: CNDRD
 License: MIT Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License Classifier: Intended
 Audience :: Developers Classifier: Natural Language :: English Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3.11 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Topic :: Internet Classifier: Topic :: Software
 Development :: Libraries Classifier: Topic :: Software Development :: Libraries
 :: Python Modules Classifier: Topic :: Utilities Classifier: Typing :: Typed
 Requires-Python: >=3.8.0 Description-Content-Type: text/markdown License-File:
-LICENSE Requires-Dist: aiohttp<3.8.0,>=3.6.0
+LICENSE Requires-Dist: aiohttp>=3.6.0
    [https://raw.githubusercontent.com/CNDRD/siegeapi/master/assets/siegeapi-
                                   banner.png]
                             ************ ssiieeggeeaappii ************
                 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_v_/_r_e_l_e_a_s_e_/_C_N_D_R_D_/
                 _s_i_e_g_e_a_p_i_?_l_a_b_e_l_=_l_a_t_e_s_t_%_2_0_r_e_l_e_a_s_e_&_s_t_y_l_e_=_f_o_r_-_t_h_e_-
        _b_a_d_g_e_&_l_o_g_o_=_g_i_t_h_u_b_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/
             _s_i_e_g_e_a_p_i_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_=_p_y_p_i_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_]
         _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_s_i_e_g_e_a_p_i_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-
 _b_a_d_g_e_&_l_o_g_o_=_p_y_t_h_o_n_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_&_c_o_l_o_r_=_y_e_l_l_o_w_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/
      _s_i_e_g_e_a_p_i_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_=_p_y_p_i_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_&_c_o_l_o_r_=_y_e_l_l_o_w_]
 ## How to install ```commandline pip install siegeapi ``` ## Quick example
 ```python from siegeapi import Auth import asyncio async def sample(): auth =
-Auth("UBI_EMAIL", "UBI_PASSWORD") player = await auth.get_player(uid="7e0f63df-
-a39b-44c5-8de0-d39a05926e77") print(f"Name: {player.name}") print(f"Profile pic
-URL: {player.profile_pic_url}") await player.load_playtime() print(f"Total Time
-Played: {player.total_time_played:,} seconds") print(f"Level: {player.level}")
+Auth(UBISOFT_EMAIL, UBISOFT_PASSW) player = await auth.get_player(name="CNDRD")
+print(f"Name: {player.name}") print(f"Profile pic URL:
+{player.profile_pic_url}") await player.load_persona() print(f"Streamer
+nickname: {player.persona.nickname}") print(f"Nickname enabled:
+{player.persona.enabled}") await player.load_playtime() print(f"Total Time
+Played: {player.total_time_played:,} seconds /
+{player.total_time_played_hours:,} hours") print(f"Level: {player.level}")
 await player.load_ranked_v2() print(f"Ranked Points:
 {player.ranked_profile.rank_points}") print(f"Rank:
 {player.ranked_profile.rank}") print(f"Max Rank Points:
 {player.ranked_profile.max_rank_points}") print(f"Max Rank:
 {player.ranked_profile.max_rank}") await player.load_progress() print(f"XP:
 {player.xp:,}") print(f"Total XP: {player.total_xp:,}") print(f"XP to level up:
-{player.xp_to_level_up:,}") await auth.close() asyncio.get_event_loop
-().run_until_complete(sample()) # Or `asyncio.run(sample())` ``` ### Output
-```text Name: CNDRD Profile pic URL: https://ubisoft-avatars.akamaized.net/
-7e0f63df-a39b-44c5-8de0-d39a05926e77/default_256_256.png Total Time Played:
-9,037,159 seconds Level: 305 Ranked Points: 4188 Rank: Diamond 4 Max Rank
-Points: 4289 Max Rank: Diamond 3 XP: 11,858 Total XP: 20,694,358 XP to level
-up: 131,642 ``` --- ## Siege Inventory If you want to see every skin, headgear,
-uniform and more, head over to **[skins.cndrd.xyz](https://skins.cndrd.xyz/)**
-## Docs For docs go to [cndrd.github.io/siegeapi](https://cndrd.github.io/
-siegeapi/) ## Credits Operator Icons from [r6operators][r6operators_] by
-[marcopixel][marcopixel_] & sourced by me straight from the game files Built
-(and re-built) on top of what [billy-yoyo][r6s_python_api] started ## Problems
-If you experience any problems, reach out to me, or submit a PR You can reach
-out here on GitHub or on Discord (_cndrd_) ![forthebadge](https://
-forthebadge.com/images/badges/works-on-my-machine.svg) ![forthebadge](https://
-forthebadge.com/images/badges/powered-by-energy-drinks.svg) [r6operators_]:
-https://github.com/marcopixel/r6operators [marcopixel_]: https://github.com/
-marcopixel [r6s_python_api]: https://github.com/billy-yoyo/RainbowSixSiege-
-Python-API
+{player.xp_to_level_up:,}") await auth.close() asyncio.run(sample()) ``` ###
+Output ```text Name: CNDRD Profile pic URL: https://ubisoft-
+avatars.akamaized.net/7e0f63df-a39b-44c5-8de0-d39a05926e77/default_256_256.png
+Streamer nickname: d1kCheeze Nickname enabled: True Total Time Played:
+9,265,890 seconds / 2,573 hours Level: 308 Ranked Points: 3919 Rank: Emerald 1
+Max Rank Points: 3933 Max Rank: Emerald 1 XP: 124,375 Total XP: 21,238,875 XP
+to level up: 20,625 ``` --- ## Siege Inventory If you want to see every skin,
+headgear, uniform and more, head over to **[skins.cndrd.xyz](https://
+skins.cndrd.xyz/)** ## Docs For docs go to [cndrd.github.io/siegeapi](https://
+cndrd.github.io/siegeapi/) ## Credits Operator Icons from [r6operators]
+[r6operators_] by [marcopixel][marcopixel_] & sourced by me straight from the
+game files Built (and re-built) on top of what [billy-yoyo][r6s_python_api]
+started ## Problems If you experience any problems, reach out to me, or submit
+a PR You can reach out here on GitHub or on Discord (_cndrd_) ![forthebadge]
+(https://forthebadge.com/images/badges/works-on-my-machine.svg) ![forthebadge]
+(https://forthebadge.com/images/badges/powered-by-energy-drinks.svg)
+[r6operators_]: https://github.com/marcopixel/r6operators [marcopixel_]: https:
+//github.com/marcopixel [r6s_python_api]: https://github.com/billy-yoyo/
+RainbowSixSiege-Python-API
```

### Comparing `siegeapi-6.2.5/README.md` & `siegeapi-6.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -23,53 +23,58 @@
 
 ## Quick example  
 ```python
 from siegeapi import Auth
 import asyncio
 
 async def sample():
-    auth = Auth("UBI_EMAIL", "UBI_PASSWORD")
-    player = await auth.get_player(uid="7e0f63df-a39b-44c5-8de0-d39a05926e77")
+    auth = Auth(UBISOFT_EMAIL, UBISOFT_PASSW)
+    player = await auth.get_player(name="CNDRD")
 
     print(f"Name: {player.name}")
     print(f"Profile pic URL: {player.profile_pic_url}")
-    
+
+    await player.load_persona()
+    print(f"Streamer nickname: {player.persona.nickname}")
+    print(f"Nickname enabled: {player.persona.enabled}")
+
     await player.load_playtime()
-    print(f"Total Time Played: {player.total_time_played:,} seconds")
+    print(f"Total Time Played: {player.total_time_played:,} seconds / {player.total_time_played_hours:,} hours")
     print(f"Level: {player.level}")
 
     await player.load_ranked_v2()
     print(f"Ranked Points: {player.ranked_profile.rank_points}")
     print(f"Rank: {player.ranked_profile.rank}")
     print(f"Max Rank Points: {player.ranked_profile.max_rank_points}")
     print(f"Max Rank: {player.ranked_profile.max_rank}")
 
     await player.load_progress()
     print(f"XP: {player.xp:,}")
     print(f"Total XP: {player.total_xp:,}")
     print(f"XP to level up: {player.xp_to_level_up:,}")
-    
+
     await auth.close()
 
-asyncio.get_event_loop().run_until_complete(sample())
-# Or `asyncio.run(sample())`  
+asyncio.run(sample())
 ```
 ### Output  
 ```text
 Name: CNDRD
 Profile pic URL: https://ubisoft-avatars.akamaized.net/7e0f63df-a39b-44c5-8de0-d39a05926e77/default_256_256.png
-Total Time Played: 9,037,159 seconds
-Level: 305
-Ranked Points: 4188
-Rank: Diamond 4
-Max Rank Points: 4289
-Max Rank: Diamond 3
-XP: 11,858
-Total XP: 20,694,358
-XP to level up: 131,642
+Streamer nickname: d1kCheeze
+Nickname enabled: True
+Total Time Played: 9,265,890 seconds / 2,573 hours
+Level: 308
+Ranked Points: 3919
+Rank: Emerald 1
+Max Rank Points: 3933
+Max Rank: Emerald 1
+XP: 124,375
+Total XP: 21,238,875
+XP to level up: 20,625
 ```
 
 ---  
 
 ## Siege Inventory  
 If you want to see every skin, headgear, uniform and more, head over to **[skins.cndrd.xyz](https://skins.cndrd.xyz/)**
```

#### html2text {}

```diff
@@ -6,36 +6,39 @@
        _b_a_d_g_e_&_l_o_g_o_=_g_i_t_h_u_b_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/
             _s_i_e_g_e_a_p_i_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_=_p_y_p_i_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_]
         _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_s_i_e_g_e_a_p_i_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-
 _b_a_d_g_e_&_l_o_g_o_=_p_y_t_h_o_n_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_&_c_o_l_o_r_=_y_e_l_l_o_w_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/
      _s_i_e_g_e_a_p_i_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_=_p_y_p_i_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_&_c_o_l_o_r_=_y_e_l_l_o_w_]
 ## How to install ```commandline pip install siegeapi ``` ## Quick example
 ```python from siegeapi import Auth import asyncio async def sample(): auth =
-Auth("UBI_EMAIL", "UBI_PASSWORD") player = await auth.get_player(uid="7e0f63df-
-a39b-44c5-8de0-d39a05926e77") print(f"Name: {player.name}") print(f"Profile pic
-URL: {player.profile_pic_url}") await player.load_playtime() print(f"Total Time
-Played: {player.total_time_played:,} seconds") print(f"Level: {player.level}")
+Auth(UBISOFT_EMAIL, UBISOFT_PASSW) player = await auth.get_player(name="CNDRD")
+print(f"Name: {player.name}") print(f"Profile pic URL:
+{player.profile_pic_url}") await player.load_persona() print(f"Streamer
+nickname: {player.persona.nickname}") print(f"Nickname enabled:
+{player.persona.enabled}") await player.load_playtime() print(f"Total Time
+Played: {player.total_time_played:,} seconds /
+{player.total_time_played_hours:,} hours") print(f"Level: {player.level}")
 await player.load_ranked_v2() print(f"Ranked Points:
 {player.ranked_profile.rank_points}") print(f"Rank:
 {player.ranked_profile.rank}") print(f"Max Rank Points:
 {player.ranked_profile.max_rank_points}") print(f"Max Rank:
 {player.ranked_profile.max_rank}") await player.load_progress() print(f"XP:
 {player.xp:,}") print(f"Total XP: {player.total_xp:,}") print(f"XP to level up:
-{player.xp_to_level_up:,}") await auth.close() asyncio.get_event_loop
-().run_until_complete(sample()) # Or `asyncio.run(sample())` ``` ### Output
-```text Name: CNDRD Profile pic URL: https://ubisoft-avatars.akamaized.net/
-7e0f63df-a39b-44c5-8de0-d39a05926e77/default_256_256.png Total Time Played:
-9,037,159 seconds Level: 305 Ranked Points: 4188 Rank: Diamond 4 Max Rank
-Points: 4289 Max Rank: Diamond 3 XP: 11,858 Total XP: 20,694,358 XP to level
-up: 131,642 ``` --- ## Siege Inventory If you want to see every skin, headgear,
-uniform and more, head over to **[skins.cndrd.xyz](https://skins.cndrd.xyz/)**
-## Docs For docs go to [cndrd.github.io/siegeapi](https://cndrd.github.io/
-siegeapi/) ## Credits Operator Icons from [r6operators][r6operators_] by
-[marcopixel][marcopixel_] & sourced by me straight from the game files Built
-(and re-built) on top of what [billy-yoyo][r6s_python_api] started ## Problems
-If you experience any problems, reach out to me, or submit a PR You can reach
-out here on GitHub or on Discord (_cndrd_) ![forthebadge](https://
-forthebadge.com/images/badges/works-on-my-machine.svg) ![forthebadge](https://
-forthebadge.com/images/badges/powered-by-energy-drinks.svg) [r6operators_]:
-https://github.com/marcopixel/r6operators [marcopixel_]: https://github.com/
-marcopixel [r6s_python_api]: https://github.com/billy-yoyo/RainbowSixSiege-
-Python-API
+{player.xp_to_level_up:,}") await auth.close() asyncio.run(sample()) ``` ###
+Output ```text Name: CNDRD Profile pic URL: https://ubisoft-
+avatars.akamaized.net/7e0f63df-a39b-44c5-8de0-d39a05926e77/default_256_256.png
+Streamer nickname: d1kCheeze Nickname enabled: True Total Time Played:
+9,265,890 seconds / 2,573 hours Level: 308 Ranked Points: 3919 Rank: Emerald 1
+Max Rank Points: 3933 Max Rank: Emerald 1 XP: 124,375 Total XP: 21,238,875 XP
+to level up: 20,625 ``` --- ## Siege Inventory If you want to see every skin,
+headgear, uniform and more, head over to **[skins.cndrd.xyz](https://
+skins.cndrd.xyz/)** ## Docs For docs go to [cndrd.github.io/siegeapi](https://
+cndrd.github.io/siegeapi/) ## Credits Operator Icons from [r6operators]
+[r6operators_] by [marcopixel][marcopixel_] & sourced by me straight from the
+game files Built (and re-built) on top of what [billy-yoyo][r6s_python_api]
+started ## Problems If you experience any problems, reach out to me, or submit
+a PR You can reach out here on GitHub or on Discord (_cndrd_) ![forthebadge]
+(https://forthebadge.com/images/badges/works-on-my-machine.svg) ![forthebadge]
+(https://forthebadge.com/images/badges/powered-by-energy-drinks.svg)
+[r6operators_]: https://github.com/marcopixel/r6operators [marcopixel_]: https:
+//github.com/marcopixel [r6s_python_api]: https://github.com/billy-yoyo/
+RainbowSixSiege-Python-API
```

### Comparing `siegeapi-6.2.5/setup.py` & `siegeapi-6.3.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name="siegeapi",
-    version="6.2.5",
+    version="6.3.0",
     url="https://github.com/CNDRD/siegeapi",
     description="Rainbow Six Siege API interface",
     author="CNDRD",
     packages=find_packages(),
     license="MIT",
     include_package_data=True,
-    install_requires=["aiohttp>=3.6.0,<3.8.0"],
+    install_requires=["aiohttp>=3.6.0"],
     python_requires=">=3.8.0",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Developers",
```

### Comparing `siegeapi-6.2.5/siegeapi/auth.py` & `siegeapi-6.3.0/siegeapi/auth.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,27 +11,29 @@
 import os
 
 from .exceptions import FailedToConnect, InvalidRequest
 from .player import Player
 
 PLATFORMS = ["uplay", "xbl", "psn"]
 
+
 class Auth:
     """ Holds the authentication information """
 
     @staticmethod
     def get_basic_token(email: str, password: str) -> str:
         return base64.b64encode(f"{email}:{password}".encode("utf-8")).decode("utf-8")
 
     def __init__(
             self,
             email: Optional[str] = None,
             password: Optional[str] = None,
             token: Optional[str] = None,
             appid: Optional[str] = None,
+            spaceids: Optional[Dict[Literal['uplay', 'psn', 'xbl', 'xplay'], str]] = None,
             creds_path: Optional[str] = None,
             cachetime: int = 120,
             max_connect_retries: int = 1,
             session: Optional[aiohttp.ClientSession] = None,
             refresh_session_period: int = 180
     ):
         self.session: aiohttp.ClientSession = session or aiohttp.ClientSession()
@@ -48,57 +50,67 @@
         self.creds_path: str = creds_path or f"{os.getcwd()}/creds/{self.token}.json"
         self.appid: str = appid or 'e3d5ea9e-50bd-43b7-88bf-39794f4e3d40'
         self.sessionid: str = ""
         self.key: Optional[str] = ""
         self.new_key: str = ""
         self.spaceid: str = ""
         self.spaceids: Dict[str, str] = {
-            "uplay": "0d2ae42d-4c27-4cb7-af6c-2099062302bb",
-            "psn": "0d2ae42d-4c27-4cb7-af6c-2099062302bb",
-            "xbl": "0d2ae42d-4c27-4cb7-af6c-2099062302bb"
+            "uplay": "5172a557-50b5-4665-b7db-e3f2e8c5041d",
+            "psn": "05bfb3f7-6c21-4c42-be1f-97a33fb5cf66",
+            "xbl": "98a601e5-ca91-4440-b1c5-753f601a2c90",
+            "xplay": "0d2ae42d-4c27-4cb7-af6c-2099062302bb"
         }
+        if spaceids:
+            self.spaceids.update(spaceids)
+
         self.profileid: str = ""
         self.userid: str = ""
         self.expiration: str = ""
         self.new_expiration: str = ""
 
         self.cachetime: int = cachetime
         self.cache = {}
 
         self._login_cooldown: int = 0
         self._session_start: float = time.time()
 
     async def _find_players(self, name: Optional[str], platform: Literal["uplay", "xbl", "psn"], uid: Optional[str]) -> List[Player]:
         """ Get a list of players matching the search term on a given platform.
-        Must provide either name or uid, but not both."""
+        Must provide either name or uid, but not both.
+
+        Raises:
+            TypeError: If neither name nor uid is provided, if both are provided, or if platform is None.
+            InvalidRequest: If the returned API request  is missing the 'profiles' key.
+
+        Returns:
+            List[Player]: A list of player objects matching the search term.
+        """        
         if (not name and not uid) or (name and uid):
             await self.close()
             raise TypeError("Exactly one non-empty parameter should be provided (name or uid)")
 
         if not platform:
             await self.close()
             raise TypeError("'platform' cannot be None")
 
         if platform not in PLATFORMS:
             await self.close()
             raise TypeError(f"'platform' has to be one of the following: {PLATFORMS}; Not {platform}")
 
         if name:
-            data = await self.get(f"https://public-ubiservices.ubi.com/v3/profiles?"
-                                  f"nameOnPlatform={parse.quote(name)}&platformType={parse.quote(platform)}")
+            data = await self.get(f"https://public-ubiservices.ubi.com/v3/profiles?nameOnPlatform={parse.quote(name)}&platformType={parse.quote(platform)}")
         else:
-            data = await self.get(f"https://public-ubiservices.ubi.com/v3/users/{uid}/profiles?"
-                                  f"platformType={parse.quote(platform)}")
+            data = await self.get(f"https://public-ubiservices.ubi.com/v3/users/{uid}/profiles?platformType={parse.quote(platform)}")
         
         if not isinstance(data, dict):
             await self.close()
             raise InvalidRequest(f"Expected a JSON object, got {type(data)}")
 
         if "profiles" in data:
-            results = [Player(self, x) for x in data.get("profiles",{}) if x.get("platformType", "") == platform]
+            results = [Player(self, x) for x in data.get("profiles", {}) if x.get("platformType", "") == platform]
             if not results:
                 await self.close()
                 raise InvalidRequest("No results")
             return results
         else:
             raise InvalidRequest(f"Missing key profiles in returned JSON object {str(data)}")
 
@@ -116,20 +128,24 @@
             except:
                 pass
 
         self.session = aiohttp.ClientSession()
         self._session_start = time.time()
 
     async def get_session(self) -> aiohttp.ClientSession:
-        """ Retrieves the current session, ensuring it's valid first."""
+        """Retrieves the current session, ensuring it's valid first.
+
+        Returns:
+            aiohttp.ClientSession: The current session.
+        """
         await self._ensure_session_valid()
         return self.session
 
     def save_creds(self) -> None:
-        """ Saves the credentials to a file. """
+        """Saves the credentials to a file."""
 
         if not os.path.exists(os.path.dirname(self.creds_path)):
             os.makedirs(os.path.dirname(self.creds_path))
 
         if not os.path.exists(self.creds_path):
             with open(self.creds_path, 'w') as f:
                 json.dump({}, f)
@@ -144,15 +160,15 @@
                 "profileid": self.profileid,
                 "userid": self.userid,
                 "expiration": self.expiration,
                 "new_expiration": self.new_expiration,
             }, f, indent=4)
 
     def load_creds(self) -> None:
-        """ Loads the credentials from a file """
+        """Loads the credentials from a file."""
 
         if not os.path.exists(self.creds_path):
             return
 
         with open(self.creds_path, "r") as f:
             data = json.load(f)
 
@@ -164,15 +180,16 @@
         self.userid = data.get("userid", "")
         self.expiration = data.get("expiration", "")
         self.new_expiration = data.get("new_expiration", "")
 
         self._login_cooldown = 0
 
     async def connect(self, _new: bool = False) -> None:
-        """ Connect to Ubisoft, automatically called when needed """
+        """Connect to the Ubisoft API.
+        This method will be automatically called when needed."""
         self.load_creds()
 
         if self._login_cooldown > time.time():
             raise FailedToConnect("Login on cooldown")
 
         # If keys are still valid, don't connect again
         if _new:
@@ -224,19 +241,21 @@
                 message = str(data["httpCode"])
             raise FailedToConnect(message)
 
         self.save_creds()
         await self.connect(_new=True)
 
     async def close(self) -> None:
-        """ Closes the session associated with the auth object """
+        """Closes the session associated with the auth object. """
         self.save_creds()
         await self.session.close()
 
     async def get(self, *args, retries: int = 0, json_: bool = True, new: bool = False, **kwargs) -> Union[dict, str]:
+        """Sends a GET request to the Ubisoft API.
+        Intended for internal use only."""
         if (not self.key and not new) or (not self.new_key and new):
             last_error = None
             for _ in range(self.max_connect_retries):
                 try:
                     await self.connect()
                     break
                 except FailedToConnect as e:
@@ -277,36 +296,55 @@
                 raise InvalidRequest(f"Received a text response, expected JSON response. Message: {message}")
 
             if "httpCode" in data:
                 if data["httpCode"] == 401:
                     if retries >= self.max_connect_retries:
                         # wait 30 seconds before sending another request
                         # pyright type checker doesn't like the below line
-                        self._login_cooldown = 30 + time.time() # type: ignore
+                        self._login_cooldown = 30 + time.time()  # type: ignore
 
                     # key no longer works, so remove key and let the following .get() call refresh it
                     self.key = None
                     return await self.get(*args, retries=retries + 1, **kwargs)
                 else:
                     msg = data.get("message", "")
                     if data["httpCode"] == 404:
                         msg = f"Missing resource {data.get('resource', args[0])}"
                     raise InvalidRequest(f"HTTP {data['httpCode']}: {msg}", code=data["httpCode"])
-
             return data
         else:
             return await resp.text()
 
     async def get_player(self, name: Optional[str] = None, uid: Optional[str] = None, platform: Literal["uplay", "xbl", "psn"] = "uplay") -> Player:
-        """ Calls get_players and returns the first element """
+        """Get a player object by name or uid.
+        Calls get_players and returns the first element.
 
+        Args:
+            name (Optional[str]): The username of the player. Defaults to None.
+            uid (Optional[str]): The UID of the player. Defaults to None.
+            platform (Literal[uplay, xbl, psn]): The playform the player plays on. Defaults to "uplay".
+
+        Returns:
+            Player: The player object.
+        """
         results = await self._find_players(name=name, platform=platform, uid=uid)
         return results[0]
 
     async def get_player_batch(self, names: Optional[List[str]] = None, uids: Optional[List[str]] = None, platform: Literal["uplay", "xbl", "psn"] = "uplay") -> Dict[str, Player]:
+        """Get a dictionary of players by name or uid.
+        Note that all players must share the same provided platform.
+
+        Args:
+            name (Optional[str]): List of usernames to lookup. Defaults to None.
+            uid (Optional[str]): List of UIDs to lookup. Defaults to None.
+            platform (Literal[uplay, xbl, psn]): The playform the players plays on. Defaults to "uplay".
+
+        Returns:
+            Dict[str, Player]: A dictionary of player objects, with the form {uid: player}.
+        """
         players = {}
         if names is not None:
             for name in names:
                 player = await self.get_player(name=name, platform=platform)
                 players[player.id] = player
 
         if uids is not None:
```

### Comparing `siegeapi-6.2.5/siegeapi/constants/operators.py` & `siegeapi-6.3.0/siegeapi/constants/operators.py`

 * *Files identical despite different names*

### Comparing `siegeapi-6.2.5/siegeapi/constants/ranks.py` & `siegeapi-6.3.0/siegeapi/constants/ranks.py`

 * *Files identical despite different names*

### Comparing `siegeapi-6.2.5/siegeapi/constants/seasons.py` & `siegeapi-6.3.0/siegeapi/constants/seasons.py`

 * *Files identical despite different names*

### Comparing `siegeapi-6.2.5/siegeapi/constants/weapons.py` & `siegeapi-6.3.0/siegeapi/constants/weapons.py`

 * *Files identical despite different names*

### Comparing `siegeapi-6.2.5/siegeapi/default_stats.py` & `siegeapi-6.3.0/siegeapi/default_stats.py`

 * *Files identical despite different names*

### Comparing `siegeapi-6.2.5/siegeapi/maps.py` & `siegeapi-6.3.0/siegeapi/maps.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,18 +20,21 @@
 
     def __repr__(self) -> str:
         return str(vars(self))
 
 
 class Maps:
     def __init__(self, data: dict):
-        self.all: MapRoles = MapRoles(data.get("platforms",{}).get("PC",{}).get("gameModes",{}).get("all", {}))
-        self.casual: MapRoles = MapRoles(data.get("platforms",{}).get("PC",{}).get("gameModes",{}).get("casual", {}))
-        self.ranked: MapRoles = MapRoles(data.get("platforms",{}).get("PC",{}).get("gameModes",{}).get("ranked", {}))
-        self.unranked: MapRoles = MapRoles(data.get("platforms",{}).get("PC",{}).get("gameModes",{}).get("unranked", {}))
+        platform_data = data.get("platforms", {})
+        platform_data = platform_data.get(list(platform_data.keys())[0] if len(platform_data.keys()) > 0 else "PC", {})
+
+        self.all: MapRoles = MapRoles(platform_data.get("gameModes", {}).get("all", {}))
+        self.casual: MapRoles = MapRoles(platform_data.get("gameModes", {}).get("casual", {}))
+        self.ranked: MapRoles = MapRoles(platform_data.get("gameModes", {}).get("ranked", {}))
+        self.unranked: MapRoles = MapRoles(platform_data.get("gameModes", {}).get("unranked", {}))
         self._start_date: str = str(data.get("startDate", ""))
         self._end_date: str = str(data.get("endDate", ""))
 
     def get_timespan_dates(self) -> Dict[str, str]:
         return {"start_date": self._start_date, "end_date": self._end_date}
 
     def __repr__(self) -> str:
```

### Comparing `siegeapi-6.2.5/siegeapi/operators.py` & `siegeapi-6.3.0/siegeapi/operators.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,14 @@
             self.unit: str = self._get_str_from_operators_const("unit")
             self.country_code: str = self._get_str_from_operators_const("country_code")
             self.season_introduced: str = self._get_str_from_operators_const("season_introduced")
 
     def _get_from_operators_const(self, value: str) -> Union[str, int, list]:
         return operator_dict.get(self.name.lower(), {}).get(value, "Missing Data")
 
-    # for typing
     def _get_str_from_operators_const(self, value: str) -> str:
         returnv = self._get_from_operators_const(value)
         if isinstance(returnv, str):
             return returnv
         raise ValueError(f"Value {value} is not a string")
     
     def _get_int_from_operators_const(self, value: str) -> int:
@@ -41,33 +40,38 @@
         raise ValueError(f"Value {value} is not an integer")
     
     def _get_list_from_operators_const(self, value: str) -> list:
         returnv = self._get_from_operators_const(value)
         if isinstance(returnv, list):
             return returnv
         raise ValueError(f"Value {value} is not a list")
-        
+    
+    def __repr__(self) -> str:
+        return str(vars(self))
 
 
 class OperatorsGameMode:
     def __init__(self, data: dict, op_about: bool):
         self.attacker: list = [Operator(operator, op_about) for operator in data.get("teamRoles", {}).get("Attacker", {})]
         self.defender: list = [Operator(operator, op_about) for operator in data.get("teamRoles", {}).get("Defender", {})]
 
     def __repr__(self) -> str:
         return str(vars(self))
 
 
 class Operators:
     def __init__(self, data: dict, op_about: bool):
-        self.all: OperatorsGameMode = OperatorsGameMode(data.get("platforms",{}).get("PC",{}).get("gameModes",{}).get("all", {}), op_about)
-        self.casual: OperatorsGameMode = OperatorsGameMode(data.get("platforms",{}).get("PC",{}).get("gameModes",{}).get("casual", {}), op_about)
-        self.ranked: OperatorsGameMode = OperatorsGameMode(data.get("platforms",{}).get("PC",{}).get("gameModes",{}).get("ranked", {}), op_about)
-        self.unranked: OperatorsGameMode = OperatorsGameMode(data.get("platforms",{}).get("PC",{}).get("gameModes",{}).get("unranked", {}), op_about)
-        self.newcomer: OperatorsGameMode = OperatorsGameMode(data.get("platforms",{}).get("PC",{}).get("gameModes",{}).get("newcomer", {}), op_about)
+        platform_data = data.get("platforms", {})
+        platform_data = platform_data.get(list(platform_data.keys())[0] if len(platform_data.keys()) > 0 else "PC", {})
+
+        self.all: OperatorsGameMode = OperatorsGameMode(platform_data.get("gameModes", {}).get("all", {}), op_about)
+        self.casual: OperatorsGameMode = OperatorsGameMode(platform_data.get("gameModes", {}).get("casual", {}), op_about)
+        self.ranked: OperatorsGameMode = OperatorsGameMode(platform_data.get("gameModes", {}).get("ranked", {}), op_about)
+        self.unranked: OperatorsGameMode = OperatorsGameMode(platform_data.get("gameModes", {}).get("unranked", {}), op_about)
+        self.newcomer: OperatorsGameMode = OperatorsGameMode(platform_data.get("gameModes", {}).get("newcomer", {}), op_about)
         self._start_date: str = str(data.get("startDate", ""))
         self._end_date: str = str(data.get("endDate", ""))
 
     def get_timespan_dates(self) -> Dict[str, str]:
         return {"start_date": self._start_date, "end_date": self._end_date}
 
     def __repr__(self) -> str:
```

### Comparing `siegeapi-6.2.5/siegeapi/rank_profile.py` & `siegeapi-6.3.0/siegeapi/rank_profile.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,21 +14,25 @@
         self.rank_id: int = profile.get("rank", 0)
         self.rank_points: int = profile.get("rank_points", 0)
         self.top_rank_position: int = profile.get("top_rank_position", 0)
         self.season_id: int = profile.get("season_id", 0)
 
         rank_constants = get_rank_constants(self.season_id)
         _, prev_, next_, _ = get_rank_from_mmr(self.rank_points)
-        self.max_rank: str = rank_constants[self.max_rank_id].get("name",'')
-        self.rank: str = rank_constants[self.rank_id].get("name",'')
+        self.max_rank: str = rank_constants[self.max_rank_id].get("name", '')
+        self.rank: str = rank_constants[self.rank_id].get("name", '')
         self.prev_rank_points: int = prev_
         self.next_rank_points: int = next_
         self.season_code: str = season_id_to_code(self.season_id)
 
         self.kills: int = season_stats.get("kills", 0)
         self.deaths: int = season_stats.get("deaths", 0)
         self.abandons: int = match_outcomes.get("abandons", 0)
         self.losses: int = match_outcomes.get("losses", 0)
         self.wins: int = match_outcomes.get("wins", 0)
 
     def get_dict(self) -> Dict[str, Union[str, int, float]]:
         return vars(self)
+
+    def __repr__(self) -> str:
+        return str(vars(self))
+
```

### Comparing `siegeapi-6.2.5/siegeapi/ranks.py` & `siegeapi-6.3.0/siegeapi/ranks.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,7 +33,11 @@
         if self.prev_rank_mmr == 0 and self.next_rank_mmr == 0:
             self.rank, self.prev_rank_mmr, self.next_rank_mmr, self.rank_id = get_rank_from_mmr(self.mmr)
             self.max_rank_id = self.max_mmr = 0
             self.max_rank = "Undefined"
 
     def get_dict(self) -> Dict[str, Union[str, int, float]]:
         return vars(self)
+
+    def __repr__(self) -> str:
+        return str(vars(self))
+
```

### Comparing `siegeapi-6.2.5/siegeapi/trends.py` & `siegeapi-6.3.0/siegeapi/trends.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,29 +30,36 @@
 
     def __repr__(self) -> str:
         return str(vars(self))
 
 
 class TrendsGameMode:
     def __init__(self, data: dict):
-        self.all: TrendData = TrendData(data.get("teamRoles", {}).get("all", [{}])[0])
-        self.attacker: TrendData = TrendData(data.get("teamRoles", {}).get("attacker", [{}])[0])
-        self.defender: TrendData = TrendData(data.get("teamRoles", {}).get("defender", [{}])[0])
+        _all = data.get("teamRoles", {}).get("all", [{}])
+        _attacker = data.get("teamRoles", {}).get("attacker", [{}])
+        _defender = data.get("teamRoles", {}).get("defender", [{}])
+
+        self.all: TrendData = TrendData(_all[0] if len(_all) > 0 else {})
+        self.attacker: TrendData = TrendData(_attacker[0] if len(_attacker) > 0 else {})
+        self.defender: TrendData = TrendData(_defender[0] if len(_defender) > 0 else {})
 
     def __repr__(self) -> str:
         return str(vars(self))
 
 
 class Trends:
     def __init__(self, data: dict):
-        self.all: TrendsGameMode = TrendsGameMode(data.get("platforms").get("PC").get("gameModes").get("all", {}))
-        self.casual: TrendsGameMode = TrendsGameMode(data.get("platforms").get("PC").get("gameModes").get("casual", {}))
-        self.ranked: TrendsGameMode = TrendsGameMode(data.get("platforms").get("PC").get("gameModes").get("ranked", {}))
-        self.unranked: TrendsGameMode = TrendsGameMode(data.get("platforms").get("PC").get("gameModes").get("unranked", {}))
-        self.newcomer: TrendsGameMode = TrendsGameMode(data.get("platforms").get("PC").get("gameModes").get("newcomer", {}))
+        platform_data = data.get("platforms", {})
+        platform_data = platform_data.get(list(platform_data.keys())[0] if len(platform_data.keys()) > 0 else "PC", {})
+
+        self.all: TrendsGameMode = TrendsGameMode(platform_data.get("gameModes").get("all", {}))
+        self.casual: TrendsGameMode = TrendsGameMode(platform_data.get("gameModes").get("casual", {}))
+        self.ranked: TrendsGameMode = TrendsGameMode(platform_data.get("gameModes").get("ranked", {}))
+        self.unranked: TrendsGameMode = TrendsGameMode(platform_data.get("gameModes").get("unranked", {}))
+        self.newcomer: TrendsGameMode = TrendsGameMode(platform_data.get("gameModes").get("newcomer", {}))
         self._start_date: str = str(data.get("startDate", ""))
         self._end_date: str = str(data.get("endDate", ""))
 
     def get_timespan_dates(self) -> dict:
         return {"start_date": self._start_date, "end_date": self._end_date}
 
     def __repr__(self) -> str:
```

### Comparing `siegeapi-6.2.5/siegeapi/url_builder.py` & `siegeapi-6.3.0/siegeapi/url_builder.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 from __future__ import annotations
+from typing import Dict
+
 
 class UrlBuilder:
-    def __init__(self, spaceid: str, platform_url: str, player_id: str, platform_group: str):
+    def __init__(self, spaceid: str, platform_url: str, player_id: str, player_uid: str, platform_group: str, spaceids: Dict[str, str]):
         self.spaceid: str = spaceid
+        self.spaceids: str = spaceids
+        self.xplay_spaceid: str = spaceids.get("xplay", "0d2ae42d-4c27-4cb7-af6c-2099062302bb")
         self.platform_url: str = platform_url
         self.platform_group: str = platform_group
-        self.player_id: str = player_id
+        self.uid: str = player_uid
+        self.id: str = player_id
+        self.player_id: str = player_uid if self.platform_group == "PC" else player_id
         self.start_date: str = ""
         self.end_date: str = ""
 
     def set_timespan_dates(self, start_date: str, end_date: str) -> None:
         self.start_date = f"&startDate={start_date}"
         self.end_date = f"&endDate={end_date}"
 
     def linked_accounts(self) -> str:
         return f"https://public-ubiservices.ubi.com/v3/users/{self.player_id}/profiles"
 
     def xp_lvl(self) -> str:
-        return f"https://public-ubiservices.ubi.com/v1/spaces/{self.spaceid}/title/r6s/rewards/public_profile?" \
+        return f"https://public-ubiservices.ubi.com/v1/spaces/{self.xplay_spaceid}/title/r6s/rewards/public_profile?" \
                f"profile_id={self.player_id}"
 
     def playtime(self) -> str:
         return f"https://public-ubiservices.ubi.com/v1/profiles/stats?" \
                f"profileIds={self.player_id}" \
-               f"&spaceId={self.spaceid}" \
+               f"&spaceId={self.xplay_spaceid}" \
                f"&statNames=PPvPTimePlayed,PPvETimePlayed,PTotalTimePlayed,PClearanceLevel"
 
     def skill_records(self, seasons: str, boards: str, regions: str):
         return f"https://public-ubiservices.ubi.com/v1/spaces/{self.spaceid}/" \
                f"sandboxes/{self.platform_url}/r6karma/player_skill_records?" \
                f"board_ids={boards}" \
                f"&season_ids={seasons}" \
@@ -39,64 +45,67 @@
                f"sandboxes/{self.platform_url}/r6karma/players?" \
                f"board_id=pvp_{board_id}" \
                f"&profile_ids={self.player_id}" \
                f"&region_id={region}" \
                f"&season_id={season}"
 
     def trends(self) -> str:
-        return f"https://prod.datadev.ubisoft.com/v1/profiles/{self.player_id}/playerstats?" \
+        return f"https://prod.datadev.ubisoft.com/v1/profiles/{self.uid}/playerstats?" \
                f"spaceId={self.spaceid}" \
                f"&view=current" \
                f"&aggregation=movingpoint" \
                f"&trendType=daily" \
                f"&gameMode=all,ranked,casual,unranked" \
-               f"&platformGroup=PC" \
+               f"&platformGroup={self.platform_group}" \
                f"&teamRole=all,attacker,defender" \
                f"{self.start_date}" \
                f"{self.end_date}"
 
     def weapons(self) -> str:
-        return f"https://prod.datadev.ubisoft.com/v1/profiles/{self.player_id}/playerstats?" \
-               f"spaceId={self.spaceid}" \
+        return f"https://prod.datadev.ubisoft.com/v1/profiles/{self.uid}/playerstats?" \
+               f"spaceId={self.xplay_spaceid}" \
                f"&view=current" \
                f"&aggregation=weapons" \
                f"&gameMode=all,ranked,casual,unranked" \
-               f"&platformGroup=PC" \
-               f"&teamRole=attacker,defender" \
+               f"&platformGroup={self.platform_group}" \
+               f"&teamRole=all,attacker,defender" \
                f"{self.start_date}" \
                f"{self.end_date}"
 
     def operators(self) -> str:
-        return f"https://prod.datadev.ubisoft.com/v1/profiles/{self.player_id}/playerstats?" \
-               f"spaceId={self.spaceid}" \
+        return f"https://prod.datadev.ubisoft.com/v1/profiles/{self.uid}/playerstats?" \
+               f"spaceId={self.xplay_spaceid}" \
                f"&view=current" \
                f"&aggregation=operators" \
                f"&gameMode=all,ranked,casual,unranked" \
-               f"&platformGroup=PC" \
+               f"&platformGroup={self.platform_group}" \
                f"&teamRole=all,Attacker,Defender" \
                f"{self.start_date}" \
                f"{self.end_date}"
 
     def maps(self) -> str:
-        return f"https://prod.datadev.ubisoft.com/v1/profiles/{self.player_id}/playerstats?" \
-               f"spaceId={self.spaceid}" \
+        return f"https://prod.datadev.ubisoft.com/v1/profiles/{self.uid}/playerstats?" \
+               f"spaceId={self.xplay_spaceid}" \
                f"&view=current" \
                f"&aggregation=maps" \
                f"&gameMode=all,ranked,casual,unranked" \
-               f"&platformGroup=PC" \
+               f"&platformGroup={self.platform_group}" \
                f"&teamRole=all,Attacker,Defender" \
                f"{self.start_date}" \
                f"{self.end_date}"
 
     def seasonal_summaries(self, gamemodes: str, team_roles: str) -> str:
         return f"https://prod.datadev.ubisoft.com/v1/users/{self.player_id}/playerstats?" \
-               f"spaceId={self.spaceid}" \
+               f"spaceId={self.xplay_spaceid}" \
                f"&view=seasonal" \
                f"&aggregation=summary" \
                f"&gameMode={gamemodes}" \
                f"&platformGroup={self.platform_group}" \
                f"&teamRole={team_roles}"
 
     def full_profiles(self) -> str:
-        return f"https://public-ubiservices.ubi.com/v2/spaces/{self.spaceid}/title/r6s/skill/full_profiles?" \
-               f"profile_ids={self.player_id}" \
+        return f"https://public-ubiservices.ubi.com/v2/spaces/{self.xplay_spaceid}/title/r6s/skill/full_profiles?" \
+               f"profile_ids={self.uid}" \
                f"&platform_families={self.platform_group.lower()}"
+
+    def persona(self) -> str:
+        return f"https://public-ubiservices.ubi.com/v1/profiles/{self.player_id}/persona?spaceId={self.xplay_spaceid}"
```

### Comparing `siegeapi-6.2.5/siegeapi/utils.py` & `siegeapi-6.3.0/siegeapi/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 from typing import Dict, List, Optional, Tuple, Union
 
-from .constants import seasons as seasons_const
-from .exceptions import InvalidAttributeCombination
 from .constants.ranks import *
 
+import re
 
 def get_xp_to_next_lvl(lvl: int) -> int:
     if lvl > 37:
         return (lvl - 18) * 500
     if lvl == 0:
         return 500
     if lvl == 1:
@@ -35,41 +34,37 @@
         return 8_500
     if lvl in (29, 30, 31):
         return 9_000
     if lvl in (32, 33, 34):
         return 9_500
     if lvl in (35, 36, 37):
         return 10_000
-    #return None
     raise ValueError(f"Level {lvl} is not a valid level.")
 
 
 def get_total_xp(lvl: int, current_xp: int) -> int:
     total = 0
     for level in range(1, lvl):
         total += get_xp_to_next_lvl(level)
     return total + current_xp
 
 
 def season_id_to_code(season_id: int) -> Optional[str]:
-    seasons_count = len(seasons_const) - 3
-    season_id = seasons_count - season_id if season_id < 0 else season_id
-
-    return seasons_const.get(season_id, {}).get("code",None)
+    yr = (season_id - 1) // 4 + 1
+    ssn = (season_id - 1) % 4 + 1
+    return f"Y{yr}S{ssn}"
 
 
 def season_code_to_id(season_code: str) -> int:
-    """Depends on 'seasons_const' always being up-to-date.."""
-    seasons_count = len(seasons_const) - 3
-    season_id = next((k for k, v in seasons_const.items() if v["code"] == season_code), None)
-
-    if season_id is None:
-        raise InvalidAttributeCombination(f"Season code '{season_code}' is invalid")
+    
+    if not re.match(r'Y\d+S\d+', season_code):
+        raise ValueError(f"Season code {season_code} does not match the expected format 'YXSX' where X is a number.")
 
-    return seasons_count - season_id if season_id < 0 else season_id
+    code_split = season_code.split('S')
+    return (int(code_split[0][1:]) - 1) * 4 + int(code_split[1])
 
 
 def get_rank_constants(season_number: int = -1) -> List[Dict[str, Union[str, int]]]:
     if 1 <= season_number <= 3:
         return ranks_v1
     if 4 == season_number:
         return ranks_v2
```

### Comparing `siegeapi-6.2.5/siegeapi/weapons.py` & `siegeapi-6.3.0/siegeapi/weapons.py`

 * *Files 23% similar despite different names*

```diff
@@ -40,28 +40,32 @@
 
     def __repr__(self) -> str:
         return str(vars(self))
 
 
 class WeaponsRole:
     def __init__(self, data: dict):
+        self.all: WeaponsGameMode = WeaponsGameMode(data.get("teamRoles", {}).get("all", {}))
         self.attacker: WeaponsGameMode = WeaponsGameMode(data.get("teamRoles", {}).get("attacker", {}))
         self.defender: WeaponsGameMode = WeaponsGameMode(data.get("teamRoles", {}).get("defender", {}))
 
     def __repr__(self) -> str:
         return str(vars(self))
 
 
 class Weapons:
     def __init__(self, data: dict):
-        self.all: WeaponsRole = WeaponsRole(data.get("platforms",{}).get("PC",{}).get("gameModes",{}).get("all", {}))
-        self.casual: WeaponsRole = WeaponsRole(data.get("platforms",{}).get("PC",{}).get("gameModes",{}).get("casual", {}))
-        self.ranked: WeaponsRole = WeaponsRole(data.get("platforms",{}).get("PC",{}).get("gameModes",{}).get("ranked", {}))
-        self.unranked: WeaponsRole = WeaponsRole(data.get("platforms",{}).get("PC",{}).get("gameModes",{}).get("unranked", {}))
-        self.newcomer: WeaponsRole = WeaponsRole(data.get("platforms",{}).get("PC",{}).get("gameModes",{}).get("newcomer", {}))
+        platform_data = data.get("platforms", {})
+        platform_data = platform_data.get(list(platform_data.keys())[0] if len(platform_data.keys()) > 0 else "PC", {})
+
+        self.all: WeaponsRole = WeaponsRole(platform_data.get("gameModes",{}).get("all", {}))
+        self.casual: WeaponsRole = WeaponsRole(platform_data.get("gameModes",{}).get("casual", {}))
+        self.ranked: WeaponsRole = WeaponsRole(platform_data.get("gameModes",{}).get("ranked", {}))
+        self.unranked: WeaponsRole = WeaponsRole(platform_data.get("gameModes",{}).get("unranked", {}))
+        self.newcomer: WeaponsRole = WeaponsRole(platform_data.get("gameModes",{}).get("newcomer", {}))
         self._start_date: str = str(data.get("startDate", ""))
         self._end_date: str = str(data.get("endDate", ""))
 
     def get_timespan_dates(self) -> dict:
         return {"start_date": self._start_date, "end_date": self._end_date}
 
     def __repr__(self) -> str:
```

### Comparing `siegeapi-6.2.5/siegeapi.egg-info/PKG-INFO` & `siegeapi-6.3.0/siegeapi.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siegeapi
-Version: 6.2.5
+Version: 6.3.0
 Summary: Rainbow Six Siege API interface
 Home-page: https://github.com/CNDRD/siegeapi
 Author: CNDRD
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -18,15 +18,15 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aiohttp<3.8.0,>=3.6.0
+Requires-Dist: aiohttp>=3.6.0
 
 <div align="center">
     <img width="250" src="https://raw.githubusercontent.com/CNDRD/siegeapi/master/assets/siegeapi-banner.png" />
     <h1>siegeapi</h1>
     <a href="https://github.com/CNDRD/siegeapi/releases">
         <img src="https://img.shields.io/github/v/release/CNDRD/siegeapi?label=latest%20release&style=for-the-badge&logo=github&logoColor=white" />
     </a>
@@ -49,53 +49,58 @@
 
 ## Quick example  
 ```python
 from siegeapi import Auth
 import asyncio
 
 async def sample():
-    auth = Auth("UBI_EMAIL", "UBI_PASSWORD")
-    player = await auth.get_player(uid="7e0f63df-a39b-44c5-8de0-d39a05926e77")
+    auth = Auth(UBISOFT_EMAIL, UBISOFT_PASSW)
+    player = await auth.get_player(name="CNDRD")
 
     print(f"Name: {player.name}")
     print(f"Profile pic URL: {player.profile_pic_url}")
-    
+
+    await player.load_persona()
+    print(f"Streamer nickname: {player.persona.nickname}")
+    print(f"Nickname enabled: {player.persona.enabled}")
+
     await player.load_playtime()
-    print(f"Total Time Played: {player.total_time_played:,} seconds")
+    print(f"Total Time Played: {player.total_time_played:,} seconds / {player.total_time_played_hours:,} hours")
     print(f"Level: {player.level}")
 
     await player.load_ranked_v2()
     print(f"Ranked Points: {player.ranked_profile.rank_points}")
     print(f"Rank: {player.ranked_profile.rank}")
     print(f"Max Rank Points: {player.ranked_profile.max_rank_points}")
     print(f"Max Rank: {player.ranked_profile.max_rank}")
 
     await player.load_progress()
     print(f"XP: {player.xp:,}")
     print(f"Total XP: {player.total_xp:,}")
     print(f"XP to level up: {player.xp_to_level_up:,}")
-    
+
     await auth.close()
 
-asyncio.get_event_loop().run_until_complete(sample())
-# Or `asyncio.run(sample())`  
+asyncio.run(sample())
 ```
 ### Output  
 ```text
 Name: CNDRD
 Profile pic URL: https://ubisoft-avatars.akamaized.net/7e0f63df-a39b-44c5-8de0-d39a05926e77/default_256_256.png
-Total Time Played: 9,037,159 seconds
-Level: 305
-Ranked Points: 4188
-Rank: Diamond 4
-Max Rank Points: 4289
-Max Rank: Diamond 3
-XP: 11,858
-Total XP: 20,694,358
-XP to level up: 131,642
+Streamer nickname: d1kCheeze
+Nickname enabled: True
+Total Time Played: 9,265,890 seconds / 2,573 hours
+Level: 308
+Ranked Points: 3919
+Rank: Emerald 1
+Max Rank Points: 3933
+Max Rank: Emerald 1
+XP: 124,375
+Total XP: 21,238,875
+XP to level up: 20,625
 ```
 
 ---  
 
 ## Siege Inventory  
 If you want to see every skin, headgear, uniform and more, head over to **[skins.cndrd.xyz](https://skins.cndrd.xyz/)**
```

#### html2text {}

```diff
@@ -1,54 +1,57 @@
-Metadata-Version: 2.1 Name: siegeapi Version: 6.2.5 Summary: Rainbow Six Siege
+Metadata-Version: 2.1 Name: siegeapi Version: 6.3.0 Summary: Rainbow Six Siege
 API interface Home-page: https://github.com/CNDRD/siegeapi Author: CNDRD
 License: MIT Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License Classifier: Intended
 Audience :: Developers Classifier: Natural Language :: English Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3.11 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Topic :: Internet Classifier: Topic :: Software
 Development :: Libraries Classifier: Topic :: Software Development :: Libraries
 :: Python Modules Classifier: Topic :: Utilities Classifier: Typing :: Typed
 Requires-Python: >=3.8.0 Description-Content-Type: text/markdown License-File:
-LICENSE Requires-Dist: aiohttp<3.8.0,>=3.6.0
+LICENSE Requires-Dist: aiohttp>=3.6.0
    [https://raw.githubusercontent.com/CNDRD/siegeapi/master/assets/siegeapi-
                                   banner.png]
                             ************ ssiieeggeeaappii ************
                 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_v_/_r_e_l_e_a_s_e_/_C_N_D_R_D_/
                 _s_i_e_g_e_a_p_i_?_l_a_b_e_l_=_l_a_t_e_s_t_%_2_0_r_e_l_e_a_s_e_&_s_t_y_l_e_=_f_o_r_-_t_h_e_-
        _b_a_d_g_e_&_l_o_g_o_=_g_i_t_h_u_b_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/
             _s_i_e_g_e_a_p_i_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_=_p_y_p_i_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_]
         _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_s_i_e_g_e_a_p_i_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-
 _b_a_d_g_e_&_l_o_g_o_=_p_y_t_h_o_n_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_&_c_o_l_o_r_=_y_e_l_l_o_w_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/
      _s_i_e_g_e_a_p_i_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_=_p_y_p_i_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_&_c_o_l_o_r_=_y_e_l_l_o_w_]
 ## How to install ```commandline pip install siegeapi ``` ## Quick example
 ```python from siegeapi import Auth import asyncio async def sample(): auth =
-Auth("UBI_EMAIL", "UBI_PASSWORD") player = await auth.get_player(uid="7e0f63df-
-a39b-44c5-8de0-d39a05926e77") print(f"Name: {player.name}") print(f"Profile pic
-URL: {player.profile_pic_url}") await player.load_playtime() print(f"Total Time
-Played: {player.total_time_played:,} seconds") print(f"Level: {player.level}")
+Auth(UBISOFT_EMAIL, UBISOFT_PASSW) player = await auth.get_player(name="CNDRD")
+print(f"Name: {player.name}") print(f"Profile pic URL:
+{player.profile_pic_url}") await player.load_persona() print(f"Streamer
+nickname: {player.persona.nickname}") print(f"Nickname enabled:
+{player.persona.enabled}") await player.load_playtime() print(f"Total Time
+Played: {player.total_time_played:,} seconds /
+{player.total_time_played_hours:,} hours") print(f"Level: {player.level}")
 await player.load_ranked_v2() print(f"Ranked Points:
 {player.ranked_profile.rank_points}") print(f"Rank:
 {player.ranked_profile.rank}") print(f"Max Rank Points:
 {player.ranked_profile.max_rank_points}") print(f"Max Rank:
 {player.ranked_profile.max_rank}") await player.load_progress() print(f"XP:
 {player.xp:,}") print(f"Total XP: {player.total_xp:,}") print(f"XP to level up:
-{player.xp_to_level_up:,}") await auth.close() asyncio.get_event_loop
-().run_until_complete(sample()) # Or `asyncio.run(sample())` ``` ### Output
-```text Name: CNDRD Profile pic URL: https://ubisoft-avatars.akamaized.net/
-7e0f63df-a39b-44c5-8de0-d39a05926e77/default_256_256.png Total Time Played:
-9,037,159 seconds Level: 305 Ranked Points: 4188 Rank: Diamond 4 Max Rank
-Points: 4289 Max Rank: Diamond 3 XP: 11,858 Total XP: 20,694,358 XP to level
-up: 131,642 ``` --- ## Siege Inventory If you want to see every skin, headgear,
-uniform and more, head over to **[skins.cndrd.xyz](https://skins.cndrd.xyz/)**
-## Docs For docs go to [cndrd.github.io/siegeapi](https://cndrd.github.io/
-siegeapi/) ## Credits Operator Icons from [r6operators][r6operators_] by
-[marcopixel][marcopixel_] & sourced by me straight from the game files Built
-(and re-built) on top of what [billy-yoyo][r6s_python_api] started ## Problems
-If you experience any problems, reach out to me, or submit a PR You can reach
-out here on GitHub or on Discord (_cndrd_) ![forthebadge](https://
-forthebadge.com/images/badges/works-on-my-machine.svg) ![forthebadge](https://
-forthebadge.com/images/badges/powered-by-energy-drinks.svg) [r6operators_]:
-https://github.com/marcopixel/r6operators [marcopixel_]: https://github.com/
-marcopixel [r6s_python_api]: https://github.com/billy-yoyo/RainbowSixSiege-
-Python-API
+{player.xp_to_level_up:,}") await auth.close() asyncio.run(sample()) ``` ###
+Output ```text Name: CNDRD Profile pic URL: https://ubisoft-
+avatars.akamaized.net/7e0f63df-a39b-44c5-8de0-d39a05926e77/default_256_256.png
+Streamer nickname: d1kCheeze Nickname enabled: True Total Time Played:
+9,265,890 seconds / 2,573 hours Level: 308 Ranked Points: 3919 Rank: Emerald 1
+Max Rank Points: 3933 Max Rank: Emerald 1 XP: 124,375 Total XP: 21,238,875 XP
+to level up: 20,625 ``` --- ## Siege Inventory If you want to see every skin,
+headgear, uniform and more, head over to **[skins.cndrd.xyz](https://
+skins.cndrd.xyz/)** ## Docs For docs go to [cndrd.github.io/siegeapi](https://
+cndrd.github.io/siegeapi/) ## Credits Operator Icons from [r6operators]
+[r6operators_] by [marcopixel][marcopixel_] & sourced by me straight from the
+game files Built (and re-built) on top of what [billy-yoyo][r6s_python_api]
+started ## Problems If you experience any problems, reach out to me, or submit
+a PR You can reach out here on GitHub or on Discord (_cndrd_) ![forthebadge]
+(https://forthebadge.com/images/badges/works-on-my-machine.svg) ![forthebadge]
+(https://forthebadge.com/images/badges/powered-by-energy-drinks.svg)
+[r6operators_]: https://github.com/marcopixel/r6operators [marcopixel_]: https:
+//github.com/marcopixel [r6s_python_api]: https://github.com/billy-yoyo/
+RainbowSixSiege-Python-API
```

### Comparing `siegeapi-6.2.5/siegeapi.egg-info/SOURCES.txt` & `siegeapi-6.3.0/siegeapi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 siegeapi/__init__.py
 siegeapi/auth.py
 siegeapi/default_stats.py
 siegeapi/exceptions.py
 siegeapi/linked_accounts.py
 siegeapi/maps.py
 siegeapi/operators.py
+siegeapi/persona.py
 siegeapi/player.py
 siegeapi/rank_profile.py
 siegeapi/ranks.py
 siegeapi/summaries.py
 siegeapi/trends.py
 siegeapi/url_builder.py
 siegeapi/utils.py
```

