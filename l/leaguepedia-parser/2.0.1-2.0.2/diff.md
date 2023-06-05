# Comparing `tmp/leaguepedia_parser-2.0.1.tar.gz` & `tmp/leaguepedia_parser-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leaguepedia_parser-2.0.1.tar", max compression
+gzip compressed data, was "leaguepedia_parser-2.0.2.tar", max compression
```

## Comparing `leaguepedia_parser-2.0.1.tar` & `leaguepedia_parser-2.0.2.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     1062 2021-12-08 02:04:39.955927 leaguepedia_parser-2.0.1/LICENSE
--rw-r--r--   0        0        0      289 2021-12-08 02:25:23.425941 leaguepedia_parser-2.0.1/leaguepedia_parser/__init__.py
--rw-r--r--   0        0        0       84 2021-12-08 02:04:39.955927 leaguepedia_parser-2.0.1/leaguepedia_parser/logger.py
--rw-r--r--   0        0        0     5632 2021-12-08 02:25:23.425941 leaguepedia_parser-2.0.1/leaguepedia_parser/parsers/game_parser.py
--rw-r--r--   0        0        0     3841 2021-12-08 02:25:23.425941 leaguepedia_parser-2.0.1/leaguepedia_parser/parsers/team_parser.py
--rw-r--r--   0        0        0     1455 2021-12-08 02:25:23.425941 leaguepedia_parser-2.0.1/leaguepedia_parser/site/leaguepedia.py
--rw-r--r--   0        0        0     1762 2021-12-08 02:25:23.425941 leaguepedia_parser-2.0.1/leaguepedia_parser/transmuters/field_names.py
--rw-r--r--   0        0        0     3540 2022-07-21 01:31:30.563161 leaguepedia_parser-2.0.1/leaguepedia_parser/transmuters/game.py
--rw-r--r--   0        0        0     2209 2021-12-08 02:04:39.955927 leaguepedia_parser-2.0.1/leaguepedia_parser/transmuters/game_players.py
--rw-r--r--   0        0        0      564 2021-12-08 02:25:23.425941 leaguepedia_parser-2.0.1/leaguepedia_parser/transmuters/picks_bans.py
--rw-r--r--   0        0        0     1013 2021-12-08 02:25:23.425941 leaguepedia_parser-2.0.1/leaguepedia_parser/transmuters/tournament.py
--rw-r--r--   0        0        0      560 2022-07-21 01:32:47.656764 leaguepedia_parser-2.0.1/pyproject.toml
--rw-r--r--   0        0        0      859 2022-07-21 01:33:03.847495 leaguepedia_parser-2.0.1/setup.py
--rw-r--r--   0        0        0      746 2022-07-21 01:33:03.847769 leaguepedia_parser-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-05 01:26:34.051180 leaguepedia_parser-2.0.2/LICENSE
+-rw-r--r--   0        0        0      289 2023-06-05 01:26:34.051373 leaguepedia_parser-2.0.2/leaguepedia_parser/__init__.py
+-rw-r--r--   0        0        0       84 2023-06-05 01:26:34.051450 leaguepedia_parser-2.0.2/leaguepedia_parser/logger.py
+-rw-r--r--   0        0        0     5632 2023-06-05 01:26:34.051596 leaguepedia_parser-2.0.2/leaguepedia_parser/parsers/game_parser.py
+-rw-r--r--   0        0        0     3841 2023-06-05 01:26:34.051680 leaguepedia_parser-2.0.2/leaguepedia_parser/parsers/team_parser.py
+-rw-r--r--   0        0        0     1455 2023-06-05 01:26:34.051798 leaguepedia_parser-2.0.2/leaguepedia_parser/site/leaguepedia.py
+-rw-r--r--   0        0        0     1788 2023-06-05 01:26:34.051913 leaguepedia_parser-2.0.2/leaguepedia_parser/transmuters/field_names.py
+-rw-r--r--   0        0        0     3956 2023-06-05 01:26:34.052011 leaguepedia_parser-2.0.2/leaguepedia_parser/transmuters/game.py
+-rw-r--r--   0        0        0     2209 2023-06-05 01:26:34.052110 leaguepedia_parser-2.0.2/leaguepedia_parser/transmuters/game_players.py
+-rw-r--r--   0        0        0      564 2023-06-05 01:26:34.052185 leaguepedia_parser-2.0.2/leaguepedia_parser/transmuters/picks_bans.py
+-rw-r--r--   0        0        0     1013 2023-06-05 01:26:34.052253 leaguepedia_parser-2.0.2/leaguepedia_parser/transmuters/tournament.py
+-rw-r--r--   0        0        0      559 2023-06-05 01:26:34.056330 leaguepedia_parser-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0      795 1970-01-01 00:00:00.000000 leaguepedia_parser-2.0.2/PKG-INFO
```

### Comparing `leaguepedia_parser-2.0.1/LICENSE` & `leaguepedia_parser-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `leaguepedia_parser-2.0.1/leaguepedia_parser/parsers/game_parser.py` & `leaguepedia_parser-2.0.2/leaguepedia_parser/parsers/game_parser.py`

 * *Files identical despite different names*

