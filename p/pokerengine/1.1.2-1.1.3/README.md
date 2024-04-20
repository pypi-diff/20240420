# Comparing `tmp/pokerengine-1.1.2.tar.gz` & `tmp/pokerengine-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokerengine-1.1.2.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "pokerengine-1.1.3.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `pokerengine-1.1.2.tar` & `pokerengine-1.1.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     3831 2022-11-09 12:37:21.000000 pokerengine-1.1.2/.clang-format
--rw-r--r--   0        0        0      137 2022-11-09 12:37:21.000000 pokerengine-1.1.2/.github/dependabot.yaml
--rw-r--r--   0        0        0      648 2022-11-09 12:37:21.000000 pokerengine-1.1.2/.github/workflows/pre-commit-updater.yml
--rw-r--r--   0        0        0      578 2022-11-09 12:37:21.000000 pokerengine-1.1.2/.gitignore
--rw-r--r--   0        0        0      563 2022-11-09 12:37:21.000000 pokerengine-1.1.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2009 2022-11-09 12:37:21.000000 pokerengine-1.1.2/CMakeLists.txt
--rw-r--r--   0        0        0       33 2022-11-09 12:37:21.000000 pokerengine-1.1.2/README.md
--rw-r--r--   0        0        0      970 2022-11-09 12:37:21.000000 pokerengine-1.1.2/examples/hand_straight.py
--rw-r--r--   0        0        0      544 2022-11-09 12:37:21.000000 pokerengine-1.1.2/include/pokerengine/bits.hpp
--rw-r--r--   0        0        0     7684 2022-11-09 12:37:21.000000 pokerengine-1.1.2/include/pokerengine/card/card.hpp
--rw-r--r--   0        0        0     2663 2022-11-09 12:37:21.000000 pokerengine-1.1.2/include/pokerengine/card/cards.hpp
--rw-r--r--   0        0        0     3223 2022-11-09 12:37:21.000000 pokerengine-1.1.2/include/pokerengine/card/hand.hpp
--rw-r--r--   0        0        0     1556 2022-11-09 12:37:21.000000 pokerengine-1.1.2/include/pokerengine/constants.hpp
--rw-r--r--   0        0        0    31677 2022-11-09 12:37:21.000000 pokerengine-1.1.2/include/pokerengine/engine.hpp
--rw-r--r--   0        0        0     3104 2022-11-09 12:37:21.000000 pokerengine-1.1.2/include/pokerengine/enums.hpp
--rw-r--r--   0        0        0     4460 2022-11-09 12:37:21.000000 pokerengine-1.1.2/include/pokerengine/evaluator/evaluation.hpp
--rw-r--r--   0        0        0     1552 2022-11-09 12:37:21.000000 pokerengine-1.1.2/include/pokerengine/evaluator/evaluation_result.hpp
--rw-r--r--   0        0        0   136152 2022-11-09 12:37:21.000000 pokerengine-1.1.2/include/pokerengine/evaluator/lookup_tables.hpp
--rw-r--r--   0        0        0     5389 2022-11-09 12:37:21.000000 pokerengine-1.1.2/include/pokerengine/evaluator/result.hpp
--rw-r--r--   0        0        0      305 2022-11-09 12:37:21.000000 pokerengine-1.1.2/include/pokerengine/pokerengine.hpp
--rw-r--r--   0        0        0     8217 2022-11-09 12:37:21.000000 pokerengine-1.1.2/include/pokerengine/python/pycard.hpp
--rw-r--r--   0        0        0     1856 2022-11-09 12:37:21.000000 pokerengine-1.1.2/include/pokerengine/python/pyconstants.hpp
--rw-r--r--   0        0        0    11836 2022-11-09 12:37:21.000000 pokerengine-1.1.2/include/pokerengine/python/pyengine.hpp
--rw-r--r--   0        0        0     5720 2022-11-09 12:37:21.000000 pokerengine-1.1.2/include/pokerengine/python/pyenums.hpp
--rw-r--r--   0        0        0     2586 2022-11-09 12:37:21.000000 pokerengine-1.1.2/include/pokerengine/python/pyevaluation.hpp
--rw-r--r--   0        0        0      240 2022-11-09 12:37:21.000000 pokerengine-1.1.2/include/pokerengine/python/python.hpp
--rw-r--r--   0        0        0     1327 2022-11-09 12:37:21.000000 pokerengine-1.1.2/include/pokerengine/string.hpp
--rw-r--r--   0        0        0      278 2022-11-09 12:37:21.000000 pokerengine-1.1.2/include/pokerengine/types.hpp
--rw-r--r--   0        0        0     1070 2022-11-09 12:37:21.000000 pokerengine-1.1.2/include/pokerengine/vector.hpp
--rw-r--r--   0        0        0     1069 2022-11-09 12:37:21.000000 pokerengine-1.1.2/licenses/MIT
--rw-r--r--   0        0        0     1190 2022-11-09 12:37:21.000000 pokerengine-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      302 2022-11-09 12:37:21.000000 pokerengine-1.1.2/src/pokerengine/__init__.py
--rw-r--r--   0        0        0      281 2022-11-09 12:37:21.000000 pokerengine-1.1.2/src/pokerengine/card.py
--rw-r--r--   0        0        0      782 2022-11-09 12:37:21.000000 pokerengine-1.1.2/src/pokerengine/constants.py
--rw-r--r--   0        0        0      435 2022-11-09 12:37:21.000000 pokerengine-1.1.2/src/pokerengine/engine.py
--rw-r--r--   0        0        0      593 2022-11-09 12:37:21.000000 pokerengine-1.1.2/src/pokerengine/enums.py
--rw-r--r--   0        0        0      253 2022-11-09 12:37:21.000000 pokerengine-1.1.2/src/pokerengine/evaluation.py
--rw-r--r--   0        0        0      323 2022-11-09 12:37:21.000000 pokerengine-1.1.2/src/pokerengine/pokerengine_core/__init__.pyi
--rw-r--r--   0        0        0     7462 2022-11-09 12:37:21.000000 pokerengine-1.1.2/src/pokerengine/pokerengine_core/card.pyi
--rw-r--r--   0        0        0      644 2022-11-09 12:37:21.000000 pokerengine-1.1.2/src/pokerengine/pokerengine_core/constants.pyi
--rw-r--r--   0        0        0     7863 2022-11-09 12:37:21.000000 pokerengine-1.1.2/src/pokerengine/pokerengine_core/engine.pyi
--rw-r--r--   0        0        0      220 2022-11-09 12:37:21.000000 pokerengine-1.1.2/src/pokerengine/pokerengine_core/enums/__init__.pyi
--rw-r--r--   0        0        0      221 2022-11-09 12:37:21.000000 pokerengine-1.1.2/src/pokerengine/pokerengine_core/enums/action.pyi
--rw-r--r--   0        0        0      320 2022-11-09 12:37:21.000000 pokerengine-1.1.2/src/pokerengine/pokerengine_core/enums/combination.pyi
--rw-r--r--   0        0        0      239 2022-11-09 12:37:21.000000 pokerengine-1.1.2/src/pokerengine/pokerengine_core/enums/position.pyi
--rw-r--r--   0        0        0      293 2022-11-09 12:37:21.000000 pokerengine-1.1.2/src/pokerengine/pokerengine_core/enums/rank.pyi
--rw-r--r--   0        0        0      210 2022-11-09 12:37:21.000000 pokerengine-1.1.2/src/pokerengine/pokerengine_core/enums/round.pyi
--rw-r--r--   0        0        0      204 2022-11-09 12:37:21.000000 pokerengine-1.1.2/src/pokerengine/pokerengine_core/enums/state.pyi
--rw-r--r--   0        0        0      182 2022-11-09 12:37:21.000000 pokerengine-1.1.2/src/pokerengine/pokerengine_core/enums/suit.pyi
--rw-r--r--   0        0        0     2418 2022-11-09 12:37:21.000000 pokerengine-1.1.2/src/pokerengine/pokerengine_core/evaluation.pyi
--rw-r--r--   0        0        0      149 2022-11-09 12:37:21.000000 pokerengine-1.1.2/src/pokerengine/pokerengine_core/utils.pyi
--rw-r--r--   0        0        0      922 2022-11-09 12:37:21.000000 pokerengine-1.1.2/src/pokerengine.cpp
--rw-r--r--   0        0        0      703 2022-11-09 12:37:21.000000 pokerengine-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3831 2022-11-09 12:37:21.000000 pokerengine-1.1.3/.clang-format
+-rw-r--r--   0        0        0      137 2022-11-09 12:37:21.000000 pokerengine-1.1.3/.github/dependabot.yaml
+-rw-r--r--   0        0        0      648 2022-11-09 12:37:21.000000 pokerengine-1.1.3/.github/workflows/pre-commit-updater.yml
+-rw-r--r--   0        0        0      578 2022-11-09 12:37:21.000000 pokerengine-1.1.3/.gitignore
+-rw-r--r--   0        0        0      563 2022-11-09 12:37:21.000000 pokerengine-1.1.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2042 2022-11-09 12:37:21.000000 pokerengine-1.1.3/CMakeLists.txt
+-rw-r--r--   0        0        0       33 2022-11-09 12:37:21.000000 pokerengine-1.1.3/README.md
+-rw-r--r--   0        0        0      970 2022-11-09 12:37:21.000000 pokerengine-1.1.3/examples/hand_straight.py
+-rw-r--r--   0        0        0      544 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/bits.hpp
+-rw-r--r--   0        0        0     7686 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/card/card.hpp
+-rw-r--r--   0        0        0     2663 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/card/cards.hpp
+-rw-r--r--   0        0        0     3223 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/card/hand.hpp
+-rw-r--r--   0        0        0     1556 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/constants.hpp
+-rw-r--r--   0        0        0    31480 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/engine.hpp
+-rw-r--r--   0        0        0     3221 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/enums.hpp
+-rw-r--r--   0        0        0     4460 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/evaluator/evaluation.hpp
+-rw-r--r--   0        0        0     1552 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/evaluator/evaluation_result.hpp
+-rw-r--r--   0        0        0   136152 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/evaluator/lookup_tables.hpp
+-rw-r--r--   0        0        0     5387 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/evaluator/result.hpp
+-rw-r--r--   0        0        0      305 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/pokerengine.hpp
+-rw-r--r--   0        0        0     8217 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/python/pycard.hpp
+-rw-r--r--   0        0        0     1856 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/python/pyconstants.hpp
+-rw-r--r--   0        0        0    11836 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/python/pyengine.hpp
+-rw-r--r--   0        0        0     5720 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/python/pyenums.hpp
+-rw-r--r--   0        0        0     2586 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/python/pyevaluation.hpp
+-rw-r--r--   0        0        0      240 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/python/python.hpp
+-rw-r--r--   0        0        0     1327 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/string.hpp
+-rw-r--r--   0        0        0      278 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/types.hpp
+-rw-r--r--   0        0        0     1070 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/vector.hpp
+-rw-r--r--   0        0        0     1069 2022-11-09 12:37:21.000000 pokerengine-1.1.3/licenses/MIT
+-rw-r--r--   0        0        0     1190 2022-11-09 12:37:21.000000 pokerengine-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0      302 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/__init__.py
+-rw-r--r--   0        0        0      281 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/card.py
+-rw-r--r--   0        0        0      782 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/constants.py
+-rw-r--r--   0        0        0      435 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/engine.py
+-rw-r--r--   0        0        0      593 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/enums.py
+-rw-r--r--   0        0        0      253 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/evaluation.py
+-rw-r--r--   0        0        0      323 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/pokerengine_core/__init__.pyi
+-rw-r--r--   0        0        0     7462 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/pokerengine_core/card.pyi
+-rw-r--r--   0        0        0      644 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/pokerengine_core/constants.pyi
+-rw-r--r--   0        0        0     7863 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/pokerengine_core/engine.pyi
+-rw-r--r--   0        0        0      220 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/pokerengine_core/enums/__init__.pyi
+-rw-r--r--   0        0        0      221 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/pokerengine_core/enums/action.pyi
+-rw-r--r--   0        0        0      320 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/pokerengine_core/enums/combination.pyi
+-rw-r--r--   0        0        0      239 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/pokerengine_core/enums/position.pyi
+-rw-r--r--   0        0        0      293 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/pokerengine_core/enums/rank.pyi
+-rw-r--r--   0        0        0      210 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/pokerengine_core/enums/round.pyi
+-rw-r--r--   0        0        0      204 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/pokerengine_core/enums/state.pyi
+-rw-r--r--   0        0        0      182 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/pokerengine_core/enums/suit.pyi
+-rw-r--r--   0        0        0     2418 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/pokerengine_core/evaluation.pyi
+-rw-r--r--   0        0        0      149 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/pokerengine_core/utils.pyi
+-rw-r--r--   0        0        0      922 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine.cpp
+-rw-r--r--   0        0        0      703 2022-11-09 12:37:21.000000 pokerengine-1.1.3/PKG-INFO
```

### Comparing `pokerengine-1.1.2/.clang-format` & `pokerengine-1.1.3/.clang-format`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.2/.github/workflows/pre-commit-updater.yml` & `pokerengine-1.1.3/.github/workflows/pre-commit-updater.yml`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.2/.gitignore` & `pokerengine-1.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.2/.pre-commit-config.yaml` & `pokerengine-1.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.2/CMakeLists.txt` & `pokerengine-1.1.3/CMakeLists.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 cmake_minimum_required(VERSION 3.12)
 
