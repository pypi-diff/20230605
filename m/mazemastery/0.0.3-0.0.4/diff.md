# Comparing `tmp/mazemastery-0.0.3.tar.gz` & `tmp/mazemastery-0.0.4.tar.gz`

## Comparing `mazemastery-0.0.3.tar` & `mazemastery-0.0.4.tar`

### file list

```diff
@@ -1,41 +1,42 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/__init__.py
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/api.py
--rw-r--r--   0        0        0     6828 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/debug_menu.py
--rw-r--r--   0        0        0     6302 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/maze.py
--rw-r--r--   0        0        0    35221 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/renderer.py
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/state.py
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/styles.py
--rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_e.png
--rw-r--r--   0        0        0     4986 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_n.png
--rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_ne.png
--rw-r--r--   0        0        0     5459 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_ne_inner_corner.png
--rw-r--r--   0        0        0     5120 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_ne_inner_corner_e.png
--rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_ne_inner_corner_n.png
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_nw.png
--rw-r--r--   0        0        0     5450 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_nw_inner_corner.png
--rw-r--r--   0        0        0     5188 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_nw_inner_corner_e.png
--rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_nw_inner_corner_n.png
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_nw_inner_corner_w.png
--rw-r--r--   0        0        0     4915 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_s.png
--rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_s_seam.png
--rw-r--r--   0        0        0     5352 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_se.png
--rw-r--r--   0        0        0     5037 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_se_inner_corner.png
--rw-r--r--   0        0        0     4950 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_se_inner_corner_e.png
--rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_se_inner_corner_s.png
--rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_se_spec.png
--rw-r--r--   0        0        0     5332 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_sw.png
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_sw_inner_corner.png
--rw-r--r--   0        0        0     4933 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_sw_inner_corner_s.png
--rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_sw_inner_corner_w.png
--rw-r--r--   0        0        0     5005 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_sw_spec.png
--rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_w.png
--rw-r--r--   0        0        0     7759 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/minotaur.png
--rw-r--r--   0        0        0    11075 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/warrior_down.png
--rw-r--r--   0        0        0    11600 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/warrior_left.png
--rw-r--r--   0        0        0    11852 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/warrior_right.png
--rw-r--r--   0        0        0    10990 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/warrior_up.png
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 mazemastery-0.0.3/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 mazemastery-0.0.3/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mazemastery-0.0.3/README.md
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 mazemastery-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 mazemastery-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/__init__.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/api.py
+-rw-r--r--   0        0        0     6828 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/debug_menu.py
+-rw-r--r--   0        0        0     6302 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/maze.py
+-rw-r--r--   0        0        0    35221 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/renderer.py
+-rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/state.py
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/styles.py
+-rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_e.png
+-rw-r--r--   0        0        0     4986 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_n.png
+-rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_ne.png
+-rw-r--r--   0        0        0     5459 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_ne_inner_corner.png
+-rw-r--r--   0        0        0     5120 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_ne_inner_corner_e.png
+-rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_ne_inner_corner_n.png
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_nw.png
+-rw-r--r--   0        0        0     5450 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_nw_inner_corner.png
+-rw-r--r--   0        0        0     5188 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_nw_inner_corner_e.png
+-rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_nw_inner_corner_n.png
+-rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_nw_inner_corner_w.png
+-rw-r--r--   0        0        0     4915 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_s.png
+-rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_s_seam.png
+-rw-r--r--   0        0        0     5352 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_se.png
+-rw-r--r--   0        0        0     5037 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_se_inner_corner.png
+-rw-r--r--   0        0        0     4950 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_se_inner_corner_e.png
+-rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_se_inner_corner_s.png
+-rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_se_spec.png
+-rw-r--r--   0        0        0     5332 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_sw.png
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_sw_inner_corner.png
+-rw-r--r--   0        0        0     4933 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_sw_inner_corner_s.png
+-rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_sw_inner_corner_w.png
+-rw-r--r--   0        0        0     5005 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_sw_spec.png
+-rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/cloud_w.png
+-rw-r--r--   0        0        0     7759 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/minotaur.png
+-rw-r--r--   0        0        0    11075 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/warrior_down.png
+-rw-r--r--   0        0        0    11600 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/warrior_left.png
+-rw-r--r--   0        0        0    11852 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/warrior_right.png
+-rw-r--r--   0        0        0    10990 2020-02-02 00:00:00.000000 mazemastery-0.0.4/src/mazemastery/sprites/warrior_up.png
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 mazemastery-0.0.4/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 mazemastery-0.0.4/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mazemastery-0.0.4/README.md
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 mazemastery-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 mazemastery-0.0.4/PKG-INFO
```

