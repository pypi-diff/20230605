# Comparing `tmp/youtube-summary-0.4.tar.gz` & `tmp/youtube-summary-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youtube-summary-0.4.tar", last modified: Wed May 24 07:45:08 2023, max compression
+gzip compressed data, was "youtube-summary-0.5.tar", last modified: Mon Jun  5 16:49:58 2023, max compression
```

## Comparing `youtube-summary-0.4.tar` & `youtube-summary-0.5.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxr-xr-x   0 maorcohen   (501) staff       (20)        0 2023-05-24 07:45:08.506552 youtube-summary-0.4/
--rw-r--r--   0 maorcohen   (501) staff       (20)     1067 2023-05-21 10:58:12.000000 youtube-summary-0.4/LICENSE
--rw-r--r--   0 maorcohen   (501) staff       (20)     1621 2023-05-24 07:45:08.506368 youtube-summary-0.4/PKG-INFO
--rw-r--r--   0 maorcohen   (501) staff       (20)       38 2023-05-24 07:45:08.506596 youtube-summary-0.4/setup.cfg
--rw-r--r--   0 maorcohen   (501) staff       (20)      561 2023-05-24 07:44:45.000000 youtube-summary-0.4/setup.py
-drwxr-xr-x   0 maorcohen   (501) staff       (20)        0 2023-05-24 07:45:08.505402 youtube-summary-0.4/youtube_summary/
--rw-r--r--   0 maorcohen   (501) staff       (20)        0 2023-05-21 18:58:41.000000 youtube-summary-0.4/youtube_summary/__init__.py
--rw-r--r--   0 maorcohen   (501) staff       (20)       29 2023-05-22 10:23:51.000000 youtube-summary-0.4/youtube_summary/__main__.py
--rw-r--r--   0 maorcohen   (501) staff       (20)     7305 2023-05-24 07:43:48.000000 youtube-summary-0.4/youtube_summary/main.py
-drwxr-xr-x   0 maorcohen   (501) staff       (20)        0 2023-05-24 07:45:08.506156 youtube-summary-0.4/youtube_summary.egg-info/
--rw-r--r--   0 maorcohen   (501) staff       (20)     1621 2023-05-24 07:45:08.000000 youtube-summary-0.4/youtube_summary.egg-info/PKG-INFO
--rw-r--r--   0 maorcohen   (501) staff       (20)      332 2023-05-24 07:45:08.000000 youtube-summary-0.4/youtube_summary.egg-info/SOURCES.txt
--rw-r--r--   0 maorcohen   (501) staff       (20)        1 2023-05-24 07:45:08.000000 youtube-summary-0.4/youtube_summary.egg-info/dependency_links.txt
--rw-r--r--   0 maorcohen   (501) staff       (20)       61 2023-05-24 07:45:08.000000 youtube-summary-0.4/youtube_summary.egg-info/entry_points.txt
--rw-r--r--   0 maorcohen   (501) staff       (20)     1050 2023-05-24 07:45:08.000000 youtube-summary-0.4/youtube_summary.egg-info/requires.txt
--rw-r--r--   0 maorcohen   (501) staff       (20)       16 2023-05-24 07:45:08.000000 youtube-summary-0.4/youtube_summary.egg-info/top_level.txt
+drwxr-xr-x   0 maorcohen   (501) staff       (20)        0 2023-06-05 16:49:58.136094 youtube-summary-0.5/
+-rw-r--r--   0 maorcohen   (501) staff       (20)     1067 2023-05-21 10:58:12.000000 youtube-summary-0.5/LICENSE
+-rw-r--r--   0 maorcohen   (501) staff       (20)     2060 2023-06-05 16:49:58.135861 youtube-summary-0.5/PKG-INFO
+-rw-r--r--   0 maorcohen   (501) staff       (20)       38 2023-06-05 16:49:58.136172 youtube-summary-0.5/setup.cfg
+-rw-r--r--   0 maorcohen   (501) staff       (20)      561 2023-06-05 16:49:14.000000 youtube-summary-0.5/setup.py
+drwxr-xr-x   0 maorcohen   (501) staff       (20)        0 2023-06-05 16:49:58.134739 youtube-summary-0.5/youtube_summary/
+-rw-r--r--   0 maorcohen   (501) staff       (20)        0 2023-05-21 18:58:41.000000 youtube-summary-0.5/youtube_summary/__init__.py
+-rw-r--r--   0 maorcohen   (501) staff       (20)       29 2023-05-22 10:23:51.000000 youtube-summary-0.5/youtube_summary/__main__.py
+-rw-r--r--   0 maorcohen   (501) staff       (20)     3500 2023-06-05 16:15:06.000000 youtube-summary-0.5/youtube_summary/main.py
+-rw-r--r--   0 maorcohen   (501) staff       (20)     1535 2023-06-05 16:11:38.000000 youtube-summary-0.5/youtube_summary/overall_summarizer.py
+-rw-r--r--   0 maorcohen   (501) staff       (20)     3029 2023-06-05 16:05:06.000000 youtube-summary-0.5/youtube_summary/section_summarizer.py
+-rw-r--r--   0 maorcohen   (501) staff       (20)      771 2023-06-05 16:14:46.000000 youtube-summary-0.5/youtube_summary/transcript.py
+-rw-r--r--   0 maorcohen   (501) staff       (20)      685 2023-06-05 15:43:23.000000 youtube-summary-0.5/youtube_summary/video_infromation.py
+drwxr-xr-x   0 maorcohen   (501) staff       (20)        0 2023-06-05 16:49:58.135641 youtube-summary-0.5/youtube_summary.egg-info/
+-rw-r--r--   0 maorcohen   (501) staff       (20)     2060 2023-06-05 16:49:58.000000 youtube-summary-0.5/youtube_summary.egg-info/PKG-INFO
+-rw-r--r--   0 maorcohen   (501) staff       (20)      475 2023-06-05 16:49:58.000000 youtube-summary-0.5/youtube_summary.egg-info/SOURCES.txt
+-rw-r--r--   0 maorcohen   (501) staff       (20)        1 2023-06-05 16:49:58.000000 youtube-summary-0.5/youtube_summary.egg-info/dependency_links.txt
+-rw-r--r--   0 maorcohen   (501) staff       (20)       61 2023-06-05 16:49:58.000000 youtube-summary-0.5/youtube_summary.egg-info/entry_points.txt
+-rw-r--r--   0 maorcohen   (501) staff       (20)     1050 2023-06-05 16:49:58.000000 youtube-summary-0.5/youtube_summary.egg-info/requires.txt
+-rw-r--r--   0 maorcohen   (501) staff       (20)       16 2023-06-05 16:49:58.000000 youtube-summary-0.5/youtube_summary.egg-info/top_level.txt
```

### Comparing `youtube-summary-0.4/LICENSE` & `youtube-summary-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `youtube-summary-0.4/PKG-INFO` & `youtube-summary-0.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,66 +1,76 @@
 Metadata-Version: 2.1
 Name: youtube-summary
-Version: 0.4
+Version: 0.5
 Home-page: https://github.com/mmaorc/youtube-summary-cli
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # YouTube Summary CLI
 
-A simple CLI tool that summarizes YouTube videos.
+A simple CLI tool that summarizes YouTube videos. This tool is designed to help users quickly understand the main points of a video without having to watch the entire content. It uses AI to generate a concise summary of the video's transcript.
 
 ![Screenshot](./docs/screenshot.png)
 
 The timestamps are also clickable, try them 🙂
 
-## Installation
+## Usage
+
+### Installation
 
-### Install from PyPi
 You can install the application using `pip` or `pipx`:
 ```bash
 pip install --user youtube-summary
