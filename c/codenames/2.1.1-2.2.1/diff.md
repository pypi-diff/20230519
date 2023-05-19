# Comparing `tmp/codenames-2.1.1.tar.gz` & `tmp/codenames-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codenames-2.1.1.tar", last modified: Sat Apr  8 21:49:22 2023, max compression
+gzip compressed data, was "codenames-2.2.1.tar", max compression
```

## Comparing `codenames-2.1.1.tar` & `codenames-2.2.1.tar`

### file list

```diff
@@ -1,55 +1,27 @@
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 21:49:22.972485 codenames-2.1.1/
--rw-rw-r--   0 akali     (1000) akali     (1000)      788 2023-04-08 21:49:22.972485 codenames-2.1.1/PKG-INFO
--rw-rw-r--   0 akali     (1000) akali     (1000)      469 2022-05-18 20:32:47.000000 codenames-2.1.1/README.md
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 21:49:22.964485 codenames-2.1.1/codenames/
--rw-rw-r--   0 akali     (1000) akali     (1000)        0 2022-05-13 11:39:47.000000 codenames-2.1.1/codenames/__init__.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 21:49:22.964485 codenames-2.1.1/codenames/boards/
--rw-rw-r--   0 akali     (1000) akali     (1000)        0 2023-04-08 14:06:47.000000 codenames-2.1.1/codenames/boards/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     2010 2023-04-08 14:40:42.000000 codenames-2.1.1/codenames/boards/builder.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     6098 2022-05-13 11:39:47.000000 codenames-2.1.1/codenames/boards/english.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     6979 2022-05-13 11:39:47.000000 codenames-2.1.1/codenames/boards/hebrew.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 21:49:22.968485 codenames-2.1.1/codenames/game/
--rw-rw-r--   0 akali     (1000) akali     (1000)        0 2023-04-08 14:06:44.000000 codenames-2.1.1/codenames/game/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     1015 2023-04-08 14:33:58.000000 codenames-2.1.1/codenames/game/base.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     4103 2023-04-08 14:42:14.000000 codenames-2.1.1/codenames/game/board.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      928 2023-04-08 14:41:06.000000 codenames-2.1.1/codenames/game/card.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     1200 2023-04-08 14:41:15.000000 codenames-2.1.1/codenames/game/color.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      470 2022-05-13 11:39:47.000000 codenames-2.1.1/codenames/game/exceptions.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     2319 2023-04-08 21:46:43.000000 codenames-2.1.1/codenames/game/move.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     2710 2023-04-08 21:36:30.000000 codenames-2.1.1/codenames/game/player.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     5041 2023-04-08 21:41:55.000000 codenames-2.1.1/codenames/game/runner.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      830 2023-04-08 14:40:42.000000 codenames-2.1.1/codenames/game/score.py
--rw-rw-r--   0 akali     (1000) akali     (1000)    10106 2023-04-08 15:11:15.000000 codenames-2.1.1/codenames/game/state.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      452 2023-04-08 14:40:42.000000 codenames-2.1.1/codenames/game/winner.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 21:49:22.968485 codenames-2.1.1/codenames/online/
--rw-rw-r--   0 akali     (1000) akali     (1000)        0 2023-04-08 14:49:02.000000 codenames-2.1.1/codenames/online/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)    13115 2023-04-08 14:59:45.000000 codenames-2.1.1/codenames/online/online_adapter.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     7862 2023-04-08 14:51:10.000000 codenames-2.1.1/codenames/online/online_game_runner.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     1090 2023-04-08 14:50:37.000000 codenames-2.1.1/codenames/online/online_players.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     2105 2022-05-13 11:39:47.000000 codenames-2.1.1/codenames/online/utils.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 21:49:22.968485 codenames-2.1.1/codenames/utils/
--rw-rw-r--   0 akali     (1000) akali     (1000)        0 2023-04-08 14:59:11.000000 codenames-2.1.1/codenames/utils/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      281 2023-04-08 21:36:52.000000 codenames-2.1.1/codenames/utils/formatting.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 21:49:22.964485 codenames-2.1.1/codenames.egg-info/
--rw-rw-r--   0 akali     (1000) akali     (1000)      788 2023-04-08 21:49:22.000000 codenames-2.1.1/codenames.egg-info/PKG-INFO
--rw-rw-r--   0 akali     (1000) akali     (1000)     1137 2023-04-08 21:49:22.000000 codenames-2.1.1/codenames.egg-info/SOURCES.txt
--rw-rw-r--   0 akali     (1000) akali     (1000)        1 2023-04-08 21:49:22.000000 codenames-2.1.1/codenames.egg-info/dependency_links.txt
--rw-rw-r--   0 akali     (1000) akali     (1000)      110 2023-04-08 21:49:22.000000 codenames-2.1.1/codenames.egg-info/requires.txt
--rw-rw-r--   0 akali     (1000) akali     (1000)       16 2023-04-08 21:49:22.000000 codenames-2.1.1/codenames.egg-info/top_level.txt
--rw-rw-r--   0 akali     (1000) akali     (1000)      728 2023-04-08 08:52:53.000000 codenames-2.1.1/pyproject.toml
--rw-rw-r--   0 akali     (1000) akali     (1000)      183 2023-04-08 21:49:22.972485 codenames-2.1.1/setup.cfg
--rw-rw-r--   0 akali     (1000) akali     (1000)      554 2023-04-08 21:49:00.000000 codenames-2.1.1/setup.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 21:49:22.968485 codenames-2.1.1/tests/
--rw-rw-r--   0 akali     (1000) akali     (1000)        0 2022-05-18 20:04:04.000000 codenames-2.1.1/tests/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     1674 2023-04-08 14:23:07.000000 codenames-2.1.1/tests/board_test.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      750 2023-04-08 14:40:42.000000 codenames-2.1.1/tests/card_test.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     8015 2023-04-08 14:48:49.000000 codenames-2.1.1/tests/flows_test.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     8668 2023-04-08 21:41:54.000000 codenames-2.1.1/tests/game_runner_test.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     7664 2023-04-08 15:12:37.000000 codenames-2.1.1/tests/game_state_test.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      805 2023-04-08 21:36:49.000000 codenames-2.1.1/tests/player_test.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      682 2023-04-08 14:40:42.000000 codenames-2.1.1/tests/serialization_test.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-08 21:49:22.968485 codenames-2.1.1/tests/utils/
--rw-rw-r--   0 akali     (1000) akali     (1000)        0 2022-02-23 19:10:50.000000 codenames-2.1.1/tests/utils/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     3735 2023-04-08 14:40:42.000000 codenames-2.1.1/tests/utils/constants.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     1124 2022-02-23 19:10:50.000000 codenames-2.1.1/tests/utils/hooks.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     2823 2023-04-08 14:41:21.000000 codenames-2.1.1/tests/utils/testing_players.py
+-rw-r--r--   0        0        0      469 2022-05-18 20:32:47.529455 codenames-2.2.1/README.md
+-rw-r--r--   0        0        0        0 2022-05-13 11:39:47.566000 codenames-2.2.1/codenames/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-08 14:06:47.757843 codenames-2.2.1/codenames/boards/__init__.py
+-rw-r--r--   0        0        0     2010 2023-04-08 14:40:42.665619 codenames-2.2.1/codenames/boards/builder.py
+-rw-r--r--   0        0        0     6098 2022-05-13 11:39:47.566000 codenames-2.2.1/codenames/boards/english.py
+-rw-r--r--   0        0        0     6979 2022-05-13 11:39:47.566000 codenames-2.2.1/codenames/boards/hebrew.py
+-rw-r--r--   0        0        0        0 2023-04-08 14:06:44.093797 codenames-2.2.1/codenames/game/__init__.py
+-rw-r--r--   0        0        0     1015 2023-04-08 14:33:58.493179 codenames-2.2.1/codenames/game/base.py
+-rw-r--r--   0        0        0     4103 2023-04-08 14:42:14.217673 codenames-2.2.1/codenames/game/board.py
+-rw-r--r--   0        0        0      928 2023-04-08 14:41:06.774983 codenames-2.2.1/codenames/game/card.py
+-rw-r--r--   0        0        0     1200 2023-04-08 14:41:15.861041 codenames-2.2.1/codenames/game/color.py
+-rw-r--r--   0        0        0      470 2022-05-13 11:39:47.566000 codenames-2.2.1/codenames/game/exceptions.py
+-rw-r--r--   0        0        0     2319 2023-04-08 21:46:43.089095 codenames-2.2.1/codenames/game/move.py
+-rw-r--r--   0        0        0     2710 2023-04-08 21:36:30.990333 codenames-2.2.1/codenames/game/player.py
+-rw-r--r--   0        0        0     5041 2023-04-08 21:41:55.209110 codenames-2.2.1/codenames/game/runner.py
+-rw-r--r--   0        0        0      830 2023-04-08 14:40:42.709628 codenames-2.2.1/codenames/game/score.py
+-rw-r--r--   0        0        0     9791 2023-05-19 13:58:25.117131 codenames-2.2.1/codenames/game/state.py
+-rw-r--r--   0        0        0      452 2023-04-08 14:40:42.713629 codenames-2.2.1/codenames/game/winner.py
+-rw-r--r--   0        0        0        0 2023-04-08 14:49:02.858029 codenames-2.2.1/codenames/online/__init__.py
+-rw-r--r--   0        0        0    13115 2023-04-08 14:59:45.968066 codenames-2.2.1/codenames/online/online_adapter.py
+-rw-r--r--   0        0        0     7862 2023-04-08 14:51:10.790486 codenames-2.2.1/codenames/online/online_game_runner.py
+-rw-r--r--   0        0        0     1090 2023-04-08 14:50:37.695952 codenames-2.2.1/codenames/online/online_players.py
+-rw-r--r--   0        0        0     2105 2022-05-13 11:39:47.570000 codenames-2.2.1/codenames/online/utils.py
+-rw-r--r--   0        0        0        0 2023-04-08 14:59:11.783159 codenames-2.2.1/codenames/utils/__init__.py
+-rw-r--r--   0        0        0      281 2023-04-08 21:36:52.662651 codenames-2.2.1/codenames/utils/formatting.py
+-rw-r--r--   0        0        0     1512 2023-05-19 14:29:22.059589 codenames-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1108 1970-01-01 00:00:00.000000 codenames-2.2.1/PKG-INFO
```

### Comparing `codenames-2.1.1/codenames/boards/builder.py` & `codenames-2.2.1/codenames/boards/builder.py`

 * *Files identical despite different names*

### Comparing `codenames-2.1.1/codenames/boards/english.py` & `codenames-2.2.1/codenames/boards/english.py`

 * *Files identical despite different names*

### Comparing `codenames-2.1.1/codenames/boards/hebrew.py` & `codenames-2.2.1/codenames/boards/hebrew.py`

 * *Files identical despite different names*

### Comparing `codenames-2.1.1/codenames/game/base.py` & `codenames-2.2.1/codenames/game/base.py`

 * *Files identical despite different names*

### Comparing `codenames-2.1.1/codenames/game/board.py` & `codenames-2.2.1/codenames/game/board.py`

 * *Files identical despite different names*

### Comparing `codenames-2.1.1/codenames/game/card.py` & `codenames-2.2.1/codenames/game/card.py`

 * *Files identical despite different names*

### Comparing `codenames-2.1.1/codenames/game/color.py` & `codenames-2.2.1/codenames/game/color.py`

 * *Files identical despite different names*

### Comparing `codenames-2.1.1/codenames/game/move.py` & `codenames-2.2.1/codenames/game/move.py`

 * *Files identical despite different names*

### Comparing `codenames-2.1.1/codenames/game/player.py` & `codenames-2.2.1/codenames/game/player.py`

 * *Files identical despite different names*

### Comparing `codenames-2.1.1/codenames/game/runner.py` & `codenames-2.2.1/codenames/game/runner.py`

 * *Files identical despite different names*

### Comparing `codenames-2.1.1/codenames/game/score.py` & `codenames-2.2.1/codenames/game/score.py`

 * *Files identical despite different names*

### Comparing `codenames-2.1.1/codenames/game/state.py` & `codenames-2.2.1/codenames/game/state.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,14 @@
         return get_moves(
             given_hints=self.given_hints, given_guesses=self.given_guesses, current_turn=self.current_player_role
         )
 
 
 class GameState(BaseGameState):
     left_guesses: int = 0
