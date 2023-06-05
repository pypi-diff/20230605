# Comparing `tmp/lvsfunc-0.7.1.tar.gz` & `tmp/lvsfunc-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lvsfunc-0.7.1.tar", last modified: Sun Mar 26 17:41:21 2023, max compression
+gzip compressed data, was "lvsfunc-0.8.0.tar", last modified: Mon Jun  5 17:28:24 2023, max compression
```

## Comparing `lvsfunc-0.7.1.tar` & `lvsfunc-0.8.0.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:41:21.735773 lvsfunc-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-26 17:40:57.000000 lvsfunc-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-03-26 17:41:21.735773 lvsfunc-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-03-26 17:40:57.000000 lvsfunc-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:41:21.731773 lvsfunc-0.7.1/lvsfunc/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-03-26 17:40:57.000000 lvsfunc-0.7.1/lvsfunc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-03-26 17:40:57.000000 lvsfunc-0.7.1/lvsfunc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-26 17:40:57.000000 lvsfunc-0.7.1/lvsfunc/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    46345 2023-03-26 17:40:57.000000 lvsfunc-0.7.1/lvsfunc/comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-03-26 17:40:57.000000 lvsfunc-0.7.1/lvsfunc/deblock.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-03-26 17:40:57.000000 lvsfunc-0.7.1/lvsfunc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-03-26 17:40:57.000000 lvsfunc-0.7.1/lvsfunc/fun.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-03-26 17:40:57.000000 lvsfunc-0.7.1/lvsfunc/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)    14997 2023-03-26 17:40:57.000000 lvsfunc-0.7.1/lvsfunc/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 17:40:57.000000 lvsfunc-0.7.1/lvsfunc/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-03-26 17:40:57.000000 lvsfunc-0.7.1/lvsfunc/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:41:21.735773 lvsfunc-0.7.1/lvsfunc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-03-26 17:41:21.000000 lvsfunc-0.7.1/lvsfunc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-03-26 17:41:21.000000 lvsfunc-0.7.1/lvsfunc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 17:41:21.000000 lvsfunc-0.7.1/lvsfunc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-26 17:41:21.000000 lvsfunc-0.7.1/lvsfunc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-26 17:41:21.000000 lvsfunc-0.7.1/lvsfunc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-26 17:41:21.735773 lvsfunc-0.7.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1754 2023-03-26 17:40:57.000000 lvsfunc-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:28:24.860834 lvsfunc-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-05 17:28:01.000000 lvsfunc-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-06-05 17:28:24.860834 lvsfunc-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-05 17:28:01.000000 lvsfunc-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:28:24.860834 lvsfunc-0.8.0/lvsfunc/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-05 17:28:01.000000 lvsfunc-0.8.0/lvsfunc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-05 17:28:01.000000 lvsfunc-0.8.0/lvsfunc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-05 17:28:01.000000 lvsfunc-0.8.0/lvsfunc/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33799 2023-06-05 17:28:01.000000 lvsfunc-0.8.0/lvsfunc/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-06-05 17:28:01.000000 lvsfunc-0.8.0/lvsfunc/deblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-05 17:28:01.000000 lvsfunc-0.8.0/lvsfunc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-05 17:28:01.000000 lvsfunc-0.8.0/lvsfunc/fun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-06-05 17:28:01.000000 lvsfunc-0.8.0/lvsfunc/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 17:28:01.000000 lvsfunc-0.8.0/lvsfunc/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-06-05 17:28:01.000000 lvsfunc-0.8.0/lvsfunc/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:28:24.860834 lvsfunc-0.8.0/lvsfunc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-06-05 17:28:24.000000 lvsfunc-0.8.0/lvsfunc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-05 17:28:24.000000 lvsfunc-0.8.0/lvsfunc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:28:24.000000 lvsfunc-0.8.0/lvsfunc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-05 17:28:24.000000 lvsfunc-0.8.0/lvsfunc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 17:28:24.000000 lvsfunc-0.8.0/lvsfunc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 17:28:24.860834 lvsfunc-0.8.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1754 2023-06-05 17:28:01.000000 lvsfunc-0.8.0/setup.py
```

### Comparing `lvsfunc-0.7.1/LICENSE` & `lvsfunc-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lvsfunc-0.7.1/PKG-INFO` & `lvsfunc-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lvsfunc
-Version: 0.7.1
+Version: 0.8.0
 Summary: Light's Vapoursynth Functions.
 Author: LightArrowsEXE
 Author-email: LightArrowsReboot@gmail.com
 Maintainer: LightArrowsEXE
 Maintainer-email: LightArrowsReboot@gmail.com
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/lvsfunc
 Project-URL: Documentation, https://lvsfunc.encode.moe/en/latest/
@@ -62,15 +62,14 @@
 ## Usage
 
 After installation, functions can be loaded and used as follows:
 
 ```py
 import lvsfunc as lvf
 
-src = lvf.misc.source(...)
 aa = lvf.aa.clamp_aa(...)
 comp = lvf.comparison.compare(...)
 ...
 ```
 
 ## Disclaimer
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lvsfunc Version: 0.7.1 Summary: Light's Vapoursynth
+Metadata-Version: 2.1 Name: lvsfunc Version: 0.8.0 Summary: Light's Vapoursynth
 Functions. Author: LightArrowsEXE Author-email: LightArrowsReboot@gmail.com
 Maintainer: LightArrowsEXE Maintainer-email: LightArrowsReboot@gmail.com
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/
 lvsfunc Project-URL: Documentation, https://lvsfunc.encode.moe/en/latest/
 Project-URL: Contact, https://discord.gg/qxTxVJGtst Classifier: Natural
 Language :: English Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Other Audience Classifier: Programming Language :: Python