### Comparing `mazemastery-0.0.3/src/mazemastery/api.py` & `mazemastery-0.0.4/src/mazemastery/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,46 @@
 import time
 import random
 from mazemastery.maze import create_maze, create_corridor, create_SAW
 from mazemastery.renderer import GUI
 import threading
 from mazemastery.state import State
 
+
 def get_pos():
     state = State()
     return state.pos
 
+
 def minotaur():
     state = State()
     return state.minotaur_coords
 
+
 def set_pos(new_pos):
     state = State()
     if state.dead:
         return
     if new_pos not in state.maze[state.pos]:
-        state.lives -= 1
+
+        # We don't subtract a life on level 1
+        if state.level != 1:
+            state.lives -= 1
         new_pos = state.pos
     old_pos = state.pos
     state.pos = new_pos
     if state.lives == 0:
         state.renderer.draw_popup("You died!")
         state.dead = True
     state.renderer.update_draw(old_pos, state.pos, state.lives)
     time.sleep(state.renderer.delay / 1000)
-    while (state.renderer.debug):
+    while state.renderer.debug:
         time.sleep(state.renderer.delay / 1000)
 
+
 def put_blue_gem(cell):
     state = State()
     if cell not in state.blue_gem_coords:
         state.renderer.push_blue_gem_buffer(cell)
         state.blue_gem_coords.append(cell)
 
 
@@ -49,43 +56,50 @@
     return cell in state.blue_gem_coords
 
 
 def has_red_gem(cell):
     state = State()
     return cell in state.red_gem_coords
 
+
 def has_minotaur(cell):
     state = State()
     return cell == state.minotaur_coords
 
 
 def found_minotaur():
     state = State()
     state.found = True
 
 
 def was_found():
     state = State()
     return state.found
 
-
-def get_neighbors(pos):
+def is_neighbor(pos, neighbor):
     state = State()
-    return state.maze[pos]
-
+    return neighbor in state.maze[pos]
 
 def push(pos):
     state = State()
     state.stack.append(pos)
 
 def pop():
     state = State()
     popped = state.stack.pop()
     return popped
 
+def are_neighbors(pos1, pos2):
+    state = State()
+    return pos2 in state.maze[pos1]
+
+def get_neighbors(pos):
+    state = State()
+    return state.maze[pos]
+
 def run(level, solve, rows=10, cols=10, cell_size=50, delay=1000, seed=None):
     random.seed(seed)
     if level == 1:
         maze = create_corridor(cols)
         minotaur_coords = (0, cols - 1)
     elif level == 2:
         maze = create_corridor(cols)
@@ -99,14 +113,12 @@
     elif level == 5:
         maze = create_maze(rows, cols, (0, 0), 0.2)
         minotaur_coords = (rows - 4, cols - 4)
     elif level == 6:
         maze = create_maze(rows, cols, (0, 0), 0.2)
         minotaur_coords = (rows - 4, cols - 4)
     renderer = GUI(maze, minotaur_coords, cell_size=cell_size, delay=delay)
-    state = State(
-        maze=maze, renderer=renderer, minotaur_coords=minotaur_coords
-    )
+    State(maze=maze, renderer=renderer, minotaur_coords=minotaur_coords)
     renderer.initial_draw()
     solution_thread = threading.Thread(target=solve, name="solution_thread")
     solution_thread.start()