-    bonus_given: bool = False
     winner: Optional[Winner] = None
     raw_hints: List[Hint] = []
 
     @root_validator(pre=True)
     def init_score(cls, values: dict) -> dict:  # pylint: disable=no-self-argument
         score = values.get("score")
         if score:
@@ -91,15 +90,14 @@
             board=self.board.censured,
             score=self.score,
             current_team_color=self.current_team_color,
             current_player_role=self.current_player_role,
             given_hints=self.given_hints,
             given_guesses=self.given_guesses,
             left_guesses=self.left_guesses,
-            bonus_given=self.bonus_given,
         )
 
     @property
     def last_given_hint(self) -> GivenHint:
         return self.given_hints[-1]
 
     @property
@@ -124,15 +122,15 @@
         if formatted_hint_word in self.hinter_state.illegal_words:
             raise InvalidHint("Hint word is on board or was already used!")
         given_hint = GivenHint(
             word=formatted_hint_word, card_amount=hint.card_amount, team_color=self.current_team_color
         )
         log.info(f"Hinter: {wrap(hint.word)} {hint.card_amount} card(s)")
         self.given_hints.append(given_hint)
-        self.left_guesses = given_hint.card_amount
+        self.left_guesses = given_hint.card_amount + 1
         self.current_player_role = PlayerRole.GUESSER
         return given_hint
 
     def process_guess(self, guess: Guess) -> Optional[GivenGuess]:
         if self.is_game_over:
             raise GameIsOver()
         if self.current_player_role != PlayerRole.GUESSER:
