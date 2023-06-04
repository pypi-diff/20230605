# Comparing `tmp/siegeapi-6.0.1.tar.gz` & `tmp/siegeapi-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siegeapi-6.0.1.tar", last modified: Wed May 31 16:43:12 2023, max compression
+gzip compressed data, was "siegeapi-6.1.0.tar", last modified: Sun Jun  4 22:36:03 2023, max compression
```

## Comparing `siegeapi-6.0.1.tar` & `siegeapi-6.1.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 16:43:12.081540 siegeapi-6.0.1/
--rw-rw-rw-   0        0        0     1088 2022-01-22 13:51:16.000000 siegeapi-6.0.1/LICENSE
--rw-rw-rw-   0        0        0     4215 2023-05-31 16:43:12.081037 siegeapi-6.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3331 2023-03-10 17:01:21.000000 siegeapi-6.0.1/README.md
--rw-rw-rw-   0        0        0       97 2021-12-02 11:40:13.000000 siegeapi-6.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-31 16:43:12.081540 siegeapi-6.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1175 2023-05-31 16:42:54.000000 siegeapi-6.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-31 16:43:12.073536 siegeapi-6.0.1/siegeapi/
--rw-rw-rw-   0        0        0       24 2022-04-13 12:58:09.000000 siegeapi-6.0.1/siegeapi/__init__.py
--rw-rw-rw-   0        0        0    12171 2023-04-13 00:49:53.000000 siegeapi-6.0.1/siegeapi/auth.py
-drwxrwxrwx   0        0        0        0 2023-05-31 16:43:12.079537 siegeapi-6.0.1/siegeapi/constants/
--rw-rw-rw-   0        0        0      103 2022-04-13 12:58:09.000000 siegeapi-6.0.1/siegeapi/constants/__init__.py
--rw-rw-rw-   0        0        0    32901 2023-05-31 16:26:20.000000 siegeapi-6.0.1/siegeapi/constants/operators.py
--rw-rw-rw-   0        0        0     9497 2023-01-01 15:53:16.000000 siegeapi-6.0.1/siegeapi/constants/ranks.py
--rw-rw-rw-   0        0        0     4487 2023-05-31 16:28:59.000000 siegeapi-6.0.1/siegeapi/constants/seasons.py
--rw-rw-rw-   0        0        0    23102 2022-08-01 16:12:06.000000 siegeapi-6.0.1/siegeapi/constants/weapons.py
--rw-rw-rw-   0        0        0     2860 2022-06-25 18:50:10.000000 siegeapi-6.0.1/siegeapi/default_stats.py
--rw-rw-rw-   0        0        0      265 2023-01-01 18:09:38.000000 siegeapi-6.0.1/siegeapi/exceptions.py
--rw-rw-rw-   0        0        0     1527 2023-01-01 22:44:20.000000 siegeapi-6.0.1/siegeapi/maps.py
--rw-rw-rw-   0        0        0     2747 2022-12-14 00:11:28.000000 siegeapi-6.0.1/siegeapi/operators.py
--rw-rw-rw-   0        0        0     9782 2023-03-10 16:55:45.000000 siegeapi-6.0.1/siegeapi/player.py
--rw-rw-rw-   0        0        0     1516 2023-01-04 20:19:56.000000 siegeapi-6.0.1/siegeapi/rank_profile.py
--rw-rw-rw-   0        0        0     1880 2023-01-01 15:55:47.000000 siegeapi-6.0.1/siegeapi/ranks.py
--rw-rw-rw-   0        0        0      210 2022-12-13 23:58:32.000000 siegeapi-6.0.1/siegeapi/summaries.py
--rw-rw-rw-   0        0        0     3178 2022-08-31 20:22:36.000000 siegeapi-6.0.1/siegeapi/trends.py
--rw-rw-rw-   0        0        0     4542 2023-03-10 16:55:19.000000 siegeapi-6.0.1/siegeapi/url_builder.py
--rw-rw-rw-   0        0        0     2602 2023-05-31 16:05:18.000000 siegeapi-6.0.1/siegeapi/utils.py
--rw-rw-rw-   0        0        0     3078 2022-08-31 20:18:00.000000 siegeapi-6.0.1/siegeapi/weapons.py
-drwxrwxrwx   0        0        0        0 2023-05-31 16:43:12.076537 siegeapi-6.0.1/siegeapi.egg-info/
--rw-rw-rw-   0        0        0     4215 2023-05-31 16:43:11.000000 siegeapi-6.0.1/siegeapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      642 2023-05-31 16:43:11.000000 siegeapi-6.0.1/siegeapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 16:43:11.000000 siegeapi-6.0.1/siegeapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-05-31 16:43:11.000000 siegeapi-6.0.1/siegeapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-31 16:43:11.000000 siegeapi-6.0.1/siegeapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:36:03.588117 siegeapi-6.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-04 22:35:53.000000 siegeapi-6.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-06-04 22:36:03.588117 siegeapi-6.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-06-04 22:35:53.000000 siegeapi-6.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-04 22:35:53.000000 siegeapi-6.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 22:36:03.588117 siegeapi-6.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-04 22:35:53.000000 siegeapi-6.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:36:03.588117 siegeapi-6.1.0/siegeapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-04 22:35:53.000000 siegeapi-6.1.0/siegeapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-06-04 22:35:53.000000 siegeapi-6.1.0/siegeapi/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:36:03.588117 siegeapi-6.1.0/siegeapi/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-04 22:35:53.000000 siegeapi-6.1.0/siegeapi/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31793 2023-06-04 22:35:53.000000 siegeapi-6.1.0/siegeapi/constants/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9323 2023-06-04 22:35:53.000000 siegeapi-6.1.0/siegeapi/constants/ranks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-06-04 22:35:53.000000 siegeapi-6.1.0/siegeapi/constants/seasons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22522 2023-06-04 22:35:53.000000 siegeapi-6.1.0/siegeapi/constants/weapons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-06-04 22:35:53.000000 siegeapi-6.1.0/siegeapi/default_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-04 22:35:53.000000 siegeapi-6.1.0/siegeapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-04 22:35:53.000000 siegeapi-6.1.0/siegeapi/linked_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-04 22:35:53.000000 siegeapi-6.1.0/siegeapi/maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-06-04 22:35:53.000000 siegeapi-6.1.0/siegeapi/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9941 2023-06-04 22:35:53.000000 siegeapi-6.1.0/siegeapi/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-04 22:35:53.000000 siegeapi-6.1.0/siegeapi/rank_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-04 22:35:53.000000 siegeapi-6.1.0/siegeapi/ranks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-04 22:35:53.000000 siegeapi-6.1.0/siegeapi/summaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-06-04 22:35:53.000000 siegeapi-6.1.0/siegeapi/trends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-06-04 22:35:53.000000 siegeapi-6.1.0/siegeapi/url_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-06-04 22:35:53.000000 siegeapi-6.1.0/siegeapi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-06-04 22:35:53.000000 siegeapi-6.1.0/siegeapi/weapons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:36:03.588117 siegeapi-6.1.0/siegeapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-06-04 22:36:03.000000 siegeapi-6.1.0/siegeapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-04 22:36:03.000000 siegeapi-6.1.0/siegeapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 22:36:03.000000 siegeapi-6.1.0/siegeapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-04 22:36:03.000000 siegeapi-6.1.0/siegeapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-04 22:36:03.000000 siegeapi-6.1.0/siegeapi.egg-info/top_level.txt
```

### Comparing `siegeapi-6.0.1/LICENSE` & `siegeapi-6.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021-2022 CNDRD
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2021-2022 CNDRD
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `siegeapi-6.0.1/PKG-INFO` & `siegeapi-6.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,117 +1,117 @@
-Metadata-Version: 2.1
-Name: siegeapi
-Version: 6.0.1
-Summary: Rainbow Six Siege API interface
-Home-page: https://github.com/CNDRD/siege-api
-Author: CNDRD
-License: MIT
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Internet
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Classifier: Typing :: Typed
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<div align="center">
-    <img width="250" src="https://raw.githubusercontent.com/CNDRD/siegeapi/master/assets/siegeapi-banner.png" />
-    <h1>siegeapi</h1>
-    <a href="https://github.com/CNDRD/siegeapi/releases">
-        <img src="https://img.shields.io/github/v/release/CNDRD/siegeapi?label=latest%20release&style=for-the-badge&logo=github&logoColor=white" />
-    </a>
-    <a href="https://pypi.org/project/siegeapi/#history">
-        <img src="https://img.shields.io/pypi/v/siegeapi?style=for-the-badge&logo=pypi&logoColor=white" />
-    </a>
-    <br />
-    <a href="https://www.python.org/downloads/">
-        <img src="https://img.shields.io/pypi/pyversions/siegeapi?style=for-the-badge&logo=python&logoColor=white&color=yellow" />
-    </a>
-    <a href="https://pypi.org/project/siegeapi">
-        <img src="https://img.shields.io/pypi/dm/siegeapi?style=for-the-badge&logo=pypi&logoColor=white&color=yellow" />
-    </a>
-</div>
-
-## How to install  
-```commandline
-pip install siegeapi
-```
-
-## Quick example  
-```python
-from siegeapi import Auth
-import asyncio
-
-async def sample():
-    auth = Auth("UBI_EMAIL", "UBI_PASSWORD")
-    player = await auth.get_player(uid="7e0f63df-a39b-44c5-8de0-d39a05926e77")
-
-    print(f"Name: {player.name}")
-    print(f"Profile pic URL: {player.profile_pic_url}")
-    
-    await player.load_playtime()
-    print(f"Total Time Played: {player.total_time_played:,} seconds")
-    print(f"Level: {player.level}")
-
-    await player.load_ranked_v2()
-    print(f"Ranked Points: {player.ranked_profile.rank_points}")
-    print(f"Rank: {player.ranked_profile.rank}")
-    print(f"Max Rank Points: {player.ranked_profile.max_rank_points}")
-    print(f"Max Rank: {player.ranked_profile.max_rank}")
-
-    await player.load_progress()
-    print(f"XP: {player.xp:,}")
-    print(f"Total XP: {player.total_xp:,}")
-    print(f"XP to level up: {player.xp_to_level_up:,}")
-    
-    await auth.close()
-
-asyncio.get_event_loop().run_until_complete(sample())
-# Or `asyncio.run(sample())`  
-```
-### Output  
-```text
-Name: CNDRD
-Profile pic URL: https://ubisoft-avatars.akamaized.net/7e0f63df-a39b-44c5-8de0-d39a05926e77/default_256_256.png
-Total Time Played: 7,910,265 seconds
-Level: 285
-Ranked Points: 1000
-Rank: Unranked
-Max Rank Points: 1000
-Max Rank: Unranked
-XP: 56,362
-Total XP: 17,973,862
-XP to level up: 77,138
-```
-
----  
-
-## Siege Inventory  
-If you want to see every skin, headgear, uniform and more, head over to **[skins.cndrd.xyz](https://skins.cndrd.xyz/)**  
-
-## Docs  
-For docs go to [cndrd.github.io/siegeapi](https://cndrd.github.io/siegeapi/)  
-
-## Credits  
-Operator Icons from [r6operators][r6operators_] by [marcopixel][marcopixel_]  
-Built (and re-built) on top of what [billy-yoyo][r6s_python_api] started  
-
-## Problems  
-If you experience any problems, reach out to me, or submit a PR  
-You can reach out here on GitHub or on Discord (_CNDRD#2233_)  
-
-
-![forthebadge](https://forthebadge.com/images/badges/works-on-my-machine.svg)  
-![forthebadge](https://forthebadge.com/images/badges/powered-by-energy-drinks.svg)  
-
-[r6operators_]: https://github.com/marcopixel/r6operators  
-[marcopixel_]: https://github.com/marcopixel  
-[r6s_python_api]: https://github.com/billy-yoyo/RainbowSixSiege-Python-API  
+Metadata-Version: 2.1
+Name: siegeapi
+Version: 6.1.0
+Summary: Rainbow Six Siege API interface
+Home-page: https://github.com/CNDRD/siege-api
+Author: CNDRD
+License: MIT
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Internet
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
+Requires-Python: >=3.8.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<div align="center">
+    <img width="250" src="https://raw.githubusercontent.com/CNDRD/siegeapi/master/assets/siegeapi-banner.png" />
+    <h1>siegeapi</h1>
+    <a href="https://github.com/CNDRD/siegeapi/releases">
+        <img src="https://img.shields.io/github/v/release/CNDRD/siegeapi?label=latest%20release&style=for-the-badge&logo=github&logoColor=white" />
+    </a>
+    <a href="https://pypi.org/project/siegeapi/#history">
+        <img src="https://img.shields.io/pypi/v/siegeapi?style=for-the-badge&logo=pypi&logoColor=white" />
+    </a>
+    <br />
+    <a href="https://www.python.org/downloads/">
+        <img src="https://img.shields.io/pypi/pyversions/siegeapi?style=for-the-badge&logo=python&logoColor=white&color=yellow" />
+    </a>
+    <a href="https://pypi.org/project/siegeapi">
+        <img src="https://img.shields.io/pypi/dm/siegeapi?style=for-the-badge&logo=pypi&logoColor=white&color=yellow" />
+    </a>
+</div>
+
+## How to install  
+```commandline
+pip install siegeapi
+```
+
+## Quick example  
+```python
+from siegeapi import Auth
+import asyncio
+
+async def sample():
+    auth = Auth("UBI_EMAIL", "UBI_PASSWORD")
+    player = await auth.get_player(uid="7e0f63df-a39b-44c5-8de0-d39a05926e77")
+
+    print(f"Name: {player.name}")
+    print(f"Profile pic URL: {player.profile_pic_url}")
+    
+    await player.load_playtime()
+    print(f"Total Time Played: {player.total_time_played:,} seconds")
+    print(f"Level: {player.level}")
+
+    await player.load_ranked_v2()
+    print(f"Ranked Points: {player.ranked_profile.rank_points}")
+    print(f"Rank: {player.ranked_profile.rank}")
+    print(f"Max Rank Points: {player.ranked_profile.max_rank_points}")
+    print(f"Max Rank: {player.ranked_profile.max_rank}")
+
+    await player.load_progress()
+    print(f"XP: {player.xp:,}")
+    print(f"Total XP: {player.total_xp:,}")
+    print(f"XP to level up: {player.xp_to_level_up:,}")
+    
+    await auth.close()
+
+asyncio.get_event_loop().run_until_complete(sample())
+# Or `asyncio.run(sample())`  
+```
+### Output  
+```text
+Name: CNDRD
+Profile pic URL: https://ubisoft-avatars.akamaized.net/7e0f63df-a39b-44c5-8de0-d39a05926e77/default_256_256.png
+Total Time Played: 7,910,265 seconds
+Level: 285
+Ranked Points: 1000
+Rank: Unranked
+Max Rank Points: 1000
+Max Rank: Unranked
+XP: 56,362
+Total XP: 17,973,862
+XP to level up: 77,138
+```
+
+---  
+
+## Siege Inventory  
+If you want to see every skin, headgear, uniform and more, head over to **[skins.cndrd.xyz](https://skins.cndrd.xyz/)**  
+
+## Docs  
+For docs go to [cndrd.github.io/siegeapi](https://cndrd.github.io/siegeapi/)  
+
+## Credits  
+Operator Icons from [r6operators][r6operators_] by [marcopixel][marcopixel_]  
+Built (and re-built) on top of what [billy-yoyo][r6s_python_api] started  
+
+## Problems  
+If you experience any problems, reach out to me, or submit a PR  
+You can reach out here on GitHub or on Discord (_CNDRD#2233_)  
+
+
+![forthebadge](https://forthebadge.com/images/badges/works-on-my-machine.svg)  
+![forthebadge](https://forthebadge.com/images/badges/powered-by-energy-drinks.svg)  
+
+[r6operators_]: https://github.com/marcopixel/r6operators  
+[marcopixel_]: https://github.com/marcopixel  
+[r6s_python_api]: https://github.com/billy-yoyo/RainbowSixSiege-Python-API
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: siegeapi Version: 6.0.1 Summary: Rainbow Six Siege
+Metadata-Version: 2.1 Name: siegeapi Version: 6.1.0 Summary: Rainbow Six Siege
 API interface Home-page: https://github.com/CNDRD/siege-api Author: CNDRD
 License: MIT Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License Classifier: Intended
 Audience :: Developers Classifier: Natural Language :: English Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Topic :: Internet Classifier:
```