-    renderer.root.mainloop()
+    renderer.root.mainloop()
```

### Comparing `mazemastery-0.0.3/src/mazemastery/debug_menu.py` & `mazemastery-0.0.4/src/mazemastery/debug_menu.py`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.3/src/mazemastery/maze.py` & `mazemastery-0.0.4/src/mazemastery/maze.py`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.3/src/mazemastery/renderer.py` & `mazemastery-0.0.4/src/mazemastery/renderer.py`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.3/src/mazemastery/state.py` & `mazemastery-0.0.4/src/mazemastery/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
         minotaur_coords=(0, 0),
         blue_gem_coords=[],
         red_gem_coords=[],
         stack=[],
         found=False,
         initial_lives=5,
         dead=False,
+        level=1,
         *args,
         **kwargs,
     ):
         if cls._self is None:
             cls._self = super(State, cls).__new__(cls, *args, **kwargs)
             cls._self.__maze = maze
             cls._self.__renderer = renderer
@@ -35,28 +36,30 @@
             cls._self.__blue_gem_coords = blue_gem_coords
             cls._self.__red_gem_coords = red_gem_coords
             cls._self.__stack = stack
             cls._self.__found = found
             cls._self.__initial_lives = initial_lives
             cls._self.__lives = initial_lives
             cls._self.__dead = dead
+            cls._self.__level = level
         return cls._self
 
     def __init__(
         self,
         maze=None,
         renderer=None,
         start_pos=(0, 0),
         minotaur_coords=(0, 0),
         blue_gem_coords=[],
         red_gem_coords=[],
         stack=[],
         found=False,
         lives=5,
         dead=False,
+        level=1,
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
 
     @property
     def maze(self):
@@ -129,7 +132,15 @@
     @property
     def dead(self):
         return self.__dead
 
     @dead.setter
     def dead(self, new):
         self.__dead = new
+
+    @property
+    def level(self):
+        return self.__level
+    
+    @level.setter
+    def level(self, new):
+        self.__level = new
```

