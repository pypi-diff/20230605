# Comparing `tmp/midi-clip-0.8.tar.gz` & `tmp/midi-clip-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midi-clip-0.8.tar", last modified: Mon Jun  5 02:13:56 2023, max compression
+gzip compressed data, was "midi-clip-0.9.tar", last modified: Mon Jun  5 02:16:37 2023, max compression
```

## Comparing `midi-clip-0.8.tar` & `midi-clip-0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 hyunshin   (501) staff       (20)        0 2023-06-05 02:13:56.278272 midi-clip-0.8/
--rw-r--r--   0 hyunshin   (501) staff       (20)      758 2023-06-01 05:50:44.000000 midi-clip-0.8/LICENSE.md
--rw-r--r--   0 hyunshin   (501) staff       (20)     2322 2023-06-05 02:13:56.278010 midi-clip-0.8/PKG-INFO
--rw-r--r--   0 hyunshin   (501) staff       (20)     2049 2023-06-05 02:12:05.000000 midi-clip-0.8/README.md
-drwxr-xr-x   0 hyunshin   (501) staff       (20)        0 2023-06-05 02:13:56.274944 midi-clip-0.8/midi_clip/
--rw-r--r--   0 hyunshin   (501) staff       (20)       74 2023-06-01 09:19:37.000000 midi-clip-0.8/midi_clip/__init__.py
--rw-r--r--   0 hyunshin   (501) staff       (20)    17959 2023-06-01 10:33:40.000000 midi-clip-0.8/midi_clip/midi_clip.py
--rw-r--r--   0 hyunshin   (501) staff       (20)     2838 2023-06-01 09:19:09.000000 midi-clip-0.8/midi_clip/midi_duration.py
-drwxr-xr-x   0 hyunshin   (501) staff       (20)        0 2023-06-05 02:13:56.277620 midi-clip-0.8/midi_clip.egg-info/
--rw-r--r--   0 hyunshin   (501) staff       (20)     2322 2023-06-05 02:13:56.000000 midi-clip-0.8/midi_clip.egg-info/PKG-INFO
--rw-r--r--   0 hyunshin   (501) staff       (20)      265 2023-06-05 02:13:56.000000 midi-clip-0.8/midi_clip.egg-info/SOURCES.txt
--rw-r--r--   0 hyunshin   (501) staff       (20)        1 2023-06-05 02:13:56.000000 midi-clip-0.8/midi_clip.egg-info/dependency_links.txt
--rw-r--r--   0 hyunshin   (501) staff       (20)        5 2023-06-05 02:13:56.000000 midi-clip-0.8/midi_clip.egg-info/requires.txt
--rw-r--r--   0 hyunshin   (501) staff       (20)       10 2023-06-05 02:13:56.000000 midi-clip-0.8/midi_clip.egg-info/top_level.txt
--rw-r--r--   0 hyunshin   (501) staff       (20)       38 2023-06-05 02:13:56.278372 midi-clip-0.8/setup.cfg
--rw-r--r--   0 hyunshin   (501) staff       (20)      650 2023-06-05 02:13:24.000000 midi-clip-0.8/setup.py
+drwxr-xr-x   0 hyunshin   (501) staff       (20)        0 2023-06-05 02:16:37.867652 midi-clip-0.9/
+-rw-r--r--   0 hyunshin   (501) staff       (20)      758 2023-06-01 05:50:44.000000 midi-clip-0.9/LICENSE.md
+-rw-r--r--   0 hyunshin   (501) staff       (20)     2342 2023-06-05 02:16:37.867412 midi-clip-0.9/PKG-INFO
+-rw-r--r--   0 hyunshin   (501) staff       (20)     2069 2023-06-05 02:16:11.000000 midi-clip-0.9/README.md
+drwxr-xr-x   0 hyunshin   (501) staff       (20)        0 2023-06-05 02:16:37.865208 midi-clip-0.9/midi_clip/
+-rw-r--r--   0 hyunshin   (501) staff       (20)       74 2023-06-01 09:19:37.000000 midi-clip-0.9/midi_clip/__init__.py
+-rw-r--r--   0 hyunshin   (501) staff       (20)    17959 2023-06-01 10:33:40.000000 midi-clip-0.9/midi_clip/midi_clip.py
+-rw-r--r--   0 hyunshin   (501) staff       (20)     2838 2023-06-01 09:19:09.000000 midi-clip-0.9/midi_clip/midi_duration.py
+drwxr-xr-x   0 hyunshin   (501) staff       (20)        0 2023-06-05 02:16:37.867060 midi-clip-0.9/midi_clip.egg-info/
+-rw-r--r--   0 hyunshin   (501) staff       (20)     2342 2023-06-05 02:16:37.000000 midi-clip-0.9/midi_clip.egg-info/PKG-INFO
+-rw-r--r--   0 hyunshin   (501) staff       (20)      265 2023-06-05 02:16:37.000000 midi-clip-0.9/midi_clip.egg-info/SOURCES.txt
+-rw-r--r--   0 hyunshin   (501) staff       (20)        1 2023-06-05 02:16:37.000000 midi-clip-0.9/midi_clip.egg-info/dependency_links.txt
+-rw-r--r--   0 hyunshin   (501) staff       (20)        5 2023-06-05 02:16:37.000000 midi-clip-0.9/midi_clip.egg-info/requires.txt
+-rw-r--r--   0 hyunshin   (501) staff       (20)       10 2023-06-05 02:16:37.000000 midi-clip-0.9/midi_clip.egg-info/top_level.txt
+-rw-r--r--   0 hyunshin   (501) staff       (20)       38 2023-06-05 02:16:37.867742 midi-clip-0.9/setup.cfg
+-rw-r--r--   0 hyunshin   (501) staff       (20)      650 2023-06-05 02:16:30.000000 midi-clip-0.9/setup.py
```

### Comparing `midi-clip-0.8/LICENSE.md` & `midi-clip-0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `midi-clip-0.8/PKG-INFO` & `midi-clip-0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midi-clip
-Version: 0.8
+Version: 0.9
 Summary: A python package for midi clip.
 Home-page: https://github.com/kyaryunha/midi-clip
 Author: kyaryunha
 Author-email: kyaryunha@gmail.com
 License: ISC
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -55,16 +55,16 @@
 <tr>
 <td></td>
 <td>0s-30s</td>
 <td>5s-15s</td>
 </tr>
 <tr>
 <td>Piano Roll</td>
-<td><img src="https://github.com/kyaryunha/midi-clip/blob/main/example/ocean_0_30.png" /></td>
-<td><img src="https://github.com/kyaryunha/midi-clip/blob/main/example/ocean_5_15.png" /></td>
+<td><img src="https://raw.githubusercontent.com/kyaryunha/midi-clip/main/example/ocean_0_30.png" /></td>
+<td><img src="https://raw.githubusercontent.com/kyaryunha/midi-clip/main/example/ocean_5_15.png" /></td>
 </tr>
 <tr>
 <td>Audio</td>
 <td>https://github.com/kyaryunha/midi-clip/blob/main/example/ocean_0_30.wav</td>
 <td>https://github.com/kyaryunha/midi-clip/blob/main/example/ocean_5_15.wav</td>
 </tr>
 </table>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: midi-clip Version: 0.8 Summary: A python package
+Metadata-Version: 2.1 Name: midi-clip Version: 0.9 Summary: A python package
 for midi clip. Home-page: https://github.com/kyaryunha/midi-clip Author:
 kyaryunha Author-email: kyaryunha@gmail.com License: ISC Description-Content-
 Type: text/markdown License-File: LICENSE.md # midi-clip [![PyPI](https://
 img.shields.io/pypi/v/midi-clip.svg)](https://pypi.python.org/pypi/midi-clip) A
 python package for midi clip (and midi duration) based on mido. ([github]
 (https://github.com/kyaryunha/midi-clip)) Author: Hyun Shin ([kyaryunha](https:
 //github.com/kyaryunha)) ### Introduce This library considers a lot of things
@@ -15,18 +15,19 @@
 ```python import mido import midi_clip # load midi use mido mid = mido.MidiFile
 ('resources/hosu.mid') # clip midi output_mid = midi_clip.midi_clip(mid, 5.,
 15.) # you can get total duration(second) of midi duration =
 midi_clip.midi_duration(output_mid) # if you see by print print(output_mid,
 duration) # if you save midi clip output_mid.save('output.mid') ``` ### Result
 Result of clip "A Town With An Ocean View" MIDI from 0 to 30 seconds and from 5
 to 15 seconds.