### Comparing `siegeapi-6.0.1/README.md` & `siegeapi-6.1.0/README.md`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-<div align="center">
-    <img width="250" src="https://raw.githubusercontent.com/CNDRD/siegeapi/master/assets/siegeapi-banner.png" />
-    <h1>siegeapi</h1>
-    <a href="https://github.com/CNDRD/siegeapi/releases">
-        <img src="https://img.shields.io/github/v/release/CNDRD/siegeapi?label=latest%20release&style=for-the-badge&logo=github&logoColor=white" />
-    </a>
-    <a href="https://pypi.org/project/siegeapi/#history">
-        <img src="https://img.shields.io/pypi/v/siegeapi?style=for-the-badge&logo=pypi&logoColor=white" />
-    </a>
-    <br />
-    <a href="https://www.python.org/downloads/">
-        <img src="https://img.shields.io/pypi/pyversions/siegeapi?style=for-the-badge&logo=python&logoColor=white&color=yellow" />
-    </a>
-    <a href="https://pypi.org/project/siegeapi">
-        <img src="https://img.shields.io/pypi/dm/siegeapi?style=for-the-badge&logo=pypi&logoColor=white&color=yellow" />
-    </a>
-</div>
-
-## How to install  
-```commandline
-pip install siegeapi
-```
-
-## Quick example  
-```python
-from siegeapi import Auth
-import asyncio
-
-async def sample():
-    auth = Auth("UBI_EMAIL", "UBI_PASSWORD")
-    player = await auth.get_player(uid="7e0f63df-a39b-44c5-8de0-d39a05926e77")
-
-    print(f"Name: {player.name}")
-    print(f"Profile pic URL: {player.profile_pic_url}")
-    
-    await player.load_playtime()
-    print(f"Total Time Played: {player.total_time_played:,} seconds")
-    print(f"Level: {player.level}")
-
-    await player.load_ranked_v2()
-    print(f"Ranked Points: {player.ranked_profile.rank_points}")
-    print(f"Rank: {player.ranked_profile.rank}")
-    print(f"Max Rank Points: {player.ranked_profile.max_rank_points}")
-    print(f"Max Rank: {player.ranked_profile.max_rank}")
-
-    await player.load_progress()
-    print(f"XP: {player.xp:,}")
-    print(f"Total XP: {player.total_xp:,}")
-    print(f"XP to level up: {player.xp_to_level_up:,}")
-    
-    await auth.close()
-
-asyncio.get_event_loop().run_until_complete(sample())
-# Or `asyncio.run(sample())`  
-```
-### Output  
-```text
-Name: CNDRD
-Profile pic URL: https://ubisoft-avatars.akamaized.net/7e0f63df-a39b-44c5-8de0-d39a05926e77/default_256_256.png
-Total Time Played: 7,910,265 seconds
-Level: 285
-Ranked Points: 1000
-Rank: Unranked
-Max Rank Points: 1000
-Max Rank: Unranked
-XP: 56,362
-Total XP: 17,973,862
-XP to level up: 77,138
-```
-
----  
-
-## Siege Inventory  
-If you want to see every skin, headgear, uniform and more, head over to **[skins.cndrd.xyz](https://skins.cndrd.xyz/)**  
-
-## Docs  
-For docs go to [cndrd.github.io/siegeapi](https://cndrd.github.io/siegeapi/)  
-
-## Credits  
-Operator Icons from [r6operators][r6operators_] by [marcopixel][marcopixel_]  
-Built (and re-built) on top of what [billy-yoyo][r6s_python_api] started  
-
-## Problems  
-If you experience any problems, reach out to me, or submit a PR  
-You can reach out here on GitHub or on Discord (_CNDRD#2233_)  
-
-
-![forthebadge](https://forthebadge.com/images/badges/works-on-my-machine.svg)  
-![forthebadge](https://forthebadge.com/images/badges/powered-by-energy-drinks.svg)  
-
-[r6operators_]: https://github.com/marcopixel/r6operators  
-[marcopixel_]: https://github.com/marcopixel  
-[r6s_python_api]: https://github.com/billy-yoyo/RainbowSixSiege-Python-API  
+<div align="center">
+    <img width="250" src="https://raw.githubusercontent.com/CNDRD/siegeapi/master/assets/siegeapi-banner.png" />
+    <h1>siegeapi</h1>
+    <a href="https://github.com/CNDRD/siegeapi/releases">
+        <img src="https://img.shields.io/github/v/release/CNDRD/siegeapi?label=latest%20release&style=for-the-badge&logo=github&logoColor=white" />
+    </a>
+    <a href="https://pypi.org/project/siegeapi/#history">
+        <img src="https://img.shields.io/pypi/v/siegeapi?style=for-the-badge&logo=pypi&logoColor=white" />
+    </a>
+    <br />
+    <a href="https://www.python.org/downloads/">
+        <img src="https://img.shields.io/pypi/pyversions/siegeapi?style=for-the-badge&logo=python&logoColor=white&color=yellow" />
+    </a>
+    <a href="https://pypi.org/project/siegeapi">
+        <img src="https://img.shields.io/pypi/dm/siegeapi?style=for-the-badge&logo=pypi&logoColor=white&color=yellow" />
+    </a>
+</div>
+
+## How to install  
+```commandline
+pip install siegeapi
+```
+
+## Quick example  
+```python
+from siegeapi import Auth
+import asyncio
+
+async def sample():
+    auth = Auth("UBI_EMAIL", "UBI_PASSWORD")
+    player = await auth.get_player(uid="7e0f63df-a39b-44c5-8de0-d39a05926e77")
+
+    print(f"Name: {player.name}")
+    print(f"Profile pic URL: {player.profile_pic_url}")
+    
+    await player.load_playtime()
+    print(f"Total Time Played: {player.total_time_played:,} seconds")
+    print(f"Level: {player.level}")
+
+    await player.load_ranked_v2()
+    print(f"Ranked Points: {player.ranked_profile.rank_points}")
+    print(f"Rank: {player.ranked_profile.rank}")
+    print(f"Max Rank Points: {player.ranked_profile.max_rank_points}")
+    print(f"Max Rank: {player.ranked_profile.max_rank}")
+
+    await player.load_progress()
+    print(f"XP: {player.xp:,}")
+    print(f"Total XP: {player.total_xp:,}")
+    print(f"XP to level up: {player.xp_to_level_up:,}")
+    
+    await auth.close()
+
+asyncio.get_event_loop().run_until_complete(sample())
+# Or `asyncio.run(sample())`  
+```
+### Output  
+```text
+Name: CNDRD
+Profile pic URL: https://ubisoft-avatars.akamaized.net/7e0f63df-a39b-44c5-8de0-d39a05926e77/default_256_256.png
+Total Time Played: 7,910,265 seconds
+Level: 285
+Ranked Points: 1000
+Rank: Unranked
+Max Rank Points: 1000
+Max Rank: Unranked
+XP: 56,362
+Total XP: 17,973,862
+XP to level up: 77,138
+```
+
+---  
+
+## Siege Inventory  
+If you want to see every skin, headgear, uniform and more, head over to **[skins.cndrd.xyz](https://skins.cndrd.xyz/)**  
+
+## Docs  
+For docs go to [cndrd.github.io/siegeapi](https://cndrd.github.io/siegeapi/)  
+
+## Credits  
+Operator Icons from [r6operators][r6operators_] by [marcopixel][marcopixel_]  
+Built (and re-built) on top of what [billy-yoyo][r6s_python_api] started  
+
+## Problems  
+If you experience any problems, reach out to me, or submit a PR  
+You can reach out here on GitHub or on Discord (_CNDRD#2233_)  
+
+
+![forthebadge](https://forthebadge.com/images/badges/works-on-my-machine.svg)  
+![forthebadge](https://forthebadge.com/images/badges/powered-by-energy-drinks.svg)  
+
+[r6operators_]: https://github.com/marcopixel/r6operators  
+[marcopixel_]: https://github.com/marcopixel  
+[r6s_python_api]: https://github.com/billy-yoyo/RainbowSixSiege-Python-API
```

### Comparing `siegeapi-6.0.1/siegeapi/auth.py` & `siegeapi-6.1.0/siegeapi/auth.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,300 +1,300 @@
-from __future__ import annotations
-
-from datetime import datetime, timezone
-
-from urllib import parse
-import aiohttp
-import base64
-import time
-import json
-import os
-
-from .exceptions import FailedToConnect, InvalidRequest
-from .player import Player
-
-
-class Auth:
-    """ Holds the authentication information """
-
-    @staticmethod
-    def get_basic_token(email: str, password: str) -> str:
-        return base64.b64encode(f"{email}:{password}".encode("utf-8")).decode("utf-8")
-
-    def __init__(
-            self,
-            email: str = None,
-            password: str = None,
-            token: str = None,
-            appid: str = None,
-            creds_path: str = None,
-            cachetime: int = 120,
-            max_connect_retries: int = 1,
-            session: aiohttp.ClientSession() = None,
-            refresh_session_period: int = 180
-    ):
-        self.session: aiohttp.ClientSession() = session or aiohttp.ClientSession()
-        self.max_connect_retries: int = max_connect_retries
-        self.refresh_session_period: int = refresh_session_period
-
-        self.token: str = token or Auth.get_basic_token(email, password)
-        self.creds_path: str = creds_path or f"{os.getcwd()}/creds/{self.token}.json"
-        self.appid: str = appid or 'e3d5ea9e-50bd-43b7-88bf-39794f4e3d40'
-        self.sessionid: str = ""
-        self.key: str = ""
-        self.new_key: str = ""
-        self.spaceid: str = ""
-        self.spaceids: dict[str: str] = {
-            "uplay": "5172a557-50b5-4665-b7db-e3f2e8c5041d",
-            "psn": "05bfb3f7-6c21-4c42-be1f-97a33fb5cf66",
-            "xbl": "98a601e5-ca91-4440-b1c5-753f601a2c90"
-        }
-        self.profileid: str = ""
-        self.userid: str = ""
-        self.expiration: str = ""
-        self.new_expiration: str = ""
-
-        self.cachetime: int = cachetime
-        self.cache = {}
-
-        self._login_cooldown: int = 0
-        self._session_start: float = time.time()
-
-    async def _find_players(self, name: str, platform: str, uid: str) -> list[Player]:
-        """ Get a list of players matching the search term on a given platform """
-
-        if name is None and uid is None:
-            raise TypeError("'name' and 'uid' are both None, exactly one must be given")
-
-        if name is not None and uid is not None:
-            raise TypeError("Cannot search by 'uid' and 'name' at the same time, please give one or the other")
-
-        if platform is None:
-            raise TypeError("platform cannot be None")
-
-        if platform not in ("uplay", "xbl", "psn"):
-            raise TypeError(f"'platform' has to be one of the following: 'uplay' / 'xbl' / 'psn'; Not {platform}")
-
-        if name:
-            data = await self.get(f"https://public-ubiservices.ubi.com/v3/profiles?"
-                                  f"nameOnPlatform={parse.quote(name)}&platformType={parse.quote(platform)}")
-        else:
-            data = await self.get(f"https://public-ubiservices.ubi.com/v3/users/{uid}/profiles?"
-                                  f"platformType={parse.quote(platform)}")
-
-        if "profiles" in data:
-            results = [Player(self, x) for x in data["profiles"] if x.get("platformType", "") == platform]
-            if len(results) == 0:
-                raise InvalidRequest("No results")
-            return results
-        else:
-            raise InvalidRequest(f"Missing key profiles in returned JSON object {str(data)}")
-
-    async def _ensure_session_valid(self) -> None:
-        if not self.session:
-            await self.refresh_session()
-        elif 0 <= self.refresh_session_period <= (time.time() - self._session_start):
-            await self.refresh_session()
-
-    async def refresh_session(self) -> None:
-        """ Closes the current session and opens a new one """
-        if self.session:
-            try:
-                await self.session.close()
-            except:
-                pass
-
-        self.session = aiohttp.ClientSession()
-        self._session_start = time.time()
-
-    async def get_session(self) -> aiohttp.ClientSession():
-        """ Retrieves the current session, ensuring it's valid first """
-        await self._ensure_session_valid()
-        return self.session
-
-    def save_creds(self) -> None:
-        """ Saves the credentials to a file """
-
-        if not os.path.exists(os.path.dirname(self.creds_path)):
-            os.makedirs(os.path.dirname(self.creds_path))
-
-        if not os.path.exists(self.creds_path):
-            with open(self.creds_path, 'w') as f:
-                json.dump({}, f)
-
-        # write to file, overwriting the old one
-        with open(self.creds_path, 'w') as f:
-            json.dump({
-                "sessionid": self.sessionid,
-                "key": self.key,
-                "new_key": self.new_key,
-                "spaceid": self.spaceid,
-                "profileid": self.profileid,
-                "userid": self.userid,
-                "expiration": self.expiration,
-                "new_expiration": self.new_expiration,
-            }, f, indent=4)
-
-    def load_creds(self) -> None:
-        """ Loads the credentials from a file """
-
-        if not os.path.exists(self.creds_path):
-            return
-
-        with open(self.creds_path, "r") as f:
-            data = json.load(f)
-
-        self.sessionid = data.get("sessionid", "")
-        self.key = data.get("key", "")
-        self.new_key = data.get("new_key", "")
-        self.spaceid = data.get("spaceid", "")
-        self.profileid = data.get("profileid", "")
-        self.userid = data.get("userid", "")
-        self.expiration = data.get("expiration", "")
-        self.new_expiration = data.get("new_expiration", "")
-
-    async def connect(self, _new: bool = False) -> None:
-        """ Connect to Ubisoft, automatically called when needed """
-        if self._login_cooldown > time.time():
-            raise FailedToConnect("Login on cooldown")
-
-        self.load_creds()
-
-        # If keys are still valid, don't connect again
-        if _new:
-            if self.new_key and datetime.fromisoformat(self.new_expiration[:26]+"+00:00") > datetime.now(timezone.utc):
-                return
-        else:
-            if self.key and datetime.fromisoformat(self.expiration[:26]+"+00:00") > datetime.now(timezone.utc):
-                await self.connect(_new=True)
-                return
-
-        session = await self.get_session()
-        headers = {
-            "Content-Type": "application/json; charset=UTF-8",
-            "Ubi-AppId": "39baebad-39e5-4552-8c25-2c9b919064e2",
-            "Authorization": "Basic " + self.token
-        }
-
-        if _new:
-            headers["Ubi-AppId"] = self.appid
-            headers["Authorization"] = "Ubi_v1 t=" + self.key
-            headers["User-Agent"] = "UbiServices_SDK_2020.Release.58_PC64_ansi_static"
-
-        resp = await session.post(
-            url="https://public-ubiservices.ubi.com/v3/profiles/sessions",
-            headers=headers,
-            data=json.dumps({"rememberMe": True})
-        )
-
-        data = await resp.json()
-
-        if "ticket" in data:
-            if _new:
-                self.new_key = data.get('ticket')
-                self.new_expiration = data.get('expiration')
-            else:
-                self.key = data.get("ticket")
-                self.expiration = data.get("expiration")
-            self.profileid = data.get('profileId')
-            self.sessionid = data.get("sessionId")
-            self.spaceid = data.get("spaceId")
-            self.userid = data.get("userId")
-        else:
-            message = "Unknown Error"
-            if "message" in data and "httpCode" in data:
-                message = f"HTTP {data['httpCode']}: {data['message']}"
-            elif "message" in data:
-                message = data["message"]
-            elif "httpCode" in data:
-                message = str(data["httpCode"])
-            raise FailedToConnect(message)
-
-        self.save_creds()
-        await self.connect(_new=True)
-
-    async def close(self) -> None:
-        """ Closes the session associated with the auth object """
-        self.save_creds()
-        await self.session.close()
-
-    async def get(self, *args, retries: int = 0, json_: bool = True, new: bool = False, **kwargs) -> dict | str:
-        if (not self.key and not new) or (not self.new_key and new):
-            last_error = None
-            for _ in range(self.max_connect_retries):
-                try:
-                    await self.connect()
-                    break
-                except FailedToConnect as e:
-                    last_error = e
-            else:
-                # assume this error is going uncaught, so we close the session
-                await self.close()
-
-                if last_error:
-                    raise last_error
-                else:
-                    raise FailedToConnect("Unknown Error")
-
-        if "headers" not in kwargs:
-            kwargs["headers"] = {}
-
-        authorization = kwargs["headers"].get("Authorization") or "Ubi_v1 t=" + (self.new_key if new else self.key)
-        appid = kwargs["headers"].get("Ubi-AppId") or self.appid
-
-        kwargs["headers"]["Authorization"] = authorization
-        kwargs["headers"]["Ubi-AppId"] = appid
-        kwargs["headers"]["Ubi-LocaleCode"] = kwargs["headers"].get("Ubi-LocaleCode") or "en-US"
-        kwargs["headers"]["Ubi-SessionId"] = kwargs["headers"].get("Ubi-SessionId") or self.sessionid
-        kwargs["headers"]["User-Agent"] = kwargs["headers"].get("User-Agent") or "UbiServices_SDK_2020.Release.58_PC64_ansi_static"
-        kwargs["headers"]["Connection"] = kwargs["headers"].get("Connection") or "keep-alive"
-        kwargs["headers"]["expiration"] = kwargs["headers"].get("expiration") or self.expiration
-
-        session = await self.get_session()
-        resp = await session.get(*args, **kwargs)
-
-        if json_:
-            try:
-                data = await resp.json()
-            except Exception:
-                text = await resp.text()
-                message = text.split("h1>")
-                message = message[1][:-2] if len(message) > 1 else text
-                raise InvalidRequest(f"Received a text response, expected JSON response. Message: {message}")
-
-            if "httpCode" in data:
-                if data["httpCode"] == 401:
-                    if retries >= self.max_connect_retries:
-                        # wait 30 seconds before sending another request
-                        self._login_cooldown = time.time() + 30
-
-                    # key no longer works, so remove key and let the following .get() call refresh it
-                    self.key = None
-                    return await self.get(*args, retries=retries + 1, **kwargs)
-                else:
-                    msg = data.get("message", "")
-                    if data["httpCode"] == 404:
-                        msg = f"Missing resource {data.get('resource', args[0])}"
-                    raise InvalidRequest(f"HTTP {data['httpCode']}: {msg}", code=data["httpCode"])
-
-            return data
-        else:
-            return await resp.text()
-
-    async def get_player(self, name: str = None, uid: str = None, platform: str = "uplay") -> Player:
-        """ Calls get_players and returns the first element """
-
-        results = await self._find_players(name=name, platform=platform, uid=uid)
-        return results[0]
-
-    async def get_player_batch(self, names: list[str] = None, uids: list[str] = None, platform: str = "uplay") -> dict[str: Player]:
-        players = {}
-        if names is not None:
-            for name in names:
-                player = await self.get_player(name=name, platform=platform)
-                players[player.id] = player
-
-        if uids is not None:
-            for uid in uids:
-                player = await self.get_player(uid=uid, platform=platform)
-                players[player.id] = player
-        return players
+from __future__ import annotations
+
+from datetime import datetime, timezone
+
+from urllib import parse
+import aiohttp
+import base64
+import time
+import json
+import os
+
+from .exceptions import FailedToConnect, InvalidRequest
+from .player import Player
+
+
+class Auth:
+    """ Holds the authentication information """
+
+    @staticmethod
+    def get_basic_token(email: str, password: str) -> str:
+        return base64.b64encode(f"{email}:{password}".encode("utf-8")).decode("utf-8")
+
+    def __init__(
+            self,
+            email: str = None,
+            password: str = None,
+            token: str = None,
+            appid: str = None,
+            creds_path: str = None,
+            cachetime: int = 120,
+            max_connect_retries: int = 1,
+            session: aiohttp.ClientSession() = None,
+            refresh_session_period: int = 180
+    ):
+        self.session: aiohttp.ClientSession() = session or aiohttp.ClientSession()
+        self.max_connect_retries: int = max_connect_retries
+        self.refresh_session_period: int = refresh_session_period
+
+        self.token: str = token or Auth.get_basic_token(email, password)
+        self.creds_path: str = creds_path or f"{os.getcwd()}/creds/{self.token}.json"
+        self.appid: str = appid or 'e3d5ea9e-50bd-43b7-88bf-39794f4e3d40'
+        self.sessionid: str = ""
+        self.key: str = ""
+        self.new_key: str = ""
+        self.spaceid: str = ""
+        self.spaceids: dict[str: str] = {
+            "uplay": "5172a557-50b5-4665-b7db-e3f2e8c5041d",
+            "psn": "05bfb3f7-6c21-4c42-be1f-97a33fb5cf66",
+            "xbl": "98a601e5-ca91-4440-b1c5-753f601a2c90"
+        }
+        self.profileid: str = ""
+        self.userid: str = ""
+        self.expiration: str = ""
+        self.new_expiration: str = ""
+
+        self.cachetime: int = cachetime
+        self.cache = {}
+
+        self._login_cooldown: int = 0
+        self._session_start: float = time.time()
+
+    async def _find_players(self, name: str, platform: str, uid: str) -> list[Player]:
+        """ Get a list of players matching the search term on a given platform """
+
+        if name is None and uid is None:
+            raise TypeError("'name' and 'uid' are both None, exactly one must be given")
+
+        if name is not None and uid is not None:
+            raise TypeError("Cannot search by 'uid' and 'name' at the same time, please give one or the other")
+
+        if platform is None:
+            raise TypeError("platform cannot be None")
+
+        if platform not in ("uplay", "xbl", "psn"):
+            raise TypeError(f"'platform' has to be one of the following: 'uplay' / 'xbl' / 'psn'; Not {platform}")
+
+        if name:
+            data = await self.get(f"https://public-ubiservices.ubi.com/v3/profiles?"
+                                  f"nameOnPlatform={parse.quote(name)}&platformType={parse.quote(platform)}")
+        else:
+            data = await self.get(f"https://public-ubiservices.ubi.com/v3/users/{uid}/profiles?"
+                                  f"platformType={parse.quote(platform)}")
+
+        if "profiles" in data:
+            results = [Player(self, x) for x in data["profiles"] if x.get("platformType", "") == platform]
+            if len(results) == 0:
+                raise InvalidRequest("No results")
+            return results
+        else:
+            raise InvalidRequest(f"Missing key profiles in returned JSON object {str(data)}")
+
+    async def _ensure_session_valid(self) -> None:
+        if not self.session:
+            await self.refresh_session()
+        elif 0 <= self.refresh_session_period <= (time.time() - self._session_start):
+            await self.refresh_session()
+
+    async def refresh_session(self) -> None:
+        """ Closes the current session and opens a new one """
+        if self.session:
+            try:
+                await self.session.close()
+            except:
+                pass
+
+        self.session = aiohttp.ClientSession()
+        self._session_start = time.time()
+
+    async def get_session(self) -> aiohttp.ClientSession():
+        """ Retrieves the current session, ensuring it's valid first """
+        await self._ensure_session_valid()
+        return self.session
+
+    def save_creds(self) -> None:
+        """ Saves the credentials to a file """
+
+        if not os.path.exists(os.path.dirname(self.creds_path)):
+            os.makedirs(os.path.dirname(self.creds_path))
+
+        if not os.path.exists(self.creds_path):
+            with open(self.creds_path, 'w') as f:
+                json.dump({}, f)
+
+        # write to file, overwriting the old one
+        with open(self.creds_path, 'w') as f:
+            json.dump({
+                "sessionid": self.sessionid,
+                "key": self.key,
+                "new_key": self.new_key,
+                "spaceid": self.spaceid,
+                "profileid": self.profileid,
+                "userid": self.userid,
+                "expiration": self.expiration,
+                "new_expiration": self.new_expiration,
+            }, f, indent=4)
+
+    def load_creds(self) -> None:
+        """ Loads the credentials from a file """
+
+        if not os.path.exists(self.creds_path):
+            return
+
+        with open(self.creds_path, "r") as f:
+            data = json.load(f)
+
+        self.sessionid = data.get("sessionid", "")
+        self.key = data.get("key", "")
+        self.new_key = data.get("new_key", "")
+        self.spaceid = data.get("spaceid", "")
+        self.profileid = data.get("profileid", "")
+        self.userid = data.get("userid", "")
+        self.expiration = data.get("expiration", "")
+        self.new_expiration = data.get("new_expiration", "")
+
+    async def connect(self, _new: bool = False) -> None:
+        """ Connect to Ubisoft, automatically called when needed """
+        if self._login_cooldown > time.time():
+            raise FailedToConnect("Login on cooldown")
+
+        self.load_creds()
+
+        # If keys are still valid, don't connect again
+        if _new:
+            if self.new_key and datetime.fromisoformat(self.new_expiration[:26]+"+00:00") > datetime.now(timezone.utc):
+                return
+        else:
+            if self.key and datetime.fromisoformat(self.expiration[:26]+"+00:00") > datetime.now(timezone.utc):
+                await self.connect(_new=True)
+                return
+
+        session = await self.get_session()
+        headers = {
+            "Content-Type": "application/json; charset=UTF-8",
+            "Ubi-AppId": "39baebad-39e5-4552-8c25-2c9b919064e2",
+            "Authorization": "Basic " + self.token
+        }
+
+        if _new:
+            headers["Ubi-AppId"] = self.appid
+            headers["Authorization"] = "Ubi_v1 t=" + self.key
+            headers["User-Agent"] = "UbiServices_SDK_2020.Release.58_PC64_ansi_static"
+
+        resp = await session.post(
+            url="https://public-ubiservices.ubi.com/v3/profiles/sessions",
+            headers=headers,
+            data=json.dumps({"rememberMe": True})
+        )
+
+        data = await resp.json()
+
+        if "ticket" in data:
+            if _new:
+                self.new_key = data.get('ticket')
+                self.new_expiration = data.get('expiration')
+            else:
+                self.key = data.get("ticket")
+                self.expiration = data.get("expiration")
+            self.profileid = data.get('profileId')
+            self.sessionid = data.get("sessionId")
+            self.spaceid = data.get("spaceId")
+            self.userid = data.get("userId")
+        else:
+            message = "Unknown Error"
+            if "message" in data and "httpCode" in data:
+                message = f"HTTP {data['httpCode']}: {data['message']}"
+            elif "message" in data:
+                message = data["message"]
+            elif "httpCode" in data:
+                message = str(data["httpCode"])
+            raise FailedToConnect(message)
+
+        self.save_creds()
+        await self.connect(_new=True)
+
+    async def close(self) -> None:
+        """ Closes the session associated with the auth object """
+        self.save_creds()
+        await self.session.close()
+
+    async def get(self, *args, retries: int = 0, json_: bool = True, new: bool = False, **kwargs) -> dict | str:
+        if (not self.key and not new) or (not self.new_key and new):
+            last_error = None
+            for _ in range(self.max_connect_retries):
+                try:
+                    await self.connect()
+                    break
+                except FailedToConnect as e:
+                    last_error = e
+            else:
+                # assume this error is going uncaught, so we close the session
+                await self.close()
+
+                if last_error:
+                    raise last_error
+                else:
+                    raise FailedToConnect("Unknown Error")
+
+        if "headers" not in kwargs:
+            kwargs["headers"] = {}
+
+        authorization = kwargs["headers"].get("Authorization") or "Ubi_v1 t=" + (self.new_key if new else self.key)
+        appid = kwargs["headers"].get("Ubi-AppId") or self.appid
+
+        kwargs["headers"]["Authorization"] = authorization
+        kwargs["headers"]["Ubi-AppId"] = appid
+        kwargs["headers"]["Ubi-LocaleCode"] = kwargs["headers"].get("Ubi-LocaleCode") or "en-US"
+        kwargs["headers"]["Ubi-SessionId"] = kwargs["headers"].get("Ubi-SessionId") or self.sessionid
+        kwargs["headers"]["User-Agent"] = kwargs["headers"].get("User-Agent") or "UbiServices_SDK_2020.Release.58_PC64_ansi_static"
+        kwargs["headers"]["Connection"] = kwargs["headers"].get("Connection") or "keep-alive"
+        kwargs["headers"]["expiration"] = kwargs["headers"].get("expiration") or self.expiration
+
+        session = await self.get_session()
+        resp = await session.get(*args, **kwargs)
+
+        if json_:
+            try:
+                data = await resp.json()
+            except Exception:
+                text = await resp.text()
+                message = text.split("h1>")
+                message = message[1][:-2] if len(message) > 1 else text
+                raise InvalidRequest(f"Received a text response, expected JSON response. Message: {message}")
+
+            if "httpCode" in data:
+                if data["httpCode"] == 401:
+                    if retries >= self.max_connect_retries:
+                        # wait 30 seconds before sending another request
+                        self._login_cooldown = time.time() + 30
+
+                    # key no longer works, so remove key and let the following .get() call refresh it
+                    self.key = None
+                    return await self.get(*args, retries=retries + 1, **kwargs)
+                else:
+                    msg = data.get("message", "")
+                    if data["httpCode"] == 404:
+                        msg = f"Missing resource {data.get('resource', args[0])}"
+                    raise InvalidRequest(f"HTTP {data['httpCode']}: {msg}", code=data["httpCode"])
+
+            return data
+        else:
+            return await resp.text()
+
+    async def get_player(self, name: str = None, uid: str = None, platform: str = "uplay") -> Player:
+        """ Calls get_players and returns the first element """
+
+        results = await self._find_players(name=name, platform=platform, uid=uid)
+        return results[0]
+
+    async def get_player_batch(self, names: list[str] = None, uids: list[str] = None, platform: str = "uplay") -> dict[str: Player]:
+        players = {}
+        if names is not None:
+            for name in names:
+                player = await self.get_player(name=name, platform=platform)
+                players[player.id] = player
+
+        if uids is not None:
+            for uid in uids:
+                player = await self.get_player(uid=uid, platform=platform)
+                players[player.id] = player
+        return players
```

### Comparing `siegeapi-6.0.1/siegeapi/constants/ranks.py` & `siegeapi-6.1.0/siegeapi/constants/ranks.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,174 +1,174 @@
-
-# Until Y1S3 | #3 | Skull Rain
-ranks_v1 = [
-    {"name": "Unranked", "min_mmr": 0, "max_mmr": 0},
-    {"name": "Copper 1", "min_mmr": 1, "max_mmr": 2199},
-    {"name": "Copper 2", "min_mmr": 2200, "max_mmr": 2399},
-    {"name": "Copper 3", "min_mmr": 2400, "max_mmr": 2549},
-    {"name": "Copper 4", "min_mmr": 2550, "max_mmr": 2699},
-    {"name": "Bronze 1", "min_mmr": 2700, "max_mmr": 2799},
-    {"name": "Bronze 2", "min_mmr": 2800, "max_mmr": 2899},
-    {"name": "Bronze 3", "min_mmr": 2900, "max_mmr": 3049},
-    {"name": "Bronze 4", "min_mmr": 3050, "max_mmr": 3199},
-    {"name": "Silver 1", "min_mmr": 3200, "max_mmr": 3349},
-    {"name": "Silver 2", "min_mmr": 3350, "max_mmr": 3519},
-    {"name": "Silver 3", "min_mmr": 3520, "max_mmr": 3699},
-    {"name": "Silver 4", "min_mmr": 3700, "max_mmr": 3929},
-    {"name": "Gold 1", "min_mmr": 3930, "max_mmr": 4159},
-    {"name": "Gold 2", "min_mmr": 4160, "max_mmr": 4399},
-    {"name": "Gold 3", "min_mmr": 4400, "max_mmr": 4639},
-    {"name": "Gold 4", "min_mmr": 4640, "max_mmr": 4899},
-    {"name": "Platinum 1", "min_mmr": 4900, "max_mmr": 5159},
-    {"name": "Platinum 2", "min_mmr": 5160, "max_mmr": 5449},
-    {"name": "Platinum 3", "min_mmr": 5450, "max_mmr": 5999},
-    {"name": "Diamond", "min_mmr": 6000, "max_mmr": 999999}
-]
-
-# Y1S4 | #4 | Red Crow
-ranks_v2 = [
-    {"name": "Unranked", "min_mmr": 0, "max_mmr": 0},
-    {"name": "Copper 1", "min_mmr": 1, "max_mmr": 1399},
-    {"name": "Copper 2", "min_mmr": 1400, "max_mmr": 1499},
-    {"name": "Copper 3", "min_mmr": 1500, "max_mmr": 1599},
-    {"name": "Copper 4", "min_mmr": 1600, "max_mmr": 1699},
-    {"name": "Bronze 1", "min_mmr": 1700, "max_mmr": 1799},
-    {"name": "Bronze 2", "min_mmr": 1800, "max_mmr": 1899},
-    {"name": "Bronze 3", "min_mmr": 1900, "max_mmr": 1999},
-    {"name": "Bronze 4", "min_mmr": 2000, "max_mmr": 2099},
-    {"name": "Silver 1", "min_mmr": 2100, "max_mmr": 2199},
-    {"name": "Silver 2", "min_mmr": 2200, "max_mmr": 2299},
-    {"name": "Silver 3", "min_mmr": 2300, "max_mmr": 2399},
-    {"name": "Silver 4", "min_mmr": 2400, "max_mmr": 2499},
-    {"name": "Gold 1", "min_mmr": 2500, "max_mmr": 2599},
-    {"name": "Gold 2", "min_mmr": 2600, "max_mmr": 2699},
-    {"name": "Gold 3", "min_mmr": 2700, "max_mmr": 2700},
-    {"name": "Gold 4", "min_mmr": 2800, "max_mmr": 2999},
-    {"name": "Platinum 1", "min_mmr": 3000, "max_mmr": 3199},
-    {"name": "Platinum 2", "min_mmr": 3200, "max_mmr": 3399},
-    {"name": "Platinum 3", "min_mmr": 3400, "max_mmr": 3699},
-    {"name": "Diamond", "min_mmr": 3700, "max_mmr": 999999}
-]
-
-# Y2S1 - Y4S2 | #5 - #14 | Velvet Shell - Phantom Sight
-ranks_v3 = [
-    {"name": "Unranked", "min_mmr": 0, "max_mmr": 0},
-    {"name": "Copper 4", "min_mmr": 1, "max_mmr": 1399},
-    {"name": "Copper 3", "min_mmr": 1400, "max_mmr": 1499},
-    {"name": "Copper 2", "min_mmr": 1500, "max_mmr": 1599},
-    {"name": "Copper 1", "min_mmr": 1600, "max_mmr": 1699},
-    {"name": "Bronze 4", "min_mmr": 1700, "max_mmr": 1799},
-    {"name": "Bronze 3", "min_mmr": 1800, "max_mmr": 1899},
-    {"name": "Bronze 2", "min_mmr": 1900, "max_mmr": 1999},
-    {"name": "Bronze 1", "min_mmr": 2000, "max_mmr": 2099},
-    {"name": "Silver 4", "min_mmr": 2100, "max_mmr": 2199},
-    {"name": "Silver 3", "min_mmr": 2200, "max_mmr": 2299},
-    {"name": "Silver 2", "min_mmr": 2300, "max_mmr": 2399},
-    {"name": "Silver 1", "min_mmr": 2400, "max_mmr": 2499},
-    {"name": "Gold 4", "min_mmr": 2500, "max_mmr": 2699},
-    {"name": "Gold 3", "min_mmr": 2700, "max_mmr": 2899},
-    {"name": "Gold 2", "min_mmr": 2900, "max_mmr": 3099},
-    {"name": "Gold 1", "min_mmr": 3100, "max_mmr": 3299},
-    {"name": "Platinum 3", "min_mmr": 3300, "max_mmr": 3699},
-    {"name": "Platinum 2", "min_mmr": 3700, "max_mmr": 4099},
-    {"name": "Platinum 1", "min_mmr": 4100, "max_mmr": 4499},
-    {"name": "Diamond", "min_mmr": 4500, "max_mmr": 999999}
-]
-
-# Y4S3 - Y6S2 | #15 - #22 | Ember Rise - North Star
-ranks_v4 = [
-    {"name": "Unranked", "min_mmr": 0, "max_mmr": 0},
-    {"name": "Copper 5", "min_mmr": 1, "max_mmr": 1199},
-    {"name": "Copper 4", "min_mmr": 1200, "max_mmr": 1299},
-    {"name": "Copper 3", "min_mmr": 1300, "max_mmr": 1399},
-    {"name": "Copper 2", "min_mmr": 1400, "max_mmr": 1499},
-    {"name": "Copper 1", "min_mmr": 1500, "max_mmr": 1599},
-    {"name": "Bronze 5", "min_mmr": 1600, "max_mmr": 1699},
-    {"name": "Bronze 4", "min_mmr": 1700, "max_mmr": 1799},
-    {"name": "Bronze 3", "min_mmr": 1800, "max_mmr": 1899},
-    {"name": "Bronze 2", "min_mmr": 1900, "max_mmr": 1999},
-    {"name": "Bronze 1", "min_mmr": 2000, "max_mmr": 2099},
-    {"name": "Silver 5", "min_mmr": 2100, "max_mmr": 2199},
-    {"name": "Silver 4", "min_mmr": 2200, "max_mmr": 2299},
-    {"name": "Silver 3", "min_mmr": 2300, "max_mmr": 2399},
-    {"name": "Silver 2", "min_mmr": 2400, "max_mmr": 2499},
-    {"name": "Silver 1", "min_mmr": 2500, "max_mmr": 2599},
-    {"name": "Gold 3", "min_mmr": 2600, "max_mmr": 2799},
-    {"name": "Gold 2", "min_mmr": 2800, "max_mmr": 2999},
-    {"name": "Gold 1", "min_mmr": 3000, "max_mmr": 3199},
-    {"name": "Platinum 3", "min_mmr": 3200, "max_mmr": 3599},
-    {"name": "Platinum 2", "min_mmr": 3600, "max_mmr": 3999},
-    {"name": "Platinum 1", "min_mmr": 4000, "max_mmr": 4399},
-    {"name": "Diamond", "min_mmr": 4400, "max_mmr": 4999},
-    {"name": "Champion", "min_mmr": 5000, "max_mmr": 999999}
-]
-
-# Y6S3 - Y7S3 | #23 - #27 | Crystal Guard - Brutal Swarm
-ranks_v5 = [
-    {"name": "Unranked", "min_mmr": 0, "max_mmr": 0},
-    {"name": "Copper 5", "min_mmr": 1, "max_mmr": 1199},
-    {"name": "Copper 4", "min_mmr": 1200, "max_mmr": 1299},
-    {"name": "Copper 3", "min_mmr": 1300, "max_mmr": 1399},
-    {"name": "Copper 2", "min_mmr": 1400, "max_mmr": 1499},
-    {"name": "Copper 1", "min_mmr": 1500, "max_mmr": 1599},
-    {"name": "Bronze 5", "min_mmr": 1600, "max_mmr": 1699},
-    {"name": "Bronze 4", "min_mmr": 1700, "max_mmr": 1799},
-    {"name": "Bronze 3", "min_mmr": 1800, "max_mmr": 1899},
-    {"name": "Bronze 2", "min_mmr": 1900, "max_mmr": 1999},
-    {"name": "Bronze 1", "min_mmr": 2000, "max_mmr": 2099},
-    {"name": "Silver 5", "min_mmr": 2100, "max_mmr": 2199},
-    {"name": "Silver 4", "min_mmr": 2200, "max_mmr": 2299},
-    {"name": "Silver 3", "min_mmr": 2300, "max_mmr": 2399},
-    {"name": "Silver 2", "min_mmr": 2400, "max_mmr": 2499},
-    {"name": "Silver 1", "min_mmr": 2500, "max_mmr": 2599},
-    {"name": "Gold 3", "min_mmr": 2600, "max_mmr": 2799},
-    {"name": "Gold 2", "min_mmr": 2800, "max_mmr": 2999},
-    {"name": "Gold 1", "min_mmr": 3000, "max_mmr": 3199},
-    {"name": "Platinum 3", "min_mmr": 3200, "max_mmr": 3499},
-    {"name": "Platinum 2", "min_mmr": 3500, "max_mmr": 3799},
-    {"name": "Platinum 1", "min_mmr": 3800, "max_mmr": 4099},
-    {"name": "Diamond 3", "min_mmr": 4100, "max_mmr": 4399},
-    {"name": "Diamond 2", "min_mmr": 4400, "max_mmr": 4699},
-    {"name": "Diamond 1", "min_mmr": 4700, "max_mmr": 4999},
-    {"name": "Champions", "min_mmr": 5000, "max_mmr": 999999}
-]
-
-# Y7S4+ | #28+ | Solar Raid+ (Ranked 2.0)
-ranks_v6 = [
-    {"min_mmr": 0,    "max_mmr": 999,  "name": "Unranked"},
-    {"min_mmr": 1000, "max_mmr": 1099, "name": "Copper 5"},
-    {"min_mmr": 1100, "max_mmr": 1199, "name": "Copper 4"},
-    {"min_mmr": 1200, "max_mmr": 1299, "name": "Copper 3"},
-    {"min_mmr": 1300, "max_mmr": 1399, "name": "Copper 2"},
-    {"min_mmr": 1400, "max_mmr": 1499, "name": "Copper 1"},
-    {"min_mmr": 1500, "max_mmr": 1599, "name": "Bronze 5"},
-    {"min_mmr": 1600, "max_mmr": 1699, "name": "Bronze 4"},
-    {"min_mmr": 1700, "max_mmr": 1799, "name": "Bronze 3"},
-    {"min_mmr": 1800, "max_mmr": 1899, "name": "Bronze 2"},
-    {"min_mmr": 1900, "max_mmr": 1999, "name": "Bronze 1"},
-    {"min_mmr": 2000, "max_mmr": 2099, "name": "Silver 5"},
-    {"min_mmr": 2100, "max_mmr": 2199, "name": "Silver 4"},
-    {"min_mmr": 2200, "max_mmr": 2299, "name": "Silver 3"},
-    {"min_mmr": 2300, "max_mmr": 2399, "name": "Silver 2"},
-    {"min_mmr": 2400, "max_mmr": 2499, "name": "Silver 1"},
-    {"min_mmr": 2500, "max_mmr": 2599, "name": "Gold 5"},
-    {"min_mmr": 2600, "max_mmr": 2699, "name": "Gold 4"},
-    {"min_mmr": 2700, "max_mmr": 2799, "name": "Gold 3"},
-    {"min_mmr": 2800, "max_mmr": 2899, "name": "Gold 2"},
-    {"min_mmr": 2900, "max_mmr": 2999, "name": "Gold 1"},
-    {"min_mmr": 3000, "max_mmr": 3099, "name": "Platinum 5"},
-    {"min_mmr": 3100, "max_mmr": 3199, "name": "Platinum 4"},
-    {"min_mmr": 3200, "max_mmr": 3299, "name": "Platinum 3"},
-    {"min_mmr": 3300, "max_mmr": 3399, "name": "Platinum 2"},
-    {"min_mmr": 3400, "max_mmr": 3499, "name": "Platinum 1"},
-    {"min_mmr": 3500, "max_mmr": 3599, "name": "Emerald 5"},
-    {"min_mmr": 3600, "max_mmr": 3699, "name": "Emerald 4"},
-    {"min_mmr": 3700, "max_mmr": 3799, "name": "Emerald 3"},
-    {"min_mmr": 3800, "max_mmr": 3899, "name": "Emerald 2"},
-    {"min_mmr": 3900, "max_mmr": 3999, "name": "Emerald 1"},
-    {"min_mmr": 4000, "max_mmr": 4099, "name": "Diamond 5"},
-    {"min_mmr": 4100, "max_mmr": 4199, "name": "Diamond 4"},
-    {"min_mmr": 4200, "max_mmr": 4299, "name": "Diamond 3"},
-    {"min_mmr": 4300, "max_mmr": 4399, "name": "Diamond 2"},
-    {"min_mmr": 4400, "max_mmr": 4499, "name": "Diamond 1"},
-    {"min_mmr": 4500, "max_mmr": 999999, "name": "Champions"}
-]
+
+# Until Y1S3 | #3 | Skull Rain
+ranks_v1 = [
+    {"name": "Unranked", "min_mmr": 0, "max_mmr": 0},
+    {"name": "Copper 1", "min_mmr": 1, "max_mmr": 2199},
+    {"name": "Copper 2", "min_mmr": 2200, "max_mmr": 2399},
+    {"name": "Copper 3", "min_mmr": 2400, "max_mmr": 2549},
+    {"name": "Copper 4", "min_mmr": 2550, "max_mmr": 2699},
+    {"name": "Bronze 1", "min_mmr": 2700, "max_mmr": 2799},
+    {"name": "Bronze 2", "min_mmr": 2800, "max_mmr": 2899},
+    {"name": "Bronze 3", "min_mmr": 2900, "max_mmr": 3049},
+    {"name": "Bronze 4", "min_mmr": 3050, "max_mmr": 3199},
+    {"name": "Silver 1", "min_mmr": 3200, "max_mmr": 3349},
+    {"name": "Silver 2", "min_mmr": 3350, "max_mmr": 3519},
+    {"name": "Silver 3", "min_mmr": 3520, "max_mmr": 3699},
+    {"name": "Silver 4", "min_mmr": 3700, "max_mmr": 3929},
+    {"name": "Gold 1", "min_mmr": 3930, "max_mmr": 4159},
+    {"name": "Gold 2", "min_mmr": 4160, "max_mmr": 4399},
+    {"name": "Gold 3", "min_mmr": 4400, "max_mmr": 4639},
+    {"name": "Gold 4", "min_mmr": 4640, "max_mmr": 4899},
+    {"name": "Platinum 1", "min_mmr": 4900, "max_mmr": 5159},
+    {"name": "Platinum 2", "min_mmr": 5160, "max_mmr": 5449},
+    {"name": "Platinum 3", "min_mmr": 5450, "max_mmr": 5999},
+    {"name": "Diamond", "min_mmr": 6000, "max_mmr": 999999}
+]
+
+# Y1S4 | #4 | Red Crow
+ranks_v2 = [
+    {"name": "Unranked", "min_mmr": 0, "max_mmr": 0},
+    {"name": "Copper 1", "min_mmr": 1, "max_mmr": 1399},
+    {"name": "Copper 2", "min_mmr": 1400, "max_mmr": 1499},
+    {"name": "Copper 3", "min_mmr": 1500, "max_mmr": 1599},
+    {"name": "Copper 4", "min_mmr": 1600, "max_mmr": 1699},
+    {"name": "Bronze 1", "min_mmr": 1700, "max_mmr": 1799},
+    {"name": "Bronze 2", "min_mmr": 1800, "max_mmr": 1899},
+    {"name": "Bronze 3", "min_mmr": 1900, "max_mmr": 1999},
+    {"name": "Bronze 4", "min_mmr": 2000, "max_mmr": 2099},
+    {"name": "Silver 1", "min_mmr": 2100, "max_mmr": 2199},
+    {"name": "Silver 2", "min_mmr": 2200, "max_mmr": 2299},
+    {"name": "Silver 3", "min_mmr": 2300, "max_mmr": 2399},
+    {"name": "Silver 4", "min_mmr": 2400, "max_mmr": 2499},
+    {"name": "Gold 1", "min_mmr": 2500, "max_mmr": 2599},
+    {"name": "Gold 2", "min_mmr": 2600, "max_mmr": 2699},
+    {"name": "Gold 3", "min_mmr": 2700, "max_mmr": 2700},
+    {"name": "Gold 4", "min_mmr": 2800, "max_mmr": 2999},
+    {"name": "Platinum 1", "min_mmr": 3000, "max_mmr": 3199},
+    {"name": "Platinum 2", "min_mmr": 3200, "max_mmr": 3399},
+    {"name": "Platinum 3", "min_mmr": 3400, "max_mmr": 3699},
+    {"name": "Diamond", "min_mmr": 3700, "max_mmr": 999999}
+]
+
+# Y2S1 - Y4S2 | #5 - #14 | Velvet Shell - Phantom Sight
+ranks_v3 = [
+    {"name": "Unranked", "min_mmr": 0, "max_mmr": 0},
+    {"name": "Copper 4", "min_mmr": 1, "max_mmr": 1399},
+    {"name": "Copper 3", "min_mmr": 1400, "max_mmr": 1499},
+    {"name": "Copper 2", "min_mmr": 1500, "max_mmr": 1599},
+    {"name": "Copper 1", "min_mmr": 1600, "max_mmr": 1699},
+    {"name": "Bronze 4", "min_mmr": 1700, "max_mmr": 1799},
+    {"name": "Bronze 3", "min_mmr": 1800, "max_mmr": 1899},
+    {"name": "Bronze 2", "min_mmr": 1900, "max_mmr": 1999},
+    {"name": "Bronze 1", "min_mmr": 2000, "max_mmr": 2099},
+    {"name": "Silver 4", "min_mmr": 2100, "max_mmr": 2199},
+    {"name": "Silver 3", "min_mmr": 2200, "max_mmr": 2299},
+    {"name": "Silver 2", "min_mmr": 2300, "max_mmr": 2399},
+    {"name": "Silver 1", "min_mmr": 2400, "max_mmr": 2499},
+    {"name": "Gold 4", "min_mmr": 2500, "max_mmr": 2699},
+    {"name": "Gold 3", "min_mmr": 2700, "max_mmr": 2899},
+    {"name": "Gold 2", "min_mmr": 2900, "max_mmr": 3099},
+    {"name": "Gold 1", "min_mmr": 3100, "max_mmr": 3299},
+    {"name": "Platinum 3", "min_mmr": 3300, "max_mmr": 3699},
+    {"name": "Platinum 2", "min_mmr": 3700, "max_mmr": 4099},
+    {"name": "Platinum 1", "min_mmr": 4100, "max_mmr": 4499},
+    {"name": "Diamond", "min_mmr": 4500, "max_mmr": 999999}
+]
+
+# Y4S3 - Y6S2 | #15 - #22 | Ember Rise - North Star
+ranks_v4 = [
+    {"name": "Unranked", "min_mmr": 0, "max_mmr": 0},
+    {"name": "Copper 5", "min_mmr": 1, "max_mmr": 1199},
+    {"name": "Copper 4", "min_mmr": 1200, "max_mmr": 1299},
+    {"name": "Copper 3", "min_mmr": 1300, "max_mmr": 1399},
+    {"name": "Copper 2", "min_mmr": 1400, "max_mmr": 1499},
+    {"name": "Copper 1", "min_mmr": 1500, "max_mmr": 1599},
+    {"name": "Bronze 5", "min_mmr": 1600, "max_mmr": 1699},
+    {"name": "Bronze 4", "min_mmr": 1700, "max_mmr": 1799},
+    {"name": "Bronze 3", "min_mmr": 1800, "max_mmr": 1899},
+    {"name": "Bronze 2", "min_mmr": 1900, "max_mmr": 1999},
+    {"name": "Bronze 1", "min_mmr": 2000, "max_mmr": 2099},
+    {"name": "Silver 5", "min_mmr": 2100, "max_mmr": 2199},
+    {"name": "Silver 4", "min_mmr": 2200, "max_mmr": 2299},
+    {"name": "Silver 3", "min_mmr": 2300, "max_mmr": 2399},
+    {"name": "Silver 2", "min_mmr": 2400, "max_mmr": 2499},
+    {"name": "Silver 1", "min_mmr": 2500, "max_mmr": 2599},
+    {"name": "Gold 3", "min_mmr": 2600, "max_mmr": 2799},
+    {"name": "Gold 2", "min_mmr": 2800, "max_mmr": 2999},
+    {"name": "Gold 1", "min_mmr": 3000, "max_mmr": 3199},
+    {"name": "Platinum 3", "min_mmr": 3200, "max_mmr": 3599},
+    {"name": "Platinum 2", "min_mmr": 3600, "max_mmr": 3999},
+    {"name": "Platinum 1", "min_mmr": 4000, "max_mmr": 4399},
+    {"name": "Diamond", "min_mmr": 4400, "max_mmr": 4999},
+    {"name": "Champion", "min_mmr": 5000, "max_mmr": 999999}
+]
+
+# Y6S3 - Y7S3 | #23 - #27 | Crystal Guard - Brutal Swarm
+ranks_v5 = [
+    {"name": "Unranked", "min_mmr": 0, "max_mmr": 0},
+    {"name": "Copper 5", "min_mmr": 1, "max_mmr": 1199},
+    {"name": "Copper 4", "min_mmr": 1200, "max_mmr": 1299},
+    {"name": "Copper 3", "min_mmr": 1300, "max_mmr": 1399},
+    {"name": "Copper 2", "min_mmr": 1400, "max_mmr": 1499},
+    {"name": "Copper 1", "min_mmr": 1500, "max_mmr": 1599},
+    {"name": "Bronze 5", "min_mmr": 1600, "max_mmr": 1699},
+    {"name": "Bronze 4", "min_mmr": 1700, "max_mmr": 1799},
+    {"name": "Bronze 3", "min_mmr": 1800, "max_mmr": 1899},
+    {"name": "Bronze 2", "min_mmr": 1900, "max_mmr": 1999},
+    {"name": "Bronze 1", "min_mmr": 2000, "max_mmr": 2099},
+    {"name": "Silver 5", "min_mmr": 2100, "max_mmr": 2199},
+    {"name": "Silver 4", "min_mmr": 2200, "max_mmr": 2299},
+    {"name": "Silver 3", "min_mmr": 2300, "max_mmr": 2399},
+    {"name": "Silver 2", "min_mmr": 2400, "max_mmr": 2499},
+    {"name": "Silver 1", "min_mmr": 2500, "max_mmr": 2599},
+    {"name": "Gold 3", "min_mmr": 2600, "max_mmr": 2799},
+    {"name": "Gold 2", "min_mmr": 2800, "max_mmr": 2999},
+    {"name": "Gold 1", "min_mmr": 3000, "max_mmr": 3199},
+    {"name": "Platinum 3", "min_mmr": 3200, "max_mmr": 3499},
+    {"name": "Platinum 2", "min_mmr": 3500, "max_mmr": 3799},
+    {"name": "Platinum 1", "min_mmr": 3800, "max_mmr": 4099},
+    {"name": "Diamond 3", "min_mmr": 4100, "max_mmr": 4399},
+    {"name": "Diamond 2", "min_mmr": 4400, "max_mmr": 4699},
+    {"name": "Diamond 1", "min_mmr": 4700, "max_mmr": 4999},
+    {"name": "Champions", "min_mmr": 5000, "max_mmr": 999999}
+]
+
+# Y7S4+ | #28+ | Solar Raid+ (Ranked 2.0)
+ranks_v6 = [
+    {"min_mmr": 0,    "max_mmr": 999,  "name": "Unranked"},
+    {"min_mmr": 1000, "max_mmr": 1099, "name": "Copper 5"},
+    {"min_mmr": 1100, "max_mmr": 1199, "name": "Copper 4"},
+    {"min_mmr": 1200, "max_mmr": 1299, "name": "Copper 3"},
+    {"min_mmr": 1300, "max_mmr": 1399, "name": "Copper 2"},
+    {"min_mmr": 1400, "max_mmr": 1499, "name": "Copper 1"},
+    {"min_mmr": 1500, "max_mmr": 1599, "name": "Bronze 5"},
+    {"min_mmr": 1600, "max_mmr": 1699, "name": "Bronze 4"},
+    {"min_mmr": 1700, "max_mmr": 1799, "name": "Bronze 3"},
+    {"min_mmr": 1800, "max_mmr": 1899, "name": "Bronze 2"},
+    {"min_mmr": 1900, "max_mmr": 1999, "name": "Bronze 1"},
+    {"min_mmr": 2000, "max_mmr": 2099, "name": "Silver 5"},
+    {"min_mmr": 2100, "max_mmr": 2199, "name": "Silver 4"},
+    {"min_mmr": 2200, "max_mmr": 2299, "name": "Silver 3"},
+    {"min_mmr": 2300, "max_mmr": 2399, "name": "Silver 2"},
+    {"min_mmr": 2400, "max_mmr": 2499, "name": "Silver 1"},
+    {"min_mmr": 2500, "max_mmr": 2599, "name": "Gold 5"},
+    {"min_mmr": 2600, "max_mmr": 2699, "name": "Gold 4"},
+    {"min_mmr": 2700, "max_mmr": 2799, "name": "Gold 3"},
+    {"min_mmr": 2800, "max_mmr": 2899, "name": "Gold 2"},
+    {"min_mmr": 2900, "max_mmr": 2999, "name": "Gold 1"},
+    {"min_mmr": 3000, "max_mmr": 3099, "name": "Platinum 5"},
+    {"min_mmr": 3100, "max_mmr": 3199, "name": "Platinum 4"},
+    {"min_mmr": 3200, "max_mmr": 3299, "name": "Platinum 3"},
+    {"min_mmr": 3300, "max_mmr": 3399, "name": "Platinum 2"},
+    {"min_mmr": 3400, "max_mmr": 3499, "name": "Platinum 1"},
+    {"min_mmr": 3500, "max_mmr": 3599, "name": "Emerald 5"},
+    {"min_mmr": 3600, "max_mmr": 3699, "name": "Emerald 4"},
+    {"min_mmr": 3700, "max_mmr": 3799, "name": "Emerald 3"},
+    {"min_mmr": 3800, "max_mmr": 3899, "name": "Emerald 2"},
+    {"min_mmr": 3900, "max_mmr": 3999, "name": "Emerald 1"},
+    {"min_mmr": 4000, "max_mmr": 4099, "name": "Diamond 5"},
+    {"min_mmr": 4100, "max_mmr": 4199, "name": "Diamond 4"},
+    {"min_mmr": 4200, "max_mmr": 4299, "name": "Diamond 3"},
+    {"min_mmr": 4300, "max_mmr": 4399, "name": "Diamond 2"},
+    {"min_mmr": 4400, "max_mmr": 4499, "name": "Diamond 1"},
+    {"min_mmr": 4500, "max_mmr": 999999, "name": "Champions"}
+]
```

### Comparing `siegeapi-6.0.1/siegeapi/constants/weapons.py` & `siegeapi-6.1.0/siegeapi/constants/weapons.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,580 +1,580 @@
-
-WEAPONS_DICT = {
-
-    # Primary Weapons
-    # AR's
-    "POF9": {
-        "type": "Assault Rifle",
-        "icon_url": "1bhuAox7U6aHN6UriXsAry/3c213cd27f5f64ba01a29b42e5b24ac5/POF9.png",
-        "imgur_url": "https://i.imgur.com/D2FkIjZ.png",
-    },
-    "AK-12": {
-        "type": "Assault Rifle",
-        "icon_url": "7KAZZgnpqD07y47jVVXEuh/e0d7e67101f8f966aa6e1c59e835454f/AK-12.png",
-        "imgur_url": "https://i.imgur.com/XkqUvyS.png",
-    },
-    "SC3000K": {
-        "type": "Assault Rifle",
-        "icon_url": "7x7eDTm2NNpfGiFMrfQqEX/9898e74c780537be3ca6d88db32ea21e/F2000.png",
-        "imgur_url": "https://i.imgur.com/93Vx6y4.png",
-    },
-    "V308": {
-        "type": "Assault Rifle",
-        "icon_url": "5YBZe76NUDO32eF66wW90g/488c315743d59230962a4d67618223d6/V308.png",
-        "imgur_url": "https://i.imgur.com/xoxtQFf.png",
-    },
-    "416-C CARBINE": {
-        "type": "Assault Rifle",
-        "icon_url": "2I86r2a2QD8EHTZVZnxcxy/2913450ba952a16c29fac1f5ce58ba1a/416-C_Carbine.png",
-        "imgur_url": "https://i.imgur.com/18j266k.png",
-    },
-    "556XI": {
-        "type": "Assault Rifle",
-        "icon_url": "2dgpAeAWb3SkZV7rxDbVdQ/fa32323256b7c6f8a1977d3f71e7d4b2/556xi.png",
-        "imgur_url": "https://i.imgur.com/l3Z9O2Q.png",
-    },
-    "M762": {
-        "type": "Assault Rifle",
-        "icon_url": "4oWAgi7tgQP1Tq0HooRtye/9109a74921ee17610d4bd85a61582823/M762.png",
-        "imgur_url": "https://i.imgur.com/bJqHwKt.png",
-    },
-    "TYPE-89": {
-        "type": "Assault Rifle",
-        "icon_url": "7wLf325q9amF8bnVP1QGr0/2faff1a197f90dcded4472852a317d6b/Type-89.png",
-        "imgur_url": "https://i.imgur.com/hGDt4zV.png",
-    },
-    "M4": {
-        "type": "Assault Rifle",
-        "icon_url": "3jhi90ycmuc8mAiuSXFoCi/bcf354459e7becd6ede52ee97917c832/M4.png",
-        "imgur_url": "https://i.imgur.com/lKDElT7.png",
-    },
-    "PARA-308": {
-        "type": "Assault Rifle",
-        "icon_url": "6ub8y2Cs5EYhVPfDWuVVkW/82ca131a41ee4ba2e0b75f2dc52ed9e3/PARA-308.png",
-        "imgur_url": "https://i.imgur.com/246krdt.png",
-    },
-    "SPEAR .308": {
-        "type": "Assault Rifle",
-        "icon_url": "29LjYuJ4s6yA8k9Uv2u28C/89ec812559e7d74b7c269279f4c46d92/Spear_.308.png",
-        "imgur_url": "https://i.imgur.com/PNyKa6N.png",
-    },
-    "AK-74M": {
-        "type": "Assault Rifle",
-        "icon_url": "1j5HiQP8aFphTe65fqDdg0/23eecb5c603c5ba9f59fc6cbc5e4a531/AK-74M.png",
-        "imgur_url": "https://i.imgur.com/bOB4yay.png",
-    },
-    "AR33": {
-        "type": "Assault Rifle",
-        "icon_url": "16U6xEvX8I5xQd9duveBLN/45d22960872cfa3fb6be9eb47fa0be4e/AR33.png",
-        "imgur_url": "https://i.imgur.com/fSUxgbS.png",
-    },
-    "L85A2": {
-        "type": "Assault Rifle",
-        "icon_url": "5vYQpoyk36foDzDq49jBd0/1479a2d7189e545555ceccecf6bd7cc3/L85A2.png",
-        "imgur_url": "https://i.imgur.com/dFG30nS.png",
-    },
-    "G36C": {
-        "type": "Assault Rifle",
-        "icon_url": "2SZoqSXKoNPvZFIJsFsDE5/cb109885bf19c8697abf832f10cfd9a6/G36C.png",
-        "imgur_url": "https://i.imgur.com/YuXb3x9.png",
-    },
-    "COMMANDO 9": {
-        "type": "Assault Rifle",
-        "icon_url": "4P9dpUph5w3MSsLNnW6be/04baba24990fcb75a9c0bcfd01b7d190/Commando_9.png",
-        "imgur_url": "https://i.imgur.com/Jo2DJHb.png",
-    },
-    "AUG A2": {
-        "type": "Assault Rifle",
-        "icon_url": "1eO39zRe8XxJXH1KZiIWhM/02049ced0fbfa630833e8b0d3c03de07/AUG_A2.png",
-        "imgur_url": "https://i.imgur.com/SG0dmYt.png",
-    },
-    "F2": {
-        "type": "Assault Rifle",
-        "icon_url": "5HTvw1cJInVAGxOLXR0war/2f142437f5c0944fdcfcce8a03c37676/F2.png",
-        "imgur_url": "https://i.imgur.com/B9oWguM.png",
-    },
-    "C8-SFW": {
-        "type": "Assault Rifle",
-        "icon_url": "1itXpz2GnvdwwRyhX1SYa2/b58ff71048fa3bb5ed09d5d935dc90f4/C8-SFW.png",
-        "imgur_url": "https://i.imgur.com/kxqQRY5.png",
-    },
-    "R4-C": {
-        "type": "Assault Rifle",
-        "icon_url": "dQbqK9VxczuiscwBDSkT8/777a062f6095dde0371eab5200dcb451/R4-C.png",
-        "imgur_url": "https://i.imgur.com/pBxDdF5.png",
-    },
-    "C7E": {
-        "type": "Assault Rifle",
-        "icon_url": "63vTDjkXeKq7rOoSBhoJD4/08603e6603d564e0fa38af9ec86b7c1f/C7E.png",
-        "imgur_url": "https://i.imgur.com/m0vBz74.png",
-    },
-    "MK17 CQB": {
-        "type": "Assault Rifle",
-        "icon_url": "4LytczDQmu0M63gO2WtCCm/331ef3b1938352ae71d7c0bd23de3596/Mk17_CQB.png",
-        "imgur_url": "https://i.imgur.com/qFieFCz.png",
-    },
-    "552 COMMANDO": {
-        "type": "Assault Rifle",
-        "icon_url": "1LT0N89YaOHvRwn3Pphr8K/02d4a3da9cda132d8201fd134f24fede/552_Commando.png",
-        "imgur_url": "https://i.imgur.com/iyeigKx.png",
-    },
-    "ARX200": {
-        "type": "Assault Rifle",
-        "icon_url": "6VgkPBsr1WApI3rWc9kcM0/b18b8e25f3e951e8e722213f2ee59eb0/ARX200.png",
-        "imgur_url": "https://i.imgur.com/pjJNhg0.png",
-    },
-    "F90": {
-        "type": "Assault Rifle",
-        "icon_url": "62tE3th2ThcGHlrcqWkmEX/d69c9de199542e25fa55f6d293f15671/r6-operator-weapon-ar-f90.png",
-        "imgur_url": "https://i.imgur.com/ltvoR5e.png",
-    },
-
-    # Submachine Guns
-    "P90": {
-        "type": "Submachine Gun",
-        "icon_url": "4nGrNspOvII2oS3lEMkg5x/2398a493c298bc654f97c58767aa40f3/P90.png",
-        "imgur_url": "https://i.imgur.com/JioXAPs.png",
-    },
-    "9mm C1": {
-        "type": "Submachine Gun",
-        "icon_url": "60sbThKtOpNOwKu3OP0oGV/672fd9263f7786402a0d855273473a6f/9mm_C1.png",
-        "imgur_url": "https://i.imgur.com/CSicnOY.png",
-    },
-    "AUG A3": {
-        "type": "Submachine Gun",
-        "icon_url": "3W9XJdMOgpHSw55HfwRSAv/cf8f220678d503e6c3e535c00b2e636a/AUG_A3.png",
-        "imgur_url": "https://i.imgur.com/EwhrsYo.png",
-    },
-    "VECTOR .45 ACP": {
-        "type": "Submachine Gun",
-        "icon_url": "7D1cDf13FqUhoLihzvuPln/068aa7e507155598449c58c0a49a90d6/Vector_.45_ACP.png",
-        "imgur_url": "https://i.imgur.com/nYqNJVY.png",
-    },
-    "M12": {
-        "type": "Submachine Gun",
-        "icon_url": "4FxqA5pa8JY9QQ7FEcjwPw/ffc779fcde5b970e7b95db6653637dab/M12.png",
-        "imgur_url": "https://i.imgur.com/xnjqNAP.png",
-    },
-    "FMG-9": {
-        "type": "Submachine Gun",
-        "icon_url": "0oneJNsBR06QjuowxwtHG/bd3b391c6eec2bd615f2ed83197a13ac/FMG-9.png",
-        "imgur_url": "https://i.imgur.com/Sv4LCCi.png",
-    },
-    "PDW9": {
-        "type": "Submachine Gun",
-        "icon_url": "4yYCuRnduMq35CTHfq6wwU/b7d49cdbcb05917e014c99efeaadd33b/PDW9.png",
-        "imgur_url": "https://i.imgur.com/SfD33PY.png",
-    },
-    "UMP45": {
-        "type": "Submachine Gun",
-        "icon_url": "6X2EZPq2s8UKrP67uxz5FI/f0df4c57d5890c79311e4eb62d4470e7/UMP45.png",
-        "imgur_url": "https://i.imgur.com/DXCAI3x.png",
-    },
-    "SCORPION EVO 3 A1": {
-        "type": "Submachine Gun",
-        "icon_url": "6OdwaLWxcnFvhlVwWbP2Du/4f7e94bdb6d34d5c0aa7b7b147b4092e/Scorpion_EVO_3_A1.png",
-        "imgur_url": "https://i.imgur.com/Xf4RkeF.png",
-    },
-    "P10 RONI": {
-        "type": "Submachine Gun",
-        "icon_url": "7K86OBjL3zmYWt0ZvUcCLj/16a947334e39f27da177d787773593e4/r6-operator-weapon-smg-p10roni.png",
-        "imgur_url": "https://i.imgur.com/am0iQln.png",
-    },
-    "MP5": {
-        "type": "Submachine Gun",
-        "icon_url": "60YbOvSBQt6ZUlu8YDXoZm/51ef3857b2986de700262432e8433714/MP5.png",
-        "imgur_url": "https://i.imgur.com/PUJ9el4.png",
-    },
-    "MPX": {
-        "type": "Submachine Gun",
-        "icon_url": "5HFewpAJ8npDDCKFnEadhL/d398bb477d6b56fe41bfdb5862ed31c0/MPX.png",
-        "imgur_url": "https://i.imgur.com/0lGbMaK.png",
-    },
-    "MP7": {
-        "type": "Submachine Gun",
-        "icon_url": "3a4dgTWGdiJqALhtRp4pKy/f2568d3de3cfe7e4b53179e8653cd2a2/MP7.png",
-        "imgur_url": "https://i.imgur.com/nTLMXY7.png",
-    },
-    "MP5SD": {
-        "type": "Submachine Gun",
-        "icon_url": "5HaMldwFltBwiiyDDfkPpD/6de3aa9aaa17458e7f6186ba59b8deff/MP5SD.png",
-        "imgur_url": "https://i.imgur.com/l5UoMyK.png",
-    },
-    "T-5 SMG": {
-        "type": "Submachine Gun",
-        "icon_url": "1Ne8bvX8BdCALevWKMllQN/4baa3e79d323de134dd182e0272b9c3b/T-5_SMG.png",
-        "imgur_url": "https://i.imgur.com/aJD4n8e.png",
-    },
-    "K1A": {
-        "type": "Submachine Gun",
-        "icon_url": "5mUa2p8WXbiyD71qUI8sGk/ed753b6f0ae30ab5737486dfcf32ee9f/K1A.png",
-        "imgur_url": "https://i.imgur.com/ASxXNFF.png",
-    },
-    "Mx4 Storm": {
-        "type": "Submachine Gun",
-        "icon_url": "4qRh1frGkQZxNyeKA4D6n1/20f89cd1d9953f06207b7340ea77fb17/Mx4_Storm.png",
-        "imgur_url": "https://i.imgur.com/0KjOTla.png",
-    },
-    "UZK50GI": {
-        "type": "Submachine Gun",
-        "icon_url": "5WMIsPUWTXprZnAwctPsTt/f1c652b681e7e9ba6ba66bcd29e12a76/uzk50gi.png",
-        "imgur_url": "https://i.imgur.com/EjnVX3B.png",
-    },
-    "9x19VSN": {
-        "type": "Submachine Gun",
-        "icon_url": "42gH96xTTYaTZsfXI3c0wL/a7edbf11af97091ee884b68e59fe6a4f/9x19VSN.png",
-        "imgur_url": "https://i.imgur.com/YM28ZXk.png",
-    },
-    "MP5K": {
-        "type": "Submachine Gun",
-        "icon_url": "1pk8nOI7ybQjYOSI4fuzOm/fcd78df0f729be545e75c09aae85c360/MP5K.png",
-        "imgur_url": "https://i.imgur.com/cJnZz6l.png",
-    },
-
-    # Marksman Rifles
-    "SR-25": {
-        "type": "Marksman Rifle",
-        "icon_url": "3H3sICdj6BK8LhtQPRd2aJ/26826ebba73e0e5fd503256d069f3256/SR-25.png",
-        "imgur_url": "https://i.imgur.com/GAwCFpP.png",
-    },
-    "AR-15.50": {
-        "type": "Marksman Rifle",
-        "icon_url": "4lGGEGZLkbldz114Wl5hCo/78a04c46654f80fae03e730bd79f3563/AR-15.50.png",
-        "imgur_url": "https://i.imgur.com/k4RWCgE.png",
-    },
-    "417": {
-        "type": "Marksman Rifle",
-        "icon_url": "5djkS4YtAtOF0vBmg0T60x/ea2b1ff7e5367e66c99bc7ad7e95bfe3/417.png",
-        "imgur_url": "https://i.imgur.com/XM1aYZ0.png",
-    },
-    "Mk 14 EBR": {
-        "type": "Marksman Rifle",
-        "icon_url": "6KIMqp5dA95z1RI3PrG9jv/eb939638169811a3fa858a44e6e5d97e/Mk_14_EBR.png",
-        "imgur_url": "https://i.imgur.com/a7tnoMB.png",
-    },
-    "OTs-03": {
-        "type": "Marksman Rifle",
-        "icon_url": "4fXznwDtLt61VCF8QIF4N3/34e2e6d6c33d4c504c945bdd13c322f6/OTs-03.png",
-        "imgur_url": "https://i.imgur.com/SvaWAHY.png",
-    },
-    "CSRX 300": {
-        "type": "Marksman Rifle",
-        "icon_url": "7tUB9ZNXJhdN6ejAkCEeFQ/99691bcc19f641cf872925905d08a539/CSRX_300.png",
-        "imgur_url": "https://i.imgur.com/QIpmJkI.png",
-    },
-    "CAMRS": {
-        "type": "Marksman Rifle",
-        "icon_url": "4dBzqVVmnpv1DZi91LAnEN/e374b4ea289fc992280b943cdbb94d60/CAMRS.png",
-        "imgur_url": "https://i.imgur.com/jRgdhPK.png",
-    },
-
-    # Shotguns
-    "ACS12": {
-        "type": "Shotgun",
-        "icon_url": "13z63kT1NLzn1U99o7WC4T/8655d3200f24b87246c36f2622603457/ACS12_PB.png",
-        "imgur_url": "https://i.imgur.com/oWkeNV1.png",
-    },
-    "M590A1": {
-        "type": "Shotgun",
-        "icon_url": "2zRHmgqENNiZqXQxC9Rsbj/e6542407c642f9b7c5a4546afb6db30a/M590A1.png",
-        "imgur_url": "https://i.imgur.com/1hKRvhC.png",
-    },
-    "M870": {
-        "type": "Shotgun",
-        "icon_url": "2rkU6g4Rlg0e0U4rczWGTV/a51589a54c43f476d8eb984c0ea881e9/M870.png",
-        "imgur_url": "https://i.imgur.com/2DulKY2.png",
-    },
-    "TCSG12": {
-        "type": "Shotgun",
-        "icon_url": "2NDbY7BTBJ9R09LUilTlRf/3728337cd3ba14ed6ab9de0c22e879af/TCSG12.png",
-        "imgur_url": "https://i.imgur.com/jxNiaOx.png",
-    },
-    # Yep, twice, because Ubi doesn't know how their own guns are named :)
-    "FO-12": {
-        "type": "Shotgun",
-        "icon_url": "4TDWnhbgvLkc6HBWDJp2ST/f50cbd83d6d295ab59f17f7e21d713bc/FO-12.png",
-        "imgur_url": "https://i.imgur.com/9mWXMtL.png",
-    },
-    "F0-12": {
-        "type": "Shotgun",
-        "icon_url": "4TDWnhbgvLkc6HBWDJp2ST/f50cbd83d6d295ab59f17f7e21d713bc/FO-12.png",
-        "imgur_url": "https://i.imgur.com/9mWXMtL.png",
-    },
-    "SIX12": {
-        "type": "Shotgun",
-        "icon_url": "2v6MwsHwjOZ5Muid53lyfN/e5f1c4997db93abfe3ac356fce23376c/SIX12.png",
-        "imgur_url": "https://i.imgur.com/XMdA44M.png",
-    },
-    "SIX12 SD": {
-        "type": "Shotgun",
-        "icon_url": "1GTua079Xbtkpjhx96sRsW/079ed1a71a0d12b5e48e1b0d40b87110/SIX12_SD.png",
-        "imgur_url": "https://i.imgur.com/yco3bh7.png",
-    },
-    "M1014": {
-        "type": "Shotgun",
-        "icon_url": "2pUiVbwNnQnDTesmWXktqW/f27c1fab9a354bb89cbe309a688f5e02/M1014.png",
-        "imgur_url": "https://i.imgur.com/QoKV2HB.png",
-    },
-    "SG-CQB": {
-        "type": "Shotgun",
-        "icon_url": "5JoL3b36Fsztt9Q2XYmrbJ/dacec96948d3f8fe92914a69b9aac593/SG-CQB.png",
-        "imgur_url": "https://i.imgur.com/878GOhH.png",
-    },
-    "SPAS-15": {
-        "type": "Shotgun",
-        "icon_url": "CyofBgipHq4RTafvPFWd4/bc3d0ecc871b70e57735855f852efacf/SPAS-15.png",
-        "imgur_url": "https://i.imgur.com/ptUqPpu.png",
-    },
-    "SPAS-12": {
-        "type": "Shotgun",
-        "icon_url": "7Hp6Fbss6uI59OT4nZNB6e/a4d09954803cb2580353cfa03e8c778b/SPAS-12.png",
-        "imgur_url": "https://i.imgur.com/wMvRHWE.png",
-    },
-    "SASG-12": {
-        "type": "Shotgun",
-        "icon_url": "2Q6mL4CbifmIgifV2yV3Hi/2bb2b323f055b03a2c1ba516c262c24e/SASG-12.png",
-        "imgur_url": "https://i.imgur.com/TASWBEp.png",
-    },
-    "Supernova": {
-        "type": "Shotgun",
-        "icon_url": "2tpjCRFLcc3hogjJGbKDsi/5ad0ab63b7245022aca5c1c1fb42d473/SuperNova.png",
-        "imgur_url": "https://i.imgur.com/gshdPvF.png",
-    },
-    "ITA12L": {
-        "type": "Shotgun",
-        "icon_url": "4Y6ziRzm9RiPii83fm8BV1/1f472744d2c2dec8d9206f4d8733d92c/ITA12L.png",
-        "imgur_url": "https://i.imgur.com/ldY0IlZ.png",
-    },
-    "BOSG.12.2": {
-        "type": "Shotgun",
-        "icon_url": "2ZjVndetsX8WEn5ZfyUQa0/e3a781be7eab22876d25f748e8fd0f5a/BOSG.12.2.png",
-        "imgur_url": "https://i.imgur.com/90I2Sb8.png",
-    },
-
-    # Light Machine Guns
-    "G8A1": {
-        "type": "Light Machine Gun",
-        "icon_url": "4TIb7oeJesaROOOfTlCBaZ/ffd6a802f9a779a0d39b2122c49b3254/G8A1.png",
-        "imgur_url": "https://i.imgur.com/Wy6HdZW.png",
-    },
-    "LMG-E": {
-        "type": "Light Machine Gun",
-        "icon_url": "7JVJIew6t3iKwgByvrFXyi/7ba44dfda28b525506633e453104a604/LMG-E.png",
-        "imgur_url": "https://i.imgur.com/UWXTqIL.png",
-    },
-    "M249 SAW": {
-        "type": "Light Machine Gun",
-        "icon_url": "3p0oG7GsLIoHaRullf7xsF/e2a9e135af63e8897355023cd34538c4/M249_SAW.png",
-        "imgur_url": "https://i.imgur.com/dWLYeNw.png",
-    },
-    "M249": {
-        "type": "Light Machine Gun",
-        "icon_url": "7z8UpVPS3P14OC1oL9dDIn/39c0c657f154218003fd4b2a9250b92f/M249.png",
-        "imgur_url": "https://i.imgur.com/gQOhuzN.png",
-    },
-    "ALDA 5.56": {
-        "type": "Light Machine Gun",
-        "icon_url": "39yB6TFl9ph6Rb4bDV4lqK/7f9b3abf8dff19bacc026a7212849ca4/ALDA_5.56.png",
-        "imgur_url": "https://i.imgur.com/uNiNSiM.png",
-    },
-    "6P41": {
-        "type": "Light Machine Gun",
-        "icon_url": "1wxS2HOCvoPAfnJEDFWjfw/7feddb98582ec37b500243d3f3e19eca/6P41.png",
-        "imgur_url": "https://i.imgur.com/nv4v9Q4.png",
-    },
-    "DP28": {
-        "type": "Light Machine Gun",
-        "icon_url": "7LoT7yAe0LK7bDOeq6MZZM/33995bc704667674af1b73fe962d4c7c/Primary_gun_DP27.png",
-        "imgur_url": "https://i.imgur.com/EuXUXJt.png",
-    },
-    "DP27": {
-        "type": "Light Machine Gun",
-        "icon_url": "7LoT7yAe0LK7bDOeq6MZZM/33995bc704667674af1b73fe962d4c7c/Primary_gun_DP27.png",
-        "imgur_url": "https://i.imgur.com/EuXUXJt.png",
-    },
-    "T-95 LSW": {
-        "type": "Light Machine Gun",
-        "icon_url": "23HCxaNTRUHBlFAvCTMZQm/fe319cc164fac034a29e9b114ae7d5cb/T-95_LSW.png",
-        "imgur_url": "https://i.imgur.com/6QCVGPg.png",
-    },
-
-    # Gadget
-    "CCE SHIELD": {
-        "type": "Gadget",
-        "icon_url": "5mmGgrYdJJHw2moBIEW9An/64e9727d959d7afdbb4fb06e2f75574a/CCE_Shield.png",
-        "imgur_url": "https://i.imgur.com/3CmDzwG.png",
-    },
-    # Shield
-    "Le Roc": {
-        "type": "Shield",
-        "icon_url": "1bmXJOakdA6SOrGxBKA70T/1e489e366d6db287f475963df2040d3d/Extendable-Shield.png",
-        "imgur_url": "https://i.imgur.com/pTB9tOm.png",
-    },
-    # Ops ability
-    "FLASH SHIELD": {
-        "type": "Ops ability",
-        "icon_url": "7qmWjGZayvK4t6E80Gvu7g/8b789d6d639744dce100c2cfb9709e6a/G52-Tactical_Shield.png",
-        "imgur_url": "https://i.imgur.com/OFeah3y.png",
-    },
-    # None
-    "None": {
-        "type": "None",
-        "icon_url": "yeah_lmao.png",
-        "imgur_url": "https://i.imgur.com/yeah_lmao.png",
-    },
-
-    # Secondary Weapons
-    # Shotguns
-    "SUPER SHORTY": {
-        "type": "Shotgun",
-        "icon_url": "7Dq8LDmIxAveRqXM17orUW/cbd96b47cd8ca74a7827b16ef73fe7cf/r6-operator-weapon-sa-supershorty.png",
-        "imgur_url": "https://i.imgur.com/ceMDeDV.png",
-    },
-    "ITA12S": {
-        "type": "Shotgun",
-        "icon_url": "5G4DroaSdqHzJWCe7qqbHZ/5dd2e03f853182c78a1e7fcbc642f0cf/ITA12S.png",
-        "imgur_url": "https://i.imgur.com/gKRXgpZ.png",
-    },
-
-    # Machine Pistols
-    "SMG-11": {
-        "type": "Machine Pistol",
-        "icon_url": "3WExw7Kepz9uAiWAbWW457/875fc631a3cf9fcc2849d9db2989cbcd/SMG-11.png",
-        "imgur_url": "https://i.imgur.com/HVuD3gD.png",
-    },
-    "SMG-12": {
-        "type": "Machine Pistol",
-        "icon_url": "EwJgB7KdgOb6dDm7ro33u/b73f0890f992c1a365210f08efcc6db5/SMG-12.png",
-        "imgur_url": "https://i.imgur.com/1fC7KAS.png",
-    },
-    "BEARING 9": {
-        "type": "Machine Pistol",
-        "icon_url": "4mdftEOh5Vu9KhhpgKLKrT/abedcc75868774018295ec2a08a7b3de/Bearing_9.png",
-        "imgur_url": "https://i.imgur.com/wT1qVsk.png",
-    },
-    "C75 Auto": {
-        "type": "Machine Pistol",
-        "icon_url": "3wUuefwPjU705mZkTdJ9UH/8ccb11884cfa34c176ac5500af139177/C75_Auto.png",
-        "imgur_url": "https://i.imgur.com/VA1Y1FG.png",
-    },
-    "SPSMG9": {
-        "type": "Machine Pistol",
-        "icon_url": "5EtwSgylXckBNg4n6gDR9J/bc6fc6c5c12ae11da59aee95828ebd76/SPSMG9.png",
-        "imgur_url": "https://i.imgur.com/owfOEEn.png",
-    },
-
-    # Pistols
-    "M45 MEUSOC": {
-        "type": "Pistol",
-        "icon_url": "3u5cecgWYl3WuJK50mKEGd/a4a0eb15c710edfc0d29e98c2ee7ea33/M45_MEUSOC.png",
-        "imgur_url": "https://i.imgur.com/eZqecY4.png",
-    },
-    "USP40": {
-        "type": "Pistol",
-        "icon_url": "7FxemzWRtlpAhK9MyKp1Gp/817cc25b6b7c3575dc1ba53a6a8170a9/USP40.png",
-        "imgur_url": "https://i.imgur.com/HF6a0qj.png",
-    },
-    "MK1 9mm": {
-        "type": "Pistol",
-        "icon_url": "3tWoNeF3jQYs3w4EOydQYs/434409c96693df1fd3e969d778e70795/Mk1_9mm_BI.png",
-        "imgur_url": "https://i.imgur.com/ntKax3y.png",
-    },
-    "GSH-18": {
-        "type": "Pistol",
-        "icon_url": "5s5Q33j3MNcXf9lwfxfd7m/4eb3a6af1d431481b6ddcec44fbc7602/GSh-18.png",
-        "imgur_url": "https://i.imgur.com/bAcjOI1.png",
-    },
-    "5.7 USG": {
-        "type": "Pistol",
-        "icon_url": "tkYcSAJSe5yGkeUhzZqBO/e81feb86df4a7eb6951052bec26b6ed7/5.7_USG.png",
-        "imgur_url": "https://i.imgur.com/fP7E1N6.png",
-    },
-    "KERATOS .357": {
-        "type": "Pistol",
-        "icon_url": "15caVAsSCr8Rsb5Hid36uc/59632c4f90727931041ced62a620018b/Keratos_.357.png",
-        "imgur_url": "https://i.imgur.com/wpVBOFb.png",
-    },
-    "P9": {
-        "type": "Pistol",
-        "icon_url": "6Fd1cl17KA0CtgodEiiY6v/d0f145ea72f2aacbd04260ba7d8f1c74/P9.png",
-        "imgur_url": "https://i.imgur.com/Nkuo7a8.png",
-    },
-    "P229": {
-        "type": "Pistol",
-        "icon_url": "76ja0RxqzHW9PpvWgpG7Sk/cb753b50b20fe67deaef54d8b2a46b54/P229.png",
-        "imgur_url": "https://i.imgur.com/jw6hygP.png",
-    },
-    "Q-929": {
-        "type": "Pistol",
-        "icon_url": "2fRVszR5yGDHbV0AL8muso/0838dac90b66aa810daa49d36382fb64/Q-929.png",
-        "imgur_url": "https://i.imgur.com/y4nQMpu.png",
-    },
-    "P12": {
-        "type": "Pistol",
-        "icon_url": "2mpM7rah7rwEW0bViIirUC/ed9caa4db58421519fa4db390b1aa164/P12.png",
-        "imgur_url": "https://i.imgur.com/bh4W2aL.png",
-    },
-    "PMM": {
-        "type": "Pistol",
-        "icon_url": "3y4LIwwm8YNQHAv8oOkWCK/a2375901cee34e68fa39c976d85de8aa/PMM.png",
-        "imgur_url": "https://i.imgur.com/tdz4YMY.png",
-    },
-    "1911 TACOPS": {
-        "type": "Pistol",
-        "icon_url": "189UukZ6fVnvQR6LJtLYry/6eec29603d5b7b0ca8cab6ac0ef083ac/1911_TACOPS.png",
-        "imgur_url": "https://i.imgur.com/QOQ6kpd.png",
-    },
-    "LFP586": {
-        "type": "Pistol",
-        "icon_url": "1zc7UtdBfCZakwbiYqBvSz/1fd3f1584de38ca7c9315d498f094276/LFP586.png",
-        "imgur_url": "https://i.imgur.com/2Qc7IPt.png",
-    },
-    "PRB92": {
-        "type": "Pistol",
-        "icon_url": "dl28J1HsE7mzhj66pmd5D/b8d8fc48d2dde13154047de94abbd8ca/PRB92.png",
-        "imgur_url": "https://i.imgur.com/Gr4wE7G.png",
-    },
-    "Bailiff 410": {
-        "type": "Pistol",
-        "icon_url": "N8FLbo4fsNyBe8msKgRhT/8f403dc0b58087bcafab786dd95ba33f/Bailiff_410.png",
-        "imgur_url": "https://i.imgur.com/Bl7MOeM.png",
-    },
-    "D-50": {
-        "type": "Pistol",
-        "icon_url": "6mMQRDsrComRFa7bC6cNkG/8cd17e545e3d28dcc11a040d000cfa16/D-50.png",
-        "imgur_url": "https://i.imgur.com/XTWaD0k.png",
-    },
-    "P-10C": {
-        "type": "Pistol",
-        "icon_url": "2l4qwB50zSFhFZVYRLNwqg/20df8114f69f96f2adc54779ccc5bbaa/P-10C.png",
-        "imgur_url": "https://i.imgur.com/WZ2m9XI.png",
-    },
-    "P226 MK 25": {
-        "type": "Pistol",
-        "icon_url": "RTQvPQcywlRwUS1FjIKCX/6fc72fee2191c2e723276bc10ae4114e/P226_Mk_25.png",
-        "imgur_url": "https://i.imgur.com/kp8NHDn.png",
-    },
-    "SDP 9mm": {
-        "type": "Pistol",
-        "icon_url": "Tgsdyz3XEqmgUYi9aZZgb/6755f4da7af7a7179ffab92acf8d477e/SDP_9mm.png",
-        "imgur_url": "https://i.imgur.com/J13BH6U.png",
-    },
-    "RG15": {
-        "type": "Pistol",
-        "icon_url": "2LNSsp7B7wUnnPUweir7Jm/9f66d53be7a63a17a55253a0bea6eec1/RG15.png",
-        "imgur_url": "https://i.imgur.com/91Lo842.png",
-    },
-    ".44 Mag Semi-Auto": {
-        "type": "Pistol",
-        "icon_url": "6W3Jz0YcQzbZ6BOPr7VVel/4c67f342964132a652f7d5821e887050/.44_Mag_Semi-Auto.png",
-        "imgur_url": "https://i.imgur.com/4QUGA4Z.png",
-    },
-
-    # Hand Cannon
-    "GONNE-6": {
-        "type": "Hand Cannon",
-        "icon_url": "23AlSVw8MwI1y3ZakEfqgW/c4561ae6e8da8db2627a146b8b55ee6c/GONNE-6_HUD_Icon__1_.png",
-        "imgur_url": "https://i.imgur.com/lc3eGIo.png",
-    },
-
-}
+
+WEAPONS_DICT = {
+
+    # Primary Weapons
+    # AR's
+    "POF9": {
+        "type": "Assault Rifle",
+        "icon_url": "1bhuAox7U6aHN6UriXsAry/3c213cd27f5f64ba01a29b42e5b24ac5/POF9.png",
+        "imgur_url": "https://i.imgur.com/D2FkIjZ.png",
+    },
+    "AK-12": {
+        "type": "Assault Rifle",
+        "icon_url": "7KAZZgnpqD07y47jVVXEuh/e0d7e67101f8f966aa6e1c59e835454f/AK-12.png",
+        "imgur_url": "https://i.imgur.com/XkqUvyS.png",
+    },
+    "SC3000K": {
+        "type": "Assault Rifle",
+        "icon_url": "7x7eDTm2NNpfGiFMrfQqEX/9898e74c780537be3ca6d88db32ea21e/F2000.png",
+        "imgur_url": "https://i.imgur.com/93Vx6y4.png",
+    },
+    "V308": {
+        "type": "Assault Rifle",
+        "icon_url": "5YBZe76NUDO32eF66wW90g/488c315743d59230962a4d67618223d6/V308.png",
+        "imgur_url": "https://i.imgur.com/xoxtQFf.png",
+    },
+    "416-C CARBINE": {
+        "type": "Assault Rifle",
+        "icon_url": "2I86r2a2QD8EHTZVZnxcxy/2913450ba952a16c29fac1f5ce58ba1a/416-C_Carbine.png",
+        "imgur_url": "https://i.imgur.com/18j266k.png",
+    },
+    "556XI": {
+        "type": "Assault Rifle",
+        "icon_url": "2dgpAeAWb3SkZV7rxDbVdQ/fa32323256b7c6f8a1977d3f71e7d4b2/556xi.png",
+        "imgur_url": "https://i.imgur.com/l3Z9O2Q.png",
+    },
+    "M762": {
+        "type": "Assault Rifle",
+        "icon_url": "4oWAgi7tgQP1Tq0HooRtye/9109a74921ee17610d4bd85a61582823/M762.png",
+        "imgur_url": "https://i.imgur.com/bJqHwKt.png",
+    },
+    "TYPE-89": {
+        "type": "Assault Rifle",
+        "icon_url": "7wLf325q9amF8bnVP1QGr0/2faff1a197f90dcded4472852a317d6b/Type-89.png",
+        "imgur_url": "https://i.imgur.com/hGDt4zV.png",
+    },
+    "M4": {
+        "type": "Assault Rifle",
+        "icon_url": "3jhi90ycmuc8mAiuSXFoCi/bcf354459e7becd6ede52ee97917c832/M4.png",
+        "imgur_url": "https://i.imgur.com/lKDElT7.png",
+    },
+    "PARA-308": {
+        "type": "Assault Rifle",
+        "icon_url": "6ub8y2Cs5EYhVPfDWuVVkW/82ca131a41ee4ba2e0b75f2dc52ed9e3/PARA-308.png",
+        "imgur_url": "https://i.imgur.com/246krdt.png",
+    },
+    "SPEAR .308": {
+        "type": "Assault Rifle",
+        "icon_url": "29LjYuJ4s6yA8k9Uv2u28C/89ec812559e7d74b7c269279f4c46d92/Spear_.308.png",
+        "imgur_url": "https://i.imgur.com/PNyKa6N.png",
+    },
+    "AK-74M": {
+        "type": "Assault Rifle",
+        "icon_url": "1j5HiQP8aFphTe65fqDdg0/23eecb5c603c5ba9f59fc6cbc5e4a531/AK-74M.png",
+        "imgur_url": "https://i.imgur.com/bOB4yay.png",
+    },
+    "AR33": {
+        "type": "Assault Rifle",
+        "icon_url": "16U6xEvX8I5xQd9duveBLN/45d22960872cfa3fb6be9eb47fa0be4e/AR33.png",
+        "imgur_url": "https://i.imgur.com/fSUxgbS.png",
+    },
+    "L85A2": {
+        "type": "Assault Rifle",
+        "icon_url": "5vYQpoyk36foDzDq49jBd0/1479a2d7189e545555ceccecf6bd7cc3/L85A2.png",
+        "imgur_url": "https://i.imgur.com/dFG30nS.png",
+    },
+    "G36C": {
+        "type": "Assault Rifle",
+        "icon_url": "2SZoqSXKoNPvZFIJsFsDE5/cb109885bf19c8697abf832f10cfd9a6/G36C.png",
+        "imgur_url": "https://i.imgur.com/YuXb3x9.png",
+    },
+    "COMMANDO 9": {
+        "type": "Assault Rifle",
+        "icon_url": "4P9dpUph5w3MSsLNnW6be/04baba24990fcb75a9c0bcfd01b7d190/Commando_9.png",
+        "imgur_url": "https://i.imgur.com/Jo2DJHb.png",
+    },
+    "AUG A2": {
+        "type": "Assault Rifle",
+        "icon_url": "1eO39zRe8XxJXH1KZiIWhM/02049ced0fbfa630833e8b0d3c03de07/AUG_A2.png",
+        "imgur_url": "https://i.imgur.com/SG0dmYt.png",
+    },
+    "F2": {
+        "type": "Assault Rifle",
+        "icon_url": "5HTvw1cJInVAGxOLXR0war/2f142437f5c0944fdcfcce8a03c37676/F2.png",
+        "imgur_url": "https://i.imgur.com/B9oWguM.png",
+    },
+    "C8-SFW": {
+        "type": "Assault Rifle",
+        "icon_url": "1itXpz2GnvdwwRyhX1SYa2/b58ff71048fa3bb5ed09d5d935dc90f4/C8-SFW.png",
+        "imgur_url": "https://i.imgur.com/kxqQRY5.png",
+    },
+    "R4-C": {
+        "type": "Assault Rifle",
+        "icon_url": "dQbqK9VxczuiscwBDSkT8/777a062f6095dde0371eab5200dcb451/R4-C.png",
+        "imgur_url": "https://i.imgur.com/pBxDdF5.png",
+    },
+    "C7E": {
+        "type": "Assault Rifle",
+        "icon_url": "63vTDjkXeKq7rOoSBhoJD4/08603e6603d564e0fa38af9ec86b7c1f/C7E.png",
+        "imgur_url": "https://i.imgur.com/m0vBz74.png",
+    },
+    "MK17 CQB": {
+        "type": "Assault Rifle",
+        "icon_url": "4LytczDQmu0M63gO2WtCCm/331ef3b1938352ae71d7c0bd23de3596/Mk17_CQB.png",
+        "imgur_url": "https://i.imgur.com/qFieFCz.png",
+    },
+    "552 COMMANDO": {
+        "type": "Assault Rifle",
+        "icon_url": "1LT0N89YaOHvRwn3Pphr8K/02d4a3da9cda132d8201fd134f24fede/552_Commando.png",
+        "imgur_url": "https://i.imgur.com/iyeigKx.png",
+    },
+    "ARX200": {
+        "type": "Assault Rifle",
+        "icon_url": "6VgkPBsr1WApI3rWc9kcM0/b18b8e25f3e951e8e722213f2ee59eb0/ARX200.png",
+        "imgur_url": "https://i.imgur.com/pjJNhg0.png",
+    },
+    "F90": {
+        "type": "Assault Rifle",
+        "icon_url": "62tE3th2ThcGHlrcqWkmEX/d69c9de199542e25fa55f6d293f15671/r6-operator-weapon-ar-f90.png",
+        "imgur_url": "https://i.imgur.com/ltvoR5e.png",
+    },
+
+    # Submachine Guns
+    "P90": {
+        "type": "Submachine Gun",
+        "icon_url": "4nGrNspOvII2oS3lEMkg5x/2398a493c298bc654f97c58767aa40f3/P90.png",
+        "imgur_url": "https://i.imgur.com/JioXAPs.png",
+    },
+    "9mm C1": {
+        "type": "Submachine Gun",
+        "icon_url": "60sbThKtOpNOwKu3OP0oGV/672fd9263f7786402a0d855273473a6f/9mm_C1.png",
+        "imgur_url": "https://i.imgur.com/CSicnOY.png",
+    },
+    "AUG A3": {
+        "type": "Submachine Gun",
+        "icon_url": "3W9XJdMOgpHSw55HfwRSAv/cf8f220678d503e6c3e535c00b2e636a/AUG_A3.png",
+        "imgur_url": "https://i.imgur.com/EwhrsYo.png",
+    },
+    "VECTOR .45 ACP": {
+        "type": "Submachine Gun",
+        "icon_url": "7D1cDf13FqUhoLihzvuPln/068aa7e507155598449c58c0a49a90d6/Vector_.45_ACP.png",
+        "imgur_url": "https://i.imgur.com/nYqNJVY.png",
+    },
+    "M12": {
+        "type": "Submachine Gun",
+        "icon_url": "4FxqA5pa8JY9QQ7FEcjwPw/ffc779fcde5b970e7b95db6653637dab/M12.png",
+        "imgur_url": "https://i.imgur.com/xnjqNAP.png",
+    },
+    "FMG-9": {
+        "type": "Submachine Gun",
+        "icon_url": "0oneJNsBR06QjuowxwtHG/bd3b391c6eec2bd615f2ed83197a13ac/FMG-9.png",
+        "imgur_url": "https://i.imgur.com/Sv4LCCi.png",
+    },
+    "PDW9": {
+        "type": "Submachine Gun",
+        "icon_url": "4yYCuRnduMq35CTHfq6wwU/b7d49cdbcb05917e014c99efeaadd33b/PDW9.png",
+        "imgur_url": "https://i.imgur.com/SfD33PY.png",
+    },
+    "UMP45": {
+        "type": "Submachine Gun",
+        "icon_url": "6X2EZPq2s8UKrP67uxz5FI/f0df4c57d5890c79311e4eb62d4470e7/UMP45.png",
+        "imgur_url": "https://i.imgur.com/DXCAI3x.png",
+    },
+    "SCORPION EVO 3 A1": {
+        "type": "Submachine Gun",
+        "icon_url": "6OdwaLWxcnFvhlVwWbP2Du/4f7e94bdb6d34d5c0aa7b7b147b4092e/Scorpion_EVO_3_A1.png",
+        "imgur_url": "https://i.imgur.com/Xf4RkeF.png",
+    },
+    "P10 RONI": {
+        "type": "Submachine Gun",
+        "icon_url": "7K86OBjL3zmYWt0ZvUcCLj/16a947334e39f27da177d787773593e4/r6-operator-weapon-smg-p10roni.png",
+        "imgur_url": "https://i.imgur.com/am0iQln.png",
+    },
+    "MP5": {
+        "type": "Submachine Gun",
+        "icon_url": "60YbOvSBQt6ZUlu8YDXoZm/51ef3857b2986de700262432e8433714/MP5.png",
+        "imgur_url": "https://i.imgur.com/PUJ9el4.png",
+    },
+    "MPX": {
+        "type": "Submachine Gun",
+        "icon_url": "5HFewpAJ8npDDCKFnEadhL/d398bb477d6b56fe41bfdb5862ed31c0/MPX.png",
+        "imgur_url": "https://i.imgur.com/0lGbMaK.png",
+    },
+    "MP7": {
+        "type": "Submachine Gun",
+        "icon_url": "3a4dgTWGdiJqALhtRp4pKy/f2568d3de3cfe7e4b53179e8653cd2a2/MP7.png",
+        "imgur_url": "https://i.imgur.com/nTLMXY7.png",
+    },
+    "MP5SD": {
+        "type": "Submachine Gun",
+        "icon_url": "5HaMldwFltBwiiyDDfkPpD/6de3aa9aaa17458e7f6186ba59b8deff/MP5SD.png",
+        "imgur_url": "https://i.imgur.com/l5UoMyK.png",
+    },
+    "T-5 SMG": {
+        "type": "Submachine Gun",
+        "icon_url": "1Ne8bvX8BdCALevWKMllQN/4baa3e79d323de134dd182e0272b9c3b/T-5_SMG.png",
+        "imgur_url": "https://i.imgur.com/aJD4n8e.png",
+    },
+    "K1A": {
+        "type": "Submachine Gun",
+        "icon_url": "5mUa2p8WXbiyD71qUI8sGk/ed753b6f0ae30ab5737486dfcf32ee9f/K1A.png",
+        "imgur_url": "https://i.imgur.com/ASxXNFF.png",
+    },
+    "Mx4 Storm": {
+        "type": "Submachine Gun",
+        "icon_url": "4qRh1frGkQZxNyeKA4D6n1/20f89cd1d9953f06207b7340ea77fb17/Mx4_Storm.png",
+        "imgur_url": "https://i.imgur.com/0KjOTla.png",
+    },
+    "UZK50GI": {
+        "type": "Submachine Gun",
+        "icon_url": "5WMIsPUWTXprZnAwctPsTt/f1c652b681e7e9ba6ba66bcd29e12a76/uzk50gi.png",
+        "imgur_url": "https://i.imgur.com/EjnVX3B.png",
+    },
+    "9x19VSN": {
+        "type": "Submachine Gun",
+        "icon_url": "42gH96xTTYaTZsfXI3c0wL/a7edbf11af97091ee884b68e59fe6a4f/9x19VSN.png",
+        "imgur_url": "https://i.imgur.com/YM28ZXk.png",
+    },
+    "MP5K": {
+        "type": "Submachine Gun",
+        "icon_url": "1pk8nOI7ybQjYOSI4fuzOm/fcd78df0f729be545e75c09aae85c360/MP5K.png",
+        "imgur_url": "https://i.imgur.com/cJnZz6l.png",
+    },
+
+    # Marksman Rifles
+    "SR-25": {
+        "type": "Marksman Rifle",
+        "icon_url": "3H3sICdj6BK8LhtQPRd2aJ/26826ebba73e0e5fd503256d069f3256/SR-25.png",
+        "imgur_url": "https://i.imgur.com/GAwCFpP.png",
+    },
+    "AR-15.50": {
+        "type": "Marksman Rifle",
+        "icon_url": "4lGGEGZLkbldz114Wl5hCo/78a04c46654f80fae03e730bd79f3563/AR-15.50.png",
+        "imgur_url": "https://i.imgur.com/k4RWCgE.png",
+    },
+    "417": {
+        "type": "Marksman Rifle",
+        "icon_url": "5djkS4YtAtOF0vBmg0T60x/ea2b1ff7e5367e66c99bc7ad7e95bfe3/417.png",
+        "imgur_url": "https://i.imgur.com/XM1aYZ0.png",
+    },
+    "Mk 14 EBR": {
+        "type": "Marksman Rifle",
+        "icon_url": "6KIMqp5dA95z1RI3PrG9jv/eb939638169811a3fa858a44e6e5d97e/Mk_14_EBR.png",
+        "imgur_url": "https://i.imgur.com/a7tnoMB.png",
+    },
+    "OTs-03": {
+        "type": "Marksman Rifle",
+        "icon_url": "4fXznwDtLt61VCF8QIF4N3/34e2e6d6c33d4c504c945bdd13c322f6/OTs-03.png",
+        "imgur_url": "https://i.imgur.com/SvaWAHY.png",
+    },
+    "CSRX 300": {
+        "type": "Marksman Rifle",
+        "icon_url": "7tUB9ZNXJhdN6ejAkCEeFQ/99691bcc19f641cf872925905d08a539/CSRX_300.png",
+        "imgur_url": "https://i.imgur.com/QIpmJkI.png",
+    },
+    "CAMRS": {
+        "type": "Marksman Rifle",
+        "icon_url": "4dBzqVVmnpv1DZi91LAnEN/e374b4ea289fc992280b943cdbb94d60/CAMRS.png",
+        "imgur_url": "https://i.imgur.com/jRgdhPK.png",
+    },
+
+    # Shotguns
+    "ACS12": {
+        "type": "Shotgun",
+        "icon_url": "13z63kT1NLzn1U99o7WC4T/8655d3200f24b87246c36f2622603457/ACS12_PB.png",
+        "imgur_url": "https://i.imgur.com/oWkeNV1.png",
+    },
+    "M590A1": {
+        "type": "Shotgun",
+        "icon_url": "2zRHmgqENNiZqXQxC9Rsbj/e6542407c642f9b7c5a4546afb6db30a/M590A1.png",
+        "imgur_url": "https://i.imgur.com/1hKRvhC.png",
+    },
+    "M870": {
+        "type": "Shotgun",
+        "icon_url": "2rkU6g4Rlg0e0U4rczWGTV/a51589a54c43f476d8eb984c0ea881e9/M870.png",
+        "imgur_url": "https://i.imgur.com/2DulKY2.png",
+    },
+    "TCSG12": {
+        "type": "Shotgun",
+        "icon_url": "2NDbY7BTBJ9R09LUilTlRf/3728337cd3ba14ed6ab9de0c22e879af/TCSG12.png",
+        "imgur_url": "https://i.imgur.com/jxNiaOx.png",
+    },
+    # Yep, twice, because Ubi doesn't know how their own guns are named :)
+    "FO-12": {
+        "type": "Shotgun",
+        "icon_url": "4TDWnhbgvLkc6HBWDJp2ST/f50cbd83d6d295ab59f17f7e21d713bc/FO-12.png",
+        "imgur_url": "https://i.imgur.com/9mWXMtL.png",
+    },
+    "F0-12": {
+        "type": "Shotgun",
+        "icon_url": "4TDWnhbgvLkc6HBWDJp2ST/f50cbd83d6d295ab59f17f7e21d713bc/FO-12.png",
+        "imgur_url": "https://i.imgur.com/9mWXMtL.png",
+    },
+    "SIX12": {
+        "type": "Shotgun",
+        "icon_url": "2v6MwsHwjOZ5Muid53lyfN/e5f1c4997db93abfe3ac356fce23376c/SIX12.png",
+        "imgur_url": "https://i.imgur.com/XMdA44M.png",
+    },
+    "SIX12 SD": {
+        "type": "Shotgun",
+        "icon_url": "1GTua079Xbtkpjhx96sRsW/079ed1a71a0d12b5e48e1b0d40b87110/SIX12_SD.png",
+        "imgur_url": "https://i.imgur.com/yco3bh7.png",
+    },
+    "M1014": {
+        "type": "Shotgun",
+        "icon_url": "2pUiVbwNnQnDTesmWXktqW/f27c1fab9a354bb89cbe309a688f5e02/M1014.png",
+        "imgur_url": "https://i.imgur.com/QoKV2HB.png",
+    },
+    "SG-CQB": {
+        "type": "Shotgun",
+        "icon_url": "5JoL3b36Fsztt9Q2XYmrbJ/dacec96948d3f8fe92914a69b9aac593/SG-CQB.png",
+        "imgur_url": "https://i.imgur.com/878GOhH.png",
+    },
+    "SPAS-15": {
+        "type": "Shotgun",
+        "icon_url": "CyofBgipHq4RTafvPFWd4/bc3d0ecc871b70e57735855f852efacf/SPAS-15.png",
+        "imgur_url": "https://i.imgur.com/ptUqPpu.png",
+    },
+    "SPAS-12": {
+        "type": "Shotgun",
+        "icon_url": "7Hp6Fbss6uI59OT4nZNB6e/a4d09954803cb2580353cfa03e8c778b/SPAS-12.png",
+        "imgur_url": "https://i.imgur.com/wMvRHWE.png",
+    },
+    "SASG-12": {
+        "type": "Shotgun",
+        "icon_url": "2Q6mL4CbifmIgifV2yV3Hi/2bb2b323f055b03a2c1ba516c262c24e/SASG-12.png",
+        "imgur_url": "https://i.imgur.com/TASWBEp.png",
+    },
+    "Supernova": {
+        "type": "Shotgun",
+        "icon_url": "2tpjCRFLcc3hogjJGbKDsi/5ad0ab63b7245022aca5c1c1fb42d473/SuperNova.png",
+        "imgur_url": "https://i.imgur.com/gshdPvF.png",
+    },
+    "ITA12L": {
+        "type": "Shotgun",
+        "icon_url": "4Y6ziRzm9RiPii83fm8BV1/1f472744d2c2dec8d9206f4d8733d92c/ITA12L.png",
+        "imgur_url": "https://i.imgur.com/ldY0IlZ.png",
+    },
+    "BOSG.12.2": {
+        "type": "Shotgun",
+        "icon_url": "2ZjVndetsX8WEn5ZfyUQa0/e3a781be7eab22876d25f748e8fd0f5a/BOSG.12.2.png",
+        "imgur_url": "https://i.imgur.com/90I2Sb8.png",
+    },
+
+    # Light Machine Guns
+    "G8A1": {
+        "type": "Light Machine Gun",
+        "icon_url": "4TIb7oeJesaROOOfTlCBaZ/ffd6a802f9a779a0d39b2122c49b3254/G8A1.png",
+        "imgur_url": "https://i.imgur.com/Wy6HdZW.png",
+    },
+    "LMG-E": {
+        "type": "Light Machine Gun",
+        "icon_url": "7JVJIew6t3iKwgByvrFXyi/7ba44dfda28b525506633e453104a604/LMG-E.png",
+        "imgur_url": "https://i.imgur.com/UWXTqIL.png",
+    },
+    "M249 SAW": {
+        "type": "Light Machine Gun",
+        "icon_url": "3p0oG7GsLIoHaRullf7xsF/e2a9e135af63e8897355023cd34538c4/M249_SAW.png",
+        "imgur_url": "https://i.imgur.com/dWLYeNw.png",
+    },
+    "M249": {
+        "type": "Light Machine Gun",
+        "icon_url": "7z8UpVPS3P14OC1oL9dDIn/39c0c657f154218003fd4b2a9250b92f/M249.png",
+        "imgur_url": "https://i.imgur.com/gQOhuzN.png",
+    },
+    "ALDA 5.56": {
+        "type": "Light Machine Gun",
+        "icon_url": "39yB6TFl9ph6Rb4bDV4lqK/7f9b3abf8dff19bacc026a7212849ca4/ALDA_5.56.png",
+        "imgur_url": "https://i.imgur.com/uNiNSiM.png",
+    },
+    "6P41": {
+        "type": "Light Machine Gun",
+        "icon_url": "1wxS2HOCvoPAfnJEDFWjfw/7feddb98582ec37b500243d3f3e19eca/6P41.png",
+        "imgur_url": "https://i.imgur.com/nv4v9Q4.png",
+    },
+    "DP28": {
+        "type": "Light Machine Gun",
+        "icon_url": "7LoT7yAe0LK7bDOeq6MZZM/33995bc704667674af1b73fe962d4c7c/Primary_gun_DP27.png",
+        "imgur_url": "https://i.imgur.com/EuXUXJt.png",
+    },
+    "DP27": {
+        "type": "Light Machine Gun",
+        "icon_url": "7LoT7yAe0LK7bDOeq6MZZM/33995bc704667674af1b73fe962d4c7c/Primary_gun_DP27.png",
+        "imgur_url": "https://i.imgur.com/EuXUXJt.png",
+    },
+    "T-95 LSW": {
+        "type": "Light Machine Gun",
+        "icon_url": "23HCxaNTRUHBlFAvCTMZQm/fe319cc164fac034a29e9b114ae7d5cb/T-95_LSW.png",
+        "imgur_url": "https://i.imgur.com/6QCVGPg.png",
+    },
+
+    # Gadget
+    "CCE SHIELD": {
+        "type": "Gadget",
+        "icon_url": "5mmGgrYdJJHw2moBIEW9An/64e9727d959d7afdbb4fb06e2f75574a/CCE_Shield.png",
+        "imgur_url": "https://i.imgur.com/3CmDzwG.png",
+    },
+    # Shield
+    "Le Roc": {
+        "type": "Shield",
+        "icon_url": "1bmXJOakdA6SOrGxBKA70T/1e489e366d6db287f475963df2040d3d/Extendable-Shield.png",
+        "imgur_url": "https://i.imgur.com/pTB9tOm.png",
+    },
+    # Ops ability
+    "FLASH SHIELD": {
+        "type": "Ops ability",
+        "icon_url": "7qmWjGZayvK4t6E80Gvu7g/8b789d6d639744dce100c2cfb9709e6a/G52-Tactical_Shield.png",
+        "imgur_url": "https://i.imgur.com/OFeah3y.png",
+    },
+    # None
+    "None": {
+        "type": "None",
+        "icon_url": "yeah_lmao.png",
+        "imgur_url": "https://i.imgur.com/yeah_lmao.png",
+    },
+
+    # Secondary Weapons
+    # Shotguns
+    "SUPER SHORTY": {
+        "type": "Shotgun",
+        "icon_url": "7Dq8LDmIxAveRqXM17orUW/cbd96b47cd8ca74a7827b16ef73fe7cf/r6-operator-weapon-sa-supershorty.png",
+        "imgur_url": "https://i.imgur.com/ceMDeDV.png",
+    },
+    "ITA12S": {
+        "type": "Shotgun",
+        "icon_url": "5G4DroaSdqHzJWCe7qqbHZ/5dd2e03f853182c78a1e7fcbc642f0cf/ITA12S.png",
+        "imgur_url": "https://i.imgur.com/gKRXgpZ.png",
+    },
+
+    # Machine Pistols
+    "SMG-11": {
+        "type": "Machine Pistol",
+        "icon_url": "3WExw7Kepz9uAiWAbWW457/875fc631a3cf9fcc2849d9db2989cbcd/SMG-11.png",
+        "imgur_url": "https://i.imgur.com/HVuD3gD.png",
+    },
+    "SMG-12": {
+        "type": "Machine Pistol",
+        "icon_url": "EwJgB7KdgOb6dDm7ro33u/b73f0890f992c1a365210f08efcc6db5/SMG-12.png",
+        "imgur_url": "https://i.imgur.com/1fC7KAS.png",
+    },
+    "BEARING 9": {
+        "type": "Machine Pistol",
+        "icon_url": "4mdftEOh5Vu9KhhpgKLKrT/abedcc75868774018295ec2a08a7b3de/Bearing_9.png",
+        "imgur_url": "https://i.imgur.com/wT1qVsk.png",
+    },
+    "C75 Auto": {
+        "type": "Machine Pistol",
+        "icon_url": "3wUuefwPjU705mZkTdJ9UH/8ccb11884cfa34c176ac5500af139177/C75_Auto.png",
+        "imgur_url": "https://i.imgur.com/VA1Y1FG.png",
+    },
+    "SPSMG9": {
+        "type": "Machine Pistol",
+        "icon_url": "5EtwSgylXckBNg4n6gDR9J/bc6fc6c5c12ae11da59aee95828ebd76/SPSMG9.png",
+        "imgur_url": "https://i.imgur.com/owfOEEn.png",
+    },
+
+    # Pistols
+    "M45 MEUSOC": {
+        "type": "Pistol",
+        "icon_url": "3u5cecgWYl3WuJK50mKEGd/a4a0eb15c710edfc0d29e98c2ee7ea33/M45_MEUSOC.png",
+        "imgur_url": "https://i.imgur.com/eZqecY4.png",
+    },
+    "USP40": {
+        "type": "Pistol",
+        "icon_url": "7FxemzWRtlpAhK9MyKp1Gp/817cc25b6b7c3575dc1ba53a6a8170a9/USP40.png",
+        "imgur_url": "https://i.imgur.com/HF6a0qj.png",
+    },
+    "MK1 9mm": {
+        "type": "Pistol",
+        "icon_url": "3tWoNeF3jQYs3w4EOydQYs/434409c96693df1fd3e969d778e70795/Mk1_9mm_BI.png",
+        "imgur_url": "https://i.imgur.com/ntKax3y.png",
+    },
+    "GSH-18": {
+        "type": "Pistol",
+        "icon_url": "5s5Q33j3MNcXf9lwfxfd7m/4eb3a6af1d431481b6ddcec44fbc7602/GSh-18.png",
+        "imgur_url": "https://i.imgur.com/bAcjOI1.png",
+    },
+    "5.7 USG": {
+        "type": "Pistol",
+        "icon_url": "tkYcSAJSe5yGkeUhzZqBO/e81feb86df4a7eb6951052bec26b6ed7/5.7_USG.png",
+        "imgur_url": "https://i.imgur.com/fP7E1N6.png",
+    },
+    "KERATOS .357": {
+        "type": "Pistol",
+        "icon_url": "15caVAsSCr8Rsb5Hid36uc/59632c4f90727931041ced62a620018b/Keratos_.357.png",
+        "imgur_url": "https://i.imgur.com/wpVBOFb.png",
+    },
+    "P9": {
+        "type": "Pistol",
+        "icon_url": "6Fd1cl17KA0CtgodEiiY6v/d0f145ea72f2aacbd04260ba7d8f1c74/P9.png",
+        "imgur_url": "https://i.imgur.com/Nkuo7a8.png",
+    },
+    "P229": {
+        "type": "Pistol",
+        "icon_url": "76ja0RxqzHW9PpvWgpG7Sk/cb753b50b20fe67deaef54d8b2a46b54/P229.png",
+        "imgur_url": "https://i.imgur.com/jw6hygP.png",
+    },
+    "Q-929": {
+        "type": "Pistol",
+        "icon_url": "2fRVszR5yGDHbV0AL8muso/0838dac90b66aa810daa49d36382fb64/Q-929.png",
+        "imgur_url": "https://i.imgur.com/y4nQMpu.png",
+    },
+    "P12": {
+        "type": "Pistol",
+        "icon_url": "2mpM7rah7rwEW0bViIirUC/ed9caa4db58421519fa4db390b1aa164/P12.png",
+        "imgur_url": "https://i.imgur.com/bh4W2aL.png",
+    },
+    "PMM": {
+        "type": "Pistol",
+        "icon_url": "3y4LIwwm8YNQHAv8oOkWCK/a2375901cee34e68fa39c976d85de8aa/PMM.png",
+        "imgur_url": "https://i.imgur.com/tdz4YMY.png",
+    },
+    "1911 TACOPS": {
+        "type": "Pistol",
+        "icon_url": "189UukZ6fVnvQR6LJtLYry/6eec29603d5b7b0ca8cab6ac0ef083ac/1911_TACOPS.png",
+        "imgur_url": "https://i.imgur.com/QOQ6kpd.png",
+    },
+    "LFP586": {
+        "type": "Pistol",
+        "icon_url": "1zc7UtdBfCZakwbiYqBvSz/1fd3f1584de38ca7c9315d498f094276/LFP586.png",
+        "imgur_url": "https://i.imgur.com/2Qc7IPt.png",
+    },
+    "PRB92": {
+        "type": "Pistol",
+        "icon_url": "dl28J1HsE7mzhj66pmd5D/b8d8fc48d2dde13154047de94abbd8ca/PRB92.png",
+        "imgur_url": "https://i.imgur.com/Gr4wE7G.png",
+    },
+    "Bailiff 410": {
+        "type": "Pistol",
+        "icon_url": "N8FLbo4fsNyBe8msKgRhT/8f403dc0b58087bcafab786dd95ba33f/Bailiff_410.png",
+        "imgur_url": "https://i.imgur.com/Bl7MOeM.png",
+    },
+    "D-50": {
+        "type": "Pistol",
+        "icon_url": "6mMQRDsrComRFa7bC6cNkG/8cd17e545e3d28dcc11a040d000cfa16/D-50.png",
+        "imgur_url": "https://i.imgur.com/XTWaD0k.png",
+    },
+    "P-10C": {
+        "type": "Pistol",
+        "icon_url": "2l4qwB50zSFhFZVYRLNwqg/20df8114f69f96f2adc54779ccc5bbaa/P-10C.png",
+        "imgur_url": "https://i.imgur.com/WZ2m9XI.png",
+    },
+    "P226 MK 25": {
+        "type": "Pistol",
+        "icon_url": "RTQvPQcywlRwUS1FjIKCX/6fc72fee2191c2e723276bc10ae4114e/P226_Mk_25.png",
+        "imgur_url": "https://i.imgur.com/kp8NHDn.png",
+    },
+    "SDP 9mm": {
+        "type": "Pistol",
+        "icon_url": "Tgsdyz3XEqmgUYi9aZZgb/6755f4da7af7a7179ffab92acf8d477e/SDP_9mm.png",
+        "imgur_url": "https://i.imgur.com/J13BH6U.png",
+    },
+    "RG15": {
+        "type": "Pistol",
+        "icon_url": "2LNSsp7B7wUnnPUweir7Jm/9f66d53be7a63a17a55253a0bea6eec1/RG15.png",
+        "imgur_url": "https://i.imgur.com/91Lo842.png",
+    },
+    ".44 Mag Semi-Auto": {
+        "type": "Pistol",
+        "icon_url": "6W3Jz0YcQzbZ6BOPr7VVel/4c67f342964132a652f7d5821e887050/.44_Mag_Semi-Auto.png",
+        "imgur_url": "https://i.imgur.com/4QUGA4Z.png",
+    },
+
+    # Hand Cannon
+    "GONNE-6": {
+        "type": "Hand Cannon",
+        "icon_url": "23AlSVw8MwI1y3ZakEfqgW/c4561ae6e8da8db2627a146b8b55ee6c/GONNE-6_HUD_Icon__1_.png",
+        "imgur_url": "https://i.imgur.com/lc3eGIo.png",
+    },
+
+}
```

### Comparing `siegeapi-6.0.1/siegeapi/default_stats.py` & `siegeapi-6.1.0/siegeapi/default_stats.py`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from __future__ import annotations
-
-
-class DefaultStats:
-    def __init__(self, data):
-        self.matches_played: int = data.get("matchesPlayed", 0)
-        self.rounds_played: int = data.get("roundsPlayed", 0)
-        self.minutes_played: int = data.get("minutesPlayed", 0)
-        self.matches_won: int = data.get("matchesWon", 0)
-        self.matches_lost: int = data.get("matchesLost", 0)
-        self.rounds_won: int = data.get("roundsWon", 0)
-        self.rounds_lost: int = data.get("roundsLost", 0)
-        self.kills: int = data.get("kills", 0)
-        self.assists: int = data.get("assists", 0)
-        self.death: int = data.get("death", 0)
-        self.headshots: int = data.get("headshots", 0)
-        self.melee_kills: int = data.get("meleeKills", 0)
-        self.team_kills: int = data.get("teamKills", 0)
-        self.opening_kills: int = data.get("openingKills", 0)
-        self.opening_deaths: int = data.get("openingDeaths", 0)
-        self.trades: int = data.get("trades", 0)
-        self.opening_kill_trades: int = data.get("openingKillTrades", 0)
-        self.opening_death_trades: int = data.get("openingDeathTrades", 0)
-        self.revives: int = data.get("revives", 0)
-        self.distance_travelled: int = data.get("distanceTravelled", 0)
-        self.win_loss_ratio: float = data.get("winLossRatio", 0)
-        self.kill_death_ratio: float = round((data.get("killDeathRatio", {}).get("value", 0) * 100), 2)
-        self.headshot_accuracy: float = round((data.get("headshotAccuracy", {}).get("value", 0) * 100), 2)
-        self.kills_per_round: float = round((data.get("killsPerRound", {}).get("value", 0) * 100), 2)
-        self.rounds_with_a_kill: float = round((data.get("roundsWithAKill", {}).get("value", 0) * 100), 2)
-        self.rounds_with_multi_kill: float = round((data.get("roundsWithMultiKill", {}).get("value", 0) * 100), 2)
-        self.rounds_with_opening_kill: float = round((data.get("roundsWithOpeningKill", {}).get("value", 0) * 100), 2)
-        self.rounds_with_opening_death: float = round((data.get("roundsWithOpeningDeath", {}).get("value", 0) * 100), 2)
-        self.rounds_with_kost: float = round((data.get("roundsWithKOST", {}).get("value", 0) * 100), 2)
-        self.rounds_survived: float = round((data.get("roundsSurvived", {}).get("value", 0) * 100), 2)
-        self.rounds_with_an_ace: float = round((data.get("roundsWithAnAce", {}).get("value", 0) * 100), 2)
-        self.rounds_with_clutch: float = round((data.get("roundsWithClutch", {}).get("value", 0) * 100), 2)
-        self.time_alive_per_match: float = data.get("timeAlivePerMatch", 0)
-        self.time_dead_per_match: float = data.get("timeDeadPerMatch", 0)
-        self.distance_per_round: float = data.get("distancePerRound", 0)
-
-    def __repr__(self) -> str:
-        return str(vars(self))
+from __future__ import annotations
+
+
+class DefaultStats:
+    def __init__(self, data):
+        self.matches_played: int = data.get("matchesPlayed", 0)
+        self.rounds_played: int = data.get("roundsPlayed", 0)
+        self.minutes_played: int = data.get("minutesPlayed", 0)
+        self.matches_won: int = data.get("matchesWon", 0)
+        self.matches_lost: int = data.get("matchesLost", 0)
+        self.rounds_won: int = data.get("roundsWon", 0)
+        self.rounds_lost: int = data.get("roundsLost", 0)
+        self.kills: int = data.get("kills", 0)
+        self.assists: int = data.get("assists", 0)
+        self.death: int = data.get("death", 0)
+        self.headshots: int = data.get("headshots", 0)
+        self.melee_kills: int = data.get("meleeKills", 0)
+        self.team_kills: int = data.get("teamKills", 0)
+        self.opening_kills: int = data.get("openingKills", 0)
+        self.opening_deaths: int = data.get("openingDeaths", 0)
+        self.trades: int = data.get("trades", 0)
+        self.opening_kill_trades: int = data.get("openingKillTrades", 0)
+        self.opening_death_trades: int = data.get("openingDeathTrades", 0)
+        self.revives: int = data.get("revives", 0)
+        self.distance_travelled: int = data.get("distanceTravelled", 0)
+        self.win_loss_ratio: float = data.get("winLossRatio", 0)
+        self.kill_death_ratio: float = round((data.get("killDeathRatio", {}).get("value", 0) * 100), 2)
+        self.headshot_accuracy: float = round((data.get("headshotAccuracy", {}).get("value", 0) * 100), 2)
+        self.kills_per_round: float = round((data.get("killsPerRound", {}).get("value", 0) * 100), 2)
+        self.rounds_with_a_kill: float = round((data.get("roundsWithAKill", {}).get("value", 0) * 100), 2)
+        self.rounds_with_multi_kill: float = round((data.get("roundsWithMultiKill", {}).get("value", 0) * 100), 2)
+        self.rounds_with_opening_kill: float = round((data.get("roundsWithOpeningKill", {}).get("value", 0) * 100), 2)
+        self.rounds_with_opening_death: float = round((data.get("roundsWithOpeningDeath", {}).get("value", 0) * 100), 2)
+        self.rounds_with_kost: float = round((data.get("roundsWithKOST", {}).get("value", 0) * 100), 2)
+        self.rounds_survived: float = round((data.get("roundsSurvived", {}).get("value", 0) * 100), 2)
+        self.rounds_with_an_ace: float = round((data.get("roundsWithAnAce", {}).get("value", 0) * 100), 2)
+        self.rounds_with_clutch: float = round((data.get("roundsWithClutch", {}).get("value", 0) * 100), 2)
+        self.time_alive_per_match: float = data.get("timeAlivePerMatch", 0)
+        self.time_dead_per_match: float = data.get("timeDeadPerMatch", 0)
+        self.distance_per_round: float = data.get("distancePerRound", 0)
+
+    def __repr__(self) -> str:
+        return str(vars(self))
```

### Comparing `siegeapi-6.0.1/siegeapi/operators.py` & `siegeapi-6.1.0/siegeapi/operators.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-from __future__ import annotations
-
-from .constants import operator_dict
-from .default_stats import DefaultStats
-
-
-class Operator(DefaultStats):
-    def __init__(self, data: dict, op_about: bool):
-        super().__init__(data)
-
-        self.name: str = data.get("statsDetail")
-        if self.name == "":
-            self.name = "Unknown Operator"
-
-        if op_about:
-            self.icon_url: str = self._get_from_operators_const("icon_url")
-            self.real_name: str = self._get_from_operators_const("realname")
-            self.birth_place: str = self._get_from_operators_const("birthplace")
-            self.date_of_birth: str = self._get_from_operators_const("date_of_birth")
-            self.age: int = self._get_from_operators_const("age")
-            self.roles: list[str] = self._get_from_operators_const("roles")
-            self.unit: str = self._get_from_operators_const("unit")
-            self.country_code: str = self._get_from_operators_const("country_code")
-            self.season_introduced: str = self._get_from_operators_const("season_introduced")
-
-    def _get_from_operators_const(self, what: str) -> str | int | list:
-        return operator_dict.get(self.name.lower(), {}).get(what, "Missing Data")
-
-
-class OperatorsGameMode:
-    def __init__(self, data: dict, op_about: bool):
-        self.attacker: list = [Operator(operator, op_about) for operator in data.get("teamRoles", {}).get("Attacker", {})]
-        self.defender: list = [Operator(operator, op_about) for operator in data.get("teamRoles", {}).get("Defender", {})]
-
-    def __repr__(self) -> str:
-        return str(vars(self))
-
-
-class Operators:
-    def __init__(self, data: dict, op_about: bool):
-        self.all: OperatorsGameMode = OperatorsGameMode(data.get("platforms").get("PC").get("gameModes").get("all", {}), op_about)
-        self.casual: OperatorsGameMode = OperatorsGameMode(data.get("platforms").get("PC").get("gameModes").get("casual", {}), op_about)
-        self.ranked: OperatorsGameMode = OperatorsGameMode(data.get("platforms").get("PC").get("gameModes").get("ranked", {}), op_about)
-        self.unranked: OperatorsGameMode = OperatorsGameMode(data.get("platforms").get("PC").get("gameModes").get("unranked", {}), op_about)
-        self.newcomer: OperatorsGameMode = OperatorsGameMode(data.get("platforms").get("PC").get("gameModes").get("newcomer", {}), op_about)
-        self._start_date: str = str(data.get("startDate", ""))
-        self._end_date: str = str(data.get("endDate", ""))
-
-    def get_timespan_dates(self) -> dict[str: str]:
-        return {"start_date": self._start_date, "end_date": self._end_date}
-
-    def __repr__(self) -> str:
-        return str(vars(self))
+from __future__ import annotations
+
+from .constants import operator_dict
+from .default_stats import DefaultStats
+
+
+class Operator(DefaultStats):
+    def __init__(self, data: dict, op_about: bool):
+        super().__init__(data)
+
+        self.name: str = data.get("statsDetail")
+        if self.name == "":
+            self.name = "Unknown Operator"
+
+        if op_about:
+            self.icon_url: str = self._get_from_operators_const("icon_url")
+            self.real_name: str = self._get_from_operators_const("realname")
+            self.birth_place: str = self._get_from_operators_const("birthplace")
+            self.date_of_birth: str = self._get_from_operators_const("date_of_birth")
+            self.age: int = self._get_from_operators_const("age")
+            self.roles: list[str] = self._get_from_operators_const("roles")
+            self.unit: str = self._get_from_operators_const("unit")
+            self.country_code: str = self._get_from_operators_const("country_code")
+            self.season_introduced: str = self._get_from_operators_const("season_introduced")
+
+    def _get_from_operators_const(self, what: str) -> str | int | list:
+        return operator_dict.get(self.name.lower(), {}).get(what, "Missing Data")
+
+
+class OperatorsGameMode:
+    def __init__(self, data: dict, op_about: bool):
+        self.attacker: list = [Operator(operator, op_about) for operator in data.get("teamRoles", {}).get("Attacker", {})]
+        self.defender: list = [Operator(operator, op_about) for operator in data.get("teamRoles", {}).get("Defender", {})]
+
+    def __repr__(self) -> str:
+        return str(vars(self))
+
+
+class Operators:
+    def __init__(self, data: dict, op_about: bool):
+        self.all: OperatorsGameMode = OperatorsGameMode(data.get("platforms").get("PC").get("gameModes").get("all", {}), op_about)
+        self.casual: OperatorsGameMode = OperatorsGameMode(data.get("platforms").get("PC").get("gameModes").get("casual", {}), op_about)
+        self.ranked: OperatorsGameMode = OperatorsGameMode(data.get("platforms").get("PC").get("gameModes").get("ranked", {}), op_about)
+        self.unranked: OperatorsGameMode = OperatorsGameMode(data.get("platforms").get("PC").get("gameModes").get("unranked", {}), op_about)
+        self.newcomer: OperatorsGameMode = OperatorsGameMode(data.get("platforms").get("PC").get("gameModes").get("newcomer", {}), op_about)
+        self._start_date: str = str(data.get("startDate", ""))
+        self._end_date: str = str(data.get("endDate", ""))
+
+    def get_timespan_dates(self) -> dict[str: str]:
+        return {"start_date": self._start_date, "end_date": self._end_date}
+
+    def __repr__(self) -> str:
+        return str(vars(self))
```

### Comparing `siegeapi-6.0.1/siegeapi/player.py` & `siegeapi-6.1.0/siegeapi/player.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,188 +1,196 @@
-from __future__ import annotations
-
-from .utils import season_id_to_code, season_code_to_id, get_total_xp, get_xp_to_next_lvl
-from .rank_profile import FullProfile
-from .url_builder import UrlBuilder
-from .operators import Operators
-from .summaries import Summary
-from .weapons import Weapons
-from .trends import Trends
-from .ranks import Rank
-from .maps import Maps
-
-import aiohttp
-import re
-
-platform_url_names = {"uplay": "OSBOR_PC_LNCH_A", "psn": "OSBOR_PS4_LNCH_A", "xbl": "OSBOR_XBOXONE_LNCH_A", "xplay": "OSBOR_XPLAY_LNCH_A"}
-date_pattern = re.compile(r"^((2\d)\d{2})(0[1-9]|1[012])([012]\d|3[01])$")
-
-
-class Player:
-    def __init__(self, auth: aiohttp.ClientSession(), data: dict):
-
-        self.id: str = data.get("profileId")
-
-        self._auth: aiohttp.ClientSession() = auth
-        self._platform: str = data.get("platformType")
-        self._platform_url: str = platform_url_names[self._platform]
-        self._spaceid: str = self._auth.spaceids[self._platform]
-        self._platform_group: str = "PC" if self._platform == "uplay" else "Console"
-        self._url_builder: UrlBuilder = UrlBuilder(self._spaceid, self._platform_url, self.id, self._platform_group)
-
-        self.profile_pic_url_146: str = f"https://ubisoft-avatars.akamaized.net/{self.id}/default_146_146.png"
-        self.profile_pic_url_256: str = f"https://ubisoft-avatars.akamaized.net/{self.id}/default_256_256.png"
-        self.profile_pic_url_500: str = f"https://ubisoft-avatars.akamaized.net/{self.id}/default_tall.png"
-        self.profile_pic_url: str = self.profile_pic_url_256
-
-        self.name: str = data.get("nameOnPlatform")
-        self.level: int = 0
-        self.alpha_pack: float = 0
-        self.xp: int = 0
-        self.total_xp: int = 0
-        self.xp_to_level_up: int = 0
-
-        self.total_time_played: int = 0
-        self.pvp_time_played: int = 0
-        self.pve_time_played: int = 0
-
-        self.rank_skill_records: dict[int: dict[str: Rank | None]] | dict = {}
-        self.casual_skill_records: dict[int: dict[str: Rank | None]] | dict = {}
-
-        self.ranked_summary: dict = {}
-        self.casual_summary: dict = {}
-        self.unranked_summary: dict = {}
-        self.all_summary: dict = {}
-
-        self.unranked_profile: FullProfile | None = None
-        self.ranked_profile: FullProfile | None = None
-        self.casual_profile: FullProfile | None = None
-        self.warmup_profile: FullProfile | None = None
-        self.event_profile: FullProfile | None = None
-
-        self.weapons: Weapons | None = None
-        self.trends: Trends | None = None
-        self.operators: Operators | None = None
-        self.maps: Maps | None = None
-
-    def set_timespan_dates(self, start_date: str, end_date: str) -> None:
-        """YYYYMMDD"""
-        if not date_pattern.match(start_date):
-            raise ValueError(f"Date for start_date '{start_date}' is invalid. The date format is 'YYYYMMDD'.")
-        if not date_pattern.match(end_date):
-            raise ValueError(f"Date for end_date '{end_date}' is invalid. The date format is 'YYYYMMDD'.")
-        else:
-            self._url_builder.set_timespan_dates(start_date, end_date)
-
-    async def load_progress(self) -> tuple[int, int]:
-        data = await self._auth.get(self._url_builder.xp_lvl(), new=True)
-        self.level = int(data.get("level", 0))
-        self.xp = int(data.get("xp", 0))
-        self.total_xp: int = get_total_xp(self.level, self.xp)
-        self.xp_to_level_up: int = get_xp_to_next_lvl(self.level) - self.xp
-        return self.xp, self.level
-
-    async def load_playtime(self) -> None:
-        data = await self._auth.get(self._url_builder.playtime())
-        stats = data.get("profiles", [])[0].get("stats", {})
-
-        self.level = int(stats.get("PClearanceLevel", {}).get("value", 0))
-        self.pvp_time_played = int(stats.get("PPvPTimePlayed", {}).get("value", 0))
-        self.pve_time_played = int(stats.get("PPvETimePlayed", {}).get("value", 0))
-        self.total_time_played = int(stats.get("PTotalTimePlayed", {}).get("value", 0))
-
-    async def load_skill_records(self, seasons: list[int] = None, boards: list[str] = None, regions: list[str] = None) -> None:
-        """Can get data only for seasons 6 (Health - Y2S2) until 27 (Brutal Swarm - Y7S3) because of ranked 2.0"""
-        _all_seasons = ",".join([str(s) for s in range(6, 28)])
-
-        if seasons and not set(list(range(6, 28))).issuperset(set(seasons)):
-            raise ValueError(f"Seasons can only be between 6 and 27. You gave {seasons}")
-
-        seasons = ",".join([str(s) for s in seasons]) if seasons else _all_seasons
-        boards = ",".join(boards) if boards else "pvp_ranked,pvp_casual"
-        regions = ",".join(regions) if regions else "emea,ncsa,apac,global"
-        data = await self._auth.get(self._url_builder.skill_records(seasons, boards, regions))
-
-        for season in data["seasons_player_skill_records"]:
-            season_id = season["season_id"]
-
-            for region in season["regions_player_skill_records"]:
-                region_id = region["region_id"]
-
-                for board in region["boards_player_skill_records"]:
-                    board_id = board["board_id"]
-                    rank_obj = Rank(board["players_skill_records"][0]) if board["players_skill_records"] else Rank({})
-
-                    # If user didn't play in this season and region
-                    played = (rank_obj.wins + rank_obj.losses + rank_obj.abandons) != 0
-
-                    if board_id == "pvp_ranked":
-                        self.rank_skill_records.setdefault(season_id, {})
-                        self.rank_skill_records[season_id]["global"] = rank_obj if played else None
-                        self.rank_skill_records[season_id][region_id] = rank_obj if played else None
-                    elif board_id == "pvp_casual":
-                        self.casual_skill_records.setdefault(season_id, {})
-                        self.casual_skill_records[season_id][region_id] = rank_obj if played else None
-
-    async def load_summaries(self, gamemodes: list[str] = None, team_roles: list[str] = None) -> None:
-        gamemodes = ",".join(gamemodes) if gamemodes else "all,ranked,unranked,casual"
-        team_roles = ",".join(team_roles) if team_roles else "all,Attacker,Defender"
-        data = await self._auth.get(self._url_builder.seasonal_summaries(gamemodes, team_roles))
-
-        data_gamemodes = data.get('profileData').get(self.id).get("platforms").get(self._platform_group).get("gameModes")
-
-        for gamemode in data_gamemodes:
-            roles = data_gamemodes[gamemode]['teamRoles']
-
-            for role in roles:
-                for season in roles[role]:
-                    season_id = season_code_to_id(f"{season['seasonYear']}{season['seasonNumber']}")
-
-                    if gamemode == "ranked":
-                        self.ranked_summary.setdefault(season_id, {}).setdefault(role, {})
-                        self.ranked_summary[season_id][role] = Summary(season)
-                    elif gamemode == "unranked":
-                        self.unranked_summary.setdefault(season_id, {}).setdefault(role, {})
-                        self.unranked_summary[season_id][role] = Summary(season)
-                    elif gamemode == "casual":
-                        self.casual_summary.setdefault(season_id, {}).setdefault(role, {})
-                        self.casual_summary[season_id][role] = Summary(season)
-                    elif gamemode == "all":
-                        self.all_summary.setdefault(season_id, {}).setdefault(role, {})
-                        self.all_summary[season_id][role] = Summary(season)
-
-    async def load_trends(self) -> Trends:
-        self.trends = Trends(await self._auth.get(self._url_builder.trends()))
-        return self.trends
-
-    async def load_weapons(self) -> Weapons:
-        self.weapons = Weapons(await self._auth.get(self._url_builder.weapons()))
-        return self.weapons
-
-    async def load_operators(self, op_about: bool = False) -> Operators:
-        self.operators = Operators(await self._auth.get(self._url_builder.operators()), op_about)
-        return self.operators
-
-    async def load_maps(self) -> Maps:
-        self.maps = Maps(await self._auth.get(self._url_builder.maps()))
-        return self.maps
-
-    async def load_ranked_v2(self) -> tuple[FullProfile | None, FullProfile | None, FullProfile | None, FullProfile | None, FullProfile | None]:
-        """ Returns a tuple of FullProfile objects for each profile board (unranked, ranked, casual, warmup, event) """
-
-        data = await self._auth.get(self._url_builder.full_profiles(), new=True)
-        boards = data.get('platform_families_full_profiles', [])[0].get('board_ids_full_profiles', [])
-
-        for board in boards:
-
-            if board.get('board_id') == 'unranked':
-                self.unranked_profile = FullProfile(board.get('full_profiles', [])[0])
-            elif board.get('board_id') == 'ranked':
-                self.ranked_profile = FullProfile(board.get('full_profiles', [])[0])
-            elif board.get('board_id') == 'casual':
-                self.casual_profile = FullProfile(board.get('full_profiles', [])[0])
-            elif board.get('board_id') == 'warmup':
-                self.warmup_profile = FullProfile(board.get('full_profiles', [])[0])
-            elif board.get('board_id') == 'event':
-                self.event_profile = FullProfile(board.get('full_profiles', [])[0])
-
-        return self.unranked_profile, self.ranked_profile, self.casual_profile, self.warmup_profile, self.event_profile
+from __future__ import annotations
+
+from .utils import season_code_to_id, get_total_xp, get_xp_to_next_lvl
+from .linked_accounts import LinkedAccount
+from .rank_profile import FullProfile
+from .url_builder import UrlBuilder
+from .operators import Operators
+from .summaries import Summary
+from .weapons import Weapons
+from .trends import Trends
+from .ranks import Rank
+from .maps import Maps
+
+import aiohttp
+import re
+
+platform_url_names = {"uplay": "OSBOR_PC_LNCH_A", "psn": "OSBOR_PS4_LNCH_A", "xbl": "OSBOR_XBOXONE_LNCH_A", "xplay": "OSBOR_XPLAY_LNCH_A"}
+date_pattern = re.compile(r"^((2\d)\d{2})(0[1-9]|1[012])([012]\d|3[01])$")
+
+
+class Player:
+    def __init__(self, auth: aiohttp.ClientSession(), data: dict):
+
+        self.id: str = data.get("profileId")
+
+        self._auth: aiohttp.ClientSession() = auth
+        self._platform: str = data.get("platformType")
+        self._platform_url: str = platform_url_names[self._platform]
+        self._spaceid: str = self._auth.spaceids[self._platform]
+        self._platform_group: str = "PC" if self._platform == "uplay" else "Console"
+        self._url_builder: UrlBuilder = UrlBuilder(self._spaceid, self._platform_url, self.id, self._platform_group)
+
+        self.profile_pic_url_146: str = f"https://ubisoft-avatars.akamaized.net/{self.id}/default_146_146.png"
+        self.profile_pic_url_256: str = f"https://ubisoft-avatars.akamaized.net/{self.id}/default_256_256.png"
+        self.profile_pic_url_500: str = f"https://ubisoft-avatars.akamaized.net/{self.id}/default_tall.png"
+        self.profile_pic_url: str = self.profile_pic_url_256
+        self.linked_accounts: list[LinkedAccount] = []
+
+        self.name: str = data.get("nameOnPlatform")
+        self.level: int = 0
+        self.alpha_pack: float = 0
+        self.xp: int = 0
+        self.total_xp: int = 0
+        self.xp_to_level_up: int = 0
+
+        self.total_time_played: int = 0
+        self.pvp_time_played: int = 0
+        self.pve_time_played: int = 0
+
+        self.rank_skill_records: dict[int: dict[str: Rank | None]] | dict = {}
+        self.casual_skill_records: dict[int: dict[str: Rank | None]] | dict = {}
+
+        self.ranked_summary: dict = {}
+        self.casual_summary: dict = {}
+        self.unranked_summary: dict = {}
+        self.all_summary: dict = {}
+
+        self.unranked_profile: FullProfile | None = None
+        self.ranked_profile: FullProfile | None = None
+        self.casual_profile: FullProfile | None = None
+        self.warmup_profile: FullProfile | None = None
+        self.event_profile: FullProfile | None = None
+
+        self.weapons: Weapons | None = None
+        self.trends: Trends | None = None
+        self.operators: Operators | None = None
+        self.maps: Maps | None = None
+
+    def set_timespan_dates(self, start_date: str, end_date: str) -> None:
+        """YYYYMMDD"""
+        if not date_pattern.match(start_date):
+            raise ValueError(f"Date for start_date '{start_date}' is invalid. The date format is 'YYYYMMDD'.")
+        if not date_pattern.match(end_date):
+            raise ValueError(f"Date for end_date '{end_date}' is invalid. The date format is 'YYYYMMDD'.")
+        else:
+            self._url_builder.set_timespan_dates(start_date, end_date)
+
+    async def load_linked_accounts(self):
+        data = await self._auth.get(self._url_builder.connected_accounts())
+        for account in data.get("profiles", []):
+            self.linked_accounts.append(LinkedAccount(account))
+        return self.linked_accounts
+
+    async def load_progress(self) -> tuple[int, int]:
+        data = await self._auth.get(self._url_builder.xp_lvl(), new=True)
+        self.level = int(data.get("level", 0))
+        self.xp = int(data.get("xp", 0))
+        self.total_xp: int = get_total_xp(self.level, self.xp)
+        self.xp_to_level_up: int = get_xp_to_next_lvl(self.level) - self.xp
+        return self.xp, self.level
+
+    async def load_playtime(self) -> None:
+        data = await self._auth.get(self._url_builder.playtime())
+        stats = data.get("profiles", [])[0].get("stats", {})
+
+        self.level = int(stats.get("PClearanceLevel", {}).get("value", 0))
+        self.pvp_time_played = int(stats.get("PPvPTimePlayed", {}).get("value", 0))
+        self.pve_time_played = int(stats.get("PPvETimePlayed", {}).get("value", 0))
+        self.total_time_played = int(stats.get("PTotalTimePlayed", {}).get("value", 0))
+
+    async def load_skill_records(self, seasons: list[int] = None, boards: list[str] = None, regions: list[str] = None) -> None:
+        """Can get data only for seasons 6 (Health - Y2S2) until 27 (Brutal Swarm - Y7S3) because of ranked 2.0"""
+        _all_seasons = ",".join([str(s) for s in range(6, 28)])
+
+        if seasons and not set(list(range(6, 28))).issuperset(set(seasons)):
+            raise ValueError(f"Seasons can only be between 6 and 27. You gave {seasons}")
+
+        seasons = ",".join([str(s) for s in seasons]) if seasons else _all_seasons
+        boards = ",".join(boards) if boards else "pvp_ranked,pvp_casual"
+        regions = ",".join(regions) if regions else "emea,ncsa,apac,global"
+        data = await self._auth.get(self._url_builder.skill_records(seasons, boards, regions))
+
+        for season in data["seasons_player_skill_records"]:
+            season_id = season["season_id"]
+
+            for region in season["regions_player_skill_records"]:
+                region_id = region["region_id"]
+
+                for board in region["boards_player_skill_records"]:
+                    board_id = board["board_id"]
+                    rank_obj = Rank(board["players_skill_records"][0]) if board["players_skill_records"] else Rank({})
+
+                    # If user didn't play in this season and region
+                    played = (rank_obj.wins + rank_obj.losses + rank_obj.abandons) != 0
+
+                    if board_id == "pvp_ranked":
+                        self.rank_skill_records.setdefault(season_id, {})
+                        self.rank_skill_records[season_id]["global"] = rank_obj if played else None
+                        self.rank_skill_records[season_id][region_id] = rank_obj if played else None
+                    elif board_id == "pvp_casual":
+                        self.casual_skill_records.setdefault(season_id, {})
+                        self.casual_skill_records[season_id][region_id] = rank_obj if played else None
+
+    async def load_summaries(self, gamemodes: list[str] = None, team_roles: list[str] = None) -> None:
+        gamemodes = ",".join(gamemodes) if gamemodes else "all,ranked,unranked,casual"
+        team_roles = ",".join(team_roles) if team_roles else "all,Attacker,Defender"
+        data = await self._auth.get(self._url_builder.seasonal_summaries(gamemodes, team_roles))
+
+        data_gamemodes = data.get('profileData').get(self.id).get("platforms").get(self._platform_group).get("gameModes")
+
+        for gamemode in data_gamemodes:
+            roles = data_gamemodes[gamemode]['teamRoles']
+
+            for role in roles:
+                for season in roles[role]:
+                    season_id = season_code_to_id(f"{season['seasonYear']}{season['seasonNumber']}")
+
+                    if gamemode == "ranked":
+                        self.ranked_summary.setdefault(season_id, {}).setdefault(role, {})
+                        self.ranked_summary[season_id][role] = Summary(season)
+                    elif gamemode == "unranked":
+                        self.unranked_summary.setdefault(season_id, {}).setdefault(role, {})
+                        self.unranked_summary[season_id][role] = Summary(season)
+                    elif gamemode == "casual":
+                        self.casual_summary.setdefault(season_id, {}).setdefault(role, {})
+                        self.casual_summary[season_id][role] = Summary(season)
+                    elif gamemode == "all":
+                        self.all_summary.setdefault(season_id, {}).setdefault(role, {})
+                        self.all_summary[season_id][role] = Summary(season)
+
+    async def load_trends(self) -> Trends:
+        self.trends = Trends(await self._auth.get(self._url_builder.trends()))
+        return self.trends
+
+    async def load_weapons(self) -> Weapons:
+        self.weapons = Weapons(await self._auth.get(self._url_builder.weapons()))
+        return self.weapons
+
+    async def load_operators(self, op_about: bool = False) -> Operators:
+        self.operators = Operators(await self._auth.get(self._url_builder.operators()), op_about)
+        return self.operators
+
+    async def load_maps(self) -> Maps:
+        self.maps = Maps(await self._auth.get(self._url_builder.maps()))
+        return self.maps
+
+    async def load_ranked_v2(self) -> tuple[FullProfile | None, FullProfile | None, FullProfile | None, FullProfile | None, FullProfile | None]:
+        """ Returns a tuple of FullProfile objects for each profile board (unranked, ranked, casual, warmup, event) """
+
+        data = await self._auth.get(self._url_builder.full_profiles(), new=True)
+        boards = data.get('platform_families_full_profiles', [])[0].get('board_ids_full_profiles', [])
+
+        for board in boards:
+
+            if board.get('board_id') == 'unranked':
+                self.unranked_profile = FullProfile(board.get('full_profiles', [])[0])
+            elif board.get('board_id') == 'ranked':
+                self.ranked_profile = FullProfile(board.get('full_profiles', [])[0])
+            elif board.get('board_id') == 'casual':
+                self.casual_profile = FullProfile(board.get('full_profiles', [])[0])
+            elif board.get('board_id') == 'warmup':
+                self.warmup_profile = FullProfile(board.get('full_profiles', [])[0])
+            elif board.get('board_id') == 'event':
+                self.event_profile = FullProfile(board.get('full_profiles', [])[0])
+
+        return self.unranked_profile, self.ranked_profile, self.casual_profile, self.warmup_profile, self.event_profile
```

### Comparing `siegeapi-6.0.1/siegeapi/rank_profile.py` & `siegeapi-6.1.0/siegeapi/rank_profile.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from __future__ import annotations
-from .utils import season_id_to_code, get_rank_from_mmr, get_rank_constants
-
-
-class FullProfile:
-    def __init__(self, data):
-        profile = data.get("profile", {})
-        season_stats = data.get("season_statistics", {})
-        match_outcomes = season_stats.get("match_outcomes", {})
-
-        self.max_rank_id: int = profile.get("max_rank", 0)
-        self.max_rank_points: int = profile.get("max_rank_points", 0)
-        self.rank_id: int = profile.get("rank", 0)
-        self.rank_points: int = profile.get("rank_points", 0)
-        self.top_rank_position: int = profile.get("top_rank_position", 0)
-        self.season_id: int = profile.get("season_id", 0)
-
-        rank_constants = get_rank_constants(self.season_id)
-        _, prev_, next_, _ = get_rank_from_mmr(self.rank_points)
-        self.max_rank: str = rank_constants[self.max_rank_id]["name"]
-        self.rank: str = rank_constants[self.rank_id]["name"]
-        self.prev_rank_points: int = prev_
-        self.next_rank_points: int = next_
-        self.season_code: str = season_id_to_code(self.season_id)
-
-        self.kills: int = season_stats.get("kills", 0)
-        self.deaths: int = season_stats.get("deaths", 0)
-        self.abandons: int = match_outcomes.get("abandons", 0)
-        self.losses: int = match_outcomes.get("losses", 0)
-        self.wins: int = match_outcomes.get("wins", 0)
-
-    def get_dict(self) -> dict[str: str | int | float]:
-        return vars(self)
+from __future__ import annotations
+from .utils import season_id_to_code, get_rank_from_mmr, get_rank_constants
+
+
+class FullProfile:
+    def __init__(self, data):
+        profile = data.get("profile", {})
+        season_stats = data.get("season_statistics", {})
+        match_outcomes = season_stats.get("match_outcomes", {})
+
+        self.max_rank_id: int = profile.get("max_rank", 0)
+        self.max_rank_points: int = profile.get("max_rank_points", 0)
+        self.rank_id: int = profile.get("rank", 0)
+        self.rank_points: int = profile.get("rank_points", 0)
+        self.top_rank_position: int = profile.get("top_rank_position", 0)
+        self.season_id: int = profile.get("season_id", 0)
+
+        rank_constants = get_rank_constants(self.season_id)
+        _, prev_, next_, _ = get_rank_from_mmr(self.rank_points)
+        self.max_rank: str = rank_constants[self.max_rank_id]["name"]
+        self.rank: str = rank_constants[self.rank_id]["name"]
+        self.prev_rank_points: int = prev_
+        self.next_rank_points: int = next_
+        self.season_code: str = season_id_to_code(self.season_id)
+
+        self.kills: int = season_stats.get("kills", 0)
+        self.deaths: int = season_stats.get("deaths", 0)
+        self.abandons: int = match_outcomes.get("abandons", 0)
+        self.losses: int = match_outcomes.get("losses", 0)
+        self.wins: int = match_outcomes.get("wins", 0)
+
+    def get_dict(self) -> dict[str: str | int | float]:
+        return vars(self)
```

### Comparing `siegeapi-6.0.1/siegeapi/ranks.py` & `siegeapi-6.1.0/siegeapi/ranks.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from __future__ import annotations
-
-from .constants.seasons import seasons
-from .utils import get_rank_constants, get_rank_from_mmr
-
-
-class Rank:
-    def __init__(self, data):
-        self.kills: int = data.get("kills", 0)
-        self.deaths: int = data.get("deaths", 0)
-        self.last_mmr_change: int = int(data.get("last_match_mmr_change", 0))
-        self.prev_rank_mmr: int = int(data.get("previous_rank_mmr", 0))
-        self.next_rank_mmr: int = int(data.get("next_rank_mmr", 0))
-        self.mmr: int = int(data.get("mmr", 0))
-        self.max_mmr: int = int(data.get("max_mmr", 0))
-        self.wins: int = data.get("wins", 0)
-        self.losses: int = data.get("losses", 0)
-        self.rank_id: int = data.get("rank", 0)
-        self.season: int = data.get("season", -10000)
-        _rank_definitions = get_rank_constants(self.season)
-        self.rank: str = _rank_definitions[self.rank_id]["name"]
-        self.max_rank_id: int = data.get("max_rank", 0)
-        self.max_rank: str = _rank_definitions[self.max_rank_id]["name"]
-        self.region: str = data.get("region", "missing")
-        self.abandons: int = data.get("abandons", 0)
-        self.skill_mean: float = data.get("skill_mean", 0)
-        self.skill_stdev: float = data.get("skill_stdev", 0)
-        self.season_name: str = seasons[self.season]["name"] or seasons[0]["name"]
-        self.season_code: str = seasons[self.season]["code"] or seasons[0]["code"]
-
-        # For casual where the API doesn't return this data
-        if self.prev_rank_mmr == 0 and self.next_rank_mmr == 0:
-            self.rank, self.prev_rank_mmr, self.next_rank_mmr, self.rank_id = get_rank_from_mmr(self.mmr)
-            self.max_rank_id = self.max_mmr = 0
-            self.max_rank = "Undefined"
-
-    def get_dict(self) -> dict[str: str | int | float]:
-        return vars(self)
+from __future__ import annotations
+
+from .constants.seasons import seasons
+from .utils import get_rank_constants, get_rank_from_mmr
+
+
+class Rank:
+    def __init__(self, data):
+        self.kills: int = data.get("kills", 0)
+        self.deaths: int = data.get("deaths", 0)
+        self.last_mmr_change: int = int(data.get("last_match_mmr_change", 0))
+        self.prev_rank_mmr: int = int(data.get("previous_rank_mmr", 0))
+        self.next_rank_mmr: int = int(data.get("next_rank_mmr", 0))
+        self.mmr: int = int(data.get("mmr", 0))
+        self.max_mmr: int = int(data.get("max_mmr", 0))
+        self.wins: int = data.get("wins", 0)
+        self.losses: int = data.get("losses", 0)
+        self.rank_id: int = data.get("rank", 0)
+        self.season: int = data.get("season", -10000)
+        _rank_definitions = get_rank_constants(self.season)
+        self.rank: str = _rank_definitions[self.rank_id]["name"]
+        self.max_rank_id: int = data.get("max_rank", 0)
+        self.max_rank: str = _rank_definitions[self.max_rank_id]["name"]
+        self.region: str = data.get("region", "missing")
+        self.abandons: int = data.get("abandons", 0)
+        self.skill_mean: float = data.get("skill_mean", 0)
+        self.skill_stdev: float = data.get("skill_stdev", 0)
+        self.season_name: str = seasons[self.season]["name"] or seasons[0]["name"]
+        self.season_code: str = seasons[self.season]["code"] or seasons[0]["code"]
+
+        # For casual where the API doesn't return this data
+        if self.prev_rank_mmr == 0 and self.next_rank_mmr == 0:
+            self.rank, self.prev_rank_mmr, self.next_rank_mmr, self.rank_id = get_rank_from_mmr(self.mmr)
+            self.max_rank_id = self.max_mmr = 0
+            self.max_rank = "Undefined"
+
+    def get_dict(self) -> dict[str: str | int | float]:
+        return vars(self)
```

### Comparing `siegeapi-6.0.1/siegeapi/url_builder.py` & `siegeapi-6.1.0/siegeapi/url_builder.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,99 +1,102 @@
-
-
-class UrlBuilder:
-    def __init__(self, spaceid: str, platform_url: str, player_id: str, platform_group: str):
-        self.spaceid: str = spaceid
-        self.platform_url: str = platform_url
-        self.platform_group: str = platform_group
-        self.player_id: str = player_id
-        self.start_date: str = ""
-        self.end_date: str = ""
-
-    def set_timespan_dates(self, start_date: str, end_date: str) -> None:
-        self.start_date = f"&startDate={start_date}"
-        self.end_date = f"&endDate={end_date}"
-
-    def xp_lvl(self) -> str:
-        return f"https://public-ubiservices.ubi.com/v1/spaces/0d2ae42d-4c27-4cb7-af6c-2099062302bb/title/r6s/rewards/public_profile?" \
-               f"profile_id={self.player_id}"
-
-    def playtime(self) -> str:
-        return f"https://public-ubiservices.ubi.com/v1/profiles/stats?" \
-               f"profileIds={self.player_id}" \
-               f"&spaceId=0d2ae42d-4c27-4cb7-af6c-2099062302bb" \
-               f"&statNames=PPvPTimePlayed,PPvETimePlayed,PTotalTimePlayed,PClearanceLevel"
-
-    def skill_records(self, seasons: str, boards: str, regions: str):
-        return f"https://public-ubiservices.ubi.com/v1/spaces/{self.spaceid}/" \
-               f"sandboxes/{self.platform_url}/r6karma/player_skill_records?" \
-               f"board_ids={boards}" \
-               f"&season_ids={seasons}" \
-               f"&region_ids={regions}" \
-               f"&profile_ids={self.player_id}"
-
-    def boards(self, season: int, board_id: str, region: str) -> str:
-        return f"https://public-ubiservices.ubi.com/v1/spaces/{self.spaceid}/" \
-               f"sandboxes/{self.platform_url}/r6karma/players?" \
-               f"board_id=pvp_{board_id}" \
-               f"&profile_ids={self.player_id}" \
-               f"&region_id={region}" \
-               f"&season_id={season}"
-
-    def trends(self) -> str:
-        return f"https://prod.datadev.ubisoft.com/v1/profiles/{self.player_id}/playerstats?" \
-               f"spaceId={self.spaceid}" \
-               f"&view=current" \
-               f"&aggregation=movingpoint" \
-               f"&trendType=daily" \
-               f"&gameMode=all,ranked,casual,unranked" \
-               f"&platformGroup=PC" \
-               f"&teamRole=all,attacker,defender" \
-               f"{self.start_date}" \
-               f"{self.end_date}"
-
-    def weapons(self) -> str:
-        return f"https://prod.datadev.ubisoft.com/v1/profiles/{self.player_id}/playerstats?" \
-               f"spaceId={self.spaceid}" \
-               f"&view=current" \
-               f"&aggregation=weapons" \
-               f"&gameMode=all,ranked,casual,unranked" \
-               f"&platformGroup=PC" \
-               f"&teamRole=attacker,defender" \
-               f"{self.start_date}" \
-               f"{self.end_date}"
-
-    def operators(self) -> str:
-        return f"https://prod.datadev.ubisoft.com/v1/profiles/{self.player_id}/playerstats?" \
-               f"spaceId={self.spaceid}" \
-               f"&view=current" \
-               f"&aggregation=operators" \
-               f"&gameMode=all,ranked,casual,unranked" \
-               f"&platformGroup=PC" \
-               f"&teamRole=all,Attacker,Defender" \
-               f"{self.start_date}" \
-               f"{self.end_date}"
-
-    def maps(self) -> str:
-        return f"https://prod.datadev.ubisoft.com/v1/profiles/{self.player_id}/playerstats?" \
-               f"spaceId={self.spaceid}" \
-               f"&view=current" \
-               f"&aggregation=maps" \
-               f"&gameMode=all,ranked,casual,unranked" \
-               f"&platformGroup=PC" \
-               f"&teamRole=all,Attacker,Defender" \
-               f"{self.start_date}" \
-               f"{self.end_date}"
-
-    def seasonal_summaries(self, gamemodes: str, team_roles: str) -> str:
-        return f"https://prod.datadev.ubisoft.com/v1/users/{self.player_id}/playerstats?" \
-               f"spaceId={self.spaceid}" \
-               f"&view=seasonal" \
-               f"&aggregation=summary" \
-               f"&gameMode={gamemodes}" \
-               f"&platformGroup={self.platform_group}" \
-               f"&teamRole={team_roles}"
-
-    def full_profiles(self) -> str:
-        return f"https://public-ubiservices.ubi.com/v2/spaces/0d2ae42d-4c27-4cb7-af6c-2099062302bb/title/r6s/skill/full_profiles?" \
-               f"profile_ids={self.player_id}" \
-               f"&platform_families={self.platform_group.lower()}"
+
+
+class UrlBuilder:
+    def __init__(self, spaceid: str, platform_url: str, player_id: str, platform_group: str):
+        self.spaceid: str = spaceid
+        self.platform_url: str = platform_url
+        self.platform_group: str = platform_group
+        self.player_id: str = player_id
+        self.start_date: str = ""
+        self.end_date: str = ""
+
+    def set_timespan_dates(self, start_date: str, end_date: str) -> None:
+        self.start_date = f"&startDate={start_date}"
+        self.end_date = f"&endDate={end_date}"
+
+    def connected_accounts(self) -> str:
+        return f"https://public-ubiservices.ubi.com/v3/users/{self.player_id}/profiles"
+
+    def xp_lvl(self) -> str:
+        return f"https://public-ubiservices.ubi.com/v1/spaces/0d2ae42d-4c27-4cb7-af6c-2099062302bb/title/r6s/rewards/public_profile?" \
+               f"profile_id={self.player_id}"
+
+    def playtime(self) -> str:
+        return f"https://public-ubiservices.ubi.com/v1/profiles/stats?" \
+               f"profileIds={self.player_id}" \
+               f"&spaceId=0d2ae42d-4c27-4cb7-af6c-2099062302bb" \
+               f"&statNames=PPvPTimePlayed,PPvETimePlayed,PTotalTimePlayed,PClearanceLevel"
+
+    def skill_records(self, seasons: str, boards: str, regions: str):
+        return f"https://public-ubiservices.ubi.com/v1/spaces/{self.spaceid}/" \
+               f"sandboxes/{self.platform_url}/r6karma/player_skill_records?" \
+               f"board_ids={boards}" \
+               f"&season_ids={seasons}" \
+               f"&region_ids={regions}" \
+               f"&profile_ids={self.player_id}"
+
+    def boards(self, season: int, board_id: str, region: str) -> str:
+        return f"https://public-ubiservices.ubi.com/v1/spaces/{self.spaceid}/" \
+               f"sandboxes/{self.platform_url}/r6karma/players?" \
+               f"board_id=pvp_{board_id}" \
+               f"&profile_ids={self.player_id}" \
+               f"&region_id={region}" \
+               f"&season_id={season}"
+
+    def trends(self) -> str:
+        return f"https://prod.datadev.ubisoft.com/v1/profiles/{self.player_id}/playerstats?" \
+               f"spaceId={self.spaceid}" \
+               f"&view=current" \
+               f"&aggregation=movingpoint" \
+               f"&trendType=daily" \
+               f"&gameMode=all,ranked,casual,unranked" \
+               f"&platformGroup=PC" \
+               f"&teamRole=all,attacker,defender" \
+               f"{self.start_date}" \
+               f"{self.end_date}"
+
+    def weapons(self) -> str:
+        return f"https://prod.datadev.ubisoft.com/v1/profiles/{self.player_id}/playerstats?" \
+               f"spaceId={self.spaceid}" \
+               f"&view=current" \
+               f"&aggregation=weapons" \
+               f"&gameMode=all,ranked,casual,unranked" \
+               f"&platformGroup=PC" \
+               f"&teamRole=attacker,defender" \
+               f"{self.start_date}" \
+               f"{self.end_date}"
+
+    def operators(self) -> str:
+        return f"https://prod.datadev.ubisoft.com/v1/profiles/{self.player_id}/playerstats?" \
+               f"spaceId={self.spaceid}" \
+               f"&view=current" \
+               f"&aggregation=operators" \
+               f"&gameMode=all,ranked,casual,unranked" \
+               f"&platformGroup=PC" \
+               f"&teamRole=all,Attacker,Defender" \
+               f"{self.start_date}" \
+               f"{self.end_date}"
+
+    def maps(self) -> str:
+        return f"https://prod.datadev.ubisoft.com/v1/profiles/{self.player_id}/playerstats?" \
+               f"spaceId={self.spaceid}" \
+               f"&view=current" \
+               f"&aggregation=maps" \
+               f"&gameMode=all,ranked,casual,unranked" \
+               f"&platformGroup=PC" \
+               f"&teamRole=all,Attacker,Defender" \
+               f"{self.start_date}" \
+               f"{self.end_date}"
+
+    def seasonal_summaries(self, gamemodes: str, team_roles: str) -> str:
+        return f"https://prod.datadev.ubisoft.com/v1/users/{self.player_id}/playerstats?" \
+               f"spaceId={self.spaceid}" \
+               f"&view=seasonal" \
+               f"&aggregation=summary" \
+               f"&gameMode={gamemodes}" \
+               f"&platformGroup={self.platform_group}" \
+               f"&teamRole={team_roles}"
+
+    def full_profiles(self) -> str:
+        return f"https://public-ubiservices.ubi.com/v2/spaces/0d2ae42d-4c27-4cb7-af6c-2099062302bb/title/r6s/skill/full_profiles?" \
+               f"profile_ids={self.player_id}" \
+               f"&platform_families={self.platform_group.lower()}"
```

### Comparing `siegeapi-6.0.1/siegeapi/utils.py` & `siegeapi-6.1.0/siegeapi/utils.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-from __future__ import annotations
-
-from .constants import seasons as seasons_const
-from .exceptions import InvalidAttributeCombination
-from .constants.ranks import *
-
-
-def get_xp_to_next_lvl(lvl: int) -> int:
-    if lvl > 37:
-        return (lvl - 18) * 500
-    if lvl == 0:
-        return 500
-    if lvl == 1:
-        return 1_500
-    if lvl in (2, 3):
-        return 3_500
-    if lvl in (4, 5):
-        return 4_000
-    if lvl in (6, 7, 8):
-        return 4_500
-    if lvl in (9, 10):
-        return 5_500
-    if lvl in (11, 12, 13):
-        return 6_000
-    if lvl in (14, 15, 16):
-        return 6_500
-    if lvl in (17, 18, 19):
-        return 7_000
-    if lvl in (20, 21, 22):
-        return 7_500
-    if lvl in (23, 24, 25):
-        return 8_000
-    if lvl in (26, 27, 28):
-        return 8_500
-    if lvl in (29, 30, 31):
-        return 9_000
-    if lvl in (32, 33, 34):
-        return 9_500
-    if lvl in (35, 36, 37):
-        return 10_000
-
-
-def get_total_xp(lvl: int, current_xp: int) -> int:
-    total = 0
-    for level in range(1, lvl):
-        total += get_xp_to_next_lvl(level)
-    return total + current_xp
-
-
-def season_id_to_code(season_id: int) -> str:
-    seasons_count = len(seasons_const) - 3
-    season_id = seasons_count - season_id if season_id < 0 else season_id
-
-    return seasons_const.get(season_id, {}).get("code")
-
-
-def season_code_to_id(season_code: str) -> int:
-    """Depends on 'seasons_const' always being up-to-date.."""
-    seasons_count = len(seasons_const) - 3
-    season_id = next((k for k, v in seasons_const.items() if v["code"] == season_code), None)
-
-    if season_id is None:
-        raise InvalidAttributeCombination(f"Season code '{season_code}' is invalid")
-
-    return seasons_count - season_id if season_id < 0 else season_id
-
-
-def get_rank_constants(season_number: int = -1) -> list[dict[str: str | int]]:
-    if 1 <= season_number <= 3:
-        return ranks_v1
-    if 4 == season_number:
-        return ranks_v2
-    if 5 <= season_number <= 14:
-        return ranks_v3
-    if 15 <= season_number <= 22:
-        return ranks_v4
-    if 23 <= season_number <= 27:
-        return ranks_v5
-    if 28 <= season_number:
-        return ranks_v6
-    return ranks_v6
-
-
-def get_rank_from_mmr(mmr: int | float, season: int = -1) -> tuple[str, int, int, int]:
-    for rank_id, r in enumerate(get_rank_constants(season)):
-        if r["min_mmr"] <= int(mmr) <= r["max_mmr"]:
-            return r["name"], r["min_mmr"], r["max_mmr"]+1, rank_id
-    return "Unranked", 0, 0, 0
+from __future__ import annotations
+
+from .constants import seasons as seasons_const
+from .exceptions import InvalidAttributeCombination
+from .constants.ranks import *
+
+
+def get_xp_to_next_lvl(lvl: int) -> int:
+    if lvl > 37:
+        return (lvl - 18) * 500
+    if lvl == 0:
+        return 500
+    if lvl == 1:
+        return 1_500
+    if lvl in (2, 3):
+        return 3_500
+    if lvl in (4, 5):
+        return 4_000
+    if lvl in (6, 7, 8):
+        return 4_500
+    if lvl in (9, 10):
+        return 5_500
+    if lvl in (11, 12, 13):
+        return 6_000
+    if lvl in (14, 15, 16):
+        return 6_500
+    if lvl in (17, 18, 19):
+        return 7_000
+    if lvl in (20, 21, 22):
+        return 7_500
+    if lvl in (23, 24, 25):
+        return 8_000
+    if lvl in (26, 27, 28):
+        return 8_500
+    if lvl in (29, 30, 31):
+        return 9_000
+    if lvl in (32, 33, 34):
+        return 9_500
+    if lvl in (35, 36, 37):
+        return 10_000
+
+
+def get_total_xp(lvl: int, current_xp: int) -> int:
+    total = 0
+    for level in range(1, lvl):
+        total += get_xp_to_next_lvl(level)
+    return total + current_xp
+
+
+def season_id_to_code(season_id: int) -> str:
+    seasons_count = len(seasons_const) - 3
+    season_id = seasons_count - season_id if season_id < 0 else season_id
+
+    return seasons_const.get(season_id, {}).get("code")
+
+
+def season_code_to_id(season_code: str) -> int:
+    """Depends on 'seasons_const' always being up-to-date.."""
+    seasons_count = len(seasons_const) - 3
+    season_id = next((k for k, v in seasons_const.items() if v["code"] == season_code), None)
+
+    if season_id is None:
+        raise InvalidAttributeCombination(f"Season code '{season_code}' is invalid")
+
+    return seasons_count - season_id if season_id < 0 else season_id
+
+
+def get_rank_constants(season_number: int = -1) -> list[dict[str: str | int]]:
+    if 1 <= season_number <= 3:
+        return ranks_v1
+    if 4 == season_number:
+        return ranks_v2
+    if 5 <= season_number <= 14:
+        return ranks_v3
+    if 15 <= season_number <= 22:
+        return ranks_v4
+    if 23 <= season_number <= 27:
+        return ranks_v5
+    if 28 <= season_number:
+        return ranks_v6
+    return ranks_v6
+
+
+def get_rank_from_mmr(mmr: int | float, season: int = -1) -> tuple[str, int, int, int]:
+    for rank_id, r in enumerate(get_rank_constants(season)):
+        if r["min_mmr"] <= int(mmr) <= r["max_mmr"]:
+            return r["name"], r["min_mmr"], r["max_mmr"]+1, rank_id
+    return "Unranked", 0, 0, 0
```

### Comparing `siegeapi-6.0.1/siegeapi/weapons.py` & `siegeapi-6.1.0/siegeapi/weapons.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-from __future__ import annotations
-
-from .constants import WEAPONS_DICT
-
-
-class Weapon:
-    def __init__(self, data: dict):
-        self.name: str = data.get("weaponName")
-        self.kills: int = data.get("kills")
-        self.headshots: int = data.get("headshots")
-        self.hs_accuracy: float = data.get("headshotAccuracy")
-        self.rounds_played: int = data.get("roundsPlayed")
-        self.rounds_won: int = data.get("roundsWon")
-        self.rounds_lost: float = data.get("roundsLost")
-        self.rounds_with_kill: float = data.get("roundsWithAKill")
-        self.rounds_with_multi_kill: float = data.get("roundsWithMultiKill")
-
-        if weapon := WEAPONS_DICT.get(self.name):
-            self.ubi_url: str = f"https://staticctf.akamaized.net/J3yJr34U2pZ2Ieem48Dwy9uqj5PNUQTn/{weapon.get('icon_url')}"
-            self.imgur_url: str = weapon.get("imgur_url")
-            self.type: str = weapon.get("type")
-        else:
-            self.ubi_url: str = "Missing Asset"
-            self.imgur_url: str = "Missing Asset"
-            self.type: str = "Missing Asset"
-
-    def __repr__(self) -> str:
-        return str(vars(self))
-
-
-class WeaponsGameMode:
-    def __init__(self, data: dict):
-        self.primary: list = self._get_weapons_list(data.get("weaponSlots", {}).get("primaryWeapons", {}).get("weaponTypes", [{}])[0].get("weapons", []))
-        self.secondary: list = self._get_weapons_list(data.get("weaponSlots", {}).get("secondaryWeapons", {}).get("weaponTypes", [{}])[0].get("weapons", []))
-
-    @staticmethod
-    def _get_weapons_list(data: list[dict] | None) -> list[Weapon] | None:
-        return None if not data else [Weapon(weapon) for weapon in data]
-
-    def __repr__(self) -> str:
-        return str(vars(self))
-
-
-class WeaponsRole:
-    def __init__(self, data: dict):
-        self.attacker: WeaponsGameMode = WeaponsGameMode(data.get("teamRoles", {}).get("attacker", {}))
-        self.defender: WeaponsGameMode = WeaponsGameMode(data.get("teamRoles", {}).get("defender", {}))
-
-    def __repr__(self) -> str:
-        return str(vars(self))
-
-
-class Weapons:
-    def __init__(self, data: dict):
-        self.all: WeaponsRole = WeaponsRole(data.get("platforms").get("PC").get("gameModes").get("all", {}))
-        self.casual: WeaponsRole = WeaponsRole(data.get("platforms").get("PC").get("gameModes").get("casual", {}))
-        self.ranked: WeaponsRole = WeaponsRole(data.get("platforms").get("PC").get("gameModes").get("ranked", {}))
-        self.unranked: WeaponsRole = WeaponsRole(data.get("platforms").get("PC").get("gameModes").get("unranked", {}))
-        self.newcomer: WeaponsRole = WeaponsRole(data.get("platforms").get("PC").get("gameModes").get("newcomer", {}))
-        self._start_date: str = str(data.get("startDate", ""))
-        self._end_date: str = str(data.get("endDate", ""))
-
-    def get_timespan_dates(self) -> dict:
-        return {"start_date": self._start_date, "end_date": self._end_date}
-
-    def __repr__(self) -> str:
-        return str(vars(self))
+from __future__ import annotations
+
+from .constants import WEAPONS_DICT
+
+
+class Weapon:
+    def __init__(self, data: dict):
+        self.name: str = data.get("weaponName")
+        self.kills: int = data.get("kills")
+        self.headshots: int = data.get("headshots")
+        self.hs_accuracy: float = data.get("headshotAccuracy")
+        self.rounds_played: int = data.get("roundsPlayed")
+        self.rounds_won: int = data.get("roundsWon")
+        self.rounds_lost: float = data.get("roundsLost")
+        self.rounds_with_kill: float = data.get("roundsWithAKill")
+        self.rounds_with_multi_kill: float = data.get("roundsWithMultiKill")
+
+        if weapon := WEAPONS_DICT.get(self.name):
+            self.ubi_url: str = f"https://staticctf.akamaized.net/J3yJr34U2pZ2Ieem48Dwy9uqj5PNUQTn/{weapon.get('icon_url')}"
+            self.imgur_url: str = weapon.get("imgur_url")
+            self.type: str = weapon.get("type")
+        else:
+            self.ubi_url: str = "Missing Asset"
+            self.imgur_url: str = "Missing Asset"
+            self.type: str = "Missing Asset"
+
+    def __repr__(self) -> str:
+        return str(vars(self))
+
+
+class WeaponsGameMode:
+    def __init__(self, data: dict):
+        self.primary: list = self._get_weapons_list(data.get("weaponSlots", {}).get("primaryWeapons", {}).get("weaponTypes", [{}])[0].get("weapons", []))
+        self.secondary: list = self._get_weapons_list(data.get("weaponSlots", {}).get("secondaryWeapons", {}).get("weaponTypes", [{}])[0].get("weapons", []))
+
+    @staticmethod
+    def _get_weapons_list(data: list[dict] | None) -> list[Weapon] | None:
+        return None if not data else [Weapon(weapon) for weapon in data]
+
+    def __repr__(self) -> str:
+        return str(vars(self))
+
+
+class WeaponsRole:
+    def __init__(self, data: dict):
+        self.attacker: WeaponsGameMode = WeaponsGameMode(data.get("teamRoles", {}).get("attacker", {}))
+        self.defender: WeaponsGameMode = WeaponsGameMode(data.get("teamRoles", {}).get("defender", {}))
+
+    def __repr__(self) -> str:
+        return str(vars(self))
+
+
+class Weapons:
+    def __init__(self, data: dict):
+        self.all: WeaponsRole = WeaponsRole(data.get("platforms").get("PC").get("gameModes").get("all", {}))
+        self.casual: WeaponsRole = WeaponsRole(data.get("platforms").get("PC").get("gameModes").get("casual", {}))
+        self.ranked: WeaponsRole = WeaponsRole(data.get("platforms").get("PC").get("gameModes").get("ranked", {}))
+        self.unranked: WeaponsRole = WeaponsRole(data.get("platforms").get("PC").get("gameModes").get("unranked", {}))
+        self.newcomer: WeaponsRole = WeaponsRole(data.get("platforms").get("PC").get("gameModes").get("newcomer", {}))
+        self._start_date: str = str(data.get("startDate", ""))
+        self._end_date: str = str(data.get("endDate", ""))
+
+    def get_timespan_dates(self) -> dict:
+        return {"start_date": self._start_date, "end_date": self._end_date}
+
+    def __repr__(self) -> str:
+        return str(vars(self))
```

### Comparing `siegeapi-6.0.1/siegeapi.egg-info/PKG-INFO` & `siegeapi-6.1.0/siegeapi.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,117 +1,117 @@
-Metadata-Version: 2.1
-Name: siegeapi
-Version: 6.0.1
-Summary: Rainbow Six Siege API interface
-Home-page: https://github.com/CNDRD/siege-api
-Author: CNDRD
-License: MIT
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Internet
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Classifier: Typing :: Typed
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<div align="center">
-    <img width="250" src="https://raw.githubusercontent.com/CNDRD/siegeapi/master/assets/siegeapi-banner.png" />
-    <h1>siegeapi</h1>
-    <a href="https://github.com/CNDRD/siegeapi/releases">
-        <img src="https://img.shields.io/github/v/release/CNDRD/siegeapi?label=latest%20release&style=for-the-badge&logo=github&logoColor=white" />
-    </a>
-    <a href="https://pypi.org/project/siegeapi/#history">
-        <img src="https://img.shields.io/pypi/v/siegeapi?style=for-the-badge&logo=pypi&logoColor=white" />
-    </a>
-    <br />
-    <a href="https://www.python.org/downloads/">
-        <img src="https://img.shields.io/pypi/pyversions/siegeapi?style=for-the-badge&logo=python&logoColor=white&color=yellow" />
-    </a>
-    <a href="https://pypi.org/project/siegeapi">
-        <img src="https://img.shields.io/pypi/dm/siegeapi?style=for-the-badge&logo=pypi&logoColor=white&color=yellow" />
-    </a>
-</div>
-
-## How to install  
-```commandline
-pip install siegeapi
-```
-
-## Quick example  
-```python
-from siegeapi import Auth
-import asyncio
-
-async def sample():
-    auth = Auth("UBI_EMAIL", "UBI_PASSWORD")
-    player = await auth.get_player(uid="7e0f63df-a39b-44c5-8de0-d39a05926e77")
-
-    print(f"Name: {player.name}")
-    print(f"Profile pic URL: {player.profile_pic_url}")
-    
-    await player.load_playtime()
-    print(f"Total Time Played: {player.total_time_played:,} seconds")
-    print(f"Level: {player.level}")
-
-    await player.load_ranked_v2()
-    print(f"Ranked Points: {player.ranked_profile.rank_points}")
-    print(f"Rank: {player.ranked_profile.rank}")
-    print(f"Max Rank Points: {player.ranked_profile.max_rank_points}")
-    print(f"Max Rank: {player.ranked_profile.max_rank}")
-
-    await player.load_progress()
-    print(f"XP: {player.xp:,}")
-    print(f"Total XP: {player.total_xp:,}")
-    print(f"XP to level up: {player.xp_to_level_up:,}")
-    
-    await auth.close()
-
-asyncio.get_event_loop().run_until_complete(sample())
-# Or `asyncio.run(sample())`  
-```
-### Output  
-```text
-Name: CNDRD
-Profile pic URL: https://ubisoft-avatars.akamaized.net/7e0f63df-a39b-44c5-8de0-d39a05926e77/default_256_256.png
-Total Time Played: 7,910,265 seconds
-Level: 285
-Ranked Points: 1000
-Rank: Unranked
-Max Rank Points: 1000
-Max Rank: Unranked
-XP: 56,362
-Total XP: 17,973,862
-XP to level up: 77,138
-```
-
----  
-
-## Siege Inventory  
-If you want to see every skin, headgear, uniform and more, head over to **[skins.cndrd.xyz](https://skins.cndrd.xyz/)**  
-
-## Docs  
-For docs go to [cndrd.github.io/siegeapi](https://cndrd.github.io/siegeapi/)  
-
-## Credits  
-Operator Icons from [r6operators][r6operators_] by [marcopixel][marcopixel_]  
-Built (and re-built) on top of what [billy-yoyo][r6s_python_api] started  
-
-## Problems  
-If you experience any problems, reach out to me, or submit a PR  
-You can reach out here on GitHub or on Discord (_CNDRD#2233_)  
-
-
-![forthebadge](https://forthebadge.com/images/badges/works-on-my-machine.svg)  
-![forthebadge](https://forthebadge.com/images/badges/powered-by-energy-drinks.svg)  
-
-[r6operators_]: https://github.com/marcopixel/r6operators  
-[marcopixel_]: https://github.com/marcopixel  
-[r6s_python_api]: https://github.com/billy-yoyo/RainbowSixSiege-Python-API  
+Metadata-Version: 2.1
+Name: siegeapi
+Version: 6.1.0
+Summary: Rainbow Six Siege API interface
+Home-page: https://github.com/CNDRD/siege-api
+Author: CNDRD
+License: MIT
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Internet
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
+Requires-Python: >=3.8.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<div align="center">
+    <img width="250" src="https://raw.githubusercontent.com/CNDRD/siegeapi/master/assets/siegeapi-banner.png" />
+    <h1>siegeapi</h1>
+    <a href="https://github.com/CNDRD/siegeapi/releases">
+        <img src="https://img.shields.io/github/v/release/CNDRD/siegeapi?label=latest%20release&style=for-the-badge&logo=github&logoColor=white" />
+    </a>
+    <a href="https://pypi.org/project/siegeapi/#history">
+        <img src="https://img.shields.io/pypi/v/siegeapi?style=for-the-badge&logo=pypi&logoColor=white" />
+    </a>
+    <br />
+    <a href="https://www.python.org/downloads/">
+        <img src="https://img.shields.io/pypi/pyversions/siegeapi?style=for-the-badge&logo=python&logoColor=white&color=yellow" />
+    </a>
+    <a href="https://pypi.org/project/siegeapi">
+        <img src="https://img.shields.io/pypi/dm/siegeapi?style=for-the-badge&logo=pypi&logoColor=white&color=yellow" />
+    </a>
+</div>
+
+## How to install  
+```commandline
+pip install siegeapi
+```
+
+## Quick example  
+```python
+from siegeapi import Auth
+import asyncio
+
+async def sample():
+    auth = Auth("UBI_EMAIL", "UBI_PASSWORD")
+    player = await auth.get_player(uid="7e0f63df-a39b-44c5-8de0-d39a05926e77")
+
+    print(f"Name: {player.name}")
+    print(f"Profile pic URL: {player.profile_pic_url}")
+    
+    await player.load_playtime()
+    print(f"Total Time Played: {player.total_time_played:,} seconds")
+    print(f"Level: {player.level}")
+
+    await player.load_ranked_v2()
+    print(f"Ranked Points: {player.ranked_profile.rank_points}")
+    print(f"Rank: {player.ranked_profile.rank}")
+    print(f"Max Rank Points: {player.ranked_profile.max_rank_points}")
+    print(f"Max Rank: {player.ranked_profile.max_rank}")
+
+    await player.load_progress()
+    print(f"XP: {player.xp:,}")
+    print(f"Total XP: {player.total_xp:,}")
+    print(f"XP to level up: {player.xp_to_level_up:,}")
+    
+    await auth.close()
+
+asyncio.get_event_loop().run_until_complete(sample())
+# Or `asyncio.run(sample())`  
+```
+### Output  
+```text
+Name: CNDRD
+Profile pic URL: https://ubisoft-avatars.akamaized.net/7e0f63df-a39b-44c5-8de0-d39a05926e77/default_256_256.png
+Total Time Played: 7,910,265 seconds
+Level: 285
+Ranked Points: 1000
+Rank: Unranked
+Max Rank Points: 1000
+Max Rank: Unranked
+XP: 56,362
+Total XP: 17,973,862
+XP to level up: 77,138
+```
+
+---  
+
+## Siege Inventory  
+If you want to see every skin, headgear, uniform and more, head over to **[skins.cndrd.xyz](https://skins.cndrd.xyz/)**  
+
+## Docs  
+For docs go to [cndrd.github.io/siegeapi](https://cndrd.github.io/siegeapi/)  
+
+## Credits  
+Operator Icons from [r6operators][r6operators_] by [marcopixel][marcopixel_]  
+Built (and re-built) on top of what [billy-yoyo][r6s_python_api] started  
+
+## Problems  
+If you experience any problems, reach out to me, or submit a PR  
+You can reach out here on GitHub or on Discord (_CNDRD#2233_)  
+
+
+![forthebadge](https://forthebadge.com/images/badges/works-on-my-machine.svg)  
+![forthebadge](https://forthebadge.com/images/badges/powered-by-energy-drinks.svg)  
+
+[r6operators_]: https://github.com/marcopixel/r6operators  
+[marcopixel_]: https://github.com/marcopixel  
+[r6s_python_api]: https://github.com/billy-yoyo/RainbowSixSiege-Python-API
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: siegeapi Version: 6.0.1 Summary: Rainbow Six Siege
+Metadata-Version: 2.1 Name: siegeapi Version: 6.1.0 Summary: Rainbow Six Siege
 API interface Home-page: https://github.com/CNDRD/siege-api Author: CNDRD
 License: MIT Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License Classifier: Intended
 Audience :: Developers Classifier: Natural Language :: English Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Topic :: Internet Classifier:
```

### Comparing `siegeapi-6.0.1/siegeapi.egg-info/SOURCES.txt` & `siegeapi-6.1.0/siegeapi.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 pyproject.toml
 setup.py
 siegeapi/__init__.py
 siegeapi/auth.py
 siegeapi/default_stats.py
 siegeapi/exceptions.py
+siegeapi/linked_accounts.py
 siegeapi/maps.py
 siegeapi/operators.py
 siegeapi/player.py
 siegeapi/rank_profile.py
 siegeapi/ranks.py
 siegeapi/summaries.py
 siegeapi/trends.py
```