-project(pokerengine VERSION 1.1.2)
+project(pokerengine VERSION 1.1.3)
 
 set(CMAKE_CXX_STANDARD 20)
 set(CMAKE_CXX_STANDARD_REQUIRED ON)
 set(CMAKE_CXX_EXTENSIONS OFF)
 
+
+set(LIBRARY_NAME pokerengine_core)
+
 set(POKERENGINE_INCLUDE_DIR ${PROJECT_SOURCE_DIR}/include/pokerengine)
 set(POKERENGINE_SOURCE_DIR ${PROJECT_SOURCE_DIR}/src)
 
 include_directories(${PROJECT_NAME} ${POKERENGINE_INCLUDE_DIR})
 
 set(SOURCE_FILES ${POKERENGINE_SOURCE_DIR}/pokerengine.cpp)
 set(HEADER_FILES
@@ -35,12 +38,12 @@
         ${POKERENGINE_INCLUDE_DIR}/types.hpp
         ${POKERENGINE_INCLUDE_DIR}/vector.hpp)
 
 find_package(Python REQUIRED COMPONENTS Interpreter Development.Module)
 find_package(pybind11 CONFIG REQUIRED)
 find_package(magic_enum CONFIG REQUIRED)
 
-python_add_library(pokerengine_core MODULE ${SOURCE_FILES} ${HEADER_FILES} WITH_SOABI)
-target_link_libraries(pokerengine_core PRIVATE pybind11::headers magic_enum::magic_enum)
-target_compile_definitions(pokerengine_core PRIVATE VERSION_INFO=${PROJECT_VERSION})
+python_add_library(${LIBRARY_NAME} MODULE ${SOURCE_FILES} ${HEADER_FILES} WITH_SOABI)
+target_link_libraries(${LIBRARY_NAME} PRIVATE pybind11::headers magic_enum::magic_enum)
+target_compile_definitions(${LIBRARY_NAME} PRIVATE VERSION_INFO=${PROJECT_VERSION})
 
