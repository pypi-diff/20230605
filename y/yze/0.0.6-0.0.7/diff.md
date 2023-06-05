# Comparing `tmp/yze-0.0.6.tar.gz` & `tmp/yze-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yze-0.0.6.tar", last modified: Tue May 30 20:56:10 2023, max compression
+gzip compressed data, was "yze-0.0.7.tar", last modified: Mon Jun  5 08:10:13 2023, max compression
```

## Comparing `yze-0.0.6.tar` & `yze-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-05-30 20:56:10.199971 yze-0.0.6/
--rw-r--r--   0 nicolas    (501) staff       (20)     4899 2023-05-30 20:56:10.199860 yze-0.0.6/PKG-INFO
--rw-r--r--   0 nicolas    (501) staff       (20)     4401 2023-05-30 20:52:24.000000 yze-0.0.6/README.md
--rw-r--r--   0 nicolas    (501) staff       (20)      735 2023-05-30 20:54:23.000000 yze-0.0.6/pyproject.toml
--rw-r--r--   0 nicolas    (501) staff       (20)       38 2023-05-30 20:56:10.200002 yze-0.0.6/setup.cfg
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-05-30 20:56:10.198207 yze-0.0.6/src/
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-05-30 20:56:10.198982 yze-0.0.6/src/yze/
--rw-r--r--   0 nicolas    (501) staff       (20)        0 2023-05-23 06:35:38.000000 yze-0.0.6/src/yze/__init__.py
--rw-r--r--   0 nicolas    (501) staff       (20)     5518 2023-05-30 20:53:35.000000 yze-0.0.6/src/yze/benchmark_mutant.py
--rw-r--r--   0 nicolas    (501) staff       (20)    17913 2023-05-30 10:50:59.000000 yze-0.0.6/src/yze/dice.py
--rw-r--r--   0 nicolas    (501) staff       (20)     5161 2023-05-30 20:51:44.000000 yze-0.0.6/src/yze/mutant_odds_of_pushing.py
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-05-30 20:56:10.199587 yze-0.0.6/src/yze.egg-info/
--rw-r--r--   0 nicolas    (501) staff       (20)     4899 2023-05-30 20:56:10.000000 yze-0.0.6/src/yze.egg-info/PKG-INFO
--rw-r--r--   0 nicolas    (501) staff       (20)      303 2023-05-30 20:56:10.000000 yze-0.0.6/src/yze.egg-info/SOURCES.txt
--rw-r--r--   0 nicolas    (501) staff       (20)        1 2023-05-30 20:56:10.000000 yze-0.0.6/src/yze.egg-info/dependency_links.txt
--rw-r--r--   0 nicolas    (501) staff       (20)      120 2023-05-30 20:56:10.000000 yze-0.0.6/src/yze.egg-info/entry_points.txt
--rw-r--r--   0 nicolas    (501) staff       (20)        4 2023-05-30 20:56:10.000000 yze-0.0.6/src/yze.egg-info/top_level.txt
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-05-30 20:56:10.199710 yze-0.0.6/tests/
--rw-r--r--   0 nicolas    (501) staff       (20)     3611 2023-05-30 10:50:59.000000 yze-0.0.6/tests/test_yze_dice.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-06-05 08:10:13.891122 yze-0.0.7/
+-rw-r--r--   0 nicolas    (501) staff       (20)     6004 2023-06-05 08:10:13.891013 yze-0.0.7/PKG-INFO
+-rw-r--r--   0 nicolas    (501) staff       (20)     5506 2023-06-05 08:07:21.000000 yze-0.0.7/README.md
+-rw-r--r--   0 nicolas    (501) staff       (20)      735 2023-06-05 08:08:59.000000 yze-0.0.7/pyproject.toml
+-rw-r--r--   0 nicolas    (501) staff       (20)       38 2023-06-05 08:10:13.891151 yze-0.0.7/setup.cfg
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-06-05 08:10:13.889110 yze-0.0.7/src/
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-06-05 08:10:13.889961 yze-0.0.7/src/yze/
+-rw-r--r--   0 nicolas    (501) staff       (20)        0 2023-05-23 06:35:38.000000 yze-0.0.7/src/yze/__init__.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     7883 2023-06-05 08:02:09.000000 yze-0.0.7/src/yze/benchmark_mutant.py
+-rw-r--r--   0 nicolas    (501) staff       (20)    17913 2023-05-30 10:50:59.000000 yze-0.0.7/src/yze/dice.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     5161 2023-05-30 20:51:44.000000 yze-0.0.7/src/yze/mutant_odds_of_pushing.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-06-05 08:10:13.890631 yze-0.0.7/src/yze.egg-info/
+-rw-r--r--   0 nicolas    (501) staff       (20)     6004 2023-06-05 08:10:13.000000 yze-0.0.7/src/yze.egg-info/PKG-INFO
+-rw-r--r--   0 nicolas    (501) staff       (20)      303 2023-06-05 08:10:13.000000 yze-0.0.7/src/yze.egg-info/SOURCES.txt
+-rw-r--r--   0 nicolas    (501) staff       (20)        1 2023-06-05 08:10:13.000000 yze-0.0.7/src/yze.egg-info/dependency_links.txt
+-rw-r--r--   0 nicolas    (501) staff       (20)      120 2023-06-05 08:10:13.000000 yze-0.0.7/src/yze.egg-info/entry_points.txt
+-rw-r--r--   0 nicolas    (501) staff       (20)        4 2023-06-05 08:10:13.000000 yze-0.0.7/src/yze.egg-info/top_level.txt
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-06-05 08:10:13.890745 yze-0.0.7/tests/
+-rw-r--r--   0 nicolas    (501) staff       (20)     3611 2023-05-30 10:50:59.000000 yze-0.0.7/tests/test_yze_dice.py
```

### Comparing `yze-0.0.6/PKG-INFO` & `yze-0.0.7/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: yze
-Version: 0.0.6
-Summary: A small package to handle YZE games mechanics
-Author-email: Nicolas Legrand <nicolas.legrand@gmail.com>
-Project-URL: Homepage, https://github.com/nlegrand/yze
-Project-URL: Bug Tracker, https://github.com/nlegrand/yze/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: ISC License (ISCL)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-
 The main goal of this Python library is to propose an object to emulate
 Year Zero Engine dice throwing.
 
 # What is it about?
 
 The Year Zero Engine is a very nice Roleplaying Game system created by
 the terrific Tomas Härenstam at [Free League
@@ -29,14 +16,18 @@
 # System supported:
 - [X] Mutant: Year Zero
 - [X] Forbidden Lands
 - [X] Twilight 2000
 - [X] Alien
 - [X] Blade Runner
 
+# TODO
+
+- [ ] negative dice for MYZ and FBL
+
 # Example
 ```
 . my_py_venv/bin/activate
 git clone https://github.com/nlegrand/yze.git
 cd yze
 python -m pip install -e .
 python
@@ -112,14 +103,16 @@
 
 Running multiple times produce different odds, but in the same order.
 
 # Benchmark
 You can also benchmark dice throw to see what are your chances to get
 some successes or damage.
 
+## Simple command
+
 ```
 $ benchmark_mutant  -a 4 -s 2 -g 2
 Throwing dice pool (attribute: 4, skill: 2, gear: 2) 100000 times !
 at least one success: 76.791 %
 at least on pushed succes: 93.235 %
 at least one damage to attribute: 73.079 %
 at least one damage to gear: 47.882 %
@@ -147,7 +140,23 @@
     chances to get 4: 0.565 %
 Gear damage:
     chances to get 1: 40.233 %
     chances to get 2: 7.649 %
 
 ```
 
+## Complet out
+
+You can have a rather complete output giving you percentage of success
+after multiple rolls (default 100000). The table is rather long so I
+have abbreviated the column names : s. is for successes, p. for pushed
+and d. for damage. alo is for at least one.
+
+    benchmark_mutant -c
+    Attr	Skill	Gear	alo s.	alo p.	alo attr d.	alo gear d.	1 s.	2 s.	3 s.	4 s.	5 s.	6 s.	7 s.	8 s.	9 s.	10 s.	1 p. s.	2 p. s.	3 p. s.	4 p. s.	5 p. s.	6 p. s.	7 p. s.	8 p. s.	9 p. s.	10 p. s.	11 p. s.	12 p. s.	1 attr. d.	2 attr. d.	3 attr. d.	4 attr. d.	5 attr. d.	6 attr. d.	1 gear d.	2 gear d.	3 gear d.
+    1	0	0	16.528 	27.636 	28.133	0.0	16.528										27.636									28.133								
+    1	0	1	30.459 	47.757 	27.962	27.701	27.671	2.788									40.042	7.715								27.962						27.701
+    1	0	2	42.234 	62.36 	27.735	47.801	34.803	6.949	0.482								43.256	17.042	2.062							27.735						40.079	7.722
+    ...
+
+You can consult a version of this output on
+[github](https://github.com/nlegrand/yze/blob/main/files/mutant_complete_benchmark.tsv).
```

### Comparing `yze-0.0.6/src/yze/benchmark_mutant.py` & `yze-0.0.7/src/yze/mutant_odds_of_pushing.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,51 +12,34 @@
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
 # OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 from yze.dice import MutantDicePool
 import argparse
-import pprint
-import logging, sys, os
 
-DEBUG=os.getenv('DEBUG')
-loglevel = logging.INFO
-if DEBUG:
-    loglevel = logging.DEBUG
-logging.basicConfig(stream=sys.stderr, level=loglevel)
-
-
-def multiple_throws(throws=10000, attribute=1, skill=0, gear=0):
+def multiple_throws(attribute, skill, gear, throws=100000):
     """Throw dice <throws> times, store results in <results>, return
     results.
     """
     results = {
-        'atleast_one': 0,
         'atleast_one_pushed': 0,
         'atleast_one_attr_botch': 0,
         'atleast_one_gear_botch': 0,
-        'successes': {},
         'pushed_successes': {},
         'attribute_botched': {},
         'gear_botched': {},
     }
     
-    print(f'Throwing dice pool (attribute: {attribute}, skill: {skill}, gear: {gear}) {throws} times !')
+    print(f'Throwing dice {throws} times !')
     for i in range(int(throws)):
-        d = MutantDicePool(attr=int(attribute), skill=int(skill), gear=int(gear))
-        res = d.throw()
+        d = MutantDicePool(attr=len(attribute), skill=len(skill), gear=len(gear))
+        d.thrown = True
+        d.result = {'attr': attribute, 'skill': skill, 'gear': gear}
         pushed_res = d.push()
-        successes = [x for x in d.result['attr'] + d.result['skill'] + d.result['gear'] if x == 6]
-        if len(successes) > 0:
-            results['atleast_one'] += 1
-            if len(successes) not in results['successes']:
-                results['successes'][len(successes)] = 1
-            else:
-                results['successes'][len(successes)] += 1
         pushed_successes = [x for x in d.pushed_res['attr'] + d.pushed_res['skill'] + d.pushed_res['gear'] if x == 6]
         if len(pushed_successes) > 0:
             results['atleast_one_pushed'] += 1
             if len(pushed_successes) not in results['pushed_successes']:
                 results['pushed_successes'][len(pushed_successes)] = 1
             else:
                 results['pushed_successes'][len(pushed_successes)] += 1
@@ -72,60 +55,64 @@
             results['atleast_one_gear_botch'] += 1
             if len(gear_botched) not in results['gear_botched']:
                 results['gear_botched'][len(gear_botched)] = 1
             else:
                 results['gear_botched'][len(gear_botched)] += 1
     return results
 
-
-def complete_benchmark():
-    """In dev yet, will launch multiple multiple_throws so as to try
-    to have almost exhaustive benchmarks.
-
-    """
-    pass
-def print_result(result_name, result, throws):
-    """Pretty print result to terminal
-    """
-    print (f'{result_name}: {result * 100 / throws} %')
-
-def print_result_list(result_list_name, result_list, throws):
-    """Pretty print the full result list
-    """
-    print(f'{result_list_name}:')
-    for key in sorted(result_list):
-        print(f'    chances to get {key}: {result_list[key] * 100 / throws} %')
-
+def unpack(args):
+    unpacked = []
+    for att in args:
+        att = int(att)
+        if (att == 0):
+            next;
+        elif ( 1 <= att <= 6 ):
+            unpacked.append(att)
+        else:
+            raise ValueError(f"got {att} should has been int between 0 and 6")
+    return unpacked
 
 def main():
     """Fetch args from the commandline and proceed.
     """
     parser = argparse.ArgumentParser(
-                        prog='benchmark_mutant',
-                        description='make a lot of YZE rolls so as to have an idea of chances of success',
-                        epilog='')
+                        prog='mutant_odds_of_pushing',
+                        description="""Once you get a result, what are your odds when pushing it?
+                        feed this command your results and see what is likely or not to happen""",
+                        epilog="""Experimental probabilities made with pseudo random numbers.
+                        Maybe it’s not the best you can get :).""")
 
     parser.add_argument('-t', '--throws', default=100000)      # option that takes a value
