# Comparing `tmp/pokerengine-1.1.3.tar.gz` & `tmp/pokerengine-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokerengine-1.1.3.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "pokerengine-1.1.4.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `pokerengine-1.1.3.tar` & `pokerengine-1.1.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     3831 2022-11-09 12:37:21.000000 pokerengine-1.1.3/.clang-format
--rw-r--r--   0        0        0      137 2022-11-09 12:37:21.000000 pokerengine-1.1.3/.github/dependabot.yaml
--rw-r--r--   0        0        0      648 2022-11-09 12:37:21.000000 pokerengine-1.1.3/.github/workflows/pre-commit-updater.yml
--rw-r--r--   0        0        0      578 2022-11-09 12:37:21.000000 pokerengine-1.1.3/.gitignore
--rw-r--r--   0        0        0      563 2022-11-09 12:37:21.000000 pokerengine-1.1.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2042 2022-11-09 12:37:21.000000 pokerengine-1.1.3/CMakeLists.txt
--rw-r--r--   0        0        0       33 2022-11-09 12:37:21.000000 pokerengine-1.1.3/README.md
--rw-r--r--   0        0        0      970 2022-11-09 12:37:21.000000 pokerengine-1.1.3/examples/hand_straight.py
--rw-r--r--   0        0        0      544 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/bits.hpp
--rw-r--r--   0        0        0     7686 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/card/card.hpp
--rw-r--r--   0        0        0     2663 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/card/cards.hpp
--rw-r--r--   0        0        0     3223 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/card/hand.hpp
--rw-r--r--   0        0        0     1556 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/constants.hpp
--rw-r--r--   0        0        0    31480 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/engine.hpp
--rw-r--r--   0        0        0     3221 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/enums.hpp
--rw-r--r--   0        0        0     4460 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/evaluator/evaluation.hpp
--rw-r--r--   0        0        0     1552 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/evaluator/evaluation_result.hpp
--rw-r--r--   0        0        0   136152 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/evaluator/lookup_tables.hpp
--rw-r--r--   0        0        0     5387 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/evaluator/result.hpp
--rw-r--r--   0        0        0      305 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/pokerengine.hpp
--rw-r--r--   0        0        0     8217 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/python/pycard.hpp
--rw-r--r--   0        0        0     1856 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/python/pyconstants.hpp
--rw-r--r--   0        0        0    11836 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/python/pyengine.hpp
--rw-r--r--   0        0        0     5720 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/python/pyenums.hpp
--rw-r--r--   0        0        0     2586 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/python/pyevaluation.hpp
--rw-r--r--   0        0        0      240 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/python/python.hpp
--rw-r--r--   0        0        0     1327 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/string.hpp
--rw-r--r--   0        0        0      278 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/types.hpp
--rw-r--r--   0        0        0     1070 2022-11-09 12:37:21.000000 pokerengine-1.1.3/include/pokerengine/vector.hpp
--rw-r--r--   0        0        0     1069 2022-11-09 12:37:21.000000 pokerengine-1.1.3/licenses/MIT
--rw-r--r--   0        0        0     1190 2022-11-09 12:37:21.000000 pokerengine-1.1.3/pyproject.toml
--rw-r--r--   0        0        0      302 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/__init__.py
--rw-r--r--   0        0        0      281 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/card.py
--rw-r--r--   0        0        0      782 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/constants.py
--rw-r--r--   0        0        0      435 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/engine.py
--rw-r--r--   0        0        0      593 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/enums.py
--rw-r--r--   0        0        0      253 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/evaluation.py
--rw-r--r--   0        0        0      323 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/pokerengine_core/__init__.pyi
--rw-r--r--   0        0        0     7462 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/pokerengine_core/card.pyi
--rw-r--r--   0        0        0      644 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/pokerengine_core/constants.pyi
--rw-r--r--   0        0        0     7863 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/pokerengine_core/engine.pyi
--rw-r--r--   0        0        0      220 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/pokerengine_core/enums/__init__.pyi
--rw-r--r--   0        0        0      221 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/pokerengine_core/enums/action.pyi
--rw-r--r--   0        0        0      320 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/pokerengine_core/enums/combination.pyi
--rw-r--r--   0        0        0      239 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/pokerengine_core/enums/position.pyi
--rw-r--r--   0        0        0      293 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/pokerengine_core/enums/rank.pyi
--rw-r--r--   0        0        0      210 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/pokerengine_core/enums/round.pyi
--rw-r--r--   0        0        0      204 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/pokerengine_core/enums/state.pyi
--rw-r--r--   0        0        0      182 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/pokerengine_core/enums/suit.pyi
--rw-r--r--   0        0        0     2418 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/pokerengine_core/evaluation.pyi
--rw-r--r--   0        0        0      149 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine/pokerengine_core/utils.pyi
--rw-r--r--   0        0        0      922 2022-11-09 12:37:21.000000 pokerengine-1.1.3/src/pokerengine.cpp
--rw-r--r--   0        0        0      703 2022-11-09 12:37:21.000000 pokerengine-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     3831 2022-11-09 12:37:21.000000 pokerengine-1.1.4/.clang-format
+-rw-r--r--   0        0        0      137 2022-11-09 12:37:21.000000 pokerengine-1.1.4/.github/dependabot.yaml
+-rw-r--r--   0        0        0      648 2022-11-09 12:37:21.000000 pokerengine-1.1.4/.github/workflows/pre-commit-updater.yml
+-rw-r--r--   0        0        0      578 2022-11-09 12:37:21.000000 pokerengine-1.1.4/.gitignore
+-rw-r--r--   0        0        0      563 2022-11-09 12:37:21.000000 pokerengine-1.1.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2042 2022-11-09 12:37:21.000000 pokerengine-1.1.4/CMakeLists.txt
+-rw-r--r--   0        0        0       33 2022-11-09 12:37:21.000000 pokerengine-1.1.4/README.md
+-rw-r--r--   0        0        0      970 2022-11-09 12:37:21.000000 pokerengine-1.1.4/examples/hand_straight.py
+-rw-r--r--   0        0        0      544 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/bits.hpp
+-rw-r--r--   0        0        0     7514 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/card/card.hpp
+-rw-r--r--   0        0        0     2663 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/card/cards.hpp
+-rw-r--r--   0        0        0     3206 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/card/hand.hpp
+-rw-r--r--   0        0        0     1556 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/constants.hpp
+-rw-r--r--   0        0        0    31498 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/engine.hpp
+-rw-r--r--   0        0        0     3119 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/enums.hpp
+-rw-r--r--   0        0        0     4460 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/evaluator/evaluation.hpp
+-rw-r--r--   0        0        0     1552 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/evaluator/evaluation_result.hpp
+-rw-r--r--   0        0        0   136152 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/evaluator/lookup_tables.hpp
+-rw-r--r--   0        0        0     5387 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/evaluator/result.hpp
+-rw-r--r--   0        0        0      305 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/pokerengine.hpp
+-rw-r--r--   0        0        0     8217 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/python/pycard.hpp
+-rw-r--r--   0        0        0     1856 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/python/pyconstants.hpp
+-rw-r--r--   0        0        0    11836 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/python/pyengine.hpp
+-rw-r--r--   0        0        0     5720 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/python/pyenums.hpp
+-rw-r--r--   0        0        0     2586 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/python/pyevaluation.hpp
+-rw-r--r--   0        0        0      240 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/python/python.hpp
+-rw-r--r--   0        0        0     1327 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/string.hpp
+-rw-r--r--   0        0        0      278 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/types.hpp
+-rw-r--r--   0        0        0     1070 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/vector.hpp
+-rw-r--r--   0        0        0     1069 2022-11-09 12:37:21.000000 pokerengine-1.1.4/licenses/MIT
+-rw-r--r--   0        0        0     1190 2022-11-09 12:37:21.000000 pokerengine-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0      302 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/__init__.py
+-rw-r--r--   0        0        0      281 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/card.py
+-rw-r--r--   0        0        0      782 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/constants.py
+-rw-r--r--   0        0        0      435 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/engine.py
+-rw-r--r--   0        0        0      593 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/enums.py
+-rw-r--r--   0        0        0      253 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/evaluation.py
+-rw-r--r--   0        0        0      323 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/pokerengine_core/__init__.pyi
+-rw-r--r--   0        0        0     7462 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/pokerengine_core/card.pyi
+-rw-r--r--   0        0        0      644 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/pokerengine_core/constants.pyi
+-rw-r--r--   0        0        0     7863 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/pokerengine_core/engine.pyi
+-rw-r--r--   0        0        0      220 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/pokerengine_core/enums/__init__.pyi
+-rw-r--r--   0        0        0      221 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/pokerengine_core/enums/action.pyi
+-rw-r--r--   0        0        0      320 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/pokerengine_core/enums/combination.pyi
+-rw-r--r--   0        0        0      239 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/pokerengine_core/enums/position.pyi
+-rw-r--r--   0        0        0      293 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/pokerengine_core/enums/rank.pyi
+-rw-r--r--   0        0        0      210 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/pokerengine_core/enums/round.pyi
+-rw-r--r--   0        0        0      204 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/pokerengine_core/enums/state.pyi
+-rw-r--r--   0        0        0      182 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/pokerengine_core/enums/suit.pyi
+-rw-r--r--   0        0        0     2418 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/pokerengine_core/evaluation.pyi
+-rw-r--r--   0        0        0      149 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/pokerengine_core/utils.pyi
+-rw-r--r--   0        0        0      922 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine.cpp
+-rw-r--r--   0        0        0      703 2022-11-09 12:37:21.000000 pokerengine-1.1.4/PKG-INFO
```

### Comparing `pokerengine-1.1.3/.clang-format` & `pokerengine-1.1.4/.clang-format`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.3/.github/workflows/pre-commit-updater.yml` & `pokerengine-1.1.4/.github/workflows/pre-commit-updater.yml`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.3/.gitignore` & `pokerengine-1.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.3/.pre-commit-config.yaml` & `pokerengine-1.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.3/CMakeLists.txt` & `pokerengine-1.1.4/CMakeLists.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 cmake_minimum_required(VERSION 3.12)
 