### Comparing `mazemastery-0.0.3/src/mazemastery/styles.py` & `mazemastery-0.0.4/src/mazemastery/styles.py`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.3/src/mazemastery/sprites/cloud_e.png` & `mazemastery-0.0.4/src/mazemastery/sprites/cloud_e.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.3/src/mazemastery/sprites/cloud_n.png` & `mazemastery-0.0.4/src/mazemastery/sprites/cloud_n.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.3/src/mazemastery/sprites/cloud_ne.png` & `mazemastery-0.0.4/src/mazemastery/sprites/cloud_ne.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.3/src/mazemastery/sprites/cloud_ne_inner_corner.png` & `mazemastery-0.0.4/src/mazemastery/sprites/cloud_ne_inner_corner.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.3/src/mazemastery/sprites/cloud_ne_inner_corner_e.png` & `mazemastery-0.0.4/src/mazemastery/sprites/cloud_ne_inner_corner_e.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.3/src/mazemastery/sprites/cloud_ne_inner_corner_n.png` & `mazemastery-0.0.4/src/mazemastery/sprites/cloud_ne_inner_corner_n.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.3/src/mazemastery/sprites/cloud_nw.png` & `mazemastery-0.0.4/src/mazemastery/sprites/cloud_nw.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.3/src/mazemastery/sprites/cloud_nw_inner_corner.png` & `mazemastery-0.0.4/src/mazemastery/sprites/cloud_nw_inner_corner.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.3/src/mazemastery/sprites/cloud_nw_inner_corner_e.png` & `mazemastery-0.0.4/src/mazemastery/sprites/cloud_nw_inner_corner_e.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.3/src/mazemastery/sprites/cloud_nw_inner_corner_n.png` & `mazemastery-0.0.4/src/mazemastery/sprites/cloud_nw_inner_corner_n.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.3/src/mazemastery/sprites/cloud_nw_inner_corner_w.png` & `mazemastery-0.0.4/src/mazemastery/sprites/cloud_nw_inner_corner_w.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.3/src/mazemastery/sprites/cloud_s.png` & `mazemastery-0.0.4/src/mazemastery/sprites/cloud_s.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.3/src/mazemastery/sprites/cloud_s_seam.png` & `mazemastery-0.0.4/src/mazemastery/sprites/cloud_s_seam.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.3/src/mazemastery/sprites/cloud_se.png` & `mazemastery-0.0.4/src/mazemastery/sprites/cloud_se.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.3/src/mazemastery/sprites/cloud_se_inner_corner.png` & `mazemastery-0.0.4/src/mazemastery/sprites/cloud_se_inner_corner.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.3/src/mazemastery/sprites/cloud_se_inner_corner_e.png` & `mazemastery-0.0.4/src/mazemastery/sprites/cloud_se_inner_corner_e.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.3/src/mazemastery/sprites/cloud_se_inner_corner_s.png` & `mazemastery-0.0.4/src/mazemastery/sprites/cloud_se_inner_corner_s.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.3/src/mazemastery/sprites/cloud_se_spec.png` & `mazemastery-0.0.4/src/mazemastery/sprites/cloud_se_spec.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.3/src/mazemastery/sprites/cloud_sw.png` & `mazemastery-0.0.4/src/mazemastery/sprites/cloud_sw.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.3/src/mazemastery/sprites/cloud_sw_inner_corner.png` & `mazemastery-0.0.4/src/mazemastery/sprites/cloud_sw_inner_corner.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.3/src/mazemastery/sprites/cloud_sw_inner_corner_s.png` & `mazemastery-0.0.4/src/mazemastery/sprites/cloud_sw_inner_corner_s.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.3/src/mazemastery/sprites/cloud_sw_inner_corner_w.png` & `mazemastery-0.0.4/src/mazemastery/sprites/cloud_sw_inner_corner_w.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.3/src/mazemastery/sprites/cloud_sw_spec.png` & `mazemastery-0.0.4/src/mazemastery/sprites/cloud_sw_spec.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.3/src/mazemastery/sprites/cloud_w.png` & `mazemastery-0.0.4/src/mazemastery/sprites/cloud_w.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.3/src/mazemastery/sprites/minotaur.png` & `mazemastery-0.0.4/src/mazemastery/sprites/minotaur.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.3/src/mazemastery/sprites/warrior_down.png` & `mazemastery-0.0.4/src/mazemastery/sprites/warrior_down.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.3/src/mazemastery/sprites/warrior_left.png` & `mazemastery-0.0.4/src/mazemastery/sprites/warrior_left.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.3/src/mazemastery/sprites/warrior_right.png` & `mazemastery-0.0.4/src/mazemastery/sprites/warrior_right.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.3/src/mazemastery/sprites/warrior_up.png` & `mazemastery-0.0.4/src/mazemastery/sprites/warrior_up.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.3/LICENSE` & `mazemastery-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.3/pyproject.toml` & `mazemastery-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires= ["hatchling", "Pillow"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mazemastery"
-version = "0.0.3"
+version = "0.0.4"
 description = "MazeMastery is a Python framework for teaching maze traversal to high school students. It helps students develop abstraction skills by providing a didactic tool. They can test their algorithms against randomized test cases of increasing complexity. The framework facilitates learning analysis and conceptual challenges. MazeMastery is an open-source project for scientists and educators."
 authors = [
     {name="Raphaël Baur", email="rabaur@ethz.ch"},
     {name="Jens Hartmann", email="s4jehart@uni-trier.de"},
     {name="Jaqueline Staub", email="staub@uni-trier.de"},
     {name="Martin Löhnertz", email="loehnert@uni-trier.de"},
 ]
```

### Comparing `mazemastery-0.0.3/PKG-INFO` & `mazemastery-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mazemastery
-Version: 0.0.3
+Version: 0.0.4
 Summary: MazeMastery is a Python framework for teaching maze traversal to high school students. It helps students develop abstraction skills by providing a didactic tool. They can test their algorithms against randomized test cases of increasing complexity. The framework facilitates learning analysis and conceptual challenges. MazeMastery is an open-source project for scientists and educators.
 Project-URL: Homepage, https://github.com/rabaur/MazeMastery
 Author-email: Raphaël Baur <rabaur@ethz.ch>, Jens Hartmann <s4jehart@uni-trier.de>, Jaqueline Staub <staub@uni-trier.de>, Martin Löhnertz <loehnert@uni-trier.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

