# Comparing `tmp/pokerengine-1.1.4.tar.gz` & `tmp/pokerengine-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokerengine-1.1.4.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "pokerengine-1.1.5.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `pokerengine-1.1.4.tar` & `pokerengine-1.1.5.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     3831 2022-11-09 12:37:21.000000 pokerengine-1.1.4/.clang-format
--rw-r--r--   0        0        0      137 2022-11-09 12:37:21.000000 pokerengine-1.1.4/.github/dependabot.yaml
--rw-r--r--   0        0        0      648 2022-11-09 12:37:21.000000 pokerengine-1.1.4/.github/workflows/pre-commit-updater.yml
--rw-r--r--   0        0        0      578 2022-11-09 12:37:21.000000 pokerengine-1.1.4/.gitignore
--rw-r--r--   0        0        0      563 2022-11-09 12:37:21.000000 pokerengine-1.1.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2042 2022-11-09 12:37:21.000000 pokerengine-1.1.4/CMakeLists.txt
--rw-r--r--   0        0        0       33 2022-11-09 12:37:21.000000 pokerengine-1.1.4/README.md
--rw-r--r--   0        0        0      970 2022-11-09 12:37:21.000000 pokerengine-1.1.4/examples/hand_straight.py
--rw-r--r--   0        0        0      544 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/bits.hpp
--rw-r--r--   0        0        0     7514 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/card/card.hpp
--rw-r--r--   0        0        0     2663 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/card/cards.hpp
--rw-r--r--   0        0        0     3206 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/card/hand.hpp
--rw-r--r--   0        0        0     1556 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/constants.hpp
--rw-r--r--   0        0        0    31498 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/engine.hpp
--rw-r--r--   0        0        0     3119 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/enums.hpp
--rw-r--r--   0        0        0     4460 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/evaluator/evaluation.hpp
--rw-r--r--   0        0        0     1552 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/evaluator/evaluation_result.hpp
--rw-r--r--   0        0        0   136152 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/evaluator/lookup_tables.hpp
--rw-r--r--   0        0        0     5387 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/evaluator/result.hpp
--rw-r--r--   0        0        0      305 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/pokerengine.hpp
--rw-r--r--   0        0        0     8217 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/python/pycard.hpp
--rw-r--r--   0        0        0     1856 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/python/pyconstants.hpp
--rw-r--r--   0        0        0    11836 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/python/pyengine.hpp
--rw-r--r--   0        0        0     5720 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/python/pyenums.hpp
--rw-r--r--   0        0        0     2586 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/python/pyevaluation.hpp
--rw-r--r--   0        0        0      240 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/python/python.hpp
--rw-r--r--   0        0        0     1327 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/string.hpp
--rw-r--r--   0        0        0      278 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/types.hpp
--rw-r--r--   0        0        0     1070 2022-11-09 12:37:21.000000 pokerengine-1.1.4/include/pokerengine/vector.hpp
--rw-r--r--   0        0        0     1069 2022-11-09 12:37:21.000000 pokerengine-1.1.4/licenses/MIT
--rw-r--r--   0        0        0     1190 2022-11-09 12:37:21.000000 pokerengine-1.1.4/pyproject.toml
--rw-r--r--   0        0        0      302 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/__init__.py
--rw-r--r--   0        0        0      281 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/card.py
--rw-r--r--   0        0        0      782 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/constants.py
--rw-r--r--   0        0        0      435 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/engine.py
--rw-r--r--   0        0        0      593 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/enums.py
--rw-r--r--   0        0        0      253 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/evaluation.py
--rw-r--r--   0        0        0      323 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/pokerengine_core/__init__.pyi
--rw-r--r--   0        0        0     7462 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/pokerengine_core/card.pyi
--rw-r--r--   0        0        0      644 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/pokerengine_core/constants.pyi
--rw-r--r--   0        0        0     7863 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/pokerengine_core/engine.pyi
--rw-r--r--   0        0        0      220 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/pokerengine_core/enums/__init__.pyi
--rw-r--r--   0        0        0      221 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/pokerengine_core/enums/action.pyi
--rw-r--r--   0        0        0      320 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/pokerengine_core/enums/combination.pyi
--rw-r--r--   0        0        0      239 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/pokerengine_core/enums/position.pyi
--rw-r--r--   0        0        0      293 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/pokerengine_core/enums/rank.pyi
--rw-r--r--   0        0        0      210 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/pokerengine_core/enums/round.pyi
--rw-r--r--   0        0        0      204 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/pokerengine_core/enums/state.pyi
--rw-r--r--   0        0        0      182 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/pokerengine_core/enums/suit.pyi
--rw-r--r--   0        0        0     2418 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/pokerengine_core/evaluation.pyi
--rw-r--r--   0        0        0      149 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine/pokerengine_core/utils.pyi
--rw-r--r--   0        0        0      922 2022-11-09 12:37:21.000000 pokerengine-1.1.4/src/pokerengine.cpp
--rw-r--r--   0        0        0      703 2022-11-09 12:37:21.000000 pokerengine-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     3831 2022-11-09 12:37:21.000000 pokerengine-1.1.5/.clang-format
+-rw-r--r--   0        0        0      137 2022-11-09 12:37:21.000000 pokerengine-1.1.5/.github/dependabot.yaml
+-rw-r--r--   0        0        0      648 2022-11-09 12:37:21.000000 pokerengine-1.1.5/.github/workflows/pre-commit-updater.yml
+-rw-r--r--   0        0        0      578 2022-11-09 12:37:21.000000 pokerengine-1.1.5/.gitignore
+-rw-r--r--   0        0        0      563 2022-11-09 12:37:21.000000 pokerengine-1.1.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2042 2022-11-09 12:37:21.000000 pokerengine-1.1.5/CMakeLists.txt
+-rw-r--r--   0        0        0       33 2022-11-09 12:37:21.000000 pokerengine-1.1.5/README.md
+-rw-r--r--   0        0        0      970 2022-11-09 12:37:21.000000 pokerengine-1.1.5/examples/hand_straight.py
+-rw-r--r--   0        0        0      544 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/bits.hpp
+-rw-r--r--   0        0        0     7514 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/card/card.hpp
+-rw-r--r--   0        0        0     2663 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/card/cards.hpp
+-rw-r--r--   0        0        0     3206 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/card/hand.hpp
+-rw-r--r--   0        0        0     1556 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/constants.hpp
+-rw-r--r--   0        0        0    31475 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/engine.hpp
+-rw-r--r--   0        0        0     3119 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/enums.hpp
+-rw-r--r--   0        0        0     4460 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/evaluator/evaluation.hpp
+-rw-r--r--   0        0        0     1552 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/evaluator/evaluation_result.hpp
+-rw-r--r--   0        0        0   136152 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/evaluator/lookup_tables.hpp
+-rw-r--r--   0        0        0     5387 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/evaluator/result.hpp
+-rw-r--r--   0        0        0      305 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/pokerengine.hpp
+-rw-r--r--   0        0        0     8217 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/python/pycard.hpp
+-rw-r--r--   0        0        0     1856 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/python/pyconstants.hpp
+-rw-r--r--   0        0        0    11836 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/python/pyengine.hpp
+-rw-r--r--   0        0        0     5720 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/python/pyenums.hpp
+-rw-r--r--   0        0        0     2586 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/python/pyevaluation.hpp
+-rw-r--r--   0        0        0      240 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/python/python.hpp
+-rw-r--r--   0        0        0     1327 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/string.hpp
+-rw-r--r--   0        0        0      278 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/types.hpp
+-rw-r--r--   0        0        0     1070 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/vector.hpp
+-rw-r--r--   0        0        0     1069 2022-11-09 12:37:21.000000 pokerengine-1.1.5/licenses/MIT
+-rw-r--r--   0        0        0     1190 2022-11-09 12:37:21.000000 pokerengine-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0      302 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/__init__.py
+-rw-r--r--   0        0        0      281 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/card.py
+-rw-r--r--   0        0        0      782 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/constants.py
+-rw-r--r--   0        0        0      435 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/engine.py
+-rw-r--r--   0        0        0      593 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/enums.py
+-rw-r--r--   0        0        0      253 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/evaluation.py
+-rw-r--r--   0        0        0      323 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/pokerengine_core/__init__.pyi
+-rw-r--r--   0        0        0     7462 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/pokerengine_core/card.pyi
+-rw-r--r--   0        0        0      644 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/pokerengine_core/constants.pyi
+-rw-r--r--   0        0        0     7863 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/pokerengine_core/engine.pyi
+-rw-r--r--   0        0        0      220 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/pokerengine_core/enums/__init__.pyi
+-rw-r--r--   0        0        0      221 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/pokerengine_core/enums/action.pyi
+-rw-r--r--   0        0        0      320 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/pokerengine_core/enums/combination.pyi
+-rw-r--r--   0        0        0      239 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/pokerengine_core/enums/position.pyi
+-rw-r--r--   0        0        0      293 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/pokerengine_core/enums/rank.pyi
+-rw-r--r--   0        0        0      210 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/pokerengine_core/enums/round.pyi
+-rw-r--r--   0        0        0      204 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/pokerengine_core/enums/state.pyi
+-rw-r--r--   0        0        0      182 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/pokerengine_core/enums/suit.pyi
+-rw-r--r--   0        0        0     2418 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/pokerengine_core/evaluation.pyi
+-rw-r--r--   0        0        0      149 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/pokerengine_core/utils.pyi
+-rw-r--r--   0        0        0      922 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine.cpp
+-rw-r--r--   0        0        0      703 2022-11-09 12:37:21.000000 pokerengine-1.1.5/PKG-INFO
```

### Comparing `pokerengine-1.1.4/.clang-format` & `pokerengine-1.1.5/.clang-format`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.4/.github/workflows/pre-commit-updater.yml` & `pokerengine-1.1.5/.github/workflows/pre-commit-updater.yml`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.4/.gitignore` & `pokerengine-1.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.4/.pre-commit-config.yaml` & `pokerengine-1.1.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.4/CMakeLists.txt` & `pokerengine-1.1.5/CMakeLists.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 cmake_minimum_required(VERSION 3.12)
 