-    parser.add_argument('-a', '--attribute', default=1)
-    parser.add_argument('-s', '--skill', default=0)
-    parser.add_argument('-g', '--gear', default=0)
-    parser.add_argument('-c', '--complete', action='store_true')
+    parser.add_argument('-a', '--attribute_dice',
+                        help="List your dice results eg: 253",
+                        required=True)
+    parser.add_argument('-s', '--skill_dice',
+                        default=0,
+                        help="List your dice results eg: 45")
+    parser.add_argument('-g', '--gear_dice',
+                        default=0,
+                        help="List your dice results eg: 32")
 
     args = parser.parse_args()
+
+    attribute_res = unpack(args.attribute_dice)
+    skill_res = unpack(args.skill_dice)
+    gear_res = unpack(args.gear_dice)
+
     throws = int(args.throws)
 
-    if args.complete:
-        print("Complete benchmark not implemented yet, sorry!")
-    else:
-        results = multiple_throws(throws, args.attribute, args.skill, args.gear)
-        print_result('at least one success', results['atleast_one'], throws)
-        print_result('at least on pushed succes', results['atleast_one_pushed'], throws)
-        print_result('at least one damage to attribute', results['atleast_one_attr_botch'], throws)
-        print_result('at least one damage to gear', results['atleast_one_gear_botch'], throws)
-        print_result_list('Successes on first roll', results['successes'], throws)
-        print_result_list('Successes on pushed roll', results['pushed_successes'], throws)
-        print_result_list('Attribute damage', results['attribute_botched'], throws)
-        print_result_list('Gear damage', results['gear_botched'], throws)
-        logging.debug(results)
+    results = multiple_throws(attribute_res, skill_res, gear_res,throws=throws)
+
+    print ("Odds of having:")
+    print (f"    -at least one success: {results['atleast_one_pushed'] * 100 / throws} %")
+    print (f"    -at least one attr botch: {results['atleast_one_attr_botch'] * 100 / throws} %")
+    print (f"    -at least one gear botch: {results['atleast_one_gear_botch'] * 100 / throws} %")
+    for key in sorted(results['pushed_successes']):
+        print (f"    - {key} successes: {results['pushed_successes'][key] * 100 / throws} %")
+    for key in sorted(results['attribute_botched']):
+        print (f"    - {key} attribute botchs: {results['attribute_botched'][key] * 100 / throws} %")
+    for key in sorted(results['gear_botched']):
+        print (f"    - {key} gear botchs: {results['gear_botched'][key] * 100 / throws} %")
+
 
 if __name__ == "__main__":
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `yze-0.0.6/src/yze/dice.py` & `yze-0.0.7/src/yze/dice.py`

 * *Files identical despite different names*