-project(pokerengine VERSION 1.1.3)
+project(pokerengine VERSION 1.1.4)
 
 set(CMAKE_CXX_STANDARD 20)
 set(CMAKE_CXX_STANDARD_REQUIRED ON)
 set(CMAKE_CXX_EXTENSIONS OFF)
 
 
 set(LIBRARY_NAME pokerengine_core)
```

### Comparing `pokerengine-1.1.3/examples/hand_straight.py` & `pokerengine-1.1.4/examples/hand_straight.py`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.3/include/pokerengine/bits.hpp` & `pokerengine-1.1.4/include/pokerengine/bits.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.3/include/pokerengine/card/card.hpp` & `pokerengine-1.1.4/include/pokerengine/card/card.hpp`

 * *Files 7% similar despite different names*

```diff
@@ -106,19 +106,19 @@
         return types::bit_set{ 1 } << card_;
     }
 
     [[nodiscard]] auto get_card() const noexcept -> uint8_t {
         return card_;
     }
 
-    [[nodiscard, maybe_unused]] auto get_rank() const noexcept -> rank {
+    [[nodiscard]] auto get_rank() const noexcept -> rank {
         return rank{ enums::rank(uint8_t(card_ % constants::RANKS)) };
     }
 
-    [[nodiscard, maybe_unused]] auto get_suit() const noexcept -> suit {
+    [[nodiscard]] auto get_suit() const noexcept -> suit {
         return suit{ enums::suit(uint8_t(card_ / constants::RANKS)) };
     }
 
 private:
     uint8_t card_;
 };
 
@@ -150,55 +150,55 @@
         }
 
         for (size_t index = 0; index < value.size(); index += 2) {
             cards_ |= card(value.substr(index, 2)).as_bitset();
         }
     }
 
-    [[nodiscard, maybe_unused]] auto size() const noexcept -> size_t {
+    [[nodiscard]] auto size() const noexcept -> size_t {
         return std::popcount(get_cards());
     }
 
-    [[nodiscard, maybe_unused]] auto contains(const card &value) const noexcept -> bool {
+    [[nodiscard]] auto contains(const card &value) const noexcept -> bool {
         return (get_cards() & value.as_bitset()) != 0;
     }
 
-    [[nodiscard, maybe_unused]] auto contains(const card_set &value) const noexcept -> bool {
+    [[nodiscard]] auto contains(const card_set &value) const noexcept -> bool {
         return (get_cards() | value.get_cards()) == get_cards();
     }
 
     [[nodiscard]] auto combine(const card &value) const noexcept -> card_set {
         return card_set{ get_cards() | value.as_bitset() };
     }
 
     [[nodiscard]] auto combine(const card_set &value) const noexcept -> card_set {
         return card_set{ get_cards() | value.get_cards() };
     }
 
-    [[maybe_unused]] auto clear() noexcept -> void {
+    auto clear() noexcept -> void {
         set_cards(0);
     }
 
-    [[maybe_unused]] auto fill() noexcept -> void {
+    auto fill() noexcept -> void {
         set_cards(constants::CARD_SET_FULL);
     }
 
-    [[maybe_unused]] auto insert(const card &value) noexcept -> void {
+    auto insert(const card &value) noexcept -> void {
         set_cards(get_cards() | value.as_bitset());
     }
 
-    [[maybe_unused]] auto join(const card_set &value) noexcept -> void {
+    auto join(const card_set &value) noexcept -> void {
         set_cards(get_cards() | value.get_cards());
     }
 
-    [[maybe_unused]] auto remove(const card &value) noexcept -> void {
+    auto remove(const card &value) noexcept -> void {
         set_cards(get_cards() ^ value.as_bitset());
     }
 
-    [[maybe_unused]] auto remove(const card_set value) noexcept -> void {
+    auto remove(const card_set value) noexcept -> void {
         set_cards(get_cards() ^ value.get_cards());
     }
 
     [[nodiscard]] auto get_cards() const noexcept -> uint64_t {
         return cards_;
     }
```