-           0s-30s                         5s-15s
-           [https://github.com/kyaryunha/ [https://github.com/kyaryunha/
-Piano Roll midi-clip/blob/main/example/   midi-clip/blob/main/example/
-           ocean_0_30.png]                ocean_5_15.png]
-           https://github.com/kyaryunha/  https://github.com/kyaryunha/midi-
-Audio      midi-clip/blob/main/example/   clip/blob/main/example/
-           ocean_0_30.wav                 ocean_5_15.wav
+           0s-30s                            5s-15s
+           [https://                         [https://
+Piano Roll raw.githubusercontent.com/        raw.githubusercontent.com/
+           kyaryunha/midi-clip/main/example/ kyaryunha/midi-clip/main/example/
+           ocean_0_30.png]                   ocean_5_15.png]
+           https://github.com/kyaryunha/     https://github.com/kyaryunha/midi-
+Audio      midi-clip/blob/main/example/      clip/blob/main/example/
+           ocean_0_30.wav                    ocean_5_15.wav
 ** Used GarageBand to obtain piano roll images and Cubase to obtain audio.
 GarageBand and Cubase fill in the measure regardless of the actual end of track
 time in the MIDI, resulting in slightly longer audio. MIDI file's time clip is
 precisely. ** Data used for result was allowed by an anonymous artist.