-project(pokerengine VERSION 1.1.4)
+project(pokerengine VERSION 1.1.5)
 
 set(CMAKE_CXX_STANDARD 20)
 set(CMAKE_CXX_STANDARD_REQUIRED ON)
 set(CMAKE_CXX_EXTENSIONS OFF)
 
 
 set(LIBRARY_NAME pokerengine_core)
```

### Comparing `pokerengine-1.1.4/examples/hand_straight.py` & `pokerengine-1.1.5/examples/hand_straight.py`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.4/include/pokerengine/bits.hpp` & `pokerengine-1.1.5/include/pokerengine/bits.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.4/include/pokerengine/card/card.hpp` & `pokerengine-1.1.5/include/pokerengine/card/card.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.4/include/pokerengine/card/cards.hpp` & `pokerengine-1.1.5/include/pokerengine/card/cards.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.4/include/pokerengine/card/hand.hpp` & `pokerengine-1.1.5/include/pokerengine/card/hand.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.4/include/pokerengine/constants.hpp` & `pokerengine-1.1.5/include/pokerengine/constants.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.4/include/pokerengine/engine.hpp` & `pokerengine-1.1.5/include/pokerengine/engine.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -80,20 +80,21 @@
     }
 
 protected:
     Engine &engine;
 };
 
 auto is_no_actions_available(enums::round round, enums::state state) noexcept -> bool {
-    return (state == enums::state::out || state == enums::state::allin) || round == enums::round::showdown;
+    return (state == enums::state::out || state == enums::state::allin) || round == enums::round::none ||
+                    round == enums::round::showdown;
 }
 
 auto get_fold_or_check(enums::position player, int32_t highest_round_bet, int32_t committed) noexcept
                 -> player_action {
-    if (committed == highest_round_bet) {
+    if (committed == highest_round_bet || !highest_round_bet) {
         return player_action{ 0, enums::action::check, player };
     }
     return player_action{ 0, enums::action::fold, player };
 }
 
 auto is_bet_available(int32_t bb_bet, int32_t highest_round_bet, int32_t remaining) noexcept -> bool {
     return !highest_round_bet && remaining > bb_bet;
@@ -238,14 +239,15 @@
     std::for_each(players.begin(), players.end(), [&, index = 0](auto &player) mutable -> void {
         player.state = enums::state::init;
         player.behind = player.stack;
         player.round_bet = 0;
         player.front = 0;
 
         if (index < 2) {
+            player.state = index == 0 ? enums::state::alive : enums::state::init;
             player.front = index == 0 ? sb_bet : bb_bet;
 
             if (player.front > player.behind) {
                 player.front = player.behind;
             }
 
             player.behind -= player.front;
@@ -436,19 +438,14 @@
 
 template < typename Engine >
 class actions_manager : public actual::engine_detail< Engine > {
 public:
     using actual::engine_detail< Engine >::engine_detail;
 
     [[nodiscard]] auto get_possible_actions() const -> std::vector< player_action > {
-        if (this->engine.round.get_round() == enums::round::none ||
-            this->engine.round.get_round() == enums::round::showdown) {
-            return std::vector< player_action >{};
-        }
-
         auto player = this->engine.positions.get_player();
         return actual::get_possible_actions(
                         this->engine.round.get_round(),
                         this->engine.positions.get_current(),
                         player.state,
                         player.is_left,
                         this->engine.get_engine_traits().get_bb_bet(),
@@ -466,15 +463,15 @@
                             this->engine.get_engine_traits().get_min_raise())) {
             throw std::runtime_error{ "Execute action failed" };
         }
 
         auto &player = this->engine.positions.get_player();
         this->engine.get_engine_traits().set_min_raise(actual::execute_action(
                         pa,
-                        this->engine.positions.get_player(),
+                        player,
                         this->engine.get_engine_traits().get_min_raise(),
                         this->engine.pot.get_round_highest_bet()));
 
         auto iterable = this->engine.players.get_players();
         if (auto actions = this->engine.positions.get_actionable();
             this->engine.positions.get_number_alive() < constants::MIN_PLAYERS ||
             (actions == 0 && this->engine.positions.get_future_actionable() < constants::MIN_PLAYERS)) {
@@ -514,14 +511,16 @@
                     element.round_bet = 0;
                     element.state = element.state == enums::state::alive ? enums::state::init : element.state;
                 });
             }
         } else {
             this->engine.positions.set_next_current();
         }
+
+        this->engine.players.set_players(iterable);
     }
 };
 
 template < typename Engine >
 class positions_manager : public actual::engine_detail< Engine > {
 public:
     using actual::engine_detail< Engine >::engine_detail;
```