### Comparing `pokerengine-1.1.3/include/pokerengine/card/cards.hpp` & `pokerengine-1.1.4/include/pokerengine/card/cards.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.3/include/pokerengine/card/hand.hpp` & `pokerengine-1.1.4/include/pokerengine/card/hand.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
     template < std::enable_if_t< is_card_v< T > && N == 2, int > = 0 >
     hand_helper(uint8_t first, uint8_t second) noexcept(allow_duplicates)
             : hand_helper{ T{ first }, T{ second } } {
     }
 
     template < std::enable_if_t< N == 2, int > = 0 >
-    [[maybe_unused]] explicit hand_helper(std::string_view str)
+    explicit hand_helper(std::string_view str)
             : hand_helper(T{ str.substr(0 * char_count, char_count) },
                           T{ str.substr(1 * char_count, char_count) }) {
         if (str.size() != 2 * char_count) {
             throw std::runtime_error{ "Tried to create a hand with a string of wrong size" };
         }
     }
```

### Comparing `pokerengine-1.1.3/include/pokerengine/constants.hpp` & `pokerengine-1.1.4/include/pokerengine/constants.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.3/include/pokerengine/engine.hpp` & `pokerengine-1.1.4/include/pokerengine/engine.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -390,15 +390,15 @@
         }
     }
 
     return result;
 }
 
 auto get_next_round(enums::round round) -> std::tuple< enums::round, bool > {
-    auto result = static_cast< enums::round >(static_cast< uint8_t >(round) + 1);
+    auto result = static_cast< enums::round >(static_cast< int8_t >(round) + 1);
     return std::make_tuple(result, result == enums::round::flop);
 }
 } // namespace v1
 
 template < typename Engine >
 class players_manager : public actual::engine_detail< Engine > {
 public:
@@ -636,15 +636,15 @@
     }
 
     [[nodiscard]] auto pot_rake() noexcept -> int32_t {
         auto flop_dealt = this->engine.round.get_flop_dealt();
         return flop_dealt ? static_cast< int32_t >(pot() * constants::RAKE_MULTI< A, B >) : pot();
     }
 