-```
-or
-```bash
 pipx install youtube-summary
 ```
 
-### Compile from source
-
-You can compile directly from source:
+You can also compile directly from source:
 ```bash
 git clone https://github.com/mmaorc/youtube-summary-cli
 cd youtube-summary-cli
 python setup.py install --user
 ```
 
+### Run
+
+Prior to running the script, ensure that the `OPENAI_API_KEY` environment variable is set up correctly.
+
+To summarize the transcript of a YouTube video, run the app with the video URL as an argument:
+
+```bash
+youtube-summary "https://www.youtube.com/watch?v=your_video_id"
+```
+
+Replace `your_video_id` with the actual video ID.
 
-### Development
+Note that generating a summary might take a couple of minutes, depending on the video's transcript length.
+
+
+## Development
 For development purposes, clone the repository, navigate to the project directory, and install in a virtual environment:
 
 ```bash
 git clone https://github.com/mmaorc/youtube-summary-cli
 cd youtube-summary-cli
 python -m venv .env
 source .env/bin/activate  # On Windows use `.env\Scripts\activate`
 pip install --editable .
 ```
 
+Ensure that the `OPENAI_API_KEY` environment variable is set up correctly.
 
-## Usage
-
-Prior to running the script, ensure that the `OPENAI_API_KEY` environment variable is set up correctly.
-
-To summarize the transcript of a YouTube video, run the `app.py` script with the video URL as an argument:
-
+Now you can run it:
 ```bash