-install(TARGETS pokerengine_core DESTINATION pokerengine)
+install(TARGETS ${LIBRARY_NAME} DESTINATION pokerengine)
```

### Comparing `pokerengine-1.1.2/examples/hand_straight.py` & `pokerengine-1.1.3/examples/hand_straight.py`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.2/include/pokerengine/bits.hpp` & `pokerengine-1.1.3/include/pokerengine/bits.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.2/include/pokerengine/card/card.hpp` & `pokerengine-1.1.3/include/pokerengine/card/card.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -213,16 +213,16 @@
 class card_generator {
 public:
     explicit card_generator(uint16_t seed = 1927)
             : rng_(seed), dist_rank_(0, constants::RANKS), dist_suit_(0, constants::SUITS) {
     }
 
     [[nodiscard]] auto generate() -> card {
-        return card{ rank{ enums::rank{ int8_t(dist_rank_(rng_)) } },
-                     suit{ enums::suit{ static_cast< int8_t >(dist_suit_(rng_)) } } };
+        return card{ rank{ enums::rank{ uint8_t(dist_rank_(rng_)) } },
+                     suit{ enums::suit{ static_cast< uint8_t >(dist_suit_(rng_)) } } };
     }
 
     [[nodiscard]] auto generate_v(uint8_t n) -> std::vector< card > {
         if (n > ((constants::RANKS) * (constants::SUITS))) {
             throw std::runtime_error("N greater than number of specified unique cards");
         }
```

