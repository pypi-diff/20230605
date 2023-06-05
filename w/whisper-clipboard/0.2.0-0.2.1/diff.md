# Comparing `tmp/whisper-clipboard-0.2.0.tar.gz` & `tmp/whisper-clipboard-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper-clipboard-0.2.0.tar", last modified: Sun Jun  4 20:50:54 2023, max compression
+gzip compressed data, was "whisper-clipboard-0.2.1.tar", last modified: Mon Jun  5 12:28:08 2023, max compression
```

## Comparing `whisper-clipboard-0.2.0.tar` & `whisper-clipboard-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:50:54.077587 whisper-clipboard-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-04 20:50:43.000000 whisper-clipboard-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-04 20:50:54.077587 whisper-clipboard-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-04 20:50:43.000000 whisper-clipboard-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 20:50:54.077587 whisper-clipboard-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-04 20:50:43.000000 whisper-clipboard-0.2.0/setup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6486 2023-06-04 20:50:43.000000 whisper-clipboard-0.2.0/transcribe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:50:54.077587 whisper-clipboard-0.2.0/whisper_clipboard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-04 20:50:54.000000 whisper-clipboard-0.2.0/whisper_clipboard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-04 20:50:54.000000 whisper-clipboard-0.2.0/whisper_clipboard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 20:50:54.000000 whisper-clipboard-0.2.0/whisper_clipboard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-04 20:50:54.000000 whisper-clipboard-0.2.0/whisper_clipboard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-04 20:50:54.000000 whisper-clipboard-0.2.0/whisper_clipboard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-04 20:50:54.000000 whisper-clipboard-0.2.0/whisper_clipboard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:28:08.026558 whisper-clipboard-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-05 12:27:54.000000 whisper-clipboard-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-05 12:28:08.026558 whisper-clipboard-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-05 12:27:54.000000 whisper-clipboard-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 12:28:08.026558 whisper-clipboard-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-05 12:27:54.000000 whisper-clipboard-0.2.1/setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6482 2023-06-05 12:27:54.000000 whisper-clipboard-0.2.1/transcribe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:28:08.026558 whisper-clipboard-0.2.1/whisper_clipboard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-05 12:28:07.000000 whisper-clipboard-0.2.1/whisper_clipboard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-05 12:28:07.000000 whisper-clipboard-0.2.1/whisper_clipboard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 12:28:07.000000 whisper-clipboard-0.2.1/whisper_clipboard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-05 12:28:07.000000 whisper-clipboard-0.2.1/whisper_clipboard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-05 12:28:07.000000 whisper-clipboard-0.2.1/whisper_clipboard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-05 12:28:07.000000 whisper-clipboard-0.2.1/whisper_clipboard.egg-info/top_level.txt
```

### Comparing `whisper-clipboard-0.2.0/LICENSE` & `whisper-clipboard-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper-clipboard-0.2.0/PKG-INFO` & `whisper-clipboard-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-clipboard
-Version: 0.2.0
+Version: 0.2.1
 Summary: A basic TUI for transcribing audio to your clipboard using OpenAI's whisper models.
 Home-page: http://github.com/data-stepper/whisper-clipboard
 Author: Bent Mueller
 Author-email: bentmuller.ai@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `whisper-clipboard-0.2.0/README.md` & `whisper-clipboard-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `whisper-clipboard-0.2.0/setup.py` & `whisper-clipboard-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     requirements = f.read().splitlines()
 
 # Rest of your setup.py code...
 
 
 setup(
     name="whisper-clipboard",
-    version="0.2.0",
+    version="0.2.1",
     description="A basic TUI for transcribing audio to your clipboard using OpenAI's whisper models.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Bent Mueller",
     author_email="bentmuller.ai@gmail.com",
     url="http://github.com/data-stepper/whisper-clipboard",
     py_modules=["transcribe"],
```

### Comparing `whisper-clipboard-0.2.0/transcribe.py` & `whisper-clipboard-0.2.1/transcribe.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
         try:
             self.model = whisper.load_model(model_name, in_memory=True)
         except Exception as e:
             error_message = (
                 f"Failed to load whisper model '{model_name}'. Make sure the model is available and correctly configured. "
                 f"Available models are 'tiny', 'base', 'small', 'medium' and 'large'. "
-                f"When using whisper-transcribe for the first time, you need to download the models first. "
+                f"When using whisper-clipboard for the first time, you need to download the models first. "
             )
             print(error_message)
             raise type(e)(error_message).with_traceback(e.__traceback__)
 
     def start_recording(self):
         print("Recording ", end="")
         self.is_recording = True
@@ -184,27 +184,27 @@
             except KeyboardInterrupt:
                 break
 
 
 def main():
     info_string = dedent(
         """
-        Welcome to whisper-transcribe! 
+        Welcome to whisper-clipboard! 
 
         Instructions:
             Press 'Space' to start / stop recording.
             Press 'Q', Ctrl+D or Ctrl+C to quit the application.
 
             Transcriptions are automatically copied to your clipboard.
             Your average WPM (Words per minute) is also calculated for relevant languages.
             A rolling average of your WPM is also shown which gives you an idea of your average WPM.
-            Fast typists may type at 70 WPM, with whisper-transcribe you can easily achieve 90+ WPM.
+            Fast typists may type at 70 WPM, with whisper-clipboard you can easily achieve 90+ WPM.
             The calculated WPM is measured from the start of the recording to the end of the transcription.
 
-            whisper-transcribe works locally and never sends your recordings anywhere.
+            whisper-clipboard works locally and never sends your recordings anywhere.
 
         Ready to speak your mind?
 
     """
     )
     print(info_string)
```

### Comparing `whisper-clipboard-0.2.0/whisper_clipboard.egg-info/PKG-INFO` & `whisper-clipboard-0.2.1/whisper_clipboard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-clipboard
-Version: 0.2.0
+Version: 0.2.1
 Summary: A basic TUI for transcribing audio to your clipboard using OpenAI's whisper models.
 Home-page: http://github.com/data-stepper/whisper-clipboard
 Author: Bent Mueller
 Author-email: bentmuller.ai@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