@@ -19,12 +19,12 @@
 //lvsfunc.encode.moe/en/latest/). For further support, drop by `#lvsfunc` in
 the [IEW Discord server](https://discord.gg/qxTxVJGtst). ## How to install If
 you have the old `lvsfunc.py` module, remove that from your system first.
 Install `lvsfunc` with the following command: ```sh $ pip3 install lvsfunc --
 no-cache-dir -U ``` Or if you want the latest git version, install it with this
 command: ```sh $ pip3 install git+https://github.com/Irrational-Encoding-
 Wizardry/lvsfunc.git --no-cache-dir -U ``` ## Usage After installation,
-functions can be loaded and used as follows: ```py import lvsfunc as lvf src =
-lvf.misc.source(...) aa = lvf.aa.clamp_aa(...) comp = lvf.comparison.compare
-(...) ... ``` ## Disclaimer Anything **MAY** change at any time. The public API
-**SHOULD NOT** be considered stable. If you use lvsfunc in any of your
-projects, consider hardcoding a version requirement.
+functions can be loaded and used as follows: ```py import lvsfunc as lvf aa =
+lvf.aa.clamp_aa(...) comp = lvf.comparison.compare(...) ... ``` ## Disclaimer
+Anything **MAY** change at any time. The public API **SHOULD NOT** be
+considered stable. If you use lvsfunc in any of your projects, consider
+hardcoding a version requirement.
```

### Comparing `lvsfunc-0.7.1/README.md` & `lvsfunc-0.8.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 ## Usage
 
 After installation, functions can be loaded and used as follows:
 
 ```py
 import lvsfunc as lvf
 
-src = lvf.misc.source(...)
 aa = lvf.aa.clamp_aa(...)
 comp = lvf.comparison.compare(...)
 ...
 ```
 
 ## Disclaimer
```

#### html2text {}

```diff
@@ -7,12 +7,12 @@
 //lvsfunc.encode.moe/en/latest/). For further support, drop by `#lvsfunc` in
 the [IEW Discord server](https://discord.gg/qxTxVJGtst). ## How to install If
 you have the old `lvsfunc.py` module, remove that from your system first.
 Install `lvsfunc` with the following command: ```sh $ pip3 install lvsfunc --
 no-cache-dir -U ``` Or if you want the latest git version, install it with this
 command: ```sh $ pip3 install git+https://github.com/Irrational-Encoding-
 Wizardry/lvsfunc.git --no-cache-dir -U ``` ## Usage After installation,
-functions can be loaded and used as follows: ```py import lvsfunc as lvf src =
-lvf.misc.source(...) aa = lvf.aa.clamp_aa(...) comp = lvf.comparison.compare
-(...) ... ``` ## Disclaimer Anything **MAY** change at any time. The public API
-**SHOULD NOT** be considered stable. If you use lvsfunc in any of your
-projects, consider hardcoding a version requirement.
+functions can be loaded and used as follows: ```py import lvsfunc as lvf aa =
+lvf.aa.clamp_aa(...) comp = lvf.comparison.compare(...) ... ``` ## Disclaimer
+Anything **MAY** change at any time. The public API **SHOULD NOT** be
+considered stable. If you use lvsfunc in any of your projects, consider
+hardcoding a version requirement.
```

### Comparing `lvsfunc-0.7.1/lvsfunc/__init__.py` & `lvsfunc-0.8.0/lvsfunc/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,14 +5,13 @@
     or reach out to me on Discord (LightArrowsEXE#0476)!
 
     For further support, drop by `#lvsfunc` in the `IEW Discord server <https://discord.gg/qxTxVJGtst>`_.
 """
 
 # flake8: noqa
 
-from . import comparison, deblock, exceptions, mask, misc, util
+from . import comparison, deblock, exceptions, misc, util
 from .comparison import *
 from .deblock import *
 from .exceptions import *
-from .mask import *
 from .misc import *
 from .util import *
```

### Comparing `lvsfunc-0.7.1/lvsfunc/__main__.py` & `lvsfunc-0.8.0/lvsfunc/__main__.py`

 * *Files identical despite different names*

### Comparing `lvsfunc-0.7.1/lvsfunc/comparison.py` & `lvsfunc-0.8.0/lvsfunc/comparison.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,34 @@
 from __future__ import annotations
 
 import math
 import random
-import re
-import warnings
 from abc import ABC, abstractmethod
 from itertools import groupby, zip_longest
-from pathlib import Path
-from typing import (Any, Callable, Iterable, Iterator, Literal, Sequence,
-                    TypeVar, overload)
+from typing import Callable, Iterable, Iterator, Literal, Sequence, overload
 
 from vskernels import Catrom, Kernel, KernelT, Point
-from vstools import (CustomError, CustomNotImplementedError, CustomTypeError,
-                     CustomValueError, DependencyNotFoundError, Direction,
-                     FormatsMismatchError, InvalidColorFamilyError,
-                     LengthMismatchError, Matrix, Sentinel,
-                     UnsupportedSubsamplingError, VariableFormatError,
-                     check_variable, check_variable_format,
-                     check_variable_resolution, clip_async_render, core, depth,
-                     get_prop, get_subsampling, get_w, merge_clip_props)
-from vstools import split as split_planes
-from vstools import vs
+from vstools import (
+    CustomError, CustomNotImplementedError, CustomTypeError, CustomValueError, Direction, FormatsMismatchError,
+    LengthMismatchError, Matrix, Sentinel, T, VariableFormatError, check_variable_format, check_variable_resolution,
+    clip_async_render, core, depth, get_prop, get_subsampling, get_w, merge_clip_props, mod2, vs
+)
 
 from .exceptions import ClipsAndNamedClipsError
-from .misc import source
-from .util import truncate_string
 
 __all__ = [
-    'compare', 'comp',
+    'compare',
     'Comparer',
     'comparison_shots',
     'diff',
-    'Interleave', 'interleave',
-    'source_mediainfo', 'srcm',
-    'Split', 'split',
-    'stack_compare', 'scomp',
-    'stack_horizontal', 'stack_vertical',
-    'stack_planes',
+    'Interleave',
+    'Split',
+    'stack_compare',
     'Stack',
-    'Tile', 'tile',
-]
-
-T = TypeVar('T')
-
-x265_me_map = [
-    "dia", "hex", "umh", "star", "sea", "full"
+    'Tile',
 ]
 
 
 class Comparer(ABC):
     """
     Base class for comparison functions.
 
@@ -64,24 +44,23 @@
                                 (Default: 7).
 
     :raises ValueError:         Less than two clips passed.
     :raises ValueError:         `label_alignment` is not between 1–9.
     :raises ValueError:         Unexpected type passed to `clips`.
     """
 
-    def __init__(self,
-                 clips: dict[str, vs.VideoNode] | Sequence[vs.VideoNode],
-                 /,
-                 *,
-                 label_alignment: int = 7
-                 ) -> None:
+    def __init__(
+        self, clips: dict[str, vs.VideoNode] | Sequence[vs.VideoNode], /, *, label_alignment: int = 7
+    ) -> None:
         if len(clips) < 2:
             raise CustomValueError("Compare functions must be used on at least 2 clips!", self.__class__)
+
         if label_alignment not in list(range(1, 10)):
             raise CustomValueError("`label_alignment` must be an integer from 1 to 9!", self.__class__)
+
         if not isinstance(clips, (dict, Sequence)):
             raise CustomTypeError(f"Unexpected type {type(clips)} for `clips` argument!", self.__class__)
 
         self.clips = list(clips.values()) if isinstance(clips, dict) else list(clips)
         self.names = list(clips.keys()) if isinstance(clips, dict) else None
 
         self.label_alignment = label_alignment
@@ -158,14 +137,26 @@
                 raise CustomValueError("StackHorizontal requires that all clips be the same height!", self.__class__)
             return core.std.StackHorizontal(self._marked_clips())
 
         if not self.width:
             raise CustomValueError("StackVertical requires that all clips be the same width!", self.__class__)
         return core.std.StackVertical(self._marked_clips())
 
+    @classmethod
+    def stack(cls, *clips: vs.VideoNode, **namedclips: vs.VideoNode) -> vs.VideoNode:
+        if clips and namedclips:
+            raise ClipsAndNamedClipsError(cls.stack)
+        return cls(clips if clips else namedclips).clip
+
+    @classmethod
+    def stack_vertical(cls, *clips: vs.VideoNode, **namedclips: vs.VideoNode) -> vs.VideoNode:
+        if clips and namedclips:
+            raise ClipsAndNamedClipsError(cls.stack)
+        return cls(clips if clips else namedclips, direction=Direction.VERTICAL).clip
+
 
 class Interleave(Comparer):
     """
     Returns a clip with the frames from all clips interleaved.
 
     For example, Interleave(A=clip1, B=clip2) will return A.Frame 0, B.Frame 0, A.Frame 1, B.Frame 1, ...
 
@@ -366,14 +357,20 @@
                     bottom_crop = crop_height * (self.num_clips - 1 - key)
 
                     if key != (self.num_clips - 1):
                         bottom_crop += overflow
 
                     self.clips[key] = clip.std.Crop(top=top_crop, bottom=bottom_crop)
 
+    @classmethod
+    def stack(cls, *clips: vs.VideoNode, **namedclips: vs.VideoNode) -> vs.VideoNode:
+        if clips and namedclips:
+            raise ClipsAndNamedClipsError(cls.stack)
+        return cls(clips if clips else namedclips, label_alignment=2).clip
+
 
 def compare(clip_a: vs.VideoNode, clip_b: vs.VideoNode,
             frames: list[int] | None = None,
             rand_total: int | None = None,
             force_resample: bool = True, print_frame: bool = True,
             mismatch: bool = False) -> vs.VideoNode:
     """
@@ -431,14 +428,15 @@
         if not rand_total:
             # More comparisons for shorter clips so you can compare stuff like NCs more conveniently
             rand_total = int(clip_a.num_frames / 1000) if clip_a.num_frames > 5000 else int(clip_a.num_frames / 100)
         frames = sorted(random.sample(range(1, clip_a.num_frames - 1), rand_total))
 
     frames_a = core.std.Splice([clip_a[f] for f in frames]).std.AssumeFPS(fpsnum=1, fpsden=1)
     frames_b = core.std.Splice([clip_b[f] for f in frames]).std.AssumeFPS(fpsnum=1, fpsden=1)
+
     return core.std.Interleave([frames_a, frames_b], mismatch=mismatch)
 
 
 def stack_compare(*clips: vs.VideoNode,
                   height: int | None = None) -> vs.VideoNode:
     """
     Compare two clips by stacking them.
@@ -460,69 +458,31 @@
         raise CustomValueError("You must pass at least two clips", stack_compare, f"{len(clips)} < 2")
 
     clipa, clipb = clips
 
     if not height:
         height = 288
     elif height > clipa.height / 2:
-        warnings.warn(f"stack_compare: 'Given 'height' ({height}) is bigger than clipa's height {clipa.height}!' "
-                      "Will be using clipa's height instead.")
+        import warnings
+        warnings.warn(
+            f"stack_compare: 'Given 'height' ({height}) is bigger than clipa's height {clipa.height}!' "
+            "Will be using clipa's height instead."
+        )
         height = int(clipa.height / 2)
 
     scaled_width = get_w(height, mod=1)
 
-    diff = core.std.MakeDiff(clipa=clipa, clipb=clipb)
-    diff = Catrom().scale(diff, scaled_width * 2, height * 2).text.FrameNum(8)
-    resized = [Catrom().scale(clipa, scaled_width, height).text.Text('Clip A', 3),
-               Catrom().scale(clipb, scaled_width, height).text.Text('Clip B', 1)]
-
-    return Stack([Stack(resized).clip, diff], direction=Direction.VERTICAL).clip
-
-
-def stack_planes(clip: vs.VideoNode, /, stack_vertical: bool = False) -> vs.VideoNode:
-    """
-    Stacks the planes of a clip.
-
-    For 4:2:0 subsampled clips, the two half-sized planes will be stacked in the opposite direction specified
-    (vertical by default),
-    then stacked with the full-sized plane in the direction specified (horizontal by default).
-
-    :param clip:                        Clip to process (must be in YUV or RGB planar format).
-    :param stack_vertical:              Stack the planes vertically (Default: ``False``).
-
-    :return:                            Clip with stacked planes.
-
-    :raises VariableFormatError:        Clip is of a variable format.
-    :raises VariableResolutionError:    Clip is of a variable resolution.
-    :raises InvalidColorFamilyError:    Clip is not YUV or RGB.
-    :raises TypeError:                  Clip returns an unexpected subsampling.
-    """
-    assert check_variable(clip, stack_planes)
-
-    InvalidColorFamilyError.check(clip, (vs.YUV, vs.RGB), stack_planes)
-
-    yuv_planes = split_planes(clip)
+    diff = Catrom.scale(clipa.std.MakeDiff(clipb), scaled_width * 2, height * 2).text.FrameNum(8)
 
-    if clip.format.color_family == vs.ColorFamily.YUV:
-        planes: dict[str, vs.VideoNode] = {'Y': yuv_planes[0], 'U': yuv_planes[1], 'V': yuv_planes[2]}
-    elif clip.format.color_family == vs.ColorFamily.RGB:
-        planes = {'R': yuv_planes[0], 'G': yuv_planes[1], 'B': yuv_planes[2]}
+    resized = [
+        Catrom.scale(clipa, scaled_width, height).text.Text('Clip A', 3),
+        Catrom.scale(clipb, scaled_width, height).text.Text('Clip B', 1)
+    ]
 
-    direction: Direction = Direction.HORIZONTAL if not stack_vertical else Direction.VERTICAL
-
-    if get_subsampling(clip) in ('444', None):
-        return Stack(planes, direction=direction).clip
-    elif get_subsampling(clip) == '420':
-        subsample_direction: Direction = Direction.HORIZONTAL if stack_vertical else Direction.VERTICAL
-        y_plane = planes.pop('Y').text.Text(text='Y')
-        subsampled_planes = Stack(planes, direction=subsample_direction).clip
-
-        return Stack([y_plane, subsampled_planes], direction=direction).clip
-    else:
-        raise UnsupportedSubsamplingError(stack_planes)
+    return Stack([Stack(resized).clip, diff], direction=Direction.VERTICAL).clip
 
 
 @overload
 def diff(*clips: vs.VideoNode,
          thr: float = ...,
          height: int = ...,
          interleave: bool = ...,
@@ -700,262 +660,14 @@
 
     if return_ranges:
         return comparison, list(_to_ranges(frames))
     else:
         return comparison
 
 
-def interleave(*clips: vs.VideoNode, **namedclips: vs.VideoNode) -> vs.VideoNode:
-    """
-    Small convenience function for interleaving clips.
-
-    :param clips:       Clips for comparison (order is kept).
-    :param namedclips:  Keyword arguments of `name=clip` for all clips in the comparison.
-                        Clips will be labeled at the top left with their `name`.
-
-    :return:            An interleaved clip of all the `clips`/`namedclips` specified.
-
-    :raises ClipsAndNamedClipsError:    Both positional and named clips are given.
-    """
-    if clips and namedclips:
-        raise ClipsAndNamedClipsError(interleave)
-    return Interleave(clips if clips else namedclips).clip
-
-
-def split(*clips: vs.VideoNode, **namedclips: vs.VideoNode) -> vs.VideoNode:
-    """
-    Small convenience function for splitting clips along the x-axis and then stacking.
-
-    Accounts for odd-resolution clips by giving overflow columns to the last clip specified.
-    All clips must have the same dimensions (width and height).
-
-    :param clips:       Clips for comparison (order is kept left to right).
-    :param namedclips:  Keyword arguments of `name=clip` for all clips in the comparison.
-                        Clips will be labeled at the bottom with their `name`.
-
-    :return:            A clip with the same dimensions as any one of the input clips.
-                        with all `clips`/`namedclips` represented as individual vertical slices.
-
-    :raises ClipsAndNamedClipsError:    Both positional and named clips are given.
-    """
-    if clips and namedclips:
-        raise ClipsAndNamedClipsError(split)
-    return Split(clips if clips else namedclips, label_alignment=2).clip
-
-
-def stack_horizontal(*clips: vs.VideoNode, **namedclips: vs.VideoNode) -> vs.VideoNode:
-    """
-    Small convenience function for stacking clips horizontally.
-
-    :param clips:       Clips for comparison (order is kept left to right).
-    :param namedclips:  Keyword arguments of `name=clip` for all clips in the comparison.
-                        Clips will be labeled at the top left with their `name`.
-
-    :return:            A horizontal stack of the `clips`/`namedclips`.
-
-    :raises ClipsAndNamedClipsError:    Both positional and named clips are given.
-    """
-    if clips and namedclips:
-        raise ClipsAndNamedClipsError(stack_horizontal)
-    return Stack(clips if clips else namedclips).clip
-
-
-def stack_vertical(*clips: vs.VideoNode, **namedclips: vs.VideoNode) -> vs.VideoNode:
-    """
-    Small convenience function for stacking clips vertically.
-
-    :param clips:       Clips for comparison (order is kept top to bottom).
-    :param namedclips:  Keyword arguments of `name=clip` for all clips in the comparison.
-                        Clips will be labeled at the top left with their `name`.
-
-    :return:            A vertical stack of the `clips`/`namedclips`.
-
-    :raises ClipsAndNamedClipsError:    Both positional and named clips are given.
-    """
-    if clips and namedclips:
-        raise ClipsAndNamedClipsError(stack_vertical)
-    return Stack(clips if clips else namedclips, direction=Direction.VERTICAL).clip
-
-
-def tile(*clips: vs.VideoNode, **namedclips: vs.VideoNode) -> vs.VideoNode:
-    """
-    Small convenience function for tiling clips in a rectangular pattern.
-
-    All clips must have the same dimensions (width and height).
-    If 3 clips are given, a 2x2 square with one blank slot will be returned.
-    If 6 clips are given, a 3x2 rectangle will be returned.
-
-    :param clips:       Clips for comparison.
-    :param namedclips:  Keyword arguments of `name=clip` for all clips in the comparison.
-                        Clips will be labeled at the top left with their `name`.
-
-    :return:            A clip with all input `clips`/`namedclips` automatically tiled most optimally
-                        into a rectangular arrrangement.
-
-    :raises ClipsAndNamedClipsError:    Both positional and named clips are given.
-    """
-    if clips and namedclips:
-        raise ClipsAndNamedClipsError(tile)
-    return Tile(clips if clips else namedclips).clip
-
-
-def source_mediainfo(filepath: str, print_mediainfo: bool = False,
-                     print_props: bool = False, **source_kwargs: Any) -> vs.VideoNode:
-    """
-    Wrap ``source`` and add MediaInfo to the clip as frameprops.
-
-    This works exactly like :py:func:`misc.source`,
-    except it further gathers information pertaining to the source file.
-    This function is meant to be used for comparisons between multiple encodes.
-
-    Alias for this function is ``lvsfunc.srcm``.
-
-    Dependencies:
-        * `pymediainfo`
-
-    :param filepath:            Path to input file.
-    :param print_mediainfo:     Print MediaInfo to stdout.
-                                This includes general, video, and audio information.
-                                Only the first track found is printed.
-    :param print_props:         Print the properties added by this function on the output clip.
-                                This is meant for comping where you want to share additional information
-                                about the sources you're comping.
-    :param source_kwargs:       Keyword arguments passed to :py:func:`misc.source`.
-
-    :raises DependencyNotFoundError: Dependencies are missing.
-
-    :return:                    Clip with MediaInfo properties added.
-    """
-    try:
-        from pymediainfo import MediaInfo  # type:ignore
-    except ModuleNotFoundError as e:
-        raise DependencyNotFoundError(source_mediainfo, e)
-
-    from pprint import pformat, pprint
-
-    # TODO: Rewrie this. It's pretty inefficient atm and has no caching.
-
-    prop_dict: dict[str, Any] = dict()
-    encset_dict: dict[str, str] = {}
-    sorted_encset: dict[str, str] = {}
-
-    filename = Path(filepath).stem
-    prop_dict.update({"filename": truncate_string(filename, 64)})
-    fallback = "Unknown"
-
-    clip = source(filepath, **source_kwargs)
-
-    stream_idx = source_kwargs.get("stream_index") or 0
-
-    mi = MediaInfo.parse(filepath)
-    gtrack = mi.general_tracks[0].to_data()
-    vtrack = mi.video_tracks[stream_idx].to_data()
-
-    # Try to obtain the grouptag to save as the output name for vspreview comping, else fall back on filename.
-    # This may not be entirely accurate, but I gotta try something!
-    if "_lossless" in filename:
-        filename = "Filtered lossless"
-
-    group = re.match(r"\[[a-zA-Z\-\u4e00-\u9fff一-]+\]", filename)
-
-    if group:
-        group = group.group(0)  # type:ignore
-
-    if print_mediainfo:
-        pprint(gtrack, sort_dicts=False, width=120, compact=True)
-        pprint(vtrack, sort_dicts=False, width=120, compact=True)
-
-    stream_size = vtrack.get("other_stream_size")
-
-    if stream_size:
-        stream_size = stream_size[-1]
-
-    prop_dict.update({
-        # Basic information
-        "encode_date": f"{gtrack.get('encoded_date', gtrack.get('file_last_modification_date', fallback)):.23}",
-        "total_filesize": gtrack.get("other_file_size", [fallback])[-1],
-        "v_filesize": stream_size or fallback,
-        # Format/writing information
-        "v_bitdepth": vtrack.get("bit_depth", fallback),
-        "v_codec": f"{vtrack.get('format', gtrack.get('video_format_list', fallback))}"
-                   + (f" ({vtrack['format_profile']})" if vtrack.get("format_profile") else ""),
-        "v_writing_library": truncate_string(vtrack.get("writing_library", fallback), 40),
-        "v_subsampling": vtrack.get("other_chroma_subsampling", [fallback])[-1],
-    })
-
-    if vtrack.get("muxing_mode") and vtrack.get("muxing_mode") == "Header stripping":
-        warnings.warn(f"Warning! {filename}'s muxing mode was set to \"Header stripping\"! Very little information "
-                      "could be gathered from the MediaInfo!", ImportWarning)
-
-    if vtrack.get("encoding_settings"):
-        # Separating useful and extra encoding settings from the long string of settings.
-        split_settings = str(vtrack.get("encoding_settings")).split(" / ")
-        aqmode: str = fallback
-
-        # TODO: Add more codecs' most useful settings
-        collected_settings: set[str] = {
-            # x265
-            "aq-bias-strength", "aq-mode", "aq-strength", "bframes", "crf", "cutree", "no-cutree", "me",
-            "no-sao", "open-gop", "psy-rd", "psy-rdoq", "qcomp", "rd", "ref", "sao", "subme", "deblock",
-            "bitrate", "vbv_maxrate", "vbv_bufsize", "no-sao-non-deblock", "sao-non-deblock",
-            "no-strong-intra-smoothing", "strong-intra-smoothing", "rc-lookahead", "merange", "zones",
-            # x264 (incl. dupes, but set will dedupe it)
-            "mbtree", "no-mbtree", "aq", "rc", "ratetol",
-        }
-
-        for x in split_settings:
-            split = x.strip().split("=")
-
-            if not collected_settings.intersection(set(split)):
-                continue
-
-            match split[0]:
-                case "cutree" | "no-cutree":
-                    split = ["cutree", str(split[0] == "cutree")]
-                case "mbtree":
-                    split = ["mbtree", str(int(split[1]) == 1)]
-                case "sao" | "no-sao":
-                    split = ["sao", str(split[0] == "sao")]
-                case "sao-non-deblock" | "no-sao-non-deblock":
-                    split = ["sao-non-deblock", str(split[0] == "sao-non-deblock")]
-                case "strong-intra-smoothing" | "no-strong-intra-smoothing":
-                    split = ["strong-intra-smoothing", str(split[0] == "strong-intra-smoothing")]
-                case "me":
-                    if vtrack.get("format") == "HEVC":
-                        split[1] = x265_me_map[int(split[1])]
-                case "aq-mode":
-                    aqmode = split[1]
-                    continue
-                case "aq-strength": split = ["aq", f"{aqmode}:{split[1]}"]
-
-            encset_dict |= {f"v_enc_settings_{split[0].replace('-', '_')}": split[1]}
-
-        sorted_encset = dict(sorted(encset_dict.items()))
-
-    if print_props:
-        print_dict = prop_dict
-
-        if vtrack.get("encoding_settings"):
-            print_dict |= {"v_encode_settings": {
-                str(k).replace("v_enc_settings_", ""): v for k, v in sorted_encset.items()
-            }}
-
-        sort = pformat(print_dict, sort_dicts=False, width=100, compact=True, indent=0)[1:-1]
-        sort = sort.replace(": {", ": {\n    ").replace("'}", "'\n}").replace("                 ", "")
-
-        clip = clip.text.Text(sort).text.FrameNum(8) \
-            .text.FrameProps(["_PictType", "_Matrix", "_Transfer", "_Primaries"], 9)
-
-    prop_dict.update(encset_dict)
-    prop_dict.update({"Name": group or filename})
-    clip = clip.std.SetFrameProps(**prop_dict)
-
-    return clip
-
-
 def comparison_shots(*clips: vs.VideoNode,
                      left: int = 0, right: int = 0, top: int = 0, bottom: int = 0,
                      height: int | None = None, kernel: KernelT = Point,
                      **namedclips: vs.VideoNode) -> vs.VideoNode:
     """
     Convenience function that crops all the given clips, optionally upscales them,
     and stacks them to allow the user to see multiple filters side-by-side.
@@ -971,15 +683,17 @@
     :param clips:       Clips for comparison (order is kept left to right).
     :param namedclips:  Keyword arguments of `name=clip` for all clips in the comparison.
                         Clips will be labeled at the top left with their `name`.
     :param left:        Left crop. Can't be negative.
     :param right:       Right crop. Can't be negative.
     :param top:         Top crop. Can't be negative.
     :param bottom:      Bottom crop. Can't be negative.
-    :param height:      Height to upscale the clips to. If `None`, do not upscale. Default: None.
+    :param height:      Height to upscale the clips to. If `None`, do not upscale.
+                        If equal to or lesser than 10, multiply the height by the given amount.
+                        Default: None.
     :param kernel:      Kernel used for upscaling the clips if applicable. Default: Point.
 
     :return:            A horizontal stack of the `clips`/`namedclips`, cropped and upscaled as specified.
 
     :raises ClipsAndNamedClipsError:    Both positional and named clips are given.
     """
     if clips and namedclips:
@@ -990,21 +704,16 @@
     if clips:
         clips = tuple([c.std.Crop(left, right, top, bottom) for c in clips])
     elif namedclips:
         namedclips = {k: v.std.Crop(left, right, top, bottom) for k, v in namedclips.items()}
 
     if height is None:
         return Stack(clips if clips else namedclips, direction=Direction.HORIZONTAL).clip
+    elif height <= 10:
+        height = mod2(clips[0].height * height)
 
     if clips:
         clips = tuple([kernel.scale(c, get_w(height), height) for c in clips])
     elif namedclips:
         namedclips = {k: kernel.scale(v, get_w(height), height) for k, v in namedclips.items()}
 
     return Stack(clips if clips else namedclips, direction=Direction.HORIZONTAL).clip
-
-
-# Aliases
-comp = compare
-scomp = stack_compare
-srcm = source_mediainfo
-cshots = comparison_shots
```

### Comparing `lvsfunc-0.7.1/lvsfunc/deblock.py` & `lvsfunc-0.8.0/lvsfunc/deblock.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,30 +5,29 @@
 
 from vsdenoise import dpir
 from vsexprtools import expr_func
 from vskernels import Catrom, Kernel, KernelT
 from vstools import CustomValueError, Matrix, check_variable, core, get_prop, vs
 
 __all__ = [
-    'autodb_dpir',
-    'dpir'
+    'autodb_dpir'
 ]
 
 
 def autodb_dpir(clip: vs.VideoNode, edgevalue: int = 24,
                 strs: Sequence[float] = [10, 50, 75],
                 thrs: Sequence[tuple[float, float, float]] = [(1.5, 2.0, 2.0), (3.0, 4.5, 4.5), (5.5, 7.0, 7.0)],
                 matrix: Matrix | int | None = None,
                 edgemasker: Callable[[vs.VideoNode], vs.VideoNode] | None = None,
                 kernel: KernelT = Catrom,
                 cuda: bool | Literal['trt'] | None = None,
                 return_mask: bool = False,
                 write_props: bool = False,
                 **vsdpir_args: Any) -> vs.VideoNode:
-    r"""
+    """
     Rewrite of fvsfunc.AutoDeblock that uses vspdir instead of dfttest to deblock.
 
     This function checks for differences between a frame and an edgemask with some processing done on it,
     and for differences between the current frame and the next frame.
     For frames where both thresholds are exceeded, it will perform deblocking at a specified strength.
     This will ideally be frames that show big temporal *and* spatial inconsistencies.
 
@@ -70,15 +69,15 @@
                             and select the fastest backend.
     :param return_mask:     Return the mask used for calculating the edgevalues.
     :param write_props:     whether to write verbose props.
     :param vsdpir_args:     Additional args to pass to :py:func:`lvsfunc.deblock.vsdpir`.
 
     :return:                Deblocked clip with different strengths applied based on the given parameters.
 
-    :raises ValueError:     Unequal number of ``strength``\s and ``thr``\s passed.
+    :raises ValueError:     Unequal number of ``strength``s and ``thr``s passed.
     """
     assert check_variable(clip, "autodb_dpir")
 
     def _eval_db(n: int, f: Sequence[vs.VideoFrame],
                  clip: vs.VideoNode, db_clips: Sequence[vs.VideoNode],
                  nthrs: Sequence[tuple[float, float, float]]) -> vs.VideoNode:
```

### Comparing `lvsfunc-0.7.1/lvsfunc/fun.py` & `lvsfunc-0.8.0/lvsfunc/fun.py`

 * *Files identical despite different names*

### Comparing `lvsfunc-0.7.1/lvsfunc/util.py` & `lvsfunc-0.8.0/lvsfunc/util.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,82 +1,30 @@
 from __future__ import annotations
 
 import colorsys
 import random
 import re
-from functools import partial
 from typing import Any
 
 from vskernels import Catrom, Kernel, KernelT
 from vstools import (
     CustomIndexError, CustomValueError, FrameRangeN, FrameRangesN, Matrix, check_variable, core, get_prop, vs
 )
 
 __all__ = [
     'colored_clips',
-    'frames_since_bookmark',
-    'load_bookmarks',
     'match_clip',
-    'truncate_string',
     'convert_rfs',
 ]
 
 
-def load_bookmarks(bookmark_path: str) -> list[int]:
+def colored_clips(
+    amount: int, max_hue: int = 300, rand: bool = True, seed: Any | None = None, **kwargs: Any
+) -> list[vs.VideoNode]:
     """
-    Load VSEdit bookmarks.
-
-    load_bookmarks(os.path.basename(__file__)+".bookmarks")
-    will load the VSEdit bookmarks for the current Vapoursynth script.
-
-    :param bookmark_path:  Path to bookmarks file.
-
-    :return:               A list of bookmarked frames.
-    """
-    with open(bookmark_path) as f:
-        bookmarks = [int(i) for i in f.read().split(", ")]
-
-        if bookmarks[0] != 0:
-            bookmarks.insert(0, 0)
-
-    return bookmarks
-
-
-def frames_since_bookmark(clip: vs.VideoNode, bookmarks: list[int]) -> vs.VideoNode:
-    """
-    Display frames since last bookmark to create easily reusable scenefiltering.
-
-    Can be used in tandem with :py:func:`lvsfunc.misc.load_bookmarks` to import VSEdit bookmarks.
-
-    :param clip:        Clip to process.
-    :param bookmarks:   A list of bookmarks.
-
-    :return:            Clip with bookmarked frames.
-    """
-    def _frames_since_bookmark(n: int, clip: vs.VideoNode, bookmarks: list[int]) -> vs.VideoNode:
-        for i, bookmark in enumerate(bookmarks):
-            frames_since = n - bookmark
-
-            if frames_since >= 0 and i + 1 >= len(bookmarks):
-                result = frames_since
-            elif frames_since >= 0 and n - bookmarks[i + 1] < 0:
-                result = frames_since
-                break
-
-        return core.text.Text(clip, str(result))
-    return core.std.FrameEval(clip, partial(_frames_since_bookmark, clip=clip, bookmarks=bookmarks))
-
-
-def colored_clips(amount: int,
-                  max_hue: int = 300,
-                  rand: bool = True,
-                  seed: bytearray | bytes | float | str | None = None,
-                  **kwargs: Any
-                  ) -> list[vs.VideoNode]:
-    r"""
     Return a list of BlankClips with unique colors in sequential or random order.
 
     The colors will be evenly spaced by hue in the HSL colorspace.
 
     Useful maybe for comparison functions or just for getting multiple uniquely colored BlankClips for testing purposes.
 
     Will always return a pure red clip in the list as this is the RGB equivalent of the lowest HSL hue possible (0).
@@ -157,22 +105,14 @@
             _Transfer=get_prop(ref_frame, '_Transfer', int),
             _Primaries=get_prop(ref_frame, '_Primaries', int)
         )
 
     return clip.std.AssumeFPS(fpsnum=ref.fps.numerator, fpsden=ref.fps.denominator)
 
 
-def truncate_string(str_in: str, max_length: int, suffix: str = "...") -> str:
-    """Truncate a string if it surpasses a certain length."""
-    if len(str_in) > max_length:
-        return str_in[:max_length - len(suffix)] + suffix
-
-    return str_in
-
-
 def convert_rfs(rfs_string: str) -> FrameRangesN:
     """
     A utility function to convert `ReplaceFramesSimple`-styled ranges to `replace_ranges`-styled ranges.
 
     This function accepts the RFS ranges as a string only. This is in line with how RFS handles them.
     The string will be validated before it's passed on. As with all framerange-related functions,
     the more ranges you have, the slower the function will become.
```

### Comparing `lvsfunc-0.7.1/lvsfunc.egg-info/PKG-INFO` & `lvsfunc-0.8.0/lvsfunc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lvsfunc
-Version: 0.7.1
+Version: 0.8.0
 Summary: Light's Vapoursynth Functions.
 Author: LightArrowsEXE
 Author-email: LightArrowsReboot@gmail.com
 Maintainer: LightArrowsEXE
 Maintainer-email: LightArrowsReboot@gmail.com
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/lvsfunc
 Project-URL: Documentation, https://lvsfunc.encode.moe/en/latest/
@@ -62,15 +62,14 @@
 ## Usage
 
 After installation, functions can be loaded and used as follows:
 
 ```py
 import lvsfunc as lvf
 
-src = lvf.misc.source(...)
 aa = lvf.aa.clamp_aa(...)
 comp = lvf.comparison.compare(...)
 ...
 ```
 
 ## Disclaimer
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lvsfunc Version: 0.7.1 Summary: Light's Vapoursynth
+Metadata-Version: 2.1 Name: lvsfunc Version: 0.8.0 Summary: Light's Vapoursynth
 Functions. Author: LightArrowsEXE Author-email: LightArrowsReboot@gmail.com
 Maintainer: LightArrowsEXE Maintainer-email: LightArrowsReboot@gmail.com
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/
 lvsfunc Project-URL: Documentation, https://lvsfunc.encode.moe/en/latest/
 Project-URL: Contact, https://discord.gg/qxTxVJGtst Classifier: Natural
 Language :: English Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Other Audience Classifier: Programming Language :: Python
@@ -19,12 +19,12 @@
 //lvsfunc.encode.moe/en/latest/). For further support, drop by `#lvsfunc` in
 the [IEW Discord server](https://discord.gg/qxTxVJGtst). ## How to install If
 you have the old `lvsfunc.py` module, remove that from your system first.
 Install `lvsfunc` with the following command: ```sh $ pip3 install lvsfunc --
 no-cache-dir -U ``` Or if you want the latest git version, install it with this
 command: ```sh $ pip3 install git+https://github.com/Irrational-Encoding-
 Wizardry/lvsfunc.git --no-cache-dir -U ``` ## Usage After installation,
-functions can be loaded and used as follows: ```py import lvsfunc as lvf src =
-lvf.misc.source(...) aa = lvf.aa.clamp_aa(...) comp = lvf.comparison.compare
-(...) ... ``` ## Disclaimer Anything **MAY** change at any time. The public API
-**SHOULD NOT** be considered stable. If you use lvsfunc in any of your
-projects, consider hardcoding a version requirement.
+functions can be loaded and used as follows: ```py import lvsfunc as lvf aa =
+lvf.aa.clamp_aa(...) comp = lvf.comparison.compare(...) ... ``` ## Disclaimer
+Anything **MAY** change at any time. The public API **SHOULD NOT** be
+considered stable. If you use lvsfunc in any of your projects, consider
+hardcoding a version requirement.
```

### Comparing `lvsfunc-0.7.1/setup.py` & `lvsfunc-0.8.0/setup.py`

 * *Files identical despite different names*