```

### Comparing `midi-clip-0.8/README.md` & `midi-clip-0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -44,16 +44,16 @@
 <tr>
 <td></td>
 <td>0s-30s</td>
 <td>5s-15s</td>
 </tr>
 <tr>
 <td>Piano Roll</td>
-<td><img src="https://github.com/kyaryunha/midi-clip/blob/main/example/ocean_0_30.png" /></td>
-<td><img src="https://github.com/kyaryunha/midi-clip/blob/main/example/ocean_5_15.png" /></td>
+<td><img src="https://raw.githubusercontent.com/kyaryunha/midi-clip/main/example/ocean_0_30.png" /></td>
+<td><img src="https://raw.githubusercontent.com/kyaryunha/midi-clip/main/example/ocean_5_15.png" /></td>
 </tr>
 <tr>
 <td>Audio</td>
 <td>https://github.com/kyaryunha/midi-clip/blob/main/example/ocean_0_30.wav</td>
 <td>https://github.com/kyaryunha/midi-clip/blob/main/example/ocean_5_15.wav</td>
 </tr>
 </table>
```

#### html2text {}

```diff
@@ -11,18 +11,19 @@
 midi-clip ``` ```python import mido import midi_clip # load midi use mido mid =
 mido.MidiFile('resources/hosu.mid') # clip midi output_mid =
 midi_clip.midi_clip(mid, 5., 15.) # you can get total duration(second) of midi
 duration = midi_clip.midi_duration(output_mid) # if you see by print print
 (output_mid, duration) # if you save midi clip output_mid.save('output.mid')
 ``` ### Result Result of clip "A Town With An Ocean View" MIDI from 0 to 30
 seconds and from 5 to 15 seconds.
-           0s-30s                         5s-15s
-           [https://github.com/kyaryunha/ [https://github.com/kyaryunha/
-Piano Roll midi-clip/blob/main/example/   midi-clip/blob/main/example/
-           ocean_0_30.png]                ocean_5_15.png]
-           https://github.com/kyaryunha/  https://github.com/kyaryunha/midi-
-Audio      midi-clip/blob/main/example/   clip/blob/main/example/
-           ocean_0_30.wav                 ocean_5_15.wav
+           0s-30s                            5s-15s
+           [https://                         [https://
+Piano Roll raw.githubusercontent.com/        raw.githubusercontent.com/
+           kyaryunha/midi-clip/main/example/ kyaryunha/midi-clip/main/example/
+           ocean_0_30.png]                   ocean_5_15.png]
+           https://github.com/kyaryunha/     https://github.com/kyaryunha/midi-
+Audio      midi-clip/blob/main/example/      clip/blob/main/example/
+           ocean_0_30.wav                    ocean_5_15.wav
 ** Used GarageBand to obtain piano roll images and Cubase to obtain audio.
 GarageBand and Cubase fill in the measure regardless of the actual end of track
 time in the MIDI, resulting in slightly longer audio. MIDI file's time clip is
 precisely. ** Data used for result was allowed by an anonymous artist.
```

### Comparing `midi-clip-0.8/midi_clip/midi_clip.py` & `midi-clip-0.9/midi_clip/midi_clip.py`

 * *Files identical despite different names*

### Comparing `midi-clip-0.8/midi_clip/midi_duration.py` & `midi-clip-0.9/midi_clip/midi_duration.py`

 * *Files identical despite different names*

