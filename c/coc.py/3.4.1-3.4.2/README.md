# Comparing `tmp/coc.py-3.4.1.tar.gz` & `tmp/coc_py-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coc.py-3.4.1.tar", last modified: Sun Mar 31 12:44:28 2024, max compression
+gzip compressed data, was "coc_py-3.4.2.tar", last modified: Sat Apr 20 11:00:26 2024, max compression
```

## Comparing `coc.py-3.4.1.tar` & `coc_py-3.4.2.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 12:44:28.462712 coc.py-3.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-31 12:44:19.000000 coc.py-3.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-31 12:44:19.000000 coc.py-3.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-03-31 12:44:28.462712 coc.py-3.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-03-31 12:44:19.000000 coc.py-3.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 12:44:28.446712 coc.py-3.4.1/coc/
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15861 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/abc.py
--rw-r--r--   0 runner    (1001) docker     (127)    11863 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/clans.py
--rw-r--r--   0 runner    (1001) docker     (127)    83280 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9189 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/entry_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    39787 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    11319 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/events.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 12:44:28.442712 coc.py-3.4.1/coc/ext/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 12:44:28.450712 coc.py-3.4.1/coc/ext/discordlinks/
--rw-r--r--   0 runner    (1001) docker     (127)     9498 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/ext/discordlinks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 12:44:28.450712 coc.py-3.4.1/coc/ext/fullwarapi/
--rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/ext/fullwarapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 12:44:28.450712 coc.py-3.4.1/coc/ext/triggers/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/ext/triggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9699 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/ext/triggers/cron.py
--rw-r--r--   0 runner    (1001) docker     (127)    21909 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/ext/triggers/triggers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/hero.py
--rw-r--r--   0 runner    (1001) docker     (127)    23363 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/iterators.py
--rw-r--r--   0 runner    (1001) docker     (127)    21407 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/miscmodels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/player_clan.py
--rw-r--r--   0 runner    (1001) docker     (127)    30035 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/players.py
--rw-r--r--   0 runner    (1001) docker     (127)    19577 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/raid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/spell.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 12:44:28.458712 coc.py-3.4.1/coc/static/
--rw-r--r--   0 runner    (1001) docker     (127)  1285798 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/static/buildings.json
--rw-r--r--   0 runner    (1001) docker     (127)  1912944 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/static/characters.json
--rw-r--r--   0 runner    (1001) docker     (127)   203189 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/static/equipment.json
--rw-r--r--   0 runner    (1001) docker     (127)   647615 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/static/heroes.json
--rw-r--r--   0 runner    (1001) docker     (127)   255209 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/static/pets.json
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/static/spell_ids.json
--rw-r--r--   0 runner    (1001) docker     (127)   539861 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/static/spells.json
--rw-r--r--   0 runner    (1001) docker     (127)     8699 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/static/supers.json
--rw-r--r--   0 runner    (1001) docker     (127)  1006132 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/static/texts_EN.json
--rw-r--r--   0 runner    (1001) docker     (127)    91535 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/static/townhall_levels.json
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/static/troop_ids.json
--rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/static/update_static.py
--rw-r--r--   0 runner    (1001) docker     (127)     8451 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/troop.py
--rw-r--r--   0 runner    (1001) docker     (127)    19780 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4595 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/war_attack.py
--rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/war_clans.py
--rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/war_members.py
--rw-r--r--   0 runner    (1001) docker     (127)    19658 2024-03-31 12:44:19.000000 coc.py-3.4.1/coc/wars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 12:44:28.462712 coc.py-3.4.1/coc.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-03-31 12:44:28.000000 coc.py-3.4.1/coc.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-03-31 12:44:28.000000 coc.py-3.4.1/coc.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 12:44:28.000000 coc.py-3.4.1/coc.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-31 12:44:28.000000 coc.py-3.4.1/coc.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-31 12:44:28.000000 coc.py-3.4.1/coc.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-03-31 12:44:19.000000 coc.py-3.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-31 12:44:19.000000 coc.py-3.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 12:44:28.462712 coc.py-3.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-31 12:44:19.000000 coc.py-3.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 12:44:28.458712 coc.py-3.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-03-31 12:44:19.000000 coc.py-3.4.1/tests/test_capitalraidseasons.py
--rw-r--r--   0 runner    (1001) docker     (127)    12050 2024-03-31 12:44:19.000000 coc.py-3.4.1/tests/test_clans.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-03-31 12:44:19.000000 coc.py-3.4.1/tests/test_clash_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 12:44:19.000000 coc.py-3.4.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 12:44:19.000000 coc.py-3.4.1/tests/test_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 12:44:19.000000 coc.py-3.4.1/tests/test_login.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 12:44:19.000000 coc.py-3.4.1/tests/test_miscmodels.py
--rw-r--r--   0 runner    (1001) docker     (127)    10293 2024-03-31 12:44:19.000000 coc.py-3.4.1/tests/test_players.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-03-31 12:44:19.000000 coc.py-3.4.1/tests/test_troop_levels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-03-31 12:44:19.000000 coc.py-3.4.1/tests/test_wars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:00:26.560305 coc_py-3.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-20 11:00:22.000000 coc_py-3.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-20 11:00:22.000000 coc_py-3.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-04-20 11:00:26.560305 coc_py-3.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-04-20 11:00:22.000000 coc_py-3.4.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:00:26.544305 coc_py-3.4.2/coc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15861 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11863 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/clans.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83280 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9189 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/entry_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39787 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11319 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/events.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:00:26.536305 coc_py-3.4.2/coc/ext/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:00:26.544305 coc_py-3.4.2/coc/ext/discordlinks/
+-rw-r--r--   0 runner    (1001) docker     (127)     9498 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/ext/discordlinks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:00:26.544305 coc_py-3.4.2/coc/ext/fullwarapi/
+-rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/ext/fullwarapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:00:26.548305 coc_py-3.4.2/coc/ext/triggers/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/ext/triggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9699 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/ext/triggers/cron.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21909 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/ext/triggers/triggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/hero.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23363 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21407 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/miscmodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/player_clan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30035 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/players.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19577 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/raid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/spell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:00:26.556305 coc_py-3.4.2/coc/static/
+-rw-r--r--   0 runner    (1001) docker     (127)  1291668 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/static/buildings.json
+-rw-r--r--   0 runner    (1001) docker     (127)  1965460 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/static/characters.json
+-rw-r--r--   0 runner    (1001) docker     (127)   220960 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/static/equipment.json
+-rw-r--r--   0 runner    (1001) docker     (127)   648975 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/static/heroes.json
+-rw-r--r--   0 runner    (1001) docker     (127)   255626 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/static/pets.json
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/static/spell_ids.json
+-rw-r--r--   0 runner    (1001) docker     (127)   566845 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/static/spells.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8699 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/static/supers.json
+-rw-r--r--   0 runner    (1001) docker     (127)  1025147 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/static/texts_EN.json
+-rw-r--r--   0 runner    (1001) docker     (127)    92590 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/static/townhall_levels.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/static/troop_ids.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/static/update_static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8451 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/troop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19780 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4595 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/war_attack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/war_clans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/war_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19658 2024-04-20 11:00:22.000000 coc_py-3.4.2/coc/wars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:00:26.560305 coc_py-3.4.2/coc.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-04-20 11:00:26.000000 coc_py-3.4.2/coc.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-20 11:00:26.000000 coc_py-3.4.2/coc.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 11:00:26.000000 coc_py-3.4.2/coc.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-20 11:00:26.000000 coc_py-3.4.2/coc.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-20 11:00:26.000000 coc_py-3.4.2/coc.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-20 11:00:22.000000 coc_py-3.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-20 11:00:22.000000 coc_py-3.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 11:00:26.560305 coc_py-3.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-20 11:00:22.000000 coc_py-3.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 11:00:26.560305 coc_py-3.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-04-20 11:00:22.000000 coc_py-3.4.2/tests/test_capitalraidseasons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12050 2024-04-20 11:00:22.000000 coc_py-3.4.2/tests/test_clans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-20 11:00:22.000000 coc_py-3.4.2/tests/test_clash_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 11:00:22.000000 coc_py-3.4.2/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 11:00:22.000000 coc_py-3.4.2/tests/test_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 11:00:22.000000 coc_py-3.4.2/tests/test_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 11:00:22.000000 coc_py-3.4.2/tests/test_miscmodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10293 2024-04-20 11:00:22.000000 coc_py-3.4.2/tests/test_players.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-20 11:00:22.000000 coc_py-3.4.2/tests/test_troop_levels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-20 11:00:22.000000 coc_py-3.4.2/tests/test_wars.py
```

### Comparing `coc.py-3.4.1/LICENSE` & `coc_py-3.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `coc.py-3.4.1/PKG-INFO` & `coc_py-3.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coc.py
-Version: 3.4.1
+Version: 3.4.2
 Summary: A python wrapper for the Clash of Clans API
 Author: mathsman5133
 Maintainer: majordoobie, MagicTheDev, Kuchenmampfer, lukasthaler, doluk
 License: MIT
 Project-URL: documentation, https://cocpy.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/mathsman5133/coc.py
 Project-URL: changelog, https://cocpy.readthedocs.io/en/latest/miscellaneous/changelog.html
```

### Comparing `coc.py-3.4.1/README.rst` & `coc_py-3.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `coc.py-3.4.1/coc/__init__.py` & `coc_py-3.4.2/coc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-__version__ = "3.4.1"
+__version__ = "3.4.2"
 
 from .abc import BasePlayer, BaseClan
 from .clans import RankedClan, Clan
 from .client import Client
 from .events import PlayerEvents, ClanEvents, WarEvents, EventsClient, ClientEvents
 from .enums import (
     PlayerHouseElementType,
```

### Comparing `coc.py-3.4.1/coc/abc.py` & `coc_py-3.4.2/coc/abc.py`

 * *Files identical despite different names*

### Comparing `coc.py-3.4.1/coc/clans.py` & `coc_py-3.4.2/coc/clans.py`

 * *Files identical despite different names*

### Comparing `coc.py-3.4.1/coc/client.py` & `coc_py-3.4.2/coc/client.py`

 * *Files identical despite different names*

### Comparing `coc.py-3.4.1/coc/entry_logs.py` & `coc_py-3.4.2/coc/entry_logs.py`

 * *Files identical despite different names*

### Comparing `coc.py-3.4.1/coc/enums.py` & `coc_py-3.4.2/coc/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,14 +200,15 @@
     "Mighty Yak",
     "Unicorn",
     "Frosty",
     "Diggy",
     "Poison Lizard",
     "Phoenix",
     "Spirit Fox",
+    "Angry Jelly",
 ]
 
 EQUIPMENT = [
     "Barbarian Puppet",
     "Rage Vial",
     "Archer Puppet",
     "Invisibility Vial",
```

### Comparing `coc.py-3.4.1/coc/errors.py` & `coc_py-3.4.2/coc/errors.py`

 * *Files identical despite different names*

### Comparing `coc.py-3.4.1/coc/events.py` & `coc_py-3.4.2/coc/events.py`

 * *Files identical despite different names*

### Comparing `coc.py-3.4.1/coc/events.pyi` & `coc_py-3.4.2/coc/events.pyi`

 * *Files identical despite different names*

### Comparing `coc.py-3.4.1/coc/ext/discordlinks/__init__.py` & `coc_py-3.4.2/coc/ext/discordlinks/__init__.py`

 * *Files identical despite different names*

### Comparing `coc.py-3.4.1/coc/ext/fullwarapi/__init__.py` & `coc_py-3.4.2/coc/ext/fullwarapi/__init__.py`

 * *Files identical despite different names*

### Comparing `coc.py-3.4.1/coc/ext/triggers/cron.py` & `coc_py-3.4.2/coc/ext/triggers/cron.py`

 * *Files identical despite different names*

### Comparing `coc.py-3.4.1/coc/ext/triggers/triggers.py` & `coc_py-3.4.2/coc/ext/triggers/triggers.py`

 * *Files identical despite different names*

### Comparing `coc.py-3.4.1/coc/hero.py` & `coc_py-3.4.2/coc/hero.py`

 * *Files identical despite different names*

### Comparing `coc.py-3.4.1/coc/http.py` & `coc_py-3.4.2/coc/http.py`

 * *Files identical despite different names*

### Comparing `coc.py-3.4.1/coc/iterators.py` & `coc_py-3.4.2/coc/iterators.py`

 * *Files identical despite different names*

### Comparing `coc.py-3.4.1/coc/miscmodels.py` & `coc_py-3.4.2/coc/miscmodels.py`

 * *Files identical despite different names*

### Comparing `coc.py-3.4.1/coc/player_clan.py` & `coc_py-3.4.2/coc/player_clan.py`

 * *Files identical despite different names*

### Comparing `coc.py-3.4.1/coc/players.py` & `coc_py-3.4.2/coc/players.py`

 * *Files identical despite different names*

### Comparing `coc.py-3.4.1/coc/raid.py` & `coc_py-3.4.2/coc/raid.py`

 * *Files identical despite different names*

### Comparing `coc.py-3.4.1/coc/spell.py` & `coc_py-3.4.2/coc/spell.py`

 * *Files identical despite different names*

### Comparing `coc.py-3.4.1/coc/static/buildings.json` & `coc_py-3.4.2/coc/static/buildings.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992350574428515%*

 * *Differences: {"'Air Blaster'": "{'StrengthWeight': [678, 840, 1003, 1165, 1328, 1490, 1653]}",*

 * * "'Air Defense'": "{'StrengthWeight': [500, 656, 813, 919, 1075, 1281, 1538, 1751, 1963, 2175, "*

 * *                  '2388, 2706, 2919, 3231]}',*

 * * "'Alliance Castle'": "{'BuildingLevel': {insert: [(11, 12)]}, 'TID': {insert: [(0, "*

 * *                      "'TID_BUILDING_ALLIANCE_CASTLE')]}, 'InfoTID': {insert: [(0, "*

 * *                      "'TID_ALLIANCE_CASTLE_INFO')]}, 'BuildingClass': {insert: [(0, 'Army')]}, "*

 * *                   […]*

```diff
@@ -521,21 +521,21 @@
         "SpeedMod": [],
         "SpellOnNearbyDamage": [],
         "Stage": [],
         "StartUpgradeBoosterCost": [],
         "StartingHomeCount": [],
         "StatusEffectTime": [],
         "StrengthWeight": [
-            20,
-            20,
-            20,
-            20,
-            20,
-            20,
-            20
+            678,
+            840,
+            1003,
+            1165,
+            1328,
+            1490,
+            1653
         ],
         "TID": [
             "TID_AIR_BLASTER",
             "TID_AIR_BLASTER",
             "TID_AIR_BLASTER",
             "TID_AIR_BLASTER",
             "TID_AIR_BLASTER",
@@ -1314,28 +1314,28 @@
         "SpeedMod": [],
         "SpellOnNearbyDamage": [],
         "Stage": [],
         "StartUpgradeBoosterCost": [],
         "StartingHomeCount": [],
         "StatusEffectTime": [],
         "StrengthWeight": [
-            50,
-            50,
-            50,
-            50,
-            50,
-            50,
-            50,
-            50,
-            50,
-            50,
-            50,
-            50,
-            50,
-            50
+            500,
+            656,
+            813,
+            919,
+            1075,
+            1281,
+            1538,
+            1751,
+            1963,
+            2175,
+            2388,
+            2706,
+            2919,
+            3231
         ],
         "TID": [
             "TID_BUILDING_AIR_DEFENSE",
             "TID_BUILDING_AIR_DEFENSE",
             "TID_BUILDING_AIR_DEFENSE",
             "TID_BUILDING_AIR_DEFENSE",
             "TID_BUILDING_AIR_DEFENSE",
@@ -2818,144 +2818,155 @@
             1200000,
             2500000,
             4200000,
             5500000,
             8000000,
             10000000,
             12600000,
-            20000000
+            20000000,
+            21000000
         ],
         "BuildResource": [
             "Elixir",
             "Elixir",
             "Elixir",
             "Elixir",
             "Elixir",
             "Elixir",
             "Elixir",
             "Elixir",
             "Elixir",
             "Elixir",
+            "Elixir",
             "Elixir"
         ],
         "BuildTimeD": [
             0,
             0,
             0,
             1,
             2,
             5,
             6,
             9,
             11,
             13,
-            14
+            14,
+            15
         ],
         "BuildTimeH": [
             0,
             8,
             12,
             0,
             0,
             0,
             6,
             0,
             0,
             0,
-            0
+            0,
+            12
         ],
         "BuildTimeM": [
             0,
             0,
             0,
             0,
             0,
             0,
             0,
             0,
             0,
             0,
+            0,
             0
         ],
         "BuildTimeS": [
             0,
             0,
             0,
             0,
             0,
             0,
             0,
             0,
             0,
             0,
+            0,
             0
         ],
         "BuildingClass": [
             "Army",
             "Army",
             "Army",
             "Army",
             "Army",
             "Army",
             "Army",
             "Army",
             "Army",
             "Army",
+            "Army",
             "Army"
         ],
         "BuildingH": [
             2,
             2,
             2,
             2,
             2,
             2,
             2,
             2,
             2,
             2,
+            2,
             2
         ],
         "BuildingLevel": [
             1,
             2,
             3,
             4,
             5,
             6,
             7,
             8,
             9,
             10,
-            11
+            11,
+            12
         ],
         "BuildingW": [
             2,
             2,
             2,
             2,
             2,
             2,
             2,
             2,
             2,
             2,
+            2,
             2
         ],
         "Bunker": [
             true,
             true,
             true,
             true,
             true,
             true,
             true,
             true,
             true,
             true,
+            true,
             true
         ],
         "BurstCount": [],
         "BurstDelay": [],
         "CapitalHallLevel": [
             3,
             4,
@@ -2963,15 +2974,16 @@
             8,
             9,
             10,
             11,
             12,
             13,
             14,
-            15
+            15,
+            16
         ],
         "ChainAttackDamageReductionPercent": [],
         "ChainAttackDelay": [],
         "ChainAttackDistance": [],
         "ChainAttackMaxTargets": [],
         "CombatActivationDelay": [],
         "CombatActivationEffect": [],
@@ -3005,14 +3017,15 @@
             "Building Destroyed",
             "Building Destroyed",
             "Building Destroyed",
             "Building Destroyed",
             "Building Destroyed",
             "Building Destroyed",
             "Building Destroyed",
+            "Building Destroyed",
             "Building Destroyed"
         ],
         "DestructionXP": [],
         "DieDamage": [],
         "DieDamageDelay": [],
         "DieDamageEffect": [],
         "DieDamageRadius": [],
@@ -3024,27 +3037,29 @@
             "alliance_castle_lvl4",
             "alliance_castle_lvl5",
             "alliance_castle_lvl6",
             "alliance_castle_lvl7",
             "alliance_castle_lvl8",
             "alliance_castle_lvl9",
             "alliance_castle_lvl10",
-            "alliance_castle_lvl11"
+            "alliance_castle_lvl11",
+            "alliance_castle_lvl12"
         ],
         "ExportNameBase": [
             "alliance_castle_base",
             "alliance_castle_base",
             "alliance_castle_base",
             "alliance_castle_base",
             "alliance_castle_base",
             "alliance_castle_base",
             "alliance_castle_base",
             "alliance_castle_base",
             "alliance_castle_base",
             "alliance_castle_base",
+            "alliance_castle_base",
             "alliance_castle_base"
         ],
         "ExportNameBeamEnd": [],
         "ExportNameBeamStart": [],
         "ExportNameBuildAnim": [
             "alliance_castle_upg",
             "alliance_castle_upg",
@@ -3052,54 +3067,58 @@
             "alliance_castle_upg",
             "alliance_castle_upg",
             "alliance_castle_upg",
             "alliance_castle_upg",
             "alliance_castle_upg",
             "alliance_castle_upg",
             "alliance_castle_upg",
+            "alliance_castle_upg",
             "alliance_castle_upg"
         ],
         "ExportNameConstruction": [
             "generic_construction_state3",
             "generic_construction_state3",
             "generic_construction_state3",
             "generic_construction_state3",
             "generic_construction_state3",
             "generic_construction_state3",
             "generic_construction_state3",
             "generic_construction_state3",
             "generic_construction_state3",
             "generic_construction_state3",
+            "generic_construction_state3",
             "generic_construction_state3"
         ],
         "ExportNameDamaged": [
             "alliance_castle_lvl1_broken",
             "alliance_castle_lvl1_broken",
             "alliance_castle_lvl1_broken",
             "alliance_castle_lvl1_broken",
             "alliance_castle_lvl1_broken",
             "alliance_castle_lvl1_broken",
             "alliance_castle_lvl1_broken",
             "alliance_castle_lvl1_broken",
             "alliance_castle_lvl1_broken",
             "alliance_castle_lvl1_broken",
+            "alliance_castle_lvl1_broken",
             "alliance_castle_lvl1_broken"
         ],
         "ExportNameDamagedSWF": [],
         "ExportNameLocked": [
             "alliance_castle_lvl1_broken",
             "alliance_castle_lvl1_broken",
             "alliance_castle_lvl1_broken",
             "alliance_castle_lvl1_broken",
             "alliance_castle_lvl1_broken",
             "alliance_castle_lvl1_broken",
             "alliance_castle_lvl1_broken",
             "alliance_castle_lvl1_broken",
             "alliance_castle_lvl1_broken",
             "alliance_castle_lvl1_broken",
+            "alliance_castle_lvl1_broken",
             "alliance_castle_lvl1_broken"
         ],
         "ExportNameNpc": [],
         "ExportNameTriggered": [],
         "ExportNameUpgradeAnim": [],
         "ForgesMiniSpells": [],
         "ForgesSpells": [],
@@ -3121,14 +3140,15 @@
             3,
             3,
             3,
             3,
             3,
             3,
             3,
+            3,
             3
         ],
         "HeroType": [],
         "Hidden": [],
         "HintPriority": [
             900,
             900,
@@ -3136,14 +3156,15 @@
             900,
             900,
             900,
             900,
             900,
             900,
             900,
+            900,
             900
         ],
         "HitEffect": [],
         "HitEffect2": [],
         "HitSpell": [],
         "HitSpellLevel": [],
         "Hitpoints": [
@@ -3153,68 +3174,73 @@
             2600,
             3000,
             3400,
             4000,
             4400,
             4800,
             5200,
-            5400
+            5400,
+            5600
         ],
         "HousingSpace": [
             10,
             15,
             20,
             25,
             30,
             35,
             35,
             40,
             45,
             45,
+            50,
             50
         ],
         "HousingSpaceAlt": [
             0,
             0,
             0,
             1,
             1,
             1,
             2,
             2,
             2,
             3,
+            3,
             3
         ],
         "HousingSpaceSiege": [
             0,
             0,
             0,
             0,
             0,
             1,
             1,
             1,
             1,
             1,
-            1
+            1,
+            2
         ],
         "Icon": [],
         "IncreasingDamage": [],
         "InfoTID": [
             "TID_ALLIANCE_CASTLE_INFO",
             "TID_ALLIANCE_CASTLE_INFO",
             "TID_ALLIANCE_CASTLE_INFO",
             "TID_ALLIANCE_CASTLE_INFO",
             "TID_ALLIANCE_CASTLE_INFO",
             "TID_ALLIANCE_CASTLE_INFO",
             "TID_ALLIANCE_CASTLE_INFO",
             "TID_ALLIANCE_CASTLE_INFO",
             "TID_ALLIANCE_CASTLE_INFO",
             "TID_ALLIANCE_CASTLE_INFO",
+            "TID_ALLIANCE_CASTLE_INFO",
             "TID_ALLIANCE_CASTLE_INFO"
         ],
         "IsHeroBarrack": [],
         "IsRed": [],
         "LevelRequirementTID": [],
         "LoadAmmoEffect": [],
         "Locked": [
@@ -3224,27 +3250,29 @@
             true,
             true,
             true,
             true,
             true,
             true,
             true,
+            true,
             true
         ],
         "LootOnDestruction": [
             true,
             true,
             true,
             true,
             true,
             true,
             true,
             true,
             true,
             true,
+            true,
             true
         ],
         "Lv2SwitchTime": [],
         "Lv3SwitchTime": [],
         "MaxStoredCommonOre": [],
         "MaxStoredDarkElixir": [],
         "MaxStoredElixir": [],
@@ -3261,41 +3289,44 @@
             4000,
             8000,
             10000,
             12000,
             14000,
             16000,
             18000,
-            20000
+            20000,
+            22000
         ],
         "MaxStoredWarElixir": [
             75000,
             250000,
             700000,
             1000000,
             1600000,
             2000000,
             2400000,
             2800000,
             3200000,
             3600000,
-            4000000
+            4000000,
+            4400000
         ],
         "MaxStoredWarGold": [
             75000,
             250000,
             700000,
             1000000,
             1600000,
             2000000,
             2400000,
             2800000,
             3200000,
             3600000,
-            4000000
+            4000000,
+            4400000
         ],
         "MergeRequirement": [],
         "MinAttackRange": [],
         "MultiHitsTarget": [],
         "MultiTargets": [],
         "Name": [],
         "NeedsAim": [],
@@ -3315,27 +3346,29 @@
             "Alliance Castle Pickup",
             "Alliance Castle Pickup",
             "Alliance Castle Pickup",
             "Alliance Castle Pickup",
             "Alliance Castle Pickup",
             "Alliance Castle Pickup",
             "Alliance Castle Pickup",
+            "Alliance Castle Pickup",
             "Alliance Castle Pickup"
         ],
         "PlacingEffect": [
             "Alliance Castle Placing",
             "Alliance Castle Placing",
             "Alliance Castle Placing",
             "Alliance Castle Placing",
             "Alliance Castle Placing",
             "Alliance Castle Placing",
             "Alliance Castle Placing",
             "Alliance Castle Placing",
             "Alliance Castle Placing",
             "Alliance Castle Placing",
+            "Alliance Castle Placing",
             "Alliance Castle Placing"
         ],
         "PreAttackEffect": [],
         "PreferredTarget": [],
         "PreferredTargetDamageMod": [],
         "PrepareSpeed": [],
         "PreventsHealing": [],
@@ -3346,14 +3379,15 @@
             "ClanCastleTH7",
             "ClanCastleTH7",
             "ClanCastleTH7",
             "ClanCastleTH11",
             "ClanCastleTH11",
             "ClanCastleTH11",
             "ClanCastleTH11",
+            "ClanCastleTH11",
             "ClanCastleTH11"
         ],
         "ProducesResource": [],
         "ProducesUnitsOfType": [],
         "Projectile": [],
         "ProjectileBounces": [],
         "ProjectileVariantByTargetMaxHP": [],
@@ -3368,14 +3402,15 @@
             30,
             30,
             30,
             30,
             30,
             30,
             30,
+            30,
             30
         ],
         "ResourceIconLimit": [],
         "ResourceMax": [],
         "ResourcePer100Hours": [],
         "SWF": [
             "sc/buildings.sc",
@@ -3384,27 +3419,29 @@
             "sc/buildings.sc",
             "sc/buildings.sc",
             "sc/buildings.sc",
             "sc/buildings.sc",
             "sc/buildings.sc",
             "sc/buildings.sc",
             "sc/buildings.sc",
+            "sc/buildings.sc",
             "sc/buildings.sc"
         ],
         "SecondaryTargetingClass": [
             "Resource",
             "Resource",
             "Resource",
             "Resource",
             "Resource",
             "Resource",
             "Resource",
             "Resource",
             "Resource",
             "Resource",
+            "Resource",
             "Resource"
         ],
         "SecondaryTroop": [],
         "SecondaryTroopCnt": [],
         "SecondaryTroopLvl": [],
         "SelfAsAoeCenter": [],
         "ShareHeroCombatData": [],
@@ -3423,29 +3460,44 @@
             1,
             1,
             1,
             1,
             1,
             1,
             1,
+            1,
             1
         ],
         "StatusEffectTime": [],
-        "StrengthWeight": [],
+        "StrengthWeight": [
+            200,
+            400,
+            600,
+            800,
+            2000,
+            2400,
+            4200,
+            4800,
+            5400,
+            6000,
+            6600,
+            7200
+        ],
         "TID": [
             "TID_BUILDING_ALLIANCE_CASTLE",
             "TID_BUILDING_ALLIANCE_CASTLE",
             "TID_BUILDING_ALLIANCE_CASTLE",
             "TID_BUILDING_ALLIANCE_CASTLE",
             "TID_BUILDING_ALLIANCE_CASTLE",
             "TID_BUILDING_ALLIANCE_CASTLE",
             "TID_BUILDING_ALLIANCE_CASTLE",
             "TID_BUILDING_ALLIANCE_CASTLE",
             "TID_BUILDING_ALLIANCE_CASTLE",
             "TID_BUILDING_ALLIANCE_CASTLE",
+            "TID_BUILDING_ALLIANCE_CASTLE",
             "TID_BUILDING_ALLIANCE_CASTLE"
         ],
         "TargetGroups": [],
         "TargetGroupsRadius": [],
         "TargetingConeAngle": [],
         "ToggleAttackModeEffect": [],
         "TownHallLevel": [
@@ -3455,15 +3507,16 @@
             8,
             9,
             10,
             11,
             12,
             13,
             14,
-            15
+            15,
+            16
         ],
         "TransitionEffectLv2": [],
         "TransitionEffectLv3": [],
         "TriggerRadius": [],
         "TurnSpeed": [],
         "UnitProduction": [],
         "UnlockWeaponMode": [],
@@ -3482,14 +3535,15 @@
             3,
             3,
             3,
             3,
             3,
             3,
             3,
+            3,
             3
         ]
     },
     "Ancient Artillery": {
         "AOESpell": [],
         "AOESpellAlternate": [],
         "ActivateCombatOnDamageTaken": [],
@@ -3497,14 +3551,15 @@
         "AimRotateStep": [],
         "AirTargets": [
             true,
             true,
             true,
             true,
             true,
+            true,
             true
         ],
         "AltAirTargets": [],
         "AltAttackMode": [],
         "AltAttackRange": [],
         "AltAttackSpeed": [],
         "AltBuildResource": [],
@@ -3520,221 +3575,244 @@
         "AlternatePickNewTargetDelay": [],
         "AmmoCost": [
             35000,
             40000,
             45000,
             50000,
             55000,
-            60000
+            60000,
+            65000
         ],
         "AmmoCount": [
             30,
             30,
             30,
             30,
             30,
+            30,
             30
         ],
         "AmmoResource": [
             "Elixir",
             "Elixir",
             "Elixir",
             "Elixir",
             "Elixir",
+            "Elixir",
             "Elixir"
         ],
         "AmountCanBeUpgraded": [],
         "AnimateTurret": [],
         "AnimationActionFrame": [],
         "AppearEffect": [],
         "ArmySlotType": [],
         "AttackEffect": [
             "Artillery Attack",
             "Artillery Attack",
             "Artillery Attack",
             "Artillery Attack",
             "Artillery Attack",
+            "Artillery Attack",
             "Artillery Attack"
         ],
         "AttackEffect2": [],
         "AttackEffectAlt": [],
         "AttackEffectLv2": [],
         "AttackEffectLv3": [],
         "AttackRange": [
             5000,
             5000,
             5000,
             5000,
             5000,
+            5000,
             5000
         ],
         "AttackSpeed": [
             10000,
             10000,
             10000,
             10000,
             10000,
+            10000,
             10000
         ],
         "BaseGfx": [],
         "Blacksmith": [],
         "BlueAdd": [],
         "BlueMul": [],
         "BoostCost": [],
         "BuildCost": [
             6000000,
             8000000,
             10000000,
             13000000,
             17000000,
-            21500000
+            21500000,
+            22000000
         ],
         "BuildResource": [
             "Gold",
             "Gold",
             "Gold",
             "Gold",
             "Gold",
+            "Gold",
             "Gold"
         ],
         "BuildTimeD": [
             5,
             5,
             9,
             10,
             13,
-            14
+            14,
+            15
         ],
         "BuildTimeH": [
             0,
             0,
             0,
             0,
             0,
-            0
+            0,
+            12
         ],
         "BuildTimeM": [
             0,
             0,
             0,
             0,
             0,
+            0,
             0
         ],
         "BuildTimeS": [
             0,
             0,
             0,
             0,
             0,
+            0,
             0
         ],
         "BuildingClass": [
             "Defense",
             "Defense",
             "Defense",
             "Defense",
             "Defense",
+            "Defense",
             "Defense"
         ],
         "BuildingH": [
             3,
             3,
             3,
             3,
             3,
+            3,
             3
         ],
         "BuildingLevel": [
             1,
             2,
             3,
             4,
             5,
-            6
+            6,
+            7
         ],
         "BuildingW": [
             3,
             3,
             3,
             3,
             3,
+            3,
             3
         ],
         "Bunker": [],
         "BurstCount": [
             3,
             3,
             3,
             3,
             3,
+            3,
             3
         ],
         "BurstDelay": [
             750,
             750,
             750,
             750,
             750,
+            750,
             750
         ],
         "CapitalHallLevel": [
             11,
             11,
             12,
             13,
             14,
-            15
+            15,
+            16
         ],
         "ChainAttackDamageReductionPercent": [],
         "ChainAttackDelay": [],
         "ChainAttackDistance": [],
         "ChainAttackMaxTargets": [],
         "CombatActivationDelay": [],
         "CombatActivationEffect": [],
         "CoolDownOverride": [
             6992,
             6992,
             6992,
             6992,
             6992,
+            6992,
             6992
         ],
         "CustomTargetHitBuildingInRange": [],
         "DPS": [
             0,
             0,
             0,
             0,
             0,
+            0,
             0
         ],
         "DPSLv2": [],
         "DPSLv3": [],
         "Damage": [
             20,
             25,
             30,
             35,
             40,
-            45
+            45,
+            50
         ],
         "Damage2": [],
         "Damage2Delay": [],
         "Damage2FalloffEnd": [],
         "Damage2FalloffStart": [],
         "Damage2Min": [],
         "Damage2Radius": [],
         "DamagePermilHp": [],
         "DamageRadius": [
             300,
             300,
             300,
             300,
             300,
+            300,
             300
         ],
         "DefaultProjectileVariant": [],
         "DefenceTroopCharacter": [],
         "DefenceTroopCharacter2": [],
         "DefenceTroopCount": [],
         "DefenceTroopLevel": [],
@@ -3744,88 +3822,97 @@
         "DestroyDamageEffect": [],
         "DestroyEffect": [
             "Building Destroyed",
             "Building Destroyed",
             "Building Destroyed",
             "Building Destroyed",
             "Building Destroyed",
+            "Building Destroyed",
             "Building Destroyed"
         ],
         "DestructionXP": [],
         "DieDamage": [],
         "DieDamageDelay": [],
         "DieDamageEffect": [],
         "DieDamageRadius": [],
         "DummyProjectileCount": [],
         "ExportName": [
             "doom_cannon_lvl1",
             "doom_cannon_lvl2",
             "doom_cannon_lvl3",
             "doom_cannon_lvl4",
             "doom_cannon_lvl5",
-            "doom_cannon_lvl6"
+            "doom_cannon_lvl6",
+            "doom_cannon_lvl7"
         ],
         "ExportNameBase": [
             "laboratory_base",
             "laboratory_base",
             "laboratory_base",
             "laboratory_base",
             "laboratory_base",
+            "laboratory_base",
             "laboratory_base"
         ],
         "ExportNameBeamEnd": [
             "beam_down",
             "beam_down",
             "beam_down",
             "beam_down",
             "beam_down",
+            "beam_down",
             "beam_down"
         ],
         "ExportNameBeamStart": [
             "beam_up",
             "beam_up",
             "beam_up",
             "beam_up",
             "beam_up",
+            "beam_up",
             "beam_up"
         ],
         "ExportNameBuildAnim": [
             "laboratory_upg",
             "laboratory_upg",
             "laboratory_upg",
             "laboratory_upg",
             "laboratory_upg",
+            "laboratory_upg",
             "laboratory_upg"
         ],
         "ExportNameConstruction": [
             "laboratory_const",
             "laboratory_const",
             "laboratory_const",
             "laboratory_const",
             "laboratory_const",
+            "laboratory_const",
             "laboratory_const"
         ],
         "ExportNameDamaged": [
             "destroyedBuilding_4m_base_rock",
             "destroyedBuilding_4m_base_rock",
             "destroyedBuilding_4m_base_rock",
             "destroyedBuilding_4m_base_rock",
             "destroyedBuilding_4m_base_rock",
+            "destroyedBuilding_4m_base_rock",
             "destroyedBuilding_4m_base_rock"
         ],
         "ExportNameDamagedSWF": [],
         "ExportNameLocked": [],
         "ExportNameNpc": [],
         "ExportNameTriggered": [],
         "ExportNameUpgradeAnim": [
             "doom_cannon_lvl1_upgrade",
             "doom_cannon_lvl2_upgrade",
             "doom_cannon_lvl3_upgrade",
             "doom_cannon_lvl4_upgrade",
             "doom_cannon_lvl5_upgrade",
+            "doom_cannon_lvl6_upgrade",
             "doom_cannon_lvl6_upgrade"
         ],
         "ForgesMiniSpells": [],
         "ForgesSpells": [],
         "FreeBoost": [],
         "GearUpBuilding": [],
         "GearUpCost": [],
@@ -3837,76 +3924,83 @@
         "GreenMul": [],
         "GroundTargets": [
             true,
             true,
             true,
             true,
             true,
+            true,
             true
         ],
         "HealthRecoveryPercent": [],
         "Height": [
             4,
             4,
             4,
             4,
             4,
+            4,
             4
         ],
         "HeroType": [],
         "Hidden": [],
         "HintPriority": [
             150,
             150,
             150,
             150,
             150,
+            150,
             150
         ],
         "HitEffect": [
             "Ancient Hit",
             "Ancient Hit",
             "Ancient Hit",
             "Ancient Hit",
             "Ancient Hit",
+            "Ancient Hit",
             "Ancient Hit"
         ],
         "HitEffect2": [],
         "HitSpell": [],
         "HitSpellLevel": [],
         "Hitpoints": [
             4000,
             4400,
             4800,
             5200,
             5600,
-            5900
+            5900,
+            6200
         ],
         "HousingSpace": [],
         "HousingSpaceAlt": [],
         "HousingSpaceSiege": [],
         "Icon": [],
         "IncreasingDamage": [],
         "InfoTID": [
             "TID_ARTILLERY_INFO",
             "TID_ARTILLERY_INFO",
             "TID_ARTILLERY_INFO",
             "TID_ARTILLERY_INFO",
             "TID_ARTILLERY_INFO",
+            "TID_ARTILLERY_INFO",
             "TID_ARTILLERY_INFO"
         ],
         "IsHeroBarrack": [],
         "IsRed": [],
         "LevelRequirementTID": [],
         "LoadAmmoEffect": [
             "Artillery Load",
             "Artillery Load",
             "Artillery Load",
             "Artillery Load",
             "Artillery Load",
+            "Artillery Load",
             "Artillery Load"
         ],
         "Locked": [],
         "LootOnDestruction": [],
         "Lv2SwitchTime": [],
         "Lv3SwitchTime": [],
         "MaxStoredCommonOre": [],
@@ -3924,27 +4018,29 @@
         "MergeRequirement": [],
         "MinAttackRange": [
             700,
             700,
             700,
             700,
             700,
+            700,
             700
         ],
         "MultiHitsTarget": [],
         "MultiTargets": [],
         "Name": [],
         "NeedsAim": [],
         "NewTargetAttackDelay": [],
         "NoAmmoEffect": [
             "Artillery No Ammo",
             "Artillery No Ammo",
             "Artillery No Ammo",
             "Artillery No Ammo",
             "Artillery No Ammo",
+            "Artillery No Ammo",
             "Artillery No Ammo"
         ],
         "NumMultiTargets": [],
         "PenetratingExtraRange": [],
         "PenetratingProjectile": [],
         "PenetratingRadius": [],
         "PercentageStoredDarkElixir": [],
@@ -3952,84 +4048,92 @@
         "PercentageStoredGold": [],
         "PickUpEffect": [
             "Basic Turret Pickup",
             "Basic Turret Pickup",
             "Basic Turret Pickup",
             "Basic Turret Pickup",
             "Basic Turret Pickup",
+            "Basic Turret Pickup",
             "Basic Turret Pickup"
         ],
         "PlacingEffect": [
             "Artillery Placing",
             "Artillery Placing",
             "Artillery Placing",
             "Artillery Placing",
             "Artillery Placing",
+            "Artillery Placing",
             "Artillery Placing"
         ],
         "PreAttackEffect": [
             "Artillery PreAttack",
             "Artillery PreAttack",
             "Artillery PreAttack",
             "Artillery PreAttack",
             "Artillery PreAttack",
+            "Artillery PreAttack",
             "Artillery PreAttack"
         ],
         "PreferredTarget": [],
         "PreferredTargetDamageMod": [],
         "PrepareSpeed": [],
         "PreventsHealing": [],
         "PreviewScenario": [
             "AncientArtillery",
             "AncientArtillery",
             "AncientArtillery",
             "AncientArtillery",
             "AncientArtillery",
+            "AncientArtillery",
             "AncientArtillery"
         ],
         "ProducesResource": [],
         "ProducesUnitsOfType": [],
         "Projectile": [
             "Artillery Ammo1",
             "Artillery Ammo2",
             "Artillery Ammo3",
             "Artillery Ammo4",
             "Artillery Ammo5",
-            "Artillery Ammo6"
+            "Artillery Ammo6",
+            "Artillery Ammo7"
         ],
         "ProjectileBounces": [],
         "ProjectileVariantByTargetMaxHP": [],
         "PushBack": [
             50,
             50,
             50,
             50,
             50,
+            50,
             50
         ],
         "RandomHitPosition": [],
         "RedAdd": [],
         "RedMul": [],
         "RegenTime": [
             20,
             21,
             21,
             21,
             21,
+            21,
             21
         ],
         "ResourceIconLimit": [],
         "ResourceMax": [],
         "ResourcePer100Hours": [],
         "SWF": [
             "sc/buildings.sc",
             "sc/buildings.sc",
             "sc/buildings.sc",
             "sc/buildings.sc",
             "sc/buildings.sc",
+            "sc/buildings.sc",
             "sc/buildings.sc"
         ],
         "SecondaryTargetingClass": [],
         "SecondaryTroop": [],
         "SecondaryTroopCnt": [],
         "SecondaryTroopLvl": [],
         "SelfAsAoeCenter": [],
@@ -4041,54 +4145,59 @@
         "SpeedMod": [],
         "SpellOnNearbyDamage": [],
         "Stage": [],
         "StartUpgradeBoosterCost": [],
         "StartingHomeCount": [],
         "StatusEffectTime": [],
         "StrengthWeight": [
-            4900,
-            4450,
-            4100,
-            3800,
-            3550,
-            3400
+            58800,
+            60075,
+            61500,
+            62700,
+            63900,
+            65450,
+            67000
         ],
         "TID": [
             "TID_BUILDING_ARTILLERY",
             "TID_BUILDING_ARTILLERY",
             "TID_BUILDING_ARTILLERY",
             "TID_BUILDING_ARTILLERY",
             "TID_BUILDING_ARTILLERY",
+            "TID_BUILDING_ARTILLERY",
             "TID_BUILDING_ARTILLERY"
         ],
         "TargetGroups": [
             true,
             true,
             true,
             true,
             true,
+            true,
             true
         ],
         "TargetGroupsRadius": [
             500,
             500,
             500,
             500,
             500,
+            500,
             500
         ],
         "TargetingConeAngle": [],
         "ToggleAttackModeEffect": [],
         "TownHallLevel": [
             11,
             11,
             12,
             13,
             14,
-            15
+            15,
+            16
         ],
         "TransitionEffectLv2": [],
         "TransitionEffectLv3": [],
         "TriggerRadius": [],
         "TurnSpeed": [],
         "UnitProduction": [],
         "UnlockWeaponMode": [],
@@ -4098,32 +4207,35 @@
         "VillageType": [],
         "WakeUpSpace": [
             200,
             200,
             200,
             200,
             200,
+            200,
             200
         ],
         "WakeUpSpeed": [
             1125,
             1125,
             1125,
             1125,
             1125,
+            1125,
             1125
         ],
         "WallCornerPieces": [],
         "Weapon": [],
         "Width": [
             4,
             4,
             4,
             4,
             4,
+            4,
             4
         ]
     },
     "Archer Tower": {
         "AOESpell": [],
         "AOESpellAlternate": [],
         "ActivateCombatOnDamageTaken": [],
@@ -5210,16 +5322,16 @@
             750,
             810,
             890,
             970,
             1050,
             1130,
             1230,
-            1330,
-            1410,
+            1310,
+            1390,
             1510,
             1600,
             1700,
             1800
         ],
         "HousingSpace": [],
         "HousingSpaceAlt": [],
@@ -5451,35 +5563,35 @@
         "SpeedMod": [],
         "SpellOnNearbyDamage": [],
         "Stage": [],
         "StartUpgradeBoosterCost": [],
         "StartingHomeCount": [],
         "StatusEffectTime": [],
         "StrengthWeight": [
-            100,
-            99,
-            98,
-            97,
-            96,
-            95,
-            94,
-            93,
-            92,
-            91,
-            90,
-            89,
-            88,
-            87,
-            85,
-            83,
-            83,
-            83,
-            83,
-            83,
-            83
+            205,
+            252,
+            299,
+            364,
+            418,
+            470,
+            543,
+            607,
+            688,
+            758,
+            830,
+            883,
+            935,
+            1029,
+            1111,
+            1147,
+            1206,
+            1309,
+            1411,
+            1498,
+            1577
         ],
         "TID": [
             "TID_BUILDING_ARCHER_TOWER",
             "TID_BUILDING_ARCHER_TOWER",
             "TID_BUILDING_ARCHER_TOWER",
             "TID_BUILDING_ARCHER_TOWER",
             "TID_BUILDING_ARCHER_TOWER",
@@ -8889,25 +9001,25 @@
         "SpeedMod": [],
         "SpellOnNearbyDamage": [],
         "Stage": [],
         "StartUpgradeBoosterCost": [],
         "StartingHomeCount": [],
         "StatusEffectTime": [],
         "StrengthWeight": [
-            400,
-            420,
-            440,
-            460,
-            460,
-            460,
-            460,
-            460,
-            460,
-            460,
-            460
+            1610,
+            1911,
+            2233,
+            2818,
+            3416,
+            4071,
+            4784,
+            5497,
+            6509,
+            7199,
+            7889
         ],
         "TID": [
             "TID_BUILDING_BOMB_TOWER",
             "TID_BUILDING_BOMB_TOWER",
             "TID_BUILDING_BOMB_TOWER",
             "TID_BUILDING_BOMB_TOWER",
             "TID_BUILDING_BOMB_TOWER",
@@ -9741,25 +9853,25 @@
         "SpeedMod": [],
         "SpellOnNearbyDamage": [],
         "Stage": [],
         "StartUpgradeBoosterCost": [],
         "StartingHomeCount": [],
         "StatusEffectTime": [],
         "StrengthWeight": [
-            350,
-            325,
-            300,
-            300,
-            300,
-            300,
-            300,
-            300,
-            300,
-            300,
-            300
+            3413,
+            3819,
+            4125,
+            4725,
+            5625,
+            6450,
+            7275,
+            8100,
+            8850,
+            9450,
+            10200
         ],
         "TID": [
             "TID_BUILDING_BOW",
             "TID_BUILDING_BOW",
             "TID_BUILDING_BOW",
             "TID_BUILDING_BOW",
             "TID_BUILDING_BOW",
@@ -11841,35 +11953,35 @@
         "SpeedMod": [],
         "SpellOnNearbyDamage": [],
         "Stage": [],
         "StartUpgradeBoosterCost": [],
         "StartingHomeCount": [],
         "StatusEffectTime": [],
         "StrengthWeight": [
-            100,
-            99,
-            98,
-            97,
-            96,
-            95,
-            94,
-            93,
-            91,
-            89,
-            87,
-            85,
-            83,
-            81,
-            79,
-            77,
-            77,
-            77,
-            77,
-            77,
-            77
+            195,
+            225,
+            274,
+            323,
+            389,
+            454,
+            548,
+            632,
+            710,
+            783,
+            874,
+            969,
+            1050,
+            1130,
+            1205,
+            1236,
+            1297,
+            1361,
+            1463,
+            1569,
+            1665
         ],
         "TID": [
             "TID_BUILDING_CANNON",
             "TID_BUILDING_CANNON",
             "TID_BUILDING_CANNON",
             "TID_BUILDING_CANNON",
             "TID_BUILDING_CANNON",
@@ -17424,24 +17536,24 @@
         "SpeedMod": [],
         "SpellOnNearbyDamage": [],
         "Stage": [],
         "StartUpgradeBoosterCost": [],
         "StartingHomeCount": [],
         "StatusEffectTime": [],
         "StrengthWeight": [
-            2800,
-            2500,
-            2250,
-            2100,
-            2000,
-            1900,
-            1800,
-            1700,
-            1650,
-            1650
+            18900,
+            20000,
+            20813,
+            23100,
+            25500,
+            27550,
+            30150,
+            32725,
+            34650,
+            37950
         ],
         "TID": [
             "TID_BUILDING_DARK_TOWER",
             "TID_BUILDING_DARK_TOWER",
             "TID_BUILDING_DARK_TOWER",
             "TID_BUILDING_DARK_TOWER",
             "TID_BUILDING_DARK_TOWER",
@@ -28169,23 +28281,23 @@
         "SpellOnNearbyDamage": [],
         "Stage": [],
         "StartUpgradeBoosterCost": [],
         "StartingHomeCount": [],
         "StatusEffectTime": [],
         "StrengthWeight": [
             422,
-            379,
-            265,
-            265,
-            212,
-            212,
-            190,
-            190,
-            190,
-            190
+            422,
+            422,
+            422,
+            422,
+            422,
+            422,
+            422,
+            422,
+            422
         ],
         "TID": [
             "TID_BUILDING_GUARD_POST",
             "TID_BUILDING_GUARD_POST",
             "TID_BUILDING_GUARD_POST",
             "TID_BUILDING_GUARD_POST",
             "TID_BUILDING_GUARD_POST",
@@ -32709,16 +32821,16 @@
         "SpeedMod": [],
         "SpellOnNearbyDamage": [],
         "Stage": [],
         "StartUpgradeBoosterCost": [],
         "StartingHomeCount": [],
         "StatusEffectTime": [],
         "StrengthWeight": [
-            400,
-            440
+            9400,
+            11000
         ],
         "TID": [
             "TID_BUILDING_MULTI_ARCHER_TOWER",
             "TID_BUILDING_MULTI_ARCHER_TOWER"
         ],
         "TargetGroups": [],
         "TargetGroupsRadius": [],
@@ -33060,16 +33172,16 @@
         "SpeedMod": [],
         "SpellOnNearbyDamage": [],
         "Stage": [],
         "StartUpgradeBoosterCost": [],
         "StartingHomeCount": [],
         "StatusEffectTime": [],
         "StrengthWeight": [
-            200,
-            220
+            9900,
+            11715
         ],
         "TID": [
             "TID_BUILDING_RICOCHET_CANNON",
             "TID_BUILDING_RICOCHET_CANNON"
         ],
         "TargetGroups": [],
         "TargetGroupsRadius": [],
@@ -33582,14 +33694,15 @@
         "AOESpell": [],
         "AOESpellAlternate": [],
         "ActivateCombatOnDamageTaken": [],
         "ActivatedCombatAddBuildingClass": [],
         "AimRotateStep": [],
         "AirTargets": [
             true,
+            true,
             true
         ],
         "AltAirTargets": [],
         "AltAttackMode": [],
         "AltAttackRange": [],
         "AltAttackSpeed": [],
         "AltBuildResource": [],
@@ -33606,217 +33719,251 @@
         "AmmoCost": [],
         "AmmoCount": [],
         "AmmoResource": [],
         "AmountCanBeUpgraded": [],
         "AnimateTurret": [],
         "AnimationActionFrame": [
             5,
+            5,
             5
         ],
         "AppearEffect": [],
         "ArmySlotType": [],
         "AttackEffect": [
             "Monolith Attack",
+            "Monolith Attack",
             "Monolith Attack"
         ],
         "AttackEffect2": [],
         "AttackEffectAlt": [],
         "AttackEffectLv2": [],
         "AttackEffectLv3": [],
         "AttackRange": [
             1100,
+            1100,
             1100
         ],
         "AttackSpeed": [
             1500,
+            1500,
             1500
         ],
         "BaseGfx": [],
         "Blacksmith": [],
         "BlueAdd": [],
         "BlueMul": [],
         "BoostCost": [],
         "BuildCost": [
             300000,
-            360000
+            360000,
+            370000
         ],
         "BuildResource": [
             "DarkElixir",
+            "DarkElixir",
             "DarkElixir"
         ],
         "BuildTimeD": [
             13,
-            14
+            14,
+            16
         ],
         "BuildTimeH": [
             12,
+            0,
             0
         ],
         "BuildTimeM": [
             0,
+            0,
             0
         ],
         "BuildTimeS": [
             0,
+            0,
             0
         ],
         "BuildingClass": [
             "Defense",
+            "Defense",
             "Defense"
         ],
         "BuildingH": [
             2,
+            2,
             2
         ],
         "BuildingLevel": [
             1,
-            2
+            2,
+            3
         ],
         "BuildingW": [
             2,
+            2,
             2
         ],
         "Bunker": [],
         "BurstCount": [],
         "BurstDelay": [],
         "CapitalHallLevel": [
             15,
-            15
+            15,
+            16
         ],
         "ChainAttackDamageReductionPercent": [],
         "ChainAttackDelay": [],
         "ChainAttackDistance": [],
         "ChainAttackMaxTargets": [],
         "CombatActivationDelay": [],
         "CombatActivationEffect": [],
         "CoolDownOverride": [
             750,
+            750,
             750
         ],
         "CustomTargetHitBuildingInRange": [],
         "DPS": [
             150,
-            175
+            175,
+            193
         ],
         "DPSLv2": [],
         "DPSLv3": [],
         "Damage": [],
         "Damage2": [],
         "Damage2Delay": [],
         "Damage2FalloffEnd": [],
         "Damage2FalloffStart": [],
         "Damage2Min": [],
         "Damage2Radius": [],
         "DamagePermilHp": [
             110,
-            120
+            120,
+            130
         ],
         "DamageRadius": [],
         "DefaultProjectileVariant": [
             3,
+            3,
             3
         ],
         "DefenceTroopCharacter": [],
         "DefenceTroopCharacter2": [],
         "DefenceTroopCount": [],
         "DefenceTroopLevel": [],
         "DefenderCharacter": [],
         "DefenderCount": [
             1,
+            1,
             1
         ],
         "DefenderZ": [
             155,
+            155,
             155
         ],
         "DestroyDamageEffect": [],
         "DestroyEffect": [
             "Building Destroyed",
+            "Building Destroyed",
             "Building Destroyed"
         ],
         "DestructionXP": [],
         "DieDamage": [],
         "DieDamageDelay": [],
         "DieDamageEffect": [],
         "DieDamageRadius": [],
         "DummyProjectileCount": [],
         "ExportName": [
             "monolith_lvl_1",
-            "monolith_lvl_2"
+            "monolith_lvl_2",
+            "monolith_lvl_3"
         ],
         "ExportNameBase": [
             "dark_tower_base",
+            "dark_tower_base",
             "dark_tower_base"
         ],
         "ExportNameBeamEnd": [],
         "ExportNameBeamStart": [],
         "ExportNameBuildAnim": [
             "tower_turret_upg",
+            "tower_turret_upg",
             "tower_turret_upg"
         ],
         "ExportNameConstruction": [
             "tower_turret_const",
+            "tower_turret_const",
             "tower_turret_const"
         ],
         "ExportNameDamaged": [
             "destroyedBuilding_3l_base_rockwood",
+            "destroyedBuilding_3l_base_rockwood",
             "destroyedBuilding_3l_base_rockwood"
         ],
         "ExportNameDamagedSWF": [],
         "ExportNameLocked": [],
         "ExportNameNpc": [],
         "ExportNameTriggered": [],
         "ExportNameUpgradeAnim": [
             "monolith_lvl_1_upgrade",
-            "monolith_lvl_2_upgrade"
+            "monolith_lvl_2_upgrade",
+            "monolith_lvl_3_upgrade"
         ],
         "ForgesMiniSpells": [],
         "ForgesSpells": [],
         "FreeBoost": [],
         "GearUpBuilding": [],
         "GearUpCost": [],
         "GearUpLevelRequirement": [],
         "GearUpResource": [],
         "GearUpTID": [],
         "GearUpTime": [],
         "GreenAdd": [],
         "GreenMul": [],
         "GroundTargets": [
             true,
+            true,
             true
         ],
         "HealthRecoveryPercent": [],
         "Height": [
             3,
+            3,
             3
         ],
         "HeroType": [],
         "Hidden": [],
         "HintPriority": [
             150,
+            150,
             150
         ],
         "HitEffect": [
             "Explosive Arrow",
+            "Explosive Arrow",
             "Explosive Arrow"
         ],
         "HitEffect2": [],
         "HitSpell": [],
         "HitSpellLevel": [],
         "Hitpoints": [
             4747,
-            5050
+            5050,
+            5353
         ],
         "HousingSpace": [],
         "HousingSpaceAlt": [],
         "HousingSpaceSiege": [],
         "Icon": [],
         "IncreasingDamage": [],
         "InfoTID": [
             "TID_BUILDING_MONOLITH_INFO",
+            "TID_BUILDING_MONOLITH_INFO",
             "TID_BUILDING_MONOLITH_INFO"
         ],
         "IsHeroBarrack": [],
         "IsRed": [],
         "LevelRequirementTID": [],
         "LoadAmmoEffect": [],
         "Locked": [],
@@ -33848,53 +33995,60 @@
         "PenetratingProjectile": [],
         "PenetratingRadius": [],
         "PercentageStoredDarkElixir": [],
         "PercentageStoredElixir": [],
         "PercentageStoredGold": [],
         "PickUpEffect": [
             "Monolith Pickup",
+            "Monolith Pickup",
             "Monolith Pickup"
         ],
         "PlacingEffect": [
             "Monolith Placing",
+            "Monolith Placing",
             "Monolith Placing"
         ],
         "PreAttackEffect": [],
         "PreferredTarget": [],
         "PreferredTargetDamageMod": [],
         "PrepareSpeed": [],
         "PreventsHealing": [],
         "PreviewScenario": [
             "Monolith",
+            "Monolith",
             "Monolith"
         ],
         "ProducesResource": [],
         "ProducesUnitsOfType": [],
         "Projectile": [
             "MonolithProjectileMin;MonolithProjectileMed;MonolithProjectileMax",
+            "MonolithProjectileMin;MonolithProjectileMed;MonolithProjectileMax",
             "MonolithProjectileMin;MonolithProjectileMed;MonolithProjectileMax"
         ],
         "ProjectileBounces": [],
         "ProjectileVariantByTargetMaxHP": [
             "600;2500",
-            "650;2750"
+            "650;2750",
+            "700;3000"
         ],
         "PushBack": [],
         "RandomHitPosition": [],
         "RedAdd": [],
         "RedMul": [],
         "RegenTime": [
             25,
+            26,
             26
         ],
         "ResourceIconLimit": [],
         "ResourceMax": [],
         "ResourcePer100Hours": [],
         "SWF": [
             "sc/buildings.sc",
+            "sc/buildings.sc",
             "sc/buildings.sc"
         ],
         "SecondaryTargetingClass": [],
         "SecondaryTroop": [],
         "SecondaryTroopCnt": [],
         "SecondaryTroopLvl": [],
         "SelfAsAoeCenter": [],
@@ -33906,28 +34060,31 @@
         "SpeedMod": [],
         "SpellOnNearbyDamage": [],
         "Stage": [],
         "StartUpgradeBoosterCost": [],
         "StartingHomeCount": [],
         "StatusEffectTime": [],
         "StrengthWeight": [
-            1400,
-            1300
+            37615,
+            39163,
+            40750
         ],
         "TID": [
             "TID_BUILDING_MONOLITH",
+            "TID_BUILDING_MONOLITH",
             "TID_BUILDING_MONOLITH"
         ],
         "TargetGroups": [],
         "TargetGroupsRadius": [],
         "TargetingConeAngle": [],
         "ToggleAttackModeEffect": [],
         "TownHallLevel": [
             15,
-            15
+            15,
+            16
         ],
         "TransitionEffectLv2": [],
         "TransitionEffectLv3": [],
         "TriggerRadius": [],
         "TurnSpeed": [],
         "UnitProduction": [],
         "UnlockWeaponMode": [],
@@ -33937,14 +34094,15 @@
         "VillageType": [],
         "WakeUpSpace": [],
         "WakeUpSpeed": [],
         "WallCornerPieces": [],
         "Weapon": [],
         "Width": [
             3,
+            3,
             3
         ]
     },
     "Mortar": {
         "AOESpell": [],
         "AOESpellAlternate": [],
         "ActivateCombatOnDamageTaken": [],
@@ -35050,30 +35208,30 @@
         "SpeedMod": [],
         "SpellOnNearbyDamage": [],
         "Stage": [],
         "StartUpgradeBoosterCost": [],
         "StartingHomeCount": [],
         "StatusEffectTime": [],
         "StrengthWeight": [
-            450,
-            440,
-            430,
-            420,
-            410,
-            400,
-            390,
-            380,
-            370,
-            360,
-            350,
-            350,
-            340,
-            340,
-            340,
-            340
+            630,
+            715,
+            796,
+            872,
+            984,
+            1090,
+            1268,
+            1520,
+            1804,
+            2070,
+            2363,
+            2643,
+            2873,
+            3290,
+            3664,
+            3995
         ],
         "TID": [
             "TID_BUILDING_MORTAR",
             "TID_BUILDING_MORTAR",
             "TID_BUILDING_MORTAR",
             "TID_BUILDING_MORTAR",
             "TID_BUILDING_MORTAR",
@@ -35503,22 +35661,22 @@
             "newVillage_multi_mortar_lvl5"
         ],
         "ExportNameBeamEnd": [],
         "ExportNameBeamStart": [],
         "ExportNameBuildAnim": [
             "mortar_upg",
             "mortar_upg",
-            "mortar_upg",
-            "mortar_upg",
-            "mortar_upg",
-            "mortar_upg",
-            "mortar_upg",
-            "mortar_upg",
-            "mortar_upg",
-            "mortar_upg"
+            "tower_turret_upg",
+            "tower_turret_upg",
+            "tower_turret_upg",
+            "tower_turret_upg",
+            "tower_turret_upg",
+            "tower_turret_upg",
+            "tower_turret_upg",
+            "tower_turret_upg"
         ],
         "ExportNameConstruction": [
             "mortar_const",
             "mortar_const",
             "mortar_const",
             "mortar_const",
             "mortar_const",
@@ -36549,127 +36707,138 @@
             12000000,
             14000000,
             16000000,
             19750000,
             20000000,
             20250000,
             20500000,
-            21000000
+            21000000,
+            21500000
         ],
         "BuildResource": [
             "Elixir",
             "Elixir",
             "Elixir",
             "Elixir",
             "Elixir",
             "Elixir",
             "Elixir",
             "Elixir",
+            "Elixir",
             "Elixir"
         ],
         "BuildTimeD": [
             12,
             12,
             12,
             13,
             13,
             13,
             13,
             14,
-            15
+            15,
+            16
         ],
         "BuildTimeH": [
             0,
             12,
             18,
             0,
             6,
             12,
             18,
             0,
+            0,
             0
         ],
         "BuildTimeM": [
             0,
             0,
             0,
             0,
             0,
             0,
             0,
             0,
+            0,
             0
         ],
         "BuildTimeS": [
             0,
             0,
             0,
             0,
             0,
             0,
             0,
             0,
+            0,
             0
         ],
         "BuildingClass": [
             "Army",
             "Army",
             "Army",
             "Army",
             "Army",
             "Army",
             "Army",
             "Army",
+            "Army",
             "Army"
         ],
         "BuildingH": [
             2,
             2,
             2,
             2,
             2,
             2,
             2,
             2,
+            2,
             2
         ],
         "BuildingLevel": [
             1,
             2,
             3,
             4,
             5,
             6,
             7,
             8,
-            9
+            9,
+            10
         ],
         "BuildingW": [
             2,
             2,
             2,
             2,
             2,
             2,
             2,
             2,
+            2,
             2
         ],
         "Bunker": [],
         "BurstCount": [],
         "BurstDelay": [],
         "CapitalHallLevel": [
             14,
             14,
             14,
             14,
             15,
             15,
             15,
             15,
+            16,
             16
         ],
         "ChainAttackDamageReductionPercent": [],
         "ChainAttackDelay": [],
         "ChainAttackDistance": [],
         "ChainAttackMaxTargets": [],
         "CombatActivationDelay": [],
@@ -36702,14 +36871,15 @@
             "Building Destroyed",
             "Building Destroyed",
             "Building Destroyed",
             "Building Destroyed",
             "Building Destroyed",
             "Building Destroyed",
             "Building Destroyed",
+            "Building Destroyed",
             "Building Destroyed"
         ],
         "DestructionXP": [],
         "DieDamage": [],
         "DieDamageDelay": [],
         "DieDamageEffect": [],
         "DieDamageRadius": [],
@@ -36719,60 +36889,65 @@
             "pet_house_lvl2",
             "pet_house_lvl3",
             "pet_house_lvl4",
             "pet_house_lvl5",
             "pet_house_lvl6",
             "pet_house_lvl7",
             "pet_house_lvl8",
-            "pet_house_lvl9"
+            "pet_house_lvl9",
+            "pet_house_lvl10"
         ],
         "ExportNameBase": [
             "pet_house_lvl1_base",
             "pet_house_lvl2_base",
             "pet_house_lvl3_base",
             "pet_house_lvl4_base",
             "pet_house_lvl5_base",
             "pet_house_lvl6_base",
             "pet_house_lvl7_base",
             "pet_house_lvl8_base",
+            "pet_house_lvl9_base",
             "pet_house_lvl9_base"
         ],
         "ExportNameBeamEnd": [],
         "ExportNameBeamStart": [],
         "ExportNameBuildAnim": [
             "laboratory_upg",
             "laboratory_upg",
             "laboratory_upg",
             "laboratory_upg",
             "laboratory_upg",
             "laboratory_upg",
             "laboratory_upg",
             "laboratory_upg",
+            "laboratory_upg",
             "laboratory_upg"
         ],
         "ExportNameConstruction": [
             "laboratory_const",
             "laboratory_const",
             "laboratory_const",
             "laboratory_const",
             "laboratory_const",
             "laboratory_const",
             "laboratory_const",
             "laboratory_const",
+            "laboratory_const",
             "laboratory_const"
         ],
         "ExportNameDamaged": [
             "destroyedBuilding_3l_pit_rockwood",
             "destroyedBuilding_3l_pit_rockwood",
             "destroyedBuilding_3l_pit_rockwood",
             "destroyedBuilding_3l_pit_rockwood",
             "destroyedBuilding_3l_pit_rockwood",
             "destroyedBuilding_3l_pit_rockwood",
             "destroyedBuilding_3l_pit_rockwood",
             "destroyedBuilding_3l_pit_rockwood",
+            "destroyedBuilding_3l_pit_rockwood",
             "destroyedBuilding_3l_pit_rockwood"
         ],
         "ExportNameDamagedSWF": [],
         "ExportNameLocked": [],
         "ExportNameNpc": [],
         "ExportNameTriggered": [],
         "ExportNameUpgradeAnim": [],
@@ -36794,27 +36969,29 @@
             3,
             3,
             3,
             3,
             3,
             3,
             3,
+            3,
             3
         ],
         "HeroType": [],
         "Hidden": [],
         "HintPriority": [
             1000,
             1000,
             1000,
             1000,
             1000,
             1000,
             1000,
             1000,
+            1000,
             1000
         ],
         "HitEffect": [],
         "HitEffect2": [],
         "HitSpell": [],
         "HitSpellLevel": [],
         "Hitpoints": [
@@ -36822,15 +36999,16 @@
             800,
             900,
             1000,
             1050,
             1100,
             1150,
             1200,
-            1250
+            1250,
+            1300
         ],
         "HousingSpace": [],
         "HousingSpaceAlt": [],
         "HousingSpaceSiege": [],
         "Icon": [],
         "IncreasingDamage": [],
         "InfoTID": [
@@ -36838,14 +37016,15 @@
             "TID_PET_SHOP_INFO",
             "TID_PET_SHOP_INFO",
             "TID_PET_SHOP_INFO",
             "TID_PET_SHOP_INFO",
             "TID_PET_SHOP_INFO",
             "TID_PET_SHOP_INFO",
             "TID_PET_SHOP_INFO",
+            "TID_PET_SHOP_INFO",
             "TID_PET_SHOP_INFO"
         ],
         "IsHeroBarrack": [],
         "IsRed": [],
         "LevelRequirementTID": [],
         "LoadAmmoEffect": [],
         "Locked": [],
@@ -36884,25 +37063,27 @@
             "Training Barrack Pickup",
             "Training Barrack Pickup",
             "Training Barrack Pickup",
             "Training Barrack Pickup",
             "Training Barrack Pickup",
             "Training Barrack Pickup",
             "Training Barrack Pickup",
+            "Training Barrack Pickup",
             "Training Barrack Pickup"
         ],
         "PlacingEffect": [
             "Training Barrack Placing",
             "Training Barrack Placing",
             "Training Barrack Placing",
             "Training Barrack Placing",
             "Training Barrack Placing",
             "Training Barrack Placing",
             "Training Barrack Placing",
             "Training Barrack Placing",
+            "Training Barrack Placing",
             "Training Barrack Placing"
         ],
         "PreAttackEffect": [],
         "PreferredTarget": [],
         "PreferredTargetDamageMod": [],
         "PrepareSpeed": [],
         "PreventsHealing": [],
@@ -36911,14 +37092,15 @@
             "NoCombatBuilding",
             "NoCombatBuilding",
             "NoCombatBuilding",
             "NoCombatBuilding",
             "NoCombatBuilding",
             "NoCombatBuilding",
             "NoCombatBuilding",
+            "NoCombatBuilding",
             "NoCombatBuilding"
         ],
         "ProducesResource": [],
         "ProducesUnitsOfType": [],
         "Projectile": [],
         "ProjectileBounces": [],
         "ProjectileVariantByTargetMaxHP": [],
@@ -36931,28 +37113,30 @@
             15,
             15,
             15,
             15,
             15,
             15,
             15,
+            15,
             15
         ],
         "ResourceIconLimit": [],
         "ResourceMax": [],
         "ResourcePer100Hours": [],
         "SWF": [
             "sc/buildings.sc",
             "sc/buildings.sc",
             "sc/buildings.sc",
             "sc/buildings.sc",
             "sc/buildings.sc",
             "sc/buildings.sc",
             "sc/buildings.sc",
             "sc/buildings.sc",
+            "sc/buildings.sc",
             "sc/buildings.sc"
         ],
         "SecondaryTargetingClass": [],
         "SecondaryTroop": [],
         "SecondaryTroopCnt": [],
         "SecondaryTroopLvl": [],
         "SelfAsAoeCenter": [],
@@ -36973,14 +37157,15 @@
             "TID_PET_SHOP",
             "TID_PET_SHOP",
             "TID_PET_SHOP",
             "TID_PET_SHOP",
             "TID_PET_SHOP",
             "TID_PET_SHOP",
             "TID_PET_SHOP",
+            "TID_PET_SHOP",
             "TID_PET_SHOP"
         ],
         "TargetGroups": [],
         "TargetGroupsRadius": [],
         "TargetingConeAngle": [],
         "ToggleAttackModeEffect": [],
         "TownHallLevel": [
@@ -36988,14 +37173,15 @@
             14,
             14,
             14,
             15,
             15,
             15,
             15,
+            16,
             16
         ],
         "TransitionEffectLv2": [],
         "TransitionEffectLv3": [],
         "TriggerRadius": [],
         "TurnSpeed": [],
         "UnitProduction": [],
@@ -37007,14 +37193,15 @@
             "PET",
             "PET",
             "PET",
             "PET",
             "PET",
             "PET",
             "PET",
+            "PET",
             "PET"
         ],
         "VillageType": [],
         "WakeUpSpace": [],
         "WakeUpSpeed": [],
         "WallCornerPieces": [],
         "Weapon": [],
@@ -37023,14 +37210,15 @@
             3,
             3,
             3,
             3,
             3,
             3,
             3,
+            3,
             3
         ]
     },
     "Recovery Building": {
         "AOESpell": [],
         "AOESpellAlternate": [],
         "ActivateCombatOnDamageTaken": [],
@@ -38224,19 +38412,19 @@
         "SpeedMod": [],
         "SpellOnNearbyDamage": [],
         "Stage": [],
         "StartUpgradeBoosterCost": [],
         "StartingHomeCount": [],
         "StatusEffectTime": [],
         "StrengthWeight": [
-            700,
-            700,
-            700,
-            700,
-            700
+            15050,
+            17850,
+            20650,
+            21875,
+            22575
         ],
         "TID": [
             "TID_BUILDING_SCATTERSHOT",
             "TID_BUILDING_SCATTERSHOT",
             "TID_BUILDING_SCATTERSHOT",
             "TID_BUILDING_SCATTERSHOT",
             "TID_BUILDING_SCATTERSHOT"
@@ -40154,17 +40342,17 @@
         "SpeedMod": [],
         "SpellOnNearbyDamage": [],
         "Stage": [],
         "StartUpgradeBoosterCost": [],
         "StartingHomeCount": [],
         "StatusEffectTime": [],
         "StrengthWeight": [
-            1000,
-            1400,
-            1800
+            6250,
+            9800,
+            13950
         ],
         "TID": [
             "TID_BUILDING_SPELL_TOWER",
             "TID_BUILDING_SPELL_TOWER",
             "TID_BUILDING_SPELL_TOWER"
         ],
         "TargetGroups": [],
@@ -40988,29 +41176,29 @@
         "SpeedMod": [],
         "SpellOnNearbyDamage": [],
         "Stage": [],
         "StartUpgradeBoosterCost": [],
         "StartingHomeCount": [],
         "StatusEffectTime": [],
         "StrengthWeight": [
-            100,
-            100,
-            100,
-            100,
-            100,
-            100,
-            100,
-            100,
-            100,
-            100,
-            100,
-            100,
-            100,
-            100,
-            100
+            490,
+            558,
+            645,
+            723,
+            823,
+            943,
+            1073,
+            1203,
+            1325,
+            1445,
+            1575,
+            1700,
+            1838,
+            1963,
+            2088
         ],
         "TID": [
             "TID_BUILDING_TESLA_TOWER",
             "TID_BUILDING_TESLA_TOWER",
             "TID_BUILDING_TESLA_TOWER",
             "TID_BUILDING_TESLA_TOWER",
             "TID_BUILDING_TESLA_TOWER",
@@ -46063,17 +46251,15 @@
         "AltNumMultiTargets": [],
         "AltPreviewScenario": [],
         "AltProjectile": [],
         "AlternatePickNewTargetDelay": [],
         "AmmoCost": [],
         "AmmoCount": [],
         "AmmoResource": [],
-        "AmountCanBeUpgraded": [
-            250
-        ],
+        "AmountCanBeUpgraded": [],
         "AnimateTurret": [],
         "AnimationActionFrame": [],
         "AppearEffect": [],
         "ArmySlotType": [],
         "AttackEffect": [],
         "AttackEffect2": [],
         "AttackEffectAlt": [],
@@ -46678,31 +46864,31 @@
             5,
             8,
             9
         ],
         "StartingHomeCount": [],
         "StatusEffectTime": [],
         "StrengthWeight": [
-            200,
-            200,
-            200,
-            200,
-            200,
-            200,
-            200,
-            200,
-            200,
-            200,
-            200,
-            200,
-            200,
-            200,
-            200,
-            200,
-            200
+            1,
+            2,
+            3,
+            4,
+            6,
+            8,
+            10,
+            12,
+            14,
+            16,
+            20,
+            28,
+            36,
+            44,
+            50,
+            54,
+            58
         ],
         "TID": [
             "TID_BUILDING_WALL",
             "TID_BUILDING_WALL",
             "TID_BUILDING_WALL",
             "TID_BUILDING_WALL",
             "TID_BUILDING_WALL",
@@ -48183,30 +48369,30 @@
         "SpeedMod": [],
         "SpellOnNearbyDamage": [],
         "Stage": [],
         "StartUpgradeBoosterCost": [],
         "StartingHomeCount": [],
         "StatusEffectTime": [],
         "StrengthWeight": [
-            450,
-            420,
-            390,
-            360,
-            330,
-            300,
-            270,
-            240,
-            240,
-            240,
-            240,
-            240,
-            240,
-            240,
-            250,
-            250
+            1193,
+            1229,
+            1287,
+            1377,
+            1485,
+            1680,
+            1890,
+            1944,
+            2208,
+            2688,
+            3024,
+            3360,
+            3636,
+            3900,
+            4250,
+            4519
         ],
         "TID": [
             "TID_BUILDING_WIZARD_TOWER",
             "TID_BUILDING_WIZARD_TOWER",
             "TID_BUILDING_WIZARD_TOWER",
             "TID_BUILDING_WIZARD_TOWER",
             "TID_BUILDING_WIZARD_TOWER",
@@ -48282,22 +48468,24 @@
         "AOESpellAlternate": [],
         "ActivateCombatOnDamageTaken": [],
         "ActivatedCombatAddBuildingClass": [
             "Defense",
             "Defense",
             "Defense",
             "Defense",
+            "Defense",
             "Defense"
         ],
         "AimRotateStep": [],
         "AirTargets": [
             true,
             true,
             true,
             true,
+            true,
             true
         ],
         "AltAirTargets": [],
         "AltAttackMode": [],
         "AltAttackRange": [],
         "AltAttackSpeed": [],
         "AltBuildResource": [],
@@ -48316,148 +48504,165 @@
         "AmmoResource": [],
         "AmountCanBeUpgraded": [],
         "AnimateTurret": [
             true,
             true,
             true,
             true,
+            true,
             true
         ],
         "AnimationActionFrame": [],
         "AppearEffect": [],
         "ArmySlotType": [],
         "AttackEffect": [
             "Nailgun Attack FX",
             "Nailgun Attack FX",
             "Nailgun Attack FX",
             "Nailgun Attack FX",
+            "Nailgun Attack FX",
             "Nailgun Attack FX"
         ],
         "AttackEffect2": [],
         "AttackEffectAlt": [],
         "AttackEffectLv2": [],
         "AttackEffectLv3": [],
         "AttackRange": [
             700,
             700,
             700,
             700,
+            700,
             700
         ],
         "AttackSpeed": [
             400,
             400,
             400,
             400,
+            400,
             400
         ],
         "BaseGfx": [],
         "Blacksmith": [],
         "BlueAdd": [],
         "BlueMul": [],
         "BoostCost": [
             500,
             500,
             500,
             500,
+            500,
             500
         ],
         "BuildCost": [
             0,
             8000000,
             10000000,
             12000000,
-            17000000
+            17000000,
+            20000000
         ],
         "BuildResource": [
             "Diamonds",
             "Gold",
             "Gold",
             "Gold",
+            "Gold",
             "Gold"
         ],
         "BuildTimeD": [
             0,
             9,
             11,
             13,
-            14
+            14,
+            15
         ],
         "BuildTimeH": [
             0,
             12,
             12,
             6,
-            6
+            6,
+            0
         ],
         "BuildTimeM": [
             0,
             0,
             0,
             0,
+            0,
             0
         ],
         "BuildTimeS": [
             0,
             0,
             0,
             0,
+            0,
             0
         ],
         "BuildingClass": [
             "Worker",
             "Worker",
             "Worker",
             "Worker",
+            "Worker",
             "Worker"
         ],
         "BuildingH": [
             1,
             1,
             1,
             1,
+            1,
             1
         ],
         "BuildingLevel": [
             1,
             2,
             3,
             4,
-            5
+            5,
+            6
         ],
         "BuildingW": [
             1,
             1,
             1,
             1,
+            1,
             1
         ],
         "Bunker": [],
         "BurstCount": [],
         "BurstDelay": [],
         "CapitalHallLevel": [
             1,
             14,
             14,
             14,
-            15
+            15,
+            16
         ],
         "ChainAttackDamageReductionPercent": [],
         "ChainAttackDelay": [],
         "ChainAttackDistance": [],
         "ChainAttackMaxTargets": [],
         "CombatActivationDelay": [],
         "CombatActivationEffect": [],
         "CoolDownOverride": [],
         "CustomTargetHitBuildingInRange": [],
         "DPS": [
             80,
             100,
             120,
-            135
+            135,
+            150
         ],
         "DPSLv2": [],
         "DPSLv3": [],
         "Damage": [],
         "Damage2": [],
         "Damage2Delay": [],
         "Damage2FalloffEnd": [],
@@ -48467,81 +48672,90 @@
         "DamagePermilHp": [],
         "DamageRadius": [],
         "DefaultProjectileVariant": [],
         "DefenceTroopCharacter": [
             "Defending Builder",
             "Defending Builder",
             "Defending Builder",
+            "Defending Builder",
             "Defending Builder"
         ],
         "DefenceTroopCharacter2": [],
         "DefenceTroopCount": [
             1,
             1,
             1,
+            1,
             1
         ],
         "DefenceTroopLevel": [
             1,
             2,
             3,
-            4
+            4,
+            5
         ],
         "DefenderCharacter": [],
         "DefenderCount": [],
         "DefenderZ": [],
         "DestroyDamageEffect": [],
         "DestroyEffect": [
             "Building Destroyed",
             "Building Destroyed",
             "Building Destroyed",
             "Building Destroyed",
+            "Building Destroyed",
             "Building Destroyed"
         ],
         "DestructionXP": [],
         "DieDamage": [],
         "DieDamageDelay": [],
         "DieDamageEffect": [],
         "DieDamageRadius": [],
         "DummyProjectileCount": [],
         "ExportName": [
             "worker_building",
             "worker_building_armed_lvl1",
             "worker_building_armed_lvl2",
             "worker_building_armed_lvl3",
-            "worker_building_armed_lvl4"
+            "worker_building_armed_lvl4",
+            "worker_building_armed_lvl5"
         ],
         "ExportNameBase": [
             "worker_building_base",
             "worker_building_base",
             "worker_building_base",
             "worker_building_base",
+            "worker_building_base",
             "worker_building_base"
         ],
         "ExportNameBeamEnd": [],
         "ExportNameBeamStart": [],
         "ExportNameBuildAnim": [
             "worker_building_upg",
             "worker_building_upg",
             "worker_building_upg",
             "worker_building_upg",
+            "worker_building_upg",
             "worker_building_upg"
         ],
         "ExportNameConstruction": [
             "worker_building_const",
             "worker_building_const",
             "worker_building_const",
             "worker_building_const",
+            "worker_building_const",
             "worker_building_const"
         ],
         "ExportNameDamaged": [
             "destroyedBuilding_2s_pit_wood_darkbrown",
             "destroyedBuilding_2s_pit_wood_darkbrown",
             "destroyedBuilding_2s_pit_wood_darkbrown",
             "destroyedBuilding_2s_pit_wood_darkgreen",
+            "destroyedBuilding_2s_pit_wood_darkpurple",
             "destroyedBuilding_2s_pit_wood_darkpurple"
         ],
         "ExportNameDamagedSWF": [],
         "ExportNameLocked": [],
         "ExportNameNpc": [],
         "ExportNameTriggered": [],
         "ExportNameUpgradeAnim": [],
@@ -48557,59 +48771,65 @@
         "GreenAdd": [],
         "GreenMul": [],
         "GroundTargets": [
             true,
             true,
             true,
             true,
+            true,
             true
         ],
         "HealthRecoveryPercent": [],
         "Height": [
             2,
             2,
             2,
             2,
+            2,
             2
         ],
         "HeroType": [],
         "Hidden": [],
         "HintPriority": [
             200,
             200,
             200,
             200,
+            200,
             200
         ],
         "HitEffect": [
             "Generic Hit",
             "Generic Hit",
             "Generic Hit",
+            "Generic Hit",
             "Generic Hit"
         ],
         "HitEffect2": [],
         "HitSpell": [],
         "HitSpellLevel": [],
         "Hitpoints": [
             250,
             1000,
             1300,
             1600,
-            1800
+            1800,
+            1900
         ],
         "HousingSpace": [],
         "HousingSpaceAlt": [],
         "HousingSpaceSiege": [],
         "Icon": [],
         "IncreasingDamage": [],
         "InfoTID": [
             "TID_WORKER_INFO",
             "TID_WORKER_INFO",
             "TID_WORKER_INFO",
             "TID_WORKER_INFO",
+            "TID_WORKER_INFO",
             "TID_WORKER_INFO"
         ],
         "IsHeroBarrack": [],
         "IsRed": [],
         "LevelRequirementTID": [],
         "LoadAmmoEffect": [],
         "Locked": [],
@@ -48644,64 +48864,70 @@
         "PercentageStoredElixir": [],
         "PercentageStoredGold": [],
         "PickUpEffect": [
             "Worker Building Pickup",
             "Worker Building Pickup",
             "Worker Building Pickup",
             "Worker Building Pickup",
+            "Worker Building Pickup",
             "Worker Building Pickup"
         ],
         "PlacingEffect": [
             "Worker Building Placing",
             "Worker Building Placing",
             "Worker Building Placing",
             "Worker Building Placing",
+            "Worker Building Placing",
             "Worker Building Placing"
         ],
         "PreAttackEffect": [],
         "PreferredTarget": [],
         "PreferredTargetDamageMod": [],
         "PrepareSpeed": [],
         "PreventsHealing": [],
         "PreviewScenario": [
             "NoCombatBuilding",
             "DefensiveBuilder",
             "DefensiveBuilder",
             "DefensiveBuilder",
+            "DefensiveBuilder",
             "DefensiveBuilder"
         ],
         "ProducesResource": [],
         "ProducesUnitsOfType": [],
         "Projectile": [
             "Nail Ammo",
             "Nail Ammo",
             "Nail Ammo 2",
+            "Nail Ammo 2",
             "Nail Ammo 2"
         ],
         "ProjectileBounces": [],
         "ProjectileVariantByTargetMaxHP": [],
         "PushBack": [],
         "RandomHitPosition": [],
         "RedAdd": [],
         "RedMul": [],
         "RegenTime": [
             20,
             20,
             20,
             20,
+            20,
             20
         ],
         "ResourceIconLimit": [],
         "ResourceMax": [],
         "ResourcePer100Hours": [],
         "SWF": [
             "sc/buildings.sc",
             "sc/buildings.sc",
             "sc/buildings.sc",
             "sc/buildings.sc",
+            "sc/buildings.sc",
             "sc/buildings.sc"
         ],
         "SecondaryTargetingClass": [],
         "SecondaryTroop": [],
         "SecondaryTroopCnt": [],
         "SecondaryTroopLvl": [],
         "SelfAsAoeCenter": [],
@@ -48715,40 +48941,45 @@
         "Stage": [],
         "StartUpgradeBoosterCost": [],
         "StartingHomeCount": [
             1,
             1,
             1,
             1,
+            1,
             1
         ],
         "StatusEffectTime": [],
         "StrengthWeight": [
-            400,
-            380,
-            360,
-            340
+            0,
+            4600,
+            5795,
+            6840,
+            7480,
+            8000
         ],
         "TID": [
             "TID_WORKER_BUILDING",
             "TID_WORKER_BUILDING",
             "TID_WORKER_BUILDING",
             "TID_WORKER_BUILDING",
+            "TID_WORKER_BUILDING",
             "TID_WORKER_BUILDING"
         ],
         "TargetGroups": [],
         "TargetGroupsRadius": [],
         "TargetingConeAngle": [],
         "ToggleAttackModeEffect": [],
         "TownHallLevel": [
             1,
             14,
             14,
             14,
-            15
+            15,
+            16
         ],
         "TransitionEffectLv2": [],
         "TransitionEffectLv3": [],
         "TriggerRadius": [],
         "TurnSpeed": [],
         "UnitProduction": [],
         "UnlockWeaponMode": [],
@@ -48756,30 +48987,33 @@
         "UpgradeTasksRequired": [],
         "UpgradesUnitType": [],
         "VillageType": [],
         "WakeUpSpace": [
             1,
             1,
             1,
+            1,
             1
         ],
         "WakeUpSpeed": [
             1600,
             1600,
             1600,
             1600,
+            1600,
             1600
         ],
         "WallCornerPieces": [],
         "Weapon": [],
         "Width": [
             2,
             2,
             2,
             2,
+            2,
             2
         ]
     },
     "Worker Building2": {
         "AOESpell": [],
         "AOESpellAlternate": [],
         "ActivateCombatOnDamageTaken": [],
```

### Comparing `coc.py-3.4.1/coc/static/characters.json` & `coc_py-3.4.2/coc/static/characters.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9671720446951801%*

 * *Differences: {"'AirDefenceSeeker'": "{'UpgradeTimeH': {insert: [(5, 192)], delete: [5]}, 'UpgradeCost': "*

 * *                       "{insert: [(5, 160000)], delete: [5]}, 'StrengthWeight': [2000, 3000, 4000, "*

 * *                       '5000, 6000, 7000]}',*

 * * "'Apprentice Warden'": "{'StrengthWeight': [6000, 7000, 8000, 9000]}",*

 * * "'Archer'": "{'StrengthWeight': [800, 1200, 1400, 1600, 1700, 1800, 2000, 3000, 4000, 6000, 7000, "*

 * *             '8000]}',*

 * * "'BabyDragon'": "{'StrengthWeight': [2000, 2500, 3000, 4000, 5000, 6000, 700 […]*

```diff
@@ -436,20 +436,20 @@
             250,
             250,
             250,
             250
         ],
         "Squad": [],
         "StrengthWeight": [
-            160,
-            240,
-            350,
-            420,
-            490,
-            560
+            2000,
+            3000,
+            4000,
+            5000,
+            6000,
+            7000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
@@ -504,15 +504,15 @@
         "UnitsInCamp": [],
         "UpgradeCost": [
             28000,
             43000,
             85000,
             120000,
             160000,
-            300000
+            160000
         ],
         "UpgradeLevelByTH": [],
         "UpgradeResource": [
             "DarkElixir",
             "DarkElixir",
             "DarkElixir",
             "DarkElixir",
@@ -521,15 +521,15 @@
         ],
         "UpgradeTimeH": [
             60,
             96,
             150,
             168,
             192,
-            216
+            192
         ],
         "UpgradeTimeM": [],
         "VillageType": [],
         "VisualLevel": [
             1,
             2,
             3,
@@ -1635,18 +1635,18 @@
             250,
             250,
             250,
             250
         ],
         "Squad": [],
         "StrengthWeight": [
-            1200,
-            1300,
-            1400,
-            1500
+            6000,
+            7000,
+            8000,
+            9000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
@@ -2287,26 +2287,26 @@
             300,
             300,
             300,
             300
         ],
         "Squad": [],
         "StrengthWeight": [
-            150,
-            150,
-            140,
-            130,
-            120,
-            110,
-            100,
-            100,
-            100,
-            100,
-            100,
-            100
+            800,
+            1200,
+            1400,
+            1600,
+            1700,
+            1800,
+            2000,
+            3000,
+            4000,
+            6000,
+            7000,
+            8000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
@@ -4139,24 +4139,24 @@
             250,
             250,
             250,
             250
         ],
         "Squad": [],
         "StrengthWeight": [
-            200,
-            250,
-            300,
-            350,
-            400,
-            450,
-            500,
-            550,
-            600,
-            600
+            2000,
+            2500,
+            3000,
+            4000,
+            5000,
+            6000,
+            7000,
+            8000,
+            9000,
+            10000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
@@ -6137,25 +6137,25 @@
             130,
             130,
             130,
             130
         ],
         "Squad": [],
         "StrengthWeight": [
-            120,
-            150,
-            160,
-            180,
-            180,
-            200,
-            300,
-            350,
-            400,
-            450,
-            475
+            1400,
+            1600,
+            1800,
+            2000,
+            2200,
+            3000,
+            4000,
+            5000,
+            6000,
+            8000,
+            10000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
@@ -8554,26 +8554,26 @@
             200,
             200,
             200,
             200
         ],
         "Squad": [],
         "StrengthWeight": [
-            100,
-            100,
-            90,
-            80,
-            70,
-            65,
-            60,
-            55,
-            55,
-            55,
-            55,
-            55
+            800,
+            1200,
+            1400,
+            1600,
+            1700,
+            1800,
+            2000,
+            3000,
+            4000,
+            6000,
+            7000,
+            8000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
@@ -9410,65 +9410,36 @@
         "SecondaryTroop": [],
         "SecondaryTroopCnt": [],
         "SelfAsAoeCenter": [],
         "SmoothJump": [],
         "SpawnIdle": [],
         "SpawnOnAttack": [],
         "SpawnWhenDamaged": [],
-        "SpecialAbilities": [],
-        "SpecialAbilitiesLevel": [],
-        "SpecialAbilityAttribute": [
-            6,
-            6,
-            8,
-            8,
-            8,
-            8,
-            10,
-            10,
-            12,
-            12,
-            14,
-            14,
-            16,
-            16,
-            18,
-            18,
-            20,
-            20,
-            22
-        ],
-        "SpecialAbilityAttribute2": [],
-        "SpecialAbilityAttribute3": [],
-        "SpecialAbilityEffect": [],
-        "SpecialAbilityHideClipName": [],
-        "SpecialAbilityIcon": [],
-        "SpecialAbilityInfo": [
-            "TID_BARB2_ABILITY_HELP",
-            "TID_BARB2_ABILITY_HELP",
-            "TID_BARB2_ABILITY_HELP",
-            "TID_BARB2_ABILITY_HELP",
-            "TID_BARB2_ABILITY_HELP",
-            "TID_BARB2_ABILITY_HELP",
-            "TID_BARB2_ABILITY_HELP",
-            "TID_BARB2_ABILITY_HELP",
-            "TID_BARB2_ABILITY_HELP",
-            "TID_BARB2_ABILITY_HELP",
-            "TID_BARB2_ABILITY_HELP",
-            "TID_BARB2_ABILITY_HELP",
-            "TID_BARB2_ABILITY_HELP",
-            "TID_BARB2_ABILITY_HELP",
-            "TID_BARB2_ABILITY_HELP",
-            "TID_BARB2_ABILITY_HELP",
-            "TID_BARB2_ABILITY_HELP",
-            "TID_BARB2_ABILITY_HELP",
-            "TID_BARB2_ABILITY_HELP",
-            "TID_BARB2_ABILITY_HELP"
+        "SpecialAbilities": [
+            "EliteBarbarianAbility",
+            "EliteBarbarianAbility",
+            "EliteBarbarianAbility",
+            "EliteBarbarianAbility",
+            "EliteBarbarianAbility",
+            "EliteBarbarianAbility",
+            "EliteBarbarianAbility",
+            "EliteBarbarianAbility",
+            "EliteBarbarianAbility",
+            "EliteBarbarianAbility",
+            "EliteBarbarianAbility",
+            "EliteBarbarianAbility",
+            "EliteBarbarianAbility",
+            "EliteBarbarianAbility",
+            "EliteBarbarianAbility",
+            "EliteBarbarianAbility",
+            "EliteBarbarianAbility",
+            "EliteBarbarianAbility",
+            "EliteBarbarianAbility"
         ],
-        "SpecialAbilityLevel": [
+        "SpecialAbilitiesLevel": [
             1,
             1,
             2,
             2,
             2,
             2,
             3,
@@ -9481,80 +9452,25 @@
             6,
             7,
             7,
             8,
             8,
             9
         ],
-        "SpecialAbilityName": [
-            "TID_BARB2_ABILITY_NAME",
-            "TID_BARB2_ABILITY_NAME",
-            "TID_BARB2_ABILITY_NAME",
-            "TID_BARB2_ABILITY_NAME",
-            "TID_BARB2_ABILITY_NAME",
-            "TID_BARB2_ABILITY_NAME",
-            "TID_BARB2_ABILITY_NAME",
-            "TID_BARB2_ABILITY_NAME",
-            "TID_BARB2_ABILITY_NAME",
-            "TID_BARB2_ABILITY_NAME",
-            "TID_BARB2_ABILITY_NAME",
-            "TID_BARB2_ABILITY_NAME",
-            "TID_BARB2_ABILITY_NAME",
-            "TID_BARB2_ABILITY_NAME",
-            "TID_BARB2_ABILITY_NAME",
-            "TID_BARB2_ABILITY_NAME",
-            "TID_BARB2_ABILITY_NAME",
-            "TID_BARB2_ABILITY_NAME",
-            "TID_BARB2_ABILITY_NAME",
-            "TID_BARB2_ABILITY_NAME"
-        ],
-        "SpecialAbilitySpell": [
-            "TroopRage",
-            "TroopRage",
-            "TroopRage",
-            "TroopRage",
-            "TroopRage",
-            "TroopRage",
-            "TroopRage",
-            "TroopRage",
-            "TroopRage",
-            "TroopRage",
-            "TroopRage",
-            "TroopRage",
-            "TroopRage",
-            "TroopRage",
-            "TroopRage",
-            "TroopRage",
-            "TroopRage",
-            "TroopRage",
-            "TroopRage",
-            "TroopRage"
-        ],
-        "SpecialAbilityType": [
-            "BoostUnitOnDeploy",
-            "BoostUnitOnDeploy",
-            "BoostUnitOnDeploy",
-            "BoostUnitOnDeploy",
-            "BoostUnitOnDeploy",
-            "BoostUnitOnDeploy",
-            "BoostUnitOnDeploy",
-            "BoostUnitOnDeploy",
-            "BoostUnitOnDeploy",
-            "BoostUnitOnDeploy",
-            "BoostUnitOnDeploy",
-            "BoostUnitOnDeploy",
-            "BoostUnitOnDeploy",
-            "BoostUnitOnDeploy",
-            "BoostUnitOnDeploy",
-            "BoostUnitOnDeploy",
-            "BoostUnitOnDeploy",
-            "BoostUnitOnDeploy",
-            "BoostUnitOnDeploy",
-            "BoostUnitOnDeploy"
-        ],
+        "SpecialAbilityAttribute": [],
+        "SpecialAbilityAttribute2": [],
+        "SpecialAbilityAttribute3": [],
+        "SpecialAbilityEffect": [],
+        "SpecialAbilityHideClipName": [],
+        "SpecialAbilityIcon": [],
+        "SpecialAbilityInfo": [],
+        "SpecialAbilityLevel": [],
+        "SpecialAbilityName": [],
+        "SpecialAbilitySpell": [],
+        "SpecialAbilityType": [],
         "SpecialMovementMod": [],
         "Speed": [
             240,
             240,
             240,
             240,
             240,
@@ -10718,26 +10634,15 @@
             250,
             250,
             250,
             250,
             250
         ],
         "Squad": [],
-        "StrengthWeight": [
-            140,
-            130,
-            120,
-            110,
-            100,
-            100,
-            100,
-            100,
-            100,
-            100
-        ],
+        "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
@@ -11752,18 +11657,18 @@
             300,
             300,
             300,
             300
         ],
         "Squad": [],
         "StrengthWeight": [
-            31,
-            31,
-            31,
-            31
+            7500,
+            8000,
+            9000,
+            10000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
@@ -12702,27 +12607,27 @@
             300,
             300,
             300,
             300
         ],
         "Squad": [],
         "StrengthWeight": [
-            150,
-            150,
-            150,
-            150,
-            220,
-            300,
-            380,
-            380,
-            400,
-            480,
-            520,
-            500,
-            480
+            1800,
+            2000,
+            2100,
+            2200,
+            3000,
+            4000,
+            5000,
+            5500,
+            6000,
+            7000,
+            8000,
+            9000,
+            10000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
@@ -14776,22 +14681,22 @@
             175,
             175,
             175,
             175
         ],
         "Squad": [],
         "StrengthWeight": [
-            600,
-            800,
-            800,
-            1000,
-            1200,
-            1250,
-            1200,
-            1200
+            3000,
+            4000,
+            5000,
+            6000,
+            7000,
+            8000,
+            9000,
+            10000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
@@ -15458,27 +15363,15 @@
             250,
             250,
             250,
             250,
             250
         ],
         "Squad": [],
-        "StrengthWeight": [
-            120,
-            120,
-            120,
-            120,
-            120,
-            120,
-            120,
-            120,
-            120,
-            120,
-            120
-        ],
+        "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
@@ -17742,25 +17635,25 @@
             200,
             200,
             200,
             200
         ],
         "Squad": [],
         "StrengthWeight": [
-            160,
-            165,
-            170,
-            250,
-            420,
-            480,
-            540,
-            600,
-            660,
-            660,
-            660
+            1800,
+            2000,
+            2200,
+            3000,
+            4000,
+            5000,
+            6000,
+            7000,
+            8000,
+            9000,
+            10000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
@@ -18234,18 +18127,18 @@
             250,
             250,
             250,
             250
         ],
         "Squad": [],
         "StrengthWeight": [
-            580,
-            660,
-            740,
-            820
+            6000,
+            7000,
+            8000,
+            10000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
@@ -18543,17 +18436,15 @@
         "SpecialAbilitySpell": [],
         "SpecialAbilityType": [],
         "SpecialMovementMod": [],
         "Speed": [
             300
         ],
         "Squad": [],
-        "StrengthWeight": [
-            120
-        ],
+        "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
@@ -19073,21 +18964,21 @@
             160,
             160,
             160,
             160
         ],
         "Squad": [],
         "StrengthWeight": [
-            650,
-            700,
-            800,
-            860,
-            920,
-            970,
-            1000
+            4000,
+            5000,
+            6000,
+            7000,
+            8000,
+            9000,
+            10000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
@@ -19186,72 +19077,82 @@
         ],
         "WallMovementCost": []
     },
     "Electro Titan": {
         "AirTargets": [
             true,
             true,
+            true,
             true
         ],
         "AltPreviewScenario": [],
         "AltProjectile": [],
         "Animation": [
             "ElectroTitan_lvl1",
             "ElectroTitan_lvl2",
-            "ElectroTitan_lvl3"
+            "ElectroTitan_lvl3",
+            "ElectroTitan_lvl4"
         ],
         "AreaDamageIgnoresWalls": [],
         "AttackCount": [],
         "AttackEffect": [
             "Electro_Titan Attack_lvl1",
             "Electro_Titan Attack_lvl1",
+            "Electro_Titan Attack_lvl1",
             "Electro_Titan Attack_lvl1"
         ],
         "AttackEffect2": [],
         "AttackEffectLv2": [],
         "AttackEffectLv3": [],
         "AttackEffectLv4": [],
         "AttackMultipleBuildings": [],
         "AttackRange": [
             125,
             125,
+            125,
             125
         ],
         "AttackSpeed": [
             1500,
             1500,
+            1500,
             1500
         ],
         "AuraSpell": [
             "ElectroTitanDamageAura",
             "ElectroTitanDamageAura",
+            "ElectroTitanDamageAura",
             "ElectroTitanDamageAura"
         ],
         "AuraSpellLevel": [
             0,
             1,
-            2
+            2,
+            3
         ],
         "AutoMergeDistance": [],
         "AutoMergeGroupSize": [],
         "AvoidNoiseInAttackPositionSelection": [],
         "BarrackLevel": [
             16,
             16,
+            16,
             16
         ],
         "BecomesTargetableEffect": [],
         "BigPicture": [
             "unit_electro_titan_big",
             "unit_electro_titan_big",
+            "unit_electro_titan_big",
             "unit_electro_titan_big"
         ],
         "BigPictureSWF": [
             "sc/info_electro_titan.sc",
             "sc/info_electro_titan.sc",
+            "sc/info_electro_titan.sc",
             "sc/info_electro_titan.sc"
         ],
         "BoostAttackSpeed": [],
         "BoostDmgPerfect": [],
         "BoostRadius": [],
         "BoostedIfAlone": [],
         "BunkerDegenerationTime": [],
@@ -19270,15 +19171,16 @@
         "ChainAttackMaxTargets": [],
         "ChainShootingDistance": [],
         "CoolDownOverride": [],
         "CustomDefenderIcon": [],
         "DPS": [
             180,
             200,
-            220
+            220,
+            240
         ],
         "DPSLv2": [],
         "DPSLv3": [],
         "Damage2": [],
         "Damage2Delay": [],
         "Damage2FalloffEnd": [],
         "Damage2FalloffStart": [],
@@ -19290,128 +19192,144 @@
         "DamageReductionToStorages": [],
         "DefaultSkin": [],
         "DefenseBonus": [],
         "DefensiveTroop": [],
         "DeployEffect": [
             "Elektro Titan Deploy",
             "Elektro Titan Deploy",
+            "Elektro Titan Deploy",
             "Elektro Titan Deploy"
         ],
         "DeployEffect2": [],
         "Deprecated": [],
         "DieDamage": [],
         "DieDamageDelay": [],
         "DieDamageEffect": [],
         "DieDamageRadius": [],
         "DieEffect": [
             "ElektroTitanDie",
             "ElektroTitanDie",
+            "ElektroTitanDie",
             "ElektroTitanDie"
         ],
         "DieEffect2": [],
         "DisableDonate": [],
         "DisableProduction": [],
         "DoesNotOpenCC": [],
         "DonateCost": [
             16,
             16,
+            16,
             16
         ],
         "DonateCount": [],
         "DonateXP": [],
         "EnabledByCalendar": [],
         "EnabledBySuperLicence": [],
         "EnemyGroupWeight": [
             3000,
             3000,
+            3000,
             3000
         ],
         "EvolveEffect": [],
         "EvolveOnDamageDealt": [],
         "EvolveTime": [],
         "EvolveToCharacter": [],
         "FightWithGroups": [],
         "FriendlyGroupWeight": [
             3000,
             3000,
+            3000,
             3000
         ],
         "FrostOnHitPercent": [],
         "FrostOnHitTime": [],
         "GroundTargets": [
             true,
             true,
+            true,
             true
         ],
         "HealerWeight": [],
         "HealthReductionPerSecond": [],
         "HeroDamageMultiplier": [],
         "HideEffect": [],
         "HitEffect": [
             "Golem Hit",
             "Golem Hit",
+            "Golem Hit",
             "Golem Hit"
         ],
         "HitEffect2": [],
         "Hitpoints": [
             7200,
             7700,
-            8200
+            8200,
+            8400
         ],
         "HousingSpace": [
             32,
             32,
+            32,
             32
         ],
         "IconExportName": [
             "icon_unit_electrotitan",
             "icon_unit_electrotitan",
+            "icon_unit_electrotitan",
             "icon_unit_electrotitan"
         ],
         "IconSWF": [
             "sc/ui.sc",
             "sc/ui.sc",
+            "sc/ui.sc",
             "sc/ui.sc"
         ],
         "ImmuneToHealing": [],
         "IncreasingDamage": [],
         "InfoTID": [
             "TID_CHARACTER_ELECTRO_TITAN_INFO",
             "TID_CHARACTER_ELECTRO_TITAN_INFO",
+            "TID_CHARACTER_ELECTRO_TITAN_INFO",
             "TID_CHARACTER_ELECTRO_TITAN_INFO"
         ],
         "InvisibilityRadius": [],
         "IsFlying": [
             false,
             false,
+            false,
             false
         ],
         "IsJumper": [
             false,
             false,
+            false,
             false
         ],
         "IsSecondaryTroop": [],
         "IsUnderground": [],
         "JumpHeightPercent": [],
         "LaboratoryLevel": [
             1,
             12,
-            13
+            13,
+            14
         ],
         "LoseHpEffect": [],
         "LoseHpInterval": [],
         "LoseHpPerTick": [],
         "Lv2SwitchTime": [],
         "Lv3SwitchTime": [],
         "MoveStartsEffect": [],
         "MovementOffsetAmount": [],
         "MovementOffsetSpeed": [
             0,
             0,
+            0,
             0
         ],
         "MovingEffect": [],
         "Name": [],
         "NewTargetAttackDelay": [],
         "NoClipping": [],
         "PenetratingExtraRange": [],
@@ -19421,26 +19339,29 @@
         "PreAttackEffect": [],
         "PreferHeroes": [],
         "PreferedTargetBuilding": [],
         "PreferedTargetBuildingClass": [],
         "PreferedTargetDamageMod": [
             1,
             1,
+            1,
             1
         ],
         "PreferredMovementTarget": [],
         "PreferredTargetNoTargeting": [],
         "PreviewScenario": [
             "TroopElectroTitan",
             "TroopElectroTitan",
+            "TroopElectroTitan",
             "TroopElectroTitan"
         ],
         "ProductionBuilding": [
             "Barrack",
             "Barrack",
+            "Barrack",
             "Barrack"
         ],
         "Projectile": [],
         "ProjectileBounces": [],
         "ProjectileConsumesBunkerTroops": [],
         "PushbackAfterHit": [],
         "PushbackSpeed": [],
@@ -19470,84 +19391,95 @@
         "SpecialAbilityName": [],
         "SpecialAbilitySpell": [],
         "SpecialAbilityType": [],
         "SpecialMovementMod": [],
         "Speed": [
             200,
             200,
+            200,
             200
         ],
         "Squad": [],
         "StrengthWeight": [
-            650,
-            700,
-            750
+            7000,
+            8000,
+            9000,
+            10000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
             "TID_CHARACTER_ELECTRO_TITAN",
             "TID_CHARACTER_ELECTRO_TITAN",
+            "TID_CHARACTER_ELECTRO_TITAN",
             "TID_CHARACTER_ELECTRO_TITAN"
         ],
         "TargetGroupsMinWeight": [],
         "TargetGroupsRadius": [],
         "TargetGroupsRange": [],
         "TargetedEffectOffset": [
             "-50",
             "-50",
+            "-50",
             "-50"
         ],
         "TombStone": [
             "TombStone",
             "TombStone",
+            "TombStone",
             "TombStone"
         ],
         "TrainingTime": [
             360,
             360,
+            360,
             360
         ],
         "TransitionEffectLv2": [],
         "TransitionEffectLv3": [],
         "TransitionEffectLv4": [],
         "TriggersTraps": [
             true,
             true,
+            true,
             true
         ],
         "UndergroundEffect": [],
         "UnderwaterEffect": [],
         "UnitsInCamp": [],
         "UpgradeCost": [
             19500000,
             20500000,
-            20500000
+            22000000,
+            22000000
         ],
         "UpgradeLevelByTH": [],
         "UpgradeResource": [
             "Elixir",
             "Elixir",
+            "Elixir",
             "Elixir"
         ],
         "UpgradeTimeH": [
             312,
             336,
-            336
+            384,
+            384
         ],
         "UpgradeTimeM": [],
         "VillageType": [],
         "VisualLevel": [
             1,
             2,
-            3
+            3,
+            4
         ],
         "WallMovementCost": []
     },
     "Electrofire Wizard": {
         "AirTargets": [
             true,
             true,
@@ -21501,28 +21433,15 @@
             300,
             300,
             300,
             300,
             300
         ],
         "Squad": [],
-        "StrengthWeight": [
-            150,
-            150,
-            150,
-            150,
-            150,
-            150,
-            150,
-            150,
-            150,
-            150,
-            150,
-            150
-        ],
+        "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
@@ -22283,28 +22202,15 @@
             250,
             250,
             250,
             250,
             250
         ],
         "Squad": [],
-        "StrengthWeight": [
-            100,
-            100,
-            100,
-            100,
-            100,
-            100,
-            100,
-            100,
-            100,
-            100,
-            100,
-            100
-        ],
+        "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
@@ -23052,28 +22958,15 @@
             150,
             150,
             150,
             150,
             150
         ],
         "Squad": [],
-        "StrengthWeight": [
-            120,
-            120,
-            120,
-            120,
-            120,
-            120,
-            120,
-            120,
-            120,
-            120,
-            120,
-            120
-        ],
+        "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
@@ -23713,25 +23606,15 @@
             400,
             400,
             400,
             400,
             400
         ],
         "Squad": [],
-        "StrengthWeight": [
-            50,
-            50,
-            50,
-            50,
-            50,
-            50,
-            50,
-            50,
-            50
-        ],
+        "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
@@ -25271,28 +25154,15 @@
             350,
             350,
             350,
             350,
             350
         ],
         "Squad": [],
-        "StrengthWeight": [
-            100,
-            100,
-            100,
-            100,
-            100,
-            100,
-            100,
-            100,
-            100,
-            100,
-            100,
-            100
-        ],
+        "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
@@ -26347,17 +26217,15 @@
         "SpecialAbilitySpell": [],
         "SpecialAbilityType": [],
         "SpecialMovementMod": [],
         "Speed": [
             270
         ],
         "Squad": [],
-        "StrengthWeight": [
-            100
-        ],
+        "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
@@ -26639,17 +26507,15 @@
         "SpecialAbilitySpell": [],
         "SpecialAbilityType": [],
         "SpecialMovementMod": [],
         "Speed": [
             200
         ],
         "Squad": [],
-        "StrengthWeight": [
-            25
-        ],
+        "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
@@ -26695,14 +26561,783 @@
         "UpgradeTimeM": [],
         "VillageType": [],
         "VisualLevel": [
             1
         ],
         "WallMovementCost": []
     },
+    "Free Kicker": {
+        "AirTargets": [
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false
+        ],
+        "AltPreviewScenario": [],
+        "AltProjectile": [],
+        "Animation": [
+            "FootballBarbarian",
+            "FootballBarbarian",
+            "FootballBarbarian",
+            "FootballBarbarian",
+            "FootballBarbarian",
+            "FootballBarbarian",
+            "FootballBarbarian",
+            "FootballBarbarian",
+            "FootballBarbarian",
+            "FootballBarbarian",
+            "FootballBarbarian",
+            "FootballBarbarian"
+        ],
+        "AreaDamageIgnoresWalls": [],
+        "AttackCount": [],
+        "AttackEffect": [
+            "Barbarian_Football_Atk",
+            "Barbarian_Football_Atk",
+            "Barbarian_Football_Atk",
+            "Barbarian_Football_Atk",
+            "Barbarian_Football_Atk",
+            "Barbarian_Football_Atk",
+            "Barbarian_Football_Atk",
+            "Barbarian_Football_Atk",
+            "Barbarian_Football_Atk",
+            "Barbarian_Football_Atk",
+            "Barbarian_Football_Atk",
+            "Barbarian_Football_Atk"
+        ],
+        "AttackEffect2": [],
+        "AttackEffectLv2": [],
+        "AttackEffectLv3": [],
+        "AttackEffectLv4": [],
+        "AttackMultipleBuildings": [],
+        "AttackRange": [
+            60,
+            60,
+            60,
+            60,
+            60,
+            60,
+            60,
+            60,
+            60,
+            60,
+            60,
+            60
+        ],
+        "AttackSpeed": [
+            1300,
+            1300,
+            1300,
+            1300,
+            1300,
+            1300,
+            1300,
+            1300,
+            1300,
+            1300,
+            1300,
+            1300
+        ],
+        "AuraSpell": [],
+        "AuraSpellLevel": [],
+        "AutoMergeDistance": [],
+        "AutoMergeGroupSize": [],
+        "AvoidNoiseInAttackPositionSelection": [],
+        "BarrackLevel": [
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1
+        ],
+        "BecomesTargetableEffect": [],
+        "BigPicture": [
+            "unit_football_barbarian_big",
+            "unit_football_barbarian_big",
+            "unit_football_barbarian_big",
+            "unit_football_barbarian_big",
+            "unit_football_barbarian_big",
+            "unit_football_barbarian_big",
+            "unit_football_barbarian_big",
+            "unit_football_barbarian_big",
+            "unit_football_barbarian_big",
+            "unit_football_barbarian_big",
+            "unit_football_barbarian_big",
+            "unit_football_barbarian_big"
+        ],
+        "BigPictureSWF": [
+            "sc/info_football_barbarian.sc",
+            "sc/info_football_barbarian.sc",
+            "sc/info_football_barbarian.sc",
+            "sc/info_football_barbarian.sc",
+            "sc/info_football_barbarian.sc",
+            "sc/info_football_barbarian.sc",
+            "sc/info_football_barbarian.sc",
+            "sc/info_football_barbarian.sc",
+            "sc/info_football_barbarian.sc",
+            "sc/info_football_barbarian.sc",
+            "sc/info_football_barbarian.sc",
+            "sc/info_football_barbarian.sc"
+        ],
+        "BoostAttackSpeed": [],
+        "BoostDmgPerfect": [],
+        "BoostRadius": [],
+        "BoostedIfAlone": [],
+        "BunkerDegenerationTime": [],
+        "BunkerSpawnDist": [],
+        "BunkerTroopCount1": [],
+        "BunkerTroopCount2": [],
+        "BunkerTroops": [],
+        "BurstCount": [],
+        "BurstDelay": [],
+        "CanAttackWhileMoving": [],
+        "CarryOverToNextStage": [],
+        "ChainAttackDamageReductionPercent": [],
+        "ChainAttackDelay": [],
+        "ChainAttackDistance": [],
+        "ChainAttackEffect": [],
+        "ChainAttackMaxTargets": [],
+        "ChainShootingDistance": [],
+        "CoolDownOverride": [],
+        "CustomDefenderIcon": [],
+        "DPS": [
+            50,
+            60,
+            90,
+            110,
+            125,
+            135,
+            145,
+            160,
+            165,
+            170,
+            180,
+            190
+        ],
+        "DPSLv2": [],
+        "DPSLv3": [],
+        "Damage2": [],
+        "Damage2Delay": [],
+        "Damage2FalloffEnd": [],
+        "Damage2FalloffStart": [],
+        "Damage2Min": [],
+        "Damage2Radius": [],
+        "DamageMultiplierPercent": [],
+        "DamageMultiplierTarget": [],
+        "DamageRadius": [],
+        "DamageReductionToStorages": [],
+        "DefaultSkin": [],
+        "DefenseBonus": [],
+        "DefensiveTroop": [],
+        "DeployEffect": [
+            "Barbarian_Football_Deploy",
+            "Barbarian_Football_Deploy",
+            "Barbarian_Football_Deploy",
+            "Barbarian_Football_Deploy",
+            "Barbarian_Football_Deploy",
+            "Barbarian_Football_Deploy",
+            "Barbarian_Football_Deploy",
+            "Barbarian_Football_Deploy",
+            "Barbarian_Football_Deploy",
+            "Barbarian_Football_Deploy",
+            "Barbarian_Football_Deploy",
+            "Barbarian_Football_Deploy"
+        ],
+        "DeployEffect2": [],
+        "Deprecated": [],
+        "DieDamage": [],
+        "DieDamageDelay": [],
+        "DieDamageEffect": [],
+        "DieDamageRadius": [],
+        "DieEffect": [
+            "Barbarian Die",
+            "Barbarian Die",
+            "Barbarian Die",
+            "Barbarian Die",
+            "Barbarian Die",
+            "Barbarian Die",
+            "Barbarian Die",
+            "Barbarian Die",
+            "Barbarian Die",
+            "Barbarian Die",
+            "Barbarian Die",
+            "Barbarian Die"
+        ],
+        "DieEffect2": [],
+        "DisableDonate": [
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true
+        ],
+        "DisableProduction": [],
+        "DoesNotOpenCC": [],
+        "DonateCost": [
+            8,
+            8,
+            8,
+            8,
+            8,
+            8,
+            8,
+            8,
+            8,
+            8,
+            8,
+            8
+        ],
+        "DonateCount": [],
+        "DonateXP": [],
+        "EnabledByCalendar": [
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true
+        ],
+        "EnabledBySuperLicence": [],
+        "EnemyGroupWeight": [
+            400,
+            400,
+            400,
+            400,
+            400,
+            400,
+            400,
+            400,
+            400,
+            400,
+            400,
+            400
+        ],
+        "EvolveEffect": [],
+        "EvolveOnDamageDealt": [],
+        "EvolveTime": [],
+        "EvolveToCharacter": [],
+        "FightWithGroups": [],
+        "FriendlyGroupWeight": [
+            400,
+            400,
+            400,
+            400,
+            400,
+            400,
+            400,
+            400,
+            400,
+            400,
+            400,
+            400
+        ],
+        "FrostOnHitPercent": [],
+        "FrostOnHitTime": [],
+        "GroundTargets": [
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true
+        ],
+        "HealerWeight": [],
+        "HealthReductionPerSecond": [],
+        "HeroDamageMultiplier": [],
+        "HideEffect": [],
+        "HitEffect": [
+            "Barbarian Hit",
+            "Barbarian Hit",
+            "Barbarian Hit",
+            "Barbarian Hit",
+            "Barbarian Hit",
+            "Barbarian Hit",
+            "Barbarian Hit",
+            "Barbarian Hit",
+            "Barbarian Hit",
+            "Barbarian Hit",
+            "Barbarian Hit",
+            "Barbarian Hit"
+        ],
+        "HitEffect2": [],
+        "Hitpoints": [
+            300,
+            350,
+            650,
+            1000,
+            1200,
+            1400,
+            1600,
+            1900,
+            2000,
+            2100,
+            2300,
+            2400
+        ],
+        "HousingSpace": [
+            12,
+            12,
+            12,
+            12,
+            12,
+            12,
+            12,
+            12,
+            12,
+            12,
+            12,
+            12
+        ],
+        "IconExportName": [
+            "icon_unit_footballbarbarian",
+            "icon_unit_footballbarbarian",
+            "icon_unit_footballbarbarian",
+            "icon_unit_footballbarbarian",
+            "icon_unit_footballbarbarian",
+            "icon_unit_footballbarbarian",
+            "icon_unit_footballbarbarian",
+            "icon_unit_footballbarbarian",
+            "icon_unit_footballbarbarian",
+            "icon_unit_footballbarbarian",
+            "icon_unit_footballbarbarian",
+            "icon_unit_footballbarbarian"
+        ],
+        "IconSWF": [
+            "sc/update.sc",
+            "sc/update.sc",
+            "sc/update.sc",
+            "sc/update.sc",
+            "sc/update.sc",
+            "sc/update.sc",
+            "sc/update.sc",
+            "sc/update.sc",
+            "sc/update.sc",
+            "sc/update.sc",
+            "sc/update.sc",
+            "sc/update.sc"
+        ],
+        "ImmuneToHealing": [],
+        "IncreasingDamage": [],
+        "InfoTID": [
+            "TID_CHARACTER_INFO_FREE_KICKER",
+            "TID_CHARACTER_INFO_FREE_KICKER",
+            "TID_CHARACTER_INFO_FREE_KICKER",
+            "TID_CHARACTER_INFO_FREE_KICKER",
+            "TID_CHARACTER_INFO_FREE_KICKER",
+            "TID_CHARACTER_INFO_FREE_KICKER",
+            "TID_CHARACTER_INFO_FREE_KICKER",
+            "TID_CHARACTER_INFO_FREE_KICKER",
+            "TID_CHARACTER_INFO_FREE_KICKER",
+            "TID_CHARACTER_INFO_FREE_KICKER",
+            "TID_CHARACTER_INFO_FREE_KICKER",
+            "TID_CHARACTER_INFO_FREE_KICKER"
+        ],
+        "InvisibilityRadius": [],
+        "IsFlying": [
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false
+        ],
+        "IsJumper": [
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false
+        ],
+        "IsSecondaryTroop": [],
+        "IsUnderground": [],
+        "JumpHeightPercent": [],
+        "LaboratoryLevel": [
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1
+        ],
+        "LoseHpEffect": [],
+        "LoseHpInterval": [],
+        "LoseHpPerTick": [],
+        "Lv2SwitchTime": [],
+        "Lv3SwitchTime": [],
+        "MoveStartsEffect": [],
+        "MovementOffsetAmount": [],
+        "MovementOffsetSpeed": [
+            0,
+            0,
+            0,
+            0,
+            0,
+            0,
+            0,
+            0,
+            0,
+            0,
+            0,
+            0
+        ],
+        "MovingEffect": [],
+        "Name": [],
+        "NewTargetAttackDelay": [],
+        "NoClipping": [],
+        "PenetratingExtraRange": [],
+        "PenetratingProjectile": [],
+        "PenetratingRadius": [],
+        "PickNewTargetAfterPushback": [],
+        "PreAttackEffect": [],
+        "PreferHeroes": [],
+        "PreferedTargetBuilding": [],
+        "PreferedTargetBuildingClass": [],
+        "PreferedTargetDamageMod": [],
+        "PreferredMovementTarget": [],
+        "PreferredTargetNoTargeting": [],
+        "PreviewScenario": [
+            "TroopFreeKicker",
+            "TroopFreeKicker",
+            "TroopFreeKicker",
+            "TroopFreeKicker",
+            "TroopFreeKicker",
+            "TroopFreeKicker",
+            "TroopFreeKicker",
+            "TroopFreeKicker",
+            "TroopFreeKicker",
+            "TroopFreeKicker",
+            "TroopFreeKicker",
+            "TroopFreeKicker"
+        ],
+        "ProductionBuilding": [
+            "Barrack",
+            "Barrack",
+            "Barrack",
+            "Barrack",
+            "Barrack",
+            "Barrack",
+            "Barrack",
+            "Barrack",
+            "Barrack",
+            "Barrack",
+            "Barrack",
+            "Barrack"
+        ],
+        "Projectile": [],
+        "ProjectileBounces": [],
+        "ProjectileConsumesBunkerTroops": [],
+        "PushbackAfterHit": [],
+        "PushbackSpeed": [],
+        "RandomizeSecSpawnDist": [],
+        "ReflectsDamage": [],
+        "RetargetAfterHit": [],
+        "ScaleByTH": [],
+        "SecondarySpawnDist": [],
+        "SecondarySpawnOffset": [],
+        "SecondaryTroop": [],
+        "SecondaryTroopCnt": [],
+        "SelfAsAoeCenter": [],
+        "SmoothJump": [],
+        "SpawnIdle": [],
+        "SpawnOnAttack": [],
+        "SpawnWhenDamaged": [],
+        "SpecialAbilities": [
+            "FreeKick",
+            "FreeKick",
+            "FreeKick",
+            "FreeKick",
+            "FreeKick",
+            "FreeKick",
+            "FreeKick",
+            "FreeKick",
+            "FreeKick",
+            "FreeKick",
+            "FreeKick",
+            "FreeKick"
+        ],
+        "SpecialAbilitiesLevel": [
+            1,
+            2,
+            3,
+            4,
+            5,
+            6,
+            7,
+            8,
+            9,
+            10,
+            11,
+            12
+        ],
+        "SpecialAbilityAttribute": [
+            507,
+            561,
+            815,
+            1015,
+            1286,
+            1685,
+            2011,
+            2247,
+            2700,
+            2900,
+            3008,
+            3153
+        ],
+        "SpecialAbilityAttribute2": [],
+        "SpecialAbilityAttribute3": [],
+        "SpecialAbilityEffect": [],
+        "SpecialAbilityHideClipName": [],
+        "SpecialAbilityIcon": [],
+        "SpecialAbilityInfo": [
+            "TID_ABILITY_FREE_KICK_INFO",
+            "TID_ABILITY_FREE_KICK_INFO",
+            "TID_ABILITY_FREE_KICK_INFO",
+            "TID_ABILITY_FREE_KICK_INFO",
+            "TID_ABILITY_FREE_KICK_INFO",
+            "TID_ABILITY_FREE_KICK_INFO",
+            "TID_ABILITY_FREE_KICK_INFO",
+            "TID_ABILITY_FREE_KICK_INFO",
+            "TID_ABILITY_FREE_KICK_INFO",
+            "TID_ABILITY_FREE_KICK_INFO",
+            "TID_ABILITY_FREE_KICK_INFO",
+            "TID_ABILITY_FREE_KICK_INFO"
+        ],
+        "SpecialAbilityLevel": [
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1
+        ],
+        "SpecialAbilityName": [
+            "TID_ABILITY_FREE_KICK",
+            "TID_ABILITY_FREE_KICK",
+            "TID_ABILITY_FREE_KICK",
+            "TID_ABILITY_FREE_KICK",
+            "TID_ABILITY_FREE_KICK",
+            "TID_ABILITY_FREE_KICK",
+            "TID_ABILITY_FREE_KICK",
+            "TID_ABILITY_FREE_KICK",
+            "TID_ABILITY_FREE_KICK",
+            "TID_ABILITY_FREE_KICK",
+            "TID_ABILITY_FREE_KICK",
+            "TID_ABILITY_FREE_KICK"
+        ],
+        "SpecialAbilitySpell": [],
+        "SpecialAbilityType": [],
+        "SpecialMovementMod": [],
+        "Speed": [
+            250,
+            250,
+            250,
+            250,
+            250,
+            250,
+            250,
+            250,
+            250,
+            250,
+            250,
+            250
+        ],
+        "Squad": [],
+        "StrengthWeight": [],
+        "SummonCooldown": [],
+        "SummonEffect": [],
+        "SummonLimit": [],
+        "SummonTime": [],
+        "SummonTroop": [],
+        "SummonTroopCount": [],
+        "TID": [
+            "TID_CHARACTER_FREE_KICKER",
+            "TID_CHARACTER_FREE_KICKER",
+            "TID_CHARACTER_FREE_KICKER",
+            "TID_CHARACTER_FREE_KICKER",
+            "TID_CHARACTER_FREE_KICKER",
+            "TID_CHARACTER_FREE_KICKER",
+            "TID_CHARACTER_FREE_KICKER",
+            "TID_CHARACTER_FREE_KICKER",
+            "TID_CHARACTER_FREE_KICKER",
+            "TID_CHARACTER_FREE_KICKER",
+            "TID_CHARACTER_FREE_KICKER",
+            "TID_CHARACTER_FREE_KICKER"
+        ],
+        "TargetGroupsMinWeight": [],
+        "TargetGroupsRadius": [],
+        "TargetGroupsRange": [],
+        "TargetedEffectOffset": [
+            "-50",
+            "-50",
+            "-50",
+            "-50",
+            "-50",
+            "-50",
+            "-50",
+            "-50",
+            "-50",
+            "-50",
+            "-50",
+            "-50"
+        ],
+        "TombStone": [
+            "TombStone",
+            "TombStone",
+            "TombStone",
+            "TombStone",
+            "TombStone",
+            "TombStone",
+            "TombStone",
+            "TombStone",
+            "TombStone",
+            "TombStone",
+            "TombStone",
+            "TombStone"
+        ],
+        "TrainingTime": [
+            90,
+            90,
+            90,
+            90,
+            90,
+            90,
+            90,
+            90,
+            90,
+            90,
+            90,
+            90
+        ],
+        "TransitionEffectLv2": [],
+        "TransitionEffectLv3": [],
+        "TransitionEffectLv4": [],
+        "TriggersTraps": [
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true
+        ],
+        "UndergroundEffect": [],
+        "UnderwaterEffect": [],
+        "UnitsInCamp": [],
+        "UpgradeCost": [],
+        "UpgradeLevelByTH": [
+            3,
+            4,
+            7,
+            8,
+            9,
+            10,
+            11,
+            12,
+            13,
+            14,
+            15,
+            16
+        ],
+        "UpgradeResource": [
+            "Elixir",
+            "Elixir",
+            "Elixir",
+            "Elixir",
+            "Elixir",
+            "Elixir",
+            "Elixir",
+            "Elixir",
+            "Elixir",
+            "Elixir",
+            "Elixir",
+            "Elixir"
+        ],
+        "UpgradeTimeH": [],
+        "UpgradeTimeM": [],
+        "VillageType": [],
+        "VisualLevel": [
+            1,
+            2,
+            3,
+            4,
+            5,
+            6,
+            7,
+            8,
+            9,
+            10,
+            11,
+            12
+        ],
+        "WallMovementCost": []
+    },
     "FrostmiteSpawner": {
         "AirTargets": [
             false,
             false,
             false,
             false,
             false,
@@ -27282,27 +27917,15 @@
             0,
             0,
             0,
             0,
             0
         ],
         "Squad": [],
-        "StrengthWeight": [
-            53,
-            53,
-            53,
-            53,
-            53,
-            53,
-            53,
-            53,
-            53,
-            53,
-            53
-        ],
+        "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
@@ -27930,26 +28553,26 @@
             400,
             400,
             400,
             400
         ],
         "Squad": [],
         "StrengthWeight": [
-            120,
-            120,
-            115,
-            110,
-            105,
-            100,
-            100,
-            100,
-            100,
-            100,
-            100,
-            100
+            1500,
+            1600,
+            1700,
+            1800,
+            1900,
+            2000,
+            3000,
+            4000,
+            5000,
+            6000,
+            7000,
+            8000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
@@ -30160,26 +30783,26 @@
             150,
             150,
             150,
             150
         ],
         "Squad": [],
         "StrengthWeight": [
-            120,
-            120,
-            120,
-            120,
-            120,
-            200,
-            240,
-            280,
-            320,
-            360,
-            380,
-            400
+            1000,
+            1500,
+            1700,
+            1900,
+            2000,
+            2500,
+            3000,
+            4000,
+            5000,
+            6000,
+            8000,
+            9000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
@@ -30547,17 +31170,15 @@
         "SpecialAbilitySpell": [],
         "SpecialAbilityType": [],
         "SpecialMovementMod": [],
         "Speed": [
             150
         ],
         "Squad": [],
-        "StrengthWeight": [
-            120
-        ],
+        "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
@@ -32984,23 +33605,23 @@
             400,
             400,
             400,
             400
         ],
         "Squad": [],
         "StrengthWeight": [
-            50,
-            50,
-            45,
-            40,
-            35,
-            30,
-            30,
-            30,
-            30
+            700,
+            900,
+            1100,
+            1300,
+            1400,
+            1700,
+            2000,
+            4000,
+            7000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
@@ -33337,17 +33958,15 @@
         "SpecialAbilitySpell": [],
         "SpecialAbilityType": [],
         "SpecialMovementMod": [],
         "Speed": [
             200
         ],
         "Squad": [],
-        "StrengthWeight": [
-            160
-        ],
+        "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
@@ -34065,27 +34684,27 @@
             150,
             150,
             150,
             150
         ],
         "Squad": [],
         "StrengthWeight": [
-            160,
-            170,
-            210,
-            270,
-            400,
-            500,
-            500,
-            500,
-            500,
-            500,
-            550,
-            600,
-            650
+            1800,
+            2000,
+            2200,
+            2500,
+            3000,
+            3500,
+            4000,
+            4500,
+            5000,
+            6000,
+            7000,
+            8000,
+            9000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
@@ -35578,26 +36197,15 @@
             150,
             150,
             150,
             150,
             150
         ],
         "Squad": [],
-        "StrengthWeight": [
-            150,
-            200,
-            250,
-            300,
-            400,
-            500,
-            500,
-            500,
-            550,
-            600
-        ],
+        "StrengthWeight": [],
         "SummonCooldown": [
             7000,
             7000,
             7000,
             7000,
             7000,
             7000,
@@ -35915,24 +36523,24 @@
         "ChainAttackDistance": [],
         "ChainAttackEffect": [],
         "ChainAttackMaxTargets": [],
         "ChainShootingDistance": [],
         "CoolDownOverride": [],
         "CustomDefenderIcon": [],
         "DPS": [
-            108,
-            108,
-            108,
-            108,
-            108,
-            162,
-            198,
-            236,
-            256,
-            276,
+            170,
+            170,
+            170,
+            170,
+            170,
+            220,
+            260,
+            270,
+            280,
+            285,
             290
         ],
         "DPSLv2": [],
         "DPSLv3": [],
         "Damage2": [],
         "Damage2Delay": [],
         "Damage2FalloffEnd": [],
@@ -35970,24 +36578,24 @@
             "Balloon Rocket Deploy",
             "Balloon Rocket Deploy",
             "Balloon Rocket Deploy"
         ],
         "DeployEffect2": [],
         "Deprecated": [],
         "DieDamage": [
-            250,
-            250,
-            250,
-            250,
-            250,
             300,
-            350,
+            300,
+            300,
+            300,
+            300,
             400,
             500,
-            600,
+            580,
+            620,
+            650,
             700
         ],
         "DieDamageDelay": [
             416,
             416,
             416,
             416,
@@ -36132,21 +36740,21 @@
             "Balloon Goblin Hit",
             "Balloon Goblin Hit",
             "Balloon Goblin Hit",
             "Balloon Goblin Hit"
         ],
         "HitEffect2": [],
         "Hitpoints": [
-            280,
-            280,
-            280,
-            280,
-            280,
+            390,
+            390,
+            390,
+            390,
             390,
             545,
+            690,
             840,
             940,
             1040,
             1140
         ],
         "HousingSpace": [
             8,
@@ -36468,27 +37076,15 @@
             150,
             150,
             150,
             150,
             150
         ],
         "Squad": [],
-        "StrengthWeight": [
-            300,
-            300,
-            300,
-            300,
-            300,
-            300,
-            300,
-            300,
-            300,
-            300,
-            300
-        ],
+        "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
@@ -37425,17 +38021,15 @@
         "SpecialAbilitySpell": [],
         "SpecialAbilityType": [],
         "SpecialMovementMod": [],
         "Speed": [
             150
         ],
         "Squad": [],
-        "StrengthWeight": [
-            120
-        ],
+        "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
@@ -37592,27 +38186,27 @@
             3
         ],
         "DonateCount": [],
         "DonateXP": [],
         "EnabledByCalendar": [],
         "EnabledBySuperLicence": [],
         "EnemyGroupWeight": [
-            500,
-            500,
-            500
+            100,
+            100,
+            100
         ],
         "EvolveEffect": [],
         "EvolveOnDamageDealt": [],
         "EvolveTime": [],
         "EvolveToCharacter": [],
         "FightWithGroups": [],
         "FriendlyGroupWeight": [
-            600,
-            600,
-            600
+            100,
+            100,
+            100
         ],
         "FrostOnHitPercent": [],
         "FrostOnHitTime": [],
         "GroundTargets": [
             true,
             true,
             true
@@ -37781,17 +38375,17 @@
         "Speed": [
             300,
             300,
             300
         ],
         "Squad": [],
         "StrengthWeight": [
-            500,
-            600,
-            700
+            5000,
+            6000,
+            7000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
@@ -38338,23 +38932,23 @@
             200,
             200,
             200,
             200
         ],
         "Squad": [],
         "StrengthWeight": [
-            180,
-            185,
-            200,
-            220,
-            240,
-            260,
-            280,
-            300,
-            320
+            1400,
+            1600,
+            1800,
+            2500,
+            4000,
+            6000,
+            7000,
+            8000,
+            9000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
@@ -40511,36 +41105,15 @@
             400,
             400,
             400,
             400,
             400
         ],
         "Squad": [],
-        "StrengthWeight": [
-            326,
-            326,
-            326,
-            326,
-            326,
-            326,
-            326,
-            326,
-            326,
-            326,
-            326,
-            326,
-            326,
-            326,
-            326,
-            338,
-            350,
-            362,
-            374,
-            386
-        ],
+        "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
@@ -41305,26 +41878,15 @@
             300,
             300,
             300,
             300,
             300
         ],
         "Squad": [],
-        "StrengthWeight": [
-            150,
-            150,
-            150,
-            220,
-            300,
-            380,
-            400,
-            480,
-            520,
-            500
-        ],
+        "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
@@ -42021,29 +42583,15 @@
             200,
             200,
             200,
             200,
             200
         ],
         "Squad": [],
-        "StrengthWeight": [
-            150,
-            150,
-            150,
-            150,
-            150,
-            150,
-            150,
-            150,
-            150,
-            150,
-            150,
-            150,
-            150
-        ],
+        "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
@@ -42157,26 +42705,28 @@
         "AirTargets": [
             false,
             false,
             false,
             false,
             false,
             false,
+            false,
             false
         ],
         "AltPreviewScenario": [],
         "AltProjectile": [],
         "Animation": [
             "IceGolem_lvl1",
             "IceGolem_lvl2",
             "IceGolem_lvl3",
             "IceGolem_lvl4",
             "IceGolem_lvl5",
             "IceGolem_lvl6",
-            "IceGolem_lvl7"
+            "IceGolem_lvl7",
+            "IceGolem_lvl8"
         ],
         "AreaDamageIgnoresWalls": [],
         "AttackCount": [],
         "AttackEffect": [],
         "AttackEffect2": [],
         "AttackEffectLv2": [],
         "AttackEffectLv3": [],
@@ -42185,56 +42735,61 @@
         "AttackRange": [
             100,
             100,
             100,
             100,
             100,
             100,
+            100,
             100
         ],
         "AttackSpeed": [
             2000,
             2000,
             2000,
             2000,
             2000,
             2000,
+            2000,
             2000
         ],
         "AuraSpell": [],
         "AuraSpellLevel": [],
         "AutoMergeDistance": [],
         "AutoMergeGroupSize": [],
         "AvoidNoiseInAttackPositionSelection": [],
         "BarrackLevel": [
             8,
             8,
             8,
             8,
             8,
             8,
+            8,
             8
         ],
         "BecomesTargetableEffect": [],
         "BigPicture": [
             "unit_ice_golem_big",
             "unit_ice_golem_big",
             "unit_ice_golem_big",
             "unit_ice_golem_big",
             "unit_ice_golem_big",
             "unit_ice_golem_big",
+            "unit_ice_golem_big",
             "unit_ice_golem_big"
         ],
         "BigPictureSWF": [
             "sc/info_ice_golem.sc",
             "sc/info_ice_golem.sc",
             "sc/info_ice_golem.sc",
             "sc/info_ice_golem.sc",
             "sc/info_ice_golem.sc",
             "sc/info_ice_golem.sc",
+            "sc/info_ice_golem.sc",
             "sc/info_ice_golem.sc"
         ],
         "BoostAttackSpeed": [],
         "BoostDmgPerfect": [],
         "BoostRadius": [],
         "BoostedIfAlone": [],
         "BunkerDegenerationTime": [],
@@ -42257,15 +42812,16 @@
         "DPS": [
             24,
             28,
             32,
             36,
             40,
             44,
-            48
+            48,
+            52
         ],
         "DPSLv2": [],
         "DPSLv3": [],
         "Damage2": [],
         "Damage2Delay": [],
         "Damage2FalloffEnd": [],
         "Damage2FalloffStart": [],
@@ -42280,23 +42836,25 @@
         "DefensiveTroop": [
             "Ice Golem_DEF",
             "Ice Golem_DEF",
             "Ice Golem_DEF",
             "Ice Golem_DEF",
             "Ice Golem_DEF",
             "Ice Golem_DEF",
+            "Ice Golem_DEF",
             "Ice Golem_DEF"
         ],
         "DeployEffect": [
             "Icegolem Deploy",
             "Icegolem Deploy",
             "Icegolem Deploy",
             "Icegolem Deploy",
             "Icegolem Deploy",
             "Icegolem Deploy",
+            "Icegolem Deploy",
             "Icegolem Deploy"
         ],
         "DeployEffect2": [],
         "Deprecated": [],
         "DieDamage": [],
         "DieDamageDelay": [],
         "DieDamageEffect": [],
@@ -42304,182 +42862,199 @@
         "DieEffect": [
             "Giant Die",
             "Giant Die",
             "Giant Die",
             "Giant Die",
             "Giant Die",
             "Giant Die",
+            "Giant Die",
             "Giant Die"
         ],
         "DieEffect2": [],
         "DisableDonate": [],
         "DisableProduction": [],
         "DoesNotOpenCC": [],
         "DonateCost": [
             8,
             8,
             8,
             8,
             8,
             8,
+            8,
             8
         ],
         "DonateCount": [],
         "DonateXP": [],
         "EnabledByCalendar": [],
         "EnabledBySuperLicence": [],
         "EnemyGroupWeight": [
             500,
             500,
             500,
             500,
             500,
             500,
+            500,
             500
         ],
         "EvolveEffect": [],
         "EvolveOnDamageDealt": [],
         "EvolveTime": [],
         "EvolveToCharacter": [],
         "FightWithGroups": [],
         "FriendlyGroupWeight": [
             600,
             600,
             600,
             600,
             600,
             600,
+            600,
             600
         ],
         "FrostOnHitPercent": [
             50,
             50,
             50,
             50,
             50,
             50,
+            50,
             50
         ],
         "FrostOnHitTime": [
             2000,
             2000,
             2000,
             2000,
             2000,
             2000,
+            2000,
             2000
         ],
         "GroundTargets": [
             true,
             true,
             true,
             true,
             true,
             true,
+            true,
             true
         ],
         "HealerWeight": [
             1,
             1,
             1,
             1,
             1,
             1,
+            1,
             1
         ],
         "HealthReductionPerSecond": [],
         "HeroDamageMultiplier": [],
         "HideEffect": [],
         "HitEffect": [
             "IceWizard Hit1",
             "IceWizard Hit1",
             "IceWizard Hit1",
             "IceWizard Hit1",
             "IceWizard Hit1",
             "IceWizard Hit1",
+            "IceWizard Hit1",
             "IceWizard Hit1"
         ],
         "HitEffect2": [],
         "Hitpoints": [
             2600,
             2800,
             3000,
             3200,
             3400,
             3600,
-            3900
+            3900,
+            4200
         ],
         "HousingSpace": [
             15,
             15,
             15,
             15,
             15,
             15,
+            15,
             15
         ],
         "IconExportName": [
             "icon_unit_iceGolem",
             "icon_unit_iceGolem",
             "icon_unit_iceGolem",
             "icon_unit_iceGolem",
             "icon_unit_iceGolem",
             "icon_unit_iceGolem",
+            "icon_unit_iceGolem",
             "icon_unit_iceGolem"
         ],
         "IconSWF": [
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
+            "sc/ui.sc",
             "sc/ui.sc"
         ],
         "ImmuneToHealing": [],
         "IncreasingDamage": [],
         "InfoTID": [
             "TID_CHARACTER_INFO_ICEGOLEM",
             "TID_CHARACTER_INFO_ICEGOLEM",
             "TID_CHARACTER_INFO_ICEGOLEM",
             "TID_CHARACTER_INFO_ICEGOLEM",
             "TID_CHARACTER_INFO_ICEGOLEM",
             "TID_CHARACTER_INFO_ICEGOLEM",
+            "TID_CHARACTER_INFO_ICEGOLEM",
             "TID_CHARACTER_INFO_ICEGOLEM"
         ],
         "InvisibilityRadius": [],
         "IsFlying": [
             false,
             false,
             false,
             false,
             false,
             false,
+            false,
             false
         ],
         "IsJumper": [
             false,
             false,
             false,
             false,
             false,
             false,
+            false,
             false
         ],
         "IsSecondaryTroop": [],
         "IsUnderground": [],
         "JumpHeightPercent": [],
         "LaboratoryLevel": [
             1,
             9,
             9,
             10,
             10,
             12,
-            13
+            13,
+            14
         ],
         "LoseHpEffect": [],
         "LoseHpInterval": [],
         "LoseHpPerTick": [],
         "Lv2SwitchTime": [],
         "Lv3SwitchTime": [],
         "MoveStartsEffect": [],
@@ -42487,14 +43062,15 @@
         "MovementOffsetSpeed": [
             0,
             0,
             0,
             0,
             0,
             0,
+            0,
             0
         ],
         "MovingEffect": [],
         "Name": [],
         "NewTargetAttackDelay": [],
         "NoClipping": [],
         "PenetratingExtraRange": [],
@@ -42504,54 +43080,59 @@
         "PreAttackEffect": [
             "Icegolem Attack",
             "Icegolem Attack",
             "Icegolem Attack",
             "Icegolem Attack",
             "Icegolem Attack",
             "Icegolem Attack",
+            "Icegolem Attack",
             "Icegolem Attack"
         ],
         "PreferHeroes": [],
         "PreferedTargetBuilding": [],
         "PreferedTargetBuildingClass": [
             "Defense",
             "Defense",
             "Defense",
             "Defense",
             "Defense",
             "Defense",
+            "Defense",
             "Defense"
         ],
         "PreferedTargetDamageMod": [
             1,
             1,
             1,
             1,
             1,
             1,
+            1,
             1
         ],
         "PreferredMovementTarget": [],
         "PreferredTargetNoTargeting": [],
         "PreviewScenario": [
             "TroopIceGolem",
             "TroopIceGolem",
             "TroopIceGolem",
             "TroopIceGolem",
             "TroopIceGolem",
             "TroopIceGolem",
+            "TroopIceGolem",
             "TroopIceGolem"
         ],
         "ProductionBuilding": [
             "Dark Elixir Barrack",
             "Dark Elixir Barrack",
             "Dark Elixir Barrack",
             "Dark Elixir Barrack",
             "Dark Elixir Barrack",
             "Dark Elixir Barrack",
+            "Dark Elixir Barrack",
             "Dark Elixir Barrack"
         ],
         "Projectile": [],
         "ProjectileBounces": [],
         "ProjectileConsumesBunkerTroops": [],
         "PushbackAfterHit": [],
         "PushbackSpeed": [],
@@ -42573,15 +43154,16 @@
         "SpecialAbilityAttribute": [
             1,
             2,
             3,
             4,
             5,
             6,
-            7
+            7,
+            8
         ],
         "SpecialAbilityAttribute2": [],
         "SpecialAbilityAttribute3": [],
         "SpecialAbilityEffect": [],
         "SpecialAbilityHideClipName": [],
         "SpecialAbilityIcon": [],
         "SpecialAbilityInfo": [],
@@ -42590,166 +43172,181 @@
         "SpecialAbilitySpell": [
             "IceGolemFreeze",
             "IceGolemFreeze",
             "IceGolemFreeze",
             "IceGolemFreeze",
             "IceGolemFreeze",
             "IceGolemFreeze",
+            "IceGolemFreeze",
             "IceGolemFreeze"
         ],
         "SpecialAbilityType": [
             "CastSpellOnDeath",
             "CastSpellOnDeath",
             "CastSpellOnDeath",
             "CastSpellOnDeath",
             "CastSpellOnDeath",
             "CastSpellOnDeath",
+            "CastSpellOnDeath",
             "CastSpellOnDeath"
         ],
         "SpecialMovementMod": [],
         "Speed": [
             150,
             150,
             150,
             150,
             150,
             150,
+            150,
             150
         ],
         "Squad": [],
         "StrengthWeight": [
-            200,
-            300,
-            400,
-            500,
-            600,
-            700,
-            750
+            3000,
+            3500,
+            4000,
+            4500,
+            5000,
+            7000,
+            8000,
+            9000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
             "TID_ICEGOLEM",
             "TID_ICEGOLEM",
             "TID_ICEGOLEM",
             "TID_ICEGOLEM",
             "TID_ICEGOLEM",
             "TID_ICEGOLEM",
+            "TID_ICEGOLEM",
             "TID_ICEGOLEM"
         ],
         "TargetGroupsMinWeight": [],
         "TargetGroupsRadius": [],
         "TargetGroupsRange": [],
         "TargetedEffectOffset": [
             "-50",
             "-50",
             "-50",
             "-50",
             "-50",
             "-50",
+            "-50",
             "-50"
         ],
         "TombStone": [
             "DarkTombStone",
             "DarkTombStone",
             "DarkTombStone",
             "DarkTombStone",
             "DarkTombStone",
             "DarkTombStone",
+            "DarkTombStone",
             "DarkTombStone"
         ],
         "TrainingTime": [
             150,
             150,
             150,
             150,
             150,
             150,
+            150,
             150
         ],
         "TransitionEffectLv2": [],
         "TransitionEffectLv3": [],
         "TransitionEffectLv4": [],
         "TriggersTraps": [
             true,
             true,
             true,
             true,
             true,
             true,
+            true,
             true
         ],
         "UndergroundEffect": [],
         "UnderwaterEffect": [],
         "UnitsInCamp": [],
         "UpgradeCost": [
             55000,
             85000,
             100000,
             125000,
             240000,
             335000,
-            340000
+            360000,
+            360000
         ],
         "UpgradeLevelByTH": [],
         "UpgradeResource": [
             "DarkElixir",
             "DarkElixir",
             "DarkElixir",
             "DarkElixir",
             "DarkElixir",
             "DarkElixir",
+            "DarkElixir",
             "DarkElixir"
         ],
         "UpgradeTimeH": [
             68,
             96,
             120,
             156,
             264,
             318,
-            342
+            372,
+            372
         ],
         "UpgradeTimeM": [],
         "VillageType": [],
         "VisualLevel": [
             1,
             2,
             3,
             4,
             5,
             6,
-            7
+            7,
+            8
         ],
         "WallMovementCost": []
     },
     "Ice Golem_DEF": {
         "AirTargets": [
             false,
             false,
             false,
             false,
             false,
             false,
+            false,
             false
         ],
         "AltPreviewScenario": [],
         "AltProjectile": [],
         "Animation": [
             "IceGolem_lvl1",
             "IceGolem_lvl2",
             "IceGolem_lvl3",
             "IceGolem_lvl4",
             "IceGolem_lvl5",
             "IceGolem_lvl6",
-            "IceGolem_lvl7"
+            "IceGolem_lvl7",
+            "IceGolem_lvl8"
         ],
         "AreaDamageIgnoresWalls": [],
         "AttackCount": [],
         "AttackEffect": [],
         "AttackEffect2": [],
         "AttackEffectLv2": [],
         "AttackEffectLv3": [],
@@ -42758,23 +43355,25 @@
         "AttackRange": [
             100,
             100,
             100,
             100,
             100,
             100,
+            100,
             100
         ],
         "AttackSpeed": [
             2000,
             2000,
             2000,
             2000,
             2000,
             2000,
+            2000,
             2000
         ],
         "AuraSpell": [],
         "AuraSpellLevel": [],
         "AutoMergeDistance": [],
         "AutoMergeGroupSize": [],
         "AvoidNoiseInAttackPositionSelection": [],
@@ -42783,23 +43382,25 @@
         "BigPicture": [
             "unit_ice_golem_big",
             "unit_ice_golem_big",
             "unit_ice_golem_big",
             "unit_ice_golem_big",
             "unit_ice_golem_big",
             "unit_ice_golem_big",
+            "unit_ice_golem_big",
             "unit_ice_golem_big"
         ],
         "BigPictureSWF": [
             "sc/info_ice_golem.sc",
             "sc/info_ice_golem.sc",
             "sc/info_ice_golem.sc",
             "sc/info_ice_golem.sc",
             "sc/info_ice_golem.sc",
             "sc/info_ice_golem.sc",
+            "sc/info_ice_golem.sc",
             "sc/info_ice_golem.sc"
         ],
         "BoostAttackSpeed": [],
         "BoostDmgPerfect": [],
         "BoostRadius": [],
         "BoostedIfAlone": [],
         "BunkerDegenerationTime": [],
@@ -42822,15 +43423,16 @@
         "DPS": [
             24,
             28,
             32,
             36,
             40,
             44,
-            48
+            48,
+            52
         ],
         "DPSLv2": [],
         "DPSLv3": [],
         "Damage2": [],
         "Damage2Delay": [],
         "Damage2FalloffEnd": [],
         "Damage2FalloffStart": [],
@@ -42846,14 +43448,15 @@
         "DeployEffect": [
             "Icegolem Deploy",
             "Icegolem Deploy",
             "Icegolem Deploy",
             "Icegolem Deploy",
             "Icegolem Deploy",
             "Icegolem Deploy",
+            "Icegolem Deploy",
             "Icegolem Deploy"
         ],
         "DeployEffect2": [],
         "Deprecated": [],
         "DieDamage": [],
         "DieDamageDelay": [],
         "DieDamageEffect": [],
@@ -42861,25 +43464,27 @@
         "DieEffect": [
             "Giant Die",
             "Giant Die",
             "Giant Die",
             "Giant Die",
             "Giant Die",
             "Giant Die",
+            "Giant Die",
             "Giant Die"
         ],
         "DieEffect2": [],
         "DisableDonate": [],
         "DisableProduction": [
             true,
             true,
             true,
             true,
             true,
             true,
+            true,
             true
         ],
         "DoesNotOpenCC": [],
         "DonateCost": [],
         "DonateCount": [],
         "DonateXP": [],
         "EnabledByCalendar": [],
@@ -42887,135 +43492,148 @@
         "EnemyGroupWeight": [
             500,
             500,
             500,
             500,
             500,
             500,
+            500,
             500
         ],
         "EvolveEffect": [],
         "EvolveOnDamageDealt": [],
         "EvolveTime": [],
         "EvolveToCharacter": [],
         "FightWithGroups": [],
         "FriendlyGroupWeight": [
             600,
             600,
             600,
             600,
             600,
             600,
+            600,
             600
         ],
         "FrostOnHitPercent": [
             50,
             50,
             50,
             50,
             50,
             50,
+            50,
             50
         ],
         "FrostOnHitTime": [
             2000,
             2000,
             2000,
             2000,
             2000,
             2000,
+            2000,
             2000
         ],
         "GroundTargets": [
             true,
             true,
             true,
             true,
             true,
             true,
+            true,
             true
         ],
         "HealerWeight": [],
         "HealthReductionPerSecond": [],
         "HeroDamageMultiplier": [],
         "HideEffect": [],
         "HitEffect": [
             "IceWizard Hit1",
             "IceWizard Hit1",
             "IceWizard Hit1",
             "IceWizard Hit1",
             "IceWizard Hit1",
             "IceWizard Hit1",
+            "IceWizard Hit1",
             "IceWizard Hit1"
         ],
         "HitEffect2": [],
         "Hitpoints": [
             2600,
             2800,
             3000,
             3200,
             3400,
             3600,
-            3900
+            3900,
+            4200
         ],
         "HousingSpace": [
             15,
             15,
             15,
             15,
             15,
             15,
+            15,
             15
         ],
         "IconExportName": [
             "icon_unit_iceGolem",
             "icon_unit_iceGolem",
             "icon_unit_iceGolem",
             "icon_unit_iceGolem",
             "icon_unit_iceGolem",
             "icon_unit_iceGolem",
+            "icon_unit_iceGolem",
             "icon_unit_iceGolem"
         ],
         "IconSWF": [
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
+            "sc/ui.sc",
             "sc/ui.sc"
         ],
         "ImmuneToHealing": [],
         "IncreasingDamage": [],
         "InfoTID": [
             "TID_CHARACTER_INFO_ICEGOLEM",
             "TID_CHARACTER_INFO_ICEGOLEM",
             "TID_CHARACTER_INFO_ICEGOLEM",
             "TID_CHARACTER_INFO_ICEGOLEM",
             "TID_CHARACTER_INFO_ICEGOLEM",
             "TID_CHARACTER_INFO_ICEGOLEM",
+            "TID_CHARACTER_INFO_ICEGOLEM",
             "TID_CHARACTER_INFO_ICEGOLEM"
         ],
         "InvisibilityRadius": [],
         "IsFlying": [
             false,
             false,
             false,
             false,
             false,
             false,
+            false,
             false
         ],
         "IsJumper": [
             false,
             false,
             false,
             false,
             false,
             false,
+            false,
             false
         ],
         "IsSecondaryTroop": [],
         "IsUnderground": [],
         "JumpHeightPercent": [],
         "LaboratoryLevel": [],
         "LoseHpEffect": [],
@@ -43028,14 +43646,15 @@
         "MovementOffsetSpeed": [
             0,
             0,
             0,
             0,
             0,
             0,
+            0,
             0
         ],
         "MovingEffect": [],
         "Name": [],
         "NewTargetAttackDelay": [],
         "NoClipping": [],
         "PenetratingExtraRange": [],
@@ -43045,46 +43664,50 @@
         "PreAttackEffect": [
             "Icegolem Attack",
             "Icegolem Attack",
             "Icegolem Attack",
             "Icegolem Attack",
             "Icegolem Attack",
             "Icegolem Attack",
+            "Icegolem Attack",
             "Icegolem Attack"
         ],
         "PreferHeroes": [],
         "PreferedTargetBuilding": [],
         "PreferedTargetBuildingClass": [
             "Defense",
             "Defense",
             "Defense",
             "Defense",
             "Defense",
             "Defense",
+            "Defense",
             "Defense"
         ],
         "PreferedTargetDamageMod": [
             1,
             1,
             1,
             1,
             1,
             1,
+            1,
             1
         ],
         "PreferredMovementTarget": [],
         "PreferredTargetNoTargeting": [],
         "PreviewScenario": [],
         "ProductionBuilding": [
             "Dark Elixir Barrack",
             "Dark Elixir Barrack",
             "Dark Elixir Barrack",
             "Dark Elixir Barrack",
             "Dark Elixir Barrack",
             "Dark Elixir Barrack",
+            "Dark Elixir Barrack",
             "Dark Elixir Barrack"
         ],
         "Projectile": [],
         "ProjectileBounces": [],
         "ProjectileConsumesBunkerTroops": [],
         "PushbackAfterHit": [],
         "PushbackSpeed": [],
@@ -43106,14 +43729,15 @@
         "SpecialAbilityAttribute": [
             1,
             2,
             3,
             4,
             5,
             6,
+            6,
             6
         ],
         "SpecialAbilityAttribute2": [],
         "SpecialAbilityAttribute3": [],
         "SpecialAbilityEffect": [],
         "SpecialAbilityHideClipName": [],
         "SpecialAbilityIcon": [],
@@ -43123,33 +43747,36 @@
         "SpecialAbilitySpell": [
             "IceGolemFreeze_DEF",
             "IceGolemFreeze_DEF",
             "IceGolemFreeze_DEF",
             "IceGolemFreeze_DEF",
             "IceGolemFreeze_DEF",
             "IceGolemFreeze_DEF",
+            "IceGolemFreeze_DEF",
             "IceGolemFreeze_DEF"
         ],
         "SpecialAbilityType": [
             "CastSpellOnDeath",
             "CastSpellOnDeath",
             "CastSpellOnDeath",
             "CastSpellOnDeath",
             "CastSpellOnDeath",
             "CastSpellOnDeath",
+            "CastSpellOnDeath",
             "CastSpellOnDeath"
         ],
         "SpecialMovementMod": [],
         "Speed": [
             150,
             150,
             150,
             150,
             150,
             150,
+            150,
             150
         ],
         "Squad": [],
         "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
@@ -43159,48 +43786,52 @@
         "TID": [
             "TID_ICEGOLEM",
             "TID_ICEGOLEM",
             "TID_ICEGOLEM",
             "TID_ICEGOLEM",
             "TID_ICEGOLEM",
             "TID_ICEGOLEM",
+            "TID_ICEGOLEM",
             "TID_ICEGOLEM"
         ],
         "TargetGroupsMinWeight": [],
         "TargetGroupsRadius": [],
         "TargetGroupsRange": [],
         "TargetedEffectOffset": [
             "-50",
             "-50",
             "-50",
             "-50",
             "-50",
             "-50",
+            "-50",
             "-50"
         ],
         "TombStone": [
             "DarkTombStone",
             "DarkTombStone",
             "DarkTombStone",
             "DarkTombStone",
             "DarkTombStone",
             "DarkTombStone",
+            "DarkTombStone",
             "DarkTombStone"
         ],
         "TrainingTime": [],
         "TransitionEffectLv2": [],
         "TransitionEffectLv3": [],
         "TransitionEffectLv4": [],
         "TriggersTraps": [
             true,
             true,
             true,
             true,
             true,
             true,
+            true,
             true
         ],
         "UndergroundEffect": [],
         "UnderwaterEffect": [],
         "UnitsInCamp": [],
         "UpgradeCost": [],
         "UpgradeLevelByTH": [],
@@ -43211,15 +43842,16 @@
         "VisualLevel": [
             1,
             2,
             3,
             4,
             5,
             6,
-            7
+            7,
+            8
         ],
         "WallMovementCost": []
     },
     "Ice Hound": {
         "AirTargets": [
             false,
             false,
@@ -43690,22 +44322,15 @@
             250,
             250,
             250,
             250,
             250
         ],
         "Squad": [],
-        "StrengthWeight": [
-            550,
-            550,
-            550,
-            550,
-            550,
-            550
-        ],
+        "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
@@ -45146,28 +45771,15 @@
             160,
             160,
             160,
             160,
             160
         ],
         "Squad": [],
-        "StrengthWeight": [
-            150,
-            150,
-            150,
-            150,
-            150,
-            150,
-            150,
-            150,
-            150,
-            150,
-            150,
-            150
-        ],
+        "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
@@ -46189,26 +46801,15 @@
             225,
             225,
             225,
             225,
             225
         ],
         "Squad": [],
-        "StrengthWeight": [
-            200,
-            200,
-            200,
-            200,
-            200,
-            200,
-            200,
-            200,
-            200,
-            200
-        ],
+        "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
@@ -46579,17 +47180,15 @@
         "SpecialAbilitySpell": [],
         "SpecialAbilityType": [],
         "SpecialMovementMod": [],
         "Speed": [
             150
         ],
         "Squad": [],
-        "StrengthWeight": [
-            29
-        ],
+        "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
@@ -47315,26 +47914,15 @@
             200,
             200,
             200,
             200,
             200
         ],
         "Squad": [],
-        "StrengthWeight": [
-            90,
-            100,
-            110,
-            120,
-            150,
-            160,
-            180,
-            180,
-            200,
-            300
-        ],
+        "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
@@ -48546,24 +49134,24 @@
             400,
             400,
             400,
             400
         ],
         "Squad": [],
         "StrengthWeight": [
-            250,
-            350,
-            450,
-            450,
-            500,
-            550,
-            600,
-            650,
-            650,
-            650
+            3000,
+            3500,
+            4000,
+            4500,
+            5000,
+            6000,
+            7000,
+            8000,
+            9000,
+            10000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
@@ -51955,25 +52543,25 @@
             200,
             200,
             200,
             200
         ],
         "Squad": [],
         "StrengthWeight": [
-            120,
-            150,
-            180,
-            220,
-            350,
-            400,
-            400,
-            400,
-            400,
-            500,
-            500
+            1600,
+            1800,
+            2000,
+            2500,
+            3000,
+            4000,
+            5000,
+            6000,
+            7000,
+            9000,
+            10000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
@@ -53701,27 +54289,15 @@
             300,
             300,
             300,
             300,
             300
         ],
         "Squad": [],
-        "StrengthWeight": [
-            150,
-            150,
-            150,
-            150,
-            150,
-            150,
-            150,
-            150,
-            150,
-            150,
-            150
-        ],
+        "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
@@ -54067,17 +54643,15 @@
         "SpecialAbilitySpell": [],
         "SpecialAbilityType": [],
         "SpecialMovementMod": [],
         "Speed": [
             200
         ],
         "Squad": [],
-        "StrengthWeight": [
-            100
-        ],
+        "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
@@ -54345,17 +54919,291 @@
         "SpecialAbilitySpell": [],
         "SpecialAbilityType": [],
         "SpecialMovementMod": [],
         "Speed": [
             200
         ],
         "Squad": [],
-        "StrengthWeight": [
+        "StrengthWeight": [],
+        "SummonCooldown": [],
+        "SummonEffect": [],
+        "SummonLimit": [],
+        "SummonTime": [],
+        "SummonTroop": [],
+        "SummonTroopCount": [],
+        "TID": [
+            "TID_BARBARIAN"
+        ],
+        "TargetGroupsMinWeight": [],
+        "TargetGroupsRadius": [],
+        "TargetGroupsRange": [],
+        "TargetedEffectOffset": [
+            "-50"
+        ],
+        "TombStone": [
+            "TombStone"
+        ],
+        "TrainingTime": [
+            5
+        ],
+        "TransitionEffectLv2": [],
+        "TransitionEffectLv3": [],
+        "TransitionEffectLv4": [],
+        "TriggersTraps": [
+            true
+        ],
+        "UndergroundEffect": [],
+        "UnderwaterEffect": [],
+        "UnitsInCamp": [],
+        "UpgradeCost": [
+            25000
+        ],
+        "UpgradeLevelByTH": [],
+        "UpgradeResource": [
+            "Elixir"
+        ],
+        "UpgradeTimeH": [
+            6
+        ],
+        "UpgradeTimeM": [],
+        "VillageType": [],
+        "VisualLevel": [
+            1
+        ],
+        "WallMovementCost": []
+    },
+    "Prototype5": {
+        "AirTargets": [
+            false
+        ],
+        "AltPreviewScenario": [],
+        "AltProjectile": [],
+        "Animation": [
+            "Barbarian"
+        ],
+        "AreaDamageIgnoresWalls": [],
+        "AttackCount": [],
+        "AttackEffect": [
+            "Barbarian Attack"
+        ],
+        "AttackEffect2": [],
+        "AttackEffectLv2": [],
+        "AttackEffectLv3": [],
+        "AttackEffectLv4": [],
+        "AttackMultipleBuildings": [],
+        "AttackRange": [
+            40
+        ],
+        "AttackSpeed": [
+            1000
+        ],
+        "AuraSpell": [],
+        "AuraSpellLevel": [],
+        "AutoMergeDistance": [],
+        "AutoMergeGroupSize": [],
+        "AvoidNoiseInAttackPositionSelection": [],
+        "BarrackLevel": [
+            1
+        ],
+        "BecomesTargetableEffect": [],
+        "BigPicture": [
+            "unit_barbarian_big"
+        ],
+        "BigPictureSWF": [
+            "sc/info_barbarian.sc"
+        ],
+        "BoostAttackSpeed": [],
+        "BoostDmgPerfect": [],
+        "BoostRadius": [],
+        "BoostedIfAlone": [],
+        "BunkerDegenerationTime": [],
+        "BunkerSpawnDist": [],
+        "BunkerTroopCount1": [],
+        "BunkerTroopCount2": [],
+        "BunkerTroops": [],
+        "BurstCount": [],
+        "BurstDelay": [],
+        "CanAttackWhileMoving": [],
+        "CarryOverToNextStage": [],
+        "ChainAttackDamageReductionPercent": [],
+        "ChainAttackDelay": [],
+        "ChainAttackDistance": [],
+        "ChainAttackEffect": [],
+        "ChainAttackMaxTargets": [],
+        "ChainShootingDistance": [],
+        "CoolDownOverride": [],
+        "CustomDefenderIcon": [],
+        "DPS": [
+            8
+        ],
+        "DPSLv2": [],
+        "DPSLv3": [],
+        "Damage2": [],
+        "Damage2Delay": [],
+        "Damage2FalloffEnd": [],
+        "Damage2FalloffStart": [],
+        "Damage2Min": [],
+        "Damage2Radius": [],
+        "DamageMultiplierPercent": [],
+        "DamageMultiplierTarget": [],
+        "DamageRadius": [],
+        "DamageReductionToStorages": [],
+        "DefaultSkin": [],
+        "DefenseBonus": [],
+        "DefensiveTroop": [],
+        "DeployEffect": [
+            "Barbarian Deploy"
+        ],
+        "DeployEffect2": [],
+        "Deprecated": [],
+        "DieDamage": [],
+        "DieDamageDelay": [],
+        "DieDamageEffect": [],
+        "DieDamageRadius": [],
+        "DieEffect": [
+            "Barbarian Die"
+        ],
+        "DieEffect2": [],
+        "DisableDonate": [
+            true
+        ],
+        "DisableProduction": [
+            true
+        ],
+        "DoesNotOpenCC": [],
+        "DonateCost": [
+            1
+        ],
+        "DonateCount": [],
+        "DonateXP": [],
+        "EnabledByCalendar": [
+            true
+        ],
+        "EnabledBySuperLicence": [],
+        "EnemyGroupWeight": [
+            100
+        ],
+        "EvolveEffect": [],
+        "EvolveOnDamageDealt": [],
+        "EvolveTime": [],
+        "EvolveToCharacter": [],
+        "FightWithGroups": [],
+        "FriendlyGroupWeight": [
             100
         ],
+        "FrostOnHitPercent": [],
+        "FrostOnHitTime": [],
+        "GroundTargets": [
+            true
+        ],
+        "HealerWeight": [],
+        "HealthReductionPerSecond": [],
+        "HeroDamageMultiplier": [],
+        "HideEffect": [],
+        "HitEffect": [
+            "Barbarian Hit"
+        ],
+        "HitEffect2": [],
+        "Hitpoints": [
+            45
+        ],
+        "HousingSpace": [
+            1
+        ],
+        "IconExportName": [
+            "icon_unit_barbarian"
+        ],
+        "IconSWF": [
+            "sc/ui.sc"
+        ],
+        "ImmuneToHealing": [],
+        "IncreasingDamage": [],
+        "InfoTID": [
+            "TID_CHARACTER_INFO_BARBARIAN"
+        ],
+        "InvisibilityRadius": [],
+        "IsFlying": [
+            false
+        ],
+        "IsJumper": [
+            false
+        ],
+        "IsSecondaryTroop": [],
+        "IsUnderground": [],
+        "JumpHeightPercent": [],
+        "LaboratoryLevel": [
+            1
+        ],
+        "LoseHpEffect": [],
+        "LoseHpInterval": [],
+        "LoseHpPerTick": [],
+        "Lv2SwitchTime": [],
+        "Lv3SwitchTime": [],
+        "MoveStartsEffect": [],
+        "MovementOffsetAmount": [],
+        "MovementOffsetSpeed": [
+            0
+        ],
+        "MovingEffect": [],
+        "NewTargetAttackDelay": [],
+        "NoClipping": [],
+        "PenetratingExtraRange": [],
+        "PenetratingProjectile": [],
+        "PenetratingRadius": [],
+        "PickNewTargetAfterPushback": [],
+        "PreAttackEffect": [],
+        "PreferHeroes": [],
+        "PreferedTargetBuilding": [],
+        "PreferedTargetBuildingClass": [],
+        "PreferedTargetDamageMod": [
+            1
+        ],
+        "PreferredMovementTarget": [],
+        "PreferredTargetNoTargeting": [],
+        "PreviewScenario": [],
+        "ProductionBuilding": [
+            "Barrack"
+        ],
+        "Projectile": [],
+        "ProjectileBounces": [],
+        "ProjectileConsumesBunkerTroops": [],
+        "PushbackAfterHit": [],
+        "PushbackSpeed": [],
+        "RandomizeSecSpawnDist": [],
+        "ReflectsDamage": [],
+        "RetargetAfterHit": [],
+        "ScaleByTH": [],
+        "SecondarySpawnDist": [],
+        "SecondarySpawnOffset": [],
+        "SecondaryTroop": [],
+        "SecondaryTroopCnt": [],
+        "SelfAsAoeCenter": [],
+        "SmoothJump": [],
+        "SpawnIdle": [],
+        "SpawnOnAttack": [],
+        "SpawnWhenDamaged": [],
+        "SpecialAbilities": [],
+        "SpecialAbilitiesLevel": [],
+        "SpecialAbilityAttribute": [],
+        "SpecialAbilityAttribute2": [],
+        "SpecialAbilityAttribute3": [],
+        "SpecialAbilityEffect": [],
+        "SpecialAbilityHideClipName": [],
+        "SpecialAbilityIcon": [],
+        "SpecialAbilityInfo": [],
+        "SpecialAbilityLevel": [],
+        "SpecialAbilityName": [],
+        "SpecialAbilitySpell": [],
+        "SpecialAbilityType": [],
+        "SpecialMovementMod": [],
+        "Speed": [
+            200
+        ],
+        "Squad": [],
+        "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
@@ -54395,15 +55243,15 @@
         "UpgradeTimeM": [],
         "VillageType": [],
         "VisualLevel": [
             1
         ],
         "WallMovementCost": []
     },
-    "Prototype5": {
+    "Prototype6": {
         "AirTargets": [
             false
         ],
         "AltPreviewScenario": [],
         "AltProjectile": [],
         "Animation": [
             "Barbarian"
@@ -54623,17 +55471,291 @@
         "SpecialAbilitySpell": [],
         "SpecialAbilityType": [],
         "SpecialMovementMod": [],
         "Speed": [
             200
         ],
         "Squad": [],
-        "StrengthWeight": [
+        "StrengthWeight": [],
+        "SummonCooldown": [],
+        "SummonEffect": [],
+        "SummonLimit": [],
+        "SummonTime": [],
+        "SummonTroop": [],
+        "SummonTroopCount": [],
+        "TID": [
+            "TID_BARBARIAN"
+        ],
+        "TargetGroupsMinWeight": [],
+        "TargetGroupsRadius": [],
+        "TargetGroupsRange": [],
+        "TargetedEffectOffset": [
+            "-50"
+        ],
+        "TombStone": [
+            "TombStone"
+        ],
+        "TrainingTime": [
+            5
+        ],
+        "TransitionEffectLv2": [],
+        "TransitionEffectLv3": [],
+        "TransitionEffectLv4": [],
+        "TriggersTraps": [
+            true
+        ],
+        "UndergroundEffect": [],
+        "UnderwaterEffect": [],
+        "UnitsInCamp": [],
+        "UpgradeCost": [
+            25000
+        ],
+        "UpgradeLevelByTH": [],
+        "UpgradeResource": [
+            "Elixir"
+        ],
+        "UpgradeTimeH": [
+            6
+        ],
+        "UpgradeTimeM": [],
+        "VillageType": [],
+        "VisualLevel": [
+            1
+        ],
+        "WallMovementCost": []
+    },
+    "Prototype7": {
+        "AirTargets": [
+            false
+        ],
+        "AltPreviewScenario": [],
+        "AltProjectile": [],
+        "Animation": [
+            "Barbarian"
+        ],
+        "AreaDamageIgnoresWalls": [],
+        "AttackCount": [],
+        "AttackEffect": [
+            "Barbarian Attack"
+        ],
+        "AttackEffect2": [],
+        "AttackEffectLv2": [],
+        "AttackEffectLv3": [],
+        "AttackEffectLv4": [],
+        "AttackMultipleBuildings": [],
+        "AttackRange": [
+            40
+        ],
+        "AttackSpeed": [
+            1000
+        ],
+        "AuraSpell": [],
+        "AuraSpellLevel": [],
+        "AutoMergeDistance": [],
+        "AutoMergeGroupSize": [],
+        "AvoidNoiseInAttackPositionSelection": [],
+        "BarrackLevel": [
+            1
+        ],
+        "BecomesTargetableEffect": [],
+        "BigPicture": [
+            "unit_barbarian_big"
+        ],
+        "BigPictureSWF": [
+            "sc/info_barbarian.sc"
+        ],
+        "BoostAttackSpeed": [],
+        "BoostDmgPerfect": [],
+        "BoostRadius": [],
+        "BoostedIfAlone": [],
+        "BunkerDegenerationTime": [],
+        "BunkerSpawnDist": [],
+        "BunkerTroopCount1": [],
+        "BunkerTroopCount2": [],
+        "BunkerTroops": [],
+        "BurstCount": [],
+        "BurstDelay": [],
+        "CanAttackWhileMoving": [],
+        "CarryOverToNextStage": [],
+        "ChainAttackDamageReductionPercent": [],
+        "ChainAttackDelay": [],
+        "ChainAttackDistance": [],
+        "ChainAttackEffect": [],
+        "ChainAttackMaxTargets": [],
+        "ChainShootingDistance": [],
+        "CoolDownOverride": [],
+        "CustomDefenderIcon": [],
+        "DPS": [
+            8
+        ],
+        "DPSLv2": [],
+        "DPSLv3": [],
+        "Damage2": [],
+        "Damage2Delay": [],
+        "Damage2FalloffEnd": [],
+        "Damage2FalloffStart": [],
+        "Damage2Min": [],
+        "Damage2Radius": [],
+        "DamageMultiplierPercent": [],
+        "DamageMultiplierTarget": [],
+        "DamageRadius": [],
+        "DamageReductionToStorages": [],
+        "DefaultSkin": [],
+        "DefenseBonus": [],
+        "DefensiveTroop": [],
+        "DeployEffect": [
+            "Barbarian Deploy"
+        ],
+        "DeployEffect2": [],
+        "Deprecated": [],
+        "DieDamage": [],
+        "DieDamageDelay": [],
+        "DieDamageEffect": [],
+        "DieDamageRadius": [],
+        "DieEffect": [
+            "Barbarian Die"
+        ],
+        "DieEffect2": [],
+        "DisableDonate": [
+            true
+        ],
+        "DisableProduction": [
+            true
+        ],
+        "DoesNotOpenCC": [],
+        "DonateCost": [
+            1
+        ],
+        "DonateCount": [],
+        "DonateXP": [],
+        "EnabledByCalendar": [
+            true
+        ],
+        "EnabledBySuperLicence": [],
+        "EnemyGroupWeight": [
+            100
+        ],
+        "EvolveEffect": [],
+        "EvolveOnDamageDealt": [],
+        "EvolveTime": [],
+        "EvolveToCharacter": [],
+        "FightWithGroups": [],
+        "FriendlyGroupWeight": [
             100
         ],
+        "FrostOnHitPercent": [],
+        "FrostOnHitTime": [],
+        "GroundTargets": [
+            true
+        ],
+        "HealerWeight": [],
+        "HealthReductionPerSecond": [],
+        "HeroDamageMultiplier": [],
+        "HideEffect": [],
+        "HitEffect": [
+            "Barbarian Hit"
+        ],
+        "HitEffect2": [],
+        "Hitpoints": [
+            45
+        ],
+        "HousingSpace": [
+            1
+        ],
+        "IconExportName": [
+            "icon_unit_barbarian"
+        ],
+        "IconSWF": [
+            "sc/ui.sc"
+        ],
+        "ImmuneToHealing": [],
+        "IncreasingDamage": [],
+        "InfoTID": [
+            "TID_CHARACTER_INFO_BARBARIAN"
+        ],
+        "InvisibilityRadius": [],
+        "IsFlying": [
+            false
+        ],
+        "IsJumper": [
+            false
+        ],
+        "IsSecondaryTroop": [],
+        "IsUnderground": [],
+        "JumpHeightPercent": [],
+        "LaboratoryLevel": [
+            1
+        ],
+        "LoseHpEffect": [],
+        "LoseHpInterval": [],
+        "LoseHpPerTick": [],
+        "Lv2SwitchTime": [],
+        "Lv3SwitchTime": [],
+        "MoveStartsEffect": [],
+        "MovementOffsetAmount": [],
+        "MovementOffsetSpeed": [
+            0
+        ],
+        "MovingEffect": [],
+        "NewTargetAttackDelay": [],
+        "NoClipping": [],
+        "PenetratingExtraRange": [],
+        "PenetratingProjectile": [],
+        "PenetratingRadius": [],
+        "PickNewTargetAfterPushback": [],
+        "PreAttackEffect": [],
+        "PreferHeroes": [],
+        "PreferedTargetBuilding": [],
+        "PreferedTargetBuildingClass": [],
+        "PreferedTargetDamageMod": [
+            1
+        ],
+        "PreferredMovementTarget": [],
+        "PreferredTargetNoTargeting": [],
+        "PreviewScenario": [],
+        "ProductionBuilding": [
+            "Barrack"
+        ],
+        "Projectile": [],
+        "ProjectileBounces": [],
+        "ProjectileConsumesBunkerTroops": [],
+        "PushbackAfterHit": [],
+        "PushbackSpeed": [],
+        "RandomizeSecSpawnDist": [],
+        "ReflectsDamage": [],
+        "RetargetAfterHit": [],
+        "ScaleByTH": [],
+        "SecondarySpawnDist": [],
+        "SecondarySpawnOffset": [],
+        "SecondaryTroop": [],
+        "SecondaryTroopCnt": [],
+        "SelfAsAoeCenter": [],
+        "SmoothJump": [],
+        "SpawnIdle": [],
+        "SpawnOnAttack": [],
+        "SpawnWhenDamaged": [],
+        "SpecialAbilities": [],
+        "SpecialAbilitiesLevel": [],
+        "SpecialAbilityAttribute": [],
+        "SpecialAbilityAttribute2": [],
+        "SpecialAbilityAttribute3": [],
+        "SpecialAbilityEffect": [],
+        "SpecialAbilityHideClipName": [],
+        "SpecialAbilityIcon": [],
+        "SpecialAbilityInfo": [],
+        "SpecialAbilityLevel": [],
+        "SpecialAbilityName": [],
+        "SpecialAbilitySpell": [],
+        "SpecialAbilityType": [],
+        "SpecialMovementMod": [],
+        "Speed": [
+            200
+        ],
+        "Squad": [],
+        "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
@@ -55096,23 +56218,15 @@
             200,
             200,
             200,
             200,
             200
         ],
         "Squad": [],
-        "StrengthWeight": [
-            100,
-            100,
-            90,
-            80,
-            70,
-            65,
-            60
-        ],
+        "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
@@ -55613,23 +56727,15 @@
             200,
             200,
             200,
             200,
             200
         ],
         "Squad": [],
-        "StrengthWeight": [
-            100,
-            100,
-            90,
-            80,
-            70,
-            65,
-            60
-        ],
+        "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
@@ -56274,27 +57380,15 @@
             280,
             280,
             280,
             280,
             280
         ],
         "Squad": [],
-        "StrengthWeight": [
-            150,
-            150,
-            150,
-            150,
-            150,
-            150,
-            150,
-            150,
-            150,
-            150,
-            150
-        ],
+        "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
@@ -56985,29 +58079,15 @@
             400,
             400,
             400,
             400,
             400
         ],
         "Squad": [],
-        "StrengthWeight": [
-            150,
-            150,
-            150,
-            150,
-            150,
-            150,
-            150,
-            150,
-            150,
-            150,
-            150,
-            150,
-            150
-        ],
+        "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
@@ -57425,17 +58505,17 @@
         "Speed": [
             150,
             150,
             150
         ],
         "Squad": [],
         "StrengthWeight": [
-            400,
-            440,
-            480
+            8000,
+            9000,
+            10000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
@@ -57957,23 +59037,15 @@
             200,
             200,
             200,
             200,
             200
         ],
         "Squad": [],
-        "StrengthWeight": [
-            86,
-            86,
-            86,
-            86,
-            86,
-            86,
-            86
-        ],
+        "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
@@ -58339,14 +59411,751 @@
         "UpgradeTimeM": [],
         "VillageType": [],
         "VisualLevel": [
             1
         ],
         "WallMovementCost": []
     },
+    "Side Thrower": {
+        "AirTargets": [
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false
+        ],
+        "AltPreviewScenario": [],
+        "AltProjectile": [],
+        "Animation": [
+            "FootballGiant",
+            "FootballGiant",
+            "FootballGiant",
+            "FootballGiant",
+            "FootballGiant",
+            "FootballGiant",
+            "FootballGiant",
+            "FootballGiant",
+            "FootballGiant",
+            "FootballGiant",
+            "FootballGiant"
+        ],
+        "AreaDamageIgnoresWalls": [],
+        "AttackCount": [],
+        "AttackEffect": [
+            "Giant_Football_Atk",
+            "Giant_Football_Atk",
+            "Giant_Football_Atk",
+            "Giant_Football_Atk",
+            "Giant_Football_Atk",
+            "Giant_Football_Atk",
+            "Giant_Football_Atk",
+            "Giant_Football_Atk",
+            "Giant_Football_Atk",
+            "Giant_Football_Atk",
+            "Giant_Football_Atk"
+        ],
+        "AttackEffect2": [],
+        "AttackEffectLv2": [],
+        "AttackEffectLv3": [],
+        "AttackEffectLv4": [],
+        "AttackMultipleBuildings": [],
+        "AttackRange": [
+            70,
+            70,
+            70,
+            70,
+            70,
+            70,
+            70,
+            70,
+            70,
+            70,
+            70
+        ],
+        "AttackSpeed": [
+            1800,
+            1800,
+            1800,
+            1800,
+            1800,
+            1800,
+            1800,
+            1800,
+            1800,
+            1800,
+            1800
+        ],
+        "AuraSpell": [],
+        "AuraSpellLevel": [],
+        "AutoMergeDistance": [],
+        "AutoMergeGroupSize": [],
+        "AvoidNoiseInAttackPositionSelection": [],
+        "BarrackLevel": [
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1
+        ],
+        "BecomesTargetableEffect": [],
+        "BigPicture": [
+            "unit_football_giant_big",
+            "unit_football_giant_big",
+            "unit_football_giant_big",
+            "unit_football_giant_big",
+            "unit_football_giant_big",
+            "unit_football_giant_big",
+            "unit_football_giant_big",
+            "unit_football_giant_big",
+            "unit_football_giant_big",
+            "unit_football_giant_big",
+            "unit_football_giant_big"
+        ],
+        "BigPictureSWF": [
+            "sc/info_football_giant.sc",
+            "sc/info_football_giant.sc",
+            "sc/info_football_giant.sc",
+            "sc/info_football_giant.sc",
+            "sc/info_football_giant.sc",
+            "sc/info_football_giant.sc",
+            "sc/info_football_giant.sc",
+            "sc/info_football_giant.sc",
+            "sc/info_football_giant.sc",
+            "sc/info_football_giant.sc",
+            "sc/info_football_giant.sc"
+        ],
+        "BoostAttackSpeed": [],
+        "BoostDmgPerfect": [],
+        "BoostRadius": [],
+        "BoostedIfAlone": [],
+        "BunkerDegenerationTime": [],
+        "BunkerSpawnDist": [],
+        "BunkerTroopCount1": [],
+        "BunkerTroopCount2": [],
+        "BunkerTroops": [],
+        "BurstCount": [],
+        "BurstDelay": [],
+        "CanAttackWhileMoving": [],
+        "CarryOverToNextStage": [],
+        "ChainAttackDamageReductionPercent": [],
+        "ChainAttackDelay": [],
+        "ChainAttackDistance": [],
+        "ChainAttackEffect": [],
+        "ChainAttackMaxTargets": [],
+        "ChainShootingDistance": [],
+        "CoolDownOverride": [],
+        "CustomDefenderIcon": [],
+        "DPS": [
+            100,
+            110,
+            120,
+            130,
+            140,
+            150,
+            160,
+            170,
+            180,
+            190,
+            200
+        ],
+        "DPSLv2": [],
+        "DPSLv3": [],
+        "Damage2": [],
+        "Damage2Delay": [],
+        "Damage2FalloffEnd": [],
+        "Damage2FalloffStart": [],
+        "Damage2Min": [],
+        "Damage2Radius": [],
+        "DamageMultiplierPercent": [],
+        "DamageMultiplierTarget": [],
+        "DamageRadius": [],
+        "DamageReductionToStorages": [],
+        "DefaultSkin": [],
+        "DefenseBonus": [],
+        "DefensiveTroop": [],
+        "DeployEffect": [
+            "Giant_Football_Deploy",
+            "Giant_Football_Deploy",
+            "Giant_Football_Deploy",
+            "Giant_Football_Deploy",
+            "Giant_Football_Deploy",
+            "Giant_Football_Deploy",
+            "Giant_Football_Deploy",
+            "Giant_Football_Deploy",
+            "Giant_Football_Deploy",
+            "Giant_Football_Deploy",
+            "Giant_Football_Deploy"
+        ],
+        "DeployEffect2": [],
+        "Deprecated": [],
+        "DieDamage": [],
+        "DieDamageDelay": [],
+        "DieDamageEffect": [],
+        "DieDamageRadius": [],
+        "DieEffect": [
+            "Giant_Football_Die",
+            "Giant_Football_Die",
+            "Giant_Football_Die",
+            "Giant_Football_Die",
+            "Giant_Football_Die",
+            "Giant_Football_Die",
+            "Giant_Football_Die",
+            "Giant_Football_Die",
+            "Giant_Football_Die",
+            "Giant_Football_Die",
+            "Giant_Football_Die"
+        ],
+        "DieEffect2": [],
+        "DisableDonate": [
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true
+        ],
+        "DisableProduction": [],
+        "DoesNotOpenCC": [],
+        "DonateCost": [
+            10,
+            10,
+            10,
+            10,
+            10,
+            10,
+            10,
+            10,
+            10,
+            10,
+            10
+        ],
+        "DonateCount": [],
+        "DonateXP": [],
+        "EnabledByCalendar": [
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true
+        ],
+        "EnabledBySuperLicence": [],
+        "EnemyGroupWeight": [
+            600,
+            600,
+            600,
+            600,
+            600,
+            600,
+            600,
+            600,
+            600,
+            600,
+            600
+        ],
+        "EvolveEffect": [],
+        "EvolveOnDamageDealt": [],
+        "EvolveTime": [],
+        "EvolveToCharacter": [],
+        "FightWithGroups": [],
+        "FriendlyGroupWeight": [
+            600,
+            600,
+            600,
+            600,
+            600,
+            600,
+            600,
+            600,
+            600,
+            600,
+            600
+        ],
+        "FrostOnHitPercent": [],
+        "FrostOnHitTime": [],
+        "GroundTargets": [
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true
+        ],
+        "HealerWeight": [],
+        "HealthReductionPerSecond": [],
+        "HeroDamageMultiplier": [],
+        "HideEffect": [],
+        "HitEffect": [
+            "Giant Hit",
+            "Giant Hit",
+            "Giant Hit",
+            "Giant Hit",
+            "Giant Hit",
+            "Giant Hit",
+            "Giant Hit",
+            "Giant Hit",
+            "Giant Hit",
+            "Giant Hit",
+            "Giant Hit"
+        ],
+        "HitEffect2": [],
+        "Hitpoints": [
+            500,
+            750,
+            1400,
+            1700,
+            1900,
+            2200,
+            2500,
+            2800,
+            3100,
+            3400,
+            3600
+        ],
+        "HousingSpace": [
+            15,
+            15,
+            15,
+            15,
+            15,
+            15,
+            15,
+            15,
+            15,
+            15,
+            15
+        ],
+        "IconExportName": [
+            "icon_unit_footballgiant",
+            "icon_unit_footballgiant",
+            "icon_unit_footballgiant",
+            "icon_unit_footballgiant",
+            "icon_unit_footballgiant",
+            "icon_unit_footballgiant",
+            "icon_unit_footballgiant",
+            "icon_unit_footballgiant",
+            "icon_unit_footballgiant",
+            "icon_unit_footballgiant",
+            "icon_unit_footballgiant"
+        ],
+        "IconSWF": [
+            "sc/update.sc",
+            "sc/update.sc",
+            "sc/update.sc",
+            "sc/update.sc",
+            "sc/update.sc",
+            "sc/update.sc",
+            "sc/update.sc",
+            "sc/update.sc",
+            "sc/update.sc",
+            "sc/update.sc",
+            "sc/update.sc"
+        ],
+        "ImmuneToHealing": [],
+        "IncreasingDamage": [],
+        "InfoTID": [
+            "TID_CHARACTER_INFO_SIDE_THROWER",
+            "TID_CHARACTER_INFO_SIDE_THROWER",
+            "TID_CHARACTER_INFO_SIDE_THROWER",
+            "TID_CHARACTER_INFO_SIDE_THROWER",
+            "TID_CHARACTER_INFO_SIDE_THROWER",
+            "TID_CHARACTER_INFO_SIDE_THROWER",
+            "TID_CHARACTER_INFO_SIDE_THROWER",
+            "TID_CHARACTER_INFO_SIDE_THROWER",
+            "TID_CHARACTER_INFO_SIDE_THROWER",
+            "TID_CHARACTER_INFO_SIDE_THROWER",
+            "TID_CHARACTER_INFO_SIDE_THROWER"
+        ],
+        "InvisibilityRadius": [],
+        "IsFlying": [
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false
+        ],
+        "IsJumper": [
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false
+        ],
+        "IsSecondaryTroop": [],
+        "IsUnderground": [],
+        "JumpHeightPercent": [],
+        "LaboratoryLevel": [
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1
+        ],
+        "LoseHpEffect": [],
+        "LoseHpInterval": [],
+        "LoseHpPerTick": [],
+        "Lv2SwitchTime": [],
+        "Lv3SwitchTime": [],
+        "MoveStartsEffect": [],
+        "MovementOffsetAmount": [],
+        "MovementOffsetSpeed": [
+            0,
+            0,
+            0,
+            0,
+            0,
+            0,
+            0,
+            0,
+            0,
+            0,
+            0
+        ],
+        "MovingEffect": [],
+        "Name": [],
+        "NewTargetAttackDelay": [],
+        "NoClipping": [],
+        "PenetratingExtraRange": [],
+        "PenetratingProjectile": [],
+        "PenetratingRadius": [],
+        "PickNewTargetAfterPushback": [],
+        "PreAttackEffect": [],
+        "PreferHeroes": [],
+        "PreferedTargetBuilding": [],
+        "PreferedTargetBuildingClass": [
+            "Defense",
+            "Defense",
+            "Defense",
+            "Defense",
+            "Defense",
+            "Defense",
+            "Defense",
+            "Defense",
+            "Defense",
+            "Defense",
+            "Defense"
+        ],
+        "PreferedTargetDamageMod": [],
+        "PreferredMovementTarget": [],
+        "PreferredTargetNoTargeting": [],
+        "PreviewScenario": [
+            "TroopSideThrower",
+            "TroopSideThrower",
+            "TroopSideThrower",
+            "TroopSideThrower",
+            "TroopSideThrower",
+            "TroopSideThrower",
+            "TroopSideThrower",
+            "TroopSideThrower",
+            "TroopSideThrower",
+            "TroopSideThrower",
+            "TroopSideThrower"
+        ],
+        "ProductionBuilding": [
+            "Barrack",
+            "Barrack",
+            "Barrack",
+            "Barrack",
+            "Barrack",
+            "Barrack",
+            "Barrack",
+            "Barrack",
+            "Barrack",
+            "Barrack",
+            "Barrack"
+        ],
+        "Projectile": [],
+        "ProjectileBounces": [],
+        "ProjectileConsumesBunkerTroops": [],
+        "PushbackAfterHit": [],
+        "PushbackSpeed": [],
+        "RandomizeSecSpawnDist": [],
+        "ReflectsDamage": [],
+        "RetargetAfterHit": [],
+        "ScaleByTH": [],
+        "SecondarySpawnDist": [],
+        "SecondarySpawnOffset": [],
+        "SecondaryTroop": [],
+        "SecondaryTroopCnt": [],
+        "SelfAsAoeCenter": [],
+        "SmoothJump": [],
+        "SpawnIdle": [],
+        "SpawnOnAttack": [],
+        "SpawnWhenDamaged": [],
+        "SpecialAbilities": [
+            "ThrowIn",
+            "ThrowIn",
+            "ThrowIn",
+            "ThrowIn",
+            "ThrowIn",
+            "ThrowIn",
+            "ThrowIn",
+            "ThrowIn",
+            "ThrowIn",
+            "ThrowIn",
+            "ThrowIn"
+        ],
+        "SpecialAbilitiesLevel": [
+            1,
+            2,
+            3,
+            4,
+            5,
+            6,
+            7,
+            8,
+            9,
+            10,
+            11
+        ],
+        "SpecialAbilityAttribute": [
+            150,
+            300,
+            450,
+            600,
+            780,
+            975,
+            1080,
+            1200,
+            1350,
+            1500,
+            1650
+        ],
+        "SpecialAbilityAttribute2": [],
+        "SpecialAbilityAttribute3": [],
+        "SpecialAbilityEffect": [],
+        "SpecialAbilityHideClipName": [],
+        "SpecialAbilityIcon": [],
+        "SpecialAbilityInfo": [
+            "TID_ABILITY_THROW_IN_INFO",
+            "TID_ABILITY_THROW_IN_INFO",
+            "TID_ABILITY_THROW_IN_INFO",
+            "TID_ABILITY_THROW_IN_INFO",
+            "TID_ABILITY_THROW_IN_INFO",
+            "TID_ABILITY_THROW_IN_INFO",
+            "TID_ABILITY_THROW_IN_INFO",
+            "TID_ABILITY_THROW_IN_INFO",
+            "TID_ABILITY_THROW_IN_INFO",
+            "TID_ABILITY_THROW_IN_INFO",
+            "TID_ABILITY_THROW_IN_INFO"
+        ],
+        "SpecialAbilityLevel": [
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1
+        ],
+        "SpecialAbilityName": [
+            "TID_ABILITY_THROW_IN",
+            "TID_ABILITY_THROW_IN",
+            "TID_ABILITY_THROW_IN",
+            "TID_ABILITY_THROW_IN",
+            "TID_ABILITY_THROW_IN",
+            "TID_ABILITY_THROW_IN",
+            "TID_ABILITY_THROW_IN",
+            "TID_ABILITY_THROW_IN",
+            "TID_ABILITY_THROW_IN",
+            "TID_ABILITY_THROW_IN",
+            "TID_ABILITY_THROW_IN"
+        ],
+        "SpecialAbilitySpell": [],
+        "SpecialAbilityType": [],
+        "SpecialMovementMod": [],
+        "Speed": [
+            200,
+            200,
+            200,
+            200,
+            200,
+            200,
+            200,
+            200,
+            200,
+            200,
+            200
+        ],
+        "Squad": [],
+        "StrengthWeight": [],
+        "SummonCooldown": [],
+        "SummonEffect": [],
+        "SummonLimit": [],
+        "SummonTime": [],
+        "SummonTroop": [],
+        "SummonTroopCount": [],
+        "TID": [
+            "TID_CHARACTER_SIDE_THROWER",
+            "TID_CHARACTER_SIDE_THROWER",
+            "TID_CHARACTER_SIDE_THROWER",
+            "TID_CHARACTER_SIDE_THROWER",
+            "TID_CHARACTER_SIDE_THROWER",
+            "TID_CHARACTER_SIDE_THROWER",
+            "TID_CHARACTER_SIDE_THROWER",
+            "TID_CHARACTER_SIDE_THROWER",
+            "TID_CHARACTER_SIDE_THROWER",
+            "TID_CHARACTER_SIDE_THROWER",
+            "TID_CHARACTER_SIDE_THROWER"
+        ],
+        "TargetGroupsMinWeight": [],
+        "TargetGroupsRadius": [],
+        "TargetGroupsRange": [],
+        "TargetedEffectOffset": [
+            "-50",
+            "-50",
+            "-50",
+            "-50",
+            "-50",
+            "-50",
+            "-50",
+            "-50",
+            "-50",
+            "-50",
+            "-50"
+        ],
+        "TombStone": [
+            "TombStone",
+            "TombStone",
+            "TombStone",
+            "TombStone",
+            "TombStone",
+            "TombStone",
+            "TombStone",
+            "TombStone",
+            "TombStone",
+            "TombStone",
+            "TombStone"
+        ],
+        "TrainingTime": [
+            120,
+            120,
+            120,
+            120,
+            120,
+            120,
+            120,
+            120,
+            120,
+            120,
+            120
+        ],
+        "TransitionEffectLv2": [],
+        "TransitionEffectLv3": [],
+        "TransitionEffectLv4": [],
+        "TriggersTraps": [
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true
+        ],
+        "UndergroundEffect": [],
+        "UnderwaterEffect": [],
+        "UnitsInCamp": [],
+        "UpgradeCost": [],
+        "UpgradeLevelByTH": [
+            6,
+            7,
+            8,
+            9,
+            10,
+            11,
+            12,
+            13,
+            14,
+            15,
+            16
+        ],
+        "UpgradeResource": [
+            "Elixir",
+            "Elixir",
+            "Elixir",
+            "Elixir",
+            "Elixir",
+            "Elixir",
+            "Elixir",
+            "Elixir",
+            "Elixir",
+            "Elixir",
+            "Elixir"
+        ],
+        "UpgradeTimeH": [],
+        "UpgradeTimeM": [],
+        "VillageType": [],
+        "VisualLevel": [
+            1,
+            2,
+            3,
+            4,
+            5,
+            6,
+            7,
+            8,
+            9,
+            10,
+            11
+        ],
+        "WallMovementCost": []
+    },
     "Siege Bowler Balloon": {
         "AirTargets": [
             false,
             false,
             false,
             false,
             false
@@ -58789,19 +60598,19 @@
             200,
             200,
             200,
             200
         ],
         "Squad": [],
         "StrengthWeight": [
-            25,
-            25,
-            25,
-            25,
-            25
+            6000,
+            6500,
+            7000,
+            8000,
+            10000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
@@ -58883,76 +60692,85 @@
         "WallMovementCost": []
     },
     "Siege Catapult": {
         "AirTargets": [
             false,
             false,
             false,
+            false,
             false
         ],
         "AltPreviewScenario": [],
         "AltProjectile": [],
         "Animation": [
             "SiegeMachine_Catapult_lvl1",
             "SiegeMachine_Catapult_lvl2",
             "SiegeMachine_Catapult_lvl3",
-            "SiegeMachine_Catapult_lvl4"
+            "SiegeMachine_Catapult_lvl4",
+            "SiegeMachine_Catapult_lvl5"
         ],
         "AreaDamageIgnoresWalls": [],
         "AttackCount": [],
         "AttackEffect": [
             "Catapult Attack",
             "Catapult Attack",
             "Catapult Attack",
+            "Catapult Attack",
             "Catapult Attack"
         ],
         "AttackEffect2": [],
         "AttackEffectLv2": [],
         "AttackEffectLv3": [],
         "AttackEffectLv4": [],
         "AttackMultipleBuildings": [],
         "AttackRange": [
             1005,
             1005,
             1005,
+            1005,
             1005
         ],
         "AttackSpeed": [
             5000,
             5000,
             5000,
+            5000,
             5000
         ],
         "AuraSpell": [],
         "AuraSpellLevel": [],
         "AutoMergeDistance": [],
         "AutoMergeGroupSize": [],
         "AvoidNoiseInAttackPositionSelection": [
             true,
             true,
             true,
+            true,
             true
         ],
         "BarrackLevel": [
             6,
             6,
             6,
+            6,
             6
         ],
         "BecomesTargetableEffect": [],
         "BigPicture": [
             "unit_siege_machine_catapult_big",
             "unit_siege_machine_catapult_big",
             "unit_siege_machine_catapult_big",
+            "unit_siege_machine_catapult_big",
             "unit_siege_machine_catapult_big"
         ],
         "BigPictureSWF": [
             "sc/info_siege_machine_catapult.sc",
             "sc/info_siege_machine_catapult.sc",
             "sc/info_siege_machine_catapult.sc",
+            "sc/info_siege_machine_catapult.sc",
             "sc/info_siege_machine_catapult.sc"
         ],
         "BoostAttackSpeed": [],
         "BoostDmgPerfect": [],
         "BoostRadius": [],
         "BoostedIfAlone": [],
         "BunkerDegenerationTime": [],
@@ -58960,236 +60778,265 @@
         "BunkerTroopCount1": [],
         "BunkerTroopCount2": [],
         "BunkerTroops": [],
         "BurstCount": [
             3,
             3,
             3,
+            3,
             3
         ],
         "BurstDelay": [
             128,
             128,
             128,
+            128,
             128
         ],
         "CanAttackWhileMoving": [],
         "CarryOverToNextStage": [],
         "ChainAttackDamageReductionPercent": [],
         "ChainAttackDelay": [],
         "ChainAttackDistance": [],
         "ChainAttackEffect": [],
         "ChainAttackMaxTargets": [],
         "ChainShootingDistance": [],
         "CoolDownOverride": [
             550,
             550,
             550,
+            550,
             550
         ],
         "CustomDefenderIcon": [],
         "DPS": [
             45,
             50,
             55,
-            60
+            60,
+            65
         ],
         "DPSLv2": [],
         "DPSLv3": [],
         "Damage2": [],
         "Damage2Delay": [],
         "Damage2FalloffEnd": [],
         "Damage2FalloffStart": [],
         "Damage2Min": [],
         "Damage2Radius": [],
         "DamageMultiplierPercent": [
             800,
             800,
             800,
+            800,
             800
         ],
         "DamageMultiplierTarget": [
             "Wall",
             "Wall",
             "Wall",
+            "Wall",
             "Wall"
         ],
         "DamageRadius": [
             100,
             100,
             100,
+            100,
             100
         ],
         "DamageReductionToStorages": [],
         "DefaultSkin": [],
         "DefenseBonus": [],
         "DefensiveTroop": [],
         "DeployEffect": [
             "Siege Ram Deploy",
             "Siege Ram Deploy",
             "Siege Ram Deploy",
+            "Siege Ram Deploy",
             "Siege Ram Deploy"
         ],
         "DeployEffect2": [],
         "Deprecated": [],
         "DieDamage": [],
         "DieDamageDelay": [],
         "DieDamageEffect": [],
         "DieDamageRadius": [],
         "DieEffect": [
             "Siege Ram Die",
             "Siege Ram Die",
             "Siege Ram Die",
+            "Siege Ram Die",
             "Siege Ram Die"
         ],
         "DieEffect2": [],
         "DisableDonate": [],
         "DisableProduction": [
             false,
             false,
             false,
+            false,
             false
         ],
         "DoesNotOpenCC": [],
         "DonateCost": [
             15,
             15,
             15,
+            15,
             15
         ],
         "DonateCount": [
             30,
             30,
             30,
+            30,
             30
         ],
         "DonateXP": [
             30,
             30,
             30,
+            30,
             30
         ],
         "EnabledByCalendar": [],
         "EnabledBySuperLicence": [],
         "EnemyGroupWeight": [
             100,
             100,
             100,
+            100,
             100
         ],
         "EvolveEffect": [],
         "EvolveOnDamageDealt": [],
         "EvolveTime": [],
         "EvolveToCharacter": [],
         "FightWithGroups": [],
         "FriendlyGroupWeight": [
             100,
             100,
             100,
+            100,
             100
         ],
         "FrostOnHitPercent": [],
         "FrostOnHitTime": [],
         "GroundTargets": [
             true,
             true,
             true,
+            true,
             true
         ],
         "HealerWeight": [],
         "HealthReductionPerSecond": [],
         "HeroDamageMultiplier": [],
         "HideEffect": [],
         "HitEffect": [
             "Catapult Hit",
             "Catapult Hit",
             "Catapult Hit",
+            "Catapult Hit",
             "Catapult Hit"
         ],
         "HitEffect2": [
             "Catapult Big Hit",
             "Catapult Big Hit",
             "Catapult Big Hit",
+            "Catapult Big Hit",
             "Catapult Big Hit"
         ],
         "Hitpoints": [
             1700,
             1800,
             1900,
-            2000
+            2000,
+            2100
         ],
         "HousingSpace": [
             1,
             1,
             1,
+            1,
             1
         ],
         "IconExportName": [
             "icon_unit_siege_machine_catapult",
             "icon_unit_siege_machine_catapult",
             "icon_unit_siege_machine_catapult",
+            "icon_unit_siege_machine_catapult",
             "icon_unit_siege_machine_catapult"
         ],
         "IconSWF": [
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
+            "sc/ui.sc",
             "sc/ui.sc"
         ],
         "ImmuneToHealing": [],
         "IncreasingDamage": [],
         "InfoTID": [
             "TID_CHARACTER_INFO_SIEGE_MACHINE_CATAPULT",
             "TID_CHARACTER_INFO_SIEGE_MACHINE_CATAPULT",
             "TID_CHARACTER_INFO_SIEGE_MACHINE_CATAPULT",
+            "TID_CHARACTER_INFO_SIEGE_MACHINE_CATAPULT",
             "TID_CHARACTER_INFO_SIEGE_MACHINE_CATAPULT"
         ],
         "InvisibilityRadius": [],
         "IsFlying": [
             false,
             false,
             false,
+            false,
             false
         ],
         "IsJumper": [
             false,
             false,
             false,
+            false,
             false
         ],
         "IsSecondaryTroop": [],
         "IsUnderground": [],
         "JumpHeightPercent": [],
         "LaboratoryLevel": [
             9,
             10,
             10,
-            11
+            11,
+            14
         ],
         "LoseHpEffect": [],
         "LoseHpInterval": [
             1000,
             1000,
             1000,
+            1000,
             1000
         ],
         "LoseHpPerTick": [
             17,
             17,
             17,
+            17,
             17
         ],
         "Lv2SwitchTime": [],
         "Lv3SwitchTime": [],
         "MoveStartsEffect": [],
         "MovementOffsetAmount": [],
         "MovementOffsetSpeed": [
             0,
             0,
             0,
+            0,
             0
         ],
         "MovingEffect": [],
         "Name": [],
         "NewTargetAttackDelay": [],
         "NoClipping": [],
         "PenetratingExtraRange": [],
@@ -59199,36 +61046,40 @@
         "PreAttackEffect": [],
         "PreferHeroes": [],
         "PreferedTargetBuilding": [],
         "PreferedTargetBuildingClass": [
             "Defense",
             "Defense",
             "Defense",
+            "Defense",
             "Defense"
         ],
         "PreferedTargetDamageMod": [],
         "PreferredMovementTarget": [],
         "PreferredTargetNoTargeting": [],
         "PreviewScenario": [
             "FlameFlinger",
             "FlameFlinger",
             "FlameFlinger",
+            "FlameFlinger",
             "FlameFlinger"
         ],
         "ProductionBuilding": [
             "SiegeWorkshop",
             "SiegeWorkshop",
             "SiegeWorkshop",
+            "SiegeWorkshop",
             "SiegeWorkshop"
         ],
         "Projectile": [
             "FireCatapultProjectile1",
             "FireCatapultProjectile2",
             "FireCatapultProjectile3",
-            "FireCatapultProjectile4"
+            "FireCatapultProjectile4",
+            "FireCatapultProjectile5"
         ],
         "ProjectileBounces": [],
         "ProjectileConsumesBunkerTroops": [],
         "PushbackAfterHit": [],
         "PushbackSpeed": [],
         "RandomizeSecSpawnDist": [],
         "ReflectsDamage": [],
@@ -59243,20 +61094,22 @@
         "SpawnIdle": [],
         "SpawnOnAttack": [],
         "SpawnWhenDamaged": [],
         "SpecialAbilities": [
             "SiegeMachineCatapultSelfDestruct",
             "SiegeMachineCatapultSelfDestruct",
             "SiegeMachineCatapultSelfDestruct",
+            "SiegeMachineCatapultSelfDestruct",
             "SiegeMachineCatapultSelfDestruct"
         ],
         "SpecialAbilitiesLevel": [
             1,
             1,
             1,
+            1,
             1
         ],
         "SpecialAbilityAttribute": [],
         "SpecialAbilityAttribute2": [],
         "SpecialAbilityAttribute3": [],
         "SpecialAbilityEffect": [],
         "SpecialAbilityHideClipName": [],
@@ -59267,94 +61120,105 @@
         "SpecialAbilitySpell": [],
         "SpecialAbilityType": [],
         "SpecialMovementMod": [],
         "Speed": [
             80,
             80,
             80,
+            80,
             80
         ],
         "Squad": [],
         "StrengthWeight": [
-            98,
-            102,
-            106,
-            110
+            7000,
+            7500,
+            8000,
+            9000,
+            11000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
             "TID_CHARACTER_SIEGE_MACHINE_CATAPULT",
             "TID_CHARACTER_SIEGE_MACHINE_CATAPULT",
             "TID_CHARACTER_SIEGE_MACHINE_CATAPULT",
+            "TID_CHARACTER_SIEGE_MACHINE_CATAPULT",
             "TID_CHARACTER_SIEGE_MACHINE_CATAPULT"
         ],
         "TargetGroupsMinWeight": [],
         "TargetGroupsRadius": [],
         "TargetGroupsRange": [],
         "TargetedEffectOffset": [
             "-50",
             "-50",
             "-50",
+            "-50",
             "-50"
         ],
         "TombStone": [],
         "TrainingTime": [
             1200,
             1200,
             1200,
+            1200,
             1200
         ],
         "TransitionEffectLv2": [],
         "TransitionEffectLv3": [],
         "TransitionEffectLv4": [],
         "TriggersTraps": [
             true,
             true,
             true,
+            true,
             true
         ],
         "UndergroundEffect": [],
         "UnderwaterEffect": [],
         "UnitsInCamp": [
             1,
             1,
             1,
+            1,
             1
         ],
         "UpgradeCost": [
             7600000,
             10500000,
             13300000,
-            18000000
+            19000000,
+            19000000
         ],
         "UpgradeLevelByTH": [],
         "UpgradeResource": [
             "Elixir",
             "Elixir",
             "Elixir",
+            "Elixir",
             "Elixir"
         ],
         "UpgradeTimeH": [
             180,
             288,
             300,
+            324,
             324
         ],
         "UpgradeTimeM": [],
         "VillageType": [],
         "VisualLevel": [
             1,
             2,
             3,
-            4
+            4,
+            5
         ],
         "WallMovementCost": []
     },
     "Siege Log Launcher": {
         "AirTargets": [
             false,
             false,
@@ -59800,19 +61664,19 @@
             70,
             70,
             70,
             70
         ],
         "Squad": [],
         "StrengthWeight": [
-            34,
-            36,
-            38,
-            40,
-            40
+            6000,
+            7000,
+            8000,
+            9000,
+            11000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
@@ -60327,19 +62191,19 @@
             0,
             0,
             0,
             0
         ],
         "Squad": [],
         "StrengthWeight": [
-            53,
-            53,
-            53,
-            53,
-            53
+            6000,
+            7000,
+            8000,
+            9000,
+            11000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
@@ -60809,18 +62673,18 @@
             225,
             225,
             225,
             225
         ],
         "Squad": [],
         "StrengthWeight": [
-            45,
-            45,
-            45,
-            45
+            6000,
+            6500,
+            7000,
+            8000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
@@ -61296,19 +63160,19 @@
             150,
             150,
             150,
             150
         ],
         "Squad": [],
         "StrengthWeight": [
-            29,
-            29,
-            29,
-            28,
-            27
+            6000,
+            6500,
+            7000,
+            8000,
+            10000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
@@ -62194,25 +64058,15 @@
             130,
             130,
             130,
             130,
             130
         ],
         "Squad": [],
-        "StrengthWeight": [
-            100,
-            100,
-            100,
-            100,
-            100,
-            190,
-            260,
-            330,
-            330
-        ],
+        "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
@@ -68537,17 +70391,15 @@
         "SpecialAbilitySpell": [],
         "SpecialAbilityType": [],
         "SpecialMovementMod": [],
         "Speed": [
             80
         ],
         "Squad": [],
-        "StrengthWeight": [
-            98
-        ],
+        "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
@@ -68809,17 +70661,15 @@
         "SpecialAbilitySpell": [],
         "SpecialAbilityType": [],
         "SpecialMovementMod": [],
         "Speed": [
             200
         ],
         "Squad": [],
-        "StrengthWeight": [
-            100
-        ],
+        "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
@@ -70019,26 +71869,26 @@
             300,
             300,
             300,
             300
         ],
         "Squad": [],
         "StrengthWeight": [
-            100,
-            100,
-            100,
-            100,
-            90,
-            80,
-            70,
-            70,
-            70,
-            70,
-            70,
-            70
+            900,
+            1000,
+            1200,
+            1400,
+            1500,
+            2500,
+            4000,
+            5000,
+            6000,
+            7000,
+            8000,
+            9000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
@@ -70615,21 +72465,21 @@
             150,
             150,
             150,
             150
         ],
         "Squad": [],
         "StrengthWeight": [
-            800,
-            900,
-            1100,
-            1250,
-            1400,
-            1600,
-            1700
+            2000,
+            3000,
+            4000,
+            5000,
+            6000,
+            9000,
+            10000
         ],
         "SummonCooldown": [
             7000,
             7000,
             7000,
             7000,
             7000,
@@ -71336,25 +73186,25 @@
             300,
             300,
             300,
             300
         ],
         "Squad": [],
         "StrengthWeight": [
-            130,
-            160,
-            190,
-            220,
-            230,
-            280,
-            310,
-            380,
-            380,
-            420,
-            440
+            1800,
+            2000,
+            2100,
+            2200,
+            3000,
+            4000,
+            5000,
+            6000,
+            7000,
+            8000,
+            9000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
@@ -72108,27 +73958,15 @@
             160,
             160,
             160,
             160,
             160
         ],
         "Squad": [],
-        "StrengthWeight": [
-            650,
-            650,
-            650,
-            650,
-            650,
-            650,
-            650,
-            650,
-            650,
-            650,
-            650
-        ],
+        "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
@@ -72743,26 +74581,15 @@
             150,
             150,
             150,
             150,
             150
         ],
         "Squad": [],
-        "StrengthWeight": [
-            120,
-            120,
-            120,
-            120,
-            120,
-            120,
-            120,
-            120,
-            120,
-            120
-        ],
+        "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
@@ -73665,26 +75492,26 @@
             200,
             200,
             200,
             200
         ],
         "Squad": [],
         "StrengthWeight": [
-            130,
-            130,
-            120,
-            120,
-            120,
-            150,
-            150,
-            150,
-            150,
-            150,
-            150,
-            150
+            1400,
+            1600,
+            1800,
+            2000,
+            2200,
+            3000,
+            4000,
+            5000,
+            6000,
+            7000,
+            8000,
+            9000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
@@ -73830,78 +75657,86 @@
     },
     "Yeti": {
         "AirTargets": [
             false,
             false,
             false,
             false,
+            false,
             false
         ],
         "AltPreviewScenario": [],
         "AltProjectile": [],
         "Animation": [
             "yeti_lvl1",
             "yeti_lvl2",
             "yeti_lvl3",
             "yeti_lvl4",
-            "yeti_lvl5"
+            "yeti_lvl5",
+            "yeti_lvl6"
         ],
         "AreaDamageIgnoresWalls": [],
         "AttackCount": [],
         "AttackEffect": [
             "Yeti Attack",
             "Yeti Attack",
             "Yeti Attack",
             "Yeti Attack",
+            "Yeti Attack",
             "Yeti Attack"
         ],
         "AttackEffect2": [],
         "AttackEffectLv2": [],
         "AttackEffectLv3": [],
         "AttackEffectLv4": [],
         "AttackMultipleBuildings": [],
         "AttackRange": [
             80,
             80,
             80,
             80,
+            80,
             80
         ],
         "AttackSpeed": [
             1000,
             1000,
             1000,
             1000,
+            1000,
             1000
         ],
         "AuraSpell": [],
         "AuraSpellLevel": [],
         "AutoMergeDistance": [],
         "AutoMergeGroupSize": [],
         "AvoidNoiseInAttackPositionSelection": [],
         "BarrackLevel": [
             14,
             14,
             14,
             14,
+            14,
             14
         ],
         "BecomesTargetableEffect": [],
         "BigPicture": [
             "unit_yeti_big",
             "unit_yeti_big",
             "unit_yeti_big",
             "unit_yeti_big",
+            "unit_yeti_big",
             "unit_yeti_big"
         ],
         "BigPictureSWF": [
             "sc/info_yeti.sc",
             "sc/info_yeti.sc",
             "sc/info_yeti.sc",
             "sc/info_yeti.sc",
+            "sc/info_yeti.sc",
             "sc/info_yeti.sc"
         ],
         "BoostAttackSpeed": [],
         "BoostDmgPerfect": [],
         "BoostRadius": [],
         "BoostedIfAlone": [],
         "BunkerDegenerationTime": [],
@@ -73922,15 +75757,16 @@
         "CoolDownOverride": [],
         "CustomDefenderIcon": [],
         "DPS": [
             230,
             250,
             270,
             290,
-            310
+            310,
+            330
         ],
         "DPSLv2": [],
         "DPSLv3": [],
         "Damage2": [],
         "Damage2Delay": [],
         "Damage2FalloffEnd": [],
         "Damage2FalloffStart": [],
@@ -73944,158 +75780,174 @@
         "DefenseBonus": [],
         "DefensiveTroop": [],
         "DeployEffect": [
             "Yeti Deploy",
             "Yeti Deploy",
             "Yeti Deploy",
             "Yeti Deploy",
+            "Yeti Deploy",
             "Yeti Deploy"
         ],
         "DeployEffect2": [],
         "Deprecated": [],
         "DieDamage": [],
         "DieDamageDelay": [],
         "DieDamageEffect": [],
         "DieDamageRadius": [],
         "DieEffect": [
             "Yeti Die",
             "Yeti Die",
             "Yeti Die",
             "Yeti Die",
+            "Yeti Die",
             "Yeti Die"
         ],
         "DieEffect2": [],
         "DisableDonate": [],
         "DisableProduction": [],
         "DoesNotOpenCC": [],
         "DonateCost": [
             9,
             9,
             9,
             9,
+            9,
             9
         ],
         "DonateCount": [],
         "DonateXP": [],
         "EnabledByCalendar": [],
         "EnabledBySuperLicence": [],
         "EnemyGroupWeight": [
             1800,
             1800,
             1800,
             1800,
+            1800,
             1800
         ],
         "EvolveEffect": [],
         "EvolveOnDamageDealt": [],
         "EvolveTime": [],
         "EvolveToCharacter": [],
         "FightWithGroups": [],
         "FriendlyGroupWeight": [
             1800,
             1800,
             1800,
             1800,
+            1800,
             1800
         ],
         "FrostOnHitPercent": [],
         "FrostOnHitTime": [],
         "GroundTargets": [
             true,
             true,
             true,
             true,
+            true,
             true
         ],
         "HealerWeight": [],
         "HealthReductionPerSecond": [],
         "HeroDamageMultiplier": [],
         "HideEffect": [],
         "HitEffect": [
             "Yeti Hit",
             "Yeti Hit",
             "Yeti Hit",
             "Yeti Hit",
+            "Yeti Hit",
             "Yeti Hit"
         ],
         "HitEffect2": [],
         "Hitpoints": [
             2900,
             3200,
             3500,
             3700,
-            3900
+            3900,
+            4100
         ],
         "HousingSpace": [
             18,
             18,
             18,
             18,
+            18,
             18
         ],
         "IconExportName": [
             "icon_unit_yeti",
             "icon_unit_yeti",
             "icon_unit_yeti",
             "icon_unit_yeti",
+            "icon_unit_yeti",
             "icon_unit_yeti"
         ],
         "IconSWF": [
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
+            "sc/ui.sc",
             "sc/ui.sc"
         ],
         "ImmuneToHealing": [],
         "IncreasingDamage": [],
         "InfoTID": [
             "TID_CHARACTER_INFO_YETI",
             "TID_CHARACTER_INFO_YETI",
             "TID_CHARACTER_INFO_YETI",
             "TID_CHARACTER_INFO_YETI",
+            "TID_CHARACTER_INFO_YETI",
             "TID_CHARACTER_INFO_YETI"
         ],
         "InvisibilityRadius": [],
         "IsFlying": [
             false,
             false,
             false,
             false,
+            false,
             false
         ],
         "IsJumper": [
             false,
             false,
             false,
             false,
+            false,
             false
         ],
         "IsSecondaryTroop": [],
         "IsUnderground": [],
         "JumpHeightPercent": [],
         "LaboratoryLevel": [
             1,
             10,
             11,
             12,
-            13
+            13,
+            14
         ],
         "LoseHpEffect": [],
         "LoseHpInterval": [],
         "LoseHpPerTick": [],
         "Lv2SwitchTime": [],
         "Lv3SwitchTime": [],
         "MoveStartsEffect": [],
         "MovementOffsetAmount": [],
         "MovementOffsetSpeed": [
             0,
             0,
             0,
             0,
+            0,
             0
         ],
         "MovingEffect": [],
         "Name": [],
         "NewTargetAttackDelay": [],
         "NoClipping": [],
         "PenetratingExtraRange": [],
@@ -74107,30 +75959,33 @@
         "PreferedTargetBuilding": [],
         "PreferedTargetBuildingClass": [],
         "PreferedTargetDamageMod": [
             1,
             1,
             1,
             1,
+            1,
             1
         ],
         "PreferredMovementTarget": [],
         "PreferredTargetNoTargeting": [],
         "PreviewScenario": [
             "TroopGroundAny2",
             "TroopGroundAny2",
             "TroopGroundAny2",
             "TroopGroundAny2",
+            "TroopGroundAny2",
             "TroopGroundAny2"
         ],
         "ProductionBuilding": [
             "Barrack",
             "Barrack",
             "Barrack",
             "Barrack",
+            "Barrack",
             "Barrack"
         ],
         "Projectile": [],
         "ProjectileBounces": [],
         "ProjectileConsumesBunkerTroops": [],
         "PushbackAfterHit": [],
         "PushbackSpeed": [],
@@ -74139,242 +75994,268 @@
         "RetargetAfterHit": [],
         "ScaleByTH": [],
         "SecondarySpawnDist": [
             100,
             100,
             100,
             100,
+            100,
             100
         ],
         "SecondarySpawnOffset": [],
         "SecondaryTroop": [
             "Yetimite",
             "Yetimite",
             "Yetimite",
             "Yetimite",
+            "Yetimite",
             "Yetimite"
         ],
         "SecondaryTroopCnt": [
             8,
             9,
             10,
             11,
-            12
+            12,
+            13
         ],
         "SelfAsAoeCenter": [],
         "SmoothJump": [],
         "SpawnIdle": [],
         "SpawnOnAttack": [],
         "SpawnWhenDamaged": [],
         "SpecialAbilities": [],
         "SpecialAbilitiesLevel": [],
         "SpecialAbilityAttribute": [
             600,
             600,
             600,
             600,
+            600,
             600
         ],
         "SpecialAbilityAttribute2": [
             1,
             1,
             1,
             1,
+            1,
             1
         ],
         "SpecialAbilityAttribute3": [],
         "SpecialAbilityEffect": [],
         "SpecialAbilityHideClipName": [
             "full",
             "full",
             "full",
             "full",
+            "full",
             "full"
         ],
         "SpecialAbilityIcon": [],
         "SpecialAbilityInfo": [],
         "SpecialAbilityLevel": [],
         "SpecialAbilityName": [],
         "SpecialAbilitySpell": [],
         "SpecialAbilityType": [
             "SpawnUnitsWhenDamaged",
             "SpawnUnitsWhenDamaged",
             "SpawnUnitsWhenDamaged",
             "SpawnUnitsWhenDamaged",
+            "SpawnUnitsWhenDamaged",
             "SpawnUnitsWhenDamaged"
         ],
         "SpecialMovementMod": [],
         "Speed": [
             150,
             150,
             150,
             150,
+            150,
             150
         ],
         "Squad": [],
         "StrengthWeight": [
-            550,
-            600,
-            650,
-            700,
-            750
+            5000,
+            6000,
+            7000,
+            8000,
+            9000,
+            10000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTime": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
             "TID_CHARACTER_YETI",
             "TID_CHARACTER_YETI",
             "TID_CHARACTER_YETI",
             "TID_CHARACTER_YETI",
+            "TID_CHARACTER_YETI",
             "TID_CHARACTER_YETI"
         ],
         "TargetGroupsMinWeight": [],
         "TargetGroupsRadius": [],
         "TargetGroupsRange": [],
         "TargetedEffectOffset": [
             "-50",
             "-50",
             "-50",
             "-50",
+            "-50",
             "-50"
         ],
         "TombStone": [
             "TombStone",
             "TombStone",
             "TombStone",
             "TombStone",
+            "TombStone",
             "TombStone"
         ],
         "TrainingTime": [
             180,
             180,
             180,
             180,
+            180,
             180
         ],
         "TransitionEffectLv2": [],
         "TransitionEffectLv3": [],
         "TransitionEffectLv4": [],
         "TriggersTraps": [
             true,
             true,
             true,
             true,
+            true,
             true
         ],
         "UndergroundEffect": [],
         "UnderwaterEffect": [],
         "UnitsInCamp": [],
         "UpgradeCost": [
             7000000,
             9000000,
             17100000,
             19000000,
-            19500000
+            21000000,
+            21000000
         ],
         "UpgradeLevelByTH": [],
         "UpgradeResource": [
             "Elixir",
             "Elixir",
             "Elixir",
             "Elixir",
+            "Elixir",
             "Elixir"
         ],
         "UpgradeTimeH": [
             144,
             168,
             288,
             330,
-            354
+            360,
+            360
         ],
         "UpgradeTimeM": [],
         "VillageType": [],
         "VisualLevel": [
             1,
             2,
             3,
             4,
-            5
+            5,
+            6
         ],
         "WallMovementCost": []
     },
     "Yetimite": {
         "AirTargets": [
             true,
             true,
             true,
             true,
+            true,
             true
         ],
         "AltPreviewScenario": [],
         "AltProjectile": [],
         "Animation": [
             "yetimite_lvl1",
             "yetimite_lvl2",
             "yetimite_lvl3",
             "yetimite_lvl4",
-            "yetimite_lvl4"
+            "yetimite_lvl4",
+            "yetimite_lvl6"
         ],
         "AreaDamageIgnoresWalls": [],
         "AttackCount": [
             1,
             1,
             1,
             1,
+            1,
             1
         ],
         "AttackEffect": [],
         "AttackEffect2": [],
         "AttackEffectLv2": [],
         "AttackEffectLv3": [],
         "AttackEffectLv4": [],
         "AttackMultipleBuildings": [],
         "AttackRange": [
             200,
             200,
             200,
             200,
+            200,
             200
         ],
         "AttackSpeed": [
             1000,
             1000,
             1000,
             1000,
+            1000,
             1000
         ],
         "AuraSpell": [],
         "AuraSpellLevel": [],
         "AutoMergeDistance": [],
         "AutoMergeGroupSize": [],
         "AvoidNoiseInAttackPositionSelection": [],
         "BarrackLevel": [
             1,
             1,
             1,
             1,
+            1,
             1
         ],
         "BecomesTargetableEffect": [],
         "BigPicture": [
             "unit_yetimite_big",
             "unit_yetimite_big",
             "unit_yetimite_big",
             "unit_yetimite_big",
+            "unit_yetimite_big",
             "unit_yetimite_big"
         ],
         "BigPictureSWF": [
             "sc/info_yeti.sc",
             "sc/info_yeti.sc",
             "sc/info_yeti.sc",
             "sc/info_yeti.sc",
+            "sc/info_yeti.sc",
             "sc/info_yeti.sc"
         ],
         "BoostAttackSpeed": [],
         "BoostDmgPerfect": [],
         "BoostRadius": [],
         "BoostedIfAlone": [],
         "BunkerDegenerationTime": [],
@@ -74395,15 +76276,16 @@
         "CoolDownOverride": [],
         "CustomDefenderIcon": [],
         "DPS": [
             56,
             64,
             72,
             78,
-            84
+            84,
+            88
         ],
         "DPSLv2": [],
         "DPSLv3": [],
         "Damage2": [],
         "Damage2Delay": [],
         "Damage2FalloffEnd": [],
         "Damage2FalloffStart": [],
@@ -74412,21 +76294,23 @@
         "DamageMultiplierPercent": [],
         "DamageMultiplierTarget": [],
         "DamageRadius": [
             80,
             80,
             80,
             80,
+            80,
             80
         ],
         "DamageReductionToStorages": [
             50,
             50,
             50,
             50,
+            50,
             50
         ],
         "DefaultSkin": [],
         "DefenseBonus": [],
         "DefensiveTroop": [],
         "DeployEffect": [],
         "DeployEffect2": [],
@@ -74436,166 +76320,184 @@
         "DieDamageEffect": [],
         "DieDamageRadius": [],
         "DieEffect": [
             "Yetimite Die",
             "Yetimite Die",
             "Yetimite Die",
             "Yetimite Die",
+            "Yetimite Die",
             "Yetimite Die"
         ],
         "DieEffect2": [],
         "DisableDonate": [],
         "DisableProduction": [
             true,
             true,
             true,
             true,
+            true,
             true
         ],
         "DoesNotOpenCC": [
             true,
             true,
             true,
             true,
+            true,
             true
         ],
         "DonateCost": [],
         "DonateCount": [],
         "DonateXP": [],
         "EnabledByCalendar": [],
         "EnabledBySuperLicence": [],
         "EnemyGroupWeight": [
             100,
             100,
             100,
             100,
+            100,
             100
         ],
         "EvolveEffect": [],
         "EvolveOnDamageDealt": [],
         "EvolveTime": [],
         "EvolveToCharacter": [],
         "FightWithGroups": [],
         "FriendlyGroupWeight": [
             100,
             100,
             100,
             100,
+            100,
             100
         ],
         "FrostOnHitPercent": [],
         "FrostOnHitTime": [],
         "GroundTargets": [
             true,
             true,
             true,
             true,
+            true,
             true
         ],
         "HealerWeight": [],
         "HealthReductionPerSecond": [],
         "HeroDamageMultiplier": [],
         "HideEffect": [],
         "HitEffect": [
             "Yeti Hit",
             "Yeti Hit",
             "Yeti Hit",
             "Yeti Hit",
+            "Yeti Hit",
             "Yeti Hit"
         ],
         "HitEffect2": [],
         "Hitpoints": [
             300,
             350,
             400,
             450,
-            500
+            500,
+            550
         ],
         "HousingSpace": [
             3,
             3,
             3,
             3,
+            3,
             3
         ],
         "IconExportName": [
             "icon_unit_yeti",
             "icon_unit_yeti",
             "icon_unit_yeti",
             "icon_unit_yeti",
+            "icon_unit_yeti",
             "icon_unit_yeti"
         ],
         "IconSWF": [
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
+            "sc/ui.sc",
             "sc/ui.sc"
         ],
         "ImmuneToHealing": [],
         "IncreasingDamage": [],
         "InfoTID": [
             "TID_CHARACTER_INFO_YETIMITE",
             "TID_CHARACTER_INFO_YETIMITE",
             "TID_CHARACTER_INFO_YETIMITE",
             "TID_CHARACTER_INFO_YETIMITE",
+            "TID_CHARACTER_INFO_YETIMITE",
             "TID_CHARACTER_INFO_YETIMITE"
         ],
         "InvisibilityRadius": [],
         "IsFlying": [
             false,
             false,
             false,
             false,
+            false,
             false
         ],
         "IsJumper": [
             true,
             true,
             true,
             true,
+            true,
             true
         ],
         "IsSecondaryTroop": [
             true,
             true,
             true,
             true,
+            true,
             true
         ],
         "IsUnderground": [],
         "JumpHeightPercent": [],
         "LaboratoryLevel": [
             1,
             1,
             1,
             1,
+            1,
             1
         ],
         "LoseHpEffect": [],
         "LoseHpInterval": [],
         "LoseHpPerTick": [],
         "Lv2SwitchTime": [],
         "Lv3SwitchTime": [],
         "MoveStartsEffect": [],
         "MovementOffsetAmount": [],
         "MovementOffsetSpeed": [
             0,
             0,
             0,
             0,
+            0,
             0
         ],
         "MovingEffect": [],
         "Name": [],
         "NewTargetAttackDelay": [
             500,
             500,
             500,
             500,
+            500,
             500
         ],
         "NoClipping": [],
         "PenetratingExtraRange": [],
         "PenetratingProjectile": [],
         "PenetratingRadius": [],
         "PickNewTargetAfterPushback": [],
@@ -74603,39 +76505,43 @@
         "PreferHeroes": [],
         "PreferedTargetBuilding": [],
         "PreferedTargetBuildingClass": [
             "Defense",
             "Defense",
             "Defense",
             "Defense",
+            "Defense",
             "Defense"
         ],
         "PreferedTargetDamageMod": [
             4,
             4,
             4,
             4,
+            4,
             4
         ],
         "PreferredMovementTarget": [],
         "PreferredTargetNoTargeting": [],
         "PreviewScenario": [
             "SecondaryTroopDefense",
             "SecondaryTroopDefense",
             "SecondaryTroopDefense",
             "SecondaryTroopDefense",
+            "SecondaryTroopDefense",
             "SecondaryTroopDefense"
         ],
         "ProductionBuilding": [],
         "Projectile": [
             "YetimiteJump",
             "YetimiteJump2",
             "YetimiteJump3",
             "YetimiteJump4",
-            "YetimiteJump4"
+            "YetimiteJump4",
+            "YetimiteJump6"
         ],
         "ProjectileBounces": [],
         "ProjectileConsumesBunkerTroops": [],
         "PushbackAfterHit": [],
         "PushbackSpeed": [],
         "RandomizeSecSpawnDist": [],
         "ReflectsDamage": [],
@@ -74665,14 +76571,15 @@
         "SpecialAbilityType": [],
         "SpecialMovementMod": [],
         "Speed": [
             300,
             300,
             300,
             300,
+            300,
             300
         ],
         "Squad": [],
         "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
@@ -74680,36 +76587,39 @@
         "SummonTroop": [],
         "SummonTroopCount": [],
         "TID": [
             "TID_CHARACTER_YETIMITE",
             "TID_CHARACTER_YETIMITE",
             "TID_CHARACTER_YETIMITE",
             "TID_CHARACTER_YETIMITE",
+            "TID_CHARACTER_YETIMITE",
             "TID_CHARACTER_YETIMITE"
         ],
         "TargetGroupsMinWeight": [],
         "TargetGroupsRadius": [],
         "TargetGroupsRange": [],
         "TargetedEffectOffset": [
             "-50",
             "-50",
             "-50",
             "-50",
+            "-50",
             "-50"
         ],
         "TombStone": [],
         "TrainingTime": [],
         "TransitionEffectLv2": [],
         "TransitionEffectLv3": [],
         "TransitionEffectLv4": [],
         "TriggersTraps": [
             false,
             false,
             false,
             false,
+            false,
             false
         ],
         "UndergroundEffect": [],
         "UnderwaterEffect": [],
         "UnitsInCamp": [],
         "UpgradeCost": [],
         "UpgradeLevelByTH": [],
@@ -74718,15 +76628,16 @@
         "UpgradeTimeM": [],
         "VillageType": [],
         "VisualLevel": [
             1,
             2,
             3,
             4,
-            5
+            5,
+            6
         ],
         "WallMovementCost": []
     },
     "Zappies": {
         "AirTargets": [
             true,
             true,
```

### Comparing `coc.py-3.4.1/coc/static/equipment.json` & `coc_py-3.4.2/coc/static/equipment.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.826250307957625%*

 * *Differences: {"'Angry Tome'": "{'StrengthWeight': [100, 200, 300, 400, 500, 600, 700, 800, 900, 1000, 1100, "*

 * *                 '1200, 1300, 1400, 1900, 2000, 2100, 2600]}',*

 * * "'Archer Crown'": "{'StrengthWeight': [100, 200, 300, 400, 500, 600, 700, 800, 900, 1000, 1100, "*

 * *                   '1200, 1300, 1400, 1900, 2000, 2100, 2600]}',*

 * * "'Barbarian Crown'": "{'StrengthWeight': [100, 200, 300, 400, 500, 600, 700, 800, 900, 1000, "*

 * *                      '1100, 1200, 1300, 1400, 1900, 2000, 2100, 2600]}',*

 * * "'Earthquake Boot […]*

```diff
@@ -266,14 +266,34 @@
             1,
             1,
             1,
             1,
             1
         ],
         "Speed": [],
+        "StrengthWeight": [
+            100,
+            200,
+            300,
+            400,
+            500,
+            600,
+            700,
+            800,
+            900,
+            1000,
+            1100,
+            1200,
+            1300,
+            1400,
+            1900,
+            2000,
+            2100,
+            2600
+        ],
         "TID": [
             "TID_GEAR_ANGRY_TOME",
             "TID_GEAR_ANGRY_TOME",
             "TID_GEAR_ANGRY_TOME",
             "TID_GEAR_ANGRY_TOME",
             "TID_GEAR_ANGRY_TOME",
             "TID_GEAR_ANGRY_TOME",
@@ -598,14 +618,34 @@
             1,
             1,
             1,
             1,
             1
         ],
         "Speed": [],
+        "StrengthWeight": [
+            100,
+            200,
+            300,
+            400,
+            500,
+            600,
+            700,
+            800,
+            900,
+            1000,
+            1100,
+            1200,
+            1300,
+            1400,
+            1900,
+            2000,
+            2100,
+            2600
+        ],
         "TID": [
             "TID_GEAR_TITLE_ARCHER_CROWN",
             "TID_GEAR_TITLE_ARCHER_CROWN",
             "TID_GEAR_TITLE_ARCHER_CROWN",
             "TID_GEAR_TITLE_ARCHER_CROWN",
             "TID_GEAR_TITLE_ARCHER_CROWN",
             "TID_GEAR_TITLE_ARCHER_CROWN",
@@ -930,14 +970,34 @@
             1,
             1,
             1,
             1,
             1
         ],
         "Speed": [],
+        "StrengthWeight": [
+            100,
+            200,
+            300,
+            400,
+            500,
+            600,
+            700,
+            800,
+            900,
+            1000,
+            1100,
+            1200,
+            1300,
+            1400,
+            1900,
+            2000,
+            2100,
+            2600
+        ],
         "TID": [
             "TID_GEAR_TITLE_BARBARIAN_CROWN",
             "TID_GEAR_TITLE_BARBARIAN_CROWN",
             "TID_GEAR_TITLE_BARBARIAN_CROWN",
             "TID_GEAR_TITLE_BARBARIAN_CROWN",
             "TID_GEAR_TITLE_BARBARIAN_CROWN",
             "TID_GEAR_TITLE_BARBARIAN_CROWN",
@@ -1262,14 +1322,34 @@
             1,
             1,
             1,
             1,
             1
         ],
         "Speed": [],
+        "StrengthWeight": [
+            100,
+            200,
+            300,
+            400,
+            500,
+            600,
+            700,
+            800,
+            900,
+            1000,
+            1100,
+            1200,
+            1300,
+            1400,
+            1900,
+            2000,
+            2100,
+            2600
+        ],
         "TID": [
             "TID_GEAR_EARTHQUAKE_BOOTS",
             "TID_GEAR_EARTHQUAKE_BOOTS",
             "TID_GEAR_EARTHQUAKE_BOOTS",
             "TID_GEAR_EARTHQUAKE_BOOTS",
             "TID_GEAR_EARTHQUAKE_BOOTS",
             "TID_GEAR_EARTHQUAKE_BOOTS",
@@ -1556,14 +1636,34 @@
             1,
             1,
             1,
             1,
             1
         ],
         "Speed": [],
+        "StrengthWeight": [
+            100,
+            200,
+            300,
+            400,
+            500,
+            600,
+            700,
+            800,
+            900,
+            1000,
+            1100,
+            1200,
+            1300,
+            1400,
+            1900,
+            2000,
+            2100,
+            2600
+        ],
         "TID": [
             "TID_GEAR_TITLE_ETERNAL_TOME",
             "TID_GEAR_TITLE_ETERNAL_TOME",
             "TID_GEAR_TITLE_ETERNAL_TOME",
             "TID_GEAR_TITLE_ETERNAL_TOME",
             "TID_GEAR_TITLE_ETERNAL_TOME",
             "TID_GEAR_TITLE_ETERNAL_TOME",
@@ -2005,14 +2105,43 @@
             1,
             1,
             1,
             1,
             1
         ],
         "Speed": [],
+        "StrengthWeight": [
+            100,
+            200,
+            300,
+            400,
+            500,
+            600,
+            700,
+            800,
+            900,
+            1000,
+            1100,
+            1200,
+            1300,
+            1400,
+            1900,
+            2000,
+            2100,
+            2600,
+            2700,
+            2800,
+            3300,
+            3400,
+            3500,
+            4000,
+            4100,
+            4200,
+            4700
+        ],
         "TID": [
             "TID_GEAR_FIRE_IN_A_CAN",
             "TID_GEAR_FIRE_IN_A_CAN",
             "TID_GEAR_FIRE_IN_A_CAN",
             "TID_GEAR_FIRE_IN_A_CAN",
             "TID_GEAR_FIRE_IN_A_CAN",
             "TID_GEAR_FIRE_IN_A_CAN",
@@ -2093,14 +2222,547 @@
             "CommonOre; RareOre; EpicOre",
             "CommonOre",
             "CommonOre",
             "CommonOre; RareOre; EpicOre",
             "CommonOre; RareOre; EpicOre"
         ]
     },
+    "Football": {
+        "AllowedCharacters": [
+            "Barbarian King;",
+            "Barbarian King;",
+            "Barbarian King;",
+            "Barbarian King;",
+            "Barbarian King;",
+            "Barbarian King;",
+            "Barbarian King;",
+            "Barbarian King;",
+            "Barbarian King;",
+            "Barbarian King;",
+            "Barbarian King;",
+            "Barbarian King;",
+            "Barbarian King;",
+            "Barbarian King;",
+            "Barbarian King;",
+            "Barbarian King;",
+            "Barbarian King;",
+            "Barbarian King;",
+            "Barbarian King;",
+            "Barbarian King;",
+            "Barbarian King;",
+            "Barbarian King;",
+            "Barbarian King;",
+            "Barbarian King;",
+            "Barbarian King;",
+            "Barbarian King;",
+            "Barbarian King;"
+        ],
+        "AttackRange": [],
+        "AttackSpeedPercentage": [],
+        "Claimable": [
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true
+        ],
+        "DPS": [
+            35,
+            38,
+            42,
+            45,
+            49,
+            52,
+            55,
+            58,
+            65,
+            76,
+            88,
+            101,
+            112,
+            124,
+            135,
+            148,
+            159,
+            171,
+            176,
+            182,
+            188,
+            194,
+            199,
+            205,
+            211,
+            217,
+            222
+        ],
+        "Deprecated": [],
+        "DiamondValue": [],
+        "ExtraAbilities": [],
+        "ExtraAbilityLevels": [],
+        "HealOnActivation": [],
+        "HitPoints": [
+            365,
+            478,
+            590,
+            703,
+            815,
+            928,
+            1040,
+            1153,
+            1265,
+            1378,
+            1490,
+            1603,
+            1715,
+            1828,
+            1940,
+            2053,
+            2165,
+            2278,
+            2390,
+            2503,
+            2615,
+            2728,
+            2840,
+            2953,
+            3065,
+            3178,
+            3290
+        ],
+        "IconExportName": [
+            "icon_gear_BK_Football",
+            "icon_gear_BK_Football",
+            "icon_gear_BK_Football",
+            "icon_gear_BK_Football",
+            "icon_gear_BK_Football",
+            "icon_gear_BK_Football",
+            "icon_gear_BK_Football",
+            "icon_gear_BK_Football",
+            "icon_gear_BK_Football",
+            "icon_gear_BK_Football",
+            "icon_gear_BK_Football",
+            "icon_gear_BK_Football",
+            "icon_gear_BK_Football",
+            "icon_gear_BK_Football",
+            "icon_gear_BK_Football",
+            "icon_gear_BK_Football",
+            "icon_gear_BK_Football",
+            "icon_gear_BK_Football",
+            "icon_gear_BK_Football",
+            "icon_gear_BK_Football",
+            "icon_gear_BK_Football",
+            "icon_gear_BK_Football",
+            "icon_gear_BK_Football",
+            "icon_gear_BK_Football",
+            "icon_gear_BK_Football",
+            "icon_gear_BK_Football",
+            "icon_gear_BK_Football"
+        ],
+        "IconSWF": [
+            "sc/ui.sc",
+            "sc/ui.sc",
+            "sc/ui.sc",
+            "sc/ui.sc",
+            "sc/ui.sc",
+            "sc/ui.sc",
+            "sc/ui.sc",
+            "sc/ui.sc",
+            "sc/ui.sc",
+            "sc/ui.sc",
+            "sc/ui.sc",
+            "sc/ui.sc",
+            "sc/ui.sc",
+            "sc/ui.sc",
+            "sc/ui.sc",
+            "sc/ui.sc",
+            "sc/ui.sc",
+            "sc/ui.sc",
+            "sc/ui.sc",
+            "sc/ui.sc",
+            "sc/ui.sc",
+            "sc/ui.sc",
+            "sc/ui.sc",
+            "sc/ui.sc",
+            "sc/ui.sc",
+            "sc/ui.sc",
+            "sc/ui.sc"
+        ],
+        "InfoTID": [
+            "TID_GEAR_INFO_FOOTBALL",
+            "TID_GEAR_INFO_FOOTBALL",
+            "TID_GEAR_INFO_FOOTBALL",
+            "TID_GEAR_INFO_FOOTBALL",
+            "TID_GEAR_INFO_FOOTBALL",
+            "TID_GEAR_INFO_FOOTBALL",
+            "TID_GEAR_INFO_FOOTBALL",
+            "TID_GEAR_INFO_FOOTBALL",
+            "TID_GEAR_INFO_FOOTBALL",
+            "TID_GEAR_INFO_FOOTBALL",
+            "TID_GEAR_INFO_FOOTBALL",
+            "TID_GEAR_INFO_FOOTBALL",
+            "TID_GEAR_INFO_FOOTBALL",
+            "TID_GEAR_INFO_FOOTBALL",
+            "TID_GEAR_INFO_FOOTBALL",
+            "TID_GEAR_INFO_FOOTBALL",
+            "TID_GEAR_INFO_FOOTBALL",
+            "TID_GEAR_INFO_FOOTBALL",
+            "TID_GEAR_INFO_FOOTBALL",
+            "TID_GEAR_INFO_FOOTBALL",
+            "TID_GEAR_INFO_FOOTBALL",
+            "TID_GEAR_INFO_FOOTBALL",
+            "TID_GEAR_INFO_FOOTBALL",
+            "TID_GEAR_INFO_FOOTBALL",
+            "TID_GEAR_INFO_FOOTBALL",
+            "TID_GEAR_INFO_FOOTBALL",
+            "TID_GEAR_INFO_FOOTBALL"
+        ],
+        "Level": [
+            1,
+            2,
+            3,
+            4,
+            5,
+            6,
+            7,
+            8,
+            9,
+            10,
+            11,
+            12,
+            13,
+            14,
+            15,
+            16,
+            17,
+            18,
+            19,
+            20,
+            21,
+            22,
+            23,
+            24,
+            25,
+            26,
+            27
+        ],
+        "MainAbilities": [
+            "FootballBounce",
+            "FootballBounce",
+            "FootballBounce",
+            "FootballBounce",
+            "FootballBounce",
+            "FootballBounce",
+            "FootballBounce",
+            "FootballBounce",
+            "FootballBounce",
+            "FootballBounce",
+            "FootballBounce",
+            "FootballBounce",
+            "FootballBounce",
+            "FootballBounce",
+            "FootballBounce",
+            "FootballBounce",
+            "FootballBounce",
+            "FootballBounce",
+            "FootballBounce",
+            "FootballBounce",
+            "FootballBounce",
+            "FootballBounce",
+            "FootballBounce",
+            "FootballBounce",
+            "FootballBounce",
+            "FootballBounce",
+            "FootballBounce"
+        ],
+        "MainAbilityLevels": [
+            1,
+            1,
+            2,
+            2,
+            2,
+            3,
+            3,
+            3,
+            4,
+            4,
+            4,
+            5,
+            5,
+            5,
+            6,
+            6,
+            6,
+            7,
+            7,
+            7,
+            8,
+            8,
+            8,
+            9,
+            9,
+            9,
+            10
+        ],
+        "Name": [],
+        "PreviewScenario": [
+            "GearFootball",
+            "GearFootball",
+            "GearFootball",
+            "GearFootball",
+            "GearFootball",
+            "GearFootball",
+            "GearFootball",
+            "GearFootball",
+            "GearFootball",
+            "GearFootball",
+            "GearFootball",
+            "GearFootball",
+            "GearFootball",
+            "GearFootball",
+            "GearFootball",
+            "GearFootball",
+            "GearFootball",
+            "GearFootball",
+            "GearFootball",
+            "GearFootball",
+            "GearFootball",
+            "GearFootball",
+            "GearFootball",
+            "GearFootball",
+            "GearFootball",
+            "GearFootball",
+            "GearFootball"
+        ],
+        "Rarity": [
+            "Epic",
+            "Epic",
+            "Epic",
+            "Epic",
+            "Epic",
+            "Epic",
+            "Epic",
+            "Epic",
+            "Epic",
+            "Epic",
+            "Epic",
+            "Epic",
+            "Epic",
+            "Epic",
+            "Epic",
+            "Epic",
+            "Epic",
+            "Epic",
+            "Epic",
+            "Epic",
+            "Epic",
+            "Epic",
+            "Epic",
+            "Epic",
+            "Epic",
+            "Epic",
+            "Epic"
+        ],
+        "RequiredBlacksmithLevel": [
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            3,
+            3,
+            3,
+            5,
+            5,
+            5,
+            7,
+            7,
+            7,
+            8,
+            8,
+            8,
+            9,
+            9,
+            9
+        ],
+        "RequiredCharacterLevel": [
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1,
+            1
+        ],
+        "Speed": [],
+        "StrengthWeight": [
+            100,
+            200,
+            300,
+            400,
+            500,
+            600,
+            700,
+            800,
+            900,
+            1000,
+            1100,
+            1200,
+            1300,
+            1400,
+            1900,
+            2000,
+            2100,
+            2600,
+            2700,
+            2800,
+            3300,
+            3400,
+            3500,
+            4000,
+            4100,
+            4200,
+            4700
+        ],
+        "TID": [
+            "TID_GEAR_TITLE_FOOTBALL",
+            "TID_GEAR_TITLE_FOOTBALL",
+            "TID_GEAR_TITLE_FOOTBALL",
+            "TID_GEAR_TITLE_FOOTBALL",
+            "TID_GEAR_TITLE_FOOTBALL",
+            "TID_GEAR_TITLE_FOOTBALL",
+            "TID_GEAR_TITLE_FOOTBALL",
+            "TID_GEAR_TITLE_FOOTBALL",
+            "TID_GEAR_TITLE_FOOTBALL",
+            "TID_GEAR_TITLE_FOOTBALL",
+            "TID_GEAR_TITLE_FOOTBALL",
+            "TID_GEAR_TITLE_FOOTBALL",
+            "TID_GEAR_TITLE_FOOTBALL",
+            "TID_GEAR_TITLE_FOOTBALL",
+            "TID_GEAR_TITLE_FOOTBALL",
+            "TID_GEAR_TITLE_FOOTBALL",
+            "TID_GEAR_TITLE_FOOTBALL",
+            "TID_GEAR_TITLE_FOOTBALL",
+            "TID_GEAR_TITLE_FOOTBALL",
+            "TID_GEAR_TITLE_FOOTBALL",
+            "TID_GEAR_TITLE_FOOTBALL",
+            "TID_GEAR_TITLE_FOOTBALL",
+            "TID_GEAR_TITLE_FOOTBALL",
+            "TID_GEAR_TITLE_FOOTBALL",
+            "TID_GEAR_TITLE_FOOTBALL",
+            "TID_GEAR_TITLE_FOOTBALL",
+            "TID_GEAR_TITLE_FOOTBALL"
+        ],
+        "UpgradeCosts": [
+            120,
+            "240;20",
+            400,
+            600,
+            "840;100",
+            1120,
+            1440,
+            "1800;200;10",
+            1900,
+            2000,
+            "2100;400;20",
+            2200,
+            2300,
+            "2400;600;30",
+            2500,
+            2600,
+            "2700;600;50",
+            2800,
+            2900,
+            "3000;600;100",
+            3100,
+            3200,
+            "3300;600;120",
+            3400,
+            3500,
+            "3600;600;150",
+            "3600;600;150"
+        ],
+        "UpgradeResources": [
+            "CommonOre",
+            "CommonOre; RareOre",
+            "CommonOre",
+            "CommonOre",
+            "CommonOre; RareOre",
+            "CommonOre",
+            "CommonOre",
+            "CommonOre; RareOre; EpicOre",
+            "CommonOre",
+            "CommonOre",
+            "CommonOre; RareOre; EpicOre",
+            "CommonOre",
+            "CommonOre",
+            "CommonOre; RareOre; EpicOre",
+            "CommonOre",
+            "CommonOre",
+            "CommonOre; RareOre; EpicOre",
+            "CommonOre",
+            "CommonOre",
+            "CommonOre; RareOre; EpicOre",
+            "CommonOre",
+            "CommonOre",
+            "CommonOre; RareOre; EpicOre",
+            "CommonOre",
+            "CommonOre",
+            "CommonOre; RareOre; EpicOre",
+            "CommonOre; RareOre; EpicOre"
+        ]
+    },
     "Frozen Arrow": {
         "AllowedCharacters": [
             "Archer Queen;",
             "Archer Queen;",
             "Archer Queen;",
             "Archer Queen;",
             "Archer Queen;",
@@ -2481,14 +3143,43 @@
             1,
             1,
             1,
             1,
             1
         ],
         "Speed": [],
+        "StrengthWeight": [
+            100,
+            200,
+            300,
+            400,
+            500,
+            600,
+            700,
+            800,
+            900,
+            1000,
+            1100,
+            1200,
+            1300,
+            1400,
+            1900,
+            2000,
+            2100,
+            2600,
+            2700,
+            2800,
+            3300,
+            3400,
+            3500,
+            4000,
+            4100,
+            4200,
+            4700
+        ],
         "TID": [
             "TID_GEAR_FROZEN_ARROW",
             "TID_GEAR_FROZEN_ARROW",
             "TID_GEAR_FROZEN_ARROW",
             "TID_GEAR_FROZEN_ARROW",
             "TID_GEAR_FROZEN_ARROW",
             "TID_GEAR_FROZEN_ARROW",
@@ -3013,14 +3704,43 @@
             1,
             1,
             1,
             1,
             1
         ],
         "Speed": [],
+        "StrengthWeight": [
+            100,
+            200,
+            300,
+            400,
+            500,
+            600,
+            700,
+            800,
+            900,
+            1000,
+            1100,
+            1200,
+            1300,
+            1400,
+            1900,
+            2000,
+            2100,
+            2600,
+            2700,
+            2800,
+            3300,
+            3400,
+            3500,
+            4000,
+            4100,
+            4200,
+            4700
+        ],
         "TID": [
             "TID_GEAR_GIANT_GAUNTLET",
             "TID_GEAR_GIANT_GAUNTLET",
             "TID_GEAR_GIANT_GAUNTLET",
             "TID_GEAR_GIANT_GAUNTLET",
             "TID_GEAR_GIANT_GAUNTLET",
             "TID_GEAR_GIANT_GAUNTLET",
@@ -3132,24 +3852,24 @@
             6,
             6,
             7,
             8,
             8,
             9,
             10,
+            10,
             11,
             12,
-            13,
+            12,
             13,
             14,
-            15,
+            14,
             15,
             16,
-            17,
-            18
+            16
         ],
         "Claimable": [],
         "DPS": [
             20,
             24,
             28,
             32,
@@ -3372,14 +4092,34 @@
             1,
             1,
             1,
             1,
             1
         ],
         "Speed": [],
+        "StrengthWeight": [
+            100,
+            200,
+            300,
+            400,
+            500,
+            600,
+            700,
+            800,
+            900,
+            1000,
+            1100,
+            1200,
+            1300,
+            1400,
+            1900,
+            2000,
+            2100,
+            2600
+        ],
         "TID": [
             "TID_GEAR_TITLE_HASTE_VIAL",
             "TID_GEAR_TITLE_HASTE_VIAL",
             "TID_GEAR_TITLE_HASTE_VIAL",
             "TID_GEAR_TITLE_HASTE_VIAL",
             "TID_GEAR_TITLE_HASTE_VIAL",
             "TID_GEAR_TITLE_HASTE_VIAL",
@@ -3723,14 +4463,34 @@
             1,
             1,
             1,
             1,
             1
         ],
         "Speed": [],
+        "StrengthWeight": [
+            100,
+            200,
+            300,
+            400,
+            500,
+            600,
+            700,
+            800,
+            900,
+            1000,
+            1100,
+            1200,
+            1300,
+            1400,
+            1900,
+            2000,
+            2100,
+            2600
+        ],
         "TID": [
             "TID_GEAR_HEALER_JAR",
             "TID_GEAR_HEALER_JAR",
             "TID_GEAR_HEALER_JAR",
             "TID_GEAR_HEALER_JAR",
             "TID_GEAR_HEALER_JAR",
             "TID_GEAR_HEALER_JAR",
@@ -4055,14 +4815,34 @@
             1,
             1,
             1,
             1,
             1
         ],
         "Speed": [],
+        "StrengthWeight": [
+            100,
+            200,
+            300,
+            400,
+            500,
+            600,
+            700,
+            800,
+            900,
+            1000,
+            1100,
+            1200,
+            1300,
+            1400,
+            1900,
+            2000,
+            2100,
+            2600
+        ],
         "TID": [
             "TID_GEAR_HEALING_TOME",
             "TID_GEAR_HEALING_TOME",
             "TID_GEAR_HEALING_TOME",
             "TID_GEAR_HEALING_TOME",
             "TID_GEAR_HEALING_TOME",
             "TID_GEAR_HEALING_TOME",
@@ -4387,14 +5167,34 @@
             1,
             1,
             1,
             1,
             1
         ],
         "Speed": [],
+        "StrengthWeight": [
+            100,
+            200,
+            300,
+            400,
+            500,
+            600,
+            700,
+            800,
+            900,
+            1000,
+            1100,
+            1200,
+            1300,
+            1400,
+            1900,
+            2000,
+            2100,
+            2600
+        ],
         "TID": [
             "TID_GEAR_HOG_TOTEM",
             "TID_GEAR_HOG_TOTEM",
             "TID_GEAR_HOG_TOTEM",
             "TID_GEAR_HOG_TOTEM",
             "TID_GEAR_HOG_TOTEM",
             "TID_GEAR_HOG_TOTEM",
@@ -4719,14 +5519,34 @@
             1,
             1,
             1,
             1,
             1
         ],
         "Speed": [],
+        "StrengthWeight": [
+            100,
+            200,
+            300,
+            400,
+            500,
+            600,
+            700,
+            800,
+            900,
+            1000,
+            1100,
+            1200,
+            1300,
+            1400,
+            1900,
+            2000,
+            2100,
+            2600
+        ],
         "TID": [
             "TID_GEAR_TITLE_IRON_FIST",
             "TID_GEAR_TITLE_IRON_FIST",
             "TID_GEAR_TITLE_IRON_FIST",
             "TID_GEAR_TITLE_IRON_FIST",
             "TID_GEAR_TITLE_IRON_FIST",
             "TID_GEAR_TITLE_IRON_FIST",
@@ -5051,14 +5871,34 @@
             1,
             1,
             1,
             1,
             1
         ],
         "Speed": [],
+        "StrengthWeight": [
+            100,
+            200,
+            300,
+            400,
+            500,
+            600,
+            700,
+            800,
+            900,
+            1000,
+            1100,
+            1200,
+            1300,
+            1400,
+            1900,
+            2000,
+            2100,
+            2600
+        ],
         "TID": [
             "TID_GEAR_TITLE_LIFE_GEM",
             "TID_GEAR_TITLE_LIFE_GEM",
             "TID_GEAR_TITLE_LIFE_GEM",
             "TID_GEAR_TITLE_LIFE_GEM",
             "TID_GEAR_TITLE_LIFE_GEM",
             "TID_GEAR_TITLE_LIFE_GEM",
@@ -5383,14 +6223,34 @@
             1,
             1,
             1,
             1,
             1
         ],
         "Speed": [],
+        "StrengthWeight": [
+            100,
+            200,
+            300,
+            400,
+            500,
+            600,
+            700,
+            800,
+            900,
+            1000,
+            1100,
+            1200,
+            1300,
+            1400,
+            1900,
+            2000,
+            2100,
+            2600
+        ],
         "TID": [
             "TID_GEAR_PIERCING_ARROW",
             "TID_GEAR_PIERCING_ARROW",
             "TID_GEAR_PIERCING_ARROW",
             "TID_GEAR_PIERCING_ARROW",
             "TID_GEAR_PIERCING_ARROW",
             "TID_GEAR_PIERCING_ARROW",
@@ -5715,14 +6575,34 @@
             1,
             1,
             1,
             1,
             1
         ],
         "Speed": [],
+        "StrengthWeight": [
+            100,
+            200,
+            300,
+            400,
+            500,
+            600,
+            700,
+            800,
+            900,
+            1000,
+            1100,
+            1200,
+            1300,
+            1400,
+            1900,
+            2000,
+            2100,
+            2600
+        ],
         "TID": [
             "TID_GEAR_PROTECTIVE_CLOAK",
             "TID_GEAR_PROTECTIVE_CLOAK",
             "TID_GEAR_PROTECTIVE_CLOAK",
             "TID_GEAR_PROTECTIVE_CLOAK",
             "TID_GEAR_PROTECTIVE_CLOAK",
             "TID_GEAR_PROTECTIVE_CLOAK",
@@ -5776,308 +6656,14 @@
             "CommonOre; RareOre",
             "CommonOre",
             "CommonOre",
             "CommonOre; RareOre",
             "CommonOre; RareOre"
         ]
     },
-    "Protective RC Gear": {
-        "AllowedCharacters": [
-            "Warrior Princess;",
-            "Warrior Princess;",
-            "Warrior Princess;",
-            "Warrior Princess;",
-            "Warrior Princess;",
-            "Warrior Princess;",
-            "Warrior Princess;",
-            "Warrior Princess;",
-            "Warrior Princess;",
-            "Warrior Princess;",
-            "Warrior Princess;",
-            "Warrior Princess;",
-            "Warrior Princess;",
-            "Warrior Princess;",
-            "Warrior Princess;",
-            "Warrior Princess;",
-            "Warrior Princess;",
-            "Warrior Princess;"
-        ],
-        "AttackRange": [],
-        "AttackSpeedPercentage": [],
-        "Claimable": [],
-        "DPS": [],
-        "Deprecated": [
-            true,
-            true,
-            true,
-            true,
-            true,
-            true,
-            true,
-            true,
-            true,
-            true,
-            true,
-            true,
-            true,
-            true,
-            true,
-            true,
-            true,
-            true
-        ],
-        "DiamondValue": [],
-        "ExtraAbilities": [],
-        "ExtraAbilityLevels": [],
-        "HealOnActivation": [
-            363,
-            423,
-            484,
-            544,
-            605,
-            665,
-            726,
-            786,
-            907,
-            1108,
-            1310,
-            1511,
-            1713,
-            1914,
-            2116,
-            2317,
-            2519,
-            2720
-        ],
-        "HitPoints": [
-            123,
-            143,
-            164,
-            184,
-            205,
-            225,
-            246,
-            266,
-            307,
-            375,
-            443,
-            511,
-            579,
-            648,
-            716,
-            784,
-            852,
-            920
-        ],
-        "IconExportName": [
-            "icon_gear_GW_HeartTome",
-            "icon_gear_GW_HeartTome",
-            "icon_gear_GW_HeartTome",
-            "icon_gear_GW_HeartTome",
-            "icon_gear_GW_HeartTome",
-            "icon_gear_GW_HeartTome",
-            "icon_gear_GW_HeartTome",
-            "icon_gear_GW_HeartTome",
-            "icon_gear_GW_HeartTome",
-            "icon_gear_GW_HeartTome",
-            "icon_gear_GW_HeartTome",
-            "icon_gear_GW_HeartTome",
-            "icon_gear_GW_HeartTome",
-            "icon_gear_GW_HeartTome",
-            "icon_gear_GW_HeartTome",
-            "icon_gear_GW_HeartTome",
-            "icon_gear_GW_HeartTome",
-            "icon_gear_GW_HeartTome"
-        ],
-        "IconSWF": [
-            "sc/ui.sc",
-            "sc/ui.sc",
-            "sc/ui.sc",
-            "sc/ui.sc",
-            "sc/ui.sc",
-            "sc/ui.sc",
-            "sc/ui.sc",
-            "sc/ui.sc",
-            "sc/ui.sc",
-            "sc/ui.sc",
-            "sc/ui.sc",
-            "sc/ui.sc",
-            "sc/ui.sc",
-            "sc/ui.sc",
-            "sc/ui.sc",
-            "sc/ui.sc",
-            "sc/ui.sc",
-            "sc/ui.sc"
-        ],
-        "InfoTID": [
-            "TID_GEAR_INFO_PROTECTIVE_CLOAK",
-            "TID_GEAR_INFO_PROTECTIVE_CLOAK",
-            "TID_GEAR_INFO_PROTECTIVE_CLOAK",
-            "TID_GEAR_INFO_PROTECTIVE_CLOAK",
-            "TID_GEAR_INFO_PROTECTIVE_CLOAK",
-            "TID_GEAR_INFO_PROTECTIVE_CLOAK",
-            "TID_GEAR_INFO_PROTECTIVE_CLOAK",
-            "TID_GEAR_INFO_PROTECTIVE_CLOAK",
-            "TID_GEAR_INFO_PROTECTIVE_CLOAK",
-            "TID_GEAR_INFO_PROTECTIVE_CLOAK",
-            "TID_GEAR_INFO_PROTECTIVE_CLOAK",
-            "TID_GEAR_INFO_PROTECTIVE_CLOAK",
-            "TID_GEAR_INFO_PROTECTIVE_CLOAK",
-            "TID_GEAR_INFO_PROTECTIVE_CLOAK",
-            "TID_GEAR_INFO_PROTECTIVE_CLOAK",
-            "TID_GEAR_INFO_PROTECTIVE_CLOAK",
-            "TID_GEAR_INFO_PROTECTIVE_CLOAK",
-            "TID_GEAR_INFO_PROTECTIVE_CLOAK"
-        ],
-        "Level": [
-            1,
-            2,
-            3,
-            4,
-            5,
-            6,
-            7,
-            8,
-            9,
-            10,
-            11,
-            12,
-            13,
-            14,
-            15,
-            16,
-            17,
-            18
-        ],
-        "MainAbilities": [
-            "RCProtectiveCloak",
-            "RCProtectiveCloak",
-            "RCProtectiveCloak",
-            "RCProtectiveCloak",
-            "RCProtectiveCloak",
-            "RCProtectiveCloak",
-            "RCProtectiveCloak",
-            "RCProtectiveCloak",
-            "RCProtectiveCloak",
-            "RCProtectiveCloak",
-            "RCProtectiveCloak",
-            "RCProtectiveCloak",
-            "RCProtectiveCloak",
-            "RCProtectiveCloak",
-            "RCProtectiveCloak",
-            "RCProtectiveCloak",
-            "RCProtectiveCloak",
-            "RCProtectiveCloak"
-        ],
-        "MainAbilityLevels": [
-            1,
-            1,
-            2,
-            2,
-            2,
-            3,
-            3,
-            3,
-            4,
-            4,
-            4,
-            5,
-            5,
-            5,
-            6,
-            6,
-            6,
-            7
-        ],
-        "Name": [],
-        "PreviewScenario": [],
-        "Rarity": [
-            "Common",
-            "Common",
-            "Common",
-            "Common",
-            "Common",
-            "Common",
-            "Common",
-            "Common",
-            "Common",
-            "Common",
-            "Common",
-            "Common",
-            "Common",
-            "Common",
-            "Common",
-            "Common",
-            "Common",
-            "Common"
-        ],
-        "RequiredBlacksmithLevel": [
-            6,
-            6,
-            6,
-            6,
-            6,
-            6,
-            6,
-            6,
-            6,
-            6,
-            6,
-            6,
-            6,
-            6,
-            6,
-            7,
-            7,
-            7
-        ],
-        "RequiredCharacterLevel": [
-            1,
-            1,
-            1,
-            1,
-            1,
-            1,
-            1,
-            1,
-            1,
-            1,
-            1,
-            1,
-            1,
-            1,
-            1,
-            1,
-            1,
-            1
-        ],
-        "Speed": [],
-        "TID": [
-            "TID_GEAR_PROTECTIVE_CLOAK",
-            "TID_GEAR_PROTECTIVE_CLOAK",
-            "TID_GEAR_PROTECTIVE_CLOAK",
-            "TID_GEAR_PROTECTIVE_CLOAK",
-            "TID_GEAR_PROTECTIVE_CLOAK",
-            "TID_GEAR_PROTECTIVE_CLOAK",
-            "TID_GEAR_PROTECTIVE_CLOAK",
-            "TID_GEAR_PROTECTIVE_CLOAK",
-            "TID_GEAR_PROTECTIVE_CLOAK",
-            "TID_GEAR_PROTECTIVE_CLOAK",
-            "TID_GEAR_PROTECTIVE_CLOAK",
-            "TID_GEAR_PROTECTIVE_CLOAK",
-            "TID_GEAR_PROTECTIVE_CLOAK",
-            "TID_GEAR_PROTECTIVE_CLOAK",
-            "TID_GEAR_PROTECTIVE_CLOAK",
-            "TID_GEAR_PROTECTIVE_CLOAK",
-            "TID_GEAR_PROTECTIVE_CLOAK",
-            "TID_GEAR_PROTECTIVE_CLOAK"
-        ],
-        "UpgradeCosts": [],
-        "UpgradeResources": []
-    },
     "Rocket Spear": {
         "AllowedCharacters": [
             "Warrior Princess;",
             "Warrior Princess;",
             "Warrior Princess;",
             "Warrior Princess;",
             "Warrior Princess;",
@@ -6486,14 +7072,43 @@
             1,
             1,
             1,
             1,
             1
         ],
         "Speed": [],
+        "StrengthWeight": [
+            100,
+            200,
+            300,
+            400,
+            500,
+            600,
+            700,
+            800,
+            900,
+            1000,
+            1100,
+            1200,
+            1300,
+            1400,
+            1900,
+            2000,
+            2100,
+            2600,
+            2700,
+            2800,
+            3300,
+            3400,
+            3500,
+            4000,
+            4100,
+            4200,
+            4700
+        ],
         "TID": [
             "TID_GEAR_ROCKET_SPEAR",
             "TID_GEAR_ROCKET_SPEAR",
             "TID_GEAR_ROCKET_SPEAR",
             "TID_GEAR_ROCKET_SPEAR",
             "TID_GEAR_ROCKET_SPEAR",
             "TID_GEAR_ROCKET_SPEAR",
@@ -6826,14 +7441,34 @@
             1,
             1,
             1,
             1,
             1
         ],
         "Speed": [],
+        "StrengthWeight": [
+            100,
+            200,
+            300,
+            400,
+            500,
+            600,
+            700,
+            800,
+            900,
+            1000,
+            1100,
+            1200,
+            1300,
+            1400,
+            1900,
+            2000,
+            2100,
+            2600
+        ],
         "TID": [
             "TID_GEAR_TITLE_ROYAL_CLOAK",
             "TID_GEAR_TITLE_ROYAL_CLOAK",
             "TID_GEAR_TITLE_ROYAL_CLOAK",
             "TID_GEAR_TITLE_ROYAL_CLOAK",
             "TID_GEAR_TITLE_ROYAL_CLOAK",
             "TID_GEAR_TITLE_ROYAL_CLOAK",
@@ -7139,14 +7774,34 @@
             1,
             1,
             1,
             1,
             1
         ],
         "Speed": [],
+        "StrengthWeight": [
+            100,
+            200,
+            300,
+            400,
+            500,
+            600,
+            700,
+            800,
+            900,
+            1000,
+            1100,
+            1200,
+            1300,
+            1400,
+            1900,
+            2000,
+            2100,
+            2600
+        ],
         "TID": [
             "TID_GEAR_TITLE_SEEKING_SHIELD",
             "TID_GEAR_TITLE_SEEKING_SHIELD",
             "TID_GEAR_TITLE_SEEKING_SHIELD",
             "TID_GEAR_TITLE_SEEKING_SHIELD",
             "TID_GEAR_TITLE_SEEKING_SHIELD",
             "TID_GEAR_TITLE_SEEKING_SHIELD",
@@ -7200,17 +7855,17 @@
             "CommonOre; RareOre",
             "CommonOre",
             "CommonOre",
             "CommonOre; RareOre",
             "CommonOre; RareOre"
         ]
     },
-    "UNUSED10": {
+    "UNUSED1": {
         "AllowedCharacters": [
-            "Grand Warden;"
+            "Archer Queen;"
         ],
         "AttackRange": [],
         "AttackSpeedPercentage": [],
         "Claimable": [],
         "DPS": [],
         "Deprecated": [
             true
@@ -7241,23 +7896,24 @@
         "RequiredBlacksmithLevel": [
             1
         ],
         "RequiredCharacterLevel": [
             1
         ],
         "Speed": [],
+        "StrengthWeight": [],
         "TID": [
             "TID_GEAR_TITLE_BARBARIAN_CROWN"
         ],
         "UpgradeCosts": [],
         "UpgradeResources": []
     },
-    "UNUSED11": {
+    "UNUSED10": {
         "AllowedCharacters": [
-            "Grand Warden;"
+            "Warrior Princess;"
         ],
         "AttackRange": [],
         "AttackSpeedPercentage": [],
         "Claimable": [],
         "DPS": [],
         "Deprecated": [
             true
@@ -7288,23 +7944,84 @@
         "RequiredBlacksmithLevel": [
             1
         ],
         "RequiredCharacterLevel": [
             1
         ],
         "Speed": [],
+        "StrengthWeight": [],
         "TID": [
             "TID_GEAR_TITLE_BARBARIAN_CROWN"
         ],
         "UpgradeCosts": [],
         "UpgradeResources": []
     },
+    "UNUSED11": {
+        "AllowedCharacters": [
+            "Warrior Princess;"
+        ],
+        "AttackRange": [],
+        "AttackSpeedPercentage": [
+            5
+        ],
+        "Claimable": [],
+        "DPS": [],
+        "Deprecated": [
+            true
+        ],
+        "DiamondValue": [],
+        "ExtraAbilities": [],
+        "ExtraAbilityLevels": [],
+        "HealOnActivation": [
+            150
+        ],
+        "HitPoints": [],
+        "IconExportName": [
+            "icon_unit_a"
+        ],
+        "IconSWF": [
+            "sc/ui.sc"
+        ],
+        "InfoTID": [
+            "TID_GEAR_INFO_HOG_TOTEM"
+        ],
+        "Level": [
+            1
+        ],
+        "MainAbilities": [
+            "RCEquipSpawnHogs"
+        ],
+        "MainAbilityLevels": [
+            1
+        ],
+        "PreviewScenario": [],
+        "Rarity": [
+            "Common"
+        ],
+        "RequiredBlacksmithLevel": [
+            7
+        ],
+        "RequiredCharacterLevel": [
+            1
+        ],
+        "Speed": [],
+        "StrengthWeight": [],
+        "TID": [
+            "TID_GEAR_HOG_TOTEM"
+        ],
+        "UpgradeCosts": [
+            120
+        ],
+        "UpgradeResources": [
+            "CommonOre"
+        ]
+    },
     "UNUSED12": {
         "AllowedCharacters": [
-            "Grand Warden;"
+            "Warrior Princess;"
         ],
         "AttackRange": [],
         "AttackSpeedPercentage": [],
         "Claimable": [],
         "DPS": [],
         "Deprecated": [
             true
@@ -7335,23 +8052,24 @@
         "RequiredBlacksmithLevel": [
             1
         ],
         "RequiredCharacterLevel": [
             1
         ],
         "Speed": [],
+        "StrengthWeight": [],
         "TID": [
             "TID_GEAR_TITLE_BARBARIAN_CROWN"
         ],
         "UpgradeCosts": [],
         "UpgradeResources": []
     },
     "UNUSED13": {
         "AllowedCharacters": [
-            "Warrior Princess;"
+            "Barbarian King;"
         ],
         "AttackRange": [],
         "AttackSpeedPercentage": [],
         "Claimable": [],
         "DPS": [],
         "Deprecated": [
             true
@@ -7369,27 +8087,32 @@
         ],
         "InfoTID": [
             "TID_GEAR_INFO_BARBARIAN_CROWN"
         ],
         "Level": [
             1
         ],
-        "MainAbilities": [],
-        "MainAbilityLevels": [],
+        "MainAbilities": [
+            "BarbarianKingSpawnOnTakeDamage"
+        ],
+        "MainAbilityLevels": [
+            1
+        ],
         "PreviewScenario": [],
         "Rarity": [
-            "Common"
+            "Epic"
         ],
         "RequiredBlacksmithLevel": [
             1
         ],
         "RequiredCharacterLevel": [
             1
         ],
         "Speed": [],
+        "StrengthWeight": [],
         "TID": [
             "TID_GEAR_TITLE_BARBARIAN_CROWN"
         ],
         "UpgradeCosts": [],
         "UpgradeResources": []
     },
     "UNUSED14": {
@@ -7416,95 +8139,137 @@
         ],
         "InfoTID": [
             "TID_GEAR_INFO_BARBARIAN_CROWN"
         ],
         "Level": [
             1
         ],
-        "MainAbilities": [],
-        "MainAbilityLevels": [],
+        "MainAbilities": [
+            "RoyalChampionElectrifiedShield"
+        ],
+        "MainAbilityLevels": [
+            1
+        ],
         "PreviewScenario": [],
         "Rarity": [
             "Common"
         ],
         "RequiredBlacksmithLevel": [
-            1
+            6
         ],
         "RequiredCharacterLevel": [
             1
         ],
         "Speed": [],
+        "StrengthWeight": [],
         "TID": [
             "TID_GEAR_TITLE_BARBARIAN_CROWN"
         ],
         "UpgradeCosts": [],
         "UpgradeResources": []
     },
     "UNUSED15": {
         "AllowedCharacters": [
-            "Warrior Princess;"
+            "Archer Queen;"
         ],
         "AttackRange": [],
-        "AttackSpeedPercentage": [
-            5
-        ],
+        "AttackSpeedPercentage": [],
         "Claimable": [],
         "DPS": [],
         "Deprecated": [
             true
         ],
         "DiamondValue": [],
         "ExtraAbilities": [],
         "ExtraAbilityLevels": [],
-        "HealOnActivation": [
-            150
-        ],
+        "HealOnActivation": [],
         "HitPoints": [],
         "IconExportName": [
             "icon_unit_a"
         ],
         "IconSWF": [
             "sc/ui.sc"
         ],
         "InfoTID": [
-            "TID_GEAR_INFO_HOG_TOTEM"
+            "TID_GEAR_INFO_BARBARIAN_CROWN"
         ],
         "Level": [
             1
         ],
-        "MainAbilities": [
-            "RCEquipSpawnHogs"
+        "MainAbilities": [],
+        "MainAbilityLevels": [],
+        "PreviewScenario": [],
+        "Rarity": [
+            "Common"
         ],
-        "MainAbilityLevels": [
+        "RequiredBlacksmithLevel": [
+            1
+        ],
+        "RequiredCharacterLevel": [
+            1
+        ],
+        "Speed": [],
+        "StrengthWeight": [],
+        "TID": [
+            "TID_GEAR_TITLE_BARBARIAN_CROWN"
+        ],
+        "UpgradeCosts": [],
+        "UpgradeResources": []
+    },
+    "UNUSED16": {
+        "AllowedCharacters": [
+            "Archer Queen;"
+        ],
+        "AttackRange": [],
+        "AttackSpeedPercentage": [],
+        "Claimable": [],
+        "DPS": [],
+        "Deprecated": [
+            true
+        ],
+        "DiamondValue": [],
+        "ExtraAbilities": [],
+        "ExtraAbilityLevels": [],
+        "HealOnActivation": [],
+        "HitPoints": [],
+        "IconExportName": [
+            "icon_unit_a"
+        ],
+        "IconSWF": [
+            "sc/ui.sc"
+        ],
+        "InfoTID": [
+            "TID_GEAR_INFO_BARBARIAN_CROWN"
+        ],
+        "Level": [
             1
         ],
+        "MainAbilities": [],
+        "MainAbilityLevels": [],
         "PreviewScenario": [],
         "Rarity": [
             "Common"
         ],
         "RequiredBlacksmithLevel": [
-            7
+            1
         ],
         "RequiredCharacterLevel": [
             1
         ],
         "Speed": [],
+        "StrengthWeight": [],
         "TID": [
-            "TID_GEAR_HOG_TOTEM"
-        ],
-        "UpgradeCosts": [
-            120
+            "TID_GEAR_TITLE_BARBARIAN_CROWN"
         ],
-        "UpgradeResources": [
-            "CommonOre"
-        ]
+        "UpgradeCosts": [],
+        "UpgradeResources": []
     },
-    "UNUSED16": {
+    "UNUSED17": {
         "AllowedCharacters": [
-            "Warrior Princess;"
+            "Archer Queen;"
         ],
         "AttackRange": [],
         "AttackSpeedPercentage": [],
         "Claimable": [],
         "DPS": [],
         "Deprecated": [
             true
@@ -7535,23 +8300,24 @@
         "RequiredBlacksmithLevel": [
             1
         ],
         "RequiredCharacterLevel": [
             1
         ],
         "Speed": [],
+        "StrengthWeight": [],
         "TID": [
             "TID_GEAR_TITLE_BARBARIAN_CROWN"
         ],
         "UpgradeCosts": [],
         "UpgradeResources": []
     },
-    "UNUSED17": {
+    "UNUSED18": {
         "AllowedCharacters": [
-            "Barbarian King;"
+            "Archer Queen;"
         ],
         "AttackRange": [],
         "AttackSpeedPercentage": [],
         "Claimable": [],
         "DPS": [],
         "Deprecated": [
             true
@@ -7569,40 +8335,85 @@
         ],
         "InfoTID": [
             "TID_GEAR_INFO_BARBARIAN_CROWN"
         ],
         "Level": [
             1
         ],
-        "MainAbilities": [
-            "BarbarianKingSpawnOnTakeDamage"
+        "MainAbilities": [],
+        "MainAbilityLevels": [],
+        "PreviewScenario": [],
+        "Rarity": [
+            "Common"
         ],
-        "MainAbilityLevels": [
+        "RequiredBlacksmithLevel": [
+            1
+        ],
+        "RequiredCharacterLevel": [
             1
         ],
+        "Speed": [],
+        "StrengthWeight": [],
+        "TID": [
+            "TID_GEAR_TITLE_BARBARIAN_CROWN"
+        ],
+        "UpgradeCosts": [],
+        "UpgradeResources": []
+    },
+    "UNUSED19": {
+        "AllowedCharacters": [
+            "Archer Queen;"
+        ],
+        "AttackRange": [],
+        "AttackSpeedPercentage": [],
+        "Claimable": [],
+        "DPS": [],
+        "Deprecated": [
+            true
+        ],
+        "DiamondValue": [],
+        "ExtraAbilities": [],
+        "ExtraAbilityLevels": [],
+        "HealOnActivation": [],
+        "HitPoints": [],
+        "IconExportName": [
+            "icon_unit_a"
+        ],
+        "IconSWF": [
+            "sc/ui.sc"
+        ],
+        "InfoTID": [
+            "TID_GEAR_INFO_BARBARIAN_CROWN"
+        ],
+        "Level": [
+            1
+        ],
+        "MainAbilities": [],
+        "MainAbilityLevels": [],
         "PreviewScenario": [],
         "Rarity": [
-            "Epic"
+            "Common"
         ],
         "RequiredBlacksmithLevel": [
             1
         ],
         "RequiredCharacterLevel": [
             1
         ],
         "Speed": [],
+        "StrengthWeight": [],
         "TID": [
             "TID_GEAR_TITLE_BARBARIAN_CROWN"
         ],
         "UpgradeCosts": [],
         "UpgradeResources": []
     },
-    "UNUSED18": {
+    "UNUSED2": {
         "AllowedCharacters": [
-            "Warrior Princess;"
+            "Archer Queen;"
         ],
         "AttackRange": [],
         "AttackSpeedPercentage": [],
         "Claimable": [],
         "DPS": [],
         "Deprecated": [
             true
@@ -7620,31 +8431,76 @@
         ],
         "InfoTID": [
             "TID_GEAR_INFO_BARBARIAN_CROWN"
         ],
         "Level": [
             1
         ],
-        "MainAbilities": [
-            "RoyalChampionElectrifiedShield"
+        "MainAbilities": [],
+        "MainAbilityLevels": [],
+        "PreviewScenario": [],
+        "Rarity": [
+            "Common"
         ],
-        "MainAbilityLevels": [
+        "RequiredBlacksmithLevel": [
             1
         ],
+        "RequiredCharacterLevel": [
+            1
+        ],
+        "Speed": [],
+        "StrengthWeight": [],
+        "TID": [
+            "TID_GEAR_TITLE_BARBARIAN_CROWN"
+        ],
+        "UpgradeCosts": [],
+        "UpgradeResources": []
+    },
+    "UNUSED3": {
+        "AllowedCharacters": [
+            "Archer Queen;"
+        ],
+        "AttackRange": [],
+        "AttackSpeedPercentage": [],
+        "Claimable": [],
+        "DPS": [],
+        "Deprecated": [
+            true
+        ],
+        "DiamondValue": [],
+        "ExtraAbilities": [],
+        "ExtraAbilityLevels": [],
+        "HealOnActivation": [],
+        "HitPoints": [],
+        "IconExportName": [
+            "icon_unit_a"
+        ],
+        "IconSWF": [
+            "sc/ui.sc"
+        ],
+        "InfoTID": [
+            "TID_GEAR_INFO_BARBARIAN_CROWN"
+        ],
+        "Level": [
+            1
+        ],
+        "MainAbilities": [],
+        "MainAbilityLevels": [],
         "PreviewScenario": [],
         "Rarity": [
             "Common"
         ],
         "RequiredBlacksmithLevel": [
-            6
+            1
         ],
         "RequiredCharacterLevel": [
             1
         ],
         "Speed": [],
+        "StrengthWeight": [],
         "TID": [
             "TID_GEAR_TITLE_BARBARIAN_CROWN"
         ],
         "UpgradeCosts": [],
         "UpgradeResources": []
     },
     "UNUSED4": {
@@ -7684,23 +8540,24 @@
         "RequiredBlacksmithLevel": [
             1
         ],
         "RequiredCharacterLevel": [
             1
         ],
         "Speed": [],
+        "StrengthWeight": [],
         "TID": [
             "TID_GEAR_TITLE_BARBARIAN_CROWN"
         ],
         "UpgradeCosts": [],
         "UpgradeResources": []
     },
     "UNUSED5": {
         "AllowedCharacters": [
-            "Archer Queen;"
+            "Grand Warden;"
         ],
         "AttackRange": [],
         "AttackSpeedPercentage": [],
         "Claimable": [],
         "DPS": [],
         "Deprecated": [
             true
@@ -7731,23 +8588,24 @@
         "RequiredBlacksmithLevel": [
             1
         ],
         "RequiredCharacterLevel": [
             1
         ],
         "Speed": [],
+        "StrengthWeight": [],
         "TID": [
             "TID_GEAR_TITLE_BARBARIAN_CROWN"
         ],
         "UpgradeCosts": [],
         "UpgradeResources": []
     },
     "UNUSED6": {
         "AllowedCharacters": [
-            "Archer Queen;"
+            "Grand Warden;"
         ],
         "AttackRange": [],
         "AttackSpeedPercentage": [],
         "Claimable": [],
         "DPS": [],
         "Deprecated": [
             true
@@ -7778,78 +8636,72 @@
         "RequiredBlacksmithLevel": [
             1
         ],
         "RequiredCharacterLevel": [
             1
         ],
         "Speed": [],
+        "StrengthWeight": [],
         "TID": [
             "TID_GEAR_TITLE_BARBARIAN_CROWN"
         ],
         "UpgradeCosts": [],
         "UpgradeResources": []
     },
     "UNUSED7": {
         "AllowedCharacters": [
-            "Archer Queen;"
+            "Grand Warden;"
         ],
         "AttackRange": [],
         "AttackSpeedPercentage": [],
         "Claimable": [],
-        "DPS": [
-            3
-        ],
+        "DPS": [],
         "Deprecated": [
             true
         ],
         "DiamondValue": [],
         "ExtraAbilities": [],
         "ExtraAbilityLevels": [],
         "HealOnActivation": [],
-        "HitPoints": [
-            10
-        ],
+        "HitPoints": [],
         "IconExportName": [
             "icon_unit_a"
         ],
         "IconSWF": [
             "sc/ui.sc"
         ],
         "InfoTID": [
             "TID_GEAR_INFO_BARBARIAN_CROWN"
         ],
         "Level": [
             1
         ],
-        "MainAbilities": [
-            "ArcherQueenExtraDamageWall"
-        ],
-        "MainAbilityLevels": [
-            1
-        ],
+        "MainAbilities": [],
+        "MainAbilityLevels": [],
         "PreviewScenario": [],
         "Rarity": [
             "Common"
         ],
         "RequiredBlacksmithLevel": [
-            3
+            1
         ],
         "RequiredCharacterLevel": [
             1
         ],
         "Speed": [],
+        "StrengthWeight": [],
         "TID": [
             "TID_GEAR_TITLE_BARBARIAN_CROWN"
         ],
         "UpgradeCosts": [],
         "UpgradeResources": []
     },
     "UNUSED8": {
         "AllowedCharacters": [
-            "Archer Queen;"
+            "Grand Warden;"
         ],
         "AttackRange": [],
         "AttackSpeedPercentage": [],
         "Claimable": [],
         "DPS": [],
         "Deprecated": [
             true
@@ -7880,23 +8732,24 @@
         "RequiredBlacksmithLevel": [
             1
         ],
         "RequiredCharacterLevel": [
             1
         ],
         "Speed": [],
+        "StrengthWeight": [],
         "TID": [
             "TID_GEAR_TITLE_BARBARIAN_CROWN"
         ],
         "UpgradeCosts": [],
         "UpgradeResources": []
     },
     "UNUSED9": {
         "AllowedCharacters": [
-            "Grand Warden;"
+            "Warrior Princess;"
         ],
         "AttackRange": [],
         "AttackSpeedPercentage": [],
         "Claimable": [],
         "DPS": [],
         "Deprecated": [
             true
@@ -7927,14 +8780,15 @@
         "RequiredBlacksmithLevel": [
             1
         ],
         "RequiredCharacterLevel": [
             1
         ],
         "Speed": [],
+        "StrengthWeight": [],
         "TID": [
             "TID_GEAR_TITLE_BARBARIAN_CROWN"
         ],
         "UpgradeCosts": [],
         "UpgradeResources": []
     },
     "Vampstache": {
@@ -8204,14 +9058,34 @@
             1,
             1,
             1,
             1,
             1
         ],
         "Speed": [],
+        "StrengthWeight": [
+            100,
+            200,
+            300,
+            400,
+            500,
+            600,
+            700,
+            800,
+            900,
+            1000,
+            1100,
+            1200,
+            1300,
+            1400,
+            1900,
+            2000,
+            2100,
+            2600
+        ],
         "TID": [
             "TID_GEAR_VAMPSTACHE",
             "TID_GEAR_VAMPSTACHE",
             "TID_GEAR_VAMPSTACHE",
             "TID_GEAR_VAMPSTACHE",
             "TID_GEAR_VAMPSTACHE",
             "TID_GEAR_VAMPSTACHE",
```

### Comparing `coc.py-3.4.1/coc/static/heroes.json` & `coc_py-3.4.2/coc/static/heroes.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9974358974358974%*

 * *Differences: {"'Archer Queen'": "{'StrengthWeight': [2520, 2574, 2638, 2694, 2815, 2883, 2942, 3019, 3080, "*

 * *                   '3212, 3284, 3368, 3451, 3524, 3678, 3757, 3844, 3945, 4032, 4203, 4305, 4400, '*

 * *                   '4506, 4612, 4805, 4915, 5027, 5139, 5265, 5486, 5616, 5743, 5873, 6017, 6270, '*

 * *                   '6407, 6569, 6705, 6870, 7155, 7322, 7491, 7663, 7846, 8170, 8361, 8550, 8756, '*

 * *                   '8961, 9326, 9530, 9739, 9972, 10198, 10773, 11011, 11264, 11520, 11780, 12429, '*

 * *                […]*

```diff
@@ -5675,206 +5675,206 @@
             300,
             300,
             300,
             300,
             300
         ],
         "StrengthWeight": [
-            50,
-            50,
-            50,
-            50,
-            51,
-            51,
-            51,
-            51,
-            51,
-            52,
-            52,
-            52,
-            52,
-            52,
-            53,
-            53,
-            53,
-            53,
-            53,
-            54,
-            54,
-            54,
-            54,
-            54,
-            55,
-            55,
-            55,
-            55,
-            55,
-            56,
-            56,
-            56,
-            56,
-            56,
-            57,
-            57,
-            57,
-            57,
-            57,
-            58,
-            58,
-            58,
-            58,
-            58,
-            59,
-            59,
-            59,
-            59,
-            59,
-            60,
-            60,
-            60,
-            60,
-            60,
-            62,
-            62,
-            62,
-            62,
-            62,
-            64,
-            64,
-            64,
-            64,
-            64,
-            66,
-            66,
-            66,
-            66,
-            66,
-            68,
-            68,
-            68,
-            68,
-            68,
-            70,
-            70,
-            70,
-            70,
-            70,
-            72,
-            72,
-            72,
-            72,
-            72,
-            74,
-            74,
-            74,
-            74,
-            74,
-            76,
-            76,
-            76,
-            76,
-            76,
-            78
+            2520,
+            2574,
+            2638,
+            2694,
+            2815,
+            2883,
+            2942,
+            3019,
+            3080,
+            3212,
+            3284,
+            3368,
+            3451,
+            3524,
+            3678,
+            3757,
+            3844,
+            3945,
+            4032,
+            4203,
+            4305,
+            4400,
+            4506,
+            4612,
+            4805,
+            4915,
+            5027,
+            5139,
+            5265,
+            5486,
+            5616,
+            5743,
+            5873,
+            6017,
+            6270,
+            6407,
+            6569,
+            6705,
+            6870,
+            7155,
+            7322,
+            7491,
+            7663,
+            7846,
+            8170,
+            8361,
+            8550,
+            8756,
+            8961,
+            9326,
+            9530,
+            9739,
+            9972,
+            10198,
+            10773,
+            11011,
+            11264,
+            11520,
+            11780,
+            12429,
+            12700,
+            12977,
+            13268,
+            13565,
+            14296,
+            14583,
+            14842,
+            15090,
+            15301,
+            15972,
+            16154,
+            16323,
+            16478,
+            16633,
+            17282,
+            17430,
+            17564,
+            17713,
+            17847,
+            18495,
+            18619,
+            18746,
+            18858,
+            18985,
+            19628,
+            19743,
+            19873,
+            19989,
+            20119,
+            20781,
+            20900,
+            21034,
+            21152,
+            21286,
+            21968
         ],
         "StrengthWeight2": [
-            28,
-            28,
-            28,
-            28,
-            29,
-            29,
-            29,
-            29,
-            29,
-            30,
-            30,
-            30,
-            30,
-            30,
-            31,
-            31,
-            31,
-            31,
-            31,
-            32,
-            32,
-            32,
-            32,
-            32,
-            33,
-            33,
-            33,
-            33,
-            33,
-            34,
-            34,
-            34,
-            34,
-            34,
-            35,
-            35,
-            35,
-            35,
-            35,
-            36,
-            36,
-            36,
-            36,
-            36,
-            37,
-            37,
-            37,
-            37,
-            37,
-            38,
-            38,
-            38,
-            38,
-            38,
-            39,
-            39,
-            39,
-            39,
-            39,
-            40,
-            40,
-            40,
-            40,
-            40,
-            41,
-            41,
-            41,
-            41,
-            41,
-            42,
-            42,
-            42,
-            42,
-            42,
-            43,
-            43,
-            43,
-            43,
-            43,
-            44,
-            44,
-            44,
-            44,
-            44,
-            45,
-            45,
-            45,
-            45,
-            45,
-            46,
-            46,
-            46,
-            46,
-            46,
-            47
+            1411,
+            1441,
+            1477,
+            1509,
+            1601,
+            1639,
+            1673,
+            1717,
+            1752,
+            1853,
+            1895,
+            1943,
+            1991,
+            2033,
+            2151,
+            2197,
+            2248,
+            2308,
+            2358,
+            2491,
+            2551,
+            2607,
+            2670,
+            2733,
+            2883,
+            2949,
+            3016,
+            3084,
+            3159,
+            3331,
+            3410,
+            3487,
+            3566,
+            3653,
+            3850,
+            3934,
+            4033,
+            4117,
+            4218,
+            4441,
+            4545,
+            4650,
+            4756,
+            4870,
+            5124,
+            5244,
+            5362,
+            5491,
+            5620,
+            5907,
+            6036,
+            6168,
+            6316,
+            6458,
+            6777,
+            6926,
+            7086,
+            7246,
+            7410,
+            7768,
+            7938,
+            8110,
+            8293,
+            8478,
+            8881,
+            9059,
+            9220,
+            9374,
+            9505,
+            9865,
+            9978,
+            10082,
+            10177,
+            10273,
+            10616,
+            10707,
+            10790,
+            10881,
+            10963,
+            11303,
+            11378,
+            11456,
+            11524,
+            11602,
+            11936,
+            12006,
+            12085,
+            12155,
+            12235,
+            12578,
+            12650,
+            12731,
+            12803,
+            12884,
+            13237
         ],
         "TID": [
             "TID_ARCHER_QUEEN",
             "TID_ARCHER_QUEEN",
             "TID_ARCHER_QUEEN",
             "TID_ARCHER_QUEEN",
             "TID_ARCHER_QUEEN",
@@ -12431,206 +12431,206 @@
             200,
             200,
             200,
             200,
             200
         ],
         "StrengthWeight": [
-            20,
-            20,
-            20,
-            20,
-            21,
-            21,
-            21,
-            21,
-            21,
-            22,
-            22,
-            22,
-            22,
-            22,
-            23,
-            23,
-            23,
-            23,
-            23,
-            24,
-            24,
-            24,
-            24,
-            24,
-            25,
-            25,
-            25,
-            25,
-            25,
-            26,
-            26,
-            26,
-            26,
-            26,
-            27,
-            27,
-            27,
-            27,
-            27,
-            28,
-            28,
-            28,
-            28,
-            28,
-            29,
-            29,
-            29,
-            29,
-            29,
-            30,
-            30,
-            30,
-            30,
-            30,
-            31,
-            31,
-            31,
-            31,
-            31,
-            32,
-            32,
-            32,
-            32,
-            32,
-            33,
-            33,
-            33,
-            33,
-            33,
-            34,
-            34,
-            34,
-            34,
-            34,
-            35,
-            35,
-            35,
-            35,
-            35,
-            36,
-            36,
-            36,
-            36,
-            36,
-            37,
-            37,
-            37,
-            37,
-            37,
-            38,
-            38,
-            38,
-            38,
-            38,
-            39
+            1564,
+            1601,
+            1634,
+            1677,
+            1802,
+            1844,
+            1890,
+            1929,
+            1978,
+            2125,
+            2174,
+            2227,
+            2277,
+            2334,
+            2495,
+            2556,
+            2613,
+            2680,
+            2740,
+            2927,
+            2997,
+            3069,
+            3141,
+            3220,
+            3433,
+            3513,
+            3596,
+            3679,
+            3770,
+            4015,
+            4108,
+            4209,
+            4310,
+            4414,
+            4694,
+            4800,
+            4914,
+            5035,
+            5154,
+            5471,
+            5655,
+            5792,
+            5932,
+            6074,
+            6440,
+            6593,
+            6756,
+            6915,
+            7084,
+            7506,
+            7688,
+            7874,
+            8063,
+            8262,
+            8747,
+            8955,
+            9174,
+            9397,
+            9622,
+            10180,
+            10417,
+            10665,
+            10925,
+            11185,
+            11813,
+            12098,
+            12379,
+            12668,
+            12962,
+            13641,
+            13933,
+            14219,
+            14511,
+            14797,
+            15533,
+            15809,
+            16090,
+            16366,
+            16647,
+            17414,
+            17647,
+            17875,
+            18108,
+            18343,
+            19092,
+            19333,
+            19566,
+            19807,
+            20047,
+            20836,
+            21082,
+            21323,
+            21569,
+            21817,
+            22643
         ],
         "StrengthWeight2": [
-            10,
-            10,
-            10,
-            10,
-            11,
-            11,
-            11,
-            11,
-            11,
-            12,
-            12,
-            12,
-            12,
-            12,
-            13,
-            13,
-            13,
-            13,
-            13,
-            14,
-            14,
-            14,
-            14,
-            14,
-            15,
-            15,
-            15,
-            15,
-            15,
-            16,
-            16,
-            16,
-            16,
-            16,
-            17,
-            17,
-            17,
-            17,
-            17,
-            18,
-            18,
-            18,
-            18,
-            18,
-            19,
-            19,
-            19,
-            19,
-            19,
-            20,
-            20,
-            20,
-            20,
-            20,
-            21,
-            21,
-            21,
-            21,
-            21,
-            22,
-            22,
-            22,
-            22,
-            22,
-            22,
-            22,
-            22,
-            22,
-            22,
-            22,
-            22,
-            22,
-            22,
-            22,
-            23,
-            23,
-            23,
-            23,
-            23,
-            23,
-            23,
-            23,
-            23,
-            23,
-            23,
-            23,
-            23,
-            23,
-            23,
-            23,
-            23,
-            23,
-            23,
-            23,
-            23
+            782,
+            800,
+            817,
+            838,
+            944,
+            966,
+            990,
+            1011,
+            1036,
+            1159,
+            1186,
+            1215,
+            1242,
+            1273,
+            1410,
+            1445,
+            1477,
+            1515,
+            1549,
+            1707,
+            1748,
+            1790,
+            1832,
+            1878,
+            2060,
+            2108,
+            2158,
+            2207,
+            2262,
+            2471,
+            2528,
+            2590,
+            2652,
+            2716,
+            2955,
+            3022,
+            3094,
+            3170,
+            3245,
+            3517,
+            3635,
+            3723,
+            3813,
+            3905,
+            4220,
+            4320,
+            4426,
+            4530,
+            4641,
+            5004,
+            5126,
+            5250,
+            5375,
+            5508,
+            5925,
+            6066,
+            6214,
+            6366,
+            6518,
+            6999,
+            7161,
+            7332,
+            7511,
+            7689,
+            7875,
+            8065,
+            8253,
+            8445,
+            8642,
+            8826,
+            9016,
+            9200,
+            9390,
+            9574,
+            10207,
+            10389,
+            10574,
+            10755,
+            10940,
+            11126,
+            11275,
+            11420,
+            11569,
+            11719,
+            11868,
+            12018,
+            12162,
+            12312,
+            12461,
+            12611,
+            12760,
+            12906,
+            13055,
+            13205,
+            13354
         ],
         "TID": [
             "TID_BARBARIAN_KING",
             "TID_BARBARIAN_KING",
             "TID_BARBARIAN_KING",
             "TID_BARBARIAN_KING",
             "TID_BARBARIAN_KING",
@@ -20168,156 +20168,156 @@
             200,
             200,
             200,
             200,
             200
         ],
         "StrengthWeight": [
-            140,
-            140,
-            140,
-            140,
-            145,
-            145,
-            145,
-            145,
-            145,
-            150,
-            150,
-            150,
-            150,
-            150,
-            155,
-            155,
-            155,
-            155,
-            155,
-            160,
-            160,
-            160,
-            160,
-            160,
-            165,
-            165,
-            165,
-            165,
-            165,
-            170,
-            170,
-            170,
-            170,
-            170,
-            175,
-            175,
-            175,
-            175,
-            175,
-            180,
-            180,
-            180,
-            180,
-            180,
-            185,
-            185,
-            185,
-            185,
-            185,
-            190,
-            190,
-            190,
-            190,
-            190,
-            195,
-            195,
-            195,
-            195,
-            195,
-            200,
-            200,
-            200,
-            200,
-            200,
-            205,
-            205,
-            205,
-            205,
-            205,
-            210
+            6150,
+            6300,
+            6450,
+            6600,
+            7000,
+            7150,
+            7300,
+            7450,
+            7600,
+            8000,
+            8150,
+            8300,
+            8450,
+            8600,
+            9000,
+            9300,
+            9600,
+            9900,
+            10200,
+            11000,
+            11300,
+            11600,
+            11900,
+            12200,
+            13000,
+            13300,
+            13600,
+            13900,
+            14200,
+            15000,
+            15450,
+            15900,
+            16350,
+            16800,
+            18000,
+            18450,
+            18900,
+            19350,
+            19800,
+            21000,
+            21300,
+            21600,
+            21900,
+            22200,
+            23000,
+            23300,
+            23600,
+            23900,
+            24200,
+            25000,
+            25300,
+            25600,
+            25900,
+            26200,
+            27000,
+            27300,
+            27600,
+            27900,
+            28200,
+            29000,
+            29300,
+            29600,
+            29900,
+            30200,
+            31000,
+            31150,
+            31300,
+            31450,
+            31600,
+            32000
         ],
         "StrengthWeight2": [
-            70,
-            70,
-            70,
-            70,
-            71,
-            71,
-            71,
-            71,
-            71,
-            72,
-            72,
-            72,
-            72,
-            72,
-            73,
-            73,
-            73,
-            73,
-            73,
-            74,
-            74,
-            74,
-            74,
-            74,
-            75,
-            75,
-            75,
-            75,
-            75,
-            76,
-            76,
-            76,
-            76,
-            76,
-            77,
-            77,
-            77,
-            77,
-            77,
-            78,
-            78,
-            78,
-            78,
-            78,
-            79,
-            79,
-            79,
-            79,
-            79,
-            80,
-            80,
-            80,
-            80,
-            80,
-            81,
-            81,
-            81,
-            81,
-            81,
-            82,
-            82,
-            82,
-            82,
-            82,
-            83,
-            83,
-            83,
-            83,
-            83,
-            84
+            2982,
+            3046,
+            3125,
+            3203,
+            3317,
+            3399,
+            3496,
+            3584,
+            3686,
+            3830,
+            3940,
+            4038,
+            4167,
+            4283,
+            4476,
+            4593,
+            4713,
+            4844,
+            4964,
+            5165,
+            5301,
+            5438,
+            5577,
+            5731,
+            5967,
+            6129,
+            6291,
+            6456,
+            6636,
+            6910,
+            7098,
+            7287,
+            7494,
+            7685,
+            7999,
+            8230,
+            8448,
+            8683,
+            8938,
+            9294,
+            9441,
+            9572,
+            9688,
+            9803,
+            10030,
+            10147,
+            10248,
+            10349,
+            10466,
+            10701,
+            10819,
+            10922,
+            11024,
+            11142,
+            11385,
+            11489,
+            11577,
+            11680,
+            11768,
+            12018,
+            12106,
+            12211,
+            12316,
+            12405,
+            12662,
+            12752,
+            12858,
+            12948,
+            13054,
+            13302
         ],
         "TID": [
             "TID_GRAND_WARDEN",
             "TID_GRAND_WARDEN",
             "TID_GRAND_WARDEN",
             "TID_GRAND_WARDEN",
             "TID_GRAND_WARDEN",
@@ -25856,106 +25856,106 @@
             300,
             300,
             300,
             300,
             300
         ],
         "StrengthWeight": [
-            110,
-            110,
-            110,
-            110,
-            150,
-            150,
-            150,
-            150,
-            150,
-            160,
-            160,
-            160,
-            160,
-            160,
-            170,
-            170,
-            170,
-            170,
-            170,
-            180,
-            180,
-            180,
-            180,
-            180,
-            190,
-            190,
-            190,
-            190,
-            190,
-            200,
-            200,
-            200,
-            200,
-            200,
-            200,
-            200,
-            200,
-            200,
-            200,
-            200,
-            200,
-            200,
-            200,
-            200,
-            200
+            20000,
+            21000,
+            22000,
+            23000,
+            25000,
+            26000,
+            27000,
+            28000,
+            29000,
+            31000,
+            32000,
+            33000,
+            34000,
+            35000,
+            36000,
+            37000,
+            38000,
+            39000,
+            40000,
+            41000,
+            41500,
+            42000,
+            42500,
+            43000,
+            44000,
+            44500,
+            45000,
+            45500,
+            46000,
+            47000,
+            47100,
+            47200,
+            47300,
+            47400,
+            48000,
+            48100,
+            48200,
+            48300,
+            48400,
+            49000,
+            49100,
+            49200,
+            49300,
+            49400,
+            50000
         ],
         "StrengthWeight2": [
-            31,
-            31,
-            31,
-            31,
-            33,
-            33,
-            33,
-            33,
-            33,
-            35,
-            35,
-            35,
-            35,
-            35,
-            37,
-            37,
-            37,
-            37,
-            37,
-            39,
-            39,
-            39,
-            39,
-            39,
-            41,
-            41,
-            41,
-            41,
-            41,
-            43,
-            43,
-            43,
-            43,
-            43,
-            45,
-            45,
-            45,
-            45,
-            45,
-            47,
-            47,
-            47,
-            47,
-            47,
-            49
+            5218,
+            5332,
+            5447,
+            5561,
+            6010,
+            6098,
+            6188,
+            6277,
+            6373,
+            6860,
+            6962,
+            7063,
+            7165,
+            7266,
+            7789,
+            7896,
+            8004,
+            8096,
+            8189,
+            8728,
+            8812,
+            8904,
+            8996,
+            9081,
+            9627,
+            9707,
+            9788,
+            9868,
+            9948,
+            10518,
+            10588,
+            10657,
+            10736,
+            10814,
+            11399,
+            11480,
+            11563,
+            11644,
+            11727,
+            12333,
+            12410,
+            12485,
+            12562,
+            12637,
+            13255
         ],
         "TID": [
             "TID_HERO_ROYAL_CHAMPION",
             "TID_HERO_ROYAL_CHAMPION",
             "TID_HERO_ROYAL_CHAMPION",
             "TID_HERO_ROYAL_CHAMPION",
             "TID_HERO_ROYAL_CHAMPION",
```

### Comparing `coc.py-3.4.1/coc/static/pets.json` & `coc_py-3.4.2/coc/static/pets.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9967278030775371%*

 * *Differences: {"'Angry Jelly'": "{'Deprecated': [], 'TID': ['TID_PET_ANGRY_JELLY', 'TID_PET_ANGRY_JELLY', "*

 * *                  "'TID_PET_ANGRY_JELLY', 'TID_PET_ANGRY_JELLY', 'TID_PET_ANGRY_JELLY', "*

 * *                  "'TID_PET_ANGRY_JELLY', 'TID_PET_ANGRY_JELLY', 'TID_PET_ANGRY_JELLY', "*

 * *                  "'TID_PET_ANGRY_JELLY', 'TID_PET_ANGRY_JELLY'], 'InfoTID': "*

 * *                  "['TID_PET_ANGRY_JELLY_INFO', 'TID_PET_ANGRY_JELLY_INFO', "*

 * *                  "'TID_PET_ANGRY_JELLY_INFO', 'TID_PET_ANGRY_JELLY_INFO', "*

 * *     […]*

```diff
@@ -273,110 +273,110 @@
         ],
         "UpgradeTimeM": [],
         "VillageType": [],
         "WallMovementCost": []
     },
     "Angry Jelly": {
         "AirTargets": [
-            false,
-            false,
-            false,
-            false,
-            false,
-            false,
-            false,
-            false,
-            false,
-            false
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true,
+            true
         ],
         "AltProjectile": [],
         "Animation": [
-            "AngryChihuahuaTempAnim",
-            "AngryChihuahuaTempAnim",
-            "AngryChihuahuaTempAnim",
-            "AngryChihuahuaTempAnim",
-            "AngryChihuahuaTempAnim",
-            "AngryChihuahuaTempAnim",
-            "AngryChihuahuaTempAnim",
-            "AngryChihuahuaTempAnim",
-            "AngryChihuahuaTempAnim",
-            "AngryChihuahuaTempAnim"
+            "RageJellyDefault",
+            "RageJellyDefault",
+            "RageJellyDefault",
+            "RageJellyDefault",
+            "RageJellyDefault",
+            "RageJellyDefault",
+            "RageJellyDefault",
+            "RageJellyDefault",
+            "RageJellyDefault",
+            "RageJellyDefault"
         ],
         "AreaDamageIgnoresWalls": [],
         "AttackCount": [],
         "AttackEffect": [
-            "Laser Owl Attack",
-            "Laser Owl Attack",
-            "Laser Owl Attack",
-            "Laser Owl Attack",
-            "Laser Owl Attack",
-            "Laser Owl Attack",
-            "Laser Owl Attack",
-            "Laser Owl Attack",
-            "Laser Owl Attack",
-            "Laser Owl Attack"
+            "RageJelly Attack",
+            "RageJelly Attack",
+            "RageJelly Attack",
+            "RageJelly Attack",
+            "RageJelly Attack",
+            "RageJelly Attack",
+            "RageJelly Attack",
+            "RageJelly Attack",
+            "RageJelly Attack",
+            "RageJelly Attack"
         ],
         "AttackEffect2": [],
         "AttackEffectLv2": [],
         "AttackEffectLv3": [],
         "AttackEffectLv4": [],
         "AttackMultipleBuildings": [],
         "AttackRange": [
-            600,
-            600,
-            600,
-            600,
-            600,
-            600,
-            600,
-            600,
-            600,
-            600
+            500,
+            500,
+            500,
+            500,
+            500,
+            500,
+            500,
+            500,
+            500,
+            500
         ],
         "AttackSpeed": [
-            900,
-            900,
-            900,
-            900,
-            900,
-            900,
-            900,
-            900,
-            900,
-            900
+            750,
+            750,
+            750,
+            750,
+            750,
+            750,
+            750,
+            750,
+            750,
+            750
         ],
         "AuraSpell": [],
         "AuraSpellLevel": [],
         "AutoMergeDistance": [],
         "AutoMergeGroupSize": [],
         "BarrackLevel": [],
         "BecomesTargetableEffect": [],
         "BigPicture": [
-            "unit_pet_lassi_big",
-            "unit_pet_lassi_big",
-            "unit_pet_lassi_big",
-            "unit_pet_lassi_big",
-            "unit_pet_lassi_big",
-            "unit_pet_lassi_big",
-            "unit_pet_lassi_big",
-            "unit_pet_lassi_big",
-            "unit_pet_lassi_big",
-            "unit_pet_lassi_big"
+            "unit_pet_rage_jelly_big",
+            "unit_pet_rage_jelly_big",
+            "unit_pet_rage_jelly_big",
+            "unit_pet_rage_jelly_big",
+            "unit_pet_rage_jelly_big",
+            "unit_pet_rage_jelly_big",
+            "unit_pet_rage_jelly_big",
+            "unit_pet_rage_jelly_big",
+            "unit_pet_rage_jelly_big",
+            "unit_pet_rage_jelly_big"
         ],
         "BigPictureSWF": [
-            "sc/info_pet_lassi.sc",
-            "sc/info_pet_lassi.sc",
-            "sc/info_pet_lassi.sc",
-            "sc/info_pet_lassi.sc",
-            "sc/info_pet_lassi.sc",
-            "sc/info_pet_lassi.sc",
-            "sc/info_pet_lassi.sc",
-            "sc/info_pet_lassi.sc",
-            "sc/info_pet_lassi.sc",
-            "sc/info_pet_lassi.sc"
+            "sc/info_pet_rage_jelly.sc",
+            "sc/info_pet_rage_jelly.sc",
+            "sc/info_pet_rage_jelly.sc",
+            "sc/info_pet_rage_jelly.sc",
+            "sc/info_pet_rage_jelly.sc",
+            "sc/info_pet_rage_jelly.sc",
+            "sc/info_pet_rage_jelly.sc",
+            "sc/info_pet_rage_jelly.sc",
+            "sc/info_pet_rage_jelly.sc",
+            "sc/info_pet_rage_jelly.sc"
         ],
         "BoostAttackSpeed": [],
         "BoostDmgPerfect": [],
         "BoostRadius": [],
         "BoostedIfAlone": [],
         "BunkerDegenerationTime": [],
         "BunkerSpawnDist": [],
@@ -395,78 +395,78 @@
         "ChainShootingDistance": [],
         "ChildTroop0_X": [],
         "ChildTroop0_Y": [],
         "ChildTroop1_X": [],
         "CoolDownOverride": [],
         "CustomDefenderIcon": [],
         "DPS": [
-            260,
-            270,
-            280,
-            290,
-            300,
-            310,
-            320,
-            330,
-            340,
-            350
+            112,
+            121,
+            130,
+            139,
+            148,
+            157,
+            166,
+            175,
+            184,
+            193
         ],
         "DPSLv2": [],
         "DPSLv3": [],
         "Damage2": [],
         "Damage2Delay": [],
         "Damage2FalloffEnd": [],
         "Damage2FalloffStart": [],
         "Damage2Min": [],
         "Damage2Radius": [],
         "DamageMultiplierPercent": [],
         "DamageMultiplierTarget": [],
         "DamageRadius": [],
         "DamageReductionToStorages": [],
-        "DefaultSkin": [],
+        "DefaultSkin": [
+            "RageJellyDefault",
+            "RageJellyDefault",
+            "RageJellyDefault",
+            "RageJellyDefault",
+            "RageJellyDefault",
+            "RageJellyDefault",
+            "RageJellyDefault",
+            "RageJellyDefault",
+            "RageJellyDefault",
+            "RageJellyDefault"
+        ],
         "DefensiveTroop": [],
         "DeployEffect": [
-            "Laser Owl Deploy",
-            "Laser Owl Deploy",
-            "Laser Owl Deploy",
-            "Laser Owl Deploy",
-            "Laser Owl Deploy",
-            "Laser Owl Deploy",
-            "Laser Owl Deploy",
-            "Laser Owl Deploy",
-            "Laser Owl Deploy",
-            "Laser Owl Deploy"
-        ],
-        "Deprecated": [
-            true,
-            true,
-            true,
-            true,
-            true,
-            true,
-            true,
-            true,
-            true,
-            true
+            "RageJelly Deploy",
+            "RageJelly Deploy",
+            "RageJelly Deploy",
+            "RageJelly Deploy",
+            "RageJelly Deploy",
+            "RageJelly Deploy",
+            "RageJelly Deploy",
+            "RageJelly Deploy",
+            "RageJelly Deploy",
+            "RageJelly Deploy"
         ],
+        "Deprecated": [],
         "DieDamage": [],
         "DieDamageDelay": [],
         "DieDamageEffect": [],
         "DieDamageRadius": [],
         "DieEffect": [
-            "Barky Die",
-            "Barky Die",
-            "Barky Die",
-            "Barky Die",
-            "Barky Die",
-            "Barky Die",
-            "Barky Die",
-            "Barky Die",
-            "Barky Die",
-            "Barky Die"
+            "RageJelly Die",
+            "RageJelly Die",
+            "RageJelly Die",
+            "RageJelly Die",
+            "RageJelly Die",
+            "RageJelly Die",
+            "RageJelly Die",
+            "RageJelly Die",
+            "RageJelly Die",
+            "RageJelly Die"
         ],
         "DieEffect2": [],
         "DisableDonate": [],
         "DisableProduction": [
             true,
             true,
             true,
@@ -541,61 +541,61 @@
         "HealthReductionPerSecond": [],
         "HeroDamageMultiplier": [],
         "HeroDeathAbilityLevel": [],
         "HeroDeathAbilitySpell": [],
         "HeroDeathAbilityType": [],
         "HideEffect": [],
         "HitEffect": [
-            "Mega Tesla Hit",
-            "Mega Tesla Hit",
-            "Mega Tesla Hit",
-            "Mega Tesla Hit",
-            "Mega Tesla Hit",
-            "Mega Tesla Hit",
-            "Mega Tesla Hit",
-            "Mega Tesla Hit",
-            "Mega Tesla Hit",
-            "Mega Tesla Hit"
+            "RageJelly Hit",
+            "RageJelly Hit",
+            "RageJelly Hit",
+            "RageJelly Hit",
+            "RageJelly Hit",
+            "RageJelly Hit",
+            "RageJelly Hit",
+            "RageJelly Hit",
+            "RageJelly Hit",
+            "RageJelly Hit"
         ],
         "HitEffect2": [],
         "Hitpoints": [
-            5200,
-            5300,
-            5400,
-            5500,
-            5600,
-            5700,
-            5800,
-            5900,
-            6000,
-            6100
+            1450,
+            1525,
+            1600,
+            1675,
+            1750,
+            1825,
+            1900,
+            1975,
+            2050,
+            2125
         ],
         "HousingSpace": [
             20,
             20,
             20,
             20,
             20,
             20,
             20,
             20,
             20,
             20
         ],
         "IconExportName": [
-            "icon_unit_pet_demonpup",
-            "icon_unit_pet_demonpup",
-            "icon_unit_pet_demonpup",
-            "icon_unit_pet_demonpup",
-            "icon_unit_pet_demonpup",
-            "icon_unit_pet_demonpup",
-            "icon_unit_pet_demonpup",
-            "icon_unit_pet_demonpup",
-            "icon_unit_pet_demonpup",
-            "icon_unit_pet_demonpup"
+            "icon_unit_pet_rage_jelly",
+            "icon_unit_pet_rage_jelly",
+            "icon_unit_pet_rage_jelly",
+            "icon_unit_pet_rage_jelly",
+            "icon_unit_pet_rage_jelly",
+            "icon_unit_pet_rage_jelly",
+            "icon_unit_pet_rage_jelly",
+            "icon_unit_pet_rage_jelly",
+            "icon_unit_pet_rage_jelly",
+            "icon_unit_pet_rage_jelly"
         ],
         "IconSWF": [
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
@@ -604,50 +604,50 @@
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc"
         ],
         "ImmuneToHealing": [],
         "IncreasingDamage": [],
         "InfoTID": [
-            "TID_PET_MELEEJUMPER_INFO",
-            "TID_PET_MELEEJUMPER_INFO",
-            "TID_PET_MELEEJUMPER_INFO",
-            "TID_PET_MELEEJUMPER_INFO",
-            "TID_PET_MELEEJUMPER_INFO",
-            "TID_PET_MELEEJUMPER_INFO",
-            "TID_PET_MELEEJUMPER_INFO",
-            "TID_PET_MELEEJUMPER_INFO",
-            "TID_PET_MELEEJUMPER_INFO",
-            "TID_PET_MELEEJUMPER_INFO"
+            "TID_PET_ANGRY_JELLY_INFO",
+            "TID_PET_ANGRY_JELLY_INFO",
+            "TID_PET_ANGRY_JELLY_INFO",
+            "TID_PET_ANGRY_JELLY_INFO",
+            "TID_PET_ANGRY_JELLY_INFO",
+            "TID_PET_ANGRY_JELLY_INFO",
+            "TID_PET_ANGRY_JELLY_INFO",
+            "TID_PET_ANGRY_JELLY_INFO",
+            "TID_PET_ANGRY_JELLY_INFO",
+            "TID_PET_ANGRY_JELLY_INFO"
         ],
         "InvisibilityRadius": [],
         "IsFlying": [
-            false,
-            false,
-            false,
-            false,
-            false,
-            false,
-            false,
-            false,
-            false,
-            false
-        ],
-        "IsJumper": [
             true,
             true,
             true,
             true,
             true,
             true,
             true,
             true,
             true,
             true
         ],
+        "IsJumper": [
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false,
+            false
+        ],
         "IsSecondaryTroop": [],
         "IsUnderground": [],
         "LaboratoryLevel": [
             10,
             10,
             10,
             10,
@@ -655,24 +655,24 @@
             10,
             10,
             10,
             10,
             10
         ],
         "LeashLength": [
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0
+            400,
+            400,
+            400,
+            400,
+            400,
+            400,
+            400,
+            400,
+            400,
+            400
         ],
         "LoseHpInterval": [],
         "LoseHpPerTick": [],
         "Lv2SwitchTime": [],
         "Lv3SwitchTime": [],
         "MoveStartsEffect": [],
         "MovementOffsetAmount": [],
@@ -692,26 +692,15 @@
         "NewTargetAttackDelay": [],
         "PenetratingExtraRange": [],
         "PenetratingProjectile": [],
         "PenetratingRadius": [],
         "PickNewTargetAfterPushback": [],
         "PreAttackEffect": [],
         "PreferHeroes": [],
-        "PreferMasterTarget": [
-            true,
-            true,
-            true,
-            true,
-            true,
-            true,
-            true,
-            true,
-            true,
-            true
-        ],
+        "PreferMasterTarget": [],
         "PreferedTargetBuilding": [],
         "PreferedTargetBuildingClass": [
             "Defense",
             "Defense",
             "Defense",
             "Defense",
             "Defense",
@@ -720,15 +709,26 @@
             "Defense",
             "Defense",
             "Defense"
         ],
         "PreferedTargetDamageMod": [],
         "PreferredMovementTarget": [],
         "PreferredTargetNoTargeting": [],
-        "PreviewScenario": [],
+        "PreviewScenario": [
+            "Pet1",
+            "Pet1",
+            "Pet1",
+            "Pet1",
+            "Pet1",
+            "Pet1",
+            "Pet1",
+            "Pet1",
+            "Pet1",
+            "Pet1"
+        ],
         "ProductionBuilding": [],
         "Projectile": [],
         "ProjectileBounces": [],
         "PushbackSpeed": [],
         "RandomizeSecSpawnDist": [],
         "RecallWithMaster": [],
         "ReflectsDamage": [],
@@ -749,124 +749,124 @@
             100,
             100,
             100,
             100
         ],
         "SpawnOnAttack": [],
         "SpecialAbilities": [
-            "AngryChihuahuaAnger",
-            "AngryChihuahuaAnger",
-            "AngryChihuahuaAnger",
-            "AngryChihuahuaAnger",
-            "AngryChihuahuaAnger",
-            "AngryChihuahuaAnger",
-            "AngryChihuahuaAnger",
-            "AngryChihuahuaAnger",
-            "AngryChihuahuaAnger",
-            "AngryChihuahuaAnger"
+            "AngryJellyAbility",
+            "AngryJellyAbility",
+            "AngryJellyAbility",
+            "AngryJellyAbility",
+            "AngryJellyAbility",
+            "AngryJellyAbility",
+            "AngryJellyAbility",
+            "AngryJellyAbility",
+            "AngryJellyAbility",
+            "AngryJellyAbility"
         ],
         "SpecialAbilitiesLevel": [
             1,
             1,
             1,
             1,
-            1,
-            1,
-            1,
-            1,
-            1,
-            1
+            2,
+            2,
+            2,
+            2,
+            2,
+            3
         ],
         "SpecialAbilityAttribute": [],
         "SpecialAbilityAttribute2": [],
         "SpecialAbilityAttribute3": [],
         "SpecialAbilityEffect": [],
         "SpecialAbilityIcon": [],
         "SpecialAbilityInfo": [
-            "TID_PET_ABILITY_INFO_BARKY",
-            "TID_PET_ABILITY_INFO_BARKY",
-            "TID_PET_ABILITY_INFO_BARKY",
-            "TID_PET_ABILITY_INFO_BARKY",
-            "TID_PET_ABILITY_INFO_BARKY",
-            "TID_PET_ABILITY_INFO_BARKY",
-            "TID_PET_ABILITY_INFO_BARKY",
-            "TID_PET_ABILITY_INFO_BARKY",
-            "TID_PET_ABILITY_INFO_BARKY",
-            "TID_PET_ABILITY_INFO_BARKY"
+            "TID_PET_ABILITY_INFO_ANGRY_JELLY",
+            "TID_PET_ABILITY_INFO_ANGRY_JELLY",
+            "TID_PET_ABILITY_INFO_ANGRY_JELLY",
+            "TID_PET_ABILITY_INFO_ANGRY_JELLY",
+            "TID_PET_ABILITY_INFO_ANGRY_JELLY",
+            "TID_PET_ABILITY_INFO_ANGRY_JELLY",
+            "TID_PET_ABILITY_INFO_ANGRY_JELLY",
+            "TID_PET_ABILITY_INFO_ANGRY_JELLY",
+            "TID_PET_ABILITY_INFO_ANGRY_JELLY",
+            "TID_PET_ABILITY_INFO_ANGRY_JELLY"
         ],
         "SpecialAbilityLevel": [],
         "SpecialAbilityName": [
-            "TID_PET_ABILITY_BARKY",
-            "TID_PET_ABILITY_BARKY",
-            "TID_PET_ABILITY_BARKY",
-            "TID_PET_ABILITY_BARKY",
-            "TID_PET_ABILITY_BARKY",
-            "TID_PET_ABILITY_BARKY",
-            "TID_PET_ABILITY_BARKY",
-            "TID_PET_ABILITY_BARKY",
-            "TID_PET_ABILITY_BARKY",
-            "TID_PET_ABILITY_BARKY"
+            "TID_PET_ABILITY_ANGRY_JELLY",
+            "TID_PET_ABILITY_ANGRY_JELLY",
+            "TID_PET_ABILITY_ANGRY_JELLY",
+            "TID_PET_ABILITY_ANGRY_JELLY",
+            "TID_PET_ABILITY_ANGRY_JELLY",
+            "TID_PET_ABILITY_ANGRY_JELLY",
+            "TID_PET_ABILITY_ANGRY_JELLY",
+            "TID_PET_ABILITY_ANGRY_JELLY",
+            "TID_PET_ABILITY_ANGRY_JELLY",
+            "TID_PET_ABILITY_ANGRY_JELLY"
         ],
         "SpecialAbilitySpell": [],
         "SpecialAbilityType": [],
         "SpecialMovementMod": [],
         "Speed": [
-            300,
-            300,
-            300,
-            300,
-            300,
-            300,
-            300,
-            300,
-            300,
-            300
+            200,
+            200,
+            200,
+            200,
+            200,
+            200,
+            200,
+            200,
+            200,
+            200
         ],
         "SpeedDecreasePerChildTroopLost": [],
         "StrengthWeight": [
-            1960,
-            1960,
-            1960,
-            1960,
-            1960,
-            1960,
-            1960,
-            1960,
-            1960,
-            1960
+            15000,
+            16000,
+            17000,
+            18000,
+            19000,
+            20000,
+            21000,
+            22000,
+            23000,
+            24000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "SummonsInheritMaster": [],
         "TID": [
-            "TID_PET_MELEEJUMPER",
-            "TID_PET_MELEEJUMPER",
-            "TID_PET_MELEEJUMPER",
-            "TID_PET_MELEEJUMPER",
-            "TID_PET_MELEEJUMPER",
-            "TID_PET_MELEEJUMPER",
-            "TID_PET_MELEEJUMPER",
-            "TID_PET_MELEEJUMPER",
-            "TID_PET_MELEEJUMPER",
-            "TID_PET_MELEEJUMPER"
+            "TID_PET_ANGRY_JELLY",
+            "TID_PET_ANGRY_JELLY",
+            "TID_PET_ANGRY_JELLY",
+            "TID_PET_ANGRY_JELLY",
+            "TID_PET_ANGRY_JELLY",
+            "TID_PET_ANGRY_JELLY",
+            "TID_PET_ANGRY_JELLY",
+            "TID_PET_ANGRY_JELLY",
+            "TID_PET_ANGRY_JELLY",
+            "TID_PET_ANGRY_JELLY"
         ],
         "TargetedEffectOffset": [
-            "-50",
-            "-50",
-            "-50",
-            "-50",
-            "-50",
-            "-50",
-            "-50",
-            "-50",
-            "-50",
-            "-50"
+            60,
+            60,
+            60,
+            60,
+            60,
+            60,
+            60,
+            60,
+            60,
+            60
         ],
         "TombStone": [],
         "TrainingCost": [
             1,
             2,
             3,
             4,
@@ -956,19 +956,19 @@
             "DarkElixir",
             "DarkElixir"
         ],
         "UpgradeTimeH": [
             72,
             96,
             120,
-            132,
             144,
-            156,
             168,
-            180,
+            192,
+            192,
+            192,
             192,
             192
         ],
         "UpgradeTimeM": [],
         "VillageType": [],
         "WallMovementCost": []
     },
@@ -1643,29 +1643,29 @@
             400,
             400,
             400,
             400
         ],
         "SpeedDecreasePerChildTroopLost": [],
         "StrengthWeight": [
-            1960,
-            2020,
-            2080,
-            2140,
-            2200,
-            2260,
-            2320,
-            2380,
-            2440,
-            2500,
-            2520,
-            2540,
-            2560,
-            2580,
-            2600
+            10000,
+            11000,
+            12000,
+            13000,
+            14000,
+            15000,
+            16000,
+            17000,
+            18000,
+            19000,
+            19500,
+            20000,
+            20500,
+            21000,
+            21500
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "SummonsInheritMaster": [],
@@ -2618,29 +2618,29 @@
             300,
             300,
             300,
             300
         ],
         "SpeedDecreasePerChildTroopLost": [],
         "StrengthWeight": [
-            1750,
-            1780,
-            1810,
-            1840,
-            1870,
-            1900,
-            1930,
-            1960,
-            1990,
-            2020,
-            2040,
-            2060,
-            2080,
-            2100,
-            2120
+            10000,
+            11000,
+            12000,
+            13000,
+            14000,
+            15000,
+            16000,
+            17000,
+            18000,
+            19000,
+            20000,
+            21000,
+            22000,
+            23000,
+            24000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "SummonsInheritMaster": [],
@@ -3452,24 +3452,24 @@
             400,
             400,
             400,
             400
         ],
         "SpeedDecreasePerChildTroopLost": [],
         "StrengthWeight": [
-            2135,
-            2170,
-            2205,
-            2240,
-            2275,
-            2310,
-            2345,
-            2380,
-            2415,
-            2450
+            15000,
+            16000,
+            17000,
+            18000,
+            19000,
+            20000,
+            21000,
+            22000,
+            23000,
+            24000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "SummonsInheritMaster": [],
@@ -4367,29 +4367,29 @@
             250,
             250,
             250,
             250
         ],
         "SpeedDecreasePerChildTroopLost": [],
         "StrengthWeight": [
-            3550,
-            3600,
-            3650,
-            3700,
-            3750,
-            3800,
-            3850,
-            3900,
-            3950,
-            4000,
-            4000,
-            4000,
-            4000,
-            4000,
-            4000
+            10000,
+            11000,
+            12000,
+            13000,
+            14000,
+            15000,
+            16000,
+            17000,
+            18000,
+            19000,
+            20000,
+            21000,
+            22000,
+            23000,
+            24000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "SummonsInheritMaster": [],
@@ -5130,24 +5130,24 @@
             300,
             300,
             300,
             300
         ],
         "SpeedDecreasePerChildTroopLost": [],
         "StrengthWeight": [
-            3270,
-            3300,
-            3330,
-            3360,
-            3390,
-            3420,
-            3440,
-            3470,
-            3500,
-            3530
+            15000,
+            16000,
+            17000,
+            18000,
+            19000,
+            20000,
+            21000,
+            22000,
+            23000,
+            24000
         ],
         "SummonCooldown": [
             8000,
             8000,
             8000,
             8000,
             8000,
@@ -6160,24 +6160,24 @@
             300,
             300,
             300,
             300
         ],
         "SpeedDecreasePerChildTroopLost": [],
         "StrengthWeight": [
-            3525,
-            3550,
-            3575,
-            3600,
-            3625,
-            3650,
-            3675,
-            3700,
-            3725,
-            3750
+            15000,
+            16000,
+            17000,
+            18000,
+            19000,
+            20000,
+            21000,
+            22000,
+            23000,
+            24000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "SummonsInheritMaster": [],
@@ -6912,24 +6912,24 @@
             200,
             200,
             200,
             200
         ],
         "SpeedDecreasePerChildTroopLost": [],
         "StrengthWeight": [
-            1830,
-            1840,
-            1850,
-            1860,
-            1870,
-            1880,
-            1890,
-            1900,
-            1910,
-            1920
+            15000,
+            16000,
+            17000,
+            18000,
+            19000,
+            20000,
+            21000,
+            22000,
+            23000,
+            24000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "SummonsInheritMaster": [
@@ -8438,24 +8438,24 @@
             450,
             450,
             450,
             450
         ],
         "SpeedDecreasePerChildTroopLost": [],
         "StrengthWeight": [
-            4050,
-            4100,
-            4150,
-            4200,
-            4250,
-            4300,
-            4350,
-            4400,
-            4450,
-            4500
+            15000,
+            16000,
+            17000,
+            18000,
+            19000,
+            20000,
+            21000,
+            22000,
+            23000,
+            24000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "SummonsInheritMaster": [],
@@ -9096,17 +9096,15 @@
         ],
         "SpecialAbilityType": [],
         "SpecialMovementMod": [],
         "Speed": [
             250
         ],
         "SpeedDecreasePerChildTroopLost": [],
-        "StrengthWeight": [
-            4550
-        ],
+        "StrengthWeight": [],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "SummonsInheritMaster": [],
         "TID": [
@@ -9967,24 +9965,24 @@
             200,
             200,
             200,
             200
         ],
         "SpeedDecreasePerChildTroopLost": [],
         "StrengthWeight": [
-            4550,
-            4600,
-            4650,
-            4700,
-            4750,
-            4800,
-            4850,
-            4900,
-            4950,
-            5000
+            10000,
+            11000,
+            12000,
+            13000,
+            14000,
+            15000,
+            16000,
+            17000,
+            18000,
+            19000
         ],
         "SummonCooldown": [],
         "SummonEffect": [],
         "SummonLimit": [],
         "SummonTroop": [],
         "SummonTroopCount": [],
         "SummonsInheritMaster": [],
@@ -10085,15 +10083,15 @@
             200000,
             210000,
             220000,
             230000,
             240000,
             250000,
             260000,
-            270000
+            260000
         ],
         "UpgradeLevelByTH": [],
         "UpgradeResource": [
             "DarkElixir",
             "DarkElixir",
             "DarkElixir",
             "DarkElixir",
@@ -10110,14 +10108,14 @@
             108,
             120,
             132,
             144,
             156,
             168,
             180,
-            192
+            180
         ],
         "UpgradeTimeM": [],
         "VillageType": [],
         "WallMovementCost": []
     }
 }
```

### Comparing `coc.py-3.4.1/coc/static/spells.json` & `coc_py-3.4.2/coc/static/spells.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9519926027594438%*

 * *Differences: {"'Apprentice Growth'": "{'ExtraHealthPermil': {insert: [(0, 200), (1, 220)], delete: [3, 2]}, "*

 * *                        "'ImmortalTime': [], 'GiveSpecialAbility': [], 'GivenSpecialAbilityLevel': "*

 * *                        "[], 'Targeted': [], 'TargetedProjectile': [], 'TargetedAgainEffect': []}",*

 * * "'AreaStun'": "{'ImmortalTime': [], 'GiveSpecialAbility': [], 'GivenSpecialAbilityLevel': [], "*

 * *               "'Targeted': [], 'TargetedProjectile': [], 'TargetedAgainEffect': []}",*

 * * "'Artillery Center'": "{'Immo […]*

```diff
@@ -60,34 +60,37 @@
             "Enemy Apprentice growth aura",
             "Enemy Apprentice growth aura"
         ],
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [
+            200,
+            220,
             240,
-            260,
-            280,
-            300
+            260
         ],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             300,
             300,
             300,
             300
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -165,14 +168,17 @@
         "TID": [],
         "TargetInfoString": [
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             300,
             300,
             300,
             300
         ],
         "TombStone": [],
@@ -238,21 +244,24 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [
             true
         ],
         "ImmunitySiegeMachines": [
             true
         ],
@@ -315,14 +324,17 @@
         "StrengthWeight": [],
         "StunTimeMS": [
             5000
         ],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
         "TornadoForce3": [],
         "TornadoForce4": [],
         "TornadoForce5": [],
@@ -395,14 +407,16 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [
             "Artillery Hit",
             "Artillery Hit",
             "Artillery Hit",
             "Artillery Hit",
@@ -410,14 +424,15 @@
             "Artillery Hit",
             "Artillery Hit"
         ],
         "HitTimeMS": [],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -505,14 +520,17 @@
         "SpeedBoost2": [],
         "SpellForgeLevel": [],
         "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             150,
             150,
             150,
             150,
             150,
             150,
@@ -619,27 +637,30 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             0,
             0,
             0,
             0,
             0
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -735,14 +756,17 @@
         ],
         "SpellForgeLevel": [],
         "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             0,
             0,
             0,
             0,
             0
         ],
@@ -943,14 +967,16 @@
             2500,
             2700,
             2900,
             3100,
             3300,
             3500
         ],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             300,
             300,
             300,
@@ -998,14 +1024,15 @@
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc"
         ],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [
@@ -1216,27 +1243,15 @@
             1,
             1,
             1,
             1,
             1,
             1
         ],
-        "StrengthWeight": [
-            460,
-            460,
-            460,
-            460,
-            460,
-            460,
-            460,
-            460,
-            460,
-            460,
-            460
-        ],
+        "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [
             "BouncingFrostmite",
             "BouncingFrostmite",
             "BouncingFrostmite",
             "BouncingFrostmite",
             "BouncingFrostmite",
@@ -1269,14 +1284,17 @@
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             300,
             300,
             300,
             300,
             300,
             300,
@@ -1405,14 +1423,16 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             0,
             0,
             0,
@@ -1424,14 +1444,15 @@
             0,
             0,
             0
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -1563,14 +1584,17 @@
             "FrostmiteSpawner",
             "FrostmiteSpawner",
             "FrostmiteSpawner",
             "FrostmiteSpawner"
         ],
         "TID": [],
         "TargetInfoString": [],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
         "TornadoForce3": [],
         "TornadoForce4": [],
         "TornadoForce5": [],
@@ -1649,23 +1673,26 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             300
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [
@@ -1723,23 +1750,24 @@
         "SpeedBoost": [
             0
         ],
         "SpeedBoost2": [
             0
         ],
         "SpellForgeLevel": [],
-        "StrengthWeight": [
-            0
-        ],
+        "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [
             "TID_RAM_RIDER_ABILITY_TITLE"
         ],
         "TargetInfoString": [],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             100
         ],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
         "TornadoForce3": [],
@@ -1806,23 +1834,26 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             0
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -1877,14 +1908,17 @@
         ],
         "SpellForgeLevel": [],
         "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             0
         ],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
         "TornadoForce3": [],
@@ -1963,14 +1997,16 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [
             "Birthday Spell Hit"
         ],
         "HitTimeMS": [
             1750
@@ -1980,14 +2016,15 @@
         ],
         "IconExportName": [
             "icon_spell_birthday"
         ],
         "IconSWF": [
             "sc/ui.sc"
         ],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [
@@ -2059,25 +2096,26 @@
         "SpeedBoost": [],
         "SpeedBoost2": [
             0
         ],
         "SpellForgeLevel": [
             1
         ],
-        "StrengthWeight": [
-            0
-        ],
+        "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [
             "TID_BIRTHDAY_SPELL"
         ],
         "TargetInfoString": [
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             0
         ],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
         "TornadoForce3": [],
@@ -2162,14 +2200,16 @@
         ],
         "FreezePercent": [
             70
         ],
         "FreezeTimeMS": [
             500
         ],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             400
         ],
         "HousingSpace": [
@@ -2177,14 +2217,15 @@
         ],
         "IconExportName": [
             "icon_spell_cc_frost"
         ],
         "IconSWF": [
             "sc/ui.sc"
         ],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [
             true
         ],
         "ImmunityTH_CC": [],
@@ -2252,25 +2293,26 @@
         "SpawnObstacle": [],
         "SpawnUpgradeLevel": [],
         "SpeedBoost": [],
         "SpeedBoost2": [],
         "SpellForgeLevel": [
             5
         ],
-        "StrengthWeight": [
-            1000
-        ],
+        "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [
             "TID_SPELL_FROST"
         ],
         "TargetInfoString": [
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             300
         ],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
         "TornadoForce3": [],
@@ -2355,27 +2397,30 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             300,
             300
         ],
         "HousingSpace": [
             2,
             2
         ],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -2442,28 +2487,28 @@
         "SpawnUpgradeLevel": [],
         "SpeedBoost": [],
         "SpeedBoost2": [],
         "SpellForgeLevel": [
             1,
             1
         ],
-        "StrengthWeight": [
-            0,
-            0
-        ],
+        "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [
             "TID_BOOSTDEFENCES_SPELL",
             "TID_BOOSTDEFENCES_SPELL"
         ],
         "TargetInfoString": [
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             300,
             300
         ],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
@@ -2541,25 +2586,28 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [
             25
         ],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             400
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [
             true
@@ -2611,23 +2659,24 @@
         "SpawnDuration": [],
         "SpawnFirstGroupSize": [],
         "SpawnObstacle": [],
         "SpawnUpgradeLevel": [],
         "SpeedBoost": [],
         "SpeedBoost2": [],
         "SpellForgeLevel": [],
-        "StrengthWeight": [
-            0
-        ],
+        "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             400
         ],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
         "TornadoForce3": [],
@@ -2704,21 +2753,24 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -2802,14 +2854,17 @@
         "SpeedBoost2": [],
         "SpellForgeLevel": [],
         "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
         "TornadoForce3": [],
         "TornadoForce4": [],
         "TornadoForce5": [],
@@ -2881,21 +2936,24 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [
             true
         ],
         "ImmunitySiegeMachines": [
             true
         ],
@@ -2958,14 +3016,17 @@
         "StrengthWeight": [],
         "StunTimeMS": [
             2000
         ],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
         "TornadoForce3": [],
         "TornadoForce4": [],
         "TornadoForce5": [],
@@ -3047,14 +3108,16 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [
             "Skeleton Dropship Bomb Hit",
             "Skeleton Dropship Bomb Hit",
             "Skeleton Dropship Bomb Hit",
             "Skeleton Dropship Bomb Hit"
@@ -3064,14 +3127,15 @@
             0,
             0,
             0
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -3159,14 +3223,17 @@
         "TID": [],
         "TargetInfoString": [
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             100,
             100,
             100,
             100
         ],
         "TombStone": [],
@@ -3310,14 +3377,16 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             400,
             400,
             400,
@@ -3353,14 +3422,15 @@
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc"
         ],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [
@@ -3503,22 +3573,22 @@
             5,
             5,
             5,
             5,
             5
         ],
         "StrengthWeight": [
-            300,
-            330,
-            360,
-            360,
-            360,
-            330,
-            310,
-            290
+            1200,
+            1300,
+            1400,
+            1500,
+            1600,
+            1800,
+            1900,
+            2000
         ],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [
             "TID_DUPLICATE_SPELL",
             "TID_DUPLICATE_SPELL",
             "TID_DUPLICATE_SPELL",
@@ -3534,14 +3604,17 @@
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             300,
             300,
             300,
             300,
             300,
             300,
@@ -3685,14 +3758,16 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             400,
             400,
             400,
@@ -3716,14 +3791,15 @@
         "IconSWF": [
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc"
         ],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [
             true,
             true,
             true,
             true,
             true
@@ -3863,19 +3939,19 @@
             2,
             2,
             2,
             2,
             2
         ],
         "StrengthWeight": [
-            150,
-            145,
-            140,
-            135,
-            130
+            1200,
+            1300,
+            1400,
+            1500,
+            1600
         ],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [
             "TID_EARTHQUAKE",
             "TID_EARTHQUAKE",
             "TID_EARTHQUAKE",
@@ -3885,14 +3961,17 @@
         "TargetInfoString": [
             "TID_INFO_TARGET_TYPE_BUILDINGS_AND_WALLS",
             "TID_INFO_TARGET_TYPE_BUILDINGS_AND_WALLS",
             "TID_INFO_TARGET_TYPE_BUILDINGS_AND_WALLS",
             "TID_INFO_TARGET_TYPE_BUILDINGS_AND_WALLS",
             "TID_INFO_TARGET_TYPE_BUILDINGS_AND_WALLS"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             400,
             400,
             400,
             400,
             400
         ],
@@ -4035,14 +4114,16 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             400,
             400,
             400,
@@ -4050,14 +4131,15 @@
             400,
             400,
             400
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [
@@ -4161,14 +4243,17 @@
             "TID_EARTHQUAKE",
             "TID_EARTHQUAKE",
             "TID_EARTHQUAKE",
             "TID_EARTHQUAKE",
             "TID_EARTHQUAKE"
         ],
         "TargetInfoString": [],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             400,
             400,
             400,
             400,
             400,
             400,
@@ -4245,25 +4330,28 @@
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [
             100
         ],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [
             "ElectrifiedShieldHit"
         ],
         "HitTimeMS": [
             100
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -4320,14 +4408,17 @@
         "SpeedBoost2": [],
         "SpellForgeLevel": [],
         "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             400
         ],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
         "TornadoForce3": [],
@@ -4452,14 +4543,16 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [
             "Lightning Spell Hit",
             "Lightning Spell Hit",
             "Lightning Spell Hit",
             "Lightning Spell Hit",
@@ -4481,14 +4574,15 @@
             1100,
             1100,
             1100
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -4591,14 +4685,17 @@
         "SpeedBoost2": [],
         "SpellForgeLevel": [],
         "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             400,
             400,
             400,
             400,
             400,
             400,
@@ -4632,14 +4729,15 @@
         "UpgradeTimeH": [],
         "VillageType": []
     },
     "ElectroTitanDamageAura": {
         "AffectsSiegeMachines": [
             true,
             true,
+            true,
             true
         ],
         "AttackSpeedBoost": [],
         "BigPicture": [],
         "BoostDefenders": [],
         "BoostLinkedToPoison": [],
         "BoostTimeMS": [],
@@ -4650,90 +4748,101 @@
         "ChangeTeamTime": [],
         "ChargingEffect": [],
         "ChargingTimeMS": [],
         "ConeAngle": [],
         "Damage": [
             30,
             40,
-            50
+            50,
+            55
         ],
         "DamageBoostPercent": [],
         "DamagePermilMin": [],
         "DamageTHPercent": [],
         "DeployEffect": [
             "E_titanAreaDamage",
             "E_titanAreaDamage",
+            "E_titanAreaDamage",
             "E_titanAreaDamage"
         ],
         "DeployEffect2": [],
         "DeployEffect2Delay": [],
         "DeployTimeMS": [],
         "DestroyWalls": [],
         "DisableDonate": [],
         "DisableProduction": [
             true,
             true,
+            true,
             true
         ],
         "DonateCost": [],
         "DuplicateHousing": [],
         "DuplicateLifetime": [],
         "EnabledByCalendar": [],
         "EnemyDeployEffect": [],
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [
             25,
             25,
+            25,
             25
         ],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             400,
             400,
+            400,
             400
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [
             true,
             true,
+            true,
             true
         ],
         "InfoTID": [],
         "InvisibilityTime": [],
         "JumpBoostMS": [],
         "JumpHousingLimit": [],
         "LaboratoryLevel": [],
         "Level": [
             1,
             2,
-            3
+            3,
+            4
         ],
         "MaxUnitsHit": [],
         "MinDamage": [],
         "MinRadius": [],
         "Name": [],
         "NumObstacles": [],
         "NumTombStones": [],
         "NumberOfHits": [
             4000,
             4000,
+            4000,
             4000
         ],
         "Overgrowth": [],
         "PauseCombatComponentsMs": [],
         "PoisonAffectAir": [],
         "PoisonDPS": [],
         "PoisonIncreaseSlowly": [],
@@ -4742,27 +4851,30 @@
         "PreferredTarget": [],
         "PreferredTargetDamageMod": [],
         "PreviewScenario": [],
         "ProductionBuilding": [],
         "Radius": [
             350,
             350,
+            350,
             350
         ],
         "RandomRadius": [
             0,
             0,
+            0,
             0
         ],
         "RandomRadiusAffectsOnlyGfx": [],
         "RecallHousing": [],
         "ScaleByTH": [],
         "ScaleDeployEffects": [
             true,
             true,
+            true,
             true
         ],
         "ShieldProjectileDamageMod": [],
         "ShieldProjectileSpeed": [],
         "ShieldProtectionPercent": [],
         "ShieldTime": [],
         "ShrinkHitpointsRatio": [],
@@ -4774,27 +4886,33 @@
         "SpawnUpgradeLevel": [],
         "SpeedBoost": [],
         "SpeedBoost2": [],
         "SpellForgeLevel": [],
         "StrengthWeight": [
             0,
             0,
+            0,
             0
         ],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
+            "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             400,
             400,
+            400,
             400
         ],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
         "TornadoForce3": [],
         "TornadoForce4": [],
@@ -4866,23 +4984,26 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             400
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -4945,14 +5066,17 @@
         ],
         "SpellForgeLevel": [],
         "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             300
         ],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
         "TornadoForce3": [],
@@ -5029,23 +5153,26 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             500
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -5107,21 +5234,22 @@
         "SpeedBoost": [
             0
         ],
         "SpeedBoost2": [
             0
         ],
         "SpellForgeLevel": [],
-        "StrengthWeight": [
-            0
-        ],
+        "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             400
         ],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
         "TornadoForce3": [],
@@ -5196,23 +5324,26 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             500
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [
             true
@@ -5276,21 +5407,22 @@
         "SpeedBoost": [
             0
         ],
         "SpeedBoost2": [
             0
         ],
         "SpellForgeLevel": [],
-        "StrengthWeight": [
-            0
-        ],
+        "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             400
         ],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
         "TornadoForce3": [],
@@ -5403,27 +5535,30 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             500,
             500,
             500,
             500,
             500
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -5538,25 +5673,22 @@
             0,
             0,
             0,
             0,
             0
         ],
         "SpellForgeLevel": [],
-        "StrengthWeight": [
-            0,
-            0,
-            0,
-            0,
-            0
-        ],
+        "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             400,
             400,
             400,
             400,
             400
         ],
@@ -5691,14 +5823,16 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [
             "Ice Breaker Hit lvl1",
             "Ice Breaker Hit lvl1",
             "Ice Breaker Hit lvl1",
             "Ice Breaker Hit lvl1",
@@ -5722,14 +5856,15 @@
             0,
             0,
             0
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -5849,14 +5984,17 @@
         "SpeedBoost2": [],
         "SpellForgeLevel": [],
         "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             0,
             0,
             0,
             0,
             0,
             0,
@@ -5997,14 +6135,16 @@
             3000,
             3500,
             4000,
             4500,
             5000,
             5500
         ],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             400,
             400,
             400,
@@ -6036,14 +6176,15 @@
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc"
         ],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [
@@ -6175,21 +6316,21 @@
             4,
             4,
             4,
             4,
             4
         ],
         "StrengthWeight": [
-            1000,
-            1150,
+            1100,
+            1200,
             1300,
-            1450,
+            1400,
+            1500,
             1600,
-            1750,
-            1900
+            1700
         ],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [
             "TID_FREEZE_SPELL",
             "TID_FREEZE_SPELL",
             "TID_FREEZE_SPELL",
@@ -6203,14 +6344,17 @@
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             0,
             0,
             0,
             0,
             0,
             0,
@@ -6327,23 +6471,26 @@
         "FreezeOuterTimeMS": [
             4500
         ],
         "FreezePercent": [],
         "FreezeTimeMS": [
             5000
         ],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             10
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -6402,14 +6549,17 @@
         "SpeedBoost2": [],
         "SpellForgeLevel": [],
         "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             0
         ],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
         "TornadoForce3": [],
@@ -6480,23 +6630,26 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             300
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -6555,14 +6708,17 @@
         "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             1000
         ],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
         "TornadoForce3": [],
@@ -6676,14 +6832,16 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             0,
             0,
             0,
@@ -6694,14 +6852,15 @@
             0,
             0,
             0
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -6848,14 +7007,17 @@
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             300,
             300,
             300,
             300,
             300,
             300,
@@ -7006,14 +7168,16 @@
             800,
             900,
             1000
         ],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             300,
             300,
             300,
@@ -7021,14 +7185,15 @@
             300,
             300,
             300
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -7132,14 +7297,17 @@
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             300,
             300,
             300,
             300,
             300,
             300,
@@ -7260,14 +7428,16 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             400,
             400,
             400,
@@ -7295,14 +7465,15 @@
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc"
         ],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [
@@ -7437,20 +7608,20 @@
             3,
             3,
             3,
             3,
             3
         ],
         "StrengthWeight": [
-            100,
-            95,
-            90,
-            85,
-            80,
-            95
+            900,
+            1000,
+            1100,
+            1200,
+            1300,
+            1700
         ],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [
             "TID_HASTE",
             "TID_HASTE",
             "TID_HASTE",
@@ -7462,14 +7633,17 @@
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             300,
             300,
             300,
             300,
             300,
             300
@@ -7617,14 +7791,16 @@
         ],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [
             "Heal spell",
             "Heal spell",
             "Heal spell",
             "Heal spell",
@@ -7640,14 +7816,15 @@
             300,
             300,
             300
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -7743,14 +7920,17 @@
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             300,
             300,
             300,
             300,
             300,
             300,
@@ -7892,14 +8072,16 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [
             55,
             55,
             55,
             55,
             55,
             55,
@@ -7965,14 +8147,15 @@
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc"
         ],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [
@@ -8137,24 +8320,24 @@
             2,
             2,
             2,
             2,
             2
         ],
         "StrengthWeight": [
-            230,
-            215,
-            200,
-            190,
-            180,
-            170,
-            170,
-            200,
-            200,
-            200
+            900,
+            1000,
+            1100,
+            1200,
+            1300,
+            1400,
+            1500,
+            1800,
+            2000,
+            2100
         ],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [
             "TID_HEALING_WAVE",
             "TID_HEALING_WAVE",
             "TID_HEALING_WAVE",
@@ -8174,14 +8357,17 @@
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             300,
             300,
             300,
             300,
             300,
             300,
@@ -8301,25 +8487,28 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [
             25
         ],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             400
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [
             true
@@ -8371,23 +8560,24 @@
         "SpawnDuration": [],
         "SpawnFirstGroupSize": [],
         "SpawnObstacle": [],
         "SpawnUpgradeLevel": [],
         "SpeedBoost": [],
         "SpeedBoost2": [],
         "SpellForgeLevel": [],
-        "StrengthWeight": [
-            0
-        ],
+        "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             400
         ],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
         "TornadoForce3": [],
@@ -8482,14 +8672,16 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [
             "Ice Breaker Hit lvl1",
             "Ice Breaker Hit lvl1",
             "Ice Breaker Hit lvl1",
             "Ice Breaker Hit lvl1",
@@ -8501,14 +8693,15 @@
             0,
             0,
             0
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -8598,14 +8791,17 @@
         "SpeedBoost2": [],
         "SpellForgeLevel": [],
         "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             0,
             0,
             0,
             0,
             0
         ],
@@ -8638,14 +8834,15 @@
         "AffectsSiegeMachines": [
             true,
             true,
             true,
             true,
             true,
             true,
+            true,
             true
         ],
         "AttackSpeedBoost": [],
         "BigPicture": [],
         "BoostDefenders": [],
         "BoostLinkedToPoison": [],
         "BoostTimeMS": [],
@@ -8658,58 +8855,63 @@
         "ChargingTimeMS": [
             300,
             300,
             300,
             300,
             300,
             300,
+            300,
             300
         ],
         "ConeAngle": [],
         "Damage": [],
         "DamageBoostPercent": [],
         "DamagePermilMin": [],
         "DamageTHPercent": [],
         "DeployEffect": [
             "IceGolem Freeze deploy lvl1",
             "IceGolem Freeze deploy lvl2",
             "IceGolem Freeze deploy lvl3",
             "IceGolem Freeze deploy lvl4",
             "IceGolem Freeze deploy lvl5",
             "IceGolem Freeze deploy lvl6",
-            "IceGolem Freeze deploy lvl7"
+            "IceGolem Freeze deploy lvl7",
+            "IceGolem Freeze deploy lvl8"
         ],
         "DeployEffect2": [
             "IceGolem Freeze deploy2 lvl1",
             "IceGolem Freeze deploy2 lvl2",
             "IceGolem Freeze deploy2 lvl3",
             "IceGolem Freeze deploy2 lvl4",
             "IceGolem Freeze deploy2 lvl5",
             "IceGolem Freeze deploy2 lvl6",
-            "IceGolem Freeze deploy2 lvl7"
+            "IceGolem Freeze deploy2 lvl7",
+            "IceGolem Freeze deploy2 lvl8"
         ],
         "DeployEffect2Delay": [],
         "DeployTimeMS": [
             0,
             0,
             0,
             0,
             0,
             0,
+            0,
             0
         ],
         "DestroyWalls": [],
         "DisableDonate": [],
         "DisableProduction": [
             true,
             true,
             true,
             true,
             true,
             true,
+            true,
             true
         ],
         "DonateCost": [],
         "DuplicateHousing": [],
         "DuplicateLifetime": [],
         "EnabledByCalendar": [],
         "EnemyDeployEffect": [],
@@ -8720,41 +8922,47 @@
         "FreezeOuterTimeMS": [
             3000,
             3563,
             4125,
             4688,
             5250,
             5625,
-            5950
+            5950,
+            6275
         ],
         "FreezePercent": [],
         "FreezeTimeMS": [
             4000,
             4750,
             5500,
             6250,
             7000,
             7500,
-            8000
+            8000,
+            8500
         ],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             400,
             400,
             400,
             400,
             400,
             400,
+            400,
             400
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -8765,29 +8973,31 @@
         "Level": [
             1,
             2,
             3,
             4,
             5,
             6,
-            7
+            7,
+            8
         ],
         "MaxUnitsHit": [],
         "MinDamage": [],
         "MinRadius": [],
         "Name": [],
         "NumObstacles": [],
         "NumTombStones": [],
         "NumberOfHits": [
             1,
             1,
             1,
             1,
             1,
             1,
+            1,
             1
         ],
         "Overgrowth": [],
         "PauseCombatComponentsMs": [],
         "PoisonAffectAir": [],
         "PoisonDPS": [],
         "PoisonIncreaseSlowly": [],
@@ -8800,32 +9010,35 @@
         "Radius": [
             750,
             750,
             750,
             750,
             750,
             750,
+            750,
             750
         ],
         "RandomRadius": [
             0,
             0,
             0,
             0,
             0,
             0,
+            0,
             0
         ],
         "RandomRadiusAffectsOnlyGfx": [
             true,
             true,
             true,
             true,
             true,
             true,
+            true,
             true
         ],
         "RecallHousing": [],
         "ScaleByTH": [],
         "ScaleDeployEffects": [],
         "ShieldProjectileDamageMod": [],
         "ShieldProjectileSpeed": [],
@@ -8842,29 +9055,34 @@
         "SpeedBoost2": [
             0,
             0,
             0,
             0,
             0,
             0,
+            0,
             0
         ],
         "SpellForgeLevel": [],
         "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             0,
             0,
             0,
             0,
             0,
             0,
+            0,
             0
         ],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
         "TornadoForce3": [],
         "TornadoForce4": [],
@@ -8978,28 +9196,31 @@
             2000,
             2250,
             2500,
             2750,
             3000,
             3250
         ],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             400,
             400,
             400,
             400,
             400,
             400
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -9082,14 +9303,17 @@
         "SpeedBoost2": [],
         "SpellForgeLevel": [],
         "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             0,
             0,
             0,
             0,
             0,
             0
@@ -9177,24 +9401,27 @@
             3666
         ],
         "FreezePercent": [],
         "FreezeTimeMS": [
             3500,
             4250
         ],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             400,
             400
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -9257,14 +9484,17 @@
         "SpeedBoost2": [],
         "SpellForgeLevel": [],
         "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             0,
             0
         ],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
@@ -9349,14 +9579,16 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             400,
             400,
             400,
@@ -9376,14 +9608,15 @@
         ],
         "IconSWF": [
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc"
         ],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [
             true,
             true,
             true,
             true
@@ -9497,18 +9730,18 @@
         "SpellForgeLevel": [
             6,
             6,
             6,
             6
         ],
         "StrengthWeight": [
-            210,
-            215,
-            220,
-            225
+            1500,
+            1600,
+            1700,
+            1800
         ],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [
             "TID_INVISIBILITY_SPELL",
             "TID_INVISIBILITY_SPELL",
             "TID_INVISIBILITY_SPELL",
@@ -9516,14 +9749,17 @@
         ],
         "TargetInfoString": [
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             250,
             250,
             250,
             250
         ],
         "TombStone": [],
@@ -9621,14 +9857,16 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             400
         ],
         "HousingSpace": [
@@ -9636,14 +9874,15 @@
         ],
         "IconExportName": [
             "icon_spell_invisibility"
         ],
         "IconSWF": [
             "sc/ui.sc"
         ],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [
             true
         ],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
@@ -9713,25 +9952,26 @@
         ],
         "SpeedBoost2": [
             0
         ],
         "SpellForgeLevel": [
             1
         ],
-        "StrengthWeight": [
-            225
-        ],
+        "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [
             "TID_INVISIBILITY_SPELL_TOWER"
         ],
         "TargetInfoString": [
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             250
         ],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
         "TornadoForce3": [],
@@ -9834,14 +10074,16 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             400,
             400,
             400,
@@ -9865,14 +10107,15 @@
         "IconSWF": [
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc"
         ],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [
@@ -9994,19 +10237,19 @@
             4,
             4,
             4,
             4,
             4
         ],
         "StrengthWeight": [
-            250,
-            170,
-            130,
-            110,
-            90
+            1200,
+            1300,
+            1400,
+            1700,
+            1900
         ],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [
             "TID_JUMP_SPELL",
             "TID_JUMP_SPELL",
             "TID_JUMP_SPELL",
@@ -10016,14 +10259,17 @@
         "TargetInfoString": [
             "TID_INFO_TARGET_TYPE_GROUND",
             "TID_INFO_TARGET_TYPE_GROUND",
             "TID_INFO_TARGET_TYPE_GROUND",
             "TID_INFO_TARGET_TYPE_GROUND",
             "TID_INFO_TARGET_TYPE_GROUND"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             300,
             300,
             300,
             300,
             300
         ],
@@ -10154,14 +10400,16 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [
             "LavaloonAttackEffect",
             "LavaloonAttackEffect",
             "LavaloonAttackEffect",
             "LavaloonAttackEffect",
@@ -10183,14 +10431,15 @@
             0,
             0,
             0
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -10299,26 +10548,15 @@
             8,
             9,
             10
         ],
         "SpeedBoost": [],
         "SpeedBoost2": [],
         "SpellForgeLevel": [],
-        "StrengthWeight": [
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0
-        ],
+        "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [
             "Lavaloon Pup",
             "Lavaloon Pup",
             "Lavaloon Pup",
             "Lavaloon Pup",
             "Lavaloon Pup",
@@ -10326,14 +10564,17 @@
             "Lavaloon Pup",
             "Lavaloon Pup",
             "Lavaloon Pup",
             "Lavaloon Pup"
         ],
         "TID": [],
         "TargetInfoString": [],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             0,
             0,
             0,
             0,
             0,
             0,
@@ -10520,14 +10761,16 @@
             100,
             100,
             100,
             100,
             100,
             100
         ],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [
             "Lightning Spell Hit",
             "Lightning Spell Hit",
             "Lightning Spell Hit",
             "Lightning Spell Hit",
@@ -10587,14 +10830,15 @@
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc"
         ],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [
             true,
             true,
             true,
@@ -10794,25 +11038,25 @@
             1,
             1,
             1,
             1,
             1
         ],
         "StrengthWeight": [
-            30,
-            30,
-            30,
-            30,
-            30,
-            27,
-            24,
-            22,
-            20,
-            22,
-            22
+            700,
+            800,
+            900,
+            1000,
+            1300,
+            1400,
+            1500,
+            1600,
+            1700,
+            2000,
+            2100
         ],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [
             "TID_LIGHTNING_STORM",
             "TID_LIGHTNING_STORM",
             "TID_LIGHTNING_STORM",
@@ -10834,14 +11078,17 @@
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             400,
             400,
             400,
             400,
             400,
             400,
@@ -10972,23 +11219,26 @@
         ],
         "ExtraHealthPermil": [
             10
         ],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             300
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -11045,14 +11295,17 @@
         "SpeedBoost2": [],
         "SpellForgeLevel": [],
         "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             300
         ],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
         "TornadoForce3": [],
@@ -11210,14 +11463,16 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             500,
             500,
             500,
@@ -11228,14 +11483,15 @@
             500,
             500,
             500
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [
             true,
             true,
             true,
             true,
             true,
             true,
@@ -11382,14 +11638,17 @@
         "SpeedBoost2": [],
         "SpellForgeLevel": [],
         "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             400,
             400,
             400,
             400,
             400,
             400,
@@ -11492,27 +11751,30 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             0,
             0,
             0,
             0,
             0
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -11608,14 +11870,17 @@
         "TargetInfoString": [
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             64,
             64,
             64,
             64,
             64
         ],
@@ -11735,14 +12000,16 @@
         "FreezePercent": [],
         "FreezeTimeMS": [
             22000,
             24000,
             26000,
             28000
         ],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             400,
             400,
             400,
@@ -11762,14 +12029,15 @@
         ],
         "IconSWF": [
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc"
         ],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [
             true,
             true,
             true,
             true
         ],
@@ -11908,18 +12176,18 @@
         "SpellForgeLevel": [
             6,
             6,
             6,
             6
         ],
         "StrengthWeight": [
-            50,
-            50,
-            50,
-            50
+            1600,
+            1700,
+            1900,
+            2100
         ],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [
             "TID_SPELL_OVERGROWTH",
             "TID_SPELL_OVERGROWTH",
             "TID_SPELL_OVERGROWTH",
@@ -11927,14 +12195,17 @@
         ],
         "TargetInfoString": [
             "TID_INFO_TARGET_TYPE_GROUND",
             "TID_INFO_TARGET_TYPE_GROUND",
             "TID_INFO_TARGET_TYPE_GROUND",
             "TID_INFO_TARGET_TYPE_GROUND"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             0,
             0,
             0,
             0
         ],
         "TombStone": [
@@ -12029,23 +12300,26 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             400
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -12108,14 +12382,17 @@
         "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [
             "TID_INFO_TARGET_TYPE_GROUND"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             300
         ],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
         "TornadoForce3": [],
@@ -12186,23 +12463,26 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             400
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -12267,14 +12547,17 @@
         "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             300
         ],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
         "TornadoForce3": [],
@@ -12337,21 +12620,28 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [
+            6500,
+            7500,
+            8500
+        ],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -12419,14 +12709,17 @@
         "SpeedBoost2": [],
         "SpellForgeLevel": [],
         "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
         "TornadoForce3": [],
         "TornadoForce4": [],
         "TornadoForce5": [],
@@ -12593,14 +12886,16 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [
             5,
             5,
             5,
             5,
             5,
             5,
@@ -12655,14 +12950,15 @@
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc"
         ],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [
             true,
             true,
             true,
             true,
             true,
             true,
@@ -12926,24 +13222,24 @@
             1,
             1,
             1,
             1,
             1
         ],
         "StrengthWeight": [
-            "-160",
-            "-170",
-            "-190",
-            "-210",
-            "-230",
-            "-250",
-            "-270",
-            "-275",
-            "-280",
-            "-285"
+            1200,
+            1300,
+            1400,
+            1500,
+            1600,
+            1700,
+            1800,
+            1900,
+            2000,
+            2100
         ],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [
             "TID_POISON_CLOUD",
             "TID_POISON_CLOUD",
             "TID_POISON_CLOUD",
@@ -12963,14 +13259,17 @@
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             400,
             400,
             400,
             400,
             400,
             400,
@@ -13102,21 +13401,24 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [
             true,
             true,
             true
         ],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
@@ -13216,14 +13518,17 @@
         ],
         "SpellForgeLevel": [],
         "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             400,
             400,
             400
         ],
         "TombStone": [],
         "TornadoForce1": [],
@@ -13306,14 +13611,16 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [
             20
         ],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             0
@@ -13323,14 +13630,15 @@
         ],
         "IconExportName": [
             "icon_spell_toxic"
         ],
         "IconSWF": [
             "sc/ui.sc"
         ],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [
             true
         ],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [
             true
@@ -13408,25 +13716,26 @@
         ],
         "SpeedBoost2": [
             "-35"
         ],
         "SpellForgeLevel": [
             1
         ],
-        "StrengthWeight": [
-            "-160"
-        ],
+        "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [
             "TID_POISON_CLOUD_TOWER"
         ],
         "TargetInfoString": [
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             400
         ],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
         "TornadoForce3": [],
@@ -13535,27 +13844,30 @@
         "FreezeTimeMS": [
             100,
             100,
             100,
             100,
             100
         ],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             0,
             0,
             0,
             0,
             0
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -13639,14 +13951,17 @@
         "TargetInfoString": [
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             400,
             400,
             400,
             400,
             400
         ],
@@ -13751,14 +14066,16 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [
             "Heal spell",
             "Heal spell",
             "Heal spell",
             "Heal spell",
@@ -13788,14 +14105,15 @@
         "IconSWF": [
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc"
         ],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [
@@ -13898,21 +14216,15 @@
         "SpellForgeLevel": [
             5,
             5,
             5,
             5,
             5
         ],
-        "StrengthWeight": [
-            230,
-            230,
-            230,
-            230,
-            230
-        ],
+        "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [
             "TID_LIGHTNING_STORM",
             "TID_LIGHTNING_STORM",
             "TID_LIGHTNING_STORM",
             "TID_LIGHTNING_STORM",
@@ -13921,14 +14233,17 @@
         "TargetInfoString": [
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             300,
             300,
             300,
             300,
             300
         ],
@@ -14027,23 +14342,26 @@
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [
             800
         ],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             400
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -14100,14 +14418,17 @@
         "SpeedBoost2": [],
         "SpellForgeLevel": [],
         "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             0
         ],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
         "TornadoForce3": [],
@@ -14222,14 +14543,16 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             300,
             300,
             300,
@@ -14237,14 +14560,15 @@
             300,
             300,
             300
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -14356,14 +14680,17 @@
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             300,
             300,
             300,
             300,
             300,
             300,
@@ -14448,14 +14775,16 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             400
         ],
         "HousingSpace": [
@@ -14463,14 +14792,15 @@
         ],
         "IconExportName": [
             "icon_spell_rage"
         ],
         "IconSWF": [
             "sc/ui.sc"
         ],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [
@@ -14534,25 +14864,26 @@
         ],
         "SpeedBoost2": [
             15
         ],
         "SpellForgeLevel": [
             1
         ],
-        "StrengthWeight": [
-            100
-        ],
+        "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [
             "TID_HASTE_TOWER"
         ],
         "TargetInfoString": [
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             300
         ],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
         "TornadoForce3": [],
@@ -14629,23 +14960,26 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             300
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [
@@ -14703,23 +15037,24 @@
         "SpeedBoost": [
             0
         ],
         "SpeedBoost2": [
             0
         ],
         "SpellForgeLevel": [],
-        "StrengthWeight": [
-            0
-        ],
+        "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [
             "TID_RAM_RIDER_ABILITY_TITLE"
         ],
         "TargetInfoString": [],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             100
         ],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
         "TornadoForce3": [],
@@ -14826,14 +15161,16 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             100,
             100,
             100,
@@ -14857,14 +15194,15 @@
         "IconSWF": [
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc"
         ],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [
@@ -14992,19 +15330,19 @@
             7,
             7,
             7,
             7,
             7
         ],
         "StrengthWeight": [
-            120,
-            130,
-            140,
-            145,
-            150
+            1700,
+            1800,
+            1900,
+            2000,
+            2100
         ],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [
             "TID_SPELL_RECALL",
             "TID_SPELL_RECALL",
             "TID_SPELL_RECALL",
@@ -15014,14 +15352,17 @@
         "TargetInfoString": [
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             100,
             100,
             100,
             100,
             100
         ],
@@ -15203,14 +15544,16 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             0,
             0,
             0,
@@ -15229,14 +15572,15 @@
             0,
             0,
             0
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [
             true,
             true,
             true,
             true,
             true,
             true,
@@ -15531,14 +15875,17 @@
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             0,
             0,
             0,
             0,
             0,
             0,
@@ -15624,23 +15971,26 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             1000
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -15705,14 +16055,17 @@
         ],
         "SpellForgeLevel": [],
         "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             250
         ],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
         "TornadoForce3": [],
@@ -15779,23 +16132,26 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             400
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [
             true
         ],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [
             true
         ],
@@ -15866,14 +16222,17 @@
         "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             300
         ],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
         "TornadoForce3": [],
@@ -15950,27 +16309,30 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             300,
             300
         ],
         "HousingSpace": [
             2,
             2
         ],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -16043,28 +16405,28 @@
             "-30",
             "-40"
         ],
         "SpellForgeLevel": [
             1,
             1
         ],
-        "StrengthWeight": [
-            0,
-            0
-        ],
+        "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [
             "TID_SLOW_SPELL",
             "TID_SLOW_SPELL"
         ],
         "TargetInfoString": [
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             300,
             300
         ],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
@@ -16185,14 +16547,16 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             0,
             0,
             0,
@@ -16220,14 +16584,15 @@
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc"
         ],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [
@@ -16369,20 +16734,20 @@
             5,
             5,
             5,
             5,
             5
         ],
         "StrengthWeight": [
-            460,
-            470,
-            480,
-            500,
-            520,
-            560
+            1300,
+            1400,
+            1500,
+            1600,
+            1700,
+            2000
         ],
         "StunTimeMS": [],
         "SummonTroop": [
             "SpellBat",
             "SpellBat",
             "SpellBat",
             "SpellBat",
@@ -16401,14 +16766,17 @@
             "TID_BUILDING_CLASS_DEFENSE",
             "TID_BUILDING_CLASS_DEFENSE",
             "TID_BUILDING_CLASS_DEFENSE",
             "TID_BUILDING_CLASS_DEFENSE",
             "TID_BUILDING_CLASS_DEFENSE",
             "TID_BUILDING_CLASS_DEFENSE"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             300,
             300,
             300,
             300,
             300,
             300
@@ -16552,14 +16920,16 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             0,
             0,
             0,
@@ -16595,14 +16965,15 @@
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc"
         ],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [
@@ -16754,22 +17125,22 @@
             4,
             4,
             4,
             4,
             4
         ],
         "StrengthWeight": [
-            460,
-            470,
-            480,
-            500,
-            520,
-            540,
-            560,
-            580
+            1200,
+            1300,
+            1400,
+            1500,
+            1600,
+            1700,
+            1800,
+            2000
         ],
         "StunTimeMS": [],
         "SummonTroop": [
             "ShieldedSkeleton",
             "ShieldedSkeleton",
             "ShieldedSkeleton",
             "ShieldedSkeleton",
@@ -16794,14 +17165,17 @@
             "TID_INFO_TARGET_TYPE_GROUND",
             "TID_INFO_TARGET_TYPE_GROUND",
             "TID_INFO_TARGET_TYPE_GROUND",
             "TID_INFO_TARGET_TYPE_GROUND",
             "TID_INFO_TARGET_TYPE_GROUND",
             "TID_INFO_TARGET_TYPE_GROUND"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             300,
             300,
             300,
             300,
             300,
             300,
@@ -16954,14 +17328,16 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             400,
             400,
             400,
@@ -16985,14 +17361,15 @@
         "IconSWF": [
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc"
         ],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [
@@ -17114,19 +17491,19 @@
             3,
             3,
             3,
             3,
             3
         ],
         "StrengthWeight": [
-            200,
-            200,
-            180,
-            180,
-            180
+            1200,
+            1300,
+            1400,
+            1500,
+            1600
         ],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [
             "TID_SPEEDUP",
             "TID_SPEEDUP",
             "TID_SPEEDUP",
@@ -17136,14 +17513,17 @@
         "TargetInfoString": [
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             250,
             250,
             250,
             250,
             250
         ],
@@ -17285,14 +17665,16 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             0,
             0,
             0,
@@ -17303,14 +17685,15 @@
             0,
             0,
             0
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -17446,14 +17829,17 @@
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             0,
             0,
             0,
             0,
             0,
             0,
@@ -17576,14 +17962,16 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             0,
             0,
             0,
@@ -17594,14 +17982,15 @@
             0,
             0,
             0
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -17737,14 +18126,17 @@
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY",
             "TID_PREFERRED_TARGET_ANY"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             0,
             0,
             0,
             0,
             0,
             0,
@@ -17873,27 +18265,30 @@
         "FreezeTimeMS": [
             0,
             0,
             4000,
             6000,
             8000
         ],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             400,
             400,
             400,
             400,
             400
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -17971,14 +18366,17 @@
         "SpeedBoost2": [],
         "SpellForgeLevel": [],
         "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             0,
             0,
             0,
             0,
             0
         ],
@@ -18101,14 +18499,16 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [
             100,
             100,
             100,
             100,
             100
         ],
@@ -18120,14 +18520,15 @@
             400,
             400,
             400
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [
             true,
             true,
             true,
             true,
             true
         ],
@@ -18259,14 +18660,17 @@
         ],
         "SpellForgeLevel": [],
         "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             400,
             400,
             400,
             400,
             400
         ],
@@ -18389,14 +18793,16 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [
             100,
             100,
             100,
             100,
             100
         ],
@@ -18408,14 +18814,15 @@
             400,
             400,
             400
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [
             true,
             true,
             true,
             true,
             true
         ],
@@ -18547,14 +18954,17 @@
         ],
         "SpellForgeLevel": [],
         "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             400,
             400,
             400,
             400,
             400
         ],
@@ -18637,25 +19047,28 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             375,
             375,
             375
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -18723,14 +19136,17 @@
         "SpeedBoost2": [],
         "SpellForgeLevel": [],
         "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             128,
             128,
             128
         ],
         "TombStone": [],
         "TornadoForce1": [
@@ -18857,27 +19273,30 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [
             25
         ],
         "HideImmunityVFX": [
             true
         ],
         "HitEffect": [],
         "HitTimeMS": [
             500
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [
             true
         ],
         "ImmunityOtherCharacters": [
             true
         ],
         "ImmunitySiegeMachines": [
@@ -18939,23 +19358,24 @@
         "SpawnDuration": [],
         "SpawnFirstGroupSize": [],
         "SpawnObstacle": [],
         "SpawnUpgradeLevel": [],
         "SpeedBoost": [],
         "SpeedBoost2": [],
         "SpellForgeLevel": [],
-        "StrengthWeight": [
-            0
-        ],
+        "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             400
         ],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
         "TornadoForce3": [],
@@ -19024,23 +19444,26 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             0
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -19101,14 +19524,17 @@
         "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [
             "TID_PREFERRED_TARGET_ANY"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             0
         ],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
         "TornadoForce3": [],
@@ -19181,23 +19607,26 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             400
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -19260,14 +19689,17 @@
         ],
         "SpellForgeLevel": [],
         "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             250
         ],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
         "TornadoForce3": [],
@@ -19330,21 +19762,28 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [
+            6000,
+            7000,
+            8000
+        ],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -19412,14 +19851,17 @@
         "SpeedBoost2": [],
         "SpellForgeLevel": [],
         "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
         "TornadoForce3": [],
         "TornadoForce4": [],
         "TornadoForce5": [],
@@ -19516,14 +19958,16 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             0,
             0,
             0,
@@ -19533,14 +19977,15 @@
             0,
             0,
             0
         ],
         "HousingSpace": [],
         "IconExportName": [],
         "IconSWF": [],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [],
@@ -19628,14 +20073,17 @@
         ],
         "SpellForgeLevel": [],
         "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [],
         "TargetInfoString": [],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             0,
             0,
             0,
             0,
             0,
             0,
@@ -19718,14 +20166,16 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [
             "Ice Breaker Hit lvl1"
         ],
         "HitTimeMS": [
             0
@@ -19735,14 +20185,15 @@
         ],
         "IconExportName": [
             "icon_spell_freeze"
         ],
         "IconSWF": [
             "sc/ui.sc"
         ],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [
@@ -19810,25 +20261,26 @@
         ],
         "SpeedBoost2": [
             0
         ],
         "SpellForgeLevel": [
             4
         ],
-        "StrengthWeight": [
-            1000
-        ],
+        "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [
             "TID_FREEZE_SPELL"
         ],
         "TargetInfoString": [
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             0
         ],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
         "TornadoForce3": [],
@@ -19911,14 +20363,16 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [
             "Ice Breaker Hit lvl1"
         ],
         "HitTimeMS": [
             0
@@ -19928,14 +20382,15 @@
         ],
         "IconExportName": [
             "icon_spell_freeze"
         ],
         "IconSWF": [
             "sc/ui.sc"
         ],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [
@@ -20003,25 +20458,26 @@
         ],
         "SpeedBoost2": [
             0
         ],
         "SpellForgeLevel": [
             4
         ],
-        "StrengthWeight": [
-            1000
-        ],
+        "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [
             "TID_FREEZE_SPELL"
         ],
         "TargetInfoString": [
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             0
         ],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
         "TornadoForce3": [],
@@ -20060,167 +20516,364 @@
         ],
         "AttackSpeedBoost": [],
         "BigPicture": [
             "icon_spell_freeze"
         ],
         "BoostDefenders": [],
         "BoostLinkedToPoison": [],
-        "BoostTimeMS": [],
+        "BoostTimeMS": [
+            0
+        ],
         "BuildingDamageBoostPercent": [],
         "BuildingDamagePermil": [],
         "CapitalAttackCount": [],
         "ChainSpell": [],
         "ChangeTeamTime": [],
         "ChargingEffect": [],
         "ChargingTimeMS": [
-            300
+            0
+        ],
+        "ConeAngle": [
+            90
         ],
-        "ConeAngle": [],
         "Damage": [
-            5
+            390
         ],
         "DamageBoostPercent": [],
         "DamagePermilMin": [],
         "DamageTHPercent": [],
-        "DeployEffect": [
-            "Blizzard"
-        ],
+        "DeployEffect": [],
         "DeployEffect2": [],
         "DeployEffect2Delay": [],
         "DeployTimeMS": [
-            800
+            0
         ],
         "DestroyWalls": [],
         "DisableDonate": [],
         "DisableProduction": [
             true
         ],
-        "DonateCost": [
-            10
-        ],
+        "DonateCost": [],
         "DuplicateHousing": [],
         "DuplicateLifetime": [],
         "EnabledByCalendar": [],
         "EnemyDeployEffect": [],
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
-        "FreezeOuterTimeMS": [
-            500
+        "FreezeOuterTimeMS": [],
+        "FreezePercent": [],
+        "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
+        "HeroDamageMultiplier": [],
+        "HideImmunityVFX": [],
+        "HitEffect": [
+            "Ice Breaker Hit lvl1"
         ],
-        "FreezePercent": [
-            70
+        "HitTimeMS": [
+            0
         ],
-        "FreezeTimeMS": [
+        "HousingSpace": [
+            1
+        ],
+        "IconExportName": [
+            "icon_spell_freeze"
+        ],
+        "IconSWF": [
+            "sc/ui.sc"
+        ],
+        "ImmortalTime": [],
+        "ImmunityOtherBuildings": [],
+        "ImmunityOtherCharacters": [],
+        "ImmunitySiegeMachines": [],
+        "ImmunityStorages": [],
+        "ImmunityTH_CC": [],
+        "ImmunityWalls": [],
+        "InfoTID": [
+            "TID_FREEZE_SPELL_INFO"
+        ],
+        "InvisibilityTime": [],
+        "JumpBoostMS": [],
+        "JumpHousingLimit": [],
+        "LaboratoryLevel": [
+            8
+        ],
+        "Level": [
+            1
+        ],
+        "MaxUnitsHit": [],
+        "MinDamage": [
+            130
+        ],
+        "MinRadius": [
+            100
+        ],
+        "NumObstacles": [],
+        "NumTombStones": [],
+        "NumberOfHits": [
+            1
+        ],
+        "Overgrowth": [],
+        "PauseCombatComponentsMs": [],
+        "PoisonAffectAir": [],
+        "PoisonDPS": [],
+        "PoisonIncreaseSlowly": [],
+        "PreDeployEffect": [],
+        "PreferredDamagePermilMin": [],
+        "PreferredTarget": [],
+        "PreferredTargetDamageMod": [],
+        "PreviewScenario": [],
+        "ProductionBuilding": [
+            "Spell Forge"
+        ],
+        "Radius": [
             500
         ],
+        "RandomRadius": [
+            0
+        ],
+        "RandomRadiusAffectsOnlyGfx": [
+            true
+        ],
+        "RecallHousing": [],
+        "ScaleByTH": [],
+        "ScaleDeployEffects": [],
+        "ShieldProjectileDamageMod": [],
+        "ShieldProjectileSpeed": [],
+        "ShieldProtectionPercent": [],
+        "ShieldTime": [],
+        "ShrinkHitpointsRatio": [],
+        "ShrinkReduceSpeedRatio": [],
+        "SnapToGrid": [],
+        "SpawnDuration": [],
+        "SpawnFirstGroupSize": [],
+        "SpawnObstacle": [],
+        "SpawnUpgradeLevel": [],
+        "SpeedBoost": [
+            0
+        ],
+        "SpeedBoost2": [
+            0
+        ],
+        "SpellForgeLevel": [
+            4
+        ],
+        "StrengthWeight": [],
+        "StunTimeMS": [],
+        "SummonTroop": [],
+        "TID": [
+            "TID_FREEZE_SPELL"
+        ],
+        "TargetInfoString": [
+            "TID_INFO_TARGET_TYPE_GROUND_AND_AIR"
+        ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
+        "TimeBetweenHitsMS": [
+            0
+        ],
+        "TombStone": [],
+        "TornadoForce1": [],
+        "TornadoForce2": [],
+        "TornadoForce3": [],
+        "TornadoForce4": [],
+        "TornadoForce5": [],
+        "TornadoForceAir1": [],
+        "TornadoForceAir2": [],
+        "TornadoForceAir3": [],
+        "TornadoForceAir4": [],
+        "TornadoForceAir5": [],
+        "TornadoInnerForcePercent": [],
+        "TornadoInnerRadius": [],
+        "TornadoOuterForcePercent": [],
+        "TornadoRotationSpeed": [],
+        "TornadoSpeedTowardsCenter": [],
+        "TrainingTime": [
+            180
+        ],
+        "TroopDamagePermil": [],
+        "UnitsToSpawn": [],
+        "UpgradeCost": [
+            0
+        ],
+        "UpgradeLevelByTH": [],
+        "UpgradeResource": [
+            "Elixir"
+        ],
+        "UpgradeTimeH": [
+            72
+        ],
+        "VillageType": []
+    },
+    "Unused13": {
+        "AffectsSiegeMachines": [
+            true
+        ],
+        "AttackSpeedBoost": [],
+        "BigPicture": [
+            "icon_spell_freeze"
+        ],
+        "BoostDefenders": [],
+        "BoostLinkedToPoison": [],
+        "BoostTimeMS": [
+            0
+        ],
+        "BuildingDamageBoostPercent": [],
+        "BuildingDamagePermil": [],
+        "CapitalAttackCount": [],
+        "ChainSpell": [],
+        "ChangeTeamTime": [],
+        "ChargingEffect": [],
+        "ChargingTimeMS": [
+            0
+        ],
+        "ConeAngle": [
+            90
+        ],
+        "Damage": [
+            390
+        ],
+        "DamageBoostPercent": [],
+        "DamagePermilMin": [],
+        "DamageTHPercent": [],
+        "DeployEffect": [],
+        "DeployEffect2": [],
+        "DeployEffect2Delay": [],
+        "DeployTimeMS": [
+            0
+        ],
+        "DestroyWalls": [],
+        "DisableDonate": [],
+        "DisableProduction": [
+            true
+        ],
+        "DonateCost": [],
+        "DuplicateHousing": [],
+        "DuplicateLifetime": [],
+        "EnabledByCalendar": [],
+        "EnemyDeployEffect": [],
+        "ExecuteHealthPermil": [],
+        "ExtraHealthMax": [],
+        "ExtraHealthMin": [],
+        "ExtraHealthPermil": [],
+        "FreezeOuterTimeMS": [],
+        "FreezePercent": [],
+        "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
-        "HitEffect": [],
+        "HitEffect": [
+            "Ice Breaker Hit lvl1"
+        ],
         "HitTimeMS": [
-            400
+            0
         ],
         "HousingSpace": [
             1
         ],
         "IconExportName": [
-            "icon_spell_cc_frost"
+            "icon_spell_freeze"
         ],
         "IconSWF": [
             "sc/ui.sc"
         ],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
-        "ImmunityStorages": [
-            true
-        ],
+        "ImmunityStorages": [],
         "ImmunityTH_CC": [],
-        "ImmunityWalls": [
-            true
-        ],
+        "ImmunityWalls": [],
         "InfoTID": [
-            "TID_SPELL_FROST_INFO"
+            "TID_FREEZE_SPELL_INFO"
         ],
         "InvisibilityTime": [],
         "JumpBoostMS": [],
         "JumpHousingLimit": [],
         "LaboratoryLevel": [
-            1
+            8
         ],
         "Level": [
             1
         ],
         "MaxUnitsHit": [],
-        "MinDamage": [],
-        "MinRadius": [],
+        "MinDamage": [
+            130
+        ],
+        "MinRadius": [
+            100
+        ],
         "NumObstacles": [],
         "NumTombStones": [],
         "NumberOfHits": [
-            67
+            1
         ],
         "Overgrowth": [],
         "PauseCombatComponentsMs": [],
         "PoisonAffectAir": [],
         "PoisonDPS": [],
         "PoisonIncreaseSlowly": [],
-        "PreDeployEffect": [
-            "Capital Frost Predeploy"
-        ],
+        "PreDeployEffect": [],
         "PreferredDamagePermilMin": [],
         "PreferredTarget": [],
         "PreferredTargetDamageMod": [],
         "PreviewScenario": [],
         "ProductionBuilding": [
-            "Mini Spell Factory"
+            "Spell Forge"
         ],
         "Radius": [
             500
         ],
         "RandomRadius": [
-            400
+            0
         ],
         "RandomRadiusAffectsOnlyGfx": [
             true
         ],
         "RecallHousing": [],
         "ScaleByTH": [],
-        "ScaleDeployEffects": [
-            true
-        ],
+        "ScaleDeployEffects": [],
         "ShieldProjectileDamageMod": [],
         "ShieldProjectileSpeed": [],
         "ShieldProtectionPercent": [],
         "ShieldTime": [],
         "ShrinkHitpointsRatio": [],
         "ShrinkReduceSpeedRatio": [],
         "SnapToGrid": [],
         "SpawnDuration": [],
         "SpawnFirstGroupSize": [],
         "SpawnObstacle": [],
         "SpawnUpgradeLevel": [],
-        "SpeedBoost": [],
-        "SpeedBoost2": [],
-        "SpellForgeLevel": [
-            5
+        "SpeedBoost": [
+            0
         ],
-        "StrengthWeight": [
-            1000
+        "SpeedBoost2": [
+            0
+        ],
+        "SpellForgeLevel": [
+            4
         ],
+        "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [
-            "TID_SPELL_FROST"
+            "TID_FREEZE_SPELL"
         ],
         "TargetInfoString": [
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
-            300
+            0
         ],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
         "TornadoForce3": [],
         "TornadoForce4": [],
         "TornadoForce5": [],
@@ -20236,188 +20889,395 @@
         "TornadoSpeedTowardsCenter": [],
         "TrainingTime": [
             180
         ],
         "TroopDamagePermil": [],
         "UnitsToSpawn": [],
         "UpgradeCost": [
-            26000
+            0
         ],
         "UpgradeLevelByTH": [],
         "UpgradeResource": [
-            "DarkElixir"
+            "Elixir"
         ],
         "UpgradeTimeH": [
-            42
+            72
         ],
         "VillageType": []
     },
-    "Unused13": {
+    "Unused14": {
         "AffectsSiegeMachines": [
             true
         ],
         "AttackSpeedBoost": [],
         "BigPicture": [
             "icon_spell_freeze"
         ],
         "BoostDefenders": [],
         "BoostLinkedToPoison": [],
+        "BoostTimeMS": [
+            0
+        ],
+        "BuildingDamageBoostPercent": [],
+        "BuildingDamagePermil": [],
+        "CapitalAttackCount": [],
+        "ChainSpell": [],
+        "ChangeTeamTime": [],
+        "ChargingEffect": [],
+        "ChargingTimeMS": [
+            0
+        ],
+        "ConeAngle": [
+            90
+        ],
+        "Damage": [
+            390
+        ],
+        "DamageBoostPercent": [],
+        "DamagePermilMin": [],
+        "DamageTHPercent": [],
+        "DeployEffect": [],
+        "DeployEffect2": [],
+        "DeployEffect2Delay": [],
+        "DeployTimeMS": [
+            0
+        ],
+        "DestroyWalls": [],
+        "DisableDonate": [],
+        "DisableProduction": [
+            true
+        ],
+        "DonateCost": [],
+        "DuplicateHousing": [],
+        "DuplicateLifetime": [],
+        "EnabledByCalendar": [],
+        "EnemyDeployEffect": [],
+        "ExecuteHealthPermil": [],
+        "ExtraHealthMax": [],
+        "ExtraHealthMin": [],
+        "ExtraHealthPermil": [],
+        "FreezeOuterTimeMS": [],
+        "FreezePercent": [],
+        "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
+        "HeroDamageMultiplier": [],
+        "HideImmunityVFX": [],
+        "HitEffect": [
+            "Ice Breaker Hit lvl1"
+        ],
+        "HitTimeMS": [
+            0
+        ],
+        "HousingSpace": [
+            1
+        ],
+        "IconExportName": [
+            "icon_spell_freeze"
+        ],
+        "IconSWF": [
+            "sc/ui.sc"
+        ],
+        "ImmortalTime": [],
+        "ImmunityOtherBuildings": [],
+        "ImmunityOtherCharacters": [],
+        "ImmunitySiegeMachines": [],
+        "ImmunityStorages": [],
+        "ImmunityTH_CC": [],
+        "ImmunityWalls": [],
+        "InfoTID": [
+            "TID_FREEZE_SPELL_INFO"
+        ],
+        "InvisibilityTime": [],
+        "JumpBoostMS": [],
+        "JumpHousingLimit": [],
+        "LaboratoryLevel": [
+            8
+        ],
+        "Level": [
+            1
+        ],
+        "MaxUnitsHit": [],
+        "MinDamage": [
+            130
+        ],
+        "MinRadius": [
+            100
+        ],
+        "NumObstacles": [],
+        "NumTombStones": [],
+        "NumberOfHits": [
+            1
+        ],
+        "Overgrowth": [],
+        "PauseCombatComponentsMs": [],
+        "PoisonAffectAir": [],
+        "PoisonDPS": [],
+        "PoisonIncreaseSlowly": [],
+        "PreDeployEffect": [],
+        "PreferredDamagePermilMin": [],
+        "PreferredTarget": [],
+        "PreferredTargetDamageMod": [],
+        "PreviewScenario": [],
+        "ProductionBuilding": [
+            "Spell Forge"
+        ],
+        "Radius": [
+            500
+        ],
+        "RandomRadius": [
+            0
+        ],
+        "RandomRadiusAffectsOnlyGfx": [
+            true
+        ],
+        "RecallHousing": [],
+        "ScaleByTH": [],
+        "ScaleDeployEffects": [],
+        "ShieldProjectileDamageMod": [],
+        "ShieldProjectileSpeed": [],
+        "ShieldProtectionPercent": [],
+        "ShieldTime": [],
+        "ShrinkHitpointsRatio": [],
+        "ShrinkReduceSpeedRatio": [],
+        "SnapToGrid": [],
+        "SpawnDuration": [],
+        "SpawnFirstGroupSize": [],
+        "SpawnObstacle": [],
+        "SpawnUpgradeLevel": [],
+        "SpeedBoost": [
+            0
+        ],
+        "SpeedBoost2": [
+            0
+        ],
+        "SpellForgeLevel": [
+            4
+        ],
+        "StrengthWeight": [],
+        "StunTimeMS": [],
+        "SummonTroop": [],
+        "TID": [
+            "TID_FREEZE_SPELL"
+        ],
+        "TargetInfoString": [
+            "TID_INFO_TARGET_TYPE_GROUND_AND_AIR"
+        ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
+        "TimeBetweenHitsMS": [
+            0
+        ],
+        "TombStone": [],
+        "TornadoForce1": [],
+        "TornadoForce2": [],
+        "TornadoForce3": [],
+        "TornadoForce4": [],
+        "TornadoForce5": [],
+        "TornadoForceAir1": [],
+        "TornadoForceAir2": [],
+        "TornadoForceAir3": [],
+        "TornadoForceAir4": [],
+        "TornadoForceAir5": [],
+        "TornadoInnerForcePercent": [],
+        "TornadoInnerRadius": [],
+        "TornadoOuterForcePercent": [],
+        "TornadoRotationSpeed": [],
+        "TornadoSpeedTowardsCenter": [],
+        "TrainingTime": [
+            180
+        ],
+        "TroopDamagePermil": [],
+        "UnitsToSpawn": [],
+        "UpgradeCost": [
+            0
+        ],
+        "UpgradeLevelByTH": [],
+        "UpgradeResource": [
+            "Elixir"
+        ],
+        "UpgradeTimeH": [
+            72
+        ],
+        "VillageType": []
+    },
+    "Yellow Card": {
+        "AffectsSiegeMachines": [],
+        "AttackSpeedBoost": [],
+        "BigPicture": [
+            "icon_spell_suspension"
+        ],
+        "BoostDefenders": [
+            true
+        ],
+        "BoostLinkedToPoison": [],
         "BoostTimeMS": [],
         "BuildingDamageBoostPercent": [],
         "BuildingDamagePermil": [],
         "CapitalAttackCount": [],
         "ChainSpell": [],
         "ChangeTeamTime": [],
         "ChargingEffect": [],
         "ChargingTimeMS": [
             300
         ],
         "ConeAngle": [],
-        "Damage": [
-            5
-        ],
+        "Damage": [],
         "DamageBoostPercent": [],
         "DamagePermilMin": [],
         "DamageTHPercent": [],
         "DeployEffect": [
-            "Blizzard"
+            "Yellow Card Effect"
         ],
         "DeployEffect2": [],
         "DeployEffect2Delay": [],
         "DeployTimeMS": [
             800
         ],
         "DestroyWalls": [],
-        "DisableDonate": [],
-        "DisableProduction": [
+        "DisableDonate": [
             true
         ],
+        "DisableProduction": [],
         "DonateCost": [
             10
         ],
         "DuplicateHousing": [],
         "DuplicateLifetime": [],
-        "EnabledByCalendar": [],
+        "EnabledByCalendar": [
+            true
+        ],
         "EnemyDeployEffect": [],
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [
-            500
-        ],
-        "FreezePercent": [
-            70
+            15000
         ],
+        "FreezePercent": [],
         "FreezeTimeMS": [
-            500
+            15000
         ],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [],
         "HitTimeMS": [
             400
         ],
         "HousingSpace": [
             1
         ],
         "IconExportName": [
-            "icon_spell_cc_frost"
+            "icon_spell_suspension"
         ],
         "IconSWF": [
             "sc/ui.sc"
         ],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
-        "ImmunitySiegeMachines": [],
-        "ImmunityStorages": [
+        "ImmunitySiegeMachines": [
             true
         ],
+        "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [
             true
         ],
         "InfoTID": [
-            "TID_SPELL_FROST_INFO"
+            "TID_SPELL_YELLOW_CARD_INFO"
+        ],
+        "InvisibilityTime": [
+            15000
         ],
-        "InvisibilityTime": [],
         "JumpBoostMS": [],
         "JumpHousingLimit": [],
         "LaboratoryLevel": [
             1
         ],
         "Level": [
             1
         ],
         "MaxUnitsHit": [],
         "MinDamage": [],
         "MinRadius": [],
         "NumObstacles": [],
         "NumTombStones": [],
         "NumberOfHits": [
-            67
+            1
         ],
         "Overgrowth": [],
         "PauseCombatComponentsMs": [],
         "PoisonAffectAir": [],
         "PoisonDPS": [],
         "PoisonIncreaseSlowly": [],
         "PreDeployEffect": [
-            "Capital Frost Predeploy"
+            "Referee Whistle Effect"
         ],
         "PreferredDamagePermilMin": [],
         "PreferredTarget": [],
         "PreferredTargetDamageMod": [],
-        "PreviewScenario": [],
+        "PreviewScenario": [
+            "SpellYellowCard"
+        ],
         "ProductionBuilding": [
-            "Mini Spell Factory"
+            "Spell Forge"
         ],
         "Radius": [
-            500
+            0
         ],
         "RandomRadius": [
-            400
+            0
         ],
         "RandomRadiusAffectsOnlyGfx": [
             true
         ],
         "RecallHousing": [],
         "ScaleByTH": [],
-        "ScaleDeployEffects": [
-            true
-        ],
+        "ScaleDeployEffects": [],
         "ShieldProjectileDamageMod": [],
         "ShieldProjectileSpeed": [],
         "ShieldProtectionPercent": [],
         "ShieldTime": [],
         "ShrinkHitpointsRatio": [],
         "ShrinkReduceSpeedRatio": [],
         "SnapToGrid": [],
         "SpawnDuration": [],
         "SpawnFirstGroupSize": [],
         "SpawnObstacle": [],
         "SpawnUpgradeLevel": [],
         "SpeedBoost": [],
         "SpeedBoost2": [],
         "SpellForgeLevel": [
-            5
-        ],
-        "StrengthWeight": [
-            1000
+            1
         ],
+        "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [
-            "TID_SPELL_FROST"
+            "TID_SPELL_YELLOW_CARD"
         ],
         "TargetInfoString": [
-            "TID_INFO_TARGET_TYPE_GROUND_AND_AIR"
+            "TID_INFO_TARGET_TYPE_DEFENSES_AND_HEROES"
+        ],
+        "Targeted": [
+            true
+        ],
+        "TargetedAgainEffect": [
+            "Red Card Effect"
+        ],
+        "TargetedProjectile": [
+            "Yellow Card Projectile"
         ],
         "TimeBetweenHitsMS": [
-            300
+            0
         ],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
         "TornadoForce3": [],
         "TornadoForce4": [],
         "TornadoForce5": [],
@@ -20432,24 +21292,22 @@
         "TornadoRotationSpeed": [],
         "TornadoSpeedTowardsCenter": [],
         "TrainingTime": [
             180
         ],
         "TroopDamagePermil": [],
         "UnitsToSpawn": [],
-        "UpgradeCost": [
-            26000
+        "UpgradeCost": [],
+        "UpgradeLevelByTH": [
+            6
         ],
-        "UpgradeLevelByTH": [],
         "UpgradeResource": [
-            "DarkElixir"
-        ],
-        "UpgradeTimeH": [
-            42
+            "Elixir"
         ],
+        "UpgradeTimeH": [],
         "VillageType": []
     },
     "xmas": {
         "AffectsSiegeMachines": [],
         "AttackSpeedBoost": [],
         "BigPicture": [
             "icon_spell_xmas"
@@ -20502,14 +21360,16 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [
             "xmas boom"
         ],
         "HitTimeMS": [
             6000
@@ -20519,14 +21379,15 @@
         ],
         "IconExportName": [
             "icon_spell_xmas"
         ],
         "IconSWF": [
             "sc/ui.sc"
         ],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [],
         "ImmunityTH_CC": [],
         "ImmunityWalls": [],
         "InfoTID": [
@@ -20590,25 +21451,26 @@
         "SpawnObstacle": [],
         "SpawnUpgradeLevel": [],
         "SpeedBoost": [],
         "SpeedBoost2": [],
         "SpellForgeLevel": [
             1
         ],
-        "StrengthWeight": [
-            0
-        ],
+        "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [
             "TID_XMAS_SPELL"
         ],
         "TargetInfoString": [
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             100
         ],
         "TombStone": [],
         "TornadoForce1": [],
         "TornadoForce2": [],
         "TornadoForce3": [],
@@ -20791,14 +21653,16 @@
         "ExecuteHealthPermil": [],
         "ExtraHealthMax": [],
         "ExtraHealthMin": [],
         "ExtraHealthPermil": [],
         "FreezeOuterTimeMS": [],
         "FreezePercent": [],
         "FreezeTimeMS": [],
+        "GiveSpecialAbility": [],
+        "GivenSpecialAbilityLevel": [],
         "HeroDamageMultiplier": [],
         "HideImmunityVFX": [],
         "HitEffect": [
             "xmas boom",
             "xmas boom",
             "xmas boom",
             "xmas boom",
@@ -20858,14 +21722,15 @@
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc",
             "sc/ui.sc"
         ],
+        "ImmortalTime": [],
         "ImmunityOtherBuildings": [],
         "ImmunityOtherCharacters": [],
         "ImmunitySiegeMachines": [],
         "ImmunityStorages": [
             true,
             true,
             true,
@@ -21064,27 +21929,15 @@
             1,
             1,
             1,
             1,
             1,
             1
         ],
-        "StrengthWeight": [
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0,
-            0
-        ],
+        "StrengthWeight": [],
         "StunTimeMS": [],
         "SummonTroop": [],
         "TID": [
             "TID_XMAS_SPELL",
             "TID_XMAS_SPELL",
             "TID_XMAS_SPELL",
             "TID_XMAS_SPELL",
@@ -21105,14 +21958,17 @@
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR",
             "TID_INFO_TARGET_TYPE_GROUND_AND_AIR"
         ],
+        "Targeted": [],
+        "TargetedAgainEffect": [],
+        "TargetedProjectile": [],
         "TimeBetweenHitsMS": [
             100,
             100,
             100,
             100,
             100,
             100,
```

### Comparing `coc.py-3.4.1/coc/static/supers.json` & `coc_py-3.4.2/coc/static/supers.json`

 * *Files identical despite different names*

### Comparing `coc.py-3.4.1/coc/static/texts_EN.json` & `coc_py-3.4.2/coc/static/texts_EN.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9787039456493337%*

 * *Differences: {"'TID_ABILITY_FREE_KICK'": "OrderedDict([('EN', ['Free Kick'])])",*

 * * "'TID_ABILITY_FREE_KICK_INFO'": "OrderedDict([('EN', ['Targets closest Defense causing <num> "*

 * *                                 "damage'])])",*

 * * "'TID_ABILITY_THROW_IN'": "OrderedDict([('EN', ['Throw In'])])",*

 * * "'TID_ABILITY_THROW_IN_INFO'": "OrderedDict([('EN', ['Bounces twice, destroys Walls and causes "*

 * *                                "<num> damage each time it lands'])])",*

 * * "'TID_BASIC_TURRET_INFO'": "{'EN': ['Cannons are great for poin […]*

```diff
@@ -70,14 +70,34 @@
         ]
     },
     "TID_ABILITY_COOLDOWN": {
         "EN": [
             "Cooldown <number>s"
         ]
     },
+    "TID_ABILITY_FREE_KICK": {
+        "EN": [
+            "Free Kick"
+        ]
+    },
+    "TID_ABILITY_FREE_KICK_INFO": {
+        "EN": [
+            "Targets closest Defense causing <num> damage"
+        ]
+    },
+    "TID_ABILITY_THROW_IN": {
+        "EN": [
+            "Throw In"
+        ]
+    },
+    "TID_ABILITY_THROW_IN_INFO": {
+        "EN": [
+            "Bounces twice, destroys Walls and causes <num> damage each time it lands"
+        ]
+    },
     "TID_ABOUT": {
         "EN": [
             "Credits\\n\\n<names>\\n\\nClash of Clans \u2122 <version>\\nCopyright 2012-2024 Supercell Ltd. All Rights Reserved.\\nUS Patent Pending\\nAll use of this software is subject to Terms and Conditions and Privacy Policy at www.supercell.com."
         ]
     },
     "TID_ABOUT_BUTTON": {
         "EN": [
@@ -3172,15 +3192,15 @@
     "TID_BASE_DPS": {
         "EN": [
             "Base damage per second: <number>"
         ]
     },
     "TID_BASIC_TURRET_INFO": {
         "EN": [
-            "Cannons are great for point defense. Upgrade Cannons to increase their firepower, but beware that your defensive turrets cannot shoot while being upgraded!"
+            "Cannons are great for point defense. Upgrade Cannons to increase their firepower, but beware that your Defenses cannot shoot while being upgraded!"
         ]
     },
     "TID_BASIC_TURRET_INFO_SHORT": {
         "EN": [
             "Blasts away at pesky ground attackers."
         ]
     },
@@ -6170,14 +6190,19 @@
         ]
     },
     "TID_BUILDER_HALL_9_INFO_SHORT": {
         "EN": [
             "A little construction to complement all that destruction."
         ]
     },
+    "TID_BUILDER_HUB_TEXT": {
+        "EN": [
+            "Enjoy your <cffcc33>Builder Boost</c>"
+        ]
+    },
     "TID_BUILDER_MENU_CAPITAL": {
         "EN": [
             "Clan Capital"
         ]
     },
     "TID_BUILDING_AIR_DEFENSE": {
         "EN": [
@@ -6835,14 +6860,29 @@
         ]
     },
     "TID_BUTTON_CLAN_MAIL_SEND": {
         "EN": [
             "Send mail"
         ]
     },
+    "TID_BUTTON_CLAN_NOTICE_BOARD": {
+        "EN": [
+            "Notice Board"
+        ]
+    },
+    "TID_BUTTON_CLAN_NOTICE_DESCRIPTION": {
+        "EN": [
+            "Notice Description"
+        ]
+    },
+    "TID_BUTTON_CLAN_NOTICE_MESSAGE": {
+        "EN": [
+            "Use Clan Message"
+        ]
+    },
     "TID_BUTTON_CLAN_NOTICE_PUBLISH": {
         "EN": [
             "Publish Notice"
         ]
     },
     "TID_BUTTON_CLAN_NOTICE_PUBLISH_INFO_1": {
         "EN": [
@@ -6850,14 +6890,19 @@
         ]
     },
     "TID_BUTTON_CLAN_NOTICE_PUBLISH_INFO_2": {
         "EN": [
             "Your Clan Notice is currently active."
         ]
     },
+    "TID_BUTTON_CLAN_SEND_REQUEST": {
+        "EN": [
+            "Send Request"
+        ]
+    },
     "TID_BUTTON_CLAN_WAR_HISTORY": {
         "EN": [
             "War Log"
         ]
     },
     "TID_BUTTON_CLAN_WAR_MATCHED_START": {
         "EN": [
@@ -7220,14 +7265,19 @@
         ]
     },
     "TID_BUTTON_SEND_AWAY_MASTERBUILDER": {
         "EN": [
             "Travel"
         ]
     },
+    "TID_BUTTON_SEND_WAR_SIGNUP": {
+        "EN": [
+            "Send War Sign-up"
+        ]
+    },
     "TID_BUTTON_SET": {
         "EN": [
             "Confirm"
         ]
     },
     "TID_BUTTON_SHARE_LAYOUT_CHAT": {
         "EN": [
@@ -7330,14 +7380,19 @@
         ]
     },
     "TID_BUTTON_UPGRADE_WEAPON": {
         "EN": [
             "Upgrade Weapon"
         ]
     },
+    "TID_BUTTON_USE": {
+        "EN": [
+            "Use"
+        ]
+    },
     "TID_BUTTON_USE_FILL_STORAGE_BOOSTER": {
         "EN": [
             "Fill"
         ]
     },
     "TID_BUTTON_VIEW": {
         "EN": [
@@ -8735,14 +8790,19 @@
         ]
     },
     "TID_CAULDRON_REWARD_INFO2": {
         "EN": [
             "When the event ends you'll receive the Sour Elixir Cauldron as a decoration"
         ]
     },
+    "TID_CHALLENGES_HUB_TEXT": {
+        "EN": [
+            "Check out <cffcc33>Challenges</c> to guide your next steps"
+        ]
+    },
     "TID_CHALLENGE_ALREADY_CLOSED": {
         "EN": [
             "Challenge already closed"
         ]
     },
     "TID_CHALLENGE_ATTACK_CODE": {
         "EN": [
@@ -8765,14 +8825,19 @@
         ]
     },
     "TID_CHALLENGE_CANT_REQUEST": {
         "EN": [
             "Join a Clan to request Clan Castle Troops, Spells and Siege Machines"
         ]
     },
+    "TID_CHALLENGE_CASTLE_EMPTY": {
+        "EN": [
+            "Your Clan Castle is empty!"
+        ]
+    },
     "TID_CHALLENGE_CHANGE_LAYOUT": {
         "EN": [
             "Change layout"
         ]
     },
     "TID_CHALLENGE_CHANGE_LAYOUT_BUTTON": {
         "EN": [
@@ -9155,24 +9220,44 @@
         ]
     },
     "TID_CHARACTER_BARCHER": {
         "EN": [
             "Barcher"
         ]
     },
+    "TID_CHARACTER_BATTLE_DRUID": {
+        "EN": [
+            "WIP Battle Druid"
+        ]
+    },
+    "TID_CHARACTER_BATTLE_DRUID_INFO": {
+        "EN": [
+            "WIP This Druid attacks buildings and heals troops around that area."
+        ]
+    },
     "TID_CHARACTER_BIG_BOY": {
         "EN": [
             "Big Boy"
         ]
     },
     "TID_CHARACTER_CANNON_CART_ACTIVE_INFO": {
         "EN": [
             "Swaps between Cart and Mortar mode when activated"
         ]
     },
+    "TID_CHARACTER_CHAIN_HEAL_DRUID": {
+        "EN": [
+            "WIP Chain Heal Druid"
+        ]
+    },
+    "TID_CHARACTER_CHAIN_HEAL_DRUID_INFO": {
+        "EN": [
+            "WIP This Druid casts a heal that chains to other nearby troops."
+        ]
+    },
     "TID_CHARACTER_CHANGE_MODE_ACTIVE": {
         "EN": [
             "Change Mode"
         ]
     },
     "TID_CHARACTER_COOKIE_PEKKA": {
         "EN": [
@@ -9222,15 +9307,20 @@
     "TID_CHARACTER_FIRECRACKER": {
         "EN": [
             "Firecracker"
         ]
     },
     "TID_CHARACTER_FIREMITE": {
         "EN": [
-            "Firemite"
+            "WIP Firemite"
+        ]
+    },
+    "TID_CHARACTER_FREE_KICKER": {
+        "EN": [
+            "Barbarian Kicker"
         ]
     },
     "TID_CHARACTER_GIANT_ACTIVE": {
         "EN": [
             "Boxer Block"
         ]
     },
@@ -9455,22 +9545,27 @@
         ]
     },
     "TID_CHARACTER_INFO_FLYING_GOBLIN": {
         "EN": [
             "Flying Menace to wreck havoc in the Village. Hopefully at enemy Village."
         ]
     },
+    "TID_CHARACTER_INFO_FREE_KICKER": {
+        "EN": [
+            "Starts the match with a calm, carefully aimed shot that smashes the nearest Defense. Then goes on the usual Barbarian rampage."
+        ]
+    },
     "TID_CHARACTER_INFO_GHOST": {
         "EN": [
             "Upset that no one notices him, the Royal Ghost is determined to smash things up until he gets the recognition he deserves. He's so unnoticeable that even Walls won't hold him back!"
         ]
     },
     "TID_CHARACTER_INFO_GIANT": {
         "EN": [
-            "These big guys may seem calm, but show them a Turret or Cannon and you\u00b4ll see their fury unleashed! Slow yet durable, these warriors are best used to soak up hits."
+            "These big guys may seem calm, but show them a Cannon or Archer Tower and you\u00b4ll see their fury unleashed! Slow yet durable, these warriors are best used to soak up hits."
         ]
     },
     "TID_CHARACTER_INFO_GIANT_SHORT": {
         "EN": [
             "These big, tough guys just wanna smash defenses!"
         ]
     },
@@ -9700,14 +9795,19 @@
         ]
     },
     "TID_CHARACTER_INFO_ROCKET_BALLOONS": {
         "EN": [
             "When terrain is working against you, a swarm of Rocket Balloons can probably get the job done... if their boosters don't run out first."
         ]
     },
+    "TID_CHARACTER_INFO_SIDE_THROWER": {
+        "EN": [
+            "This big budding sportsman throws a heavy bouncing ball at the nearest Building. Then he moves on to the typical Giant smashing!"
+        ]
+    },
     "TID_CHARACTER_INFO_SIEGE_CART": {
         "EN": [
             "A Cannon on wheels?! Bet they won't see that coming! Tons of fire-power, but not that sturdy!"
         ]
     },
     "TID_CHARACTER_INFO_SIEGE_MACHINE_CARRIER": {
         "EN": [
@@ -9767,15 +9867,15 @@
     "TID_CHARACTER_INFO_SIEGE_MACHINE_RAM_SHORT": {
         "EN": [
             "Breaks a path right through to the Town Hall."
         ]
     },
     "TID_CHARACTER_INFO_SIEGE_MACHINE_TROOP_CATAPULT": {
         "EN": [
-            "Flings your Siege Machine troops"
+            "WIP Flings your Siege Machine troops"
         ]
     },
     "TID_CHARACTER_INFO_SKELETON": {
         "EN": [
             "This undead creature poses little threat by itself. But it never fights alone, since the Witch can summon an endless horde of Skeletons against your enemy!"
         ]
     },
@@ -10000,14 +10100,29 @@
         ]
     },
     "TID_CHARACTER_RIDERLESS_HOG_INFO": {
         "EN": [
             "Without its Rider, the Hog jumps over Walls and attacks defenses. So, what's the Rider even there for, in the first place?"
         ]
     },
+    "TID_CHARACTER_SHAPESHIFTER_DRUID": {
+        "EN": [
+            "WIP Shapeshifter Druid"
+        ]
+    },
+    "TID_CHARACTER_SHAPESHIFTER_DRUID_INFO": {
+        "EN": [
+            "WIP Starts as a ground healer and switche to another troops after some time."
+        ]
+    },
+    "TID_CHARACTER_SIDE_THROWER": {
+        "EN": [
+            "Giant Thrower"
+        ]
+    },
     "TID_CHARACTER_SIEGE_BATTLE_DRILL": {
         "EN": [
             "Battle Drill"
         ]
     },
     "TID_CHARACTER_SIEGE_BATTLE_DRILL_INFO": {
         "EN": [
@@ -10022,15 +10137,15 @@
     "TID_CHARACTER_SIEGE_MACHINE_CATAPULT": {
         "EN": [
             "Flame Flinger"
         ]
     },
     "TID_CHARACTER_SIEGE_MACHINE_TROOP_CATAPULT": {
         "EN": [
-            "Troop Catapult Prototype"
+            "WIP Troop Catapult Prototype"
         ]
     },
     "TID_CHARACTER_SKELETON_BARREL": {
         "EN": [
             "Skeleton Barrel"
         ]
     },
@@ -10115,14 +10230,34 @@
         ]
     },
     "TID_CHAT_BUTTON_REMOVE_PIN": {
         "EN": [
             "Unpin"
         ]
     },
+    "TID_CHAT_ENTRY_WAR_SIGNUP_INFO": {
+        "EN": [
+            "<cffffff>Sign up for the upcoming Clan War?</c>"
+        ]
+    },
+    "TID_CHAT_ENTRY_WAR_SIGNUP_NO": {
+        "EN": [
+            "<cff6266>You\u2019ve opted out from the next Clan War</c>"
+        ]
+    },
+    "TID_CHAT_ENTRY_WAR_SIGNUP_TITLE": {
+        "EN": [
+            "Clan War Sign-Up"
+        ]
+    },
+    "TID_CHAT_ENTRY_WAR_SIGNUP_YES": {
+        "EN": [
+            "<c6cd900>You\u2019ve opted in for the next Clan War</c>"
+        ]
+    },
     "TID_CHAT_ERROR_INVALID_TAGS": {
         "EN": [
             "You used invalid tags. Please try again."
         ]
     },
     "TID_CHAT_ERROR_MESSAGE": {
         "EN": [
@@ -10290,14 +10425,19 @@
         ]
     },
     "TID_CHESS_QUEEN": {
         "EN": [
             "Chess Queen"
         ]
     },
+    "TID_CHIEFSJOURNEY_HUB_TEXT": {
+        "EN": [
+            "View <cffcc33>Chief's Journey</c> to see what you\u2019ve unlocked"
+        ]
+    },
     "TID_CHIEFS_JOURNEY": {
         "EN": [
             "Chief's Journey"
         ]
     },
     "TID_CHINA_REAL_NAME_REGULATION": {
         "EN": [
@@ -11633,14 +11773,29 @@
         ]
     },
     "TID_CLANGAMES_TASK_USE_ELECTROFIREWIZARD": {
         "EN": [
             "Electrofire Crackle"
         ]
     },
+    "TID_CLANGAMES_TASK_USE_EQUIPMENT": {
+        "EN": [
+            "Earn a Star in <num>x Multiplayer Battles using <equipment>."
+        ]
+    },
+    "TID_CLANGAMES_TASK_USE_EQUIPMENT_FOOTBALL": {
+        "EN": [
+            "Hat Trick!"
+        ]
+    },
+    "TID_CLANGAMES_TASK_USE_FREE_KICKERS": {
+        "EN": [
+            "Kicker Kickoff"
+        ]
+    },
     "TID_CLANGAMES_TASK_USE_GIANTS": {
         "EN": [
             "Giant Opportunity"
         ]
     },
     "TID_CLANGAMES_TASK_USE_GOBLINS": {
         "EN": [
@@ -12008,15 +12163,15 @@
     "TID_CLANPERK_DESC_DONATION_LIMIT": {
         "EN": [
             "Donation limit:"
         ]
     },
     "TID_CLANPERK_DESC_DONATION_LIMIT_VALUE": {
         "EN": [
-            "<troops> Troops, <spells> Spells"
+            "<troops> Troops, <spells> Spells, <sieges> Siege Machines"
         ]
     },
     "TID_CLANPERK_DESC_DONATION_LIMIT_VALUE_SINGLE_SPELL": {
         "EN": [
             "<troops> troops, 1 spell"
         ]
     },
@@ -13606,14 +13761,19 @@
         ]
     },
     "TID_DAILY_BONUS_LIMIT_REACHED": {
         "EN": [
             "Daily loot limit reached"
         ]
     },
+    "TID_DAILY_LOGIN_HUB_TEXT": {
+        "EN": [
+            "Check out the <cffcc33>Login Calendar</c> for daily rewards"
+        ]
+    },
     "TID_DAILY_LOOT_LIMIT_FILLED": {
         "EN": [
             "Daily Loot Limit Reached"
         ]
     },
     "TID_DAILY_LOOT_LIMIT_FULL_INFO": {
         "EN": [
@@ -14051,14 +14211,45 @@
         ]
     },
     "TID_DECO_CAP_REACHED": {
         "EN": [
             "You've already built the maximum amount of these decorations."
         ]
     },
+    "TID_DECO_CLASHBALL_GOAL": {
+        "EN": [
+            "WIP: Goal"
+        ]
+    },
+    "TID_DECO_CLASHBALL_GOLDENBOOT": {
+        "EN": [
+            "Golden Boot"
+        ]
+    },
+    "TID_DECO_CLASHBALL_STATUECHARACTER": {
+        "EN": []
+    },
+    "TID_DECO_CLASHBALL_TROPHYBALL": {
+        "EN": [
+            "Bestest Ball"
+        ]
+    },
+    "TID_DECO_CLASHBALL_TROPHYBEVERAGE": {
+        "EN": []
+    },
+    "TID_DECO_CLASHBALL_TROPHYCROWN": {
+        "EN": [
+            "Triumphant Trophy"
+        ]
+    },
+    "TID_DECO_CLASHBALL_TROPHYCUP": {
+        "EN": [
+            "Celebration Cup"
+        ]
+    },
     "TID_DECO_CLOWN": {
         "EN": [
             "\\qFriendly\\q Clown"
         ]
     },
     "TID_DECO_COFFIN": {
         "EN": [
@@ -14156,14 +14347,22 @@
         ]
     },
     "TID_DECO_FOREST_3": {
         "EN": [
             "Forest"
         ]
     },
+    "TID_DECO_GAME_CAMPAIGN": {
+        "EN": []
+    },
+    "TID_DECO_GIFT_2024_CROWNSWORD": {
+        "EN": [
+            "Crown Sword"
+        ]
+    },
     "TID_DECO_GINGERBREAD_BUILDING": {
         "EN": [
             "Gingerbread Bakery"
         ]
     },
     "TID_DECO_GOBLIN_BARREL": {
         "EN": [
@@ -14436,14 +14635,29 @@
         ]
     },
     "TID_DECO_TH14_FOUNTAIN": {
         "EN": [
             "Flowing Fountain"
         ]
     },
+    "TID_DECO_WILDWEST_CACTUS": {
+        "EN": [
+            "Cactus Guy"
+        ]
+    },
+    "TID_DECO_WILDWEST_SKELLY": {
+        "EN": [
+            "Cowboy Skeleton"
+        ]
+    },
+    "TID_DECO_WILDWEST_TOTEM": {
+        "EN": [
+            "Dragon Totem"
+        ]
+    },
     "TID_DEFAULT_VILLAGE_NAME": {
         "EN": [
             "<name>'s Village"
         ]
     },
     "TID_DEFEAT": {
         "EN": [
@@ -14486,14 +14700,19 @@
         ]
     },
     "TID_DELETE_ACCOUNT_TITLE": {
         "EN": [
             "Delete Account"
         ]
     },
+    "TID_DELETE_BUTTON": {
+        "EN": [
+            "Remove"
+        ]
+    },
     "TID_DEMOTED_TO_TEXT": {
         "EN": [
             "Demoted to"
         ]
     },
     "TID_DEMOTE_POPUP_TITLE": {
         "EN": [
@@ -15861,14 +16080,19 @@
         ]
     },
     "TID_EDIT_CAPITAL_ARMY": {
         "EN": [
             "Change Capital Army"
         ]
     },
+    "TID_EDIT_CLAN_NOTICE_TITLE": {
+        "EN": [
+            "Edit Clan Notice"
+        ]
+    },
     "TID_EDIT_MODE_BLOCKED": {
         "EN": [
             "Buildings blocked by obstacles have been moved to your inventory"
         ]
     },
     "TID_EDIT_MODE_BLOCKED_COPY": {
         "EN": [
@@ -15966,14 +16190,34 @@
         ]
     },
     "TID_EFFECT_TIME": {
         "EN": [
             "Effect duration: <number> Seconds"
         ]
     },
+    "TID_EGYPTIAN_CHAMPION": {
+        "EN": [
+            "Egypt Champion"
+        ]
+    },
+    "TID_EGYPTIAN_QUEEN": {
+        "EN": [
+            "Egypt Queen"
+        ]
+    },
+    "TID_EGYPTIAN_WARDEN": {
+        "EN": [
+            "Egypt Warden"
+        ]
+    },
+    "TID_EGYPT_KING": {
+        "EN": [
+            "Egypt King"
+        ]
+    },
     "TID_ELDER_KICK_FAIL_COOLDOWN": {
         "EN": [
             "You have recently kicked a clan member. Try again in <time>."
         ]
     },
     "TID_ELECTROFIRE_WIZARD": {
         "EN": [
@@ -16171,19 +16415,39 @@
         ]
     },
     "TID_EP_RECEIVED": {
         "EN": [
             "Event Pass received!"
         ]
     },
+    "TID_EP_RESOURCE_REWARD_GET_GEM_ALTERNATIVE_NO_BLACKSMITH_TEXT": {
+        "EN": [
+            "Build Blacksmith in order to store <resource>.\\nSell for <amount> Gems instead?"
+        ]
+    },
+    "TID_EP_RESOURCE_REWARD_GET_GEM_ALTERNATIVE_NO_BLACKSMITH_TITLE": {
+        "EN": [
+            "No Storage"
+        ]
+    },
     "TID_EP_RESOURCE_REWARD_GET_GEM_ALTERNATIVE_TEXT": {
         "EN": [
             "Your storage cannot fit all of the <resource>.\\nSell the extra for <amount> Gems?"
         ]
     },
+    "TID_EP_RESOURCE_REWARD_GET_GEM_ALTERNATIVE_TOO_LOW_TH_TEXT": {
+        "EN": [
+            "<resource> can be stored after building Blacksmith on Town Hall 8.\\nSell for <amount> Gems instead?"
+        ]
+    },
+    "TID_EP_RESOURCE_REWARD_GET_GEM_ALTERNATIVE_TOO_LOW_TH_TITLE": {
+        "EN": [
+            "No Storage"
+        ]
+    },
     "TID_EP_REWARD_CLAIMED": {
         "EN": [
             "You collected this reward already."
         ]
     },
     "TID_EP_REWARD_GET_GEM_ALTERNATIVE_TITLE": {
         "EN": [
@@ -16486,14 +16750,19 @@
         ]
     },
     "TID_ERROR_POP_UP_WRONG_CLIENT_VERSION_TITLE": {
         "EN": [
             "Update is available!"
         ]
     },
+    "TID_EVENTS_HUB_TEXT": {
+        "EN": [
+            "Check our <cffcc33>Events</c> for more fun and rewards"
+        ]
+    },
     "TID_EVENT_ACHIEVEMENT_BOOSTER_GEM_XP_REWARD_CLAIMED": {
         "EN": [
             "Event completed! You received <gem> Gems, <number>x <booster> and <xp> XP!"
         ]
     },
     "TID_EVENT_ACHIEVEMENT_BOOSTER_XP_REWARD_CLAIMED": {
         "EN": [
@@ -16944,14 +17213,24 @@
         ]
     },
     "TID_EVENT_TRACK_REWARD_INFO_SPELL_NOT_AVAILABLE": {
         "EN": [
             "Temporary Spells are no longer available"
         ]
     },
+    "TID_EVENT_TRACK_REWARD_INFO_SUPER_TROOP": {
+        "EN": [
+            "Activate <name> for free!"
+        ]
+    },
+    "TID_EVENT_TRACK_REWARD_INFO_SUPER_TROOP_BOOSTED": {
+        "EN": [
+            "Activate <name> for free!\\nTraining time shortened by <pct>%."
+        ]
+    },
     "TID_EVENT_TRACK_REWARD_INFO_SUPER_TROOP_NOT_AVAILABLE": {
         "EN": [
             "Free Super Troop is no longer available"
         ]
     },
     "TID_EVENT_TROOP": {
         "EN": [
@@ -17689,24 +17968,54 @@
         ]
     },
     "TID_GEAR_ANGRY_TOME": {
         "EN": [
             "Rage Gem"
         ]
     },
+    "TID_GEAR_BARBARIAN_CROWN_GIVEN_ABILITY": {
+        "EN": [
+            "Rage"
+        ]
+    },
+    "TID_GEAR_CLONING_CLOAK_GIVEN_ABILITY": {
+        "EN": [
+            "Clone"
+        ]
+    },
     "TID_GEAR_EARTHQUAKE_BOOTS": {
         "EN": [
             "Earthquake Boots"
         ]
     },
     "TID_GEAR_FIRE_IN_A_CAN": {
         "EN": [
             "Fireball"
         ]
     },
+    "TID_GEAR_FOOTBALL_BOUNCE": {
+        "EN": [
+            "WIP: Townhall Bounce"
+        ]
+    },
+    "TID_GEAR_FOOTBALL_BOUNCE_INFO": {
+        "EN": [
+            "WIP: Football that targets Town Hall then defenses"
+        ]
+    },
+    "TID_GEAR_FOOTBALL_STRIKE": {
+        "EN": [
+            "WIP: Townhall Strike"
+        ]
+    },
+    "TID_GEAR_FOOTBALL_STRIKE_INFO": {
+        "EN": [
+            "WIP: Piercing football that targets Town Hall, causing damage on the way"
+        ]
+    },
     "TID_GEAR_FROZEN_ARROW": {
         "EN": [
             "Frozen Arrow"
         ]
     },
     "TID_GEAR_GIANT_GAUNTLET": {
         "EN": [
@@ -17744,14 +18053,19 @@
         ]
     },
     "TID_GEAR_INFO_BARBARIAN_CROWN": {
         "EN": [
             "Summons a pack of raged Barbarians"
         ]
     },
+    "TID_GEAR_INFO_CLONING_CLOAK": {
+        "EN": [
+            "Summons clones of the Archer Queen"
+        ]
+    },
     "TID_GEAR_INFO_EARTHQUAKE_BOOTS": {
         "EN": [
             "Causes a powerful earthquake which destroys Walls and damages Buildings"
         ]
     },
     "TID_GEAR_INFO_ETERNAL_TOME": {
         "EN": [
@@ -17759,14 +18073,19 @@
         ]
     },
     "TID_GEAR_INFO_FIRE_IN_A_CAN": {
         "EN": [
             "Throws a giant exploding fireball at the closest defense."
         ]
     },
+    "TID_GEAR_INFO_FOOTBALL": {
+        "EN": [
+            "Shoots a Spiky Ball which smashes between buildings"
+        ]
+    },
     "TID_GEAR_INFO_FROZEN_ARROW": {
         "EN": [
             "Icy arrows slow down the targets they hit"
         ]
     },
     "TID_GEAR_INFO_GIANT_GAUNTLET": {
         "EN": [
@@ -17799,14 +18118,34 @@
         ]
     },
     "TID_GEAR_INFO_LIFE_GEM": {
         "EN": [
             "Nearby friendly units gain extra hitpoints"
         ]
     },
+    "TID_GEAR_INFO_LIGHT_BOMB": {
+        "EN": [
+            "WIP Shoots a bomb of light that stuns a large area"
+        ]
+    },
+    "TID_GEAR_INFO_OLYMPIC_BATON": {
+        "EN": [
+            "WIP Troops that dies while close to the Olympic Baton stay alive for an extra <num> seconds before perishing"
+        ]
+    },
+    "TID_GEAR_INFO_OLYMPIC_TORCH": {
+        "EN": [
+            "WIP Gives troops nearby Jump, increased move speed and reduced damage taken for <num> seconds"
+        ]
+    },
+    "TID_GEAR_INFO_OLYMPIC_TORCH_GIVEN_ABILITY": {
+        "EN": [
+            "WIP The troop is able to jump over walls for the next <num> seconds"
+        ]
+    },
     "TID_GEAR_INFO_PIERCING_ARROW": {
         "EN": [
             "Shoots a giant piercing arrow that crosses the entire village"
         ]
     },
     "TID_GEAR_INFO_PROTECTIVE_CLOAK": {
         "EN": [
@@ -17824,14 +18163,19 @@
         ]
     },
     "TID_GEAR_INFO_SEEKING_SHIELD": {
         "EN": [
             "Throws her shield which bounces between defenses, dealing damage"
         ]
     },
+    "TID_GEAR_INFO_SUPER_ARCHER_PUPPET": {
+        "EN": [
+            "WIP Summons a regiment of Super Archers"
+        ]
+    },
     "TID_GEAR_INFO_VAMPSTACHE": {
         "EN": [
             "Every time the Barbarian King attacks, he heals himself"
         ]
     },
     "TID_GEAR_PIERCING_ARROW": {
         "EN": [
@@ -17924,19 +18268,29 @@
         ]
     },
     "TID_GEAR_TITLE_BARBARIAN_CROWN": {
         "EN": [
             "Barbarian Puppet"
         ]
     },
+    "TID_GEAR_TITLE_CLONING_CLOAK": {
+        "EN": [
+            "Magic Mirror"
+        ]
+    },
     "TID_GEAR_TITLE_ETERNAL_TOME": {
         "EN": [
             "Eternal Tome"
         ]
     },
+    "TID_GEAR_TITLE_FOOTBALL": {
+        "EN": [
+            "Spiky Ball"
+        ]
+    },
     "TID_GEAR_TITLE_HASTE_VIAL": {
         "EN": [
             "Haste Vial"
         ]
     },
     "TID_GEAR_TITLE_IRON_FIST": {
         "EN": [
@@ -17944,24 +18298,49 @@
         ]
     },
     "TID_GEAR_TITLE_LIFE_GEM": {
         "EN": [
             "Life Gem"
         ]
     },
+    "TID_GEAR_TITLE_LIGHT_BOMB": {
+        "EN": [
+            "WIP Light Bomb"
+        ]
+    },
+    "TID_GEAR_TITLE_OLYMPIC_BATON": {
+        "EN": [
+            "WIP Olympic Baton"
+        ]
+    },
+    "TID_GEAR_TITLE_OLYMPIC_TORCH": {
+        "EN": [
+            "WIP Olympic Torch"
+        ]
+    },
+    "TID_GEAR_TITLE_OLYMPIC_TORCH_GIVEN_ABILITY": {
+        "EN": [
+            "WIP Olympic Jumper"
+        ]
+    },
     "TID_GEAR_TITLE_ROYAL_CLOAK": {
         "EN": [
             "Invisibility Vial"
         ]
     },
     "TID_GEAR_TITLE_SEEKING_SHIELD": {
         "EN": [
             "Seeking Shield"
         ]
     },
+    "TID_GEAR_TITLE_SUPER_ARCHER_PUPPET": {
+        "EN": [
+            "WIP Super Archer Puppet"
+        ]
+    },
     "TID_GEAR_TYPE_OTHER": {
         "EN": [
             "Other"
         ]
     },
     "TID_GEAR_TYPE_POTION": {
         "EN": [
@@ -18204,14 +18583,29 @@
         ]
     },
     "TID_GINGERBREAD_WARDEN": {
         "EN": [
             "Gingerbread Warden"
         ]
     },
+    "TID_GIVEN_ABILITY_BOOST_DAMAGE_PERCENTAGE": {
+        "EN": [
+            "<ability> damage increase: <number>%"
+        ]
+    },
+    "TID_GIVEN_ABILITY_DURATION": {
+        "EN": [
+            "<ability> duration: Seconds"
+        ]
+    },
+    "TID_GIVEN_ABILITY_NERF_DAMAGE_PERCENTAGE": {
+        "EN": [
+            "<ability> damage decreased to: <number>%"
+        ]
+    },
     "TID_GIVE_NAME_TITLE": {
         "EN": [
             "My name is..."
         ]
     },
     "TID_GLADIATOR_CHAMPION": {
         "EN": [
@@ -18785,14 +19179,29 @@
         ]
     },
     "TID_HERO_ABILITY_BATTLE_COPTER_DESC": {
         "EN": [
             "The Battle Copter rushes towards its target and throws a powerful bomb at it. One satisfying big bang later, the target and everything close to it will be a lot less together. Charge it up to increase the bomb\u00b4s area of damage!"
         ]
     },
+    "TID_HERO_ABILITY_CLONE_DAMAGE": {
+        "EN": [
+            "Clone damage: <number>"
+        ]
+    },
+    "TID_HERO_ABILITY_CLONE_DPS": {
+        "EN": [
+            "Clone DPS: <number>"
+        ]
+    },
+    "TID_HERO_ABILITY_CLONE_HEALTH": {
+        "EN": [
+            "Clone health: <number>"
+        ]
+    },
     "TID_HERO_ABILITY_COOLDOWN_ACTIVE": {
         "EN": [
             "You need to wait before using the hero ability again!"
         ]
     },
     "TID_HERO_ABILITY_DURATION": {
         "EN": [
@@ -18810,14 +19219,19 @@
         ]
     },
     "TID_HERO_ABILITY_LEVEL_UNLOCK_PROMPT": {
         "EN": [
             "Ability unlocks at level <number>!"
         ]
     },
+    "TID_HERO_ABILITY_NUM_CLONES": {
+        "EN": [
+            "Clones: <number>"
+        ]
+    },
     "TID_HERO_ABILITY_NUM_SUMMONED_UNITS": {
         "EN": [
             "Summoned units: <number>"
         ]
     },
     "TID_HERO_ABILITY_QUEEN_DESC": {
         "EN": [
@@ -18840,14 +19254,29 @@
         ]
     },
     "TID_HERO_ABILITY_SUMMONED_TROOP_TYPE": {
         "EN": [
             "Summoned unit:"
         ]
     },
+    "TID_HERO_ABILITY_SUMMONED_UNITS_DAMAGE": {
+        "EN": [
+            "Summoned units damage: <number>"
+        ]
+    },
+    "TID_HERO_ABILITY_SUMMONED_UNITS_DPS": {
+        "EN": [
+            "Summoned units DPS: <number>"
+        ]
+    },
+    "TID_HERO_ABILITY_SUMMONED_UNITS_HEALTH": {
+        "EN": [
+            "Summoned units health: <number>"
+        ]
+    },
     "TID_HERO_ABILITY_SUMMONED_UNITS_LEVEL": {
         "EN": [
             "Summoned units level: <number>"
         ]
     },
     "TID_HERO_ABILITY_TIME": {
         "EN": [
@@ -19292,15 +19721,15 @@
     "TID_HINT_DEFENSE": {
         "EN": [
             "Building good defenses is just as important as aggressive attacking"
         ]
     },
     "TID_HINT_DPS": {
         "EN": [
-            "The Damage statistic in unit and turret info is measured as Damage Per Second."
+            "The Damage statistic in Unit and Defense info is measured as Damage Per Second."
         ]
     },
     "TID_HINT_DRAGON_AIR": {
         "EN": [
             "The Dragon is a mighty flying unit that can attack both ground and air targets"
         ]
     },
@@ -20275,19 +20704,29 @@
         ]
     },
     "TID_INFO_TARGET_TYPE_AIR": {
         "EN": [
             "Air"
         ]
     },
+    "TID_INFO_TARGET_TYPE_BUILDINGS": {
+        "EN": [
+            "Buildings"
+        ]
+    },
     "TID_INFO_TARGET_TYPE_BUILDINGS_AND_WALLS": {
         "EN": [
             "Buildings & Walls"
         ]
     },
+    "TID_INFO_TARGET_TYPE_DEFENSES_AND_HEROES": {
+        "EN": [
+            "Defenses and Heroes"
+        ]
+    },
     "TID_INFO_TARGET_TYPE_GROUND": {
         "EN": [
             "Ground"
         ]
     },
     "TID_INFO_TARGET_TYPE_GROUND_AND_AIR": {
         "EN": [
@@ -20470,14 +20909,19 @@
         ]
     },
     "TID_JOINALLIANCEQUESTION": {
         "EN": [
             "Accept Clan invitation?"
         ]
     },
+    "TID_JOINCLAN_HUB_TEXT": {
+        "EN": [
+            "<cffcc33>Join a Clan</c> and play with others for even more fun"
+        ]
+    },
     "TID_JOINQUESTION": {
         "EN": [
             "Want to join?"
         ]
     },
     "TID_JOIN_ALLIANCE_TAB": {
         "EN": [
@@ -20755,14 +21199,19 @@
         ]
     },
     "TID_LABORATORY_HINT2": {
         "EN": [
             "Swipe the screen to see the whole list of upgrades"
         ]
     },
+    "TID_LABORATORY_HUB_TEXT": {
+        "EN": [
+            "Enjoy your <cffcc33>Research Boost</c>"
+        ]
+    },
     "TID_LABORATORY_INFO": {
         "EN": [
             "What dark secrets do these Wizards hide inside their Laboratory? Nobody has dared to look. All we know is that their research makes our Spells and Troops harder, better, faster and stronger!"
         ]
     },
     "TID_LABORATORY_UPGRADING": {
         "EN": [
@@ -22854,14 +23303,19 @@
         ]
     },
     "TID_LOOT": {
         "EN": [
             "You lost resources:"
         ]
     },
+    "TID_LOOTCART_HUB_TEXT": {
+        "EN": [
+            "Collect <cffcc33>Bonus Loot</c> and start upgrading your Village"
+        ]
+    },
     "TID_LOOT_AVAILABLE": {
         "EN": [
             "Loot Available:"
         ]
     },
     "TID_LOOT_CART": {
         "EN": [
@@ -23129,14 +23583,24 @@
         ]
     },
     "TID_MAP_LOCATION_9": {
         "EN": [
             "Sour Lake"
         ]
     },
+    "TID_MASS_TAG_CLAN": {
+        "EN": [
+            "clan"
+        ]
+    },
+    "TID_MASS_TAG_LEADERS": {
+        "EN": [
+            "leaders"
+        ]
+    },
     "TID_MASTER_BUILDER'S_RETURN": {
         "EN": [
             "Master Builder's Return"
         ]
     },
     "TID_MASTER_BUILDER_BUILDING": {
         "EN": [
@@ -23221,15 +23685,15 @@
     "TID_MEDAL_EVENT_HARD_CURRENCY": {
         "EN": [
             "Medal Event Hard Currency"
         ]
     },
     "TID_MEDAL_EVENT_INFO_TRACK_ENDED": {
         "EN": [
-            "<soft_currency> is gone, but there's still time to claim rewards and spend your <hard_currency> at the Trader!"
+            "Progress can be earned no more, but there's still time to claim rewards and spend your <hard_currency> at the Trader!"
         ]
     },
     "TID_MEDAL_EVENT_SOFT_CURRENCY": {
         "EN": [
             "Medal Event Soft Currency"
         ]
     },
@@ -23299,14 +23763,29 @@
         ]
     },
     "TID_MERGE_REQUIREMENTS": {
         "EN": [
             "Requirements:"
         ]
     },
+    "TID_MESSAGE_INFO_WAR_SIGNUP_ACTIVE": {
+        "EN": [
+            "You already have an active War Sign-up in the Chat."
+        ]
+    },
+    "TID_MESSAGE_WAR_SIGNUP_CONFIRM": {
+        "EN": [
+            "Send a War Sign-up to the Clan Chat?"
+        ]
+    },
+    "TID_MESSAGE_WAR_SIGNUP_CONFIRM_TITLE": {
+        "EN": [
+            "Send War Sign-up?"
+        ]
+    },
     "TID_ME_BONUS_POINTS_INFO": {
         "EN": [
             "Gain <num> <soft_currency> by purchasing the Event Pass!"
         ]
     },
     "TID_ME_BONUS_POINTS_TITLE": {
         "EN": [
@@ -23799,14 +24278,19 @@
         ]
     },
     "TID_NEED_TO_GIVE_WL_BONUSES": {
         "EN": [
             "You need to give out War League bonus medals before you can start a war."
         ]
     },
+    "TID_NERF_DAMAGE_PERCENTAGE": {
+        "EN": [
+            "Damage decreased to: <number>%"
+        ]
+    },
     "TID_NEW": {
         "EN": [
             "New"
         ]
     },
     "TID_NEWS_ACCOUNT_TRANSFER": {
         "EN": [
@@ -24352,14 +24836,29 @@
         ]
     },
     "TID_NOTHING_TO_PASTE": {
         "EN": [
             "Nothing to paste"
         ]
     },
+    "TID_NOTICE_BOARD_FTUE_ACTIVITY": {
+        "EN": [
+            "WIP: Clan Activity"
+        ]
+    },
+    "TID_NOTICE_BOARD_FTUE_SUBTEXT": {
+        "EN": [
+            "You can still change these settings later"
+        ]
+    },
+    "TID_NOTICE_BOARD_FTUE_TITLE": {
+        "EN": [
+            "Hey Chief! Let\u2019s find the best possible Clan for you by selecting a few quick preferences first!"
+        ]
+    },
     "TID_NOTIFICATION_ARMY": {
         "EN": [
             "Army"
         ]
     },
     "TID_NOTIFICATION_BUILDER_IS_BACK": {
         "EN": [
@@ -24560,14 +25059,19 @@
         ]
     },
     "TID_NO_FRIENDLY_ARMY": {
         "EN": [
             "You need to create Friendly Army first."
         ]
     },
+    "TID_NO_MATCHING_RESULTS_FOUND": {
+        "EN": [
+            "No matching results found"
+        ]
+    },
     "TID_NO_MESSAGES": {
         "EN": [
             "No new messages currently"
         ]
     },
     "TID_NO_MESSAGES_TEXT": {
         "EN": [
@@ -26460,14 +26964,19 @@
         ]
     },
     "TID_OFFER_TITLE_GENERIC": {
         "EN": [
             "Special Offer"
         ]
     },
+    "TID_OFFER_TOWNHALL_UPGRADE_PACK": {
+        "EN": [
+            "Townhall <num> Pack now available in the Shop!"
+        ]
+    },
     "TID_OFTHENORTH_BATTLE_MACHINE": {
         "EN": [
             "Battle Machine of the North"
         ]
     },
     "TID_ONGOING_EVENTS": {
         "EN": [
@@ -26790,14 +27299,19 @@
         ]
     },
     "TID_PETS_FEATURE_DESCRIPTION": {
         "EN": [
             "Help your Heroes in attacks by giving them a mighty, magical companion!"
         ]
     },
+    "TID_PET_ABILITY_ANGRY_JELLY": {
+        "EN": [
+            "Brainwash"
+        ]
+    },
     "TID_PET_ABILITY_BARKY": {
         "EN": [
             "High Jumper"
         ]
     },
     "TID_PET_ABILITY_BULLDOZER": {
         "EN": [
@@ -26805,14 +27319,19 @@
         ]
     },
     "TID_PET_ABILITY_ELECTROWL": {
         "EN": [
             "High Voltage"
         ]
     },
+    "TID_PET_ABILITY_INFO_ANGRY_JELLY": {
+        "EN": [
+            "Its Hero targets Defenses for a while after deployment."
+        ]
+    },
     "TID_PET_ABILITY_INFO_BARKY": {
         "EN": [
             "L.A.S.S.I can jump over Walls to attack targets on the other side."
         ]
     },
     "TID_PET_ABILITY_INFO_BULLDOZER": {
         "EN": [
@@ -26845,14 +27364,24 @@
         ]
     },
     "TID_PET_ALREADY_AT_MAX_LEVEL": {
         "EN": [
             "Pet is already at maximum level!"
         ]
     },
+    "TID_PET_ANGRY_JELLY": {
+        "EN": [
+            "Angry Jelly"
+        ]
+    },
+    "TID_PET_ANGRY_JELLY_INFO": {
+        "EN": [
+            "This blob of pure anger gets impatient waiting around the Village, it's hungry for a good fight. During Battle it convinces its Hero to attack Defenses before splitting to fight separately."
+        ]
+    },
     "TID_PET_DESCRIPTION": {
         "EN": [
             "Mighty companions for the mightiest Heroes!"
         ]
     },
     "TID_PET_DIGGY": {
         "EN": [
@@ -28085,14 +28614,19 @@
         ]
     },
     "TID_POWER_BOOST_INFO": {
         "EN": [
             "Boost your Troops and Spells to the max allowed at your Town Hall level."
         ]
     },
+    "TID_PRACTICELEVELS_HUB_TEXT": {
+        "EN": [
+            "Replay <cffcc33>Practice Attacks</c> to sharpen your skills"
+        ]
+    },
     "TID_PRACTICE_MODE_UNLOCKS_LATER": {
         "EN": [
             "Practice mode unlocks at Town Hall 4"
         ]
     },
     "TID_PREFERRED_TARGET_ANY": {
         "EN": [
@@ -28582,15 +29116,15 @@
     "TID_PUSH_ATTACKED": {
         "EN": [
             "Your Village was raided by <attacker>!"
         ]
     },
     "TID_PUSH_CHAT_TAG": {
         "EN": [
-            "You were mentioned in Clan Chat"
+            "<name>, you have been mentioned in Clan Chat!"
         ]
     },
     "TID_PUSH_UNDER_ATTACK": {
         "EN": [
             "Your Village is being raided by <attacker>!"
         ]
     },
@@ -29090,14 +29624,19 @@
         ]
     },
     "TID_REENGAGEMENT_DAILYCALENDAR_2": {
         "EN": [
             "You'll get a reward each day you come back, Chief."
         ]
     },
+    "TID_REENGAGEMENT_HUB_TITLE": {
+        "EN": [
+            "Tutorial Hub"
+        ]
+    },
     "TID_REENGAGEMENT_INTRO_1": {
         "EN": [
             "Not a step closer!"
         ]
     },
     "TID_REENGAGEMENT_INTRO_2": {
         "EN": [
@@ -29985,14 +30524,19 @@
         ]
     },
     "TID_SCENERY_CHESS": {
         "EN": [
             "Chess Scenery"
         ]
     },
+    "TID_SCENERY_CLASHBALL": {
+        "EN": [
+            "WIP Football scenery"
+        ]
+    },
     "TID_SCENERY_CLASHY_CONSTRUCTS": {
         "EN": [
             "Clashy Constructs Scenery"
         ]
     },
     "TID_SCENERY_CLASSIC": {
         "EN": [
@@ -30005,14 +30549,19 @@
         ]
     },
     "TID_SCENERY_DESCRIPTION": {
         "EN": [
             "<scenery>"
         ]
     },
+    "TID_SCENERY_EGYPT": {
+        "EN": [
+            "WIP: Egypt"
+        ]
+    },
     "TID_SCENERY_EPIC_JUNGLE": {
         "EN": [
             "Epic Jungle Scenery"
         ]
     },
     "TID_SCENERY_EPIC_WINTER": {
         "EN": [
@@ -30060,14 +30609,19 @@
         ]
     },
     "TID_SCENERY_PIRATE": {
         "EN": [
             "Pirate Scenery"
         ]
     },
+    "TID_SCENERY_SPACE": {
+        "EN": [
+            "WIP-SPACE"
+        ]
+    },
     "TID_SCID_GIFT_ACCEPT_BUTTON": {
         "EN": [
             "Accept"
         ]
     },
     "TID_SCID_GIFT_DECLINE_BUTTON": {
         "EN": [
@@ -30897,20 +31451,20 @@
     "TID_SIEGE_MACHINE_FLYER": {
         "EN": [
             "Battle Blimp"
         ]
     },
     "TID_SIEGE_MACHINE_INVISIBLE": {
         "EN": [
-            "Invisible Machine"
+            "WIP Invisible Machine"
         ]
     },
     "TID_SIEGE_MACHINE_INVISIBLE_FLYING": {
         "EN": [
-            "Invisibility Drone"
+            "WIP Invisibility Drone"
         ]
     },
     "TID_SIEGE_MACHINE_LOG_LAUNCHER": {
         "EN": [
             "Log Launcher"
         ]
     },
@@ -31090,14 +31644,34 @@
         ]
     },
     "TID_SOUR_ELIXIR_LOOTED": {
         "EN": [
             "Sour Elixir:"
         ]
     },
+    "TID_SPACE_CHAMPION": {
+        "EN": [
+            "Space Champion"
+        ]
+    },
+    "TID_SPACE_KING": {
+        "EN": [
+            "Space King"
+        ]
+    },
+    "TID_SPACE_QUEEN": {
+        "EN": [
+            "Space Queen"
+        ]
+    },
+    "TID_SPACE_WARDEN": {
+        "EN": [
+            "Space Warden"
+        ]
+    },
     "TID_SPECIAL_OFFER": {
         "EN": [
             "Special Offer"
         ]
     },
     "TID_SPECIAL_OFFER_BUILDERBASE_ANNIVERSARY_ALLPRICEPOINTS": {
         "EN": [
@@ -31342,25 +31916,25 @@
     "TID_SPELL_FORGE_INFO": {
         "EN": [
             "The Spell Factory is home to veteran Wizards who are better suited to creating magical weapons than front-line combat. Use their powerful Attack Spells to turn the tide of battle in your favor!"
         ]
     },
     "TID_SPELL_FROST": {
         "EN": [
-            "Targeted Frost"
+            "WIP Targeted Frost"
         ]
     },
     "TID_SPELL_FROST_INFO": {
         "EN": [
             "WIP Applies frost in a small area for a long time, and does small damage in the area"
         ]
     },
     "TID_SPELL_HEAL_SPIRIT": {
         "EN": [
-            "Heal Spirit"
+            "WIP Heal Spirit"
         ]
     },
     "TID_SPELL_HEAL_SPIRIT_INFO": {
         "EN": [
             "WIP Summons a heal spirit that heavily heals a troop nearby."
         ]
     },
@@ -31372,15 +31946,15 @@
     "TID_SPELL_OVERGROWTH": {
         "EN": [
             "Overgrowth Spell"
         ]
     },
     "TID_SPELL_OVERGROWTH_INFO": {
         "EN": [
-            "Traps nearby Buildings in tough roots, stopping defenses attacking. Troops ignore trapped Buildings."
+            "Ever wish you could ignore a whole chunk of that enemy base? The Overgrowth Spell traps nearby Buildings in tough roots, stopping Defenses attacking. Troops ignore trapped Buildings."
         ]
     },
     "TID_SPELL_OVERGROWTH_INFO_SHORT": {
         "EN": [
             "Tangle the enemy up to take them down."
         ]
     },
@@ -31435,14 +32009,24 @@
         ]
     },
     "TID_SPELL_TIME": {
         "EN": [
             "Spell duration: <number> Seconds"
         ]
     },
+    "TID_SPELL_YELLOW_CARD": {
+        "EN": [
+            "Yellow Card"
+        ]
+    },
+    "TID_SPELL_YELLOW_CARD_INFO": {
+        "EN": [
+            "Bad sportsmanship deserves punishment and spoiling your attack is rude. Temporarily suspend the targeted Defense or Hero. They can't attack or be attacked while suspended."
+        ]
+    },
     "TID_SPOOKY2022_SCENERY": {
         "EN": [
             "Spooky Scenery"
         ]
     },
     "TID_SPOOKY_QUEEN": {
         "EN": [
@@ -32097,20 +32681,30 @@
     "TID_STREAK_COUNTER": {
         "EN": [
             "<num>/<max>"
         ]
     },
     "TID_STREAK_COUNTER_STREAKS": {
         "EN": [
-            "Streak"
+            "Progress"
         ]
     },
     "TID_STREAK_DESCRIPTION_TASK_BROKEN": {
         "EN": [
-            "Your Streak was broken! You can continue your Streak or reset it back to start."
+            "You broke your Streak! You can continue your Streak or start over."
+        ]
+    },
+    "TID_STREAK_EVENT_BANNER_TITLE": {
+        "EN": [
+            "Progress"
+        ]
+    },
+    "TID_STREAK_EVENT_BROKEN_TIMER": {
+        "EN": [
+            "Task failed: 0h 0m"
         ]
     },
     "TID_STREAK_EVENT_BUTTON_BOOSTS": {
         "EN": [
             "Boosts"
         ]
     },
@@ -32127,49 +32721,119 @@
     "TID_STREAK_EVENT_BUTTON_PURCHASE": {
         "EN": [
             "<TID_STREAK_EVENT_BUTTON_PURCHASE>"
         ]
     },
     "TID_STREAK_EVENT_BUTTON_RESET": {
         "EN": [
-            "Reset!"
+            "Start Over!"
         ]
     },
     "TID_STREAK_EVENT_BUTTON_RUSH": {
         "EN": [
-            "Rush!"
+            "Unlock!"
         ]
     },
     "TID_STREAK_EVENT_COMPLETE_CURRENT_TIER_TO_RUSH": {
         "EN": [
-            "Complete current task in order to rush"
+            "You need to complete the current task before you can rush"
+        ]
+    },
+    "TID_STREAK_EVENT_EXTRA_REWARD": {
+        "EN": [
+            "+<num>"
+        ]
+    },
+    "TID_STREAK_EVENT_FAILED": {
+        "EN": [
+            "Task Failed"
         ]
     },
     "TID_STREAK_EVENT_HUD_NOTIFICATION": {
         "EN": [
             "Task <num>/<max> completed!"
         ]
     },
+    "TID_STREAK_EVENT_INFO_SCREEN_1": {
+        "EN": [
+            "Complete a task every day within the given time limit to extend your Streak"
+        ]
+    },
+    "TID_STREAK_EVENT_INFO_SCREEN_2": {
+        "EN": [
+            "A longer Streak unlocks bigger League Bonus multipliers and other Rewards"
+        ]
+    },
+    "TID_STREAK_EVENT_INFO_SCREEN_3": {
+        "EN": [
+            "If you don't complete your task in time, start over or use Gems to retry the task"
+        ]
+    },
+    "TID_STREAK_EVENT_INFO_SCREEN_4": {
+        "EN": [
+            "Can't wait until the next task unlocks? Spend Gems to unlock it now."
+        ]
+    },
+    "TID_STREAK_EVENT_INFO_SCREEN_TITLE": {
+        "EN": [
+            "Streak Event"
+        ]
+    },
+    "TID_STREAK_EVENT_LEAGUE_BOOST": {
+        "EN": [
+            "Streak Bonus"
+        ]
+    },
+    "TID_STREAK_EVENT_LEAGUE_BOOST_DESCRIPTION": {
+        "EN": [
+            "Gain <num>% extra resources from your League loot bonus!"
+        ]
+    },
+    "TID_STREAK_EVENT_NOTIFICATION_STREAK_ADVANCED": {
+        "EN": [
+            "Task Completed!"
+        ]
+    },
+    "TID_STREAK_EVENT_NOTIFICATION_STREAK_BROKEN": {
+        "EN": [
+            "Streak Broken"
+        ]
+    },
+    "TID_STREAK_EVENT_NO_TIMER_YET": {
+        "EN": [
+            "Complete your first task to get started!"
+        ]
+    },
     "TID_STREAK_EVENT_PERK_LEAGUE_BOOST_INFO": {
         "EN": [
-            "With higher league boost, you can get bigger rewards for attacking!"
+            "With a bigger Streak Bonus, you'll get more Loot Bonus in Multiplayer Attacks!"
         ]
     },
     "TID_STREAK_EVENT_PERK_LEAGUE_BOOST_NAME": {
         "EN": [
-            "League boost"
+            "Streak Bonus"
         ]
     },
     "TID_STREAK_EVENT_PERK_LEAGUE_BOOST_TOPIC": {
         "EN": [
-            "League boost:"
+            "Streak Bonus:"
+        ]
+    },
+    "TID_STREAK_EVENT_REWARDS": {
+        "EN": [
+            "Rewards:"
         ]
     },
     "TID_STREAK_EVENT_REWARD_PERCENT": {
         "EN": [
+            "+<num>%"
+        ]
+    },
+    "TID_STREAK_EVENT_REWARD_PERCENT_TOTAL": {
+        "EN": [
             "<num>%"
         ]
     },
     "TID_STREAK_EVENT_RUSH_STREAK_BUTTON_CANCEL": {
         "EN": [
             "Cancel!"
         ]
@@ -32177,45 +32841,45 @@
     "TID_STREAK_EVENT_RUSH_STREAK_BUTTON_CONTINUE": {
         "EN": [
             "Rush!"
         ]
     },
     "TID_STREAK_EVENT_RUSH_STREAK_TEXT": {
         "EN": [
-            "You can unlock next tier of the Streak early!"
+            "Unlock the next tier of the Streak early?"
         ]
     },
     "TID_STREAK_EVENT_RUSH_STREAK_TITLE": {
         "EN": [
             "Rush your Streak!"
         ]
     },
     "TID_STREAK_EVENT_STREAK_BROKEN_BUTTON_BREAK": {
         "EN": [
-            "Reset!"
+            "Start Over!"
         ]
     },
     "TID_STREAK_EVENT_STREAK_BROKEN_BUTTON_CONTINUE": {
         "EN": [
             "Continue!"
         ]
     },
     "TID_STREAK_EVENT_STREAK_BROKEN_TEXT": {
         "EN": [
-            "You can continue your Streak or reset it back to start"
+            "You can continue your Streak or start over with a new one"
         ]
     },
     "TID_STREAK_EVENT_STREAK_BROKEN_TEXT_CONTINUE": {
         "EN": [
-            "Continue your Streak from where you left off"
+            "Continue your Streak from where you were or start over?"
         ]
     },
     "TID_STREAK_EVENT_STREAK_BROKEN_TEXT_RESET": {
         "EN": [
-            "Reset your Streak back to start"
+            "Start"
         ]
     },
     "TID_STREAK_EVENT_STREAK_BROKEN_TITLE": {
         "EN": [
             "Your Streak was broken!"
         ]
     },
@@ -32235,14 +32899,24 @@
         ]
     },
     "TID_STREAK_EVENT_TIME_LEFT": {
         "EN": [
             "Event ends in: <time>"
         ]
     },
+    "TID_STREAK_EVENT_TIME_REMAINING": {
+        "EN": [
+            "Time left: <time>"
+        ]
+    },
+    "TID_STREAK_TASK_REVEALED_IN": {
+        "EN": [
+            "Task <task> revealed in:"
+        ]
+    },
     "TID_STREAM_BUTTON_ATTACK": {
         "EN": [
             "Attack"
         ]
     },
     "TID_STREAM_BUTTON_FIND_CLAN": {
         "EN": [
@@ -32275,14 +32949,19 @@
         ]
     },
     "TID_STREAM_EVENT_ACCEPTED": {
         "EN": [
             "was accepted to the clan by <name>"
         ]
     },
+    "TID_STREAM_EVENT_ACCEPTED_NEW": {
+        "EN": [
+            "<player> was accepted to the clan by <name>"
+        ]
+    },
     "TID_STREAM_EVENT_ALLIANCE_LEVEL_UP": {
         "EN": [
             "Clan has reached level <value>! New perks unlocked:"
         ]
     },
     "TID_STREAM_EVENT_ALLIANCE_LEVEL_UP_NO_PERKS": {
         "EN": [
@@ -32290,39 +32969,64 @@
         ]
     },
     "TID_STREAM_EVENT_CANCELLED_ARRANGED_WAR": {
         "EN": [
             "cancelled Friendly War"
         ]
     },
+    "TID_STREAM_EVENT_CANCELLED_ARRANGED_WAR_NEW": {
+        "EN": [
+            "<player> cancelled Friendly War"
+        ]
+    },
     "TID_STREAM_EVENT_CANCELLED_WAR": {
         "EN": [
             "cancelled Clan War search"
         ]
     },
     "TID_STREAM_EVENT_CANCELLED_WAR_LEAGUE": {
         "EN": [
             "cancelled Clan War League search"
         ]
     },
+    "TID_STREAM_EVENT_CANCELLED_WAR_LEAGUE_NEW": {
+        "EN": [
+            "<player> cancelled Clan War League search"
+        ]
+    },
+    "TID_STREAM_EVENT_CANCELLED_WAR_NEW": {
+        "EN": [
+            "<player> cancelled Clan War search"
+        ]
+    },
     "TID_STREAM_EVENT_CHANGED_SETTINGS": {
         "EN": [
             "updated clan settings"
         ]
     },
+    "TID_STREAM_EVENT_CHANGED_SETTINGS_NEW": {
+        "EN": [
+            "<player> updated clan settings"
+        ]
+    },
     "TID_STREAM_EVENT_CHANGED_SETTINGS_PLAYERS_LEFT": {
         "EN": [
             "Clan settings were updated. Some players have left the Clan."
         ]
     },
     "TID_STREAM_EVENT_DEMOTED": {
         "EN": [
             "was demoted by <name>"
         ]
     },
+    "TID_STREAM_EVENT_DEMOTED_NEW": {
+        "EN": [
+            "<player> was demoted to <role> by <name>"
+        ]
+    },
     "TID_STREAM_EVENT_DISTRICT_LAYOUT_SCRAMBLED": {
         "EN": [
             "A Clan Capital layout has been reset due to inappropriate content"
         ]
     },
     "TID_STREAM_EVENT_JOINED": {
         "EN": [
@@ -32330,49 +33034,94 @@
         ]
     },
     "TID_STREAM_EVENT_JOINED_AND_LEFT": {
         "EN": [
             "joined and left the clan"
         ]
     },
+    "TID_STREAM_EVENT_JOINED_AND_LEFT_NEW": {
+        "EN": [
+            "<player> joined and left the clan"
+        ]
+    },
+    "TID_STREAM_EVENT_JOINED_NEW": {
+        "EN": [
+            "<player> joined the clan"
+        ]
+    },
     "TID_STREAM_EVENT_KICKED": {
         "EN": [
             "has been kicked out of the clan by <name>"
         ]
     },
+    "TID_STREAM_EVENT_KICKED_NEW": {
+        "EN": [
+            "<player> has been kicked out of the clan by <name>"
+        ]
+    },
     "TID_STREAM_EVENT_LEFT": {
         "EN": [
             "has left the clan"
         ]
     },
+    "TID_STREAM_EVENT_LEFT_NEW": {
+        "EN": [
+            "<player> has left the clan"
+        ]
+    },
     "TID_STREAM_EVENT_NAME_CHANGED": {
         "EN": [
             "Changed their name to <name>"
         ]
     },
+    "TID_STREAM_EVENT_NAME_CHANGED_NEW": {
+        "EN": [
+            "<player> changed their name to <name>"
+        ]
+    },
     "TID_STREAM_EVENT_PROMOTED": {
         "EN": [
             "was promoted by <name>"
         ]
     },
     "TID_STREAM_EVENT_PROMOTED_AUTOMATICALLY": {
         "EN": [
             "was promoted automatically"
         ]
     },
+    "TID_STREAM_EVENT_PROMOTED_AUTOMATICALLY_NEW": {
+        "EN": [
+            "<player> was promoted to <role> automatically"
+        ]
+    },
+    "TID_STREAM_EVENT_PROMOTED_NEW": {
+        "EN": [
+            "<player> was promoted to <role> by <name>"
+        ]
+    },
     "TID_STREAM_EVENT_STARTED_WAR": {
         "EN": [
             "started Clan War search"
         ]
     },
     "TID_STREAM_EVENT_STARTED_WAR_LEAGUE": {
         "EN": [
             "started Clan War League search"
         ]
     },
+    "TID_STREAM_EVENT_STARTED_WAR_LEAGUE_NEW": {
+        "EN": [
+            "<player> started Clan War League search"
+        ]
+    },
+    "TID_STREAM_EVENT_STARTED_WAR_NEW": {
+        "EN": [
+            "<player> started Clan War search"
+        ]
+    },
     "TID_STREAM_EVENT_WAR_NO_MATCH_FOUND": {
         "EN": [
             "No Clan War opponent found. Please try starting a war again."
         ]
     },
     "TID_STREAM_REPLAY_BUTTON": {
         "EN": [
@@ -33763,14 +34512,19 @@
         ]
     },
     "TID_TRAINING_FULL": {
         "EN": [
             "Queue is full!"
         ]
     },
+    "TID_TRAINING_HUB_TEXT": {
+        "EN": [
+            "Enjoy your <cffcc33>Training Boost</c> and battle away"
+        ]
+    },
     "TID_TRAINING_INFO": {
         "EN": [
             "Tap and hold down unit icon to train multiple troops."
         ]
     },
     "TID_TRAINING_INFO2": {
         "EN": [
@@ -34323,14 +35077,19 @@
         ]
     },
     "TID_TROPHIES": {
         "EN": [
             "Trophies:"
         ]
     },
+    "TID_TRYING_TO_TYPE_TOO_MANY_TAGS": {
+        "EN": [
+            "You can tag only up to <num> players per message"
+        ]
+    },
     "TID_TUTORIAL_ACHIEVEMENTS": {
         "EN": [
             "If you're looking for new challenges to beat, just tap here."
         ]
     },
     "TID_TUTORIAL_ACHIEVEMENTS2": {
         "EN": [
@@ -34678,14 +35437,19 @@
         ]
     },
     "TID_TUTORIAL_ENTER_AGE": {
         "EN": [
             "Oh, and one more question..."
         ]
     },
+    "TID_TUTORIAL_ENTER_AGE_ALTERNATE_PATH": {
+        "EN": [
+            "Welcome Chief! Let's get started."
+        ]
+    },
     "TID_TUTORIAL_FAILED": {
         "EN": [
             "Oops, something went wrong. Restart and try again!"
         ]
     },
     "TID_TUTORIAL_FORGE_1": {
         "EN": [
@@ -35983,14 +36747,19 @@
         ]
     },
     "TID_WAIT_BEFORE_ARRANGING_WAR_AGAIN": {
         "EN": [
             "You can send another challenge in <time>"
         ]
     },
+    "TID_WAIT_BEFORE_TAGGING": {
+        "EN": [
+            "Chat tagging will be available <number> minutes after joining a Clan!"
+        ]
+    },
     "TID_WALL_BREAKER": {
         "EN": [
             "Wall Breaker"
         ]
     },
     "TID_WALL_INFO": {
         "EN": [
@@ -36378,14 +37147,19 @@
         ]
     },
     "TID_WAR_SELECT_MEMBERS_HINTS": {
         "EN": [
             "You can select more or less members using the buttons above."
         ]
     },
+    "TID_WAR_SIGNUP_RESPONSE_NOT_AVAILABLE_IN_MODE": {
+        "EN": [
+            "Return Home to respond!"
+        ]
+    },
     "TID_WAR_SIZE": {
         "EN": [
             "War Size: <num> vs <num>"
         ]
     },
     "TID_WAR_SIZE_TEXT": {
         "EN": [
```

### Comparing `coc.py-3.4.1/coc/static/townhall_levels.json` & `coc_py-3.4.2/coc/static/townhall_levels.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.993566176470588%*

 * *Differences: {"'1'": "{'StrengthMaxTroopTypes': [2], 'StrengthMaxSpellTypes': [1], 'ChallengeLootPercentage': "*

 * *        '[1]}',*

 * * "'10'": "{'StrengthMaxTroopTypes': [7], 'StrengthMaxSpellTypes': [5], 'ChallengeLootPercentage': "*

 * *         '[80]}',*

 * * "'11'": "{'StrengthMaxSpellTypes': [7], 'ChallengeLootPercentage': [90]}",*

 * * "'12'": "{'StrengthMaxTroopTypes': [11], 'ChallengeLootPercentage': [95]}",*

 * * "'13'": "{'StrengthMaxTroopTypes': [11], 'ChallengeLootPercentage': [100]}",*

 * * "'14'": "{'StrengthMaxTroopTypes': [11], 'Chall […]*

```diff
@@ -51,14 +51,17 @@
         ],
         "CartLootReengagementDarkElixir": [
             0
         ],
         "CartLootReengagementResource": [
             5000
         ],
+        "ChallengeLootPercentage": [
+            1
+        ],
         "Clock Tower": [],
         "Communications mast": [],
         "Crusher": [],
         "Dark Elixir Barrack": [],
         "Dark Elixir Pump": [],
         "Dark Elixir Storage": [],
         "Dark Tower": [],
@@ -197,18 +200,18 @@
         "StarBonusBoostHours": [
             0
         ],
         "StrengthMaxSiegeTypes": [
             0
         ],
         "StrengthMaxSpellTypes": [
-            6
+            1
         ],
         "StrengthMaxTroopTypes": [
-            6
+            2
         ],
         "Superbomb": [],
         "Tesla Tower": [],
         "Tesla Tower2": [],
         "TornadoTrap": [],
         "Totem": [],
         "TreasuryDarkElixir": [
@@ -312,14 +315,17 @@
         ],
         "CartLootReengagementDarkElixir": [
             130000
         ],
         "CartLootReengagementResource": [
             13000000
         ],
+        "ChallengeLootPercentage": [
+            80
+        ],
         "Clock Tower": [],
         "Communications mast": [],
         "Crusher": [],
         "Dark Elixir Barrack": [],
         "Dark Elixir Pump": [],
         "Dark Elixir Storage": [],
         "Dark Tower": [
@@ -448,18 +454,18 @@
         "StarBonusBoostHours": [
             120
         ],
         "StrengthMaxSiegeTypes": [
             0
         ],
         "StrengthMaxSpellTypes": [
-            8
+            5
         ],
         "StrengthMaxTroopTypes": [
-            8
+            7
         ],
         "Superbomb": [
             5
         ],
         "Tesla Tower": [],
         "Tesla Tower2": [],
         "TornadoTrap": [],
@@ -551,14 +557,17 @@
         ],
         "CartLootReengagementDarkElixir": [
             140000
         ],
         "CartLootReengagementResource": [
             14000000
         ],
+        "ChallengeLootPercentage": [
+            90
+        ],
         "Clock Tower": [],
         "Communications mast": [],
         "Crusher": [],
         "Dark Elixir Barrack": [],
         "Dark Elixir Pump": [],
         "Dark Elixir Storage": [],
         "Dark Tower": [],
@@ -677,15 +686,15 @@
         "StarBonusBoostHours": [
             120
         ],
         "StrengthMaxSiegeTypes": [
             0
         ],
         "StrengthMaxSpellTypes": [
-            8
+            7
         ],
         "StrengthMaxTroopTypes": [
             10
         ],
         "Superbomb": [],
         "Tesla Tower": [],
         "Tesla Tower2": [],
@@ -772,14 +781,17 @@
         ],
         "CartLootReengagementDarkElixir": [
             150000
         ],
         "CartLootReengagementResource": [
             15000000
         ],
+        "ChallengeLootPercentage": [
+            95
+        ],
         "Clock Tower": [],
         "Communications mast": [],
         "Crusher": [],
         "Dark Elixir Barrack": [],
         "Dark Elixir Pump": [],
         "Dark Elixir Storage": [],
         "Dark Tower": [
@@ -907,15 +919,15 @@
         "StrengthMaxSiegeTypes": [
             3
         ],
         "StrengthMaxSpellTypes": [
             8
         ],
         "StrengthMaxTroopTypes": [
-            12
+            11
         ],
         "Superbomb": [
             6
         ],
         "Tesla Tower": [
             5
         ],
@@ -997,14 +1009,17 @@
         ],
         "CartLootReengagementDarkElixir": [
             160000
         ],
         "CartLootReengagementResource": [
             16000000
         ],
+        "ChallengeLootPercentage": [
+            100
+        ],
         "Clock Tower": [],
         "Communications mast": [],
         "Crusher": [],
         "Dark Elixir Barrack": [],
         "Dark Elixir Pump": [],
         "Dark Elixir Storage": [],
         "Dark Tower": [],
@@ -1134,15 +1149,15 @@
         "StrengthMaxSiegeTypes": [
             3
         ],
         "StrengthMaxSpellTypes": [
             8
         ],
         "StrengthMaxTroopTypes": [
-            12
+            11
         ],
         "Superbomb": [],
         "Tesla Tower": [],
         "Tesla Tower2": [],
         "TornadoTrap": [],
         "Totem": [],
         "TreasuryDarkElixir": [],
@@ -1222,14 +1237,17 @@
         ],
         "CartLootReengagementDarkElixir": [
             170000
         ],
         "CartLootReengagementResource": [
             17000000
         ],
+        "ChallengeLootPercentage": [
+            100
+        ],
         "Clock Tower": [],
         "Communications mast": [],
         "Crusher": [],
         "Dark Elixir Barrack": [],
         "Dark Elixir Pump": [],
         "Dark Elixir Storage": [],
         "Dark Tower": [],
@@ -1357,15 +1375,15 @@
         "StrengthMaxSiegeTypes": [
             3
         ],
         "StrengthMaxSpellTypes": [
             8
         ],
         "StrengthMaxTroopTypes": [
-            12
+            11
         ],
         "Superbomb": [
             7
         ],
         "Tesla Tower": [],
         "Tesla Tower2": [],
         "TornadoTrap": [],
@@ -1445,14 +1463,17 @@
         ],
         "CartLootReengagementDarkElixir": [
             180000
         ],
         "CartLootReengagementResource": [
             18000000
         ],
+        "ChallengeLootPercentage": [
+            100
+        ],
         "Clock Tower": [],
         "Communications mast": [],
         "Crusher": [],
         "Dark Elixir Barrack": [],
         "Dark Elixir Pump": [],
         "Dark Elixir Storage": [],
         "Dark Tower": [],
@@ -1662,14 +1683,17 @@
         ],
         "CartLootReengagementDarkElixir": [
             190000
         ],
         "CartLootReengagementResource": [
             19000000
         ],
+        "ChallengeLootPercentage": [
+            100
+        ],
         "Clock Tower": [],
         "Communications mast": [],
         "Crusher": [],
         "Dark Elixir Barrack": [],
         "Dark Elixir Pump": [],
         "Dark Elixir Storage": [],
         "Dark Tower": [],
@@ -1887,14 +1911,17 @@
         ],
         "CartLootReengagementDarkElixir": [
             0
         ],
         "CartLootReengagementResource": [
             25000
         ],
+        "ChallengeLootPercentage": [
+            2
+        ],
         "Clock Tower": [],
         "Communications mast": [],
         "Crusher": [],
         "Dark Elixir Barrack": [],
         "Dark Elixir Pump": [],
         "Dark Elixir Storage": [],
         "Dark Tower": [],
@@ -2025,18 +2052,18 @@
         "StarBonusBoostHours": [
             0
         ],
         "StrengthMaxSiegeTypes": [
             0
         ],
         "StrengthMaxSpellTypes": [
-            6
+            1
         ],
         "StrengthMaxTroopTypes": [
-            6
+            2
         ],
         "Superbomb": [],
         "Tesla Tower": [],
         "Tesla Tower2": [],
         "TornadoTrap": [],
         "Totem": [],
         "TreasuryDarkElixir": [],
@@ -2126,14 +2153,17 @@
         ],
         "CartLootReengagementDarkElixir": [
             0
         ],
         "CartLootReengagementResource": [
             150000
         ],
+        "ChallengeLootPercentage": [
+            3
+        ],
         "Clock Tower": [],
         "Communications mast": [],
         "Crusher": [
             1
         ],
         "Dark Elixir Barrack": [],
         "Dark Elixir Pump": [],
@@ -2282,18 +2312,18 @@
         "StarBonusBoostHours": [
             0
         ],
         "StrengthMaxSiegeTypes": [
             0
         ],
         "StrengthMaxSpellTypes": [
-            6
+            1
         ],
         "StrengthMaxTroopTypes": [
-            6
+            2
         ],
         "Superbomb": [],
         "Tesla Tower": [],
         "Tesla Tower2": [
             1
         ],
         "TornadoTrap": [],
@@ -2391,14 +2421,17 @@
         ],
         "CartLootReengagementDarkElixir": [
             0
         ],
         "CartLootReengagementResource": [
             1000000
         ],
+        "ChallengeLootPercentage": [
+            5
+        ],
         "Clock Tower": [
             1
         ],
         "Communications mast": [],
         "Crusher": [],
         "Dark Elixir Barrack": [],
         "Dark Elixir Pump": [],
@@ -2537,18 +2570,18 @@
         "StarBonusBoostHours": [
             72
         ],
         "StrengthMaxSiegeTypes": [
             0
         ],
         "StrengthMaxSpellTypes": [
-            6
+            1
         ],
         "StrengthMaxTroopTypes": [
-            6
+            3
         ],
         "Superbomb": [],
         "Tesla Tower": [],
         "Tesla Tower2": [],
         "TornadoTrap": [],
         "Totem": [],
         "TreasuryDarkElixir": [],
@@ -2642,14 +2675,17 @@
         ],
         "CartLootReengagementDarkElixir": [
             0
         ],
         "CartLootReengagementResource": [
             4000000
         ],
+        "ChallengeLootPercentage": [
+            8
+        ],
         "Clock Tower": [],
         "Communications mast": [],
         "Crusher": [],
         "Dark Elixir Barrack": [],
         "Dark Elixir Pump": [],
         "Dark Elixir Storage": [],
         "Dark Tower": [],
@@ -2792,18 +2828,18 @@
         "StarBonusBoostHours": [
             72
         ],
         "StrengthMaxSiegeTypes": [
             0
         ],
         "StrengthMaxSpellTypes": [
-            6
+            1
         ],
         "StrengthMaxTroopTypes": [
-            6
+            3
         ],
         "Superbomb": [],
         "Tesla Tower": [],
         "Tesla Tower2": [],
         "TornadoTrap": [],
         "Totem": [],
         "TreasuryDarkElixir": [],
@@ -2897,14 +2933,17 @@
         ],
         "CartLootReengagementDarkElixir": [
             0
         ],
         "CartLootReengagementResource": [
             6000000
         ],
+        "ChallengeLootPercentage": [
+            16
+        ],
         "Clock Tower": [],
         "Communications mast": [],
         "Crusher": [
             2
         ],
         "Dark Elixir Barrack": [],
         "Dark Elixir Pump": [],
@@ -3053,18 +3092,18 @@
         "StarBonusBoostHours": [
             72
         ],
         "StrengthMaxSiegeTypes": [
             0
         ],
         "StrengthMaxSpellTypes": [
-            6
+            1
         ],
         "StrengthMaxTroopTypes": [
-            6
+            4
         ],
         "Superbomb": [
             1
         ],
         "Tesla Tower": [],
         "Tesla Tower2": [
             2
@@ -3166,14 +3205,17 @@
         ],
         "CartLootReengagementDarkElixir": [
             80000
         ],
         "CartLootReengagementResource": [
             8000000
         ],
+        "ChallengeLootPercentage": [
+            30
+        ],
         "Clock Tower": [],
         "Communications mast": [],
         "Crusher": [],
         "Dark Elixir Barrack": [
             1
         ],
         "Dark Elixir Pump": [
@@ -3316,18 +3358,18 @@
         "StarBonusBoostHours": [
             96
         ],
         "StrengthMaxSiegeTypes": [
             0
         ],
         "StrengthMaxSpellTypes": [
-            6
+            2
         ],
         "StrengthMaxTroopTypes": [
-            6
+            4
         ],
         "Superbomb": [
             2
         ],
         "Tesla Tower": [
             2
         ],
@@ -3429,14 +3471,17 @@
         ],
         "CartLootReengagementDarkElixir": [
             100000
         ],
         "CartLootReengagementResource": [
             10000000
         ],
+        "ChallengeLootPercentage": [
+            50
+        ],
         "Clock Tower": [],
         "Communications mast": [],
         "Crusher": [],
         "Dark Elixir Barrack": [],
         "Dark Elixir Pump": [
             2
         ],
@@ -3589,18 +3634,18 @@
         "StarBonusBoostHours": [
             96
         ],
         "StrengthMaxSiegeTypes": [
             0
         ],
         "StrengthMaxSpellTypes": [
-            7
+            2
         ],
         "StrengthMaxTroopTypes": [
-            6
+            5
         ],
         "Superbomb": [
             3
         ],
         "Tesla Tower": [
             3
         ],
@@ -3700,14 +3745,17 @@
         ],
         "CartLootReengagementDarkElixir": [
             115000
         ],
         "CartLootReengagementResource": [
             11500000
         ],
+        "ChallengeLootPercentage": [
+            65
+        ],
         "Clock Tower": [],
         "Communications mast": [],
         "Crusher": [],
         "Dark Elixir Barrack": [],
         "Dark Elixir Pump": [
             3
         ],
@@ -3854,18 +3902,18 @@
         "StarBonusBoostHours": [
             96
         ],
         "StrengthMaxSiegeTypes": [
             0
         ],
         "StrengthMaxSpellTypes": [
-            7
+            3
         ],
         "StrengthMaxTroopTypes": [
-            7
+            5
         ],
         "Superbomb": [
             4
         ],
         "Tesla Tower": [
             4
         ],
```

### Comparing `coc.py-3.4.1/coc/static/troop_ids.json` & `coc_py-3.4.2/coc/static/troop_ids.json`

 * *Files identical despite different names*

### Comparing `coc.py-3.4.1/coc/static/update_static.py` & `coc_py-3.4.2/coc/static/update_static.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     ("logic/pets.csv", "pets.csv"),
     ("logic/spells.csv", "spells.csv"),
     ("logic/super_licences.csv", "supers.csv"),
     ("logic/townhall_levels.csv", "townhall_levels.csv"),
     ("logic/character_items.csv", "equipment.csv"),
     ("localization/texts.csv", "texts_EN.csv"),
 ]
-FINGERPRINT = "c4e8c2976dcf42530d68dcb1fdfb61d071085abf"
+FINGERPRINT = "ef352b21171ef765a724f84dae76d8edbc79a93a"
 BASE_URL = f"https://game-assets.clashofclans.com/{FINGERPRINT}"
 APK_URL = "https://d.apkpure.net/b/APK/com.supercell.clashofclans?version=latest"
 
 
 def decompress(data):
     if data[0:4] == b"SCLZ":
         logging.debug("Decompressing using LZHAM ...")
```

### Comparing `coc.py-3.4.1/coc/troop.py` & `coc_py-3.4.2/coc/troop.py`

 * *Files identical despite different names*

### Comparing `coc.py-3.4.1/coc/utils.py` & `coc_py-3.4.2/coc/utils.py`

 * *Files identical despite different names*

### Comparing `coc.py-3.4.1/coc/war_attack.py` & `coc_py-3.4.2/coc/war_attack.py`

 * *Files identical despite different names*

### Comparing `coc.py-3.4.1/coc/war_clans.py` & `coc_py-3.4.2/coc/war_clans.py`

 * *Files identical despite different names*

### Comparing `coc.py-3.4.1/coc/war_members.py` & `coc_py-3.4.2/coc/war_members.py`

 * *Files identical despite different names*

### Comparing `coc.py-3.4.1/coc/wars.py` & `coc_py-3.4.2/coc/wars.py`

 * *Files identical despite different names*

### Comparing `coc.py-3.4.1/coc.py.egg-info/PKG-INFO` & `coc_py-3.4.2/coc.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coc.py
-Version: 3.4.1
+Version: 3.4.2
 Summary: A python wrapper for the Clash of Clans API
 Author: mathsman5133
 Maintainer: majordoobie, MagicTheDev, Kuchenmampfer, lukasthaler, doluk
 License: MIT
 Project-URL: documentation, https://cocpy.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/mathsman5133/coc.py
 Project-URL: changelog, https://cocpy.readthedocs.io/en/latest/miscellaneous/changelog.html
```

### Comparing `coc.py-3.4.1/coc.py.egg-info/SOURCES.txt` & `coc_py-3.4.2/coc.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coc.py-3.4.1/pyproject.toml` & `coc_py-3.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "coc.py"
 authors = [{ name = "mathsman5133" }]
 maintainers = [{ name = "majordoobie" }, { name = "MagicTheDev" }, { name = "Kuchenmampfer" },
     { name = "lukasthaler"}, { name = "doluk"}]
-version = "3.4.1"
+version = "3.4.2"
 description = "A python wrapper for the Clash of Clans API"
 requires-python = ">=3.7.3"
 readme = "README.rst"
 license = { text = "MIT" }
 keywords = ["coc", "clash of clans", "coc.py", "clash api"]
 classifiers = ["Development Status :: 5 - Production/Stable",
     "Programming Language :: Python",
```

### Comparing `coc.py-3.4.1/tests/test_capitalraidseasons.py` & `coc_py-3.4.2/tests/test_capitalraidseasons.py`

 * *Files identical despite different names*

### Comparing `coc.py-3.4.1/tests/test_clans.py` & `coc_py-3.4.2/tests/test_clans.py`

 * *Files identical despite different names*

### Comparing `coc.py-3.4.1/tests/test_clash_meta.py` & `coc_py-3.4.2/tests/test_clash_meta.py`

 * *Files identical despite different names*

### Comparing `coc.py-3.4.1/tests/test_players.py` & `coc_py-3.4.2/tests/test_players.py`

 * *Files identical despite different names*

### Comparing `coc.py-3.4.1/tests/test_troop_levels.py` & `coc_py-3.4.2/tests/test_troop_levels.py`

 * *Files identical despite different names*

### Comparing `coc.py-3.4.1/tests/test_wars.py` & `coc_py-3.4.2/tests/test_wars.py`

 * *Files identical despite different names*

