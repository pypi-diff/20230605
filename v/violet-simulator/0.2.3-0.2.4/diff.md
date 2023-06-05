# Comparing `tmp/violet_simulator-0.2.3.tar.gz` & `tmp/violet_simulator-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "violet_simulator-0.2.3.tar", last modified: Thu May  4 14:45:33 2023, max compression
+gzip compressed data, was "violet_simulator-0.2.4.tar", last modified: Mon Jun  5 10:04:27 2023, max compression
```

## Comparing `violet_simulator-0.2.3.tar` & `violet_simulator-0.2.4.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1073 2023-05-04 10:04:14.538843 violet_simulator-0.2.3/LICENSE
--rw-r--r--   0        0        0     1250 2023-05-04 11:07:23.861471 violet_simulator-0.2.3/README.md
--rw-r--r--   0        0        0     1100 2023-05-04 14:45:33.685229 violet_simulator-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     6215 2023-05-04 11:55:19.107727 violet_simulator-0.2.3/vi/__init__.py
--rw-r--r--   0        0        0      754 2023-05-04 11:56:20.032548 violet_simulator-0.2.3/vi/_static.py
--rw-r--r--   0        0        0    20219 2023-05-04 11:47:40.841524 violet_simulator-0.2.3/vi/agent.py
--rw-r--r--   0        0        0    16075 2023-05-04 11:53:52.918788 violet_simulator-0.2.3/vi/config.py
--rw-r--r--   0        0        0     9734 2023-05-04 10:58:54.083770 violet_simulator-0.2.3/vi/metrics.py
--rw-r--r--   0        0        0    10571 2023-05-04 11:45:47.034248 violet_simulator-0.2.3/vi/proximity.py
--rw-r--r--   0        0        0     2536 2023-05-04 11:33:22.900862 violet_simulator-0.2.3/vi/replay.py
--rw-r--r--   0        0        0    15462 2023-05-04 11:47:49.827135 violet_simulator-0.2.3/vi/simulation.py
--rw-r--r--   0        0        0     1430 2023-05-04 11:56:40.310462 violet_simulator-0.2.3/vi/util.py
--rw-r--r--   0        0        0     1848 1970-01-01 00:00:00.000000 violet_simulator-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-04 10:04:14.538843 violet_simulator-0.2.4/LICENSE
+-rw-r--r--   0        0        0     1250 2023-05-04 11:07:23.861471 violet_simulator-0.2.4/README.md
+-rw-r--r--   0        0        0     1184 2023-06-05 10:04:27.810543 violet_simulator-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     6636 2023-05-08 10:54:55.231379 violet_simulator-0.2.4/vi/__init__.py
+-rw-r--r--   0        0        0      754 2023-05-04 19:35:01.932371 violet_simulator-0.2.4/vi/_static.py
+-rw-r--r--   0        0        0    20248 2023-05-04 19:35:01.932165 violet_simulator-0.2.4/vi/agent.py
+-rw-r--r--   0        0        0    16110 2023-05-04 18:47:52.672820 violet_simulator-0.2.4/vi/config.py
+-rw-r--r--   0        0        0     9752 2023-05-08 10:53:55.003544 violet_simulator-0.2.4/vi/metrics.py
+-rw-r--r--   0        0        0    10579 2023-05-04 16:07:17.116626 violet_simulator-0.2.4/vi/proximity.py
+-rw-r--r--   0        0        0        0 2023-05-04 15:50:55.262208 violet_simulator-0.2.4/vi/py.typed
+-rw-r--r--   0        0        0     2571 2023-05-04 16:06:05.513631 violet_simulator-0.2.4/vi/replay.py
+-rw-r--r--   0        0        0    15522 2023-05-04 19:35:01.931843 violet_simulator-0.2.4/vi/simulation.py
+-rw-r--r--   0        0        0     1520 2023-05-04 16:02:31.078068 violet_simulator-0.2.4/vi/util.py
+-rw-r--r--   0        0        0     1848 1970-01-01 00:00:00.000000 violet_simulator-0.2.4/PKG-INFO
```

### Comparing `violet_simulator-0.2.3/LICENSE` & `violet_simulator-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `violet_simulator-0.2.3/README.md` & `violet_simulator-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `violet_simulator-0.2.3/pyproject.toml` & `violet_simulator-0.2.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "violet-simulator"
-version = "0.2.3"
+version = "0.2.4"
 description = "A smol simulator framework built on top of PyGame"
 requires-python = ">=3.9"
 readme = "README.md"
 dependencies = [
     "pygame>=2.4.0",
     "polars>=0.17.11",
     "pyserde[toml]>=0.10.4",
@@ -34,14 +34,21 @@
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "pdoc>=13.1.1",
 ]
 
