# Comparing `tmp/nonebot_plugin_game_collection-2.1.5.tar.gz` & `tmp/nonebot_plugin_game_collection-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_game_collection-2.1.5.tar", last modified: Sun Jun  4 13:26:00 2023, max compression
+gzip compressed data, was "nonebot_plugin_game_collection-2.1.6.tar", last modified: Mon Jun  5 05:48:12 2023, max compression
```

## Comparing `nonebot_plugin_game_collection-2.1.5.tar` & `nonebot_plugin_game_collection-2.1.6.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 13:26:00.359868 nonebot_plugin_game_collection-2.1.5/
--rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_game_collection-2.1.5/LICENSE
--rw-rw-rw-   0        0        0      193 2022-12-20 21:13:32.000000 nonebot_plugin_game_collection-2.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0      376 2023-06-04 13:26:00.359368 nonebot_plugin_game_collection-2.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     8291 2022-08-13 12:03:08.000000 nonebot_plugin_game_collection-2.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-04 13:26:00.286893 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/
--rw-rw-rw-   0        0        0    17451 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/Account.py
--rw-rw-rw-   0        0        0    48705 2023-06-04 12:18:21.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/Game.py
-drwxrwxrwx   0        0        0        0 2023-06-04 13:26:00.305030 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/HorseRace/
--rw-rw-rw-   0        0        0    15602 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/HorseRace/events_main.py
--rw-rw-rw-   0        0        0     6399 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/HorseRace/horse.py
--rw-rw-rw-   0        0        0     5151 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/HorseRace/race_group.py
--rw-rw-rw-   0        0        0     9187 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/HorseRace/start.py
--rw-rw-rw-   0        0        0    11410 2023-06-04 13:24:05.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/Manager.py
--rw-rw-rw-   0        0        0    20170 2023-06-04 13:24:04.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/Market.py
--rw-rw-rw-   0        0        0    16202 2023-06-04 11:51:18.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/Prop.py
--rw-rw-rw-   0        0        0    30093 2023-06-04 08:55:32.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/__init__.py
--rw-rw-rw-   0        0        0     3249 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/config.py
-drwxrwxrwx   0        0        0        0 2023-06-04 13:26:00.311539 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/data/
--rw-rw-rw-   0        0        0      525 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/data/api.py
--rw-rw-rw-   0        0        0     5589 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/data/data.py
--rw-rw-rw-   0        0        0      102 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/data/run.py
-drwxrwxrwx   0        0        0        0 2023-06-04 13:26:00.316542 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/
--rw-rw-rw-   0        0        0      171 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/element_library.json
-drwxrwxrwx   0        0        0        0 2023-06-04 13:26:00.347382 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/
--rw-rw-rw-   0        0        0     5488 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/Stand.json
--rw-rw-rw-   0        0        0     4549 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
--rw-rw-rw-   0        0        0     1757 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
--rw-rw-rw-   0        0        0      906 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/基础事件.json
--rw-rw-rw-   0        0        0     2717 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
--rw-rw-rw-   0        0        0     1257 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json
--rw-rw-rw-   0        0        0    22637 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/群友日常.json
--rw-rw-rw-   0        0        0     4751 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json
--rw-rw-rw-   0        0        0     1010 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json
--rw-rw-rw-   0        0        0     2253 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json
--rw-rw-rw-   0        0        0    12958 2023-06-04 12:00:23.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/menu_data.json
--rw-rw-rw-   0        0        0     5375 2023-06-04 11:46:30.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/props_library.json
-drwxrwxrwx   0        0        0        0 2023-06-04 13:26:00.350029 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/subprocess/
--rw-rw-rw-   0        0        0     2245 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/subprocess/ohlc.py
-drwxrwxrwx   0        0        0        0 2023-06-04 13:26:00.356866 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/utils/
--rw-rw-rw-   0        0        0     1321 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/utils/avatar.py
--rw-rw-rw-   0        0        0     7133 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/utils/chart.py
--rw-rw-rw-   0        0        0     1619 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-04 13:26:00.296352 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection.egg-info/
--rw-rw-rw-   0        0        0      376 2023-06-04 13:26:00.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2038 2023-06-04 13:26:00.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 13:26:00.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-06-04 13:26:00.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-06-04 13:26:00.000000 nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 13:26:00.359868 nonebot_plugin_game_collection-2.1.5/setup.cfg
--rw-rw-rw-   0        0        0      738 2023-06-04 13:25:56.000000 nonebot_plugin_game_collection-2.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 05:48:12.808094 nonebot_plugin_game_collection-2.1.6/
+-rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_game_collection-2.1.6/LICENSE
+-rw-rw-rw-   0        0        0      193 2022-12-20 21:13:32.000000 nonebot_plugin_game_collection-2.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      376 2023-06-05 05:48:12.807593 nonebot_plugin_game_collection-2.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     8291 2022-08-13 12:03:08.000000 nonebot_plugin_game_collection-2.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 05:48:12.743672 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/
+-rw-rw-rw-   0        0        0    17451 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/Account.py
+-rw-rw-rw-   0        0        0    48714 2023-06-05 05:46:24.000000 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/Game.py
+drwxrwxrwx   0        0        0        0 2023-06-05 05:48:12.760688 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/HorseRace/
+-rw-rw-rw-   0        0        0    15602 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/HorseRace/events_main.py
+-rw-rw-rw-   0        0        0     6399 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/HorseRace/horse.py
+-rw-rw-rw-   0        0        0     5151 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/HorseRace/race_group.py
+-rw-rw-rw-   0        0        0     9187 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/HorseRace/start.py
+-rw-rw-rw-   0        0        0    11410 2023-06-04 13:24:05.000000 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/Manager.py
+-rw-rw-rw-   0        0        0    20170 2023-06-04 13:24:04.000000 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/Market.py
+-rw-rw-rw-   0        0        0    16202 2023-06-04 11:51:18.000000 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/Prop.py
+-rw-rw-rw-   0        0        0    30278 2023-06-05 05:44:39.000000 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/__init__.py
+-rw-rw-rw-   0        0        0     3249 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/config.py
+drwxrwxrwx   0        0        0        0 2023-06-05 05:48:12.767694 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/data/
+-rw-rw-rw-   0        0        0      525 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/data/api.py
+-rw-rw-rw-   0        0        0     5589 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/data/data.py
+-rw-rw-rw-   0        0        0      102 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/data/run.py
+drwxrwxrwx   0        0        0        0 2023-06-05 05:48:12.772699 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/resource/
+-rw-rw-rw-   0        0        0      171 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/resource/element_library.json
+drwxrwxrwx   0        0        0        0 2023-06-05 05:48:12.796083 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/resource/horserace/
+-rw-rw-rw-   0        0        0     5488 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/resource/horserace/Stand.json
+-rw-rw-rw-   0        0        0     4549 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
+-rw-rw-rw-   0        0        0     1757 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
+-rw-rw-rw-   0        0        0      906 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/resource/horserace/基础事件.json
+-rw-rw-rw-   0        0        0     2717 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
+-rw-rw-rw-   0        0        0     1257 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json
+-rw-rw-rw-   0        0        0    22637 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/resource/horserace/群友日常.json
+-rw-rw-rw-   0        0        0     4751 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json
+-rw-rw-rw-   0        0        0     1010 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json
+-rw-rw-rw-   0        0        0     2253 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json
+-rw-rw-rw-   0        0        0    12958 2023-06-04 12:00:23.000000 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/resource/menu_data.json
+-rw-rw-rw-   0        0        0     5375 2023-06-04 11:46:30.000000 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/resource/props_library.json
+drwxrwxrwx   0        0        0        0 2023-06-05 05:48:12.797585 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/resource/subprocess/
+-rw-rw-rw-   0        0        0     2245 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/resource/subprocess/ohlc.py
+drwxrwxrwx   0        0        0        0 2023-06-05 05:48:12.805593 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/utils/
+-rw-rw-rw-   0        0        0     1321 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/utils/avatar.py
+-rw-rw-rw-   0        0        0     7133 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/utils/chart.py
+-rw-rw-rw-   0        0        0     1619 2023-04-29 02:47:59.000000 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-05 05:48:12.752180 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection.egg-info/
+-rw-rw-rw-   0        0        0      376 2023-06-05 05:48:12.000000 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2038 2023-06-05 05:48:12.000000 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 05:48:12.000000 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-06-05 05:48:12.000000 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-06-05 05:48:12.000000 nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 05:48:12.808094 nonebot_plugin_game_collection-2.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      738 2023-06-05 05:48:06.000000 nonebot_plugin_game_collection-2.1.6/setup.py
```

### Comparing `nonebot_plugin_game_collection-2.1.5/LICENSE` & `nonebot_plugin_game_collection-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.5/README.md` & `nonebot_plugin_game_collection-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/Account.py` & `nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/Account.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/Game.py` & `nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/Game.py`

 * *Files 0% similar despite different names*

```diff
@@ -984,19 +984,19 @@
     """
     flag, msg = start(event, gold)
     if flag == False:
         return msg
     session = current_games[event.group_id]
     session.gold = gold
     session.info = lucky_number_info(gold)
-    return (f"随机牌堆已生成。"
+    return (f"随机 1-100 数字已生成。"
             f"挑战金额：{gold}/次\n"
             f"{msg}")
 
-async def check_card(bot:Bot, event:GroupMessageEvent, N:int):
+async def guess_number(bot:Bot, event:GroupMessageEvent, N:int):
     """
     猜数字
     """
     group_id = event.group_id
     global current_games
     session = current_games[group_id]
     if msg := session.shot_check(event):
```

### Comparing `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/HorseRace/events_main.py` & `nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/HorseRace/events_main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/HorseRace/horse.py` & `nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/HorseRace/horse.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/HorseRace/race_group.py` & `nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/HorseRace/race_group.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/HorseRace/start.py` & `nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/HorseRace/start.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/Manager.py` & `nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/Manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/Market.py` & `nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/Market.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/Prop.py` & `nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/Prop.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/__init__.py` & `nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -363,14 +363,19 @@
     r"^\d{1,3}$",
     rule = lambda event:event.group_id in current_games and current_games[event.group_id].info.get("game") == "lucky_number",
     permission = GROUP,
     priority = 20,
     block = True
     )
 
+@guess_number.handle()
+async def _(bot:Bot, event:GroupMessageEvent):
+    msg = await Game.guess_number(bot, event, int(event.get_plaintext()))
+    await guess_number.finish(msg)
+
 # 港式五张
 cantrell = on_command("同花顺",aliases = {"五张牌","港式五张","梭哈"}, permission = GROUP, priority = 20, block = True)
 
 @cantrell.handle()
 async def _(event:GroupMessageEvent, arg:Message = CommandArg()):
     gold = arg.extract_plain_text().strip()
     if gold.isdigit():
```

### Comparing `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/config.py` & `nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/data/api.py` & `nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/data/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/data/data.py` & `nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/data/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/Stand.json` & `nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/resource/horserace/Stand.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json` & `nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json` & `nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/基础事件.json` & `nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/resource/horserace/基础事件.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json` & `nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json` & `nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/群友日常.json` & `nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/resource/horserace/群友日常.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json` & `nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json` & `nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json` & `nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/menu_data.json` & `nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/resource/menu_data.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/props_library.json` & `nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/resource/props_library.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/resource/subprocess/ohlc.py` & `nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/resource/subprocess/ohlc.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/utils/avatar.py` & `nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/utils/avatar.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/utils/chart.py` & `nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/utils/chart.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection/utils/utils.py` & `nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection/utils/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.5/nonebot_plugin_game_collection.egg-info/SOURCES.txt` & `nonebot_plugin_game_collection-2.1.6/nonebot_plugin_game_collection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.1.5/setup.py` & `nonebot_plugin_game_collection-2.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_namespace_packages
 
 setup(
 name='nonebot_plugin_game_collection',
-version='2.1.5',
+version='2.1.6',
 description='改自nonebot_plugin_russian合并了nonebot_plugin_horserace还有一些自编玩法的小游戏合集。',
 #long_description=open('README.md','r').read(),
 author='karisaya',
 author_email='1048827424@qq.com',
 license='MIT license',
 include_package_data=True,
 packages=find_namespace_packages(include=["nonebot_plugin_game_collection","nonebot_plugin_game_collection.*"]),
```

