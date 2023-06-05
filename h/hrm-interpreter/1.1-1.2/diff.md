# Comparing `tmp/hrm-interpreter-1.1.tar.gz` & `tmp/hrm-interpreter-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hrm-interpreter-1.1.tar", last modified: Wed Oct  5 15:17:39 2022, max compression
+gzip compressed data, was "hrm-interpreter-1.2.tar", last modified: Mon Jun  5 13:55:37 2023, max compression
```

## Comparing `hrm-interpreter-1.1.tar` & `hrm-interpreter-1.2.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2022-10-05 15:17:39.127353 hrm-interpreter-1.1/
--rw-rw-r--   0 franck    (1000) franck    (1000)     1073 2022-04-04 16:49:30.000000 hrm-interpreter-1.1/LICENSE
--rw-rw-r--   0 franck    (1000) franck    (1000)     1305 2022-10-05 15:17:39.127353 hrm-interpreter-1.1/PKG-INFO
--rw-rw-r--   0 franck    (1000) franck    (1000)     5402 2022-10-05 09:30:47.000000 hrm-interpreter-1.1/README.md
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2022-10-05 15:17:39.127353 hrm-interpreter-1.1/hrm/
--rw-rw-r--   0 franck    (1000) franck    (1000)     6679 2022-10-05 15:17:18.000000 hrm-interpreter-1.1/hrm/__init__.py
--rw-rw-r--   0 franck    (1000) franck    (1000)     3866 2022-10-05 13:41:34.000000 hrm-interpreter-1.1/hrm/__main__.py
--rw-rw-r--   0 franck    (1000) franck    (1000)    28361 2022-04-05 17:21:40.000000 hrm-interpreter-1.1/hrm/levels.json
--rw-rw-r--   0 franck    (1000) franck    (1000)     2360 2022-04-06 13:12:22.000000 hrm-interpreter-1.1/hrm/parse.py
--rw-rw-r--   0 franck    (1000) franck    (1000)     3666 2022-04-06 14:33:57.000000 hrm-interpreter-1.1/hrm/tikz.py
-drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2022-10-05 15:17:39.127353 hrm-interpreter-1.1/hrm_interpreter.egg-info/
--rw-rw-r--   0 franck    (1000) franck    (1000)     1305 2022-10-05 15:17:39.000000 hrm-interpreter-1.1/hrm_interpreter.egg-info/PKG-INFO
--rw-rw-r--   0 franck    (1000) franck    (1000)      345 2022-10-05 15:17:39.000000 hrm-interpreter-1.1/hrm_interpreter.egg-info/SOURCES.txt
--rw-rw-r--   0 franck    (1000) franck    (1000)        1 2022-10-05 15:17:39.000000 hrm-interpreter-1.1/hrm_interpreter.egg-info/dependency_links.txt
--rw-rw-r--   0 franck    (1000) franck    (1000)       44 2022-10-05 15:17:39.000000 hrm-interpreter-1.1/hrm_interpreter.egg-info/entry_points.txt
--rw-rw-r--   0 franck    (1000) franck    (1000)        9 2022-10-05 15:17:39.000000 hrm-interpreter-1.1/hrm_interpreter.egg-info/requires.txt
--rw-rw-r--   0 franck    (1000) franck    (1000)        4 2022-10-05 15:17:39.000000 hrm-interpreter-1.1/hrm_interpreter.egg-info/top_level.txt
--rw-rw-r--   0 franck    (1000) franck    (1000)       79 2022-10-05 15:17:39.127353 hrm-interpreter-1.1/setup.cfg
--rw-rw-r--   0 franck    (1000) franck    (1000)     1105 2022-04-07 10:43:03.000000 hrm-interpreter-1.1/setup.py
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-06-05 13:55:37.012182 hrm-interpreter-1.2/
+-rw-rw-r--   0 franck    (1000) franck    (1000)     1073 2022-04-04 16:49:30.000000 hrm-interpreter-1.2/LICENSE
+-rw-rw-r--   0 franck    (1000) franck    (1000)     1324 2023-06-05 13:55:37.012182 hrm-interpreter-1.2/PKG-INFO
+-rw-rw-r--   0 franck    (1000) franck    (1000)     5402 2022-10-05 09:30:47.000000 hrm-interpreter-1.2/README.md
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-06-05 13:55:37.012182 hrm-interpreter-1.2/hrm/
+-rw-rw-r--   0 franck    (1000) franck    (1000)     8312 2023-06-05 13:47:53.000000 hrm-interpreter-1.2/hrm/__init__.py
+-rw-rw-r--   0 franck    (1000) franck    (1000)     4117 2022-11-29 15:34:01.000000 hrm-interpreter-1.2/hrm/__main__.py
+-rw-rw-r--   0 franck    (1000) franck    (1000)    28361 2022-04-05 17:21:40.000000 hrm-interpreter-1.2/hrm/levels.json
+-rw-rw-r--   0 franck    (1000) franck    (1000)     2362 2023-06-05 13:28:27.000000 hrm-interpreter-1.2/hrm/parse.py
+-rw-rw-r--   0 franck    (1000) franck    (1000)     3666 2022-04-06 14:33:57.000000 hrm-interpreter-1.2/hrm/tikz.py
+drwxrwxr-x   0 franck    (1000) franck    (1000)        0 2023-06-05 13:55:37.012182 hrm-interpreter-1.2/hrm_interpreter.egg-info/
+-rw-rw-r--   0 franck    (1000) franck    (1000)     1324 2023-06-05 13:55:36.000000 hrm-interpreter-1.2/hrm_interpreter.egg-info/PKG-INFO
+-rw-rw-r--   0 franck    (1000) franck    (1000)      307 2023-06-05 13:55:36.000000 hrm-interpreter-1.2/hrm_interpreter.egg-info/SOURCES.txt
+-rw-rw-r--   0 franck    (1000) franck    (1000)        1 2023-06-05 13:55:36.000000 hrm-interpreter-1.2/hrm_interpreter.egg-info/dependency_links.txt
+-rw-rw-r--   0 franck    (1000) franck    (1000)       44 2023-06-05 13:55:36.000000 hrm-interpreter-1.2/hrm_interpreter.egg-info/entry_points.txt
+-rw-rw-r--   0 franck    (1000) franck    (1000)        4 2023-06-05 13:55:36.000000 hrm-interpreter-1.2/hrm_interpreter.egg-info/top_level.txt
+-rw-rw-r--   0 franck    (1000) franck    (1000)       79 2023-06-05 13:55:37.012182 hrm-interpreter-1.2/setup.cfg
+-rw-rw-r--   0 franck    (1000) franck    (1000)     1079 2023-06-05 13:48:49.000000 hrm-interpreter-1.2/setup.py
```

### Comparing `hrm-interpreter-1.1/LICENSE` & `hrm-interpreter-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hrm-interpreter-1.1/PKG-INFO` & `hrm-interpreter-1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: hrm-interpreter
-Version: 1.1
+Version: 1.2
 Summary: Minimalist Human Resource Machine interpreter
 Home-page: https://github.com/fpom/hrm
 Author: Franck Pommereau
 Author-email: franck.pommereau@univ-evry.fr
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Interpreters
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
+Requires: colorama
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Human Resource Machine interpreter
 
 This is a Python interpreter for programs from the [Human Resource Machine](http://tomorrowcorporation.com/humanresourcemachine) game from [Tomorrow Corporation](http://tomorrowcorporation.com).
```

### Comparing `hrm-interpreter-1.1/README.md` & `hrm-interpreter-1.2/README.md`

 * *Files identical despite different names*

### Comparing `hrm-interpreter-1.1/hrm/__init__.py` & `hrm-interpreter-1.2/hrm/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # coding: utf-8
 
-VERSION = "1.1"
+VERSION = "1.2"
 
-import functools, pathlib, json
-from collections import deque
+import functools, pathlib, json, inspect
 
 from colorama import Fore as F, Back as B, Style as S
 
 from .parse import parse
 
 colors = {"inbox" : F.GREEN,
           "outbox" : F.GREEN,
@@ -23,62 +22,57 @@
 op_width = max(len(v) for v in colors)
 
 def log (method) :
     name = method.__name__[3:]
     @functools.wraps(method)
     def wrapper (self, *args) :
         if self.verbose :
-            pre = dict(self.tiles)
-            pre["ip"] = self.ip
-            pre["hands"] = self.hands
-            pre["inbox"] = len(self.inbox)
-            pre["outbox"] = len(self.outbox)
+            self.update = {"inbox" : len(self.inbox),
+                           "outbox" : len(self.outbox)}
         err = None
         try :
             ret = method(self, *args)
         except AssertionError as exc :
             err = exc
         if self.verbose :
-            post = []
-            hands = False
-            for addr in range(max(self.tiles, default=-1) + 1) :
-                if (be := pre.get(addr, None)) != (af := self.tiles.get(addr, None)) :
-                    post.append(f"🔢 {addr}={af}")
-            if len(self.inbox) != pre["inbox"] :
-                post.append(f"📤 {self.hands}")
-                hands = True
-            if len(self.outbox) != pre["outbox"] :
-                post.append(f"📥 {self.outbox[-1]}")
-            if hands or self.hands != pre["hands"] :
-                post.append(f"😬 {self.hands if self.hands is not None else ''}")
-            if pre["ip"] != self.ip :
-                post.append(f"👉 {self.ip}")
             head = (colors[name]
                     + " ".join([name] + [str(a) for a in args]).ljust(op_width + 3)
                     + S.RESET_ALL)
             if err :
                 print(head, f"😡 {err}")
             elif ret is True :
                 print(head, "🛑")
-            elif post :
-                print(head, " / ".join(post))
             else :
-                print(head)
+                post = []
+                for key, val in self.update.items() :
+                    if key == "inbox" and len(self.inbox) != val :
+                        post.append(f"📤 {self.hands}")
+                    elif key == "outbox" and len(self.outbox) != val :
+                        post.append(f"📥 {self.outbox[-1]}")
+                    elif isinstance(key, int) :
+                        post.append(f"🔢 {key}←{val}")
+                    elif key == "ip" :
+                        post.append(f"👉 {self.ip}")
+                    elif key == "hands" :
+                        post.append(f"😬 {self.hands if self.hands is not None else ''}")
+                print(head, " / ".join(post))
         if err is not None :
             raise err
         else :
             return ret
     return wrapper
 
 class HRM (object) :
-    def __init__ (self, prog) :
+    def __init__ (self, prog, labels) :
         self.prog = tuple(prog)
+        self.labels = dict(labels)
+        self.check()
     @classmethod
     def parse (cls, src) :
-        return cls(parse(src))
+        return cls(*parse(src))
     def level (self, level) :
         path = pathlib.Path(__file__).parent / "levels.json"
         for lvl in json.load(path.open()) :
             if lvl["number"] == level :
                 return lvl
     def runlevel (self, level, example=0, verbose=False) :
         if isinstance(level, int) :
@@ -86,106 +80,147 @@
         if "floor" in level and "tiles" in level["floor"] :
             floor = level["floor"]["tiles"]
         else :
             floor = []
         return self(level["examples"][example]["inbox"], floor, verbose)
     def __call__ (self, inbox, floor=[], verbose=False) :
         self.verbose = verbose
-        self.ip = 0
+        self.state = {"ip" : 0, "hands" : None}
         if isinstance(floor, dict) :
-            self.tiles = {int(k) : v for k, v in floor.items()}
+            self.state.update((int(k), v) for k, v in floor.items())
         else :
-            self.tiles = dict(enumerate(floor))
-        self.inbox = deque(inbox)
+            self.state.update(enumerate(floor))
+        self.inbox = list(inbox)
         self.outbox = []
-        self.hands = None
         while True :
             if self.ip >= len(self.prog) :
                 break
             op, *args = self.prog[self.ip]
             self.ip += 1
             handler = getattr(self, f"op_{op.lower()}")
             if handler(*args) :
                 break
         return self.outbox
+    @property
+    def ip (self) :
+        return self["ip"]
+    @ip.setter
+    def ip (self, value) :
+        self["ip"] = value
+    @property
+    def hands (self) :
+        return self["hands"]
+    @hands.setter
+    def hands (self, value) :
+        self["hands"] = value
     def __getitem__ (self, addr) :
-        if isinstance(addr, int) :
-            assert self.tiles.get(addr, None) is not None, f"tile {addr} is empty"
-            return self.tiles[addr]
-        elif isinstance(addr, list) :
-            assert len(addr)==1 and isinstance(addr[0], int), f"invalid address {addr!r}"
+        if addr == "ip" :
+            return self.state["ip"]
+        elif addr == "hands" :
+            return self.state["hands"]
+        elif isinstance(addr, int) :
+            assert self.state.get(addr, None) is not None, f"tile {addr} is empty"
+            return self.state[addr]
+        elif isinstance(addr, list) and len(addr) == 1 and isinstance(addr[0], int) :
             return self[self[addr[0]]]
         else :
             raise ValueError(f"invalid address {addr!r}")
     def __setitem__ (self, addr, value) :
-        if isinstance(addr, int) :
-            self.tiles[addr] = value
-        elif isinstance(addr, list) :
-            self[self[addr[0]]] = value
+        update = getattr(self, "update", {})
+        if addr == "ip" :
+            self.state["ip"] = update["ip"] = value
+        elif addr == "hands" :
+            self.state["hands"] = update["hands"] = value
+        elif isinstance(addr, int) :
+            self.state[addr] = update[addr] = value
+        elif isinstance(addr, list) and len(addr) == 1 and isinstance(addr[0], int) :
+            a = self[addr[0]]
+            self[a] = update[a] = value
         else :
             raise ValueError(f"invalid address {addr!r}")
+    def check(self):
+        for op, *args in self.prog:
+            fun = getattr(self, f"op_{op.lower()}", None)
+            assert fun is not None, f"unknown operation {op}"
+            sig = inspect.signature(fun)
+            try:
+                bound = sig.bind(*args)
+            except TypeError:
+                assert False, f"invalid arguments for {op}: {args}"
+            for name, value in bound.arguments.items():
+                annot = sig.parameters[name].annotation
+                assert isinstance(value, annot), f"invalid argument for {op}: {value}"
+                if annot is str:
+                    assert value in self.labels, f"undefined label {value}"
     @log
     def op_inbox (self) :
         if self.inbox :
-            self.hands = self.inbox.popleft()
+            self.hands = self.inbox.pop(0)
         else :
             return True
     @log
     def op_outbox (self) :
         assert self.hands is not None, f"you don't hold any value"
         self.outbox.append(self.hands)
         self.hands = None
     @log
-    def op_copyfrom (self, addr) :
+    def op_copyfrom (self, addr: int) :
         self.hands = self[addr]
     @log
-    def op_copyto (self, addr) :
+    def op_copyto (self, addr: int) :
+        assert self.hands is not None, f"you don't hold any value"
         self[addr] = self.hands
     @log
-    def op_add (self, addr) :
+    def op_add (self, addr: int) :
         assert self.hands is not None, f"you don't hold any value"
         assert isinstance(self.hands, int), f"cannot add to value {self.hands!r}"
         val = self[addr]
         assert isinstance(val, int), f"cannot add value {val!r}"
         self.hands += val
     @log
-    def op_sub (self, addr) :
+    def op_sub (self, addr: int) :
         assert self.hands is not None, f"you don't hold any value"
         val = self[addr]
         if isinstance(self.hands, int) and isinstance(val, int) :
             self.hands -= val
         elif isinstance(self.hands, str) and isinstance(val, str) :
             self.hands = ord(self.hands) - ord(val)
         else :
             assert False, f"cannot sub {val!r} from {self.hands!r}"
     @log
-    def op_bumpup (self, addr) :
+    def op_bumpup (self, addr: int) :
         val = self[addr]
         assert isinstance(val, int), f"cannot increment value {self.hands!r}"
         self.hands = self[addr] = val + 1
     @log
-    def op_bumpdn (self, addr) :
+    def op_bumpdn (self, addr: int) :
         val = self[addr]
         assert isinstance(val, int), f"cannot decrement value {self.hands!r}"
         self.hands = self[addr] = val - 1
     @log
-    def op_jump (self, pos) :
+    def op_jump (self, lbl: str) :
+        assert lbl in self.labels, f"labels {lbl} is not defined"
+        pos = self.labels[lbl]
         assert 0 <= pos <= len(self.prog), f"invalid program position"
         if pos == len(self.prog) :
             return True
         self.ip = pos
     @log
-    def op_jumpz (self, pos) :
+    def op_jumpz (self, lbl: str) :
+        assert lbl in self.labels, f"labels {lbl} is not defined"
+        pos = self.labels[lbl]
         assert self.hands is not None, f"you don't hold any value"
         assert 0 <= pos <= len(self.prog), f"invalid program position"
         if self.hands == 0 :
             if pos == len(self.prog) :
                 return True
             self.ip = pos
     @log
-    def op_jumpn (self, pos) :
+    def op_jumpn (self, lbl: str) :
+        assert lbl in self.labels, f"labels {lbl} is not defined"
+        pos = self.labels[lbl]
         assert self.hands is not None, f"you don't hold any value"
         assert 0 <= pos <= len(self.prog), f"invalid program position"
         if self.hands < 0 :
             if pos == len(self.prog) :
                 return True
             self.ip = pos
```

### Comparing `hrm-interpreter-1.1/hrm/__main__.py` & `hrm-interpreter-1.2/hrm/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,14 +24,16 @@
                     help="export program as a PDF image")
 parser.add_argument("-l", dest="latex", type=str, default=None, action="store",
                     help="export program as a LaTeX/TikZ file")
 parser.add_argument("-i", dest="inbox", type=str, default=None, action="store",
                     help="run with INBOX given as comma-separated values")
 parser.add_argument("-n", dest="numeric", default=False, action="store_true",
                     help="generate INBOX with only numeric values")
+parser.add_argument("-N", dest="positive", default=False, action="store_true",
+                    help="generate INBOX with no negative values")
 parser.add_argument("-s", dest="size", type=int, default=None, action="store",
                     help="generate INBOX with SIZE values")
 parser.add_argument("-t", dest="tiles", type=str, default=None, action="store",
                     help="run with TILES given as comma-separated values")
 parser.add_argument("-q", dest="quit", default=False, action="store_true",
                     help="quit interpreter without running the program")
 parser.add_argument("prog", type=str, metavar="PROG", action="store",
@@ -64,18 +66,22 @@
             else :
                 try :
                     inbox[i] = int(v)
                 except :
                     parser.exit(2, f"invalid inbox value {v!r}")
     else :
         size = args.size or random.randint(10,20)
+        if args.positive :
+            MIN, MAX = 0, 20
+        else :
+            MIN, MAX = -20, 20
         if args.numeric :
-            inbox = [random.randint(-20,20) for _ in range(size)]
+            inbox = [random.randint(MIN,MAX) for _ in range(size)]
         else :
-            inbox = [random.choice(list(range(-20, 21)) + list(string.ascii_uppercase))
+            inbox = [random.choice(list(range(MIN,MAX+1)) + list(string.ascii_uppercase))
                      for _ in range(size)]
 
     if args.tiles :
         tiles = args.tiles.split(",")
         for i, v in enumerate(tiles) :
             if not v :
                 tiles[i] = None
```

### Comparing `hrm-interpreter-1.1/hrm/levels.json` & `hrm-interpreter-1.2/hrm/levels.json`

 * *Files identical despite different names*

### Comparing `hrm-interpreter-1.1/hrm/parse.py` & `hrm-interpreter-1.2/hrm/parse.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         elif not line :
             continue
         elif toks and toks[0].lower() == "define" :
             skip = True
         elif line.startswith("--") or (toks and toks[0].lower() == "comment") :
             continue
         elif line.endswith(":") :
-            lbl = line[:-1]
+            lbl = line[:-1].strip()
             assert lbl not in labels, (f"[{num}] parse error:"
                                        f" duplicate label {raw!r}")
             labels.add(lbl)
             yield num, "lbl", lbl
         else :
             assert toks and (toks[0].lower() in ops), (f"[{num}] parse error:"
                                                        f" unknown operation {raw!r}")
@@ -49,20 +49,20 @@
             labels[obj] = len(prog)
         elif kind == "op" :
             op, *args = obj
             prog.append((num, [op] + args))
     for pos, (num, cmd) in enumerate(prog) :
         for i, a in enumerate(cmd[1:], start=1) :
             if a in labels :
-                cmd[i] = labels[a]
+                pass
             elif a.startswith("[") and a.endswith("]") :
                 try :
                     cmd[i] = [int(a[1:-1])]
                 except :
                     assert False, f"[{num}] parse error: invalid integer {a[1:-1]!r}"
             else :
                 try :
                     cmd[i] = int(a)
                 except :
                     assert False, f"[{num}] parse error: invalid integer {a!r}"
         prog[pos] = cmd
-    return prog
+    return prog, labels
```

### Comparing `hrm-interpreter-1.1/hrm/tikz.py` & `hrm-interpreter-1.2/hrm/tikz.py`

 * *Files identical despite different names*

### Comparing `hrm-interpreter-1.1/hrm_interpreter.egg-info/PKG-INFO` & `hrm-interpreter-1.2/hrm_interpreter.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: hrm-interpreter
-Version: 1.1
+Version: 1.2
 Summary: Minimalist Human Resource Machine interpreter
 Home-page: https://github.com/fpom/hrm
 Author: Franck Pommereau
 Author-email: franck.pommereau@univ-evry.fr
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Interpreters
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
+Requires: colorama
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Human Resource Machine interpreter
 
 This is a Python interpreter for programs from the [Human Resource Machine](http://tomorrowcorporation.com/humanresourcemachine) game from [Tomorrow Corporation](http://tomorrowcorporation.com).
```

### Comparing `hrm-interpreter-1.1/setup.py` & `hrm-interpreter-1.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
-import hrm
-
 readme = (Path(__file__).parent / "README.md").read_text(encoding="utf-8")
 
 setup(name="hrm-interpreter",
-      version=hrm.VERSION,
+      version="1.2",
       description="Minimalist Human Resource Machine interpreter",
       long_description=readme.split("##")[0].strip(),
       long_description_content_type="text/markdown",
       licence="MIT",
       url="https://github.com/fpom/hrm",
       author="Franck Pommereau",
       author_email="franck.pommereau@univ-evry.fr",
@@ -18,10 +16,10 @@
                    "Intended Audience :: Developers",
                    "Topic :: Software Development :: Interpreters",
                    "License :: OSI Approved :: MIT License",
                    "Programming Language :: Python :: 3.8",
                    "Operating System :: OS Independent"],
       packages=find_packages(where="."),
       python_requires=">=3.8",
-      install_requires=["colorama"],
+      requires=["colorama"],
       package_data={"" : ["*.json"]},
       entry_points={"console_scripts": ["hrmi=hrm.__main__:main"]})
```