### Comparing `leaguepedia_parser-2.0.1/leaguepedia_parser/parsers/team_parser.py` & `leaguepedia_parser-2.0.2/leaguepedia_parser/parsers/team_parser.py`

 * *Files identical despite different names*

### Comparing `leaguepedia_parser-2.0.1/leaguepedia_parser/site/leaguepedia.py` & `leaguepedia_parser-2.0.2/leaguepedia_parser/site/leaguepedia.py`

 * *Files identical despite different names*

### Comparing `leaguepedia_parser-2.0.1/leaguepedia_parser/transmuters/field_names.py` & `leaguepedia_parser-2.0.2/leaguepedia_parser/transmuters/field_names.py`

 * *Files 13% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     "Team2Towers",
     "Team1RiftHeralds",
     "Team2RiftHeralds",
     "Team1Inhibitors",
     "Team2Inhibitors",
     "Patch",
     "MatchHistory",
+    "RiotPlatformGameId",
     "VOD",
     "Gamename",
     "N_GameInMatch",
     "OverviewPage",
 }
```

### Comparing `leaguepedia_parser-2.0.1/leaguepedia_parser/transmuters/game.py` & `leaguepedia_parser-2.0.2/leaguepedia_parser/transmuters/game.py`

 * *Files 10% similar despite different names*

```diff
@@ -106,9 +106,18 @@
         game_hash = query["gameHash"][0]
 
         setattr(
             game.sources,
             "riotLolApi",
             RiotGameSource(gameId=game_id, platformId=platform_id, gameHash=game_hash),
         )
+    # For new tournaments, where the ID is directly input in the wiki instead of the match history URL.
+    elif not source_dict.get("MatchHistory") and source_dict.get("RiotPlatformGameId"):
+        platform_id, game_id = source_dict["RiotPlatformGameId"].split("_")
+
+        setattr(
+            game.sources,
+            "riotLolApi",
+            RiotGameSource(gameId=game_id, platformId=platform_id),
+        )
 
     return game
```

### Comparing `leaguepedia_parser-2.0.1/leaguepedia_parser/transmuters/game_players.py` & `leaguepedia_parser-2.0.2/leaguepedia_parser/transmuters/game_players.py`

 * *Files identical despite different names*

### Comparing `leaguepedia_parser-2.0.1/leaguepedia_parser/transmuters/picks_bans.py` & `leaguepedia_parser-2.0.2/leaguepedia_parser/transmuters/picks_bans.py`

 * *Files identical despite different names*

### Comparing `leaguepedia_parser-2.0.1/leaguepedia_parser/transmuters/tournament.py` & `leaguepedia_parser-2.0.2/leaguepedia_parser/transmuters/tournament.py`

 * *Files identical despite different names*