### Comparing `pokerengine-1.1.4/include/pokerengine/enums.hpp` & `pokerengine-1.1.5/include/pokerengine/enums.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.4/include/pokerengine/evaluator/evaluation.hpp` & `pokerengine-1.1.5/include/pokerengine/evaluator/evaluation.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.4/include/pokerengine/evaluator/evaluation_result.hpp` & `pokerengine-1.1.5/include/pokerengine/evaluator/evaluation_result.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.4/include/pokerengine/evaluator/lookup_tables.hpp` & `pokerengine-1.1.5/include/pokerengine/evaluator/lookup_tables.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.4/include/pokerengine/evaluator/result.hpp` & `pokerengine-1.1.5/include/pokerengine/evaluator/result.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.4/include/pokerengine/python/pycard.hpp` & `pokerengine-1.1.5/include/pokerengine/python/pycard.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.4/include/pokerengine/python/pyconstants.hpp` & `pokerengine-1.1.5/include/pokerengine/python/pyconstants.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.4/include/pokerengine/python/pyengine.hpp` & `pokerengine-1.1.5/include/pokerengine/python/pyengine.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.4/include/pokerengine/python/pyenums.hpp` & `pokerengine-1.1.5/include/pokerengine/python/pyenums.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.4/include/pokerengine/python/pyevaluation.hpp` & `pokerengine-1.1.5/include/pokerengine/python/pyevaluation.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.4/include/pokerengine/string.hpp` & `pokerengine-1.1.5/include/pokerengine/string.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.4/include/pokerengine/vector.hpp` & `pokerengine-1.1.5/include/pokerengine/vector.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.4/licenses/MIT` & `pokerengine-1.1.5/licenses/MIT`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.4/pyproject.toml` & `pokerengine-1.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["scikit-build-core==0.6.1", "pybind11"]
 build-backend = "scikit_build_core.build"
 
 [project]
 name = "pokerengine"