### Comparing `yze-0.0.6/src/yze.egg-info/PKG-INFO` & `yze-0.0.7/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yze
-Version: 0.0.6
+Version: 0.0.7
 Summary: A small package to handle YZE games mechanics
 Author-email: Nicolas Legrand <nicolas.legrand@gmail.com>
 Project-URL: Homepage, https://github.com/nlegrand/yze
 Project-URL: Bug Tracker, https://github.com/nlegrand/yze/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
@@ -29,14 +29,18 @@
 # System supported:
 - [X] Mutant: Year Zero
 - [X] Forbidden Lands
 - [X] Twilight 2000
 - [X] Alien
 - [X] Blade Runner
 
+# TODO
+
+- [ ] negative dice for MYZ and FBL
+
 # Example
 ```
 . my_py_venv/bin/activate
 git clone https://github.com/nlegrand/yze.git
 cd yze
 python -m pip install -e .
 python
@@ -112,14 +116,16 @@
 
 Running multiple times produce different odds, but in the same order.
 
 # Benchmark
 You can also benchmark dice throw to see what are your chances to get
 some successes or damage.
 
+## Simple command
+
 ```
 $ benchmark_mutant  -a 4 -s 2 -g 2
 Throwing dice pool (attribute: 4, skill: 2, gear: 2) 100000 times !
 at least one success: 76.791 %
 at least on pushed succes: 93.235 %
 at least one damage to attribute: 73.079 %
 at least one damage to gear: 47.882 %