-youtube-summary "https://www.youtube.com/watch?v=your_video_id"
+python -m youtube_summary "https://www.youtube.com/watch?v=your_video_id"
 ```
 
 Replace `your_video_id` with the actual video ID.
 
-Note that generating a summary might take a couple of minutes, depending on the video's transcript length.
 
 ## License
 
 This project is licensed under the MIT License. See the [LICENSE](./LICENSE) file for details.
+
+
+## Contact Me
+
+You can find me on [Twitter](https://bit.ly/43ow5WT).
```

### Comparing `youtube-summary-0.4/setup.py` & `youtube-summary-0.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="youtube-summary",
-    version="0.4",
+    version="0.5",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     url="https://github.com/mmaorc/youtube-summary-cli",
     install_requires=[line.strip() for line in open("requirements.txt")],
     entry_points={
         "console_scripts": [
```

### Comparing `youtube-summary-0.4/youtube_summary.egg-info/PKG-INFO` & `youtube-summary-0.5/youtube_summary.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,66 +1,76 @@
 Metadata-Version: 2.1
 Name: youtube-summary
-Version: 0.4
+Version: 0.5
 Home-page: https://github.com/mmaorc/youtube-summary-cli
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # YouTube Summary CLI
 
-A simple CLI tool that summarizes YouTube videos.
+A simple CLI tool that summarizes YouTube videos. This tool is designed to help users quickly understand the main points of a video without having to watch the entire content. It uses AI to generate a concise summary of the video's transcript.
 
 ![Screenshot](./docs/screenshot.png)
 
 The timestamps are also clickable, try them 🙂
 
-## Installation
+## Usage
+
+### Installation
 
-### Install from PyPi
 You can install the application using `pip` or `pipx`:
 ```bash
 pip install --user youtube-summary
-```
-or
-```bash
 pipx install youtube-summary
 ```
 
-### Compile from source
-
-You can compile directly from source:
+You can also compile directly from source:
 ```bash
 git clone https://github.com/mmaorc/youtube-summary-cli
 cd youtube-summary-cli
 python setup.py install --user
 ```
 
+### Run
+
+Prior to running the script, ensure that the `OPENAI_API_KEY` environment variable is set up correctly.
+
+To summarize the transcript of a YouTube video, run the app with the video URL as an argument:
+
+```bash
+youtube-summary "https://www.youtube.com/watch?v=your_video_id"
+```
+
+Replace `your_video_id` with the actual video ID.
 
-### Development
+Note that generating a summary might take a couple of minutes, depending on the video's transcript length.
+
+
+## Development
 For development purposes, clone the repository, navigate to the project directory, and install in a virtual environment:
 
 ```bash
 git clone https://github.com/mmaorc/youtube-summary-cli
 cd youtube-summary-cli
 python -m venv .env
 source .env/bin/activate  # On Windows use `.env\Scripts\activate`
 pip install --editable .
 ```
 
+Ensure that the `OPENAI_API_KEY` environment variable is set up correctly.
 
-## Usage
-
-Prior to running the script, ensure that the `OPENAI_API_KEY` environment variable is set up correctly.
-
-To summarize the transcript of a YouTube video, run the `app.py` script with the video URL as an argument:
-
+Now you can run it:
 ```bash
-youtube-summary "https://www.youtube.com/watch?v=your_video_id"
+python -m youtube_summary "https://www.youtube.com/watch?v=your_video_id"
 ```
 
 Replace `your_video_id` with the actual video ID.
 
-Note that generating a summary might take a couple of minutes, depending on the video's transcript length.
 
 ## License
 
 This project is licensed under the MIT License. See the [LICENSE](./LICENSE) file for details.
+
+
+## Contact Me
+
+You can find me on [Twitter](https://bit.ly/43ow5WT).
```

### Comparing `youtube-summary-0.4/youtube_summary.egg-info/requires.txt` & `youtube-summary-0.5/youtube_summary.egg-info/requires.txt`

 * *Files identical despite different names*