### Comparing `pokerengine-1.1.2/include/pokerengine/card/cards.hpp` & `pokerengine-1.1.3/include/pokerengine/card/cards.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.2/include/pokerengine/card/hand.hpp` & `pokerengine-1.1.3/include/pokerengine/card/hand.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.2/include/pokerengine/constants.hpp` & `pokerengine-1.1.3/include/pokerengine/constants.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.2/include/pokerengine/engine.hpp` & `pokerengine-1.1.3/include/pokerengine/engine.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -238,21 +238,15 @@
     std::for_each(players.begin(), players.end(), [&, index = 0](auto &player) mutable -> void {
         player.state = enums::state::init;
         player.behind = player.stack;
         player.round_bet = 0;
         player.front = 0;
 
         if (index < 2) {
-            if (players.size() == constants::MIN_PLAYERS) {
-                player.front = index == 0 ? sb_bet : bb_bet;
-            } else {
-                player.front = index == 0 ? bb_bet : sb_bet;
-            }
-
-            player.state = enums::state::alive;
+            player.front = index == 0 ? sb_bet : bb_bet;
 
             if (player.front > player.behind) {
                 player.front = player.behind;
             }
 
             player.behind -= player.front;
             player.round_bet = player.front;
@@ -533,19 +527,19 @@
     using actual::engine_detail< Engine >::engine_detail;
 
     [[nodiscard]] auto get_current() const noexcept -> enums::position {
         return current_;
     }
 
     [[nodiscard]] auto get_player() const -> player {
-        return this->engine.players.get_player(static_cast< int >(get_current()));
+        return this->engine.players.get_player(static_cast< int8_t >(get_current()));
     }
 
     [[nodiscard]] auto get_player() -> player & {
-        return this->engine.players.get_player(static_cast< int >(get_current()));
+        return this->engine.players.get_player(static_cast< int8_t >(get_current()));
     }
 
     [[nodiscard]] auto get_number_alive() const -> int {
         auto iterable = this->engine.players.get_players();
         return std::accumulate(
                         iterable.cbegin(), iterable.cend(), 0, [&](int value, auto const &element) -> int {
                             return element.state != enums::state::out ? value + 1 : value;
@@ -580,25 +574,25 @@
         current_ = position;
     }
 
     auto set_next_current() -> void {
         auto iterable_size = this->engine.players.get_players().size();
         do {
             set_current(static_cast< enums::position >(
-                            (static_cast< int >(get_current()) + 1) % iterable_size));
+                            (static_cast< int8_t >(get_current()) + 1) % iterable_size));
         } while (get_player().state == enums::state::out || get_player().state == enums::state::allin);
     }
 
     auto set_next_round_player() -> void {
         set_current(enums::position::sb);
 
         auto iterable_size = this->engine.players.get_players().size();
         while (get_player().state == enums::state::out || get_player().state == enums::state::allin) {
             set_current(static_cast< enums::position >(
-                            (static_cast< int >(get_current()) + 1) % iterable_size));
+                            (static_cast< int8_t >(get_current()) + 1) % iterable_size));
         }
     }
 
 private:
     enums::position current_{ enums::position::none };
 };