+[tool.pyright]
+include = [
+    "examples",
+    "vi",
+]
+typeCheckingMode = "strict"
+
 [tool.ruff]
 ignore = [
     "E501",
 ]
 select = [
     "C",
     "E",
```

### Comparing `violet_simulator-0.2.3/vi/__init__.py` & `violet_simulator-0.2.4/vi/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -152,11 +152,46 @@
 
 from pygame.math import Vector2
 from serde.de import deserialize
 from serde.se import serialize
 
 from .agent import Agent
 from .config import Config, Matrix, Window
+from .metrics import Fps, Metrics
 from .proximity import ProximityIter
 from .replay import TimeMachine
 from .simulation import HeadlessSimulation, Simulation
 from .util import probability
+
+
+__all__ = [
+    # agent
+    "Agent",
+
+    # config
+    "Config",
+    "Matrix",
+    "Window",
+
+    # metrics
+    "Fps",
+    "Metrics",
+
+    # proximity
+    "ProximityIter",
+
+    # replay
+    "TimeMachine",
+
+    # simulation
+    "HeadlessSimulation",
+    "Simulation",
+
+    # util
+    "probability",
+
+    # re-exports
+    "dataclass",
+    "deserialize",
+    "serialize",
+    "Vector2"
+]
```

### Comparing `violet_simulator-0.2.3/vi/_static.py` & `violet_simulator-0.2.4/vi/_static.py`

 * *Files identical despite different names*

### Comparing `violet_simulator-0.2.3/vi/agent.py` & `violet_simulator-0.2.4/vi/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,19 @@
 
     from ._static import _StaticSprite
     from .config import Config
     from .proximity import ProximityIter
     from .simulation import HeadlessSimulation, Shared
 
 
+__all__ = [
+    "Agent",
+]
+
+
 class Agent(Sprite):
     """
     The `Agent` class is home to Violet's various additions and is
     built on top of [PyGame's Sprite](https://www.pygame.org/docs/ref/sprite.html) class.
 
     While you can simply add this `Agent` class to your simulations by calling `batch_spawn_agents`,
     the agents won't actually do anything interesting.
```

### Comparing `violet_simulator-0.2.3/vi/config.py` & `violet_simulator-0.2.4/vi/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,23 @@
 from typing import Any, Generic, Optional, Type, TypeVar, Union
 
 from serde.de import deserialize
 from serde.se import serialize
 from serde.toml import from_toml
 
 
+__all__ = [
+    "dataclass",
+    "Config",
+    "Matrix",
+    "Schema",
+    "Window"
+]
+
+
 def _embiggen(input_list: list[Any], copies: int):
     """The in-place deep-copy variant of list multiplication."""
 
     head = input_list[:]
 
     for _ in range(copies - 1):
         input_list.extend(deepcopy(head))
@@ -409,10 +418,7 @@
     ...     Simulation(MyConfig())
     ...     .batch_spawn_agents(100, MyAgent, ["examples/images/white.png"])
     ...     .run()
     ... )
     """
 
     ...
-
-
-__all__ = ["Schema", "Config", "Matrix", "Window"]
```

### Comparing `violet_simulator-0.2.3/vi/metrics.py` & `violet_simulator-0.2.4/vi/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,14 +184,20 @@
 from collections import defaultdict
 from dataclasses import dataclass, field
 from typing import Any
 
 import polars as pl
 
 
+__all__ = [
+    "Fps",
+    "Metrics",
+]
+
+
 @dataclass
 class Fps:
     _fps: list[float] = field(default_factory=list)
 
     def _push(self, fps: float):
         self._fps.append(fps)
 
@@ -219,10 +225,7 @@
 
     def _merge(self):
         df = pl.from_dict(self._temporary_snapshots)
 
         self.snapshots.vstack(df, in_place=True)
 
         self._temporary_snapshots = defaultdict(list)
-
-
-__all__ = ["Metrics"]
```

### Comparing `violet_simulator-0.2.3/vi/proximity.py` & `violet_simulator-0.2.4/vi/proximity.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,20 @@
 
 
 if TYPE_CHECKING:
     from pygame.sprite import Group
 
     from .agent import Agent
 
+
+__all__ = [
+    "ProximityIter",
+]
+
+
 AgentClass = TypeVar("AgentClass", bound="Agent")
 T = TypeVar("T")
 U = TypeVar("U")
 
 
 class ProximityIter(Generic[T]):
     """The `ProximityIter` is a small wrapper around a *generator* of agents that are in proximity.
@@ -324,10 +330,7 @@
     ) -> ProximityIter[tuple[AgentClass, float]]:
         """Retrieve a set of agents that are in the same chunk as the given agent,
         in addition to the agents in the eight neighbouring chunks.
         """
 
         agents = self.__accurate_retrieval(agent)
         return ProximityIter(agents)
-
-
-__all__ = ["ProximityIter"]
```

### Comparing `violet_simulator-0.2.3/vi/replay.py` & `violet_simulator-0.2.4/vi/replay.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,19 @@
 from .config import Window
 
 
 if TYPE_CHECKING:
     from polars import DataFrame, Series
 
 
+__all__ = [
+    "TimeMachine",
+]
+
+
 def load_images(image_paths: list[str]) -> list[pg.surface.Surface]:
     return [pg.image.load(path).convert_alpha() for path in image_paths]
 
 
 class TimeMachine:
     images: list[pg.surface.Surface]
     window: Window
```

### Comparing `violet_simulator-0.2.3/vi/simulation.py` & `violet_simulator-0.2.4/vi/simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,20 @@
     from typing_extensions import Self
 
     from .agent import Agent
 
     AgentClass = TypeVar("AgentClass", bound=Agent)
 
 
+__all__ = [
+    "HeadlessSimulation",
+    "Simulation",
+]
+
+
 @dataclass
 class Shared:
     """A mutatable container for data that needs to be shared between `vi.agent.Agent` and `Simulation`."""
 
     prng_move: random.Random
     """A PRNG for agent movement exclusively.
```

### Comparing `violet_simulator-0.2.3/vi/util.py` & `violet_simulator-0.2.4/vi/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,22 @@
 from pygame.math import Vector2
 
 
 if TYPE_CHECKING:
     from pygame.rect import Rect
 
 
+__all__ = [
+    "probability",
+    "round_pos",
+    "random_angle",
+    "random_pos",
+]
+
+
 def probability(threshold: float, prng: Optional[random.Random] = None) -> bool:
     """Randomly retrieve True or False depending on the given probability.
 
     The probability should be between 0 and 1.
     If you give a probability equal or higher than 1, this function will always return True.
     Likewise, if you give a probability equal or lower than 0, this function will always return False.
     """
```

### Comparing `violet_simulator-0.2.3/PKG-INFO` & `violet_simulator-0.2.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: violet-simulator
-Version: 0.2.3
+Version: 0.2.4
 Summary: A smol simulator framework built on top of PyGame
 Home-page: https://violet.m-rots.com
 Author-Email: Storm Timmermans <stormtimmermans@icloud.com>
 License: MIT
 Project-URL: Homepage, https://violet.m-rots.com
 Project-URL: Repository, https://github.com/m-rots/violet
 Project-URL: Documentation, https://api.violet.m-rots.com/vi
```