### Comparing `midi-clip-0.8/midi_clip.egg-info/PKG-INFO` & `midi-clip-0.9/midi_clip.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midi-clip
-Version: 0.8
+Version: 0.9
 Summary: A python package for midi clip.
 Home-page: https://github.com/kyaryunha/midi-clip
 Author: kyaryunha
 Author-email: kyaryunha@gmail.com
 License: ISC
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -55,16 +55,16 @@
 <tr>
 <td></td>
 <td>0s-30s</td>
 <td>5s-15s</td>
 </tr>
 <tr>
 <td>Piano Roll</td>
-<td><img src="https://github.com/kyaryunha/midi-clip/blob/main/example/ocean_0_30.png" /></td>
-<td><img src="https://github.com/kyaryunha/midi-clip/blob/main/example/ocean_5_15.png" /></td>
+<td><img src="https://raw.githubusercontent.com/kyaryunha/midi-clip/main/example/ocean_0_30.png" /></td>
+<td><img src="https://raw.githubusercontent.com/kyaryunha/midi-clip/main/example/ocean_5_15.png" /></td>
 </tr>
 <tr>
 <td>Audio</td>
 <td>https://github.com/kyaryunha/midi-clip/blob/main/example/ocean_0_30.wav</td>
 <td>https://github.com/kyaryunha/midi-clip/blob/main/example/ocean_5_15.wav</td>
 </tr>
 </table>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: midi-clip Version: 0.8 Summary: A python package
+Metadata-Version: 2.1 Name: midi-clip Version: 0.9 Summary: A python package
 for midi clip. Home-page: https://github.com/kyaryunha/midi-clip Author:
 kyaryunha Author-email: kyaryunha@gmail.com License: ISC Description-Content-
 Type: text/markdown License-File: LICENSE.md # midi-clip [![PyPI](https://
 img.shields.io/pypi/v/midi-clip.svg)](https://pypi.python.org/pypi/midi-clip) A
 python package for midi clip (and midi duration) based on mido. ([github]
 (https://github.com/kyaryunha/midi-clip)) Author: Hyun Shin ([kyaryunha](https:
 //github.com/kyaryunha)) ### Introduce This library considers a lot of things
@@ -15,18 +15,19 @@
 ```python import mido import midi_clip # load midi use mido mid = mido.MidiFile
 ('resources/hosu.mid') # clip midi output_mid = midi_clip.midi_clip(mid, 5.,
 15.) # you can get total duration(second) of midi duration =
 midi_clip.midi_duration(output_mid) # if you see by print print(output_mid,
 duration) # if you save midi clip output_mid.save('output.mid') ``` ### Result
 Result of clip "A Town With An Ocean View" MIDI from 0 to 30 seconds and from 5
 to 15 seconds.
-           0s-30s                         5s-15s
-           [https://github.com/kyaryunha/ [https://github.com/kyaryunha/
-Piano Roll midi-clip/blob/main/example/   midi-clip/blob/main/example/
-           ocean_0_30.png]                ocean_5_15.png]
-           https://github.com/kyaryunha/  https://github.com/kyaryunha/midi-
-Audio      midi-clip/blob/main/example/   clip/blob/main/example/
-           ocean_0_30.wav                 ocean_5_15.wav
+           0s-30s                            5s-15s
+           [https://                         [https://
+Piano Roll raw.githubusercontent.com/        raw.githubusercontent.com/
+           kyaryunha/midi-clip/main/example/ kyaryunha/midi-clip/main/example/
+           ocean_0_30.png]                   ocean_5_15.png]
+           https://github.com/kyaryunha/     https://github.com/kyaryunha/midi-
+Audio      midi-clip/blob/main/example/      clip/blob/main/example/
+           ocean_0_30.wav                    ocean_5_15.wav
 ** Used GarageBand to obtain piano roll images and Cubase to obtain audio.
 GarageBand and Cubase fill in the measure regardless of the actual end of track
 time in the MIDI, resulting in slightly longer audio. MIDI file's time clip is
 precisely. ** Data used for result was allowed by an anonymous artist.
```

### Comparing `midi-clip-0.8/setup.py` & `midi-clip-0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="midi-clip",
-    version="0.8",
+    version="0.9",
     packages=find_packages(),
     description="A python package for midi clip.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="kyaryunha",
     author_email="kyaryunha@gmail.com",
     license="ISC",
```