-version = "1.1.4"
+version = "1.1.5"
 description = "Poker Library"
 readme = "README.md"
 authors = [
     {name = "raindinners"}
 ]
 requires-python = ">=3.8"
 keywords = [
```

### Comparing `pokerengine-1.1.4/src/pokerengine/constants.py` & `pokerengine-1.1.5/src/pokerengine/constants.py`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.4/src/pokerengine/enums.py` & `pokerengine-1.1.5/src/pokerengine/enums.py`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.4/src/pokerengine/pokerengine_core/card.pyi` & `pokerengine-1.1.5/src/pokerengine/pokerengine_core/card.pyi`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.4/src/pokerengine/pokerengine_core/constants.pyi` & `pokerengine-1.1.5/src/pokerengine/pokerengine_core/constants.pyi`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.4/src/pokerengine/pokerengine_core/engine.pyi` & `pokerengine-1.1.5/src/pokerengine/pokerengine_core/engine.pyi`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.4/src/pokerengine/pokerengine_core/evaluation.pyi` & `pokerengine-1.1.5/src/pokerengine/pokerengine_core/evaluation.pyi`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.4/src/pokerengine.cpp` & `pokerengine-1.1.5/src/pokerengine.cpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.4/PKG-INFO` & `pokerengine-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pokerengine
-Version: 1.1.4
+Version: 1.1.5
 Summary: Poker Library
 Keywords: raindinners,engine,poker,texas,holdem,texas-holdem,texas_holdem,pybind11,scikit-build-core,fast,c++,magic_enum,stubs,python-stubs,python_stubs,pythonstubs,py-stubs,py_stubs,pystubs
 Author: raindinners
 Requires-Python: >=3.8
 Provides-Extra: dev
 Provides-Extra: build
 Requires-Dist: black~=23.10.0; extra == "dev"
```