@@ -147,7 +153,23 @@
     chances to get 4: 0.565 %
 Gear damage:
     chances to get 1: 40.233 %
     chances to get 2: 7.649 %
 
 ```
 
+## Complet out
+
+You can have a rather complete output giving you percentage of success
+after multiple rolls (default 100000). The table is rather long so I
+have abbreviated the column names : s. is for successes, p. for pushed
+and d. for damage. alo is for at least one.
+
+    benchmark_mutant -c
+    Attr	Skill	Gear	alo s.	alo p.	alo attr d.	alo gear d.	1 s.	2 s.	3 s.	4 s.	5 s.	6 s.	7 s.	8 s.	9 s.	10 s.	1 p. s.	2 p. s.	3 p. s.	4 p. s.	5 p. s.	6 p. s.	7 p. s.	8 p. s.	9 p. s.	10 p. s.	11 p. s.	12 p. s.	1 attr. d.	2 attr. d.	3 attr. d.	4 attr. d.	5 attr. d.	6 attr. d.	1 gear d.	2 gear d.	3 gear d.
+    1	0	0	16.528 	27.636 	28.133	0.0	16.528										27.636									28.133								
+    1	0	1	30.459 	47.757 	27.962	27.701	27.671	2.788									40.042	7.715								27.962						27.701
+    1	0	2	42.234 	62.36 	27.735	47.801	34.803	6.949	0.482								43.256	17.042	2.062							27.735						40.079	7.722
+    ...
+
+You can consult a version of this output on
+[github](https://github.com/nlegrand/yze/blob/main/files/mutant_complete_benchmark.tsv).
```

### Comparing `yze-0.0.6/tests/test_yze_dice.py` & `yze-0.0.7/tests/test_yze_dice.py`

 * *Files identical despite different names*