```

### Comparing `pokerengine-1.1.2/include/pokerengine/enums.hpp` & `pokerengine-1.1.3/include/pokerengine/enums.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -8,49 +8,49 @@
 #include <cstdint>
 
 #include <magic_enum.hpp>
 
 #include "pokerengine.hpp"
 
 namespace pokerengine::enums {
-enum class action : int {
+enum class action : int8_t {
     none = -1,
     fold = 0,
     check = 1,
     call = 2,
     bet = 3,
     raise = 4,
     allin = 5,
 };
 
-enum class combination : int {
-    none = -1,
+enum class combination : int8_t {
+    none [[maybe_unused]] = -1,
     no_pair = 0,
     one_pair = 1,
     two_pair = 2,
     three_of_a_kind = 3,
     straight = 4,
     flush = 5,
     full_house = 6,
     four_of_a_kind = 7,
     straight_flush = 8,
 };
 
-enum class position : int {
+enum class position : int8_t {
     none = -1,
     sb = 0,
     bb = 1,
     utg = 2,
     lwj [[maybe_unused]] = 3,
     hij [[maybe_unused]] = 4,
     cof [[maybe_unused]] = 5,
     btn [[maybe_unused]] = 6,
 };
 
-enum class rank : int {
+enum class rank : uint8_t {
     two = 0,
     three = 1,
     four = 2,
     five = 3,
     six = 4,
     seven = 5,
     eight = 6,
@@ -58,42 +58,43 @@
     ten = 8,
     jack = 9,
     queen = 10,
     king = 11,
     ace = 12,
 };
 
-enum class round : int {
+enum class round : int8_t {
     none = -1,
     preflop = 0,
     flop = 1,
-    turn = 2,
+    turn [[maybe_unused]] = 2,
     river = 3,
     showdown = 4,
 };
 
-enum class state : int {
+enum class state : int8_t {
     none = -1,
     init = 0,
     out = 1,
     alive = 2,
     allin = 3,
 };
 
-enum class suit : int32_t {
+enum class suit : uint8_t {
     clubs = 0,
     diamonds = 1,
     hearts = 2,
     spades = 3,
 };
 } // namespace pokerengine::enums
 
 template <>
-[[maybe_unused]] constexpr magic_enum::customize::customize_t magic_enum::customize::enum_name< pokerengine::enums::rank >(
-                pokerengine::enums::rank value) noexcept {
+[[maybe_unused]] constexpr magic_enum::customize::customize_t
+                magic_enum::customize::enum_name< pokerengine::enums::rank >(
+                                pokerengine::enums::rank value) noexcept {
     switch (value) {
     case pokerengine::enums::rank::two: {
         return "2";
     }
     case pokerengine::enums::rank::three: {
         return "3";
     }
@@ -133,16 +134,17 @@
     default: {
         return default_tag;
     }
     }
 }
 
 template <>
-[[maybe_unused]] constexpr magic_enum::customize::customize_t magic_enum::customize::enum_name< pokerengine::enums::suit >(
-                pokerengine::enums::suit value) noexcept {
+[[maybe_unused]] constexpr magic_enum::customize::customize_t
+                magic_enum::customize::enum_name< pokerengine::enums::suit >(
+                                pokerengine::enums::suit value) noexcept {
     switch (value) {
     case pokerengine::enums::suit::clubs: {
         return "c";
     }
     case pokerengine::enums::suit::diamonds: {
         return "d";
     }
```

### Comparing `pokerengine-1.1.2/include/pokerengine/evaluator/evaluation.hpp` & `pokerengine-1.1.3/include/pokerengine/evaluator/evaluation.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.2/include/pokerengine/evaluator/evaluation_result.hpp` & `pokerengine-1.1.3/include/pokerengine/evaluator/evaluation_result.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.2/include/pokerengine/evaluator/lookup_tables.hpp` & `pokerengine-1.1.3/include/pokerengine/evaluator/lookup_tables.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.2/include/pokerengine/evaluator/result.hpp` & `pokerengine-1.1.3/include/pokerengine/evaluator/result.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -51,16 +51,16 @@
         }
         }
     }
     [[nodiscard]] auto get_result() const noexcept -> uint32_t {
         return result_;
     }
 
-    [[nodiscard]] auto get_type() const noexcept -> uint8_t {
-        return static_cast< uint8_t >(get_result() >> constants::OFFSET_TYPE);
+    [[nodiscard]] auto get_type() const noexcept -> int8_t {
+        return static_cast< int8_t >(get_result() >> constants::OFFSET_TYPE);
     }
 
     [[nodiscard]] auto get_major_rank() const noexcept -> rank {
         return rank{ enums::rank(
                         constants::MASK_RANKS_NUMBER & ((get_result() >> constants::OFFSET_MAJOR) - 0)) };
     }
```

### Comparing `pokerengine-1.1.2/include/pokerengine/python/pycard.hpp` & `pokerengine-1.1.3/include/pokerengine/python/pycard.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.2/include/pokerengine/python/pyconstants.hpp` & `pokerengine-1.1.3/include/pokerengine/python/pyconstants.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.2/include/pokerengine/python/pyengine.hpp` & `pokerengine-1.1.3/include/pokerengine/python/pyengine.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.2/include/pokerengine/python/pyenums.hpp` & `pokerengine-1.1.3/include/pokerengine/python/pyenums.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.2/include/pokerengine/python/pyevaluation.hpp` & `pokerengine-1.1.3/include/pokerengine/python/pyevaluation.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.2/include/pokerengine/string.hpp` & `pokerengine-1.1.3/include/pokerengine/string.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.2/include/pokerengine/vector.hpp` & `pokerengine-1.1.3/include/pokerengine/vector.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.2/licenses/MIT` & `pokerengine-1.1.3/licenses/MIT`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.2/pyproject.toml` & `pokerengine-1.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["scikit-build-core==0.6.1", "pybind11"]
 build-backend = "scikit_build_core.build"
 
 [project]
 name = "pokerengine"
-version = "1.1.2"
+version = "1.1.3"
 description = "Poker Library"
 readme = "README.md"
 authors = [
     {name = "raindinners"}
 ]
 requires-python = ">=3.8"
 keywords = [
```

### Comparing `pokerengine-1.1.2/src/pokerengine/constants.py` & `pokerengine-1.1.3/src/pokerengine/constants.py`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.2/src/pokerengine/enums.py` & `pokerengine-1.1.3/src/pokerengine/enums.py`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.2/src/pokerengine/pokerengine_core/card.pyi` & `pokerengine-1.1.3/src/pokerengine/pokerengine_core/card.pyi`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.2/src/pokerengine/pokerengine_core/constants.pyi` & `pokerengine-1.1.3/src/pokerengine/pokerengine_core/constants.pyi`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.2/src/pokerengine/pokerengine_core/engine.pyi` & `pokerengine-1.1.3/src/pokerengine/pokerengine_core/engine.pyi`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.2/src/pokerengine/pokerengine_core/evaluation.pyi` & `pokerengine-1.1.3/src/pokerengine/pokerengine_core/evaluation.pyi`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.2/src/pokerengine.cpp` & `pokerengine-1.1.3/src/pokerengine.cpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.2/PKG-INFO` & `pokerengine-1.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pokerengine
-Version: 1.1.2
+Version: 1.1.3
 Summary: Poker Library
 Keywords: raindinners,engine,poker,texas,holdem,texas-holdem,texas_holdem,pybind11,scikit-build-core,fast,c++,magic_enum,stubs,python-stubs,python_stubs,pythonstubs,py-stubs,py_stubs,pystubs
 Author: raindinners
 Requires-Python: >=3.8
 Provides-Extra: dev
 Provides-Extra: build
 Requires-Dist: black~=23.10.0; extra == "dev"
```