@@ -157,36 +155,30 @@
         if not given_guess.correct:
             log.info("Guesser wrong, turn is over")
             self._end_turn()
             return given_guess
         self.left_guesses -= 1
         if self.left_guesses > 0:
             return given_guess
-        if self.bonus_given:
-            log.info("Bonus already given, turn is over")
-            self._end_turn()
-            return given_guess
-        log.info("Giving bonus guess!")
-        self.bonus_given = True
-        self.left_guesses += 1
+        log.info("Turn is over")
+        self._end_turn()
         return given_guess
 
     def _reveal_guessed_card(self, guess: Guess) -> Card:
         try:
             guessed_card = self.board[guess.card_index]
         except (IndexError, CardNotFoundError) as e:
             raise InvalidGuess("Given card index is out of range!") from e
         if guessed_card.revealed:
             raise InvalidGuess("Given card is already revealed!")
         guessed_card.revealed = True
         return guessed_card
 
     def _end_turn(self, switch_role: bool = True):
         self.left_guesses = 0
-        self.bonus_given = False
         self.current_team_color = self.current_team_color.opponent
         if switch_role:
             self.current_player_role = self.current_player_role.other
 
     def _team_quit(self):
         winner_color = self.current_team_color.opponent
         self.winner = Winner(team_color=winner_color, reason=WinningReason.OPPONENT_QUIT)
@@ -214,15 +206,14 @@
     @cached_property
     def illegal_words(self) -> WordGroup:
         return *self.board.all_words, *self.given_hint_words
 
 
 class GuesserGameState(BaseGameState):
     left_guesses: int
-    bonus_given: bool
 
     @cached_property
     def current_hint(self) -> GivenHint:
         return self.given_hints[-1]
 
 
 def build_game_state(language: str, board: Optional[Board] = None) -> GameState:
```

### Comparing `codenames-2.1.1/codenames/online/online_adapter.py` & `codenames-2.2.1/codenames/online/online_adapter.py`

 * *Files identical despite different names*

### Comparing `codenames-2.1.1/codenames/online/online_game_runner.py` & `codenames-2.2.1/codenames/online/online_game_runner.py`

 * *Files identical despite different names*

### Comparing `codenames-2.1.1/codenames/online/online_players.py` & `codenames-2.2.1/codenames/online/online_players.py`

 * *Files identical despite different names*

### Comparing `codenames-2.1.1/codenames/online/utils.py` & `codenames-2.2.1/codenames/online/utils.py`

 * *Files identical despite different names*