-    [[maybe_unused]] auto pay(const cards &cards) -> std::vector< std::pair< result, int32_t > > {
+    auto pay(const cards &cards) -> std::vector< std::pair< result, int32_t > > {
         auto iterable = this->engine.players.get_players();
         auto pots = actual::get_all_pots(iterable, get_highest_bet());
         auto chips = std::accumulate(
                         pots.cbegin(),
                         pots.cend(),
                         std::vector< int32_t >{},
                         [&](auto value, const auto &element) {
@@ -664,15 +664,15 @@
             player.stack += result.second;
         });
         this->engine.players.set_players(iterable);
 
         return results;
     }
 
-    [[maybe_unused]] auto pay_noshowdown() -> std::vector< int32_t > {
+    auto pay_noshowdown() -> std::vector< int32_t > {
         auto iterable = this->engine.players.get_players();
         auto adjusted_pot = actual::get_adjust_pot< A, B >(
                         iterable, get_highest_bet(), this->engine.round.get_flop_dealt());
         auto winner = std::distance(
                         iterable.cbegin(),
                         std::find_if(iterable.cbegin(), iterable.cend(), [](const auto &element) {
                             return element.state != enums::state::out;
@@ -802,14 +802,16 @@
         actual::set_blinds(new_players, engine_traits_.get_sb_bet(), engine_traits_.get_bb_bet());
 
         players.set_players(new_players);
 
         if (actual::is_all_allin(new_players)) {
             round.set_round(enums::round::showdown);
         } else {
+            round.set_round(enums::round::preflop);
+
             positions.set_current(
                             new_players.size() > constants::MIN_PLAYERS ? enums::position::utg :
                                                                           enums::position::sb);
 
             if (positions.get_player().state == enums::state::allin) {
                 positions.set_next_current();
             }
```

### Comparing `pokerengine-1.1.3/include/pokerengine/enums.hpp` & `pokerengine-1.1.4/include/pokerengine/enums.hpp`

 * *Files 24% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     call = 2,
     bet = 3,
     raise = 4,
     allin = 5,
 };
 
 enum class combination : int8_t {
-    none [[maybe_unused]] = -1,
+    none = -1,
     no_pair = 0,
     one_pair = 1,
     two_pair = 2,
     three_of_a_kind = 3,
     straight = 4,
     flush = 5,
     full_house = 6,
@@ -36,18 +36,18 @@
 };
 
 enum class position : int8_t {
     none = -1,
     sb = 0,
     bb = 1,
     utg = 2,
-    lwj [[maybe_unused]] = 3,
-    hij [[maybe_unused]] = 4,
-    cof [[maybe_unused]] = 5,
-    btn [[maybe_unused]] = 6,
+    lwj = 3,
+    hij = 4,
+    cof = 5,
+    btn = 6,
 };
 
 enum class rank : uint8_t {
     two = 0,
     three = 1,
     four = 2,
     five = 3,
@@ -62,15 +62,15 @@
     ace = 12,
 };
 
 enum class round : int8_t {
     none = -1,
     preflop = 0,
     flop = 1,
-    turn [[maybe_unused]] = 2,
+    turn = 2,
     river = 3,
     showdown = 4,
 };
 
 enum class state : int8_t {
     none = -1,
     init = 0,
```

### Comparing `pokerengine-1.1.3/include/pokerengine/evaluator/evaluation.hpp` & `pokerengine-1.1.4/include/pokerengine/evaluator/evaluation.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.3/include/pokerengine/evaluator/evaluation_result.hpp` & `pokerengine-1.1.4/include/pokerengine/evaluator/evaluation_result.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.3/include/pokerengine/evaluator/lookup_tables.hpp` & `pokerengine-1.1.4/include/pokerengine/evaluator/lookup_tables.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.3/include/pokerengine/evaluator/result.hpp` & `pokerengine-1.1.4/include/pokerengine/evaluator/result.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.3/include/pokerengine/python/pycard.hpp` & `pokerengine-1.1.4/include/pokerengine/python/pycard.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.3/include/pokerengine/python/pyconstants.hpp` & `pokerengine-1.1.4/include/pokerengine/python/pyconstants.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.3/include/pokerengine/python/pyengine.hpp` & `pokerengine-1.1.4/include/pokerengine/python/pyengine.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.3/include/pokerengine/python/pyenums.hpp` & `pokerengine-1.1.4/include/pokerengine/python/pyenums.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.3/include/pokerengine/python/pyevaluation.hpp` & `pokerengine-1.1.4/include/pokerengine/python/pyevaluation.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.3/include/pokerengine/string.hpp` & `pokerengine-1.1.4/include/pokerengine/string.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.3/include/pokerengine/vector.hpp` & `pokerengine-1.1.4/include/pokerengine/vector.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.3/licenses/MIT` & `pokerengine-1.1.4/licenses/MIT`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.3/pyproject.toml` & `pokerengine-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["scikit-build-core==0.6.1", "pybind11"]
 build-backend = "scikit_build_core.build"
 
 [project]
 name = "pokerengine"
-version = "1.1.3"
+version = "1.1.4"
 description = "Poker Library"
 readme = "README.md"
 authors = [
     {name = "raindinners"}
 ]
 requires-python = ">=3.8"
 keywords = [
```

### Comparing `pokerengine-1.1.3/src/pokerengine/constants.py` & `pokerengine-1.1.4/src/pokerengine/constants.py`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.3/src/pokerengine/enums.py` & `pokerengine-1.1.4/src/pokerengine/enums.py`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.3/src/pokerengine/pokerengine_core/card.pyi` & `pokerengine-1.1.4/src/pokerengine/pokerengine_core/card.pyi`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.3/src/pokerengine/pokerengine_core/constants.pyi` & `pokerengine-1.1.4/src/pokerengine/pokerengine_core/constants.pyi`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.3/src/pokerengine/pokerengine_core/engine.pyi` & `pokerengine-1.1.4/src/pokerengine/pokerengine_core/engine.pyi`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.3/src/pokerengine/pokerengine_core/evaluation.pyi` & `pokerengine-1.1.4/src/pokerengine/pokerengine_core/evaluation.pyi`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.3/src/pokerengine.cpp` & `pokerengine-1.1.4/src/pokerengine.cpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.3/PKG-INFO` & `pokerengine-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pokerengine
-Version: 1.1.3
+Version: 1.1.4
 Summary: Poker Library
 Keywords: raindinners,engine,poker,texas,holdem,texas-holdem,texas_holdem,pybind11,scikit-build-core,fast,c++,magic_enum,stubs,python-stubs,python_stubs,pythonstubs,py-stubs,py_stubs,pystubs
 Author: raindinners
 Requires-Python: >=3.8
 Provides-Extra: dev
 Provides-Extra: build
 Requires-Dist: black~=23.10.0; extra == "dev"
```

