# Comparing `tmp/term-image-0.6.1.tar.gz` & `tmp/term-image-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "term-image-0.6.1.tar", last modified: Sun Apr 30 18:57:28 2023, max compression
+gzip compressed data, was "term-image-0.7.0.tar", last modified: Sun Jun  4 23:34:49 2023, max compression
```

## Comparing `term-image-0.6.1.tar` & `term-image-0.7.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-04-30 18:57:28.145185 term-image-0.6.1/
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     1076 2023-03-06 12:44:15.000000 term-image-0.6.1/LICENSE
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     9747 2023-04-30 18:57:28.145185 term-image-0.6.1/PKG-INFO
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     8125 2023-04-30 17:57:47.000000 term-image-0.6.1/README.md
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)      268 2023-03-29 13:56:11.000000 term-image-0.6.1/pyproject.toml
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)       38 2023-04-30 18:57:28.145185 term-image-0.6.1/setup.cfg
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     2025 2023-04-30 18:56:54.000000 term-image-0.6.1/setup.py
-drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-04-30 18:57:28.138519 term-image-0.6.1/src/
-drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-04-30 18:57:28.141852 term-image-0.6.1/src/term_image/
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     6539 2023-04-30 18:56:54.000000 term-image-0.6.1/src/term_image/__init__.py
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     2499 2023-03-20 16:23:42.000000 term-image-0.6.1/src/term_image/exceptions.py
-drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-04-30 18:57:28.141852 term-image-0.6.1/src/term_image/image/
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     2502 2023-03-30 03:34:36.000000 term-image-0.6.1/src/term_image/image/__init__.py
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     5965 2023-03-25 21:38:19.000000 term-image-0.6.1/src/term_image/image/block.py
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    85250 2023-04-30 18:56:54.000000 term-image-0.6.1/src/term_image/image/common.py
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    28024 2023-04-30 18:56:54.000000 term-image-0.6.1/src/term_image/image/iterm2.py
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    21887 2023-04-30 18:56:54.000000 term-image-0.6.1/src/term_image/image/kitty.py
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    28444 2023-04-22 04:14:12.000000 term-image-0.6.1/src/term_image/utils.py
-drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-04-30 18:57:28.145185 term-image-0.6.1/src/term_image/widget/
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)      305 2023-03-06 02:28:38.000000 term-image-0.6.1/src/term_image/widget/__init__.py
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    24532 2023-04-30 18:56:54.000000 term-image-0.6.1/src/term_image/widget/urwid.py
-drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-04-30 18:57:28.141852 term-image-0.6.1/src/term_image.egg-info/
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     9747 2023-04-30 18:57:28.000000 term-image-0.6.1/src/term_image.egg-info/PKG-INFO
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)      577 2023-04-30 18:57:28.000000 term-image-0.6.1/src/term_image.egg-info/SOURCES.txt
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)        1 2023-04-30 18:57:28.000000 term-image-0.6.1/src/term_image.egg-info/dependency_links.txt
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)       38 2023-04-30 18:57:28.000000 term-image-0.6.1/src/term_image.egg-info/requires.txt
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)       11 2023-04-30 18:57:28.000000 term-image-0.6.1/src/term_image.egg-info/top_level.txt
-drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-04-30 18:57:28.145185 term-image-0.6.1/tests/
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    13479 2023-03-30 13:54:35.000000 term-image-0.6.1/tests/test_iterator.py
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     2036 2023-02-28 01:12:57.000000 term-image-0.6.1/tests/test_top_level.py
+drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-06-04 23:34:49.588169 term-image-0.7.0/
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     1076 2023-03-06 12:44:15.000000 term-image-0.7.0/LICENSE
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     9953 2023-06-04 23:34:49.588169 term-image-0.7.0/PKG-INFO
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     8331 2023-06-04 17:56:26.000000 term-image-0.7.0/README.md
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)      268 2023-03-29 13:56:11.000000 term-image-0.7.0/pyproject.toml
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)       38 2023-06-04 23:34:49.588169 term-image-0.7.0/setup.cfg
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     2025 2023-06-04 22:54:12.000000 term-image-0.7.0/setup.py
+drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-06-04 23:34:49.584836 term-image-0.7.0/src/
+drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-06-04 23:34:49.584836 term-image-0.7.0/src/term_image/
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     6360 2023-06-04 22:54:12.000000 term-image-0.7.0/src/term_image/__init__.py
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     3592 2023-06-04 17:56:26.000000 term-image-0.7.0/src/term_image/ctlseqs.py
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     1062 2023-06-04 17:56:26.000000 term-image-0.7.0/src/term_image/exceptions.py
+drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-06-04 23:34:49.588169 term-image-0.7.0/src/term_image/image/
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     2378 2023-06-04 17:56:26.000000 term-image-0.7.0/src/term_image/image/__init__.py
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     5909 2023-05-25 05:11:38.000000 term-image-0.7.0/src/term_image/image/block.py
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    77517 2023-06-04 17:56:26.000000 term-image-0.7.0/src/term_image/image/common.py
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    28372 2023-06-04 17:56:26.000000 term-image-0.7.0/src/term_image/image/iterm2.py
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    22241 2023-06-04 17:56:26.000000 term-image-0.7.0/src/term_image/image/kitty.py
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    26782 2023-06-04 17:56:26.000000 term-image-0.7.0/src/term_image/utils.py
+drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-06-04 23:34:49.588169 term-image-0.7.0/src/term_image/widget/
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)      305 2023-03-06 02:28:38.000000 term-image-0.7.0/src/term_image/widget/__init__.py
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    25840 2023-06-04 23:03:30.000000 term-image-0.7.0/src/term_image/widget/urwid.py
+drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-06-04 23:34:49.588169 term-image-0.7.0/src/term_image.egg-info/
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     9953 2023-06-04 23:34:49.000000 term-image-0.7.0/src/term_image.egg-info/PKG-INFO
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)      603 2023-06-04 23:34:49.000000 term-image-0.7.0/src/term_image.egg-info/SOURCES.txt
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)        1 2023-06-04 23:34:49.000000 term-image-0.7.0/src/term_image.egg-info/dependency_links.txt
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)       38 2023-06-04 23:34:49.000000 term-image-0.7.0/src/term_image.egg-info/requires.txt
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)       11 2023-06-04 23:34:49.000000 term-image-0.7.0/src/term_image.egg-info/top_level.txt
+drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-06-04 23:34:49.588169 term-image-0.7.0/tests/
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    13187 2023-06-04 17:56:26.000000 term-image-0.7.0/tests/test_iterator.py
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     1984 2023-05-25 05:11:38.000000 term-image-0.7.0/tests/test_top_level.py
```

### Comparing `term-image-0.6.1/LICENSE` & `term-image-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `term-image-0.6.1/PKG-INFO` & `term-image-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: term-image
-Version: 0.6.1
+Version: 0.7.0
 Summary: Display images in the terminal
 Home-page: https://github.com/AnonymouX47/term-image
 Author: Toluwaleke Ogundipe
 Author-email: anonymoux47@gmail.com
 License: MIT
 Project-URL: Changelog, https://github.com/AnonymouX47/term-image/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://term-image.readthedocs.io/
@@ -29,24 +29,20 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Terminals :: Terminal Emulators/X Terminals
 Classifier: Topic :: Multimedia :: Graphics :: Viewers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<a href="https://www.buymeacoffee.com/anonymoux47" target="_blank">
-   <img align="right" src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" >
-</a><br><br>
-
 <div align="center">
 
 <h1><b>Term-Image</b></h1>
 
 <p>
-<img src="https://raw.githubusercontent.com/AnonymouX47/term-image/abca69a2cc50f60aa16d982a8f11ccd294ce50bf/docs/source/resources/logo.png" height="200">
+<img src="https://raw.githubusercontent.com/AnonymouX47/term-image/92ff4b2d2e4731be9e1b2ac7378964ebed9f10f9/docs/source/resources/logo.png" height="200">
 </p>
 
 <p>
 <b>Display images in the terminal with Python</b>
 </p>
 
 <p>
@@ -90,15 +86,15 @@
 - [Quick Start](#library-quick-start)
 - [Usage](#usage)
 - [Contribution](#contribution)
 - [Planned Features](#planned-features)
 - [Known Issues](#known-issues)
 - [FAQs](#faqs)
 - [Credits](#credits)
-- [Donate](#donate)
+- [Sponsor This Project](#sponsor-this-project)
 
 
 > ### ⚠️ NOTICE!!! ⚠️
 > The image viewer (CLI and TUI) has been moved to [termvisage].
 
 
 ## Installation
@@ -212,15 +208,15 @@
 ## Usage
 
 <p align="center"><b>
    🚧 Under Construction - There will most likely be incompatible changes between minor versions of
    <a href='https://semver.org/spec/v2.0.0.html#spec-item-4'>version zero</a>!
 </b></p>
 
-**If you want to use this library in a project while it's still on version zero, ensure you pin the dependency version to a specific minor version e.g `>=0.4,<0.5`.**
+**If you want to use this library in a project while it's still on version zero, ensure you pin the dependency to a specific minor version e.g `>=0.4,<0.5`.**
 
 See the [docs](https://term-image.readthedocs.io) for the User Guide and API Reference.
 
 
 ## Contribution
 
 Please read through the [guidelines](https://github.com/AnonymouX47/term-image/blob/main/CONTRIBUTING.md).
@@ -244,21 +240,24 @@
 ## FAQs
 
 See the [FAQs](https://term-image.readthedocs.io/en/stable/faqs.html) section of the docs.
 
 ## Credits
 
 The following projects have been (and are still) crucial to the development of this project:
+- [Pillow](https://python-pillow.org) by [Fredrik Lundh, Jeffrey A. Clark (Alex) and contributors](https://github.com/python-pillow/Pillow/graphs/contributors)
+- [Requests](https://requests.readthedocs.io) by [Kenneth Reitz and others](https://requests.readthedocs.io/en/latest/dev/authors/)
 
-- [Pillow](https://python-pillow.org)
+The logo was composed using resource(s) from the following source(s):
+- [Gallery icons created by Andrean Prabowo - Flaticon](https://www.flaticon.com/free-icons/gallery)
 
-## Donate
+## Sponsor This Project
 
 <a href="https://www.buymeacoffee.com/anonymoux47" target="_blank">
    <img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" >
 </a>
 
-Your donation will go a long way in aiding the progress and development of this project.
+Any amount will go a long way in aiding the progress and development of this project.
 Thank you! 💓
 
 
 [termvisage]: https://github.com/AnonymouX47/termvisage
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: term-image Version: 0.6.1 Summary: Display images
+Metadata-Version: 2.1 Name: term-image Version: 0.7.0 Summary: Display images
 in the terminal Home-page: https://github.com/AnonymouX47/term-image Author:
 Toluwaleke Ogundipe Author-email: anonymoux47@gmail.com License: MIT Project-
 URL: Changelog, https://github.com/AnonymouX47/term-image/blob/main/
 CHANGELOG.md Project-URL: Documentation, https://term-image.readthedocs.io/
 Project-URL: Funding, https://github.com/AnonymouX47/term-image#donate Project-
 URL: Source, https://github.com/AnonymouX47/term-image Project-URL: Tracker,
 https://github.com/AnonymouX47/term-image/issues Keywords:
@@ -15,85 +15,85 @@
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3 ::
 Only Classifier: Topic :: Software Development :: Libraries Classifier: Topic
 :: Terminals :: Terminal Emulators/X Terminals Classifier: Topic :: Multimedia
 :: Graphics :: Viewers Requires-Python: >=3.7 Description-Content-Type: text/
-markdown License-File: LICENSE [Buy_Me_A_Coffee]
-
+markdown License-File: LICENSE
                            ****** Term-Image ******
           [https://raw.githubusercontent.com/AnonymouX47/term-image/
-   abca69a2cc50f60aa16d982a8f11ccd294ce50bf/docs/source/resources/logo.png]
+   92ff4b2d2e4731be9e1b2ac7378964ebed9f10f9/docs/source/resources/logo.png]
                   Display images in the terminal with Python
                                Docs ║  Tutorial
  [https://img.shields.io/pypi/v/term-image.svg] [https://pepy.tech/badge/term-
 image/month] [https://img.shields.io/pypi/pyversions/term-image.svg] [https://
    img.shields.io/badge/code%20style-black-000000.svg] [https://github.com/
   AnonymouX47/term-image/actions/workflows/test.yml/badge.svg] [Documentation
   Status] [https://img.shields.io/github/last-commit/AnonymouX47/term-image]
      [https://img.shields.io/twitter/url/http/shields.io.svg?style=social]
 ## Contents - [Installation](#installation) - [Features](#features) - [Demo]
 (#demo) - [Quick Start](#library-quick-start) - [Usage](#usage) -
 [Contribution](#contribution) - [Planned Features](#planned-features) - [Known
-Issues](#known-issues) - [FAQs](#faqs) - [Credits](#credits) - [Donate]
-(#donate) > ### â ï¸ NOTICE!!! â ï¸ > The image viewer (CLI and TUI) has
-been moved to [termvisage]. ## Installation ### Requirements - Operating
-System: Unix / Linux / Mac OS X / Windows (limited support, see the [FAQs]
-(https://term-image.readthedocs.io/en/stable/faqs.html)) - [Python](https://
-www.python.org/) >= 3.7 - A terminal emulator with **any** of the following: -
-support for the [Kitty graphics protocol](https://sw.kovidgoyal.net/kitty/
-graphics-protocol/). - support for the [iTerm2 inline image protocol](https://
-iterm2.com/documentation-images.html). - full Unicode support and ANSI 24-bit
-color support **Plans to support a wider variety of terminal emulators are in
-motion** (see [Planned Features](#planned-features)). ### Steps The latest
-**stable** version can be installed from [PyPI](https://pypi.org/project/term-
-image) with: ```shell pip install term-image ``` The **development** version
-can be installed with: ```shell pip install git+https://github.com/AnonymouX47/
-term-image.git ``` ### Supported Terminal Emulators See [here](https://term-
-image.readthedocs.io/en/stable/start/installation.html#supported-terminal-
-emulators) for a list of tested terminal emulators. If you've tested this
-library on any other terminal emulator that meets the requirements for any of
-the render styles, please mention the name (and version) in a new thread under
-[this discussion](https://github.com/AnonymouX47/term-image/discussions/4).
-Also, if you have any issue with terminal support, you may report or check
-information about it in the discussion linked above. ## Features - Multiple
-image formats (basically all formats supported by [`PIL.Image.open()`](https://
-pillow.readthedocs.io/en/stable/handbook/image-file-formats.html)) - Multiple
-image source types: PIL image instance, local file, URL - Multiple image render
-styles (with automatic support detection) - Support for multiple terminal
-graphics protocols: [Kitty](https://sw.kovidgoyal.net/kitty/graphics-protocol/
-), [iTerm2](https://iterm2.com/documentation-images.html) - Exposes various
-features of the protocols - Transparency support (with multiple options) -
-Animated image support (including transparent ones) - Multiple formats: GIF,
-WEBP, APNG (and possibly more) - Fully controllable iteration over rendered
-frames of animated images - Image animation with multiple parameters -
-Integration into various TUI / terminal-based output libraries. - Terminal size
-awareness - Automatic and manual image sizing - Horizontal and vertical
-alignment - Automatic and manual font ratio adjustment (to preserve image
-aspect ratio) - and more... ð ## Demo Check out this [image viewer]
-[termvisage] based on this library. ## Quick Start ### Creating an instance 1.
-Initialize with a file path: ```python from term_image.image import from_file
-image = from_file("path/to/image.png") ``` 2. Initialize with a URL: ```python
-from term_image.image import from_url image = from_url("https://
-www.example.com/image.png") ``` 3. Initialize with a PIL (Pillow) image
-instance: ```python from PIL import Image from term_image.image import
-AutoImage img = Image.open("path/to/image.png") image = AutoImage(img) ``` ###
-Drawing/Displaying an Image There are two basic ways to draw an image to the
-terminal screen: 1. Using the `draw()` method: ```python image.draw() ```
-**NOTE:** `draw()` has various parameters for render formatting. 2. Using
-`print()` with an image render output: ```python print(image) # without
-formatting # OR print(f"{image:>200.^100#ffffff}") # with formatting ``` For
-animated images, only the former animates the output, the latter only draws the
-current frame. See the [tutorial](https://term-image.readthedocs.io/en/stable/
-start/tutorial.html) for a more detailed introduction. ## Usage
+Issues](#known-issues) - [FAQs](#faqs) - [Credits](#credits) - [Sponsor This
+Project](#sponsor-this-project) > ### â ï¸ NOTICE!!! â ï¸ > The image
+viewer (CLI and TUI) has been moved to [termvisage]. ## Installation ###
+Requirements - Operating System: Unix / Linux / Mac OS X / Windows (limited
+support, see the [FAQs](https://term-image.readthedocs.io/en/stable/faqs.html))
+- [Python](https://www.python.org/) >= 3.7 - A terminal emulator with **any**
+of the following: - support for the [Kitty graphics protocol](https://
+sw.kovidgoyal.net/kitty/graphics-protocol/). - support for the [iTerm2 inline
+image protocol](https://iterm2.com/documentation-images.html). - full Unicode
+support and ANSI 24-bit color support **Plans to support a wider variety of
+terminal emulators are in motion** (see [Planned Features](#planned-features)).
+### Steps The latest **stable** version can be installed from [PyPI](https://
+pypi.org/project/term-image) with: ```shell pip install term-image ``` The
+**development** version can be installed with: ```shell pip install git+https:/
+/github.com/AnonymouX47/term-image.git ``` ### Supported Terminal Emulators See
+[here](https://term-image.readthedocs.io/en/stable/start/
+installation.html#supported-terminal-emulators) for a list of tested terminal
+emulators. If you've tested this library on any other terminal emulator that
+meets the requirements for any of the render styles, please mention the name
+(and version) in a new thread under [this discussion](https://github.com/
+AnonymouX47/term-image/discussions/4). Also, if you have any issue with
+terminal support, you may report or check information about it in the
+discussion linked above. ## Features - Multiple image formats (basically all
+formats supported by [`PIL.Image.open()`](https://pillow.readthedocs.io/en/
+stable/handbook/image-file-formats.html)) - Multiple image source types: PIL
+image instance, local file, URL - Multiple image render styles (with automatic
+support detection) - Support for multiple terminal graphics protocols: [Kitty]
+(https://sw.kovidgoyal.net/kitty/graphics-protocol/), [iTerm2](https://
+iterm2.com/documentation-images.html) - Exposes various features of the
+protocols - Transparency support (with multiple options) - Animated image
+support (including transparent ones) - Multiple formats: GIF, WEBP, APNG (and
+possibly more) - Fully controllable iteration over rendered frames of animated
+images - Image animation with multiple parameters - Integration into various
+TUI / terminal-based output libraries. - Terminal size awareness - Automatic
+and manual image sizing - Horizontal and vertical alignment - Automatic and
+manual font ratio adjustment (to preserve image aspect ratio) - and more...
+ð ## Demo Check out this [image viewer][termvisage] based on this library.
+## Quick Start ### Creating an instance 1. Initialize with a file path:
+```python from term_image.image import from_file image = from_file("path/to/
+image.png") ``` 2. Initialize with a URL: ```python from term_image.image
+import from_url image = from_url("https://www.example.com/image.png") ``` 3.
+Initialize with a PIL (Pillow) image instance: ```python from PIL import Image
+from term_image.image import AutoImage img = Image.open("path/to/image.png")
+image = AutoImage(img) ``` ### Drawing/Displaying an Image There are two basic
+ways to draw an image to the terminal screen: 1. Using the `draw()` method:
+```python image.draw() ``` **NOTE:** `draw()` has various parameters for render
+formatting. 2. Using `print()` with an image render output: ```python print
+(image) # without formatting # OR print(f"{image:>200.^100#ffffff}") # with
+formatting ``` For animated images, only the former animates the output, the
+latter only draws the current frame. See the [tutorial](https://term-
+image.readthedocs.io/en/stable/start/tutorial.html) for a more detailed
+introduction. ## Usage
    ð§ Under Construction - There will most likely be incompatible changes
                     between minor versions of version_zero!
 **If you want to use this library in a project while it's still on version
-zero, ensure you pin the dependency version to a specific minor version e.g
+zero, ensure you pin the dependency to a specific minor version e.g
 `>=0.4,<0.5`.** See the [docs](https://term-image.readthedocs.io) for the User
 Guide and API Reference. ## Contribution Please read through the [guidelines]
 (https://github.com/AnonymouX47/term-image/blob/main/CONTRIBUTING.md). For code
 contributions, you should also check out the [Planned Features](#planned-
 features). If you wish to work on any of the listed features/improvements,
 please click on the linked issue or go through the [issues](https://github.com/
 AnonymouX47/term-image/issues) section and join in on an ongoing discussion
@@ -101,10 +101,16 @@
 the implementation can be discussed. Hint: You can filter issues by *label* or
 simply *search* using the features's description. Thanks! ð ## Planned
 Features See [here](https://term-image.readthedocs.io/en/stable/planned.html).
 ## Known Issues See [here](https://term-image.readthedocs.io/en/stable/
 issues.html). ## FAQs See the [FAQs](https://term-image.readthedocs.io/en/
 stable/faqs.html) section of the docs. ## Credits The following projects have
 been (and are still) crucial to the development of this project: - [Pillow]
-(https://python-pillow.org) ## Donate [Buy_Me_A_Coffee] Your donation will go a
-long way in aiding the progress and development of this project. Thank you!
-ð [termvisage]: https://github.com/AnonymouX47/termvisage
+(https://python-pillow.org) by [Fredrik Lundh, Jeffrey A. Clark (Alex) and
+contributors](https://github.com/python-pillow/Pillow/graphs/contributors) -
+[Requests](https://requests.readthedocs.io) by [Kenneth Reitz and others]
+(https://requests.readthedocs.io/en/latest/dev/authors/) The logo was composed
+using resource(s) from the following source(s): - [Gallery icons created by
+Andrean Prabowo - Flaticon](https://www.flaticon.com/free-icons/gallery) ##
+Sponsor This Project [Buy_Me_A_Coffee] Any amount will go a long way in aiding
+the progress and development of this project. Thank you! ð [termvisage]:
+https://github.com/AnonymouX47/termvisage
```

### Comparing `term-image-0.6.1/README.md` & `term-image-0.7.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,13 @@
-<a href="https://www.buymeacoffee.com/anonymoux47" target="_blank">
-   <img align="right" src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" >
-</a><br><br>
-
 <div align="center">
 
 <h1><b>Term-Image</b></h1>
 
 <p>
-<img src="https://raw.githubusercontent.com/AnonymouX47/term-image/abca69a2cc50f60aa16d982a8f11ccd294ce50bf/docs/source/resources/logo.png" height="200">
+<img src="https://raw.githubusercontent.com/AnonymouX47/term-image/92ff4b2d2e4731be9e1b2ac7378964ebed9f10f9/docs/source/resources/logo.png" height="200">
 </p>
 
 <p>
 <b>Display images in the terminal with Python</b>
 </p>
 
 <p>
@@ -55,15 +51,15 @@
 - [Quick Start](#library-quick-start)
 - [Usage](#usage)
 - [Contribution](#contribution)
 - [Planned Features](#planned-features)
 - [Known Issues](#known-issues)
 - [FAQs](#faqs)
 - [Credits](#credits)
-- [Donate](#donate)
+- [Sponsor This Project](#sponsor-this-project)
 
 
 > ### ⚠️ NOTICE!!! ⚠️
 > The image viewer (CLI and TUI) has been moved to [termvisage].
 
 
 ## Installation
@@ -177,15 +173,15 @@
 ## Usage
 
 <p align="center"><b>
    🚧 Under Construction - There will most likely be incompatible changes between minor versions of
    <a href='https://semver.org/spec/v2.0.0.html#spec-item-4'>version zero</a>!
 </b></p>
 
-**If you want to use this library in a project while it's still on version zero, ensure you pin the dependency version to a specific minor version e.g `>=0.4,<0.5`.**
+**If you want to use this library in a project while it's still on version zero, ensure you pin the dependency to a specific minor version e.g `>=0.4,<0.5`.**
 
 See the [docs](https://term-image.readthedocs.io) for the User Guide and API Reference.
 
 
 ## Contribution
 
 Please read through the [guidelines](https://github.com/AnonymouX47/term-image/blob/main/CONTRIBUTING.md).
@@ -209,21 +205,24 @@
 ## FAQs
 
 See the [FAQs](https://term-image.readthedocs.io/en/stable/faqs.html) section of the docs.
 
 ## Credits
 
 The following projects have been (and are still) crucial to the development of this project:
+- [Pillow](https://python-pillow.org) by [Fredrik Lundh, Jeffrey A. Clark (Alex) and contributors](https://github.com/python-pillow/Pillow/graphs/contributors)
+- [Requests](https://requests.readthedocs.io) by [Kenneth Reitz and others](https://requests.readthedocs.io/en/latest/dev/authors/)
 
-- [Pillow](https://python-pillow.org)
+The logo was composed using resource(s) from the following source(s):
+- [Gallery icons created by Andrean Prabowo - Flaticon](https://www.flaticon.com/free-icons/gallery)
 
-## Donate
+## Sponsor This Project
 
 <a href="https://www.buymeacoffee.com/anonymoux47" target="_blank">
    <img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" >
 </a>
 
-Your donation will go a long way in aiding the progress and development of this project.
+Any amount will go a long way in aiding the progress and development of this project.
 Thank you! 💓
 
 
 [termvisage]: https://github.com/AnonymouX47/termvisage
```

#### html2text {}

```diff
@@ -1,78 +1,77 @@
-[Buy_Me_A_Coffee]
-
                            ****** Term-Image ******
           [https://raw.githubusercontent.com/AnonymouX47/term-image/
-   abca69a2cc50f60aa16d982a8f11ccd294ce50bf/docs/source/resources/logo.png]
+   92ff4b2d2e4731be9e1b2ac7378964ebed9f10f9/docs/source/resources/logo.png]
                   Display images in the terminal with Python
                                Docs ║  Tutorial
  [https://img.shields.io/pypi/v/term-image.svg] [https://pepy.tech/badge/term-
 image/month] [https://img.shields.io/pypi/pyversions/term-image.svg] [https://
    img.shields.io/badge/code%20style-black-000000.svg] [https://github.com/
   AnonymouX47/term-image/actions/workflows/test.yml/badge.svg] [Documentation
   Status] [https://img.shields.io/github/last-commit/AnonymouX47/term-image]
      [https://img.shields.io/twitter/url/http/shields.io.svg?style=social]
 ## Contents - [Installation](#installation) - [Features](#features) - [Demo]
 (#demo) - [Quick Start](#library-quick-start) - [Usage](#usage) -
 [Contribution](#contribution) - [Planned Features](#planned-features) - [Known
-Issues](#known-issues) - [FAQs](#faqs) - [Credits](#credits) - [Donate]
-(#donate) > ### â ï¸ NOTICE!!! â ï¸ > The image viewer (CLI and TUI) has
-been moved to [termvisage]. ## Installation ### Requirements - Operating
-System: Unix / Linux / Mac OS X / Windows (limited support, see the [FAQs]
-(https://term-image.readthedocs.io/en/stable/faqs.html)) - [Python](https://
-www.python.org/) >= 3.7 - A terminal emulator with **any** of the following: -
-support for the [Kitty graphics protocol](https://sw.kovidgoyal.net/kitty/
-graphics-protocol/). - support for the [iTerm2 inline image protocol](https://
-iterm2.com/documentation-images.html). - full Unicode support and ANSI 24-bit
-color support **Plans to support a wider variety of terminal emulators are in
-motion** (see [Planned Features](#planned-features)). ### Steps The latest
-**stable** version can be installed from [PyPI](https://pypi.org/project/term-
-image) with: ```shell pip install term-image ``` The **development** version
-can be installed with: ```shell pip install git+https://github.com/AnonymouX47/
-term-image.git ``` ### Supported Terminal Emulators See [here](https://term-
-image.readthedocs.io/en/stable/start/installation.html#supported-terminal-
-emulators) for a list of tested terminal emulators. If you've tested this
-library on any other terminal emulator that meets the requirements for any of
-the render styles, please mention the name (and version) in a new thread under
-[this discussion](https://github.com/AnonymouX47/term-image/discussions/4).
-Also, if you have any issue with terminal support, you may report or check
-information about it in the discussion linked above. ## Features - Multiple
-image formats (basically all formats supported by [`PIL.Image.open()`](https://
-pillow.readthedocs.io/en/stable/handbook/image-file-formats.html)) - Multiple
-image source types: PIL image instance, local file, URL - Multiple image render
-styles (with automatic support detection) - Support for multiple terminal
-graphics protocols: [Kitty](https://sw.kovidgoyal.net/kitty/graphics-protocol/
-), [iTerm2](https://iterm2.com/documentation-images.html) - Exposes various
-features of the protocols - Transparency support (with multiple options) -
-Animated image support (including transparent ones) - Multiple formats: GIF,
-WEBP, APNG (and possibly more) - Fully controllable iteration over rendered
-frames of animated images - Image animation with multiple parameters -
-Integration into various TUI / terminal-based output libraries. - Terminal size
-awareness - Automatic and manual image sizing - Horizontal and vertical
-alignment - Automatic and manual font ratio adjustment (to preserve image
-aspect ratio) - and more... ð ## Demo Check out this [image viewer]
-[termvisage] based on this library. ## Quick Start ### Creating an instance 1.
-Initialize with a file path: ```python from term_image.image import from_file
-image = from_file("path/to/image.png") ``` 2. Initialize with a URL: ```python
-from term_image.image import from_url image = from_url("https://
-www.example.com/image.png") ``` 3. Initialize with a PIL (Pillow) image
-instance: ```python from PIL import Image from term_image.image import
-AutoImage img = Image.open("path/to/image.png") image = AutoImage(img) ``` ###
-Drawing/Displaying an Image There are two basic ways to draw an image to the
-terminal screen: 1. Using the `draw()` method: ```python image.draw() ```
-**NOTE:** `draw()` has various parameters for render formatting. 2. Using
-`print()` with an image render output: ```python print(image) # without
-formatting # OR print(f"{image:>200.^100#ffffff}") # with formatting ``` For
-animated images, only the former animates the output, the latter only draws the
-current frame. See the [tutorial](https://term-image.readthedocs.io/en/stable/
-start/tutorial.html) for a more detailed introduction. ## Usage
+Issues](#known-issues) - [FAQs](#faqs) - [Credits](#credits) - [Sponsor This
+Project](#sponsor-this-project) > ### â ï¸ NOTICE!!! â ï¸ > The image
+viewer (CLI and TUI) has been moved to [termvisage]. ## Installation ###
+Requirements - Operating System: Unix / Linux / Mac OS X / Windows (limited
+support, see the [FAQs](https://term-image.readthedocs.io/en/stable/faqs.html))
+- [Python](https://www.python.org/) >= 3.7 - A terminal emulator with **any**
+of the following: - support for the [Kitty graphics protocol](https://
+sw.kovidgoyal.net/kitty/graphics-protocol/). - support for the [iTerm2 inline
+image protocol](https://iterm2.com/documentation-images.html). - full Unicode
+support and ANSI 24-bit color support **Plans to support a wider variety of
+terminal emulators are in motion** (see [Planned Features](#planned-features)).
+### Steps The latest **stable** version can be installed from [PyPI](https://
+pypi.org/project/term-image) with: ```shell pip install term-image ``` The
+**development** version can be installed with: ```shell pip install git+https:/
+/github.com/AnonymouX47/term-image.git ``` ### Supported Terminal Emulators See
+[here](https://term-image.readthedocs.io/en/stable/start/
+installation.html#supported-terminal-emulators) for a list of tested terminal
+emulators. If you've tested this library on any other terminal emulator that
+meets the requirements for any of the render styles, please mention the name
+(and version) in a new thread under [this discussion](https://github.com/
+AnonymouX47/term-image/discussions/4). Also, if you have any issue with
+terminal support, you may report or check information about it in the
+discussion linked above. ## Features - Multiple image formats (basically all
+formats supported by [`PIL.Image.open()`](https://pillow.readthedocs.io/en/
+stable/handbook/image-file-formats.html)) - Multiple image source types: PIL
+image instance, local file, URL - Multiple image render styles (with automatic
+support detection) - Support for multiple terminal graphics protocols: [Kitty]
+(https://sw.kovidgoyal.net/kitty/graphics-protocol/), [iTerm2](https://
+iterm2.com/documentation-images.html) - Exposes various features of the
+protocols - Transparency support (with multiple options) - Animated image
+support (including transparent ones) - Multiple formats: GIF, WEBP, APNG (and
+possibly more) - Fully controllable iteration over rendered frames of animated
+images - Image animation with multiple parameters - Integration into various
+TUI / terminal-based output libraries. - Terminal size awareness - Automatic
+and manual image sizing - Horizontal and vertical alignment - Automatic and
+manual font ratio adjustment (to preserve image aspect ratio) - and more...
+ð ## Demo Check out this [image viewer][termvisage] based on this library.
+## Quick Start ### Creating an instance 1. Initialize with a file path:
+```python from term_image.image import from_file image = from_file("path/to/
+image.png") ``` 2. Initialize with a URL: ```python from term_image.image
+import from_url image = from_url("https://www.example.com/image.png") ``` 3.
+Initialize with a PIL (Pillow) image instance: ```python from PIL import Image
+from term_image.image import AutoImage img = Image.open("path/to/image.png")
+image = AutoImage(img) ``` ### Drawing/Displaying an Image There are two basic
+ways to draw an image to the terminal screen: 1. Using the `draw()` method:
+```python image.draw() ``` **NOTE:** `draw()` has various parameters for render
+formatting. 2. Using `print()` with an image render output: ```python print
+(image) # without formatting # OR print(f"{image:>200.^100#ffffff}") # with
+formatting ``` For animated images, only the former animates the output, the
+latter only draws the current frame. See the [tutorial](https://term-
+image.readthedocs.io/en/stable/start/tutorial.html) for a more detailed
+introduction. ## Usage
    ð§ Under Construction - There will most likely be incompatible changes
                     between minor versions of version_zero!
 **If you want to use this library in a project while it's still on version
-zero, ensure you pin the dependency version to a specific minor version e.g
+zero, ensure you pin the dependency to a specific minor version e.g
 `>=0.4,<0.5`.** See the [docs](https://term-image.readthedocs.io) for the User
 Guide and API Reference. ## Contribution Please read through the [guidelines]
 (https://github.com/AnonymouX47/term-image/blob/main/CONTRIBUTING.md). For code
 contributions, you should also check out the [Planned Features](#planned-
 features). If you wish to work on any of the listed features/improvements,
 please click on the linked issue or go through the [issues](https://github.com/
 AnonymouX47/term-image/issues) section and join in on an ongoing discussion
@@ -80,10 +79,16 @@
 the implementation can be discussed. Hint: You can filter issues by *label* or
 simply *search* using the features's description. Thanks! ð ## Planned
 Features See [here](https://term-image.readthedocs.io/en/stable/planned.html).
 ## Known Issues See [here](https://term-image.readthedocs.io/en/stable/
 issues.html). ## FAQs See the [FAQs](https://term-image.readthedocs.io/en/
 stable/faqs.html) section of the docs. ## Credits The following projects have
 been (and are still) crucial to the development of this project: - [Pillow]
-(https://python-pillow.org) ## Donate [Buy_Me_A_Coffee] Your donation will go a
-long way in aiding the progress and development of this project. Thank you!
-ð [termvisage]: https://github.com/AnonymouX47/termvisage
+(https://python-pillow.org) by [Fredrik Lundh, Jeffrey A. Clark (Alex) and
+contributors](https://github.com/python-pillow/Pillow/graphs/contributors) -
+[Requests](https://requests.readthedocs.io) by [Kenneth Reitz and others]
+(https://requests.readthedocs.io/en/latest/dev/authors/) The logo was composed
+using resource(s) from the following source(s): - [Gallery icons created by
+Andrean Prabowo - Flaticon](https://www.flaticon.com/free-icons/gallery) ##
+Sponsor This Project [Buy_Me_A_Coffee] Any amount will go a long way in aiding
+the progress and development of this project. Thank you! ð [termvisage]:
+https://github.com/AnonymouX47/termvisage
```

### Comparing `term-image-0.6.1/setup.py` & `term-image-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 ]
 
 with open("README.md", "r") as fp:
     long_description = fp.read()
 
 setup(
     name="term-image",
-    version="0.6.1",
+    version="0.7.0",
     author="Toluwaleke Ogundipe",
     author_email="anonymoux47@gmail.com",
     url="https://github.com/AnonymouX47/term-image",
     description="Display images in the terminal",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
```

### Comparing `term-image-0.6.1/src/term_image/__init__.py` & `term-image-0.7.0/src/term_image/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,17 +23,16 @@
 
 from enum import Enum, auto
 from operator import truediv
 from typing import Optional, Union
 
 from . import utils
 from .exceptions import TermImageError
-from .utils import get_cell_size
 
-version_info = (0, 6, 1)
+version_info = (0, 7, 0)
 
 # Follows https://semver.org/spec/v2.0.0.html
 __version__ = ".".join(map(str, version_info[:3]))
 if version_info[3:]:
     __version__ += "-" + ".".join(map(str, version_info[3:]))
 
 #: Default timeout for :ref:`terminal-queries`
@@ -117,24 +116,24 @@
 
 def get_cell_ratio() -> float:
     """Returns the global :term:`cell ratio`.
 
     See :py:func:`set_cell_ratio`.
     """
     # `(1, 2)` is a fallback in case the terminal doesn't respond in time
-    return _cell_ratio or truediv(*(get_cell_size() or (1, 2)))
+    return _cell_ratio or truediv(*(utils.get_cell_size() or (1, 2)))
 
 
 def set_cell_ratio(ratio: Union[float, AutoCellRatio]) -> None:
     """Sets the global :term:`cell ratio`.
 
     Args:
         ratio: Can be one of the following values.
 
-          * A positive ``float`` value.
+          * A positive :py:class:`float` value.
           * :py:attr:`AutoCellRatio.FIXED`, the ratio is immediately determined from
             the :term:`active terminal`.
           * :py:attr:`AutoCellRatio.DYNAMIC`, the ratio is determined from the
             :term:`active terminal` whenever :py:func:`get_cell_ratio` is called,
             though with some caching involved, such that the ratio is re-determined
             only if the terminal size changes.
 
@@ -157,50 +156,47 @@
     ATTENTION:
         See :ref:`auto-cell-ratio` for details about the auto modes.
     """
     global _cell_ratio
 
     if isinstance(ratio, AutoCellRatio):
         if AutoCellRatio.is_supported is None:
-            AutoCellRatio.is_supported = get_cell_size() is not None
+            AutoCellRatio.is_supported = utils.get_cell_size() is not None
 
         if not AutoCellRatio.is_supported:
             raise TermImageError(
                 "Auto cell ratio is not supported in the active terminal or on the "
                 "current platform"
             )
         elif ratio is AutoCellRatio.FIXED:
             # `(1, 2)` is a fallback in case the terminal doesn't respond in time
-            _cell_ratio = truediv(*(get_cell_size() or (1, 2)))
+            _cell_ratio = truediv(*(utils.get_cell_size() or (1, 2)))
         else:
             _cell_ratio = None
     elif isinstance(ratio, float):
         if ratio <= 0.0:
-            raise ValueError(f"'ratio' must be greater than zero (got: {ratio})")
+            raise utils.arg_value_error_range("ratio", ratio)
         _cell_ratio = ratio
     else:
-        raise TypeError(
-            "'ratio' must be a float or AutoCellRatio enum member "
-            f"(got: {type(ratio).__name__})"
-        )
+        raise utils.arg_type_error("ratio", ratio)
 
 
 def set_query_timeout(timeout: float) -> None:
     """Sets the timeout for :ref:`terminal-queries`.
 
     Args:
         timeout: Time limit for awaiting a response from the terminal, in seconds.
 
     Raises:
         TypeError: *timeout* is not a float.
         ValueError: *timeout* is less than or equal to zero.
     """
     if not isinstance(timeout, float):
-        raise TypeError(f"'timeout' must be a float (got: {type(timeout).__name__!r})")
+        raise utils.arg_type_error("timeout", timeout)
     if timeout <= 0.0:
-        raise ValueError(f"'timeout' must be greater than zero (got: {timeout!r})")
+        raise utils.arg_value_error_range("timeout", timeout)
 
     utils._query_timeout = timeout
 
 
 _cell_ratio = 0.5
 AutoCellRatio.is_supported = None
```

### Comparing `term-image-0.6.1/src/term_image/image/__init__.py` & `term-image-0.7.0/src/term_image/image/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,26 +7,25 @@
 __all__ = (
     "auto_image_class",
     "AutoImage",
     "from_file",
     "from_url",
     "ImageSource",
     "Size",
-    "ImageMeta",
     "BaseImage",
     "TextImage",
     "BlockImage",
     "GraphicsImage",
     "ITerm2Image",
     "KittyImage",
     "ImageIterator",
 )
 
 import os
-from typing import Optional, Tuple, Union
+from typing import Optional, Union
 
 import PIL
 
 from .block import BlockImage
 from .common import (
     BaseImage,
     GraphicsImage,
@@ -53,45 +52,44 @@
 
 
 def AutoImage(
     image: PIL.Image.Image,
     *,
     width: Optional[int] = None,
     height: Optional[int] = None,
-    scale: Tuple[float, float] = (1.0, 1.0),
 ) -> BaseImage:
     """Creates an image instance from a PIL image instance.
 
     Returns:
         An instance of the automatically selected image render style (as returned by
         :py:func:`auto_image_class`).
 
     Same arguments and raised exceptions as the :py:class:`BaseImage` class constructor.
     """
-    return auto_image_class()(image, width=width, height=height, scale=scale)
+    return auto_image_class()(image, width=width, height=height)
 
 
 def from_file(
     filepath: Union[str, os.PathLike],
-    **kwargs: Union[None, int, Tuple[float, float]],
+    **kwargs: Union[None, int],
 ) -> BaseImage:
     """Creates an image instance from an image file.
 
     Returns:
         An instance of the automatically selected image render style (as returned by
         :py:func:`auto_image_class`).
 
     Same arguments and raised exceptions as :py:meth:`BaseImage.from_file`.
     """
     return auto_image_class().from_file(filepath, **kwargs)
 
 
 def from_url(
     url: str,
-    **kwargs: Union[None, int, Tuple[float, float]],
+    **kwargs: Union[None, int],
 ) -> BaseImage:
     """Creates an image instance from an image URL.
 
     Returns:
         An instance of the automatically selected image render style (as returned by
         :py:func:`auto_image_class`).
```

### Comparing `term-image-0.6.1/src/term_image/image/block.py` & `term-image-0.7.0/src/term_image/image/block.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from __future__ import annotations
 
 __all__ = ("BlockImage",)
 
 import io
 import os
-import warnings
 from math import ceil
 from operator import mul
 from typing import Optional, Tuple, Union
 
 import PIL
 
-from ..utils import BG_FMT, COLOR_RESET, FG_FMT, get_fg_bg_colors
+from ..ctlseqs import SGR_BG_RGB, SGR_FG_RGB, SGR_NORMAL
+from ..utils import get_fg_bg_colors
 from .common import TextImage
 
-warnings.filterwarnings("once", category=DeprecationWarning, module=__name__)
-
 LOWER_PIXEL = "\u2584"  # lower-half block element
 UPPER_PIXEL = "\u2580"  # upper-half block element
 
 
 class BlockImage(TextImage):
     """A render style using unicode half blocks and 24-bit colour escape codes.
 
@@ -64,37 +62,37 @@
         # It's more efficient to write separate strings to the buffer separately
         # than concatenate and write together.
 
         def update_buffer():
             if alpha:
                 no_alpha = False
                 if a_cluster1 == 0 == a_cluster2:
-                    buf_write(COLOR_RESET)
+                    buf_write(SGR_NORMAL)
                     buf_write(blank * n)
                 elif a_cluster1 == 0:  # up is transparent
-                    buf_write(COLOR_RESET)
-                    buf_write(FG_FMT % cluster2)
+                    buf_write(SGR_NORMAL)
+                    buf_write(SGR_FG_RGB % cluster2)
                     buf_write(lower_pixel * n)
                 elif a_cluster2 == 0:  # down is transparent
-                    buf_write(COLOR_RESET)
-                    buf_write(FG_FMT % cluster1)
+                    buf_write(SGR_NORMAL)
+                    buf_write(SGR_FG_RGB % cluster1)
                     buf_write(upper_pixel * n)
                 else:
                     no_alpha = True
 
             if not alpha or no_alpha:
                 r, g, b = cluster2
                 # Kitty does not render BG colors equal to the default BG color
                 if is_on_kitty and cluster2 == bg_color:
                     r += r < 255 or -1
-                buf_write(BG_FMT % (r, g, b))
+                buf_write(SGR_BG_RGB % (r, g, b))
                 if cluster1 == cluster2:
                     buf_write(blank * n)
                 else:
-                    buf_write(FG_FMT % cluster1)
+                    buf_write(SGR_FG_RGB % cluster1)
                     buf_write(upper_pixel * n)
 
         buffer = io.StringIO()
         buf_write = buffer.write  # Eliminate attribute resolution cost
 
         bg_color = get_fg_bg_colors()[1]
         is_on_kitty = self._is_on_kitty()
@@ -102,15 +100,15 @@
             blank = " \0"
             lower_pixel = LOWER_PIXEL + "\0"
             upper_pixel = UPPER_PIXEL + "\0"
         else:
             blank = " "
             lower_pixel = LOWER_PIXEL
             upper_pixel = UPPER_PIXEL
-        end_of_line = COLOR_RESET + "\n"
+        end_of_line = SGR_NORMAL + "\n"
 
         width, height = self._get_render_size()
         frame_img = img if frame else None
         img, rgb, a = self._get_render_data(img, alpha, round_alpha=True, frame=frame)
         alpha = img.mode == "RGBA"
 
         # clean up (ImageIterator uses one PIL image throughout)
@@ -167,11 +165,11 @@
             update_buffer()  # Rest of the line
             if split_cells:
                 # Set the last "\0" to be overwriten by the next byte
                 buffer.seek(buffer.tell() - 1)
             if row_no < height:  # last line not yet rendered
                 buf_write(end_of_line)
 
-        buf_write(COLOR_RESET)  # Reset color after last line
+        buf_write(SGR_NORMAL)  # Reset color after last line
 
         with buffer:
             return buffer.getvalue()
```

### Comparing `term-image-0.6.1/src/term_image/image/common.py` & `term-image-0.7.0/src/term_image/image/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 """
 
 from __future__ import annotations
 
 __all__ = (
     "ImageSource",
     "Size",
-    "ImageMeta",
     "BaseImage",
     "GraphicsImage",
     "TextImage",
     "ImageIterator",
 )
 
 import atexit
@@ -20,38 +19,41 @@
 import re
 import sys
 import time
 from abc import ABCMeta, abstractmethod
 from enum import Enum
 from functools import wraps
 from math import ceil
-from operator import gt, mul, sub
+from operator import gt, mul
 from shutil import rmtree
 from tempfile import mkdtemp, mkstemp
 from types import FunctionType, TracebackType
 from typing import Any, Dict, Generator, List, Optional, Set, Tuple, Union
 from urllib.parse import urlparse
 
 import PIL
 import requests
 from PIL import Image, UnidentifiedImageError
 
 from .. import get_cell_ratio
+from ..ctlseqs import CURSOR_DOWN, CURSOR_UP, HIDE_CURSOR, SGR_NORMAL, SHOW_CURSOR
 from ..exceptions import (
     InvalidSizeError,
+    RenderError,
+    StyleError,
     TermImageError,
     URLNotFoundError,
-    _style_error,
 )
 from ..utils import (
-    COLOR_RESET,
-    CSI,
     ClassInstanceMethod,
     ClassProperty,
-    ClassPropertyMeta,
+    arg_type_error,
+    arg_value_error,
+    arg_value_error_msg,
+    arg_value_error_range,
     cached,
     get_cell_size,
     get_fg_bg_colors,
     get_terminal_name_version,
     get_terminal_size,
     no_redecorate,
 )
@@ -130,120 +132,87 @@
     URL = SourceAttr("_url")
 
 
 class Size(Enum):
     """Enumeration for :term:`automatic sizing`."""
 
     #: Equivalent to :py:attr:`ORIGINAL` if it will fit into the
-    #: :term:`available size`, else :py:attr:`FIT`.
+    #: :term:`frame size`, else :py:attr:`FIT`.
     #:
     #: :meta hide-value:
     AUTO = Hidden()
 
-    #: The image size is set to fit optimally **within** the :term:`available size`.
+    #: The image size is set to fit optimally **within** the :term:`frame size`.
     #:
     #: :meta hide-value:
     FIT = Hidden()
 
-    #: The size is set such that the width is exactly the :term:`available width`,
+    #: The size is set such that the width is exactly the :term:`frame width`,
     #: regardless of the :term:`cell ratio`.
     #:
     #: :meta hide-value:
     FIT_TO_WIDTH = Hidden()
 
     #: The image size is set such that the image is rendered with as many pixels as the
     #: the original image consists of.
     #:
     #: :meta hide-value:
     ORIGINAL = Hidden()
 
 
-class ImageMeta(ClassPropertyMeta, ABCMeta):
-    """Type of all render style classes.
+class ImageMeta(ABCMeta):
+    """Type of all render style classes."""
 
-    NOTE:
-        | For all render style classes (instances of this class) defined **within** this
-          package, ``str(cls)`` yields the same value as :py:attr:`cls.style <style>`.
-        | For render style classes defined **outside** this package (subclasses of those
-          defined within this package), ``str(cls)`` is equivalent to ``repr(cls)``.
-    """
-
-    def __str__(self):
-        return self.style or super().__str__()
-
-    style = property(
-        cached(
-            lambda self: (
-                self.__name__[:-5].lower()
-                if self.__module__.startswith("term_image.image")
-                else None
-            )
-        ),
-        doc="""Name of the render style [category].
-
-        Returns:
-            * The name of the render style [category] implemented by the invoking
-              class, if defined **within** this package (``term_image``)
-            * ``None``, if the invoking class is defined **outside** this package
-              (``term_image``)
-
-        :type: Optional[str]
-
-        **Examples**
-
-        For a class defined within this package:
-
-        >>> from term_image.image import KittyImage
-        >>> KittyImage.style
-        'kitty'
-
-        For a class defined outside this package:
+    _forced_support: bool = False
 
-        >>> from term_image.image import KittyImage
-        >>> class MyImage(KittyImage): pass
-        >>> MyImage.style is None
-        True
+    forced_support = ClassProperty(
+        lambda self: self._forced_support,
+        doc="""Forced render style support
 
-        HINT:
-            Equivalent to ``str(cls)`` for all render style classes (instances of
-            :py:class:`ImageMeta`) defined **within** this package.
+        See the base instance of this metaclass for the complete description.
         """,
     )
 
+    @forced_support.setter
+    def forced_support(self, status: bool):
+        if not isinstance(status, bool):
+            raise arg_type_error("forced_support", status)
+
+        self._forced_support = status
+
 
 class BaseImage(metaclass=ImageMeta):
     """Base of all render styles.
 
     Args:
         image: Source image.
         width: Can be
 
-          * an integer; horizontal dimension of the image, in columns.
+          * a positive integer; horizontal dimension of the image, in columns.
           * a :py:class:`~term_image.image.Size` enum member.
 
         height: Can be
 
-          * an integer; vertical dimension of the image, in lines.
+          * a positive integer; vertical dimension of the image, in lines.
           * a :py:class:`~term_image.image.Size` enum member.
 
-        scale: The fraction of the size (on respective axes) to render the image with.
-
     Raises:
         TypeError: An argument is of an inappropriate type.
         ValueError: An argument is of an appropriate type but has an
           unexpected/invalid value.
 
     Propagates exceptions raised by :py:meth:`set_size`, if *width* or *height* is
     given.
 
     NOTE:
         * If neither *width* nor *height* is given (or both are ``None``),
           :py:attr:`~term_image.image.Size.FIT` applies.
-        * The image size is multiplied by the :term:`scale` on respective axes when
-          the image is :term:`rendered`.
+        * If both width and height are not ``None``, they must be positive integers
+          and :term:`manual sizing` applies i.e the image size is set as given without
+          preserving aspect ratio.
         * For animated images, the seek position is initialized to the current seek
           position of the given image.
         * It's allowed to set properties for :term:`animated` images on non-animated
           ones, the values are simply ignored.
 
     ATTENTION:
         This class cannot be directly instantiated. Image instances should be created
@@ -264,35 +233,29 @@
 
     def __init__(
         self,
         image: PIL.Image.Image,
         *,
         width: Union[int, Size, None] = None,
         height: Union[int, Size, None] = None,
-        scale: Tuple[float, float] = (1.0, 1.0),
     ) -> None:
         """See the class description"""
         if not isinstance(image, Image.Image):
-            raise TypeError(
-                "Expected a 'PIL.Image.Image' instance for 'image' "
-                f"(got: {type(image).__name__!r})."
-            )
+            raise arg_type_error("image", image)
         if 0 in image.size:
             raise ValueError("'image' is null-sized")
 
         self._closed = False
         self._source = image
         self._source_type = ImageSource.PIL_IMAGE
         self._original_size = image.size
         if width is None is height:
             self.size = Size.FIT
         else:
             self.set_size(width, height)
-        self._scale = []
-        self._scale[:] = self._check_scale(scale)
 
         self._is_animated = hasattr(image, "is_animated") and image.is_animated
         if self._is_animated:
             self._frame_duration = (image.info.get("duration") or 100) / 1000
             self._seek_position = image.tell()
             self._n_frames = None
 
@@ -321,23 +284,22 @@
             height,
         )
 
     def __iter__(self) -> ImageIterator:
         return ImageIterator(self, 1, "1.1", False)
 
     def __repr__(self) -> str:
-        return "<{}: source_type={} size={} scale={} is_animated={}>".format(
+        return "<{}: source_type={} size={} is_animated={}>".format(
             type(self).__name__,
             self._source_type.name,
             (
                 self._size.name
                 if isinstance(self._size, Size)
                 else "x".join(map(str, self._size))
             ),
-            "x".join(format(x, ".2") for x in self._scale),
             self._is_animated,
         )
 
     def __str__(self) -> str:
         """Renders the image with transparency enabled and without alignment"""
         # Only the currently set frame is rendered for animated images
         return self._renderer(self._render_image, _ALPHA_THRESHOLD)
@@ -345,342 +307,295 @@
     # Properties
 
     closed = property(
         lambda self: self._closed,
         doc="""Instance finalization status
 
         :type: bool
+
+        GET:
+            Returns ``True`` if the instance has been finalized (:py:meth:`close` has
+            been called). Otherwise, ``False``.
         """,
     )
 
     forced_support = ClassProperty(
-        lambda cls: cls._forced_support,
-        doc="""Render style forced support status
+        lambda self: type(self)._forced_support,
+        doc="""Forced render style support
 
         :type: bool
 
         GET:
-            Returns the forced support status of the render style of the invoker.
+            Returns the forced support status of the invoking class or class of the
+            invoking instance.
 
         SET:
-            Forced support is enabled or disabled for the render style of the invoker.
+            Forced support is enabled or disabled for the invoking class.
+
+            Can not be set on an instance.
 
         If forced support is:
 
         * **enabled**, the render style is treated as if it were supported,
           regardless of the return value of :py:meth:`is_supported`.
         * **disabled**, the return value of :py:meth:`is_supported` determines if
           the render style is supported or not.
 
-        By **default**, forced support is **disabled** by the base style class
-        (:py:class:`BaseImage`).
+        By **default**, forced support is **disabled** for all render style classes.
 
         NOTE:
             * This property is :term:`descendant`.
             * This doesn't affect the return value of :py:meth:`is_supported` but
               may affect operations that require that a render style be supported e.g
               instantiation of some render style classes.
         """,
     )
 
-    @forced_support.setter
-    def forced_support(cls, status):
-        if not isinstance(status, bool):
-            raise TypeError(f"Invalid type for 'status' (got: {type(status).__name__})")
-
-        cls._forced_support = status
-
     frame_duration = property(
         lambda self: self._frame_duration if self._is_animated else None,
-        doc="""Duration of a single frame for :term:`animated` images
-
-        Returns:
-            * A duration (in seconds), if the image is animated.
-            * ``None``, if the image is not animated.
+        doc="""Duration of a single frame
 
         :type: Optional[float]
 
-        Setting this on non-animated images is simply ignored.
+        GET:
+            Returns:
+
+            * The duration of a single frame (in seconds), if the image is animated.
+            * ``None``, if otherwise.
+
+        SET:
+            If the image is animated, The frame duration is set.
+            Otherwise, nothing is done.
         """,
     )
 
     @frame_duration.setter
     def frame_duration(self, value: float) -> None:
         if not isinstance(value, float):
-            raise TypeError(f"Invalid duration type (got: {type(value).__name__})")
+            raise arg_type_error("frame_duration", value)
         if value <= 0.0:
-            raise ValueError(f"Invalid frame duration (got: {value})")
+            raise arg_value_error_range("frame_duration", value)
         if self._is_animated:
             self._frame_duration = value
 
     height = property(
         lambda self: self._size if isinstance(self._size, Size) else self._size[1],
         lambda self, height: self.set_size(height=height),
         doc="""
-        The **unscaled** height of the image
+        Image height
+
+        :type: Union[Size, int]
+
+        GET:
+            Returns:
 
-        Returns:
             * The image height (in lines), if the image size is
               :term:`fixed <fixed size>`.
-            * A :py:class:`~term_image.image.Size` enum member; if the image size
+            * A :py:class:`~term_image.image.Size` enum member, if the image size
               is :term:`dynamic <dynamic size>`.
 
-        :type: Union[Size, int]
-
-        SETTABLE VALUES:
-
-        * a positive :py:class:`int`; the image height is set to the given value and
-          the width is set proportionally.
-        * a :py:class:`~term_image.image.Size` enum member; the image size
-          is set as prescibed by the enum member.
-        * ``None``; equivalent to :py:attr:`~term_image.image.Size.FIT`.
+        SET:
+            If set to:
 
-        Setting this
+            * a positive :py:class:`int`; the image height is set to the given value
+              and the width is set proportionally.
+            * a :py:class:`~term_image.image.Size` enum member; the image size is set
+              as prescibed by the enum member.
+            * ``None``; equivalent to :py:attr:`~term_image.image.Size.FIT`.
 
-        * results in a :term:`fixed size`.
-        * resets the recognized advanced sizing options to their defaults.
+            This results in a :term:`fixed size`.
         """,
     )
 
     is_animated = property(
         lambda self: self._is_animated,
-        doc="``True`` if the image is :term:`animated`. Otherwise, ``False``.",
+        doc="""
+        Animatability of the image
+
+        :type: bool
+
+        GET:
+            Returns ``True`` if the image is :term:`animated`. Otherwise, ``False``.
+        """,
     )
 
     original_size = property(
         lambda self: self._original_size,
-        doc="""Size of the source image (in pixels)
+        doc="""Size of the source (in pixels)
 
         :type: Tuple[int, int]
+
+        GET:
+            Returns the source size.
         """,
     )
 
     @property
     def n_frames(self) -> int:
-        """The number of frames in the image
+        """Image frame count
 
         :type: int
+
+        GET:
+            Returns the number of frames the image has.
         """
         if not self._is_animated:
             return 1
 
         if not self._n_frames:
             img = self._get_image()
             try:
                 self._n_frames = img.n_frames
             finally:
                 self._close_image(img)
 
         return self._n_frames
 
     rendered_height = property(
-        lambda self: round(
-            (
-                self._valid_size(None, self._size)
-                if isinstance(self._size, Size)
-                else self._size
-            )[1]
-            * self._scale[1]
-        )
-        or 1,
+        lambda self: (
+            self._valid_size(None, self._size)
+            if isinstance(self._size, Size)
+            else self._size
+        )[1],
         doc="""
-        The **scaled** height of the image
-
-        Also the exact number of lines that the drawn image will occupy in a terminal.
+        The height with which the image is :term:`rendered`
 
         :type: int
+
+        GET:
+            Returns the number of lines the image will occupy when drawn in a terminal.
         """,
     )
 
     rendered_size = property(
-        lambda self: tuple(
-            map(
-                lambda x: x or 1,
-                map(
-                    round,
-                    map(
-                        mul,
-                        (
-                            self._valid_size(self._size, None)
-                            if isinstance(self._size, Size)
-                            else self._size
-                        ),
-                        self._scale,
-                    ),
-                ),
-            )
+        lambda self: (
+            self._valid_size(self._size, None)
+            if isinstance(self._size, Size)
+            else self._size
         ),
         doc="""
-        The **scaled** size of the image
-
-        Also the exact number of columns and lines (respectively) that the drawn image
-        will occupy in a terminal.
+        The size with which the image is :term:`rendered`
 
         :type: Tuple[int, int]
+
+        GET:
+            Returns the number of columns and lines (respectively) the image will
+            occupy when drawn in a terminal.
         """,
     )
 
     rendered_width = property(
-        lambda self: round(
-            (
-                self._valid_size(self._size, None)
-                if isinstance(self._size, Size)
-                else self._size
-            )[0]
-            * self._scale[0]
-        )
-        or 1,
+        lambda self: (
+            self._valid_size(self._size, None)
+            if isinstance(self._size, Size)
+            else self._size
+        )[0],
         doc="""
-        The **scaled** width of the image
-
-        Also the exact number of columns that the drawn image will occupy in a terminal.
+        The width with which the image is :term:`rendered`
 
         :type: int
-        """,
-    )
-
-    scale = property(
-        lambda self: tuple(self._scale),
-        doc="""
-        Image :term:`scale`
-
-        SETTABLE VALUES:
-
-        * A *scale value*; sets both axes.
-        * A :py:class:`tuple` of two *scale values*; sets ``(x, y)`` respectively.
 
-        A scale value is a :py:class:`float` in the range **0.0 < value <= 1.0**.
-
-        :type: Tuple[float, float]
-        """,
-    )
-
-    @scale.setter
-    def scale(self, scale: Union[float, Tuple[float, float]]) -> None:
-        if isinstance(scale, float):
-            if not 0.0 < scale <= 1.0:
-                raise ValueError(f"Scale value out of range (got: {scale})")
-            self._scale[:] = (scale,) * 2
-        elif isinstance(scale, tuple):
-            self._scale[:] = self._check_scale(scale)
-        else:
-            raise TypeError("'scale' must be a float or a tuple of floats")
-
-    scale_x = property(
-        lambda self: self._scale[0],
-        doc="""
-        Horizontal :term:`scale`
-
-        A scale value is a :py:class:`float` in the range **0.0 < x <= 1.0**.
-
-        :type: float
-        """,
-    )
-
-    @scale_x.setter
-    def scale_x(self, x: float) -> None:
-        self._scale[0] = self._check_scale_2(x)
-
-    scale_y = property(
-        lambda self: self._scale[1],
-        doc="""
-        Vertical :term:`scale`
-
-        A scale value is a :py:class:`float` in the range **0.0 < y <= 1.0**.
-
-        :type: float
+        GET:
+            Returns the number of columns the image will occupy when drawn in a
+            terminal.
         """,
     )
 
-    @scale_y.setter
-    def scale_y(self, y: float) -> None:
-        self._scale[1] = self._check_scale_2(y)
-
     size = property(
         lambda self: self._size,
         doc="""
-        The **unscaled** size of the image
+        Image size
+
+        :type: Union[Size, Tuple[int, int]]
+
+        GET:
+            Returns:
 
-        Returns:
             * The image size, ``(columns, lines)``, if the image size is
               :term:`fixed <fixed size>`.
             * A :py:class:`~term_image.image.Size` enum member, if the image size
               is :term:`dynamic <dynamic size>`.
 
-        :type: Union[Size, Tuple[int, int]]
-
-        SETTABLE VALUES:
+        SET:
+            If set to a:
 
-        * A :py:class:`~term_image.image.Size` enum member; the image size
-          is set as prescibed by the enum member.
+            * :py:class:`~term_image.image.Size` enum member, the image size is set
+              as prescibed by the given member.
 
-        Setting this
+              This results in a :term:`dynamic size` i.e the size is computed whenever
+              the image is :term:`rendered` using the default :term:`frame size`.
 
-        * implies :term:`dynamic sizing` i.e the size is computed whenever the image is
-          :term:`rendered`.
-        * resets the recognized advanced sizing options to their defaults.
+            * 2-tuple of integers, ``(width, height)``, the image size set as given.
 
-        This is multiplied by the :term:`scale` on respective axes when the image
-        is :term:`rendered`.
+              This results in a :term:`fixed size` i.e the size will not change until
+              it is re-set.
         """,
     )
 
     @size.setter
-    def size(self, value: Size) -> None:
-        if not isinstance(value, Size):
-            raise TypeError("'size' must be a `Size` enum member")
-        self._size = value
-        self._fit_to_width = value is Size.FIT_TO_WIDTH
-        self._h_allow = 0
-        self._v_allow = 2  # A 2-line allowance for the shell prompt, etc
+    def size(self, size: Size | Tuple[int, int]) -> None:
+        if isinstance(size, Size):
+            self._size = size
+        elif isinstance(size, tuple):
+            if len(size) != 2:
+                raise arg_value_error("size", size)
+            self.set_size(*size)
+        else:
+            raise arg_type_error("size", size)
 
     source = property(
         _close_validated(lambda self: getattr(self, self._source_type.value)),
         doc="""
-        The :term:`source` from which the instance was initialized
+        Image :term:`source`
 
         :type: Union[PIL.Image.Image, str]
+
+        GET:
+            Returns the :term:`source` from which the instance was initialized.
         """,
     )
 
     source_type = property(
         lambda self: self._source_type,
         doc="""
-        The kind of :term:`source` from which the instance was initialized
+        Image :term:`source` type
 
         :type: ImageSource
+
+        GET:
+            Returns the type of :term:`source` from which the instance was initialized.
         """,
     )
 
     width = property(
         lambda self: self._size if isinstance(self._size, Size) else self._size[0],
         lambda self, width: self.set_size(width),
         doc="""
-        The **unscaled** width of the image
+        Image width
+
+        :type: Union[Size, int]
+
+        GET:
+            Returns:
 
-        Returns:
             * The image width (in columns), if the image size is
               :term:`fixed <fixed size>`.
             * A :py:class:`~term_image.image.Size` enum member; if the image size
               is :term:`dynamic <dynamic size>`.
 
-        :type: Union[Size, int]
-
-        SETTABLE VALUES:
-
-        * a positive :py:class:`int`; the image width is set to the given value and
-          the height is set proportionally.
-        * a :py:class:`~term_image.image.Size` enum member; the image size
-          is set as prescibed by the enum member.
-        * ``None``; equivalent to :py:attr:`~term_image.image.Size.FIT`.
+        SET:
+            If set to:
 
-        Setting this
+            * a positive :py:class:`int`; the image width is set to the given value
+              and the height is set proportionally.
+            * a :py:class:`~term_image.image.Size` enum member; the image size is set
+              as prescibed by the enum member.
+            * ``None``; equivalent to :py:attr:`~term_image.image.Size.FIT`.
 
-        * results in a :term:`fixed size`.
-        * resets the recognized advanced sizing options to their defaults.
+            This results in a :term:`fixed size`.
         """,
     )
 
     # # Private
 
     @property
     @abstractmethod
@@ -712,155 +627,150 @@
             pass  # Instance creation or initialization was unsuccessful
         finally:
             self._closed = True
 
     def draw(
         self,
         h_align: Optional[str] = None,
-        pad_width: Optional[int] = None,
+        pad_width: int = 0,
         v_align: Optional[str] = None,
-        pad_height: Optional[int] = None,
+        pad_height: int = -2,
         alpha: Optional[float, str] = _ALPHA_THRESHOLD,
         *,
-        scroll: bool = False,
         animate: bool = True,
         repeat: int = -1,
         cached: Union[bool, int] = 100,
+        scroll: bool = False,
         check_size: bool = True,
         **style: Any,
     ) -> None:
-        """Draws an image to standard output.
+        """Draws the image to standard output.
 
         Args:
             h_align: Horizontal alignment ("left" / "<", "center" / "|" or
               "right" / ">"). Default: center.
             pad_width: Number of columns within which to align the image.
 
               * Excess columns are filled with spaces.
-              * Must not be greater than the
-                :term:`available terminal width <available width>`.
-              * Default: terminal width, minus horizontal allowance.
+              * Must not be greater than the :term:`terminal width`.
 
             v_align: Vertical alignment ("top"/"^", "middle"/"-" or "bottom"/"_").
               Default: middle.
             pad_height: Number of lines within which to align the image.
 
               * Excess lines are filled with spaces.
-              * Must not be greater than the :term:`available terminal height
-                <available height>`, **for animations**.
-              * Default: terminal height, minus vertical allowance.
+              * Must not be greater than the :term:`terminal height`,
+                **for animations**.
 
             alpha: Transparency setting.
 
               * If ``None``, transparency is disabled (alpha channel is removed).
               * If a ``float`` (**0.0 <= x < 1.0**), specifies the alpha ratio
                 **above** which pixels are taken as **opaque**. **(Applies to only
                 text-based render styles)**.
               * If a string, specifies a color to replace transparent background with.
                 Can be:
 
                 * **"#"** -> The terminal's default background color (or black, if
                   undetermined) is used.
                 * A hex color e.g ``ffffff``, ``7faa52``.
 
-            scroll: Only applies to non-animations. If ``True``, allows the image's
-                :term:`rendered height` to be greater than the
-                :term:`available terminal height <available height>`.
-
             animate: If ``False``, disable animation i.e draw only the current frame of
               an animated image.
             repeat: The number of times to go over all frames of an animated image.
               A negative value implies infinite repetition.
             cached: Determines if :term:`rendered` frames of an animated image will be
               cached (for speed up of subsequent renders of the same frame) or not.
 
               * If :py:class:`bool`, it directly sets if the frames will be cached or
                 not.
               * If :py:class:`int`, caching is enabled only if the framecount of the
                 image is less than or equal to the given number.
 
-            check_size: If ``False``, does not perform size validation for
-              non-animations.
+            scroll: Only applies to non-animations. If ``True``, allows the image's
+              :term:`rendered height` to be greater than the :term:`terminal height`.
+            check_size: If ``False``, rendered size validation is not performed for
+              non-animations. Does not affect padding size validation.
             style: Style-specific render parameters. See each subclass for it's own
               usage.
 
         Raises:
             TypeError: An argument is of an inappropriate type.
             ValueError: An argument is of an appropriate type but has an
               unexpected/invalid value.
-            ValueError: Unable to convert or resize image.
             term_image.exceptions.InvalidSizeError: The image's :term:`rendered size`
-              can not fit into the :term:`available terminal size <available size>`.
-            term_image.exceptions.StyleError: Unrecognized style-specific parameter(s).
+              can not fit into the :term:`terminal size`.
+            term_image.exceptions.StyleError: Unrecognized style-specific render
+              parameter(s).
+            term_image.exceptions.RenderError: An error occured during
+              :term:`rendering`.
+
+        * If *pad_width* or *pad_height* is:
+
+          * positive, it is **absolute** and used as-is.
+          * non-positive, it is **relative** to the corresponding terminal dimension
+            (**at the point of calling this method**) and equivalent to the absolute
+            dimension ``max(terminal_dimension + frame_dimension, 1)``.
 
-        * If :py:meth:`set_size` was used to set the image size, the horizontal and
-          vertical allowances (set when :py:meth:`set_size` was called) are taken into
-          consideration during size validation. If the size was set via another means or
-          the size is :term:`dynamic <dynamic size>`, the default allowances apply.
-        * For **non-animations**, if the image size was set with
-          :py:attr:`~term_image.image.Size.FIT_TO_WIDTH`, the image **height** is not
-          validated and setting *scroll* is unnecessary.
+        * :term:`padding width` is always validated.
         * *animate*, *repeat* and *cached* apply to :term:`animated` images only.
           They are simply ignored for non-animated images.
         * For animations (i.e animated images with *animate* set to ``True``):
 
           * *scroll* is ignored.
-          * Image size and :term:`padding height` are always validated, if set or given.
-          * **with the exception of native animations provided by some render styles**.
+          * Image size is always validated, if set.
+          * :term:`Padding height` is always validated.
 
         * Animations, **by default**, are infinitely looped and can be terminated
-          with :py:data:`~signal.SIGINT` (``CTRL + C``), raising
+          with :py:data:`~signal.SIGINT` (``CTRL + C``), **without** raising
           :py:class:`KeyboardInterrupt`.
         """
         fmt = self._check_formatting(h_align, pad_width, v_align, pad_height)
 
         if alpha is not None:
             if isinstance(alpha, float):
                 if not 0.0 <= alpha < 1.0:
-                    raise ValueError(f"Alpha threshold out of range (got: {alpha})")
+                    raise arg_value_error_range("alpha", alpha)
             elif isinstance(alpha, str):
                 if not _ALPHA_BG_FORMAT.fullmatch(alpha):
-                    raise ValueError(f"Invalid hex color string (got: {alpha})")
+                    raise arg_value_error_msg("Invalid hex color string", alpha)
             else:
-                raise TypeError(
-                    "'alpha' must be `None` or of type `float` or `str` "
-                    f"(got: {type(alpha).__name__})"
-                )
+                raise arg_type_error("alpha", alpha)
 
         if self._is_animated and not isinstance(animate, bool):
-            raise TypeError("'animate' must be a boolean")
+            raise arg_type_error("animate", animate)
 
-        if None is not pad_width > get_terminal_size()[0] - self._h_allow:
-            raise ValueError(
-                "Padding width is greater than the available terminal width"
+        terminal_width, terminal_height = get_terminal_size()
+        if pad_width > terminal_width:
+            raise arg_value_error_range(
+                "pad_width", pad_width, got_extra=f"terminal_width={terminal_width}"
             )
 
-        if (
-            not style.get("native")
-            and self._is_animated
-            and animate
-            and None is not pad_height > get_terminal_size()[1]
-        ):
-            raise ValueError(
-                "Padding height can not be greater than the terminal height for "
-                "animations"
+        animation = self._is_animated and animate
+
+        if animation and pad_height > terminal_height:
+            raise arg_value_error_range(
+                "pad_height",
+                pad_height,
+                got_extra=f"terminal_height={terminal_height}, animation={animation}",
             )
 
         for arg in ("scroll", "check_size"):
-            if not isinstance(locals()[arg], bool):
-                raise TypeError(f"{arg!r} must be a boolean")
+            arg_value = locals()[arg]
+            if not isinstance(arg_value, bool):
+                raise arg_type_error(arg, arg_value)
 
         # Checks for *repeat* and *cached* are delegated to `ImageIterator`.
 
         def render(image: PIL.Image.Image) -> None:
             # Hide the cursor immediately if the output is a terminal device
-            sys.stdout.isatty() and print(f"{CSI}?25l", end="", flush=True)
+            sys.stdout.isatty() and print(HIDE_CURSOR, end="", flush=True)
             try:
                 style_args = self._check_style_args(style)
-                if self._is_animated and animate:
+                if animation:
                     self._display_animated(
                         image, alpha, fmt, repeat, cached, **style_args
                     )
                 else:
                     try:
                         print(
                             self._format_render(
@@ -871,28 +781,28 @@
                             flush=True,
                         )
                     except (KeyboardInterrupt, Exception):
                         self._handle_interrupted_draw()
                         raise
             finally:
                 # Reset color and show the cursor
-                print(COLOR_RESET, f"{CSI}?25h" * sys.stdout.isatty(), sep="")
+                print(SGR_NORMAL, SHOW_CURSOR * sys.stdout.isatty(), sep="")
 
         self._renderer(
             render,
             scroll=scroll,
             check_size=check_size,
-            animated=not style.get("native") and self._is_animated and animate,
+            animated=animation,
         )
 
     @classmethod
     def from_file(
         cls,
         filepath: Union[str, os.PathLike],
-        **kwargs: Union[None, int, Tuple[float, float]],
+        **kwargs: Union[None, int],
     ) -> BaseImage:
         """Creates an instance from an image file.
 
         Args:
             filepath: Relative/Absolute path to an image file.
             kwargs: Same keyword arguments as the class constructor.
 
@@ -904,18 +814,15 @@
             FileNotFoundError: The given path does not exist.
             IsADirectoryError: Propagated from from :py:func:`PIL.Image.open`.
             PIL.UnidentifiedImageError: Propagated from from :py:func:`PIL.Image.open`.
 
         Also Propagates exceptions raised or propagated by the class constructor.
         """
         if not isinstance(filepath, (str, os.PathLike)):
-            raise TypeError(
-                "File path must be a string or path-like object "
-                f"(got: {type(filepath).__name__!r})."
-            )
+            raise arg_type_error("filepath", filepath)
 
         if isinstance(filepath, os.PathLike):
             filepath = filepath.__fspath__()
             if isinstance(filepath, bytes):
                 filepath = filepath.decode()
 
         # Intentionally propagates `IsADirectoryError` since the message is OK
@@ -935,15 +842,15 @@
         new._source_type = ImageSource.FILE_PATH
         return new
 
     @classmethod
     def from_url(
         cls,
         url: str,
-        **kwargs: Union[None, int, Tuple[float, float]],
+        **kwargs: Union[None, int],
     ) -> BaseImage:
         """Creates an instance from an image URL.
 
         Args:
             url: URL of an image file.
             kwargs: Same keyword arguments as the class constructor.
 
@@ -965,17 +872,17 @@
 
             - when :py:meth:`close` is called,
             - upon exiting a ``with`` statement block that uses the instance as a
               context manager, or
             - when the instance is garbage collected.
         """
         if not isinstance(url, str):
-            raise TypeError(f"URL must be a string (got: {type(url).__name__!r}).")
+            raise arg_type_error("url", url)
         if not all(urlparse(url)[:3]):
-            raise ValueError(f"Invalid URL: {url!r}")
+            raise arg_value_error_msg("Invalid URL", url)
 
         # Propagates connection-related errors.
         response = requests.get(url, stream=True)
         if response.status_code == 404:
             raise URLNotFoundError(f"URL {url!r} does not exist.")
 
         # Ensure initialization is successful before writing to file
@@ -1027,35 +934,33 @@
             TypeError: An argument is of an inappropriate type.
             ValueError: An argument is of an appropriate type but has an
               unexpected/invalid value.
 
         Frame numbers start from 0 (zero).
         """
         if not isinstance(pos, int):
-            raise TypeError(f"Invalid frame number type (got: {type(pos).__name__})")
+            raise arg_type_error("pos", pos)
         if not 0 <= pos < self.n_frames:
-            raise ValueError(
-                f"Frame number out of range (got: {pos}, n_frames={self.n_frames})"
-            )
+            raise arg_value_error_range("pos", pos, f"n_frames={self.n_frames}")
         if self._is_animated:
             self._seek_position = pos
 
     @ClassInstanceMethod
-    def set_render_method(self_or_cls, method: Optional[str] = None) -> None:
+    def set_render_method(cls, method: Optional[str] = None) -> None:
         """Sets the :term:`render method` used by instances of a :term:`render style`
         class that implements multiple render methods.
 
         Args:
             method: The render method to be set or ``None`` for a reset
               (case-insensitive).
 
         Raises:
-            TypeError: *method* is not a string or ``None``.
-            ValueError: the given method is not implmented by the invoking class
-              (or class of the invoking instance).
+            TypeError: An argument is of an inappropriate type.
+            ValueError: An argument is of an appropriate type but has an
+              unexpected/invalid value.
 
         See the **Render Methods** section in the description of subclasses that
         implement such for their specific usage.
 
         If *method* is not ``None`` and this method is called via:
 
         - a class, the class-wide render method is set.
@@ -1073,169 +978,141 @@
         NOTE:
             *method* = ``None`` is always allowed, even if the render style doesn't
             implement multiple render methods.
 
             The **class-wide** render method is :term:`descendant`.
         """
         if method is not None and not isinstance(method, str):
-            raise TypeError(
-                f"'method' must be a string or `None` (got: {type(method).__name__!r})"
-            )
+            raise arg_type_error("method", method)
+        if method is not None and method.lower() not in cls._render_methods:
+            raise ValueError(f"Unknown render method {method!r} for {cls.__name__}")
+
+        if not method:
+            if cls._render_methods:
+                cls._render_method = cls._default_render_method
+        else:
+            cls._render_method = method
 
-        if method is not None and method.lower() not in self_or_cls._render_methods:
-            cls = (
-                type(self_or_cls) if isinstance(self_or_cls, __class__) else self_or_cls
+    @set_render_method.instancemethod
+    def set_render_method(self, method: Optional[str] = None) -> None:
+        if method is not None and not isinstance(method, str):
+            raise arg_type_error("method", method)
+        if method is not None and method.lower() not in type(self)._render_methods:
+            raise ValueError(
+                f"Unknown render method {method!r} for {type(self).__name__}"
             )
-            raise ValueError(f"Unknown render method {method!r} for {cls.__name__}")
 
         if not method:
-            if isinstance(self_or_cls, __class__):
-                try:
-                    del self_or_cls._render_method
-                except AttributeError:
-                    pass
-            elif self_or_cls._render_methods:
-                self_or_cls._render_method = self_or_cls._default_render_method
+            try:
+                del self._render_method
+            except AttributeError:
+                pass
         else:
-            self_or_cls._render_method = method
+            self._render_method = method
 
     def set_size(
         self,
         width: Union[int, Size, None] = None,
         height: Union[int, Size, None] = None,
-        h_allow: int = 0,
-        v_allow: int = 2,
-        maxsize: Optional[Tuple[int, int]] = None,
+        frame_size: Tuple[int, int] = (0, -2),
     ) -> None:
-        """Sets the image size with extended control.
+        """Sets the image size (with extended control).
 
         Args:
             width: Can be
 
-              * an integer; horizontal dimension of the image, in columns.
+              * a positive integer; horizontal dimension of the image, in columns.
               * a :py:class:`~term_image.image.Size` enum member.
 
             height: Can be
 
-              * an integer; vertical dimension of the image, in lines.
+              * a positive integer; vertical dimension of the image, in lines.
               * a :py:class:`~term_image.image.Size` enum member.
 
-            h_allow: Horizontal allowance i.e minimum number of columns to leave unused.
-            v_allow: Vertical allowance i.e minimum number of lines to leave unused.
-            maxsize: If given, as ``(columns, lines)``, it's used instead of the
-              terminal size.
+            frame_size: :term:`Frame size`, ``(columns, lines)``.
+              If *columns* or *lines* is
+
+              * positive, it is **absolute** and used as-is.
+              * non-positive, it is **relative** to the corresponding terminal dimension
+                and equivalent to the absolute dimension
+                ``max(terminal_dimension + frame_dimension, 1)``.
+
+              This is used only when neither *width* nor *height* is an ``int``.
 
         Raises:
             TypeError: An argument is of an inappropriate type.
             ValueError: An argument is of an appropriate type but has an
               unexpected/invalid value.
-            ValueError: Both *width* and *height* are specified.
-            ValueError: The :term:`available size` is too small for
-              :term:`automatic sizing`.
-            term_image.exceptions.InvalidSizeError: *maxsize* is given and the
-              resulting size will not fit into it.
 
-        If neither *width* nor *height* is given (or both are ``None``),
-        :py:attr:`~term_image.image.Size.FIT` applies.
-
-        If *width* or *height* is a :py:class:`~term_image.image.Size` enum
-        member, :term:`automatic sizing` applies as prescribed by the enum member.
-
-        When :py:attr:`~term_image.image.Size.FIT_TO_WIDTH` is given,
-
-        * size validation operations take it into consideration.
-        * :term:`Vertical allowance` is nullified.
-
-        :term:`Allowances <allowance>` are ignored when *maxsize* is given.
-
-        Render formatting and size validation operations recognize and respect the
-        horizontal and vertical allowances, until the image size is re-set.
-
-        NOTE:
-           The size is checked to fit in only when *maxsize* is given along with a fixed
-           *width* or *height* because :py:meth:`draw` is generally not the means of
-           drawing such an image and all rendering methods don't perform any sort of
-           size validation.
-
-           If the validation is not desired, specify only one of *maxsize* and
-           *width* or *height*, not both.
+        * If both width and height are not ``None``, they must be positive integers
+          and :term:`manual sizing` applies i.e the image size is set as given without
+          preserving aspect ratio.
+        * If *width* or *height* is a :py:class:`~term_image.image.Size` enum
+          member, :term:`automatic sizing` applies as prescribed by the enum member.
+        * If neither *width* nor *height* is given (or both are ``None``),
+          :py:attr:`~term_image.image.Size.FIT` applies.
         """
+        width_height = (width, height)
+        for arg_name, arg_value in zip(("width", "height"), width_height):
+            if not (arg_value is None or isinstance(arg_value, (Size, int))):
+                raise arg_type_error(arg_name, arg_value)
+            if isinstance(arg_value, int) and arg_value <= 0:
+                raise arg_value_error_range(arg_name, arg_value)
+
         if width is not None is not height:
-            raise ValueError("Cannot specify both width and height")
-        for argname, x in zip(("width", "height"), (width, height)):
-            if not (x is None or isinstance(x, (Size, int))):
+            if not all(isinstance(x, int) for x in width_height):
+                width_type = type(width).__name__
+                height_type = type(height).__name__
                 raise TypeError(
-                    f"{argname!r} must be `None`, a `Size` enum member or an integer "
-                    f"(got: type {type(x).__name__!r})"
+                    "Both 'width' and 'height' are specified but are not both integers "
+                    f"(got: ({width_type}, {height_type}))"
                 )
-            if isinstance(x, int) and x <= 0:
-                raise ValueError(f"{argname!r} must be positive (got: {x})")
 
-        for argname, x in zip(("h_allow", "v_allow"), (h_allow, v_allow)):
-            if not isinstance(x, int):
-                raise TypeError(
-                    f"{argname!r} must be an integer (got: type {type(x).__name__!r})"
-                )
-            if x < 0:
-                raise ValueError(f"{argname!r} must be non-negative (got: {x})")
+            self._size = width_height
+            return
 
-        if maxsize is not None:
-            if not (
-                isinstance(maxsize, tuple) and all(isinstance(x, int) for x in maxsize)
-            ):
-                raise TypeError(
-                    f"'maxsize' must be a tuple of integers (got: {maxsize!r})"
-                )
-
-            if not (len(maxsize) == 2 and all(x > 0 for x in maxsize)):
-                raise ValueError(
-                    f"'maxsize' must contain two positive integers (got: {maxsize})"
-                )
+        if not (
+            isinstance(frame_size, tuple)
+            and all(isinstance(x, int) for x in frame_size)
+        ):
+            raise arg_type_error("frame_size", frame_size)
+        if not len(frame_size) == 2:
+            raise arg_value_error("frame_size", frame_size)
 
-        fit_to_width = Size.FIT_TO_WIDTH in (width, height)
-        self._size = self._valid_size(
-            width,
-            height,
-            h_allow,
-            v_allow * (not fit_to_width),
-            maxsize,
-        )
-        self._fit_to_width = fit_to_width
-        self._h_allow = h_allow
-        self._v_allow = v_allow * (not fit_to_width)
+        self._size = self._valid_size(width, height, frame_size)
 
     def tell(self) -> int:
         """Returns the current image frame number.
 
         :rtype: int
         """
         return self._seek_position if self._is_animated else 0
 
     # Private Methods
 
     @classmethod
     def _check_format_spec(
         cls, spec: str
     ) -> Tuple[
-        Optional[str],
-        Optional[int],
-        Optional[str],
-        Optional[int],
+        str | None,
+        int,
+        str | None,
+        int,
         Union[None, float, str],
         Dict[str, Any],
     ]:
         """Validates a format specifier and translates it into the required values.
 
         Returns:
             A tuple ``(h_align, width, v_align, height, alpha, style_args)`` containing
             values as required by ``_format_render()`` and ``_render_image()``.
         """
         match_ = _FORMAT_SPEC.fullmatch(spec)
         if not match_ or _NO_VERTICAL_SPEC.fullmatch(spec):
-            raise ValueError(f"Invalid format specifier (got: {spec!r})")
+            raise arg_value_error_msg("Invalid format specifier", spec)
 
         (
             _,
             h_align,
             width,
             _,
             v_align,
@@ -1244,15 +1121,18 @@
             threshold_or_bg,
             _,
             style_spec,
         ) = match_.groups()
 
         return (
             *cls._check_formatting(
-                h_align, width and int(width), v_align, height and int(height)
+                h_align,
+                int(width) if width else 0,
+                v_align,
+                int(height) if height else -2,
             ),
             (
                 threshold_or_bg
                 and (
                     "#" + threshold_or_bg.lstrip("#")
                     if _ALPHA_BG_FORMAT.fullmatch("#" + threshold_or_bg.lstrip("#"))
                     else float(threshold_or_bg)
@@ -1261,91 +1141,51 @@
                 else _ALPHA_THRESHOLD
             ),
             style_spec and cls._check_style_format_spec(style_spec, style_spec) or {},
         )
 
     @staticmethod
     def _check_formatting(
-        h_align: Optional[str] = None,
-        width: Optional[int] = None,
-        v_align: Optional[str] = None,
-        height: Optional[int] = None,
-    ) -> Tuple[Union[None, str, int]]:
-        """Validates formatting arguments while also translating literal ones.
+        h_align: str | None = None,
+        width: int = 0,
+        v_align: str | None = None,
+        height: int = -2,
+    ) -> Tuple[str | None, int, str | None, int]:
+        """Validates and transforms formatting arguments.
 
         Returns:
             The respective arguments appropriate for ``_format_render()``.
         """
         if not isinstance(h_align, (type(None), str)):
-            raise TypeError("'h_align' must be a string.")
+            raise arg_type_error("h_align", h_align)
         if None is not h_align not in set("<|>"):
             align = {"left": "<", "center": "|", "right": ">"}.get(h_align)
             if not align:
-                raise ValueError(f"Invalid horizontal alignment option: {h_align!r}")
+                raise arg_value_error("h_align", h_align)
             h_align = align
 
-        if not isinstance(width, (type(None), int)):
-            raise TypeError("Padding width must be `None` or an integer.")
-        if width is not None:
-            if width <= 0:
-                raise ValueError(f"Padding width must be positive (got: {width})")
-
         if not isinstance(v_align, (type(None), str)):
-            raise TypeError("'v_align' must be a string.")
+            raise arg_type_error("v_align", v_align)
         if None is not v_align not in set("^-_"):
             align = {"top": "^", "middle": "-", "bottom": "_"}.get(v_align)
             if not align:
-                raise ValueError(f"Invalid vertical alignment option: {v_align!r}")
+                raise arg_value_error("v_align", v_align)
             v_align = align
 
-        if not isinstance(height, (type(None), int)):
-            raise TypeError("Padding height must be `None` or an integer.")
-        if None is not height <= 0:
-            raise ValueError(f"Padding height must be positive (got: {height})")
-
-        return h_align, width, v_align, height
-
-    @staticmethod
-    def _check_scale(scale: Tuple[float, float]) -> Tuple[float, float]:
-        """Checks a tuple of scale values.
-
-        Returns:
-            The tuple of scale values, if valid.
-
-        Raises:
-            TypeError: The object is not a tuple of ``float``\\ s.
-            ValueError: The object is not a 2-tuple or the values are out of range.
-        """
-        if not (isinstance(scale, tuple) and all(isinstance(x, float) for x in scale)):
-            raise TypeError(f"'scale' must be a tuple of floats (got: {scale!r})")
-
-        if not (len(scale) == 2 and all(0.0 < x <= 1.0 for x in scale)):
-            raise ValueError(
-                f"'scale' must be a tuple of two floats, 0.0 < x <= 1.0 (got: {scale})"
-            )
-        return scale
-
-    @staticmethod
-    def _check_scale_2(value: float) -> float:
-        """Checks a single scale value.
+        terminal_size = get_terminal_size()
 
-        Returns:
-            The scale value, if valid.
+        if not isinstance(width, int):
+            raise arg_type_error("pad_width", width)
+        width = width if width > 0 else max(terminal_size.columns + width, 1)
+
+        if not isinstance(height, int):
+            raise arg_type_error("pad_height", height)
+        height = height if height > 0 else max(terminal_size.lines + height, 1)
 
-        Raises:
-            TypeError: The object is not a ``float``.
-            ValueError: The value is out of range.
-        """
-        if not isinstance(value, float):
-            raise TypeError(
-                f"Given value must be a float (got: type {type(value).__name__!r})"
-            )
-        if not 0.0 < value <= 1.0:
-            raise ValueError(f"Scale value out of range (got: {value})")
-        return value
+        return h_align, width, v_align, height
 
     @classmethod
     def _check_style_args(cls, style_args: Dict[str, Any]) -> Dict[str, Any]:
         """Validates style-specific arguments and translates them into the required
         values.
 
         Removes any argument having a value equal to the default.
@@ -1367,16 +1207,17 @@
                     (check_type, type_msg),
                     (check_value, value_msg),
                 ) = cls._style_args[name]
             except KeyError:
                 for other_cls in cls.__mro__:
                     # less costly than memebership tests on every class' __bases__
                     if other_cls is __class__:
-                        raise _style_error(cls)(
-                            f"Unknown style-specific parameter {name!r}"
+                        raise StyleError(
+                            f"Unknown style-specific render parameter {name!r} for "
+                            f"{cls.__name__!r}"
                         )
 
                     if not issubclass(
                         other_cls, __class__
                     ) or "_style_args" not in vars(other_cls):
                         continue
 
@@ -1384,16 +1225,17 @@
                         (check_type, type_msg), (check_value, value_msg) = super(
                             other_cls, cls
                         )._style_args[name]
                         break
                     except KeyError:
                         pass
                 else:
-                    raise _style_error(cls)(
-                        f"Unknown style-specific parameter {name!r}"
+                    raise StyleError(
+                        f"Unknown style-specific render parameter {name!r} for "
+                        f"{cls.__name__!r}"
                     )
 
             if not check_type(value):
                 raise TypeError(f"{type_msg} (got: {type(value).__name__})")
             if not check_value(value):
                 raise ValueError(f"{value_msg} (got: {value!r})")
 
@@ -1439,16 +1281,17 @@
         successful check ends up at `BaseImage._check_style_args()` or when *parent* is
         empty.
 
         :py:meth:`_get_style_format_spec` may be used to parse the format spec at each
         level of the call chain.
         """
         if spec:
-            raise _style_error(cls)(
-                f"Invalid style-specific format specifier {original!r}"
+            raise StyleError(
+                f"Invalid style-specific format specifier {original!r} "
+                f"for {cls.__name__!r}"
                 + (f", detected at {spec!r}" if spec != original else "")
             )
         return {}
 
     @classmethod
     def _clear_frame(cls) -> bool:
         """Clears an animation frame on-screen.
@@ -1470,88 +1313,88 @@
         if img is not self._source:
             img.close()
 
     def _display_animated(
         self,
         img: PIL.Image.Image,
         alpha: Union[None, float, str],
-        fmt: Tuple[Union[None, str, int]],
+        fmt: Tuple[str | None, int, str | None, int],
         repeat: int,
         cached: Union[bool, int],
         **style_args: Any,
     ) -> None:
         """Displays an animated GIF image in the terminal."""
-        lines = max(
-            (fmt or (None,))[-1] or get_terminal_size()[1] - self._v_allow,
-            self.rendered_height,
-        )
+        lines = max(fmt[-1], self.rendered_height)
         prev_seek_pos = self._seek_position
         duration = self._frame_duration
         image_it = ImageIterator(self, repeat, "", cached)
         image_it._animator = image_it._animate(img, alpha, fmt, style_args)
+        cursor_up = CURSOR_UP % (lines - 1)
+        cursor_down = CURSOR_DOWN % lines
 
         try:
             print(next(image_it._animator), end="", flush=True)  # First frame
 
             # Render next frame during current frame's duration
             start = time.time()
             for frame in image_it._animator:  # Renders next frame
                 # Left-over of current frame's duration
                 time.sleep(max(0, duration - (time.time() - start)))
 
                 # Clear the current frame, if necessary,
                 # move cursor up to the begining of the first line of the image
                 # and print the new current frame.
                 self._clear_frame()
-                print(f"\r{CSI}{lines - 1}A", frame, sep="", end="", flush=True)
+                print("\r", cursor_up, frame, sep="", end="", flush=True)
 
                 # Render next frame during current frame's duration
                 start = time.time()
-        except (KeyboardInterrupt, Exception):
+        except KeyboardInterrupt:
+            self._handle_interrupted_draw()
+        except Exception:
             self._handle_interrupted_draw()
             raise
         finally:
             image_it.close()
             self._close_image(img)
             self._seek_position = prev_seek_pos
             # Move the cursor to the last line of the image to prevent "overlayed"
             # output in the terminal
-            print(f"{CSI}{lines}B", end="")
+            print(cursor_down, end="")
 
     def _format_render(
         self,
         render: str,
-        h_align: Optional[str] = None,
-        width: Optional[int] = None,
-        v_align: Optional[str] = None,
-        height: Optional[int] = None,
+        h_align: str | None,
+        width: int,
+        v_align: str | None,
+        height: int,
     ) -> str:
-        """Formats rendered image text.
+        """Pads and aligns a primary :term:`render` output.
 
-        All arguments should be passed through ``_check_formatting()`` first.
+        NOTE:
+            * All arguments should be passed through ``_check_formatting()`` first.
+            * Only **absolute** padding dimensions are expected.
         """
         cols, lines = self.rendered_size
-        terminal_size = get_terminal_size()
 
-        width = width or terminal_size[0] - self._h_allow
         if width > cols:
             if h_align == "<":  # left
                 left = ""
                 right = " " * (width - cols)
             elif h_align == ">":  # right
                 left = " " * (width - cols)
                 right = ""
             else:  # center
                 left = " " * ((width - cols) // 2)
                 right = " " * (width - cols - len(left))
             render = render.replace("\n", f"{right}\n{left}")
         else:
             left = right = ""
 
-        height = height or terminal_size[1] - self._v_allow
         if height > lines:
             if v_align == "^":  # top
                 top = 0
                 bottom = height - lines
             elif v_align == "_":  # bottom
                 top = height - lines
                 bottom = 0
@@ -1620,26 +1463,26 @@
 
             if img.mode != mode:
                 prev_img = img
                 try:
                     img = img.convert(mode)
                 # Possible for images in some modes e.g "La"
                 except Exception as e:
-                    raise ValueError("Unable to convert image") from e
+                    raise RenderError("Unable to convert image") from e
                 finally:
                     if frame_img is not prev_img:
                         self._close_image(prev_img)
 
             if img.size != size:
                 prev_img = img
                 try:
                     img = img.resize(size, Image.Resampling.BOX)
                 # Highly unlikely since render size can never be zero
                 except Exception as e:
-                    raise ValueError("Unable to resize image") from e
+                    raise RenderError("Unable to resize image") from e
                 finally:
                     if frame_img is not prev_img:
                         self._close_image(prev_img)
 
         frame_img = img if frame else None
         if self._is_animated:
             img.seek(self._seek_position)
@@ -1682,18 +1525,15 @@
             if pixel_data:
                 rgb = list((img if img.mode == "RGB" else img.convert("RGB")).getdata())
 
         return (img, *(pixel_data and (rgb, a) or (None, None)))
 
     @abstractmethod
     def _get_render_size(self) -> Tuple[int, int]:
-        """Returns the size (in pixels) required to render the image.
-
-        Applies the image scale.
-        """
+        """Returns the size (in pixels) required to render the image."""
         raise NotImplementedError
 
     @classmethod
     def _get_style_format_spec(
         cls, spec: str, original: str
     ) -> Tuple[str, List[Union[None, str, Tuple[Optional[str]]]]]:
         """Parses a style-specific format specifier.
@@ -1749,17 +1589,17 @@
             else:
                 fields.append(
                     (None,) * (pattern.groups + 1) if pattern.groups else None
                 )
 
         parent, invalid = spec[:start], spec[end:]
         if invalid:
-            raise _style_error(cls)(
-                f"Invalid style-specific format specifier {original!r}"
-                f", detected at {invalid!r}"
+            raise StyleError(
+                f"Invalid style-specific format specifier {original!r} "
+                f"for {cls.__name__!r}, detected at {invalid!r}"
             )
 
         return parent, fields
 
     @staticmethod
     def _handle_interrupted_draw():
         """Performs any neccessary actions when image drawing is interrupted."""
@@ -1829,90 +1669,72 @@
 
         Returns:
             The return value of *renderer*.
 
         Raises:
             term_image.exceptions.InvalidSizeError: *check_size* or *animated* is
               ``True`` and the image's :term:`rendered size` can not fit into the
-              :term:`available terminal size <available size>`.
+              :term:`terminal size`.
             term_image.exceptions.TermImageError: The image has been finalized.
-
-        NOTE:
-            For **non-animations**, if the image size was set with
-            :py:attr:term_image.image.Size.FIT_TO_WIDTH`, the image **height** is not
-            validated and setting *scroll* is unnecessary.
         """
         _size = self._size
         try:
             if isinstance(_size, Size):
                 self.set_size(_size)
             elif check_size or animated:
-                # NOTE: If the set size is larger than the available terminal size but
-                # the scale makes it fit in, then it's all good.
-
-                columns, lines = map(
-                    sub,
-                    get_terminal_size(),
-                    # *scroll* nullifies vertical allowance for non-animations
-                    # Makes a difference when terminal height < vertical allowance
-                    (self._h_allow, self._v_allow * (animated or not scroll)),
-                )
-
+                terminal_size = get_terminal_size()
                 if any(
                     map(
                         gt,
-                        # the compared height will be 0 if *_fit_to_width* or *scroll*
-                        # is `True`. So, the height comparison will always be `False`
+                        # The compared height will be 0 if *scroll* is `True`.
+                        # So, the height comparison will always be `False`
                         # since the terminal height should never be < 0.
-                        map(
-                            mul,
-                            self.rendered_size,
-                            (1, not (self._fit_to_width or scroll)),
-                        ),
-                        (columns, lines),
+                        map(mul, self.rendered_size, (1, not scroll)),
+                        terminal_size,
                     )
                 ):
                     raise InvalidSizeError(
                         "The "
                         + ("animation" if animated else "image")
-                        + " cannot fit into the available terminal size"
+                        + " cannot fit into the terminal size"
                     )
 
-                # Reaching here means it's either valid or *_fit_to_width* and/or
-                # *scroll* is/are `True`.
-                if animated and self.rendered_height > lines:
+                # Reaching here means it's either valid or *scroll* is `True`.
+                if animated and self.rendered_height > terminal_size.lines:
                     raise InvalidSizeError(
-                        "The rendered height cannot be greater than the terminal "
-                        "height for animations"
+                        "The rendered height is greater than the terminal height for "
+                        "an animation"
                     )
 
             return renderer(self._get_image(), *args, **kwargs)
 
         finally:
             if isinstance(_size, Size):
                 self.size = _size
 
     def _valid_size(
         self,
         width: Union[int, Size, None] = None,
         height: Union[int, Size, None] = None,
-        h_allow: int = 0,
-        v_allow: int = 2,
-        maxsize: Optional[Tuple[int, int]] = None,
+        frame_size: Tuple[int, int] = (0, -2),
     ) -> Tuple[int, int]:
         """Returns an image size tuple.
 
-        See the description of :py:meth:`set_size` for the parameters.
+        See :py:meth:`set_size` for the description of the parameters.
         """
         ori_width, ori_height = self._original_size
-        columns, lines = maxsize or map(sub, get_terminal_size(), (h_allow, v_allow))
-        max_width = self._pixels_cols(cols=columns)
-        max_height = self._pixels_lines(lines=lines)
-
-        # NOTE: The image scale is not considered since it should never be > 1
+        columns, lines = map(
+            lambda frame_dim, terminal_dim: (
+                frame_dim if frame_dim > 0 else max(terminal_dim + frame_dim, 1)
+            ),
+            frame_size,
+            get_terminal_size(),
+        )
+        frame_width = self._pixels_cols(cols=columns)
+        frame_height = self._pixels_lines(lines=lines)
 
         # As for cell ratio...
         #
         # Take for example, pixel ratio = 2.0
         # (i.e cell ratio = 1.0; square character cells).
         # To adjust the image to the proper scale, we either reduce the
         # width (i.e divide by 2.0) or increase the height (i.e multiply by 2.0).
@@ -1923,33 +1745,29 @@
         # (i.e divide by the 0.5) or reduce the height (i.e multiply by the 0.5).
         #
         # Therefore, for the height, we always multiply by the pixel ratio
         # and for the width, we always divide by the pixel ratio.
         # The non-constraining axis is always the one directly adjusted.
 
         if all(not isinstance(x, int) for x in (width, height)):
-            for name in ("columns", "lines"):
-                if locals()[name] <= 0:
-                    raise ValueError(f"Amount of available {name} too small")
-
             if Size.AUTO in (width, height):
                 width = height = (
                     Size.FIT
                     if (
-                        ori_width > max_width
-                        or round(ori_height * self._pixel_ratio) > max_height
+                        ori_width > frame_width
+                        or round(ori_height * self._pixel_ratio) > frame_height
                     )
                     else Size.ORIGINAL
                 )
             elif Size.FIT_TO_WIDTH in (width, height):
                 return (
-                    self._pixels_cols(pixels=max_width) or 1,
+                    self._pixels_cols(pixels=frame_width) or 1,
                     self._pixels_lines(
                         pixels=round(
-                            self._width_height_px(w=max_width) * self._pixel_ratio
+                            self._width_height_px(w=frame_width) * self._pixel_ratio
                         )
                     )
                     or 1,
                 )
 
             if Size.ORIGINAL in (width, height):
                 return (
@@ -1958,34 +1776,38 @@
                     or 1,
                 )
 
             # The smaller fraction will fit on both axis.
             # Hence, the axis with the smaller ratio is the constraining axis.
             # Constraining by the axis with the larger ratio will cause the image
             # to not fit into the axis with the smaller ratio.
-            x = max_width / ori_width
-            y = max_height / ori_height
-            _width_px = ori_width * min(x, y)
-            _height_px = ori_height * min(x, y)
-
-            # The cell ratio should affect the axis with the larger ratio since the axis
-            # the smaller ratio is already fully occupied
-
-            if x < y:
+            width_ratio = frame_width / ori_width
+            height_ratio = frame_height / ori_height
+            smaller_ratio = min(width_ratio, height_ratio)
+
+            # Set the dimension on the constraining axis to exactly its corresponding
+            # frame dimension and the dimension on the other axis to the same ratio of
+            # its corresponding original image dimension
+            _width_px = ori_width * smaller_ratio
+            _height_px = ori_height * smaller_ratio
+
+            # The cell ratio should directly affect the non-constraining axis since the
+            # constraining axis is already fully occupied at this point
+            if height_ratio > width_ratio:
                 _height_px = _height_px * self._pixel_ratio
                 # If height becomes greater than the max, reduce it to the max
-                height_px = min(_height_px, max_height)
+                height_px = min(_height_px, frame_height)
                 # Calculate the corresponding width
                 width_px = round((height_px / _height_px) * _width_px)
                 # Round the height
                 height_px = round(height_px)
             else:
                 _width_px = _width_px / self._pixel_ratio
                 # If width becomes greater than the max, reduce it to the max
-                width_px = min(_width_px, max_width)
+                width_px = min(_width_px, frame_width)
                 # Calculate the corresponding height
                 height_px = round((width_px / _width_px) * _height_px)
                 # Round the width
                 width_px = round(width_px)
             return (
                 self._pixels_cols(pixels=width_px) or 1,
                 self._pixels_lines(pixels=height_px) or 1,
@@ -1999,20 +1821,14 @@
         elif height is None:
             height_px = round(
                 self._width_height_px(w=self._pixels_cols(cols=width))
                 * self._pixel_ratio
             )
             height = self._pixels_lines(pixels=height_px)
 
-        if maxsize and (width > columns or height > lines):
-            raise InvalidSizeError(
-                f"The resulting size {width, height} will not fit into "
-                f"'maxsize' {maxsize}"
-            )
-
         return (width or 1, height or 1)
 
     def _width_height_px(
         self, *, w: Optional[int] = None, h: Optional[int] = None
     ) -> float:
         """Converts the given width (in pixels) to the **unrounded** proportional height
         (in pixels) OR vice-versa.
@@ -2048,25 +1864,24 @@
 
     def __new__(
         cls,
         image: PIL.Image.Image,
         *,
         width: Union[int, Size, None] = None,
         height: Union[int, Size, None] = None,
-        scale: Tuple[float, float] = (1.0, 1.0),
     ) -> None:
         # calls `is_supported()` first to set required class attributes, in case
         # support is forced for a style that is actually supported
         if not (cls.is_supported() or cls._forced_support):
-            raise _style_error(cls)(
-                "This render style is not supported in the active terminal"
+            raise StyleError(
+                f"{cls.__name__!r} is not supported in the active terminal"
             )
         return super().__new__(cls)
 
-    def _get_minimal_render_size(self, *, adjust: bool) -> Tuple[int, int]:
+    def _get_minimal_render_size(self, *, adjust: bool = False) -> Tuple[int, int]:
         render_size = self._get_render_size()
         r_height = self.rendered_height
         width, height = (
             render_size
             if mul(*render_size) < mul(*self._original_size)
             else self._original_size
         )
@@ -2166,27 +1981,26 @@
         repeat: The number of times to go over the entire image. A negative value
           implies infinite repetition.
         format_spec: The :ref:`format specifier <format-spec>` for the rendered
           frames (default: auto).
         cached: Determines if the :term:`rendered` frames will be cached (for speed up
           of subsequent renders) or not. If it is
 
-          * a boolean, it directly sets if the frames will be cached or not.
-          * an integer, caching is enabled only if the framecount of the image
+          * a boolean, caching is enabled if ``True``. Otherwise, caching is disabled.
+          * a positive integer, caching is enabled only if the framecount of the image
             is less than or equal to the given number.
 
     Raises:
         TypeError: An argument is of an inappropriate type.
         ValueError: An argument is of an appropriate type but has an
           unexpected/invalid value.
         term_image.exceptions.StyleError: Invalid style-specific format specifier.
 
     * If *repeat* equals ``1``, caching is disabled.
-    * The iterator has immediate response to changes in the image size
-      and :term:`scale`.
+    * The iterator has immediate response to changes in the image size.
     * If the image size is :term:`dynamic <dynamic size>`, it's computed per frame.
     * The number of the last yielded frame is set as the image's seek position.
     * Directly adjusting the seek position of the image doesn't affect iteration.
       Use :py:meth:`ImageIterator.seek` instead.
     * After the iterator is exhausted, the underlying image is set to frame ``0``.
     """
 
@@ -2194,40 +2008,38 @@
         self,
         image: BaseImage,
         repeat: int = -1,
         format_spec: str = "",
         cached: Union[bool, int] = 100,
     ) -> None:
         if not isinstance(image, BaseImage):
-            raise TypeError(f"Invalid type for 'image' (got: {type(image).__name__})")
+            raise arg_type_error("image", image)
         if not image._is_animated:
-            raise ValueError("This image is not animated")
+            raise ValueError("'image' is not animated")
 
         if not isinstance(repeat, int):
-            raise TypeError(f"Invalid type for 'repeat' (got: {type(repeat).__name__})")
+            raise arg_type_error("repeat", repeat)
         if not repeat:
-            raise ValueError("'repeat' must be non-zero")
+            raise arg_value_error("repeat", repeat)
 
         if not isinstance(format_spec, str):
-            raise TypeError(
-                f"Invalid type for 'format_spec' (got: {type(format_spec).__name__})"
-            )
+            raise arg_type_error("format_spec", format_spec)
         *fmt, alpha, style_args = image._check_format_spec(format_spec)
 
         if not isinstance(cached, int):  # `bool` is a subclass of `int`
-            raise TypeError(f"Invalid type for 'cached' (got: {type(cached).__name__})")
+            raise arg_type_error("cached", cached)
         if False is not cached <= 0:
-            raise ValueError("'cached' must be a boolean or a positive integer")
+            raise arg_value_error_range("cached", cached)
 
         self._image = image
         self._repeat = repeat
         self._format = format_spec
-        self._cached = (
+        self._cached = repeat != 1 and (
             cached if isinstance(cached, bool) else image.n_frames <= cached
-        ) and repeat != 1
+        )
         self._loop_no = None
         self._animator = image._renderer(
             self._animate, alpha, fmt, style_args, check_size=False
         )
 
     def __del__(self) -> None:
         self.close()
@@ -2261,18 +2073,24 @@
             )
         )
 
     loop_no = property(
         lambda self: self._loop_no,
         doc="""Iteration repeat countdown
 
-        :type: int
+        :type: Optional[int]
+
+        GET:
+            Returns:
+
+            * ``None``, if iteration hasn't started.
+            * Otherwise, the current iteration repeat countdown value.
 
         Changes on the first iteration of each loop, except for infinite iteration
-        where it's always ``-1``.
+        where it's always ``-1``. When iteration has ended, the value is zero.
         """,
     )
 
     def close(self) -> None:
         """Closes the iterator and releases resources used.
 
         Does not reset the frame number of the underlying image.
@@ -2302,20 +2120,17 @@
               unexpected/invalid value.
             term_image.exceptions.TermImageError: Iteration has not yet started or the
               iterator is exhausted/closed.
 
         Frame numbers start from ``0`` (zero).
         """
         if not isinstance(pos, int):
-            raise TypeError(f"Invalid frame number type (got: {type(pos).__name__})")
+            raise arg_type_error("pos", pos)
         if not 0 <= pos < self._image.n_frames:
-            raise ValueError(
-                "Frame number out of range "
-                f"(got: {pos}, n_frames={self._image._n_frames})"
-            )
+            raise arg_value_error_range("pos", pos, f"n_frames={self._image.n_frames}")
 
         try:
             self._animator.send(pos)
         except TypeError:
             raise TermImageError("Iteration has not yet started") from None
         except AttributeError:
             raise TermImageError("Iterator exhausted or closed") from None
```

### Comparing `term-image-0.6.1/src/term_image/image/iterm2.py` & `term-image-0.7.0/src/term_image/image/iterm2.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,44 +5,113 @@
 import io
 import os
 import re
 import sys
 import warnings
 from base64 import standard_b64encode
 from operator import mul
-from threading import Event
 from typing import Any, Dict, Optional, Set, Tuple, Union
 
 import PIL
 
-from ..exceptions import TermImageWarning, _style_error
+from .. import ctlseqs
+
+# These sequences are used during performance-critical operations that occur often
+from ..ctlseqs import CURSOR_FORWARD, CURSOR_UP, ERASE_CHARS, ITERM2_START, ST
+from ..exceptions import RenderError, TermImageWarning
 from ..utils import (
-    CSI,
-    OSC,
-    ST,
     ClassInstanceProperty,
     ClassProperty,
+    arg_type_error,
+    arg_value_error_range,
     get_terminal_name_version,
-    get_terminal_size,
     write_tty,
 )
-from .common import GraphicsImage, ImageSource
-from .kitty import (
-    DELETE_ALL_IMAGES,
-    DELETE_CURSOR_IMAGES,
-    DELETE_ALL_IMAGES_b,
-    DELETE_CURSOR_IMAGES_b,
-)
+from .common import GraphicsImage, ImageMeta, ImageSource
 
 # Constants for render methods
 LINES = "lines"
 WHOLE = "whole"
+ANIM = "anim"
+
+
+class ITerm2ImageMeta(ImageMeta):
+    """Type of iterm2 render style classes."""
+
+    __native_anim_max_bytes = _native_anim_max_bytes = 2 * 2**20  # 2 MiB default
+
+    jpeg_quality = ClassInstanceProperty(
+        lambda self: getattr(self, "_jpeg_quality", -1),
+        doc="""JPEG encoding quality
+
+        See the base instance of this metaclass for the complete description.
+        """,
+    )
+
+    @jpeg_quality.setter
+    def jpeg_quality(self, quality: int) -> None:
+        if not isinstance(quality, int):
+            raise arg_type_error("jpeg_quality", quality)
+        if quality > 95:
+            raise arg_value_error_range("jpeg_quality", quality)
+
+        self._jpeg_quality = quality
+
+    @jpeg_quality.deleter
+    def jpeg_quality(self) -> None:
+        try:
+            del self._jpeg_quality
+        except AttributeError:
+            pass
+
+    native_anim_max_bytes = ClassProperty(
+        lambda self: __class__._native_anim_max_bytes,
+        doc="""Maximum size (in bytes) of image data for native animation
+
+        See the base instance of this metaclass for the complete description.
+        """,
+    )
+
+    @native_anim_max_bytes.setter
+    def native_anim_max_bytes(self, max_bytes: int):
+        if not isinstance(max_bytes, int):
+            raise arg_type_error("native_anim_max_bytes", max_bytes)
+        if max_bytes <= 0:
+            raise arg_value_error_range("native_anim_max_bytes", max_bytes)
 
+        __class__._native_anim_max_bytes = max_bytes
+
+    @native_anim_max_bytes.deleter
+    def native_anim_max_bytes(self):
+        __class__._native_anim_max_bytes = __class__.__native_anim_max_bytes
+
+    read_from_file = ClassInstanceProperty(
+        lambda self: getattr(self, "_read_from_file", True),
+        doc="""Read-from-file optimization
+
+        See the base instance of this metaclass for the complete description.
+        """,
+    )
 
-class ITerm2Image(GraphicsImage):
+    @read_from_file.setter
+    def read_from_file(self, policy: bool) -> None:
+        if not isinstance(policy, bool):
+            raise arg_type_error("read_from_file", policy)
+
+        self._read_from_file = policy
+
+    @read_from_file.deleter
+    def read_from_file(self) -> None:
+        try:
+            del self._read_from_file
+        except AttributeError:
+            pass
+
+
+class ITerm2Image(GraphicsImage, metaclass=ITerm2ImageMeta):
     """A render style using the iTerm2 inline image protocol.
 
     See :py:class:`GraphicsImage` for the complete description of the constructor.
 
     |
 
     **Render Methods**
@@ -51,39 +120,53 @@
 
     LINES (default)
        Renders an image line-by-line i.e the image is evenly split across the number
        of lines it should occupy.
 
        Pros:
 
-       * Good for use cases where it might be required to trim some lines of the
-         image.
+       * Good for use cases where it might be required to trim some lines of the image.
 
        Cons:
 
-       * Image drawing is very slow on iTerm2 due to the terminal emulator's
+       * Image drawing is significantly slower on iTerm2 due to the terminal emulator's
          performance.
 
     WHOLE
        Renders an image all at once i.e the entire image data is encoded into one
-       line of the :term:`rendered` output, such that the entire image is drawn once
+       line of the :term:`render` output, such that the entire image is drawn once
        by the terminal and still occupies the correct amount of lines and columns.
 
        Pros:
 
        * Render results are more compact (i.e less in character count) than with
          the **LINES** method since the entire image is encoded at once.
        * Image drawing is faster than with **LINES** on most terminals.
        * Smoother animations.
 
        Cons:
 
        * This method currently doesn't work well on iTerm2 and WezTerm when the image
          height is greater than the terminal height.
 
+    ANIM
+        Renders an animated image to utilize the protocol's native animation feature
+        [1]_.
+
+        Similar to the **WHOLE** render method, except that the terminal emulator
+        animates the image, provided it supports the feature of the protocol.
+        The animation is completely controled by the terminal emulator.
+
+        .. note::
+            * If the image data size (in bytes) is greater than the value of
+              :py:attr:`native_anim_max_bytes`, a warning is issued.
+            * If used with :py:class:`~term_image.image.ImageIterator` or an animation,
+              the **WHOLE** render method is used instead.
+            * If the image is non-animated, the **WHOLE** render method is used instead.
+
     NOTE:
         The **LINES** method is the default only because it works properly in all cases,
         it's more advisable to use the **WHOLE** method except when the image height is
         greater than the terminal height or when trimming the image is required.
 
     The render method can be set with
     :py:meth:`set_render_method() <BaseImage.set_render_method>` using the names
@@ -113,47 +196,29 @@
       format.
 
       * ``0`` <= *compress* <= ``9``
       * ``1`` → best speed, ``9`` → best compression, ``0`` → no compression
       * *default* → ``4``
       * Results in a trade-off between render time and data size/draw speed
 
-    * **native** (*bool*) → Native animation policy. [1]_
-
-      * ``True`` → use the protocol's native animation feature
-      * ``False`` → use the normal animation
-      * *default* → ``False``
-      * *alpha*, *repeat*, *cached* and *style* do not apply
-      * Ignored if the image is not animated or *animate* is ``False``
-      * Normal restrictions for sizing of animations do not apply
-      * Uses **WHOLE** render method
-      * The terminal emulator completely controls the animation
-
-    * **stall_native** (*bool*) → Native animation execution control.
-
-      * ``True`` → block until ``SIGINT`` (Ctrl+C) is recieved
-      * ``False`` → return as soon as the image is transmitted
-      * *default* → ``True``
-
     |
 
     **Format Specification**
 
     See :ref:`format-spec`.
 
     ::
 
         [ <method> ]  [ m <mix> ]  [ c <compress> ]
 
     * ``method`` → render method override
 
       * ``L`` → **LINES** render method (current frame only, for animated images)
       * ``W`` → **WHOLE** render method (current frame only, for animated images)
-      * ``N`` → Native animation [1]_ (ignored when used with non-animated images or
-        :py:class:`~term_image.image.ImageIterator`)
+      * ``A`` → **ANIM** render method [1]_
       * *default* → current effective render method of the instance
 
     * ``m`` → cell content inter-mix policy (**Only supported in WezTerm**, ignored
       otherwise)
 
       * ``mix`` → inter-mix policy
 
@@ -181,28 +246,29 @@
     IMPORTANT:
         Currently supported terminal emulators are:
 
         * `iTerm2 <https://iterm2.com>`_
         * `Konsole <https://konsole.kde.org>`_ >= 22.04.0
         * `WezTerm <https://wezfurlong.org/wezterm/>`_
 
+
     .. [1] Native animation support:
 
        * Not all animated image formats may be supported by every supported terminal
          emulator
        * Not all supported terminal emulators implement this feature of the protocol
          e.g on Konsole, the first frame is drawn but the image is not animated
 
     |
     """
 
     _FORMAT_SPEC: Tuple[re.Pattern] = tuple(
-        map(re.compile, "[LWN] m[01] c[0-9]".split(" "))
+        map(re.compile, "[LWA] m[01] c[0-9]".split(" "))
     )
-    _render_methods: Set[str] = {LINES, WHOLE}
+    _render_methods: Set[str] = {LINES, WHOLE, ANIM}
     _default_render_method: str = LINES
     _render_method: str = LINES
     _style_args = {
         "method": (
             None,
             (
                 lambda x: isinstance(x, str),
@@ -228,45 +294,30 @@
                 "Compression level must be an integer",
             ),
             (
                 lambda x: 0 <= x <= 9,
                 "Compression level must be between 0 and 9, both inclusive",
             ),
         ),
-        "native": (
-            False,
-            (
-                lambda x: isinstance(x, bool),
-                "Native animation policy must be a boolean",
-            ),
-            (lambda _: True, ""),
-        ),
-        "stall_native": (
-            True,
-            (
-                lambda x: isinstance(x, bool),
-                "Native animation execution policy must be a boolean",
-            ),
-            (lambda _: True, ""),
-        ),
     }
 
     _TERM: str = ""
     _TERM_VERSION: str = ""
 
     jpeg_quality = ClassInstanceProperty(
-        lambda self_or_cls: getattr(self_or_cls, "_jpeg_quality", -1),
-        doc="""
-        JPEG encoding quality
+        ITerm2ImageMeta.jpeg_quality.fget,
+        ITerm2ImageMeta.jpeg_quality.fset,
+        ITerm2ImageMeta.jpeg_quality.fdel,
+        doc="""JPEG encoding quality
 
         :type: int
 
         GET:
             Returns the effective JPEG encoding quality of the invoker
-            (negative if disabled).
+            (class or instance).
 
         SET:
             If invoked via:
 
             * a **class**, the **class-wide** quality is set.
             * an **instance**, the **instance-specific** quality is set.
 
@@ -282,17 +333,17 @@
         * ``0`` <= *value* <= ``95``; JPEG encoding is enabled with the given quality.
 
         If **unset** for:
 
         * a **class**, it uses that of its parent *iterm2* style class (if any) or the
           default (disabled), if unset for all parents or the class has no parent
           *iterm2* style class.
-        * an **instance**, it uses that of it's class.
+        * an **instance**, it uses that of its class.
 
-        By **default**, the quality is **unset** i.e JPEG encoding is **disabled** and
+        By **default**, the quality is **unset** (i.e JPEG encoding is **disabled**) and
         images are encoded in the PNG format (when not reading directly from file) but
         in some cases, higher and/or faster compression may be desired.
         JPEG encoding is significantly faster than PNG encoding and produces smaller
         (in data size) output but **at the cost of image quality**.
 
         NOTE:
             * This property is :term:`descendant`.
@@ -312,92 +363,58 @@
         SEE ALSO:
             * the *alpha* parameter of :py:meth:`~term_image.image.BaseImage.draw`
               and the ``#``, ``bgcolor`` fields of the :ref:`format-spec`
             * :py:attr:`read_from_file`
         """,
     )
 
-    @jpeg_quality.setter
-    def jpeg_quality(self_or_cls, quality: int) -> None:
-        if not isinstance(quality, int):
-            raise TypeError(
-                f"Invalid type for 'quality' (got: {type(quality).__name__})"
-            )
-        if quality > 95:
-            raise ValueError(f"'quality' out of range (got: {quality})")
-
-        self_or_cls._jpeg_quality = quality
-
-    @jpeg_quality.deleter
-    def jpeg_quality(self_or_cls) -> None:
-        try:
-            del self_or_cls._jpeg_quality
-        except AttributeError:
-            pass
-
     native_anim_max_bytes = ClassProperty(
-        # 2 MiB default
-        lambda cls: getattr(__class__, "_native_anim_max_bytes", 2 * 2**20),
-        doc="""
-        Maximum size (in bytes) of image data for native animation
+        lambda self: type(self)._native_anim_max_bytes,
+        doc="""Maximum size (in bytes) of image data for native animation
 
         :type: int
 
         GET:
             Returns the set value.
 
         SET:
-            A positive integer; the value is set on the *iterm2* render style baseclass
-            (:py:class:`ITerm2Image`).
+            A positive integer; the value is set.
+
+            Can not be set via an instance.
 
         DELETE:
-            The value is unset, thereby resetting it to the default.
+            The value is reset to the default.
+
+            Can not be reset via an instance.
 
         :py:class:`~term_image.exceptions.TermImageWarning` is issued (and shown
-        **only the first time**, except a filter is set to do otherwise) if the
-        image data size for a native animation is above this value.
+        **only the first time**, except the warning filters are modified to do
+        otherwise) if the image data size for a native animation is above this value.
 
         NOTE:
-            This property is :term:`descendant` but is always unset for all subclasses
-            and instances. Hence, setting/resetting it on this class, a subclass or an
-            instance affects this class, all its subclasses and all their instances.
+            This property is a global setting. Hence, setting/resetting it on this
+            class or any subclass affects all classes and their instances.
 
         WARNING:
             This property should be altered with caution to avoid excessive memory
-            usage.
+            usage, particularly on the terminal emulator's end.
         """,
     )
 
-    @native_anim_max_bytes.setter
-    def native_anim_max_bytes(cls, max_bytes: int):
-        if not isinstance(max_bytes, int):
-            raise TypeError(
-                f"Invalid type for 'max_bytes' (got: {type(max_bytes).__name__})"
-            )
-        if max_bytes <= 0:
-            raise ValueError(f"'max_bytes' out of range (got: {max_bytes})")
-
-        __class__._native_anim_max_bytes = max_bytes
-
-    @native_anim_max_bytes.deleter
-    def native_anim_max_bytes(cls):
-        try:
-            del __class__._native_anim_max_bytes
-        except AttributeError:
-            pass
-
     read_from_file = ClassInstanceProperty(
-        lambda self_or_cls: getattr(self_or_cls, "_read_from_file", True),
-        doc="""
-        Read-from-file optimization policy
+        ITerm2ImageMeta.read_from_file.fget,
+        ITerm2ImageMeta.read_from_file.fset,
+        ITerm2ImageMeta.read_from_file.fdel,
+        doc="""Read-from-file optimization
 
         :type: bool
 
         GET:
-            Returns the effective read-from-file policy of the invoker.
+            Returns the effective read-from-file policy of the invoker
+            (class or instance).
 
         SET:
             If invoked via:
 
             * a **class**, the **class-wide** policy is set.
             * an **instance**, the **instance-specific** policy is set.
 
@@ -414,15 +431,15 @@
         * ``False``, images are always re-encoded (in the PNG format by default).
 
         If **unset** for:
 
         * a **class**, it uses that of its parent *iterm2* style class (if any) or the
           default (``True``), if unset for all parents or the class has no parent
           *iterm2* style class.
-        * an **instance**, it uses that of it's class.
+        * an **instance**, it uses that of its class.
 
         By **default**, the policy is **unset**, which is equivalent to ``True``
         i.e the optimization is **enabled**.
 
         NOTE:
             * This property is :term:`descendant`.
             * This is an optimization to reduce render times and is only applicable to
@@ -433,65 +450,45 @@
               to be re-encoded.
 
         SEE ALSO:
             :py:attr:`jpeg_quality`
         """,
     )
 
-    @read_from_file.setter
-    def read_from_file(self_or_cls, policy: bool) -> None:
-        if not isinstance(policy, bool):
-            raise TypeError(f"Invalid type for 'policy' (got: {type(policy).__name__})")
-
-        self_or_cls._read_from_file = policy
-
-    @read_from_file.deleter
-    def read_from_file(self_or_cls) -> None:
-        try:
-            del self_or_cls._read_from_file
-        except AttributeError:
-            pass
-
     @classmethod
     def clear(cls, cursor: bool = False, now: bool = False) -> None:
         """Clears images.
 
         Args:
             cursor: If ``True``, all images intersecting with the current cursor
               position are cleared. Otherwise, all visible images are cleared.
             now: If ``True`` the images are cleared immediately, without affecting
               any standard I/O stream.
               Otherwise they're cleared when next :py:data:`sys.stdout` is flushed.
 
         NOTE:
             Required and works only on Konsole, as text doesn't overwrite images.
         """
+        if not isinstance(cursor, bool):
+            raise arg_type_error("cursor", cursor)
+        if not isinstance(now, bool):
+            raise arg_type_error("now", now)
+
         # There's no point checking for forced support since this is only required on
         # konsole which supports the protocol.
         # `is_supported()` is first called to ensure `_TERM` has been set.
         if cls.is_supported() and cls._TERM == "konsole":
             # Konsole utilizes the same image rendering implementation as it
             # uses for the kiity graphics protocol.
             (write_tty if now else _stdout_write)(
-                (DELETE_CURSOR_IMAGES_b if now else DELETE_CURSOR_IMAGES)
+                (ctlseqs.KITTY_DELETE_CURSOR_b if now else ctlseqs.KITTY_DELETE_CURSOR)
                 if cursor
-                else (DELETE_ALL_IMAGES_b if now else DELETE_ALL_IMAGES)
+                else (ctlseqs.KITTY_DELETE_ALL_b if now else ctlseqs.KITTY_DELETE_ALL)
             )
 
-    def draw(self, *args, **kwargs):
-        # Ignore (and omit) native animation arguments for non-animations
-        if not (self._is_animated and kwargs.get("animate", True)):
-            for arg_name in ("native", "stall_native"):
-                try:
-                    del kwargs[arg_name]
-                except KeyError:
-                    pass
-
-        super().draw(*args, **kwargs)
-
     @classmethod
     def is_supported(cls):
         if cls._supported is None:
             cls._supported = False
 
             name, version = get_terminal_name_version()
             if name in {"iterm2", "konsole", "wezterm"}:
@@ -508,127 +505,123 @@
 
     @classmethod
     def _check_style_format_spec(cls, spec: str, original: str) -> Dict[str, Any]:
         parent, (method, mix, compress) = cls._get_style_format_spec(spec, original)
         args = {}
         if parent:
             args.update(super()._check_style_format_spec(parent, original))
-        if method == "N":
-            args["native"] = True
-        elif method:
-            args["method"] = LINES if method == "L" else WHOLE
+        if method:
+            args["method"] = {"L": LINES, "W": WHOLE, "A": ANIM}[method]
         if mix:
             args["mix"] = bool(int(mix[-1]))
         if compress:
             args["compress"] = int(compress[-1])
 
         return cls._check_style_args(args)
 
     def _display_animated(
         self,
         img,
         alpha,
         fmt,
         *args,
         mix: bool = False,
-        native: bool = False,
-        stall_native: bool = True,
         **kwargs,
     ):
-        if native:
-            try:
-                print(
-                    self._format_render(
-                        self._render_image(img, alpha, mix=mix, native=True),
-                        *fmt,
-                    ),
-                    end="",
-                    flush=True,
-                )
-            except (KeyboardInterrupt, Exception):
-                self._handle_interrupted_draw()
-                raise
-            else:
-                stall_native and native_anim.wait()
-        else:
-            if not mix and self._TERM == "wezterm":
-                lines = max(
-                    (fmt or (None,))[-1] or get_terminal_size()[1] - self._v_allow,
-                    self.rendered_height,
-                )
-                r_width = self.rendered_width
-                erase_and_jump = f"{CSI}{r_width}X{CSI}{r_width}C"
-                first_frame = self._format_render(
-                    f"{erase_and_jump}\n" * (lines - 1) + f"{erase_and_jump}", *fmt
-                )
-                print(first_frame, f"\r{CSI}{lines - 1}A", sep="", end="", flush=True)
+        if not mix and self._TERM == "wezterm":
+            lines = max(fmt[-1], self.rendered_height)
+            r_width = self.rendered_width
+            erase_and_move_cursor = ERASE_CHARS % r_width + CURSOR_FORWARD % r_width
+            first_frame = self._format_render(
+                f"{erase_and_move_cursor}\n" * (lines - 1) + erase_and_move_cursor,
+                *fmt,
+            )
+            print(
+                first_frame,
+                "\r",
+                CURSOR_UP % (lines - 1),
+                sep="",
+                end="",
+                flush=True,
+            )
 
-            super()._display_animated(img, alpha, fmt, *args, mix=True, **kwargs)
+        super()._display_animated(img, alpha, fmt, *args, mix=True, **kwargs)
 
     @staticmethod
     def _handle_interrupted_draw():
         """Performs neccessary actions when image drawing is interrupted.
 
         If drawing is interruped while transmiting an image, it causes terminal to
         wait for more data (while consuming any output following) until the output
         reaches the expected payload size or ST (String Terminator) is written.
         """
 
         # End last transmission (does no harm if there wasn't an unterminated
         # transmission)
         # Konsole sometimes requires ST to be written twice.
-        print(f"{ST * 2}", end="", flush=True)
+        print(ctlseqs.ST * 2, end="", flush=True)
 
     def _render_image(
         self,
         img: PIL.Image.Image,
         alpha: Union[None, float, str],
         *,
         frame: bool = False,
         method: Optional[str] = None,
         mix: bool = False,
         compress: int = 4,
-        native: bool = False,
     ) -> str:
+        # NOTE: It's more efficient to write separate strings to the buffer separately
+        # than concatenate and write together.
+
         # Using `width=<columns>`, `height=<lines>` and `preserveAspectRatio=0` ensures
         # that an image always occupies the correct amount of columns and lines even if
         # the cell size has changed when it's drawn.
         # Since we use `width` and `height` control data keys, there's no need
-        # upscaling an image on this end; ensures minimal payload.
+        # upscaling the image on this end to reduce payload.
+        # Anyways, this also implies that the image(s) have to be resized by the
+        # terminal emulator, thereby leaving various details of resizing in the hands
+        # of the terminal emulator such as the resampling method, etc.
+        # This particularly affects the LINES render method negatively, resulting in
+        # slant/curved edges not lining up across lines (amongst other artifacts
+        # observed on Konsole) supposedly because the terminal emulator resizes each
+        # line separately.
+        # Hence, this optimization is only used for the WHOLE render method.
 
         r_width, r_height = self.rendered_size
+        render_method = (method or self._render_method).lower()
 
         # Workarounds
         is_on_konsole = self._TERM == "konsole"
         is_on_wezterm = self._TERM == "wezterm"
-        jump_right = f"{CSI}{r_width}C"
-        jump_up = f"{CSI}{r_height - 1}A" if r_height > 1 else ""
-        erase = f"{CSI}{r_width}X" if not mix and is_on_wezterm else ""
+        cursor_right = CURSOR_FORWARD % r_width
+        cursor_up = CURSOR_UP % (r_height - 1) if r_height > 1 else ""
+        erase = ERASE_CHARS % r_width if not mix and is_on_wezterm else ""
 
         file_is_readable = True
         if self._source_type is ImageSource.PIL_IMAGE:
             try:
                 file_is_readable = os.access(img.filename, os.R_OK)
             except (AttributeError, OSError):
                 file_is_readable = False
 
-        if native and self._is_animated and not frame:
+        if render_method == ANIM and self._is_animated and not frame:
             if self._source_type is ImageSource.PIL_IMAGE:
                 if file_is_readable:
                     compressed_image = open(img.filename, "rb")
                 else:
                     compressed_image = io.BytesIO()
                     try:
                         img.save(compressed_image, img.format, save_all=True)
-                    except ValueError:
+                    except ValueError as e:
                         self._close_image(img)
-                        raise _style_error(type(self))(
-                            "Native animation not supported: This image was sourced "
-                            "from a PIL image of an unknown format"
-                        ) from None
+                        raise RenderError(
+                            "iTerm2 native animation not supported: This image was "
+                            "sourced from a PIL image with an unknown format"
+                        ) from e
             else:
                 compressed_image = open(self._source, "rb")
 
             self._close_image(img)
 
             with compressed_image:
                 compressed_image.seek(0, 2)
@@ -647,29 +640,32 @@
                 )
                 compressed_image.seek(0)
                 return "".join(
                     (
                         (
                             ""
                             if is_on_konsole
-                            else f"{erase}{jump_right}\n" * (r_height - 1)
+                            else f"{erase}{cursor_right}\n" * (r_height - 1)
                         ),
                         erase,
-                        "" if is_on_konsole else jump_up,
-                        START,
+                        "" if is_on_konsole else cursor_up,
+                        ITERM2_START,
                         control_data,
                         standard_b64encode(compressed_image.read()).decode(),
                         ST,
-                        f"{jump_right}\n" * (r_height - 1) if is_on_konsole else "",
-                        jump_right * is_on_konsole,
+                        f"{cursor_right}\n" * (r_height - 1) if is_on_konsole else "",
+                        cursor_right * is_on_konsole,
                     )
                 )
 
-        render_method = (method or self._render_method).lower()
-        width, height = self._get_minimal_render_size(adjust=render_method == LINES)
+        width, height = (
+            self._get_minimal_render_size()
+            if render_method == WHOLE
+            else self._get_render_size()
+        )
 
         if (  # Read directly from file when possible and reasonable
             self.read_from_file
             and not self._is_animated
             and file_is_readable
             and render_method == WHOLE
             and mul(*self._original_size) <= mul(*self._get_render_size())
@@ -739,21 +735,22 @@
                             format,
                             compress_level=compress,  # PNG
                             quality=jpeg_quality,
                         )
                     compressed_image.truncate()
 
                     buffer.write(erase)
-                    buffer.write(f"{START}size={compressed_image.tell()}")
+                    buffer.write(ITERM2_START)
+                    buffer.write(f"size={compressed_image.tell()}")
                     buffer.write(control_data)
                     buffer.write(
                         standard_b64encode(compressed_image.getvalue()).decode()
                     )
                     buffer.write(ST)
-                    is_on_konsole and buffer.write(jump_right)
+                    is_on_konsole and buffer.write(cursor_right)
                     line < r_height and buffer.write("\n")
 
                 return buffer.getvalue()
 
         # WHOLE
         with compressed_image:
             compressed_image.seek(0, 2)
@@ -763,23 +760,25 @@
                     f";height={r_height};preserveAspectRatio=0;inline=1"
                     f"{';doNotMoveCursor=1' * is_on_konsole}:"
                 )
             )
             compressed_image.seek(0)
             return "".join(
                 (
-                    "" if is_on_konsole else f"{erase}{jump_right}\n" * (r_height - 1),
+                    (
+                        ""
+                        if is_on_konsole
+                        else f"{erase}{cursor_right}\n" * (r_height - 1)
+                    ),
                     erase,
-                    "" if is_on_konsole else jump_up,
-                    START,
+                    "" if is_on_konsole else cursor_up,
+                    ITERM2_START,
                     control_data,
                     standard_b64encode(compressed_image.read()).decode(),
                     ST,
-                    f"{jump_right}\n" * (r_height - 1) if is_on_konsole else "",
-                    jump_right * is_on_konsole,
+                    f"{cursor_right}\n" * (r_height - 1) if is_on_konsole else "",
+                    cursor_right * is_on_konsole,
                 )
             )
 
 
-START = f"{OSC}1337;File="
-native_anim = Event()
 _stdout_write = sys.stdout.write
```

### Comparing `term-image-0.6.1/src/term_image/image/kitty.py` & `term-image-0.7.0/src/term_image/image/kitty.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,31 @@
 from base64 import standard_b64encode
 from dataclasses import asdict, dataclass
 from typing import Any, Dict, Generator, Optional, Set, Tuple, Union
 from zlib import compress, decompress
 
 import PIL
 
-from ..utils import CSI, ESC, ST, get_terminal_name_version, query_terminal, write_tty
+from .. import ctlseqs
+
+# These sequences are used during performance-critical operations that occur often
+from ..ctlseqs import (
+    CURSOR_FORWARD,
+    ERASE_CHARS,
+    KITTY_DELETE_CURSOR,
+    KITTY_TRANSMISSION,
+)
+from ..utils import (
+    arg_type_error,
+    arg_value_error_msg,
+    arg_value_error_range,
+    get_terminal_name_version,
+    query_terminal,
+    write_tty,
+)
 from .common import GraphicsImage
 
 # Constants for render methods
 LINES = "lines"
 WHOLE = "whole"
 
 
@@ -234,76 +250,75 @@
         NOTE:
             This method does nothing if the render style is not supported.
         """
         if not (cls._forced_support or cls.is_supported()):
             return
 
         if not isinstance(cursor, bool):
-            raise TypeError(f"Invalid type for 'cursor' (got: {type(cursor).__name__})")
+            raise arg_type_error("cursor", cursor)
 
         if z_index is not None:
             if not isinstance(z_index, int):
-                raise TypeError(
-                    f"Invalid type for 'z_index' (got: {type(z_index).__name__})"
-                )
+                raise arg_type_error("z_index", z_index)
             if not -(1 << 31) <= z_index < (1 << 31):
-                raise ValueError(
-                    "z-index must be within the 32-bit signed integer range "
-                    f"(got: {z_index})"
-                )
+                raise arg_value_error_range("z_index", z_index)
 
         if not isinstance(now, bool):
-            raise TypeError(f"Invalid type for 'now' (got: {type(now).__name__})")
+            raise arg_type_error("now", now)
 
         default_args = __class__.clear.__func__.__kwdefaults__
         nonlocals = locals()
         args = {name: nonlocals[name] for name in default_args}
         given_args = args.items() - (default_args.items() | {("now", True)})
 
         if len(given_args) > 1:
-            raise ValueError("Only one argument may be given")
+            raise arg_value_error_msg(
+                "Only one argument (aside 'now') may be given", len(given_args)
+            )
         elif given_args:
             arg, _ = given_args.pop()
             (write_tty if now else _stdout_write)(
-                (DELETE_CURSOR_IMAGES_b if now else DELETE_CURSOR_IMAGES)
+                (ctlseqs.KITTY_DELETE_CURSOR_b if now else ctlseqs.KITTY_DELETE_CURSOR)
                 if arg == "cursor"
                 else (
-                    (DELETE_Z_INDEX_IMAGES_b if now else DELETE_Z_INDEX_IMAGES)
+                    (
+                        ctlseqs.KITTY_DELETE_Z_INDEX_b
+                        if now
+                        else ctlseqs.KITTY_DELETE_Z_INDEX
+                    )
                     % z_index
                 )
             )
         elif now:
-            write_tty(DELETE_ALL_IMAGES_b)
+            write_tty(ctlseqs.KITTY_DELETE_ALL_b)
         else:
-            _stdout_write(DELETE_ALL_IMAGES)
+            _stdout_write(ctlseqs.KITTY_DELETE_ALL)
 
     @classmethod
     def is_supported(cls) -> bool:
         if cls._supported is None:
             cls._supported = False
 
             # The graphics query for support detection messes up iTerm2's window title
             if get_terminal_name_version()[0] == "iterm2":
                 return False
 
             # Kitty graphics query + terminal attribute query
             # The second query is to speed up the query since most (if not all)
             # terminals should support it and most terminals treat queries as FIFO
             response = query_terminal(
-                (
-                    f"{START}a=q,t=d,i=31,f=24,s=1,v=1,C=1,c=1,r=1;AAAA{ST}{CSI}c"
-                ).encode(),
+                ctlseqs.KITTY_SUPPORT_QUERY_b + ctlseqs.DA1_b,
                 lambda s: not s.endswith(b"c"),
             )
 
             # Not supported if it doesn't respond to either query
             # or responds to the second but not the first
-            if response and (
-                response.decode().rpartition(ESC)[0] == f"{START}i=31;OK{ST}"
-            ):
+            if response:
+                response = ctlseqs.KITTY_RESPONSE_re.match(response.decode())
+            if response and response["id"] == "31" and response["message"] == "OK":
                 name, version = get_terminal_name_version()
                 # Only kitty >= 0.20.0 implement the protocol features utilized
                 if name == "kitty" and version:
                     try:
                         version_tuple = tuple(map(int, version.split(".")))
                     except ValueError:  # Version string not "understood"
                         pass
@@ -371,18 +386,18 @@
         is written.
 
         Also, if the image data was chunked, it would be expecting the last chunk.
         In this case, output is not consumed but the next graphics command sent
         might not be treated as expected on some terminals e.g Konsole.
         """
 
-        # End last command (does no harm if there wasn't an unterminated commanand)
+        # End last command (does no harm if there wasn't an unterminated command)
         # and send "last chunk" in case the last transmission was chunked.
         # Konsole sometimes requires ST to be written twice.
-        print(f"{ST * 2}{START}q=1,m=0;{ST}", end="", flush=True)
+        print(ctlseqs.ST * 2 + ctlseqs.KITTY_END_CHUNKED, end="", flush=True)
 
     def _render_image(
         self,
         img: PIL.Image.Image,
         alpha: Union[None, float, str],
         *,
         frame: bool = False,
@@ -402,72 +417,78 @@
         """
         # NOTE: It's more efficient to write separate strings to the buffer separately
         # than concatenate and write together.
 
         # Using `c` and `r` ensures that an image always occupies the correct amount
         # of columns and lines even if the cell size has changed when it's drawn.
         # Since we use `c` and `r` control data keys, there's no need upscaling the
-        # image on this end; ensures minimal payload.
+        # image on this end to reduce payload.
+        # Anyways, this also implies that the image(s) have to be resized by the
+        # terminal emulator, thereby leaving various details of resizing in the hands
+        # of the terminal emulator such as the resampling method, etc.
+        # This particularly affects the LINES render method negatively, resulting in
+        # slant/curved edges not lining up across lines (amongst other artifacts
+        # observed on Konsole) supposedly because the terminal emulator resizes each
+        # line separately.
+        # Hence, this optimization is only used for the WHOLE render method.
 
         render_method = (method or self._render_method).lower()
         r_width, r_height = self.rendered_size
-        width, height = self._get_minimal_render_size(adjust=render_method == LINES)
+        width, height = (
+            self._get_minimal_render_size()
+            if render_method == WHOLE
+            else self._get_render_size()
+        )
 
         frame_img = img if frame else None
         img = self._get_render_data(
             img, alpha, size=(width, height), pixel_data=False, frame=frame  # fmt: skip
         )[0]
         format = getattr(f, img.mode)
         raw_image = img.tobytes()
 
         # clean up (ImageIterator uses one PIL image throughout)
         if frame_img is not img:
             self._close_image(img)
 
         control_data = ControlData(f=format, s=width, c=r_width, z=z_index)
-        erase = "" if mix else f"{CSI}{r_width}X"
-        jump_right = f"{CSI}{r_width}C"
-        if not blend:
-            delete = f"{START}a=d,d=C;{ST}"
+        fill = ("" if mix else ERASE_CHARS % r_width) + (CURSOR_FORWARD % r_width)
+        fill_newline = fill + "\n"
 
         if render_method == LINES:
             cell_height = height // r_height
             bytes_per_line = width * cell_height * (format // 8)
             vars(control_data).update(dict(v=cell_height, r=1))
 
             with io.StringIO() as buffer, io.BytesIO(raw_image) as raw_image:
                 trans = Transmission(
                     control_data, raw_image.read(bytes_per_line), compress
                 )
-                blend or buffer.write(delete)
+                blend or buffer.write(KITTY_DELETE_CURSOR)
                 for chunk in trans.get_chunks():
                     buffer.write(chunk)
-                # Writing spaces clears any text under transparent areas of an image
                 for _ in range(r_height - 1):
-                    buffer.write(erase)
-                    buffer.write(jump_right)
-                    buffer.write("\n")
+                    buffer.write(fill_newline)
                     trans = Transmission(
                         control_data, raw_image.read(bytes_per_line), compress
                     )
-                    blend or buffer.write(delete)
+                    blend or buffer.write(KITTY_DELETE_CURSOR)
                     for chunk in trans.get_chunks():
                         buffer.write(chunk)
-                buffer.write(erase)
-                buffer.write(jump_right)
+                buffer.write(fill)
 
                 return buffer.getvalue()
 
         vars(control_data).update(v=height, r=r_height)
         return "".join(
             (
-                ("" if blend else delete),
+                KITTY_DELETE_CURSOR * (not blend),
                 Transmission(control_data, raw_image, compress).get_chunked(),
-                f"{erase}{jump_right}\n" * (r_height - 1),
-                f"{erase}{jump_right}",
+                fill_newline * (r_height - 1),
+                fill,
             )
         )
 
 
 @dataclass
 class Transmission:
     """An abstraction of the kitty terminal graphics escape code.
@@ -511,24 +532,25 @@
     def get_chunked(self) -> str:
         return "".join(self.get_chunks())
 
     def get_chunks(self, size: int = 4096) -> Generator[str, None, None]:
         with self.get_payload() as payload:
             chunk, next_chunk = payload.read(size), payload.read(size)
             yield (
-                f"{START}{self.get_control_data()},m={bool(next_chunk):d};{chunk}{ST}"
+                KITTY_TRANSMISSION
+                % (f"{self.get_control_data()},m={bool(next_chunk):d}", chunk)
             )
 
             chunk, next_chunk = next_chunk, payload.read(size)
             while next_chunk:
-                yield f"{START}m=1;{chunk}{ST}"
+                yield KITTY_TRANSMISSION % ("m=1", chunk)
                 chunk, next_chunk = next_chunk, payload.read(size)
 
             if chunk:  # false if there was never a next chunk
-                yield f"{START}m=0;{chunk}{ST}"
+                yield KITTY_TRANSMISSION % ("m=0", chunk)
 
     def get_control_data(self) -> str:
         return ",".join(
             f"{key}={value}"
             for key, value in asdict(self.control).items()
             if value is not None
         )
@@ -619,16 +641,8 @@
     x: Optional[int] = None
     y: Optional[int] = None
     # # crop rectangle size
     w: Optional[int] = None
     h: Optional[int] = None
 
 
-START = f"{ESC}_G"
-FMT = f"{START}%(control)s;%(payload)s{ST}"
-DELETE_ALL_IMAGES = f"{ESC}_Ga=d,d=A;{ST}"
-DELETE_ALL_IMAGES_b = DELETE_ALL_IMAGES.encode()
-DELETE_CURSOR_IMAGES = f"{ESC}_Ga=d,d=C;{ST}"
-DELETE_CURSOR_IMAGES_b = DELETE_CURSOR_IMAGES.encode()
-DELETE_Z_INDEX_IMAGES = f"{ESC}_Ga=d,d=Z,z=%d;{ST}"
-DELETE_Z_INDEX_IMAGES_b = DELETE_Z_INDEX_IMAGES.encode()
 _stdout_write = sys.stdout.write
```

### Comparing `term-image-0.6.1/src/term_image/utils.py` & `term-image-0.7.0/src/term_image/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 """
 .. Utilities
 """
 
 from __future__ import annotations
 
 __all__ = (
+    "get_cell_size",
     "get_terminal_name_version",
     "get_terminal_size",
     "lock_tty",
     "read_tty_all",
     "write_tty",
 )
 
 import os
-import re
 import sys
 import warnings
 from array import array
 from functools import wraps
 from multiprocessing import Array, Process, Queue as mp_Queue, RLock as mp_RLock
 from operator import floordiv
 from queue import Empty, Queue
 from shutil import get_terminal_size as _get_terminal_size
 from threading import RLock
 from time import monotonic
 from types import FunctionType
-from typing import Callable, Optional, Tuple, Union
+from typing import Any, Callable, Optional, Tuple, Union
 
+from . import ctlseqs
 from .exceptions import TermImageWarning
 
 # import logging
 
 OS_IS_UNIX: bool
 try:
     import fcntl
@@ -48,107 +49,63 @@
 
 
 class ClassInstanceMethod(classmethod):
     """A method which when invoked via the owner, behaves like a class method
     and when invoked via an instance, behaves like an instance method.
     """
 
+    def __init__(
+        self, f_owner: FunctionType, f_instance: Optional[FunctionType] = None
+    ):
+        super().__init__(f_owner)
+        self.f_owner = f_owner
+        self.f_instance = f_instance
+
     def __get__(self, instance, owner=None):
-        # classmethod just uses `owner` directly if given.
-        # Otherwise, type(instance) but we're not concerned with this.
-        return super().__get__(None, instance or owner)
+        if instance:
+            return self.f_instance.__get__(instance, owner)
+        else:
+            return super().__get__(instance, owner)
 
+    def classmethod(self, function: FunctionType) -> ClassInstanceMethod:
+        return type(self)(function, self.f_instance)
 
-class ClassPropertyBase(property):
-    """Base class for properties that operate on their **owner**.
+    def instancemethod(self, function: FunctionType) -> ClassInstanceMethod:
+        return type(self)(self.f_owner, function)
 
-    NOTE:
-        For ``__set__()`` and ``__delete__()`` to actually work, the metaclass of the
-        owner must be made to recognize and directly call these methods within it's
-        ``__setattr__()`` and ``__delattr__()``.
-
-        If the owner defines (not inherits) a ``_class_properties_`` attribute, it must
-        be a :py:class:``dict`` and is populated with the names (as in the owner's
-        namespace) of all instances of this class (i.e class properties) mapped to the
-        respective instances.
 
-        For this reason, :py:class:`ClassPropertyMeta` is provided.
+class ClassPropertyBase(property):
+    """Base class for owner properties that also have a counterpart/shadow on the
+    instance.
     """
 
     def __init__(self, fget=None, fset=None, fdel=None, doc=None):
         super().__init__(fget, fset, fdel, doc)
-        # `property` doesn't set `__doc__`, probably cos this class' `__doc__`
+        # `property` doesn't set `__doc__`, probably cos the subclass' `__doc__`
         # attribute overrides its `__doc__` descriptor.
-        super().__setattr__("__doc__", doc)
-
-    def __set_name__(self, owner, name):
-        self.__objclass__ = owner
-        try:
-            class_properties = owner.__dict__["_class_properties_"]
-        except KeyError:
-            pass
-        else:
-            class_properties[name] = self
+        super().__setattr__("__doc__", doc or fget.__doc__)
 
 
 class ClassInstanceProperty(ClassPropertyBase):
-    """A property which operates on the invoker, be it the owner or an instance."""
+    """A an instance-specific counterpart of a property of the owner.
 
-    def __get__(self, instance, owner=None):
-        return super().__get__(instance or owner, owner)
-
-
-class ClassProperty(ClassPropertyBase):
-    """A property which always operates on the owner, even when invoked by an
-    instance.
+    Operation on the owner is actually implemented by a property defined on the
+    owner's metaclass. This class is only for the sake of ease of documentation
+    without having to bother the user about metaclasses.
     """
 
-    def __get__(self, instance, owner=None):
-        return super().__get__(owner, owner)
-
-    def __set__(self, obj, value):
-        super().__set__(type(obj) if isinstance(obj, self.__objclass__) else obj, value)
-
-    def __delete__(self, obj):
-        super().__delete__(type(obj) if isinstance(obj, self.__objclass__) else obj)
 
+class ClassProperty(ClassPropertyBase):
+    """A read-only shadow of a property of the owner.
 
-class ClassPropertyMeta(type):
-    """A metaclass that implements support for modifiable class properties owned by
-    its instances.
-
-    - Takes care of inherited class properties.
-    - Works with both cooperative multiple ane multi-level inheritance.
-
-    SEE ALSO:
-        :py:class:`ClassPropertyBase`
+    Operation on the owner is actually implemented by a property defined on the
+    owner's metaclass. This class is only for the sake of ease of documentation
+    without having to bother the user about metaclasses.
     """
 
-    def __new__(cls, name, bases, dict, **kwds):
-        class_properties = dict["_class_properties_"] = {}
-        for base in bases:
-            if isinstance(base, __class__):
-                class_properties.update(base._class_properties_)
-
-        return super().__new__(cls, name, bases, dict, **kwds)
-
-    def __setattr__(self, name, value):
-        class_property = self._class_properties_.get(name)
-        if class_property:
-            class_property.__set__(self, value)
-        else:
-            super().__setattr__(name, value)
-
-    def __delattr__(self, name):
-        class_property = self._class_properties_.get(name)
-        if class_property:
-            class_property.__delete__(self)
-        else:
-            super().__delattr__(name)
-
 
 # Decorator Functions
 
 
 def no_redecorate(decor: FunctionType) -> FunctionType:
     """Prevents a decorator from re-decorating objects.
 
@@ -305,28 +262,48 @@
 
     Args:
         func: The function to be wrapped.
     """
 
     @wraps(func)
     def unix_only_wrapper(*args, **kwargs):
-        return _tty and func(*args, **kwargs)
+        return _tty_fd and func(*args, **kwargs)
 
     unix_only_wrapper.__doc__ += """
     NOTE:
         Currently works on UNIX only, returns ``None`` on any other platform or when
         there is no :term:`active terminal`.
     """
 
     return unix_only_wrapper
 
 
 # Non-decorators
 
 
+def arg_type_error(arg: str, value: Any) -> TypeError:
+    return TypeError(f"Invalid type for {arg!r} (got: {type(value).__name__})")
+
+
+def arg_value_error(arg: str, value: Any) -> ValueError:
+    return ValueError(f"Invalid value for {arg!r} (got: {value!r})")
+
+
+def arg_value_error_msg(msg: str, value: Any) -> ValueError:
+    return ValueError(f"{msg!r} (got: {value!r})")
+
+
+def arg_value_error_range(arg: str, value: Any, got_extra: str = "") -> ValueError:
+    return ValueError(
+        f"{arg!r} out of range (got: {value!r}, {got_extra})"
+        if got_extra
+        else f"{arg!r} out of range (got: {value!r})"
+    )
+
+
 def clear_queue(queue: Union[Queue, mp_Queue]):
     """Purges the given queue"""
     while True:
         try:
             queue.get(timeout=0.005)
         except Empty:
             break
@@ -345,33 +322,90 @@
         end: If ``True``, the color reset sequence is appended to the returned string.
 
     Returns:
         The color-coded string.
 
     The color code is ommited for any of *fg* or *bg* that is empty.
     """
-    return (FG_FMT * bool(fg) + BG_FMT * bool(bg) + "%s") % (
+    return (ctlseqs.SGR_FG_RGB * bool(fg) + ctlseqs.SGR_BG_RGB * bool(bg) + "%s") % (
         *fg,
         *bg,
         text,
-    ) + COLOR_RESET * end
+    ) + ctlseqs.SGR_NORMAL * end
 
 
 @unix_tty_only
-@terminal_size_cached
 def get_cell_size() -> Optional[Tuple[int, int]]:
     """Returns the current size of a character cell in the :term:`active terminal`.
 
     Returns:
-        The terminal cell size in pixels or `None` if undetermined.
+        The cell size in pixels or `None` if undetermined.
+
+    The speed of this implementation is almost entirely dependent on the terminal; the
+    method it supports and its response time if it has to be queried.
     """
-    ws = get_window_size()
-    size = ws and tuple(map(floordiv, ws, get_terminal_size()))
+    # If a thread reaches this point while the lock is being changed
+    # (the old lock has been acquired but hasn't been changed), after the lock has
+    # been changed and the former lock is released, the waiting thread will acquire
+    # the old lock making it to be out of sync.
+    # Hence the second expression, which allows such a thread to acquire the new
+    # lock and be in sync.
+    # NB: Multiple expressions are processed as multiple nested with statements.
+    with _cell_size_lock, _cell_size_lock:
+        ts = get_terminal_size()
+        if ts == tuple(_cell_size_cache[:2]):
+            size = tuple(_cell_size_cache[2:])
+            return None if 0 in size else size
 
-    return size if size and 0 not in size else None
+        size = text_area_size = None
+
+        # First try ioctl
+        buf = array("H", [0, 0, 0, 0])
+        try:
+            if not fcntl.ioctl(_tty_fd, termios.TIOCGWINSZ, buf):
+                text_area_size = tuple(buf[2:])
+                if 0 in text_area_size:
+                    text_area_size = None
+        except OSError:
+            pass
+
+        if not text_area_size:
+            # Then XTWINOPS
+            # The last sequence is to speed up the entire query since most (if not all)
+            # terminals should support it and most terminals treat queries as FIFO
+            response = query_terminal(
+                ctlseqs.CELL_SIZE_PX_b + ctlseqs.TEXT_AREA_SIZE_PX_b + ctlseqs.DA1_b,
+                more=lambda s: not s.endswith(b"c"),
+            )
+            if response:
+                cell_size_match = ctlseqs.CELL_SIZE_PX_re.match(response.decode())
+                if not cell_size_match:
+                    text_area_size_match = ctlseqs.TEXT_AREA_SIZE_PX_re.match(
+                        response.decode()
+                    )
+            # XTWINOPS specifies (height, width)
+            if cell_size_match:
+                size = tuple(map(int, cell_size_match.groups()))[::-1]
+            elif text_area_size_match:
+                text_area_size = tuple(map(int, text_area_size_match.groups()))[::-1]
+
+                # Termux seems to respond with (height / 2, width), though the values
+                # are incorrect as they change with different zoom levels but still
+                # always give a reasonable (almost always the same) cell size and ratio.
+                if os.environ.get("SHELL", "").startswith("/data/data/com.termux/"):
+                    text_area_size = (text_area_size[0], text_area_size[1] * 2)
+
+        if text_area_size and _swap_win_size:
+            text_area_size = text_area_size[::-1]
+        size = size or (
+            tuple(map(floordiv, text_area_size, ts)) if text_area_size else (0, 0)
+        )
+        _cell_size_cache[:] = ts + size
+
+        return None if 0 in size else size
 
 
 @cached
 def get_fg_bg_colors(
     *, hex: bool = False
 ) -> Tuple[
     Union[None, str, Tuple[int, int, int]], Union[None, str, Tuple[int, int, int]]
@@ -385,29 +419,29 @@
         * an RGB hex string if *hex* is ``True``
         * ``None`` if undetermined
     """
     # The terminal's response to the queries is not read all at once
     with _tty_lock, _tty_lock:  # See the comment in `lock_tty_wrapper()`
         response = query_terminal(
             # Not all terminals (e.g VTE-based) support multiple queries in one escape
-            # sequence, hence the repetition of OSC ... ST
-            f"{OSC}10;?{ST}{OSC}11;?{ST}{CSI}c".encode(),
+            # sequence, hence the separate sequences for FG and BG
+            ctlseqs.TEXT_FG_QUERY_b + ctlseqs.TEXT_BG_QUERY_b + ctlseqs.DA1_b,
             # The response might contain a "c"; can't stop reading at "c"
-            lambda s: not s.endswith(CSI_b),
+            lambda s: not s.endswith(ctlseqs.CSI_b),
         )
         if _queries_enabled:
-            read_tty()  # The rest of the response to `CSI c`
+            read_tty()  # The rest of the response to DA1
 
     fg = bg = None
     if response:
-        for c, spec in RGB_SPEC.findall(response.decode().rpartition(ESC)[0]):
+        for c, spec in ctlseqs.RGB_SPEC_re.findall(response.decode()):
             if c == "10":
-                fg = x_parse_color(spec)
+                fg = ctlseqs.x_parse_color(spec)
             elif c == "11":
-                bg = x_parse_color(spec)
+                bg = ctlseqs.x_parse_color(spec)
 
     return tuple(
         rgb and ("#" + ("{:02x}" * 3).format(*rgb) if hex else rgb) for rgb in (fg, bg)
     )
 
 
 @cached
@@ -420,22 +454,22 @@
     """
     # The terminal's response to the queries is not read all at once
     with _tty_lock, _tty_lock:  # See the comment in `lock_tty_wrapper()`
         # Terminal name/version query + terminal attribute query
         # The latter is to speed up the entire query since most (if not all)
         # terminals should support it and most terminals treat queries as FIFO
         response = query_terminal(
-            f"{CSI}>q{CSI}c".encode(),
+            ctlseqs.XTVERSION_b + ctlseqs.DA1_b,
             # The response might contain a "c"; can't stop reading at "c"
-            lambda s: not s.endswith(CSI_b),
+            lambda s: not s.endswith(ctlseqs.CSI_b),
         )
         if _queries_enabled:
-            read_tty()  # The rest of the response to `CSI c`
+            read_tty()  # The rest of the response to DA1
 
-    match = response and NAME_VERSION.fullmatch(response.decode().rpartition(ESC)[0])
+    match = response and ctlseqs.XTVERSION_re.match(response.decode())
     name, version = (
         match.groups()
         if match
         else map(os.environ.get, ("TERM_PROGRAM", "TERM_PROGRAM_VERSION"))
     )
 
     return (name and name.lower(), version)
@@ -452,87 +486,27 @@
         and :py:func:`os.get_terminal_size` in that it:
 
         - gives the correct size of the :term:`active terminal` even when output is
           redirected, in most cases
         - gives different results in certain situations
         - is what this library works with
     """
-    if _tty:
+    if _tty_fd:
         # faster and gives correct results when output is redirected
         try:
-            size = os.get_terminal_size(_tty)
+            size = os.get_terminal_size(_tty_fd)
         except OSError:
             size = None
     else:
         size = None
 
     return size or _get_terminal_size()
 
 
 @unix_tty_only
-def get_window_size() -> Optional[Tuple[int, int]]:
-    """Returns the current window size of the :term:`active terminal`.
-
-    Returns:
-        The terminal size in pixels.
-
-    The speed of this implementation is almost entirely dependent on the terminal; the
-    method it supports and its response time if it has to be queried.
-
-    Returns ``None`` if the size couldn't be gotten in time or the terminal lacks
-    support.
-    """
-    # If a thread reaches this point while the lock is being changed
-    # (the old lock has been acquired but hasn't been changed), after the lock has
-    # been changed and the former lock is released, the waiting thread will acquire
-    # the old lock making it to be out of sync.
-    # Hence the second expression, which allows such a thread to acquire the new
-    # lock and be in sync.
-    # NB: Multiple expressions are processed as multiple nested with statements.
-    with _win_size_lock, _win_size_lock:
-        ts = get_terminal_size()
-        if ts == tuple(_win_size_cache[:2]):
-            size = tuple(_win_size_cache[2:])
-            return None if 0 in size else size
-
-        # First try ioctl
-        size = None
-        buf = array("H", [0, 0, 0, 0])
-        try:
-            if not fcntl.ioctl(_tty, termios.TIOCGWINSZ, buf):
-                size = tuple(buf[2:])
-                if size == (0, 0):
-                    size = None
-        except OSError:
-            pass
-
-        if not size:
-            # Then CSI 14 t
-            # The second sequence is to speed up the entire query since most (if not
-            # all) terminals should support it and most terminals treat queries as FIFO
-            response = query_terminal(
-                f"{CSI}14t{CSI}c".encode(), more=lambda s: not s.endswith(b"c")
-            )
-            size = (response or None) and WIN_SIZE.match(response.decode())
-            if size:
-                # XTWINOPS specifies (height, width)
-                size = tuple(map(int, size.groups()))[::-1]
-
-                # Termux seems to respond with (height / 2, width), though the values
-                # are incorrect as they change with different zoom levels but still
-                # always give a reasonable (almost always the same) cell size and ratio.
-                if os.environ.get("SHELL", "").startswith("/data/data/com.termux/"):
-                    size = (size[0], size[1] * 2)
-
-        size = size[:: -_swap_win_size or 1] if size else (0, 0)
-        _win_size_cache[:] = ts + size
-        return None if 0 in size else size
-
-
-@unix_tty_only
 @lock_tty
 def query_terminal(
     request: bytes, more: Callable[[bytearray], bool], timeout: float = None
 ) -> Optional[bytes]:
     """Sends a query to the :term:`active terminal` and returns the response.
 
     Args:
@@ -557,23 +531,23 @@
     ATTENTION:
         Any unread input is discared before the query. If the input might be needed,
         it can be read using :py:func:`read_tty()` before calling this fucntion.
     """
     if not _queries_enabled:
         return None
 
-    old_attr = termios.tcgetattr(_tty)
-    new_attr = termios.tcgetattr(_tty)
+    old_attr = termios.tcgetattr(_tty_fd)
+    new_attr = termios.tcgetattr(_tty_fd)
     new_attr[3] &= ~termios.ECHO  # Disable input echo
     try:
-        termios.tcsetattr(_tty, termios.TCSAFLUSH, new_attr)
+        termios.tcsetattr(_tty_fd, termios.TCSAFLUSH, new_attr)
         write_tty(request)
         return read_tty(more, timeout or _query_timeout)
     finally:
-        termios.tcsetattr(_tty, termios.TCSANOW, old_attr)
+        termios.tcsetattr(_tty_fd, termios.TCSANOW, old_attr)
 
 
 @unix_tty_only
 @lock_tty
 def read_tty(
     more: Callable[[bytearray], bool] = lambda _: True,
     timeout: Optional[float] = None,
@@ -612,53 +586,53 @@
       * *more* is not given, input is read or waited for until *timeout* is up.
       * *more* is given, input is read or waited for until ``more(input)`` returns
         ``False`` or *timeout* is up.
 
     Upon return or interruption, the :term:`active terminal` is **immediately** restored
     to the state in which it was met.
     """
-    old_attr = termios.tcgetattr(_tty)
-    new_attr = termios.tcgetattr(_tty)
+    old_attr = termios.tcgetattr(_tty_fd)
+    new_attr = termios.tcgetattr(_tty_fd)
     new_attr[3] &= ~termios.ICANON  # Disable cannonical mode
     new_attr[6][termios.VTIME] = 0  # Never block based on time
     if echo:
         new_attr[3] |= termios.ECHO  # Enable input echo
     else:
         new_attr[3] &= ~termios.ECHO  # Disable input echo
     # Block until *min* bytes are read, when *timeout* is not `None`.
     new_attr[6][termios.VMIN] = 0 if timeout is None else min
 
     input = bytearray()
     try:
-        termios.tcsetattr(_tty, termios.TCSANOW, new_attr)
-        r, w, x = [_tty], [], []
+        termios.tcsetattr(_tty_fd, termios.TCSANOW, new_attr)
+        r, w, x = [_tty_fd], [], []
 
         if timeout is None:
             # VMIN=0 does not work as expected on some platforms when there's no input
             while select(r, w, x, 0.0)[0]:
-                input.extend(os.read(_tty, 100))
+                input.extend(os.read(_tty_fd, 100))
         else:
             start = monotonic()
             if min > 0:
-                input.extend(os.read(_tty, min))
+                input.extend(os.read(_tty_fd, min))
 
                 # Don't block based on based on amount of bytes anymore
                 new_attr[6][termios.VMIN] = 0
-                termios.tcsetattr(_tty, termios.TCSANOW, new_attr)
+                termios.tcsetattr(_tty_fd, termios.TCSANOW, new_attr)
 
             duration = monotonic() - start
             while (timeout < 0 or duration < timeout) and more(input):
                 # Reduces CPU usage
                 # Also, VMIN=0 does not work on some platforms when there's no input
                 if select(r, w, x, None if timeout < 0 else timeout - duration)[0]:
-                    input.extend(os.read(_tty, 1))
+                    input.extend(os.read(_tty_fd, 1))
                 duration = monotonic() - start
             # logging.debug(duration)
     finally:
-        termios.tcsetattr(_tty, termios.TCSANOW, old_attr)
+        termios.tcsetattr(_tty_fd, termios.TCSANOW, old_attr)
 
     return bytes(input)
 
 
 @unix_tty_only
 def read_tty_all() -> bytes:
     """Reads all available input directly from the :term:`active terminal` **without
@@ -677,29 +651,23 @@
 @lock_tty
 def write_tty(data: bytes) -> None:
     """Writes to the :term:`active terminal` and waits until complete transmission.
 
     Args:
         data: Data to be written.
     """
-    os.write(_tty, data)
+    os.write(_tty_fd, data)
     try:
-        termios.tcdrain(_tty)
+        termios.tcdrain(_tty_fd)
     except termios.error:  # "Permission denied" on some platforms e.g Termux
         pass
 
 
-def x_parse_color(spec: str) -> Tuple[int, int, int]:
-    """Converts an RGB device specification according to XParseColor"""
-    # One hex char -> 4 bits
-    return tuple(int(x, 16) * 255 // ((1 << (len(x) * 4)) - 1) for x in spec.split("/"))
-
-
 def _process_start_wrapper(self, *args, **kwargs):
-    global _tty_lock, _win_size_cache, _win_size_lock
+    global _tty_lock, _cell_size_cache, _cell_size_lock
 
     # Ensure a lock is not acquired by another process/thread before changing it.
     # The only case in which this is useless is when the owner thread is the
     # one starting a process. In such a situation, the owner thread will be partially
     # (may acquire the new lock in a nested call while still holding the old lock)
     # out of sync until it has fully released the old lock.
 
@@ -721,104 +689,73 @@
                     "Simply set an 'ignore' filter for this warning (before starting "
                     "any subprocess) if not using any of the affected features.",
                     TermImageWarning,
                 )
         else:
             self._tty_lock = _tty_lock
 
-    with _win_size_lock:
-        if isinstance(_win_size_lock, _rlock_type):
+    with _cell_size_lock:
+        if isinstance(_cell_size_lock, _rlock_type):
             try:
-                self._win_size_cache = _win_size_cache = Array("i", _win_size_cache)
-                _win_size_lock = _win_size_cache.get_lock()
+                self._cell_size_cache = _cell_size_cache = Array("i", _cell_size_cache)
+                _cell_size_lock = _cell_size_cache.get_lock()
             except ImportError:
-                self._win_size_cache = None
+                self._cell_size_cache = None
         else:
-            self._win_size_cache = _win_size_cache
+            self._cell_size_cache = _cell_size_cache
 
     return _process_start_wrapper.__wrapped__(self, *args, **kwargs)
 
 
 def _process_run_wrapper(self, *args, **kwargs):
-    global _tty_lock, _win_size_cache, _win_size_lock
+    global _tty_lock, _cell_size_cache, _cell_size_lock
 
     if self._tty_lock:
         _tty_lock = self._tty_lock
-    if self._win_size_cache:
-        _win_size_cache = self._win_size_cache
-        _win_size_lock = _win_size_cache.get_lock()
+    if self._cell_size_cache:
+        _cell_size_cache = self._cell_size_cache
+        _cell_size_lock = _cell_size_cache.get_lock()
 
     return _process_run_wrapper.__wrapped__(self, *args, **kwargs)
 
 
-RGB_SPEC = re.compile(r"\033](\d+);rgb:([\da-fA-F/]+)\033\\", re.ASCII)
-WIN_SIZE = re.compile(r"\033\[4;(\d+);(\d+)t", re.ASCII)
-NAME_VERSION = re.compile(r"\033P>\|(\w+)[( ]([^)\033]+)\)?\033\\", re.ASCII)
-
-# Constants for escape sequences
-ESC = "\033"
-ESC_b = ESC.encode()
-CSI = f"{ESC}["
-CSI_b = CSI.encode()
-OSC = f"{ESC}]"
-OSC_b = OSC.encode()
-ST = f"{ESC}\\"
-ST_b = ST.encode()
-BG_FMT = f"{CSI}48;2;%d;%d;%dm"
-BG_FMT_b = BG_FMT.encode()
-FG_FMT = f"{CSI}38;2;%d;%d;%dm"
-FG_FMT_b = FG_FMT.encode()
-COLOR_RESET = f"{CSI}m"
-COLOR_RESET_b = COLOR_RESET.encode()
-DECSET = f"{CSI}?%dh"
-DECSET_b = DECSET.encode()
-DECRST = f"{CSI}?%dl"
-DECRST_b = DECRST.encode()
-
-# Terminal Synchronized Output
-# See https://gist.github.com/christianparpart/d8a62cc1ab659194337d73e399004036
-BEGIN_SYNCED_UPDATE = DECSET % 2026
-BEGIN_SYNCED_UPDATE_b = BEGIN_SYNCED_UPDATE.encode()
-END_SYNCED_UPDATE = DECRST % 2026
-END_SYNCED_UPDATE_b = END_SYNCED_UPDATE.encode()
-
 # Private internal variables
 _query_timeout = 0.1
 _queries_enabled: bool = True
 _swap_win_size: bool = False
-_tty: Optional[int] = None
+_tty_fd: Optional[int] = None
 _tty_lock = RLock()
-_win_size_cache = [0] * 4
-_win_size_lock = RLock()
+_cell_size_cache = [0] * 4
+_cell_size_lock = RLock()
 _rlock_type = type(_tty_lock)
 
 if OS_IS_UNIX:
     for stream in ("out", "in", "err"):  # In order of priority
         try:
-            _tty = os.ttyname(getattr(sys, f"__std{stream}__").fileno())
+            _tty_fd = os.ttyname(getattr(sys, f"__std{stream}__").fileno())
             break
         except (OSError, AttributeError):
             pass
     else:
         try:
-            _tty = os.open("/dev/tty", os.O_RDWR | os.O_NOCTTY)
+            _tty_fd = os.open("/dev/tty", os.O_RDWR | os.O_NOCTTY)
         except OSError:
             warnings.warn(
                 "It seems this process is not running within a terminal. "
                 "Hence, some features will behave differently or be disabled.\n"
                 "See https://term-image.readthedocs.io/en/stable/guide/concepts"
                 ".html#active-terminal\n"
                 "Any filter for this warning must be set before loading `term_image`, "
                 "using `UserWarning` with the warning message (since "
                 "`TermImageWarning` won't be available).",
                 TermImageWarning,
             )
-    if _tty:
-        if isinstance(_tty, str):
-            _tty = os.open(_tty, os.O_RDWR)
+    if _tty_fd:
+        if isinstance(_tty_fd, str):
+            _tty_fd = os.open(_tty_fd, os.O_RDWR)
 
         Process.start = wraps(Process.start)(_process_start_wrapper)
         Process.run = wraps(Process.run)(_process_run_wrapper)
 
         # Shouldn't be needed since we're getting our own separate file descriptors
         # but the validity of the assumed safety is stil under probation
         """
```

### Comparing `term-image-0.6.1/src/term_image/widget/urwid.py` & `term-image-0.7.0/src/term_image/widget/urwid.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,23 +4,21 @@
 
 __all__ = ("UrwidImage", "UrwidImageCanvas", "UrwidImageScreen")
 
 from typing import Optional, Tuple
 
 import urwid
 
+from .. import ctlseqs
+
+# These sequences are used during performance-critical operations that occur often
+from ..ctlseqs import BEGIN_SYNCED_UPDATE, END_SYNCED_UPDATE, ESC_b, SGR_NORMAL_b
 from ..exceptions import UrwidImageError
-from ..image import BaseImage, ITerm2Image, KittyImage, Size, TextImage, kitty
-from ..utils import (
-    BEGIN_SYNCED_UPDATE,
-    END_SYNCED_UPDATE,
-    COLOR_RESET_b,
-    ESC_b,
-    lock_tty,
-)
+from ..image import BaseImage, ITerm2Image, KittyImage, Size, TextImage
+from ..utils import arg_type_error, get_terminal_name_version, lock_tty, write_tty
 
 # NOTE: Any new "private" attribute of any subclass of an urwid class should be
 # prepended with "_ti" to prevent clashes with names used by urwid itself.
 
 
 class UrwidImage(urwid.Widget):
     """Image widget (box/flow) for the urwid TUI framework.
@@ -76,26 +74,22 @@
     # from -(2**31)
     _ti_next_z_index = 1
 
     def __init__(
         self, image: BaseImage, format_spec: str = "", *, upscale: bool = False
     ) -> None:
         if not isinstance(image, BaseImage):
-            raise TypeError(f"Invalid type for 'image' (got: {type(image).__name__})")
+            raise arg_type_error("image", image)
 
         if not isinstance(format_spec, str):
-            raise TypeError(
-                f"Invalid type for 'format_spec' (got: {type(format_spec).__name__})"
-            )
+            raise arg_type_error("format_spec", format_spec)
         *fmt, alpha, style_args = image._check_format_spec(format_spec)
 
         if not isinstance(upscale, bool):
-            raise TypeError(
-                f"Invalid type for 'upscale' (got: {type(upscale).__name__})"
-            )
+            raise arg_type_error("upscale", upscale)
 
         super().__init__()
         self._ti_image = image
         self._ti_h_align, _, self._ti_v_align, _ = fmt
         self._ti_alpha = alpha
         self._ti_style_args = style_args
         self._ti_sizing = Size.FIT if upscale else Size.AUTO
@@ -104,75 +98,54 @@
             style_args["split_cells"] = True
         elif isinstance(image, KittyImage):
             style_args["z_index"] = self._ti_z_index = self._ti_get_z_index()
 
             # Since Konsole doesn't blend images placed at the same location and
             # z-index, unlike Kitty (and potentially others), `blend=True` is
             # better on Konsole as it reduces/eliminates flicker.
-            if KittyImage._TERM != "konsole":
+            if get_terminal_name_version()[0] != "konsole":
                 # To clear directly overlapped images when urwid redraws a line without
                 # a change in image position
                 style_args["blend"] = False
 
     def __del__(self) -> None:
         if hasattr(self, "_ti_z_index"):
             __class__._ti_free_z_indexes.add(self._ti_z_index)
 
     image = property(
         lambda self: self._ti_image,
         doc="""
-        The image rendered by the widget.
+        The image rendered by the widget
 
         :type: BaseImage
+
+        GET:
+            Returns the image instance rendered by the widget.
         """,
     )
 
-    def clear(self, *, now: bool = False) -> None:
-        """Clears all images drawn by the widget, if the image rendered by the widget
-        is of the :py:class:`kitty <term_image.image.KittyImage>` render style.
-
-        Args:
-            now: If ``True`` the images are cleared immediately. Otherwise they're
-              cleared just before the next screen redraw.
-        """
-        if isinstance(self._ti_image, KittyImage):
-            KittyImage.clear(z_index=self._ti_z_index, now=now)
-            self._ti_disguise_state = (self._ti_disguise_state + 1) % 3
-
-    @staticmethod
-    def clear_all(*, now: bool = False) -> None:
-        """Clears all on-screen images of :ref:`graphics-based <graphics-based>` styles
-        that support/require such an operation.
-
-        Args:
-            now: If ``True`` the images are cleared immediately. Otherwise they're
-              cleared just before the next screen redraw.
-        """
-        KittyImage.clear(now=now)  # Also takes care of iterm2 images on Konsole
-        UrwidImageCanvas._ti_change_disguise()
-
     def render(self, size: Tuple[int, int], focus: bool = False) -> urwid.Canvas:
         image = self._ti_image
 
         if len(size) == 2:  # box
-            image.set_size(self._ti_sizing, maxsize=size)
+            image.set_size(self._ti_sizing, frame_size=size)
         elif len(size) == 1:  # flow
             if self._ti_sizing is Size.FIT:
                 image.set_size(size[0])
             else:
                 fit_size = self._ti_image._valid_size(size[0])
                 ori_size = self._ti_image._valid_size(Size.ORIGINAL)
                 image._size = (
                     ori_size
                     if ori_size[0] <= fit_size[0] and ori_size[1] <= fit_size[1]
                     else fit_size
                 )
             size = (size[0], image._size[1])
         else:  # fixed
-            raise ValueError("Not a fixed widget")
+            raise UrwidImageError("Not a fixed widget")
 
         try:
             render = image._format_render(
                 image._renderer(
                     image._render_image, self._ti_alpha, **self._ti_style_args
                 ),
                 self._ti_h_align,
@@ -213,15 +186,15 @@
         Raises:
             TypeError: *widget* is not an urwid widget.
 
         If set, any exception raised during rendering is **suppressed** and the
         placeholder is rendered in place of the image.
         """
         if not isinstance(widget, urwid.Widget):
-            raise TypeError("Invalid type for 'widget' (got: {type(widget).__name__})")
+            raise arg_type_error("widget", widget)
 
         cls._ti_error_placeholder = widget
 
     @staticmethod
     def _ti_get_z_index() -> int:
         if __class__._ti_free_z_indexes:
             return __class__._ti_free_z_indexes.pop()
@@ -229,14 +202,18 @@
         z_index = __class__._ti_next_z_index
         if z_index == 2**31:
             raise UrwidImageError("Too many image widgets with the kitty render style")
         __class__._ti_next_z_index = -z_index if z_index > 0 else -z_index + 1
 
         return z_index
 
+    def _ti_change_disguise(self) -> None:
+        """See :py:meth`UrwidImageCanvas._ti_change_disguise`."""
+        self._ti_disguise_state = (self._ti_disguise_state + 1) % 3
+
 
 class UrwidImageCanvas(urwid.Canvas):
     """Image canvas for the urwid TUI framework.
 
     Args:
         render: The rendered image.
         size: The canvas size. Also, the size of the rendered (and formatted) image.
@@ -359,15 +336,15 @@
                 left_padding = (
                     ((None, "U", b" " * new_pad_left),) if new_pad_left else ()
                 )
                 right_padding = (
                     ((None, "U", b" " * new_pad_right),) if new_pad_right else ()
                 )
                 color_reset = (
-                    ((None, "U", COLOR_RESET_b),)
+                    ((None, "U", SGR_NORMAL_b),)
                     if image_size[0] > trim_image_right > 0
                     else ()
                 )
                 last_row_workaround = ((None, "U", b"\0\0"),)
 
             if image_is_empty:
                 image_lines = []
@@ -424,15 +401,15 @@
         else:
             disguise = (
                 b"\b "
                 * (self._ti_disguise_state + widget._ti_disguise_state)
                 * (
                     isinstance(image, KittyImage)
                     or isinstance(image, ITerm2Image)
-                    and ITerm2Image._TERM == "konsole"
+                    and get_terminal_name_version()[0] == "konsole"
                 )
             )
             for line in self._ti_lines[trim_top : -trim_bottom or None]:
                 yield [(None, "U", line + disguise)]
 
     def rows(self) -> int:
         return self.size[1]
@@ -528,14 +505,73 @@
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._ti_screen_canv = None
         self._ti_image_cviews = frozenset()
 
+    def clear(self):
+        self.clear_images()
+        return super().clear()
+
+    def clear_images(self, *widgets: UrwidImage, now: bool = False) -> None:
+        """Clears on-screen images of :ref:`graphics-based <graphics-based>`
+        styles **that support/require such an operation**.
+
+        Args:
+            widgets: Image widgets to clear.
+
+              All on-screen images rendered by each of the widgets are cleared,
+              provided the widget was initialized with a
+              :py:class:`term_image.image.KittyImage` instance.
+
+              If none is given, all images (of styles **that support/require such an
+              operation**) on-screen are cleared.
+
+            now: If ``True`` the images are cleared immediately.
+              Otherwise, they're cleared when next the output buffer is flushed,
+              such as at the next screen redraw.
+        """
+        # Also takes care of iterm2 images on Konsole
+        if not (KittyImage.forced_support or KittyImage.is_supported()):
+            return
+
+        if widgets:
+            # Better to send the delete commands in a batch than individually
+            kitty_widgets = []
+            for index, widget in enumerate(widgets):
+                if not isinstance(widget, UrwidImage):
+                    raise arg_type_error(f"widgets[{index}]", widget)
+
+                if isinstance(widget._ti_image, KittyImage):
+                    kitty_widgets.append(widget)
+                    widget._ti_change_disguise()
+
+            if kitty_widgets:
+                if now:
+                    write_tty(
+                        b"".join(
+                            ctlseqs.KITTY_DELETE_Z_INDEX_b % widget._ti_z_index
+                            for widget in kitty_widgets
+                        )
+                    )
+                else:
+                    self.write(
+                        "".join(
+                            ctlseqs.KITTY_DELETE_Z_INDEX % widget._ti_z_index
+                            for widget in kitty_widgets
+                        )
+                    )
+        else:
+            if now:
+                write_tty(ctlseqs.KITTY_DELETE_ALL_b)
+            else:
+                self.write(ctlseqs.KITTY_DELETE_ALL)
+            UrwidImageCanvas._ti_change_disguise()
+
     # `@lock_tty` prevents queries during a synced update.
     # Otherwise, responses would be delayed until the synced update ends and that might
     # be after the query has timed out.
     @lock_tty
     def draw_screen(self, maxres, canvas):
         """See the description of the baseclass' method.
 
@@ -565,39 +601,35 @@
     @lock_tty
     def write(self, data):
         """See the baseclass' method for the description."""
         return super().write(data)
 
     def _start(self, *args, **kwargs):
         ret = super()._start(*args, **kwargs)
-        if KittyImage._forced_support or KittyImage.is_supported():
-            self.write(kitty.DELETE_ALL_IMAGES)
-
+        self.clear_images()
         return ret
 
     def _stop(self):
-        if KittyImage._forced_support or KittyImage.is_supported():
-            self.write(kitty.DELETE_ALL_IMAGES)
-
+        self.clear_images()
         return super()._stop()
 
     def _ti_clear_images(self):
         if not (
-            KittyImage._forced_support
+            KittyImage.forced_support
             or KittyImage.is_supported()
             or ITerm2Image.is_supported()
-            and ITerm2Image._TERM == "konsole"
+            and get_terminal_name_version()[0] == "konsole"
         ):
             return
 
         screen_canv = self._ti_screen_canv
 
         if not isinstance(screen_canv, urwid.CompositeCanvas):
             if self._ti_image_cviews:
-                UrwidImage.clear_all()
+                self.clear_images()
                 self._ti_image_cviews.clear()
             return
 
         def process_shard_tails():
             nonlocal col
 
             while col in shard_tails:
@@ -623,15 +655,15 @@
                         widget = canv.widget_info[0]
                     except TypeError:
                         pass
                     else:
                         if (
                             isinstance(widget._ti_image, KittyImage)
                             or isinstance(widget._ti_image, ITerm2Image)
-                            and ITerm2Image._TERM == "konsole"
+                            and get_terminal_name_version()[0] == "konsole"
                         ):
                             image_cviews.add((canv, row, col, *trim, cols, rows))
 
                 if rows > n_rows:
                     shard_tails[col] = (*trim, cols, rows - n_rows, canv)
                 col += cols
             process_shard_tails()
@@ -639,16 +671,16 @@
 
         kitty_widgets = []
         for canv, *_ in self._ti_image_cviews - image_cviews:
             widget = canv.widget_info[0]
             if isinstance(widget._ti_image, KittyImage):
                 kitty_widgets.append(widget)
             else:
-                UrwidImage.clear_all()
-                # Multiple `clear_all()`s messes up the canvas disguise
-                # Also, a single `clear_all()` takes care of all images
+                self.clear_images()
+                # Multiple `clear_images()`s messes up the canvas disguise
+                # A single `clear_images()` takes care of all images anyways
                 break
         else:
-            for widget in kitty_widgets:
-                widget.clear()
+            if kitty_widgets:
+                self.clear_images(*kitty_widgets)
 
         self._ti_image_cviews = frozenset(image_cviews)
```

### Comparing `term-image-0.6.1/src/term_image.egg-info/PKG-INFO` & `term-image-0.7.0/src/term_image.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: term-image
-Version: 0.6.1
+Version: 0.7.0
 Summary: Display images in the terminal
 Home-page: https://github.com/AnonymouX47/term-image
 Author: Toluwaleke Ogundipe
 Author-email: anonymoux47@gmail.com
 License: MIT
 Project-URL: Changelog, https://github.com/AnonymouX47/term-image/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://term-image.readthedocs.io/
@@ -29,24 +29,20 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Terminals :: Terminal Emulators/X Terminals
 Classifier: Topic :: Multimedia :: Graphics :: Viewers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<a href="https://www.buymeacoffee.com/anonymoux47" target="_blank">
-   <img align="right" src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" >
-</a><br><br>
-
 <div align="center">
 
 <h1><b>Term-Image</b></h1>
 
 <p>
-<img src="https://raw.githubusercontent.com/AnonymouX47/term-image/abca69a2cc50f60aa16d982a8f11ccd294ce50bf/docs/source/resources/logo.png" height="200">
+<img src="https://raw.githubusercontent.com/AnonymouX47/term-image/92ff4b2d2e4731be9e1b2ac7378964ebed9f10f9/docs/source/resources/logo.png" height="200">
 </p>
 
 <p>
 <b>Display images in the terminal with Python</b>
 </p>
 
 <p>
@@ -90,15 +86,15 @@
 - [Quick Start](#library-quick-start)
 - [Usage](#usage)
 - [Contribution](#contribution)
 - [Planned Features](#planned-features)
 - [Known Issues](#known-issues)
 - [FAQs](#faqs)
 - [Credits](#credits)
-- [Donate](#donate)
+- [Sponsor This Project](#sponsor-this-project)
 
 
 > ### ⚠️ NOTICE!!! ⚠️
 > The image viewer (CLI and TUI) has been moved to [termvisage].
 
 
 ## Installation
@@ -212,15 +208,15 @@
 ## Usage
 
 <p align="center"><b>
    🚧 Under Construction - There will most likely be incompatible changes between minor versions of
    <a href='https://semver.org/spec/v2.0.0.html#spec-item-4'>version zero</a>!
 </b></p>
 
-**If you want to use this library in a project while it's still on version zero, ensure you pin the dependency version to a specific minor version e.g `>=0.4,<0.5`.**
+**If you want to use this library in a project while it's still on version zero, ensure you pin the dependency to a specific minor version e.g `>=0.4,<0.5`.**
 
 See the [docs](https://term-image.readthedocs.io) for the User Guide and API Reference.
 
 
 ## Contribution
 
 Please read through the [guidelines](https://github.com/AnonymouX47/term-image/blob/main/CONTRIBUTING.md).
@@ -244,21 +240,24 @@
 ## FAQs
 
 See the [FAQs](https://term-image.readthedocs.io/en/stable/faqs.html) section of the docs.
 
 ## Credits
 
 The following projects have been (and are still) crucial to the development of this project:
+- [Pillow](https://python-pillow.org) by [Fredrik Lundh, Jeffrey A. Clark (Alex) and contributors](https://github.com/python-pillow/Pillow/graphs/contributors)
+- [Requests](https://requests.readthedocs.io) by [Kenneth Reitz and others](https://requests.readthedocs.io/en/latest/dev/authors/)
 
-- [Pillow](https://python-pillow.org)
+The logo was composed using resource(s) from the following source(s):
+- [Gallery icons created by Andrean Prabowo - Flaticon](https://www.flaticon.com/free-icons/gallery)
 
-## Donate
+## Sponsor This Project
 
 <a href="https://www.buymeacoffee.com/anonymoux47" target="_blank">
    <img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" >
 </a>
 
-Your donation will go a long way in aiding the progress and development of this project.
+Any amount will go a long way in aiding the progress and development of this project.
 Thank you! 💓
 
 
 [termvisage]: https://github.com/AnonymouX47/termvisage
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: term-image Version: 0.6.1 Summary: Display images
+Metadata-Version: 2.1 Name: term-image Version: 0.7.0 Summary: Display images
 in the terminal Home-page: https://github.com/AnonymouX47/term-image Author:
 Toluwaleke Ogundipe Author-email: anonymoux47@gmail.com License: MIT Project-
 URL: Changelog, https://github.com/AnonymouX47/term-image/blob/main/
 CHANGELOG.md Project-URL: Documentation, https://term-image.readthedocs.io/
 Project-URL: Funding, https://github.com/AnonymouX47/term-image#donate Project-
 URL: Source, https://github.com/AnonymouX47/term-image Project-URL: Tracker,
 https://github.com/AnonymouX47/term-image/issues Keywords:
@@ -15,85 +15,85 @@
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3 ::
 Only Classifier: Topic :: Software Development :: Libraries Classifier: Topic
 :: Terminals :: Terminal Emulators/X Terminals Classifier: Topic :: Multimedia
 :: Graphics :: Viewers Requires-Python: >=3.7 Description-Content-Type: text/
-markdown License-File: LICENSE [Buy_Me_A_Coffee]
-
+markdown License-File: LICENSE
                            ****** Term-Image ******
           [https://raw.githubusercontent.com/AnonymouX47/term-image/
-   abca69a2cc50f60aa16d982a8f11ccd294ce50bf/docs/source/resources/logo.png]
+   92ff4b2d2e4731be9e1b2ac7378964ebed9f10f9/docs/source/resources/logo.png]
                   Display images in the terminal with Python
                                Docs ║  Tutorial
  [https://img.shields.io/pypi/v/term-image.svg] [https://pepy.tech/badge/term-
 image/month] [https://img.shields.io/pypi/pyversions/term-image.svg] [https://
    img.shields.io/badge/code%20style-black-000000.svg] [https://github.com/
   AnonymouX47/term-image/actions/workflows/test.yml/badge.svg] [Documentation
   Status] [https://img.shields.io/github/last-commit/AnonymouX47/term-image]
      [https://img.shields.io/twitter/url/http/shields.io.svg?style=social]
 ## Contents - [Installation](#installation) - [Features](#features) - [Demo]
 (#demo) - [Quick Start](#library-quick-start) - [Usage](#usage) -
 [Contribution](#contribution) - [Planned Features](#planned-features) - [Known
-Issues](#known-issues) - [FAQs](#faqs) - [Credits](#credits) - [Donate]
-(#donate) > ### â ï¸ NOTICE!!! â ï¸ > The image viewer (CLI and TUI) has
-been moved to [termvisage]. ## Installation ### Requirements - Operating
-System: Unix / Linux / Mac OS X / Windows (limited support, see the [FAQs]
-(https://term-image.readthedocs.io/en/stable/faqs.html)) - [Python](https://
-www.python.org/) >= 3.7 - A terminal emulator with **any** of the following: -
-support for the [Kitty graphics protocol](https://sw.kovidgoyal.net/kitty/
-graphics-protocol/). - support for the [iTerm2 inline image protocol](https://
-iterm2.com/documentation-images.html). - full Unicode support and ANSI 24-bit
-color support **Plans to support a wider variety of terminal emulators are in
-motion** (see [Planned Features](#planned-features)). ### Steps The latest
-**stable** version can be installed from [PyPI](https://pypi.org/project/term-
-image) with: ```shell pip install term-image ``` The **development** version
-can be installed with: ```shell pip install git+https://github.com/AnonymouX47/
-term-image.git ``` ### Supported Terminal Emulators See [here](https://term-
-image.readthedocs.io/en/stable/start/installation.html#supported-terminal-
-emulators) for a list of tested terminal emulators. If you've tested this
-library on any other terminal emulator that meets the requirements for any of
-the render styles, please mention the name (and version) in a new thread under
-[this discussion](https://github.com/AnonymouX47/term-image/discussions/4).
-Also, if you have any issue with terminal support, you may report or check
-information about it in the discussion linked above. ## Features - Multiple
-image formats (basically all formats supported by [`PIL.Image.open()`](https://
-pillow.readthedocs.io/en/stable/handbook/image-file-formats.html)) - Multiple
-image source types: PIL image instance, local file, URL - Multiple image render
-styles (with automatic support detection) - Support for multiple terminal
-graphics protocols: [Kitty](https://sw.kovidgoyal.net/kitty/graphics-protocol/
-), [iTerm2](https://iterm2.com/documentation-images.html) - Exposes various
-features of the protocols - Transparency support (with multiple options) -
-Animated image support (including transparent ones) - Multiple formats: GIF,
-WEBP, APNG (and possibly more) - Fully controllable iteration over rendered
-frames of animated images - Image animation with multiple parameters -
-Integration into various TUI / terminal-based output libraries. - Terminal size
-awareness - Automatic and manual image sizing - Horizontal and vertical
-alignment - Automatic and manual font ratio adjustment (to preserve image
-aspect ratio) - and more... ð ## Demo Check out this [image viewer]
-[termvisage] based on this library. ## Quick Start ### Creating an instance 1.
-Initialize with a file path: ```python from term_image.image import from_file
-image = from_file("path/to/image.png") ``` 2. Initialize with a URL: ```python
-from term_image.image import from_url image = from_url("https://
-www.example.com/image.png") ``` 3. Initialize with a PIL (Pillow) image
-instance: ```python from PIL import Image from term_image.image import
-AutoImage img = Image.open("path/to/image.png") image = AutoImage(img) ``` ###
-Drawing/Displaying an Image There are two basic ways to draw an image to the
-terminal screen: 1. Using the `draw()` method: ```python image.draw() ```
-**NOTE:** `draw()` has various parameters for render formatting. 2. Using
-`print()` with an image render output: ```python print(image) # without
-formatting # OR print(f"{image:>200.^100#ffffff}") # with formatting ``` For
-animated images, only the former animates the output, the latter only draws the
-current frame. See the [tutorial](https://term-image.readthedocs.io/en/stable/
-start/tutorial.html) for a more detailed introduction. ## Usage
+Issues](#known-issues) - [FAQs](#faqs) - [Credits](#credits) - [Sponsor This
+Project](#sponsor-this-project) > ### â ï¸ NOTICE!!! â ï¸ > The image
+viewer (CLI and TUI) has been moved to [termvisage]. ## Installation ###
+Requirements - Operating System: Unix / Linux / Mac OS X / Windows (limited
+support, see the [FAQs](https://term-image.readthedocs.io/en/stable/faqs.html))
+- [Python](https://www.python.org/) >= 3.7 - A terminal emulator with **any**
+of the following: - support for the [Kitty graphics protocol](https://
+sw.kovidgoyal.net/kitty/graphics-protocol/). - support for the [iTerm2 inline
+image protocol](https://iterm2.com/documentation-images.html). - full Unicode
+support and ANSI 24-bit color support **Plans to support a wider variety of
+terminal emulators are in motion** (see [Planned Features](#planned-features)).
+### Steps The latest **stable** version can be installed from [PyPI](https://
+pypi.org/project/term-image) with: ```shell pip install term-image ``` The
+**development** version can be installed with: ```shell pip install git+https:/
+/github.com/AnonymouX47/term-image.git ``` ### Supported Terminal Emulators See
+[here](https://term-image.readthedocs.io/en/stable/start/
+installation.html#supported-terminal-emulators) for a list of tested terminal
+emulators. If you've tested this library on any other terminal emulator that
+meets the requirements for any of the render styles, please mention the name
+(and version) in a new thread under [this discussion](https://github.com/
+AnonymouX47/term-image/discussions/4). Also, if you have any issue with
+terminal support, you may report or check information about it in the
+discussion linked above. ## Features - Multiple image formats (basically all
+formats supported by [`PIL.Image.open()`](https://pillow.readthedocs.io/en/
+stable/handbook/image-file-formats.html)) - Multiple image source types: PIL
+image instance, local file, URL - Multiple image render styles (with automatic
+support detection) - Support for multiple terminal graphics protocols: [Kitty]
+(https://sw.kovidgoyal.net/kitty/graphics-protocol/), [iTerm2](https://
+iterm2.com/documentation-images.html) - Exposes various features of the
+protocols - Transparency support (with multiple options) - Animated image
+support (including transparent ones) - Multiple formats: GIF, WEBP, APNG (and
+possibly more) - Fully controllable iteration over rendered frames of animated
+images - Image animation with multiple parameters - Integration into various
+TUI / terminal-based output libraries. - Terminal size awareness - Automatic
+and manual image sizing - Horizontal and vertical alignment - Automatic and
+manual font ratio adjustment (to preserve image aspect ratio) - and more...
+ð ## Demo Check out this [image viewer][termvisage] based on this library.
+## Quick Start ### Creating an instance 1. Initialize with a file path:
+```python from term_image.image import from_file image = from_file("path/to/
+image.png") ``` 2. Initialize with a URL: ```python from term_image.image
+import from_url image = from_url("https://www.example.com/image.png") ``` 3.
+Initialize with a PIL (Pillow) image instance: ```python from PIL import Image
+from term_image.image import AutoImage img = Image.open("path/to/image.png")
+image = AutoImage(img) ``` ### Drawing/Displaying an Image There are two basic
+ways to draw an image to the terminal screen: 1. Using the `draw()` method:
+```python image.draw() ``` **NOTE:** `draw()` has various parameters for render
+formatting. 2. Using `print()` with an image render output: ```python print
+(image) # without formatting # OR print(f"{image:>200.^100#ffffff}") # with
+formatting ``` For animated images, only the former animates the output, the
+latter only draws the current frame. See the [tutorial](https://term-
+image.readthedocs.io/en/stable/start/tutorial.html) for a more detailed
+introduction. ## Usage
    ð§ Under Construction - There will most likely be incompatible changes
                     between minor versions of version_zero!
 **If you want to use this library in a project while it's still on version
-zero, ensure you pin the dependency version to a specific minor version e.g
+zero, ensure you pin the dependency to a specific minor version e.g
 `>=0.4,<0.5`.** See the [docs](https://term-image.readthedocs.io) for the User
 Guide and API Reference. ## Contribution Please read through the [guidelines]
 (https://github.com/AnonymouX47/term-image/blob/main/CONTRIBUTING.md). For code
 contributions, you should also check out the [Planned Features](#planned-
 features). If you wish to work on any of the listed features/improvements,
 please click on the linked issue or go through the [issues](https://github.com/
 AnonymouX47/term-image/issues) section and join in on an ongoing discussion
@@ -101,10 +101,16 @@
 the implementation can be discussed. Hint: You can filter issues by *label* or
 simply *search* using the features's description. Thanks! ð ## Planned
 Features See [here](https://term-image.readthedocs.io/en/stable/planned.html).
 ## Known Issues See [here](https://term-image.readthedocs.io/en/stable/
 issues.html). ## FAQs See the [FAQs](https://term-image.readthedocs.io/en/
 stable/faqs.html) section of the docs. ## Credits The following projects have
 been (and are still) crucial to the development of this project: - [Pillow]
-(https://python-pillow.org) ## Donate [Buy_Me_A_Coffee] Your donation will go a
-long way in aiding the progress and development of this project. Thank you!
-ð [termvisage]: https://github.com/AnonymouX47/termvisage
+(https://python-pillow.org) by [Fredrik Lundh, Jeffrey A. Clark (Alex) and
+contributors](https://github.com/python-pillow/Pillow/graphs/contributors) -
+[Requests](https://requests.readthedocs.io) by [Kenneth Reitz and others]
+(https://requests.readthedocs.io/en/latest/dev/authors/) The logo was composed
+using resource(s) from the following source(s): - [Gallery icons created by
+Andrean Prabowo - Flaticon](https://www.flaticon.com/free-icons/gallery) ##
+Sponsor This Project [Buy_Me_A_Coffee] Any amount will go a long way in aiding
+the progress and development of this project. Thank you! ð [termvisage]:
+https://github.com/AnonymouX47/termvisage
```

### Comparing `term-image-0.6.1/src/term_image.egg-info/SOURCES.txt` & `term-image-0.7.0/src/term_image.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 src/term_image/__init__.py
+src/term_image/ctlseqs.py
 src/term_image/exceptions.py
 src/term_image/utils.py
 src/term_image.egg-info/PKG-INFO
 src/term_image.egg-info/SOURCES.txt
 src/term_image.egg-info/dependency_links.txt
 src/term_image.egg-info/requires.txt
 src/term_image.egg-info/top_level.txt
```

### Comparing `term-image-0.6.1/tests/test_iterator.py` & `term-image-0.7.0/tests/test_iterator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import atexit
 from types import GeneratorType
 
 import pytest
 from PIL import Image
 
+from term_image.ctlseqs import SGR_NORMAL
 from term_image.exceptions import TermImageError
 from term_image.image import BlockImage, ImageIterator, Size
-from term_image.utils import COLOR_RESET
 
 _size = (30, 15)
 
 png_img = Image.open("tests/images/python.png")
 png_image = BlockImage(png_img)
 gif_img = Image.open("tests/images/lion.gif")
 gif_image = BlockImage(gif_img)
@@ -204,23 +204,14 @@
     gif_image2._size = (40, 20)
     frame_0_2 = next(image_it)
     assert frame_0_2 is not frame_0_1
     assert frame_0_2.count("\n") + 1 == 20
     image_it.seek(gif_image2.n_frames - 1)
     assert next(image_it).count("\n") + 1 == 20
 
-    # Change in scale
-    gif_image2.scale = 0.5
-    frame_0_3 = next(image_it)
-    assert frame_0_3 is not frame_0_1
-    assert frame_0_3 is not frame_0_2
-    assert frame_0_3.count("\n") + 1 == 10
-    image_it.seek(gif_image2.n_frames - 1)
-    assert next(image_it).count("\n") + 1 == 10
-
     image_it.close()
 
 
 def test_sizing():
     def test(image_it):
         for value in Size:
             gif_image2.size = value
@@ -253,21 +244,21 @@
 
 
 def test_formatting():
     # Transparency enabled, not padded
     image_it = ImageIterator(gif_image, 1, "1.1")
     assert next(image_it).count("\n") + 1 == _size[1]
     # First line without escape codes
-    assert next(image_it).partition("\n")[0].strip(COLOR_RESET) == " " * _size[0]
+    assert next(image_it).partition("\n")[0].strip(SGR_NORMAL) == " " * _size[0]
 
     # Transparency disabled, not padded
     image_it = ImageIterator(gif_image, 1, "1.1#")
     assert next(image_it).count("\n") + 1 == _size[1]
     # First line without escape codes
-    assert next(image_it).partition("\n")[0].strip(COLOR_RESET) != " " * _size[0]
+    assert next(image_it).partition("\n")[0].strip(SGR_NORMAL) != " " * _size[0]
 
     # Transparency disabled, padded
     image_it = ImageIterator(gif_image, 1, f"{_size[0] + 2}.{_size[1] + 2}#")
     assert next(image_it).count("\n") + 1 == _size[1] + 2
     # First line should be padding, so no escape codes
     assert next(image_it).partition("\n")[0] == " " * (_size[0] + 2)
```

### Comparing `term-image-0.6.1/tests/test_top_level.py` & `term-image-0.7.0/tests/test_top_level.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 from . import reset_cell_size_ratio, set_cell_size
 
 
 class TestCellRatio:
     @reset_cell_size_ratio()
     def test_args(self):
         for value in (0, "1", ()):
-            with pytest.raises(TypeError, match=r"'ratio' must be"):
+            with pytest.raises(TypeError):
                 set_cell_ratio(value)
         for value in (0.0, -0.1, -1.0):
-            with pytest.raises(ValueError, match=r"'ratio' must be"):
+            with pytest.raises(ValueError):
                 set_cell_ratio(value)
 
         set_cell_size(None)
         for value in AutoCellRatio:
             with pytest.raises(TermImageError):
                 set_cell_ratio(value)
```

