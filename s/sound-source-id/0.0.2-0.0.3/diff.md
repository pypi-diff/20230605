# Comparing `tmp/sound_source_id-0.0.2.tar.gz` & `tmp/sound_source_id-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sound_source_id-0.0.2.tar", last modified: Sat Jun  3 06:57:23 2023, max compression
+gzip compressed data, was "sound_source_id-0.0.3.tar", last modified: Mon Jun  5 08:17:45 2023, max compression
```

## Comparing `sound_source_id-0.0.2.tar` & `sound_source_id-0.0.3.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-03 06:57:23.980374 sound_source_id-0.0.2/
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    35147 2010-06-04 09:15:48.000000 sound_source_id-0.0.2/COPYING.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      408 2023-06-03 06:35:59.000000 sound_source_id-0.0.2/MANIFEST.in
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    41505 2023-06-03 06:57:23.980374 sound_source_id-0.0.2/PKG-INFO
--rw-rwxr--   0 sam       (1000) extdrive  (1777)       46 2023-02-28 10:13:11.000000 sound_source_id-0.0.2/README.md
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-03 06:57:23.936373 sound_source_id-0.0.2/icons/
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    13103 2012-08-13 00:56:29.000000 sound_source_id-0.0.2/icons/audio-headphones.svgz
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     7056 2012-08-13 00:59:09.000000 sound_source_id-0.0.2/icons/help-about.svgz
--rw-rwxr--   0 sam       (1000) extdrive  (1777)   679822 2015-11-04 09:40:24.000000 sound_source_id-0.0.2/icons/help-contents.svgz
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)   255671 2012-08-13 01:04:33.000000 sound_source_id-0.0.2/icons/help-contextual.svgz
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     7408 2023-06-02 05:19:07.000000 sound_source_id-0.0.2/icons/point-left.svg
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4761 2023-06-02 05:19:10.000000 sound_source_id-0.0.2/icons/point-right.svg
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    10662 2012-08-13 00:56:47.000000 sound_source_id-0.0.2/icons/preferences-other.svgz
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-03 06:57:23.937373 sound_source_id-0.0.2/make_noises/
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     2120 2023-05-31 05:23:34.000000 sound_source_id-0.0.2/make_noises/make_pink_noises.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)   171895 2020-04-12 10:56:23.000000 sound_source_id-0.0.2/make_noises/sndlib.py
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-03 06:57:23.941373 sound_source_id-0.0.2/prep-release/
--rw-rwxr--   0 sam       (1000) extdrive  (1777)        1 2023-06-03 06:57:00.000000 sound_source_id-0.0.2/prep-release/minor_minor_number.txt
--rwxrwxr-x   0 sam       (1000) extdrive  (1777)      178 2023-05-30 15:49:16.000000 sound_source_id-0.0.2/prep-release/mkupdate_pyqt5.sh
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)      542 2023-06-01 16:37:56.000000 sound_source_id-0.0.2/prep-release/mkupdate_pyqt6.sh
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     2669 2023-06-03 06:30:00.000000 sound_source_id-0.0.2/prep-release/release.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)      473 2023-06-01 16:03:08.000000 sound_source_id-0.0.2/prep-release/sound_source_id.pro
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    19141 2023-06-02 05:26:04.000000 sound_source_id-0.0.2/prep-release/sound_source_id_el.ts
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    19141 2023-06-02 05:26:04.000000 sound_source_id-0.0.2/prep-release/sound_source_id_en_GB.ts
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    19141 2023-06-02 05:26:04.000000 sound_source_id-0.0.2/prep-release/sound_source_id_en_US.ts
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    19141 2023-06-02 05:26:04.000000 sound_source_id-0.0.2/prep-release/sound_source_id_es.ts
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    19121 2023-06-02 05:26:04.000000 sound_source_id-0.0.2/prep-release/sound_source_id_fr.ts
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    19146 2023-06-02 05:26:04.000000 sound_source_id-0.0.2/prep-release/sound_source_id_it.ts
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      937 2023-05-30 15:51:22.000000 sound_source_id-0.0.2/prep-release/switch_pyqt5.py
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      937 2023-05-30 15:51:35.000000 sound_source_id-0.0.2/prep-release/switch_pyqt6.py
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     1307 2023-06-03 06:57:00.000000 sound_source_id-0.0.2/pyproject.toml
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      821 2023-06-02 05:25:58.000000 sound_source_id-0.0.2/resources.qrc
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       38 2023-06-03 06:57:23.980374 sound_source_id-0.0.2/setup.cfg
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-03 06:57:23.949373 sound_source_id-0.0.2/sound_source_id/
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)        0 2008-10-28 02:30:54.000000 sound_source_id-0.0.2/sound_source_id/__init__.py
--rwxrwxr-x   0 sam       (1000) extdrive  (1777)    42187 2023-06-03 06:42:21.000000 sound_source_id-0.0.2/sound_source_id/__main__.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      107 2023-06-03 06:57:00.000000 sound_source_id-0.0.2/sound_source_id/_version_info.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    16558 2023-06-01 15:19:47.000000 sound_source_id-0.0.2/sound_source_id/audio_manager.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    15283 2023-06-01 15:18:30.000000 sound_source_id-0.0.2/sound_source_id/dialog_edit_phones.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    19749 2023-06-01 15:25:57.000000 sound_source_id-0.0.2/sound_source_id/dialog_edit_preferences.py
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-03 06:57:23.954373 sound_source_id-0.0.2/sound_source_id/doc/
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-03 06:57:23.954373 sound_source_id-0.0.2/sound_source_id/doc/Figures/
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    10241 2023-03-14 14:49:17.000000 sound_source_id-0.0.2/sound_source_id/doc/Figures/stim_file.png
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      634 2023-02-23 15:00:48.000000 sound_source_id-0.0.2/sound_source_id/doc/Makefile
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-03 06:57:23.930373 sound_source_id-0.0.2/sound_source_id/doc/_build/
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-03 06:57:23.958373 sound_source_id-0.0.2/sound_source_id/doc/_build/html/
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      230 2023-06-03 06:56:25.000000 sound_source_id-0.0.2/sound_source_id/doc/_build/html/.buildinfo
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-03 06:57:23.959373 sound_source_id-0.0.2/sound_source_id/doc/_build/html/_images/
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    17653 2023-02-23 14:52:34.000000 sound_source_id-0.0.2/sound_source_id/doc/_build/html/_images/pyloc_screenshot.png
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    17653 2023-02-23 14:52:34.000000 sound_source_id-0.0.2/sound_source_id/doc/_build/html/_images/sound_source_id_screenshot.png
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    10241 2023-03-14 14:49:17.000000 sound_source_id-0.0.2/sound_source_id/doc/_build/html/_images/stim_file.png
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-03 06:57:23.960373 sound_source_id-0.0.2/sound_source_id/doc/_build/html/_sources/
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     2660 2023-03-14 16:33:42.000000 sound_source_id-0.0.2/sound_source_id/doc/_build/html/_sources/experiment_setup.rst.txt
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      506 2023-06-03 06:24:20.000000 sound_source_id-0.0.2/sound_source_id/doc/_build/html/_sources/index.rst.txt
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     1499 2023-06-03 06:56:22.000000 sound_source_id-0.0.2/sound_source_id/doc/_build/html/_sources/installation.rst.txt
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      436 2023-06-03 06:22:36.000000 sound_source_id-0.0.2/sound_source_id/doc/_build/html/_sources/intro.rst.txt
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-03 06:57:23.966374 sound_source_id-0.0.2/sound_source_id/doc/_build/html/_static/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4418 2023-03-29 08:31:27.000000 sound_source_id-0.0.2/sound_source_id/doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    11185 2023-06-03 06:56:25.000000 sound_source_id-0.0.2/sound_source_id/doc/_build/html/_static/alabaster.css
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    14810 2023-06-03 06:56:25.000000 sound_source_id-0.0.2/sound_source_id/doc/_build/html/_static/basic.css
--rw-rwxr--   0 sam       (1000) extdrive  (1777)       42 2016-05-05 22:56:17.000000 sound_source_id-0.0.2/sound_source_id/doc/_build/html/_static/custom.css
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     4472 2023-03-29 08:31:27.000000 sound_source_id-0.0.2/sound_source_id/doc/_build/html/_static/doctools.js
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      420 2023-06-03 06:56:25.000000 sound_source_id-0.0.2/sound_source_id/doc/_build/html/_static/documentation_options.js
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      286 2021-01-01 06:53:29.000000 sound_source_id-0.0.2/sound_source_id/doc/_build/html/_static/file.png
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4787 2021-06-13 20:25:40.000000 sound_source_id-0.0.2/sound_source_id/doc/_build/html/_static/forkme_right_darkblue_121621.png
--rw-rwxr--   0 sam       (1000) extdrive  (1777)   289782 2022-08-29 08:27:59.000000 sound_source_id-0.0.2/sound_source_id/doc/_build/html/_static/jquery.js
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     4758 2023-06-03 06:56:25.000000 sound_source_id-0.0.2/sound_source_id/doc/_build/html/_static/language_data.js
--rw-rwxr--   0 sam       (1000) extdrive  (1777)       90 2021-01-01 06:53:29.000000 sound_source_id-0.0.2/sound_source_id/doc/_build/html/_static/minus.png
--rw-rwxr--   0 sam       (1000) extdrive  (1777)       90 2021-01-01 06:53:29.000000 sound_source_id-0.0.2/sound_source_id/doc/_build/html/_static/plus.png
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     5327 2023-06-03 06:56:25.000000 sound_source_id-0.0.2/sound_source_id/doc/_build/html/_static/pygments.css
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    18747 2023-03-29 08:31:27.000000 sound_source_id-0.0.2/sound_source_id/doc/_build/html/_static/searchtools.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     5097 2023-03-29 08:31:27.000000 sound_source_id-0.0.2/sound_source_id/doc/_build/html/_static/sphinx_highlight.js
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    68416 2022-06-02 12:39:04.000000 sound_source_id-0.0.2/sound_source_id/doc/_build/html/_static/underscore.js
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    10202 2023-06-03 06:55:21.000000 sound_source_id-0.0.2/sound_source_id/doc/_build/html/experiment_setup.html
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     3137 2023-06-03 06:56:25.000000 sound_source_id-0.0.2/sound_source_id/doc/_build/html/genindex.html
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     4912 2023-06-03 06:56:25.000000 sound_source_id-0.0.2/sound_source_id/doc/_build/html/index.html
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     6331 2023-06-03 06:56:25.000000 sound_source_id-0.0.2/sound_source_id/doc/_build/html/installation.html
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     4827 2023-06-03 06:55:21.000000 sound_source_id-0.0.2/sound_source_id/doc/_build/html/intro.html
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      430 2023-06-03 06:56:25.000000 sound_source_id-0.0.2/sound_source_id/doc/_build/html/objects.inv
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     3414 2023-06-03 06:56:25.000000 sound_source_id-0.0.2/sound_source_id/doc/_build/html/search.html
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4401 2023-06-03 06:56:25.000000 sound_source_id-0.0.2/sound_source_id/doc/_build/html/searchindex.js
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-03 06:57:23.966374 sound_source_id-0.0.2/sound_source_id/doc/_build/latex/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)   169508 2023-06-03 06:56:27.000000 sound_source_id-0.0.2/sound_source_id/doc/_build/latex/sound_source_id.pdf
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     2165 2023-06-03 06:57:00.000000 sound_source_id-0.0.2/sound_source_id/doc/conf.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     2660 2023-03-14 16:33:42.000000 sound_source_id-0.0.2/sound_source_id/doc/experiment_setup.rst
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      506 2023-06-03 06:24:20.000000 sound_source_id-0.0.2/sound_source_id/doc/index.rst
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     1499 2023-06-03 06:56:22.000000 sound_source_id-0.0.2/sound_source_id/doc/installation.rst
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      436 2023-06-03 06:22:36.000000 sound_source_id-0.0.2/sound_source_id/doc/intro.rst
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      795 2023-02-23 15:00:48.000000 sound_source_id-0.0.2/sound_source_id/doc/make.bat
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)      104 2023-02-23 14:58:04.000000 sound_source_id-0.0.2/sound_source_id/doc/mkdoc.sh
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    10073 2023-06-01 16:54:43.000000 sound_source_id-0.0.2/sound_source_id/global_parameters.py
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-03 06:57:23.967373 sound_source_id-0.0.2/sound_source_id/icons/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    21662 2023-06-02 05:27:00.000000 sound_source_id-0.0.2/sound_source_id/icons/point-right.ico
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-03 06:57:23.968374 sound_source_id-0.0.2/sound_source_id/prm_files/
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-03 06:57:23.979374 sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise1.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise10.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise11.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise12.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise13.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise14.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise15.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise16.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise17.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise18.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise19.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise2.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise20.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise21.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise22.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise23.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise24.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise25.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise26.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise27.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise28.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise29.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise3.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise30.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise4.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise5.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise6.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise7.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise8.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise9.wav
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      321 2023-03-02 09:58:54.000000 sound_source_id-0.0.2/sound_source_id/prm_files/prm.txt
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      181 2023-03-26 08:03:59.000000 sound_source_id-0.0.2/sound_source_id/prm_files/prm_2_speak.txt
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     1183 2023-03-13 14:52:25.000000 sound_source_id-0.0.2/sound_source_id/prm_files/stim_list.csv
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      425 2023-03-26 08:49:05.000000 sound_source_id-0.0.2/sound_source_id/prm_files/stim_list_2_speak.csv
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      824 2023-06-02 05:57:59.000000 sound_source_id-0.0.2/sound_source_id/pyqtver.py
--rw-rw-r--   0 sam       (1000) extdrive  (1777)  4024537 2023-06-02 05:26:04.000000 sound_source_id-0.0.2/sound_source_id/qrc_resources.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)      996 2015-09-04 15:46:24.000000 sound_source_id-0.0.2/sound_source_id/scipy_wav.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)   171895 2020-04-12 10:56:23.000000 sound_source_id-0.0.2/sound_source_id/sndlib.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      183 2023-03-13 15:52:45.000000 sound_source_id-0.0.2/sound_source_id/utils.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    10419 2023-05-09 08:07:18.000000 sound_source_id-0.0.2/sound_source_id/wavpy.py
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     2953 2023-05-08 10:12:35.000000 sound_source_id-0.0.2/sound_source_id/wavpy_sndf.py
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-03 06:57:23.951373 sound_source_id-0.0.2/sound_source_id.egg-info/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    41505 2023-06-03 06:57:23.000000 sound_source_id-0.0.2/sound_source_id.egg-info/PKG-INFO
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     5171 2023-06-03 06:57:23.000000 sound_source_id-0.0.2/sound_source_id.egg-info/SOURCES.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)        1 2023-06-03 06:57:23.000000 sound_source_id-0.0.2/sound_source_id.egg-info/dependency_links.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       62 2023-06-03 06:57:23.000000 sound_source_id-0.0.2/sound_source_id.egg-info/entry_points.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       86 2023-06-03 06:57:23.000000 sound_source_id-0.0.2/sound_source_id.egg-info/requires.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       16 2023-06-03 06:57:23.000000 sound_source_id-0.0.2/sound_source_id.egg-info/top_level.txt
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:17:45.909276 sound_source_id-0.0.3/
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    35147 2010-06-04 09:15:48.000000 sound_source_id-0.0.3/COPYING.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      408 2023-06-03 06:35:59.000000 sound_source_id-0.0.3/MANIFEST.in
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    41505 2023-06-05 08:17:45.908276 sound_source_id-0.0.3/PKG-INFO
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)       46 2023-02-28 10:13:11.000000 sound_source_id-0.0.3/README.md
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:17:45.869275 sound_source_id-0.0.3/icons/
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    13103 2012-08-13 00:56:29.000000 sound_source_id-0.0.3/icons/audio-headphones.svgz
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     7056 2012-08-13 00:59:09.000000 sound_source_id-0.0.3/icons/help-about.svgz
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)   679822 2015-11-04 09:40:24.000000 sound_source_id-0.0.3/icons/help-contents.svgz
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)   255671 2012-08-13 01:04:33.000000 sound_source_id-0.0.3/icons/help-contextual.svgz
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     7408 2023-06-02 05:19:07.000000 sound_source_id-0.0.3/icons/point-left.svg
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4761 2023-06-02 05:19:10.000000 sound_source_id-0.0.3/icons/point-right.svg
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    10662 2012-08-13 00:56:47.000000 sound_source_id-0.0.3/icons/preferences-other.svgz
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:17:45.870275 sound_source_id-0.0.3/make_noises/
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     2120 2023-05-31 05:23:34.000000 sound_source_id-0.0.3/make_noises/make_pink_noises.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)   171895 2020-04-12 10:56:23.000000 sound_source_id-0.0.3/make_noises/sndlib.py
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:17:45.874275 sound_source_id-0.0.3/prep-release/
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)        1 2023-06-05 08:16:57.000000 sound_source_id-0.0.3/prep-release/minor_minor_number.txt
+-rwxrwxr-x   0 sam       (1000) extdrive  (1777)      178 2023-05-30 15:49:16.000000 sound_source_id-0.0.3/prep-release/mkupdate_pyqt5.sh
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)      542 2023-06-01 16:37:56.000000 sound_source_id-0.0.3/prep-release/mkupdate_pyqt6.sh
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     2669 2023-06-03 06:30:00.000000 sound_source_id-0.0.3/prep-release/release.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)      473 2023-06-01 16:03:08.000000 sound_source_id-0.0.3/prep-release/sound_source_id.pro
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    19141 2023-06-02 05:26:04.000000 sound_source_id-0.0.3/prep-release/sound_source_id_el.ts
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    19141 2023-06-02 05:26:04.000000 sound_source_id-0.0.3/prep-release/sound_source_id_en_GB.ts
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    19141 2023-06-02 05:26:04.000000 sound_source_id-0.0.3/prep-release/sound_source_id_en_US.ts
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    19141 2023-06-02 05:26:04.000000 sound_source_id-0.0.3/prep-release/sound_source_id_es.ts
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    19121 2023-06-02 05:26:04.000000 sound_source_id-0.0.3/prep-release/sound_source_id_fr.ts
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    19146 2023-06-02 05:26:04.000000 sound_source_id-0.0.3/prep-release/sound_source_id_it.ts
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      937 2023-05-30 15:51:22.000000 sound_source_id-0.0.3/prep-release/switch_pyqt5.py
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      937 2023-05-30 15:51:35.000000 sound_source_id-0.0.3/prep-release/switch_pyqt6.py
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     1307 2023-06-05 08:16:57.000000 sound_source_id-0.0.3/pyproject.toml
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      821 2023-06-02 05:25:58.000000 sound_source_id-0.0.3/resources.qrc
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       38 2023-06-05 08:17:45.909276 sound_source_id-0.0.3/setup.cfg
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:17:45.881275 sound_source_id-0.0.3/sound_source_id/
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)        0 2008-10-28 02:30:54.000000 sound_source_id-0.0.3/sound_source_id/__init__.py
+-rwxrwxr-x   0 sam       (1000) extdrive  (1777)    42187 2023-06-03 06:42:21.000000 sound_source_id-0.0.3/sound_source_id/__main__.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      107 2023-06-05 08:16:57.000000 sound_source_id-0.0.3/sound_source_id/_version_info.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    16558 2023-06-01 15:19:47.000000 sound_source_id-0.0.3/sound_source_id/audio_manager.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    15283 2023-06-01 15:18:30.000000 sound_source_id-0.0.3/sound_source_id/dialog_edit_phones.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    19749 2023-06-01 15:25:57.000000 sound_source_id-0.0.3/sound_source_id/dialog_edit_preferences.py
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:17:45.886275 sound_source_id-0.0.3/sound_source_id/doc/
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:17:45.886275 sound_source_id-0.0.3/sound_source_id/doc/Figures/
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    10241 2023-03-14 14:49:17.000000 sound_source_id-0.0.3/sound_source_id/doc/Figures/stim_file.png
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      634 2023-02-23 15:00:48.000000 sound_source_id-0.0.3/sound_source_id/doc/Makefile
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:17:45.864275 sound_source_id-0.0.3/sound_source_id/doc/_build/
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:17:45.889275 sound_source_id-0.0.3/sound_source_id/doc/_build/html/
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      230 2023-06-05 08:17:25.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/.buildinfo
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:17:45.890275 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_images/
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    17653 2023-02-23 14:52:34.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_images/pyloc_screenshot.png
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    17653 2023-02-23 14:52:34.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_images/sound_source_id_screenshot.png
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    10241 2023-03-14 14:49:17.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_images/stim_file.png
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:17:45.891275 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_sources/
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     2670 2023-06-05 07:43:19.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_sources/experiment_setup.rst.txt
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      506 2023-06-03 06:24:20.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_sources/index.rst.txt
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     1499 2023-06-03 06:56:22.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_sources/installation.rst.txt
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      436 2023-06-03 06:22:36.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_sources/intro.rst.txt
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:17:45.896276 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4418 2023-03-29 08:31:27.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    11185 2023-06-05 07:41:46.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/alabaster.css
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    14810 2023-06-05 08:17:25.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/basic.css
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)       42 2016-05-05 22:56:17.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/custom.css
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     4472 2023-03-29 08:31:27.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/doctools.js
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      420 2023-06-05 08:17:25.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/documentation_options.js
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      286 2021-01-01 06:53:29.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/file.png
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4787 2021-06-13 20:25:40.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/forkme_right_darkblue_121621.png
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)   289782 2022-08-29 08:27:59.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/jquery.js
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     4758 2023-06-05 08:17:25.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/language_data.js
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)       90 2021-01-01 06:53:29.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/minus.png
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)       90 2021-01-01 06:53:29.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/plus.png
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     4819 2023-06-05 08:17:25.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/pygments.css
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    18747 2023-03-29 08:31:27.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/searchtools.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     5097 2023-03-29 08:31:27.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/sphinx_highlight.js
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    68416 2022-06-02 12:39:04.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/underscore.js
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    11129 2023-06-05 08:17:25.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/experiment_setup.html
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     3866 2023-06-05 08:17:25.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/genindex.html
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     5780 2023-06-05 08:17:25.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/index.html
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     7274 2023-06-05 08:17:25.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/installation.html
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     5924 2023-06-05 08:17:25.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/intro.html
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      430 2023-06-05 08:17:25.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/objects.inv
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     4265 2023-06-05 08:17:25.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/search.html
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4407 2023-06-05 08:17:25.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/html/searchindex.js
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:17:45.896276 sound_source_id-0.0.3/sound_source_id/doc/_build/latex/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)   169379 2023-06-05 08:17:28.000000 sound_source_id-0.0.3/sound_source_id/doc/_build/latex/sound_source_id.pdf
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     2172 2023-06-05 08:16:57.000000 sound_source_id-0.0.3/sound_source_id/doc/conf.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     2670 2023-06-05 07:43:19.000000 sound_source_id-0.0.3/sound_source_id/doc/experiment_setup.rst
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      506 2023-06-03 06:24:20.000000 sound_source_id-0.0.3/sound_source_id/doc/index.rst
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     1499 2023-06-03 06:56:22.000000 sound_source_id-0.0.3/sound_source_id/doc/installation.rst
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      436 2023-06-03 06:22:36.000000 sound_source_id-0.0.3/sound_source_id/doc/intro.rst
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      795 2023-02-23 15:00:48.000000 sound_source_id-0.0.3/sound_source_id/doc/make.bat
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)      104 2023-02-23 14:58:04.000000 sound_source_id-0.0.3/sound_source_id/doc/mkdoc.sh
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    10073 2023-06-01 16:54:43.000000 sound_source_id-0.0.3/sound_source_id/global_parameters.py
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:17:45.897276 sound_source_id-0.0.3/sound_source_id/icons/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    21662 2023-06-02 05:27:00.000000 sound_source_id-0.0.3/sound_source_id/icons/point-right.ico
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:17:45.898275 sound_source_id-0.0.3/sound_source_id/prm_files/
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:17:45.908276 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise1.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise10.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise11.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise12.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise13.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise14.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise15.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise16.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise17.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise18.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise19.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise2.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise20.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise21.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise22.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise23.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise24.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise25.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise26.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise27.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise28.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise29.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise3.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise30.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise4.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise5.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise6.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise7.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise8.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    28844 2023-03-26 08:39:28.000000 sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise9.wav
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      321 2023-03-02 09:58:54.000000 sound_source_id-0.0.3/sound_source_id/prm_files/prm.txt
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      181 2023-03-26 08:03:59.000000 sound_source_id-0.0.3/sound_source_id/prm_files/prm_2_speak.txt
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     1183 2023-03-13 14:52:25.000000 sound_source_id-0.0.3/sound_source_id/prm_files/stim_list.csv
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      425 2023-03-26 08:49:05.000000 sound_source_id-0.0.3/sound_source_id/prm_files/stim_list_2_speak.csv
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      824 2023-06-02 05:57:59.000000 sound_source_id-0.0.3/sound_source_id/pyqtver.py
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)  4024537 2023-06-02 05:26:04.000000 sound_source_id-0.0.3/sound_source_id/qrc_resources.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)      996 2015-09-04 15:46:24.000000 sound_source_id-0.0.3/sound_source_id/scipy_wav.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)   171895 2020-04-12 10:56:23.000000 sound_source_id-0.0.3/sound_source_id/sndlib.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      183 2023-03-13 15:52:45.000000 sound_source_id-0.0.3/sound_source_id/utils.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    10419 2023-05-09 08:07:18.000000 sound_source_id-0.0.3/sound_source_id/wavpy.py
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     2953 2023-05-08 10:12:35.000000 sound_source_id-0.0.3/sound_source_id/wavpy_sndf.py
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:17:45.883275 sound_source_id-0.0.3/sound_source_id.egg-info/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    41505 2023-06-05 08:17:45.000000 sound_source_id-0.0.3/sound_source_id.egg-info/PKG-INFO
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     5171 2023-06-05 08:17:45.000000 sound_source_id-0.0.3/sound_source_id.egg-info/SOURCES.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)        1 2023-06-05 08:17:45.000000 sound_source_id-0.0.3/sound_source_id.egg-info/dependency_links.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       62 2023-06-05 08:17:45.000000 sound_source_id-0.0.3/sound_source_id.egg-info/entry_points.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       86 2023-06-05 08:17:45.000000 sound_source_id-0.0.3/sound_source_id.egg-info/requires.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       16 2023-06-05 08:17:45.000000 sound_source_id-0.0.3/sound_source_id.egg-info/top_level.txt
```

### Comparing `sound_source_id-0.0.2/COPYING.txt` & `sound_source_id-0.0.3/COPYING.txt`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/PKG-INFO` & `sound_source_id-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sound_source_id
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python application for running sound localization experiments
 Author-email: Samuele Carcagno <sam.carcagno@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `sound_source_id-0.0.2/icons/audio-headphones.svgz` & `sound_source_id-0.0.3/icons/audio-headphones.svgz`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/icons/help-about.svgz` & `sound_source_id-0.0.3/icons/help-about.svgz`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/icons/help-contents.svgz` & `sound_source_id-0.0.3/icons/help-contents.svgz`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/icons/help-contextual.svgz` & `sound_source_id-0.0.3/icons/help-contextual.svgz`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/icons/point-left.svg` & `sound_source_id-0.0.3/icons/point-left.svg`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/icons/point-right.svg` & `sound_source_id-0.0.3/icons/point-right.svg`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/icons/preferences-other.svgz` & `sound_source_id-0.0.3/icons/preferences-other.svgz`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/make_noises/make_pink_noises.py` & `sound_source_id-0.0.3/make_noises/make_pink_noises.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/make_noises/sndlib.py` & `sound_source_id-0.0.3/make_noises/sndlib.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/prep-release/mkupdate_pyqt6.sh` & `sound_source_id-0.0.3/prep-release/mkupdate_pyqt6.sh`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/prep-release/release.py` & `sound_source_id-0.0.3/prep-release/release.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/prep-release/sound_source_id_el.ts` & `sound_source_id-0.0.3/prep-release/sound_source_id_el.ts`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/prep-release/sound_source_id_en_GB.ts` & `sound_source_id-0.0.3/prep-release/sound_source_id_en_GB.ts`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/prep-release/sound_source_id_en_US.ts` & `sound_source_id-0.0.3/prep-release/sound_source_id_en_US.ts`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/prep-release/sound_source_id_es.ts` & `sound_source_id-0.0.3/prep-release/sound_source_id_es.ts`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/prep-release/sound_source_id_fr.ts` & `sound_source_id-0.0.3/prep-release/sound_source_id_fr.ts`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/prep-release/sound_source_id_it.ts` & `sound_source_id-0.0.3/prep-release/sound_source_id_it.ts`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/prep-release/switch_pyqt5.py` & `sound_source_id-0.0.3/prep-release/switch_pyqt5.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/prep-release/switch_pyqt6.py` & `sound_source_id-0.0.3/prep-release/switch_pyqt6.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/pyproject.toml` & `sound_source_id-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sound_source_id"
-    version="0.0.2"
+    version="0.0.3"
 
 authors = [
   { name="Samuele Carcagno", email="sam.carcagno@gmail.com" },
 ]
 description = "Python application for running sound localization experiments"
 license = {file = "COPYING.txt"}
 readme = "README.md"
```

### Comparing `sound_source_id-0.0.2/resources.qrc` & `sound_source_id-0.0.3/resources.qrc`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/__main__.py` & `sound_source_id-0.0.3/sound_source_id/__main__.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/audio_manager.py` & `sound_source_id-0.0.3/sound_source_id/audio_manager.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/dialog_edit_phones.py` & `sound_source_id-0.0.3/sound_source_id/dialog_edit_phones.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/dialog_edit_preferences.py` & `sound_source_id-0.0.3/sound_source_id/dialog_edit_preferences.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/doc/Figures/stim_file.png` & `sound_source_id-0.0.3/sound_source_id/doc/Figures/stim_file.png`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/doc/Makefile` & `sound_source_id-0.0.3/sound_source_id/doc/Makefile`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/doc/_build/html/_images/pyloc_screenshot.png` & `sound_source_id-0.0.3/sound_source_id/doc/_build/html/_images/pyloc_screenshot.png`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/doc/_build/html/_images/sound_source_id_screenshot.png` & `sound_source_id-0.0.3/sound_source_id/doc/_build/html/_images/sound_source_id_screenshot.png`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/doc/_build/html/_images/stim_file.png` & `sound_source_id-0.0.3/sound_source_id/doc/_build/html/_images/stim_file.png`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/doc/_build/html/_sources/experiment_setup.rst.txt` & `sound_source_id-0.0.3/sound_source_id/doc/_build/html/_sources/experiment_setup.rst.txt`

 * *Files 4% similar despite different names*

```diff
@@ -45,10 +45,10 @@
    Example stimulation file.
 
 Each row of the file represents a trial. Stimulation files contain the following columns:
 
   - `angle`: the angle at which the sound will be presented (stimuli will be sent to the corresponding soundcard channel as specified in the parameters file)
   - `sound_file`: the path (relative or absolute) to the WAV file to be played
   - `condition`: an optional label specifying the experimental condition
-  - `level`: the `base` sound level (in dB SPL) at which the sound will be presented (this assumes that `pyloc` has been correctly calibrated)
+  - `level`: the `base` sound level (in dB SPL) at which the sound will be presented (this assumes that `sound_source_id` has been correctly calibrated)
   - `roving`: a level rove, actual sound level will be euqual to the base level plus a value drawn from a random uniform distribution between +/- the roving level
   - `feedback`: if `true`, feedback will be given to the listener at the end of each trial
```

### Comparing `sound_source_id-0.0.2/sound_source_id/doc/_build/html/_sources/installation.rst.txt` & `sound_source_id-0.0.3/sound_source_id/doc/_build/html/_sources/installation.rst.txt`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js` & `sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/doc/_build/html/_static/alabaster.css` & `sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/doc/_build/html/_static/basic.css` & `sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/doc/_build/html/_static/doctools.js` & `sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/doc/_build/html/_static/forkme_right_darkblue_121621.png` & `sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/forkme_right_darkblue_121621.png`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/doc/_build/html/_static/jquery.js` & `sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/doc/_build/html/_static/language_data.js` & `sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/doc/_build/html/_static/pygments.css` & `sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/pygments.css`

 * *Files 16% similar despite different names*

```diff
@@ -1,83 +1,74 @@
 pre { line-height: 125%; }
 td.linenos .normal { color: inherit; background-color: transparent; padding-left: 5px; padding-right: 5px; }
 span.linenos { color: inherit; background-color: transparent; padding-left: 5px; padding-right: 5px; }
 td.linenos .special { color: #000000; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
 span.linenos.special { color: #000000; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
 .highlight .hll { background-color: #ffffcc }
 .highlight { background: #f8f8f8; }
-.highlight .c { color: #8f5902; font-style: italic } /* Comment */
-.highlight .err { color: #a40000; border: 1px solid #ef2929 } /* Error */
-.highlight .g { color: #000000 } /* Generic */
-.highlight .k { color: #004461; font-weight: bold } /* Keyword */
-.highlight .l { color: #000000 } /* Literal */
-.highlight .n { color: #000000 } /* Name */
-.highlight .o { color: #582800 } /* Operator */
-.highlight .x { color: #000000 } /* Other */
-.highlight .p { color: #000000; font-weight: bold } /* Punctuation */
-.highlight .ch { color: #8f5902; font-style: italic } /* Comment.Hashbang */
-.highlight .cm { color: #8f5902; font-style: italic } /* Comment.Multiline */
-.highlight .cp { color: #8f5902 } /* Comment.Preproc */
-.highlight .cpf { color: #8f5902; font-style: italic } /* Comment.PreprocFile */
-.highlight .c1 { color: #8f5902; font-style: italic } /* Comment.Single */
-.highlight .cs { color: #8f5902; font-style: italic } /* Comment.Special */
-.highlight .gd { color: #a40000 } /* Generic.Deleted */
-.highlight .ge { color: #000000; font-style: italic } /* Generic.Emph */
-.highlight .gr { color: #ef2929 } /* Generic.Error */
+.highlight .c { color: #3D7B7B; font-style: italic } /* Comment */
+.highlight .err { border: 1px solid #FF0000 } /* Error */
+.highlight .k { color: #008000; font-weight: bold } /* Keyword */
+.highlight .o { color: #666666 } /* Operator */
+.highlight .ch { color: #3D7B7B; font-style: italic } /* Comment.Hashbang */
+.highlight .cm { color: #3D7B7B; font-style: italic } /* Comment.Multiline */
+.highlight .cp { color: #9C6500 } /* Comment.Preproc */
+.highlight .cpf { color: #3D7B7B; font-style: italic } /* Comment.PreprocFile */
+.highlight .c1 { color: #3D7B7B; font-style: italic } /* Comment.Single */
+.highlight .cs { color: #3D7B7B; font-style: italic } /* Comment.Special */
+.highlight .gd { color: #A00000 } /* Generic.Deleted */
+.highlight .ge { font-style: italic } /* Generic.Emph */
+.highlight .gr { color: #E40000 } /* Generic.Error */
 .highlight .gh { color: #000080; font-weight: bold } /* Generic.Heading */
-.highlight .gi { color: #00A000 } /* Generic.Inserted */
-.highlight .go { color: #888888 } /* Generic.Output */
-.highlight .gp { color: #745334 } /* Generic.Prompt */
-.highlight .gs { color: #000000; font-weight: bold } /* Generic.Strong */
+.highlight .gi { color: #008400 } /* Generic.Inserted */
+.highlight .go { color: #717171 } /* Generic.Output */
+.highlight .gp { color: #000080; font-weight: bold } /* Generic.Prompt */
+.highlight .gs { font-weight: bold } /* Generic.Strong */
 .highlight .gu { color: #800080; font-weight: bold } /* Generic.Subheading */
-.highlight .gt { color: #a40000; font-weight: bold } /* Generic.Traceback */
-.highlight .kc { color: #004461; font-weight: bold } /* Keyword.Constant */
-.highlight .kd { color: #004461; font-weight: bold } /* Keyword.Declaration */
-.highlight .kn { color: #004461; font-weight: bold } /* Keyword.Namespace */
-.highlight .kp { color: #004461; font-weight: bold } /* Keyword.Pseudo */
-.highlight .kr { color: #004461; font-weight: bold } /* Keyword.Reserved */
-.highlight .kt { color: #004461; font-weight: bold } /* Keyword.Type */
-.highlight .ld { color: #000000 } /* Literal.Date */
-.highlight .m { color: #990000 } /* Literal.Number */
-.highlight .s { color: #4e9a06 } /* Literal.String */
-.highlight .na { color: #c4a000 } /* Name.Attribute */
-.highlight .nb { color: #004461 } /* Name.Builtin */
-.highlight .nc { color: #000000 } /* Name.Class */
-.highlight .no { color: #000000 } /* Name.Constant */
-.highlight .nd { color: #888888 } /* Name.Decorator */
-.highlight .ni { color: #ce5c00 } /* Name.Entity */
-.highlight .ne { color: #cc0000; font-weight: bold } /* Name.Exception */
-.highlight .nf { color: #000000 } /* Name.Function */
-.highlight .nl { color: #f57900 } /* Name.Label */
-.highlight .nn { color: #000000 } /* Name.Namespace */
-.highlight .nx { color: #000000 } /* Name.Other */
-.highlight .py { color: #000000 } /* Name.Property */
-.highlight .nt { color: #004461; font-weight: bold } /* Name.Tag */
-.highlight .nv { color: #000000 } /* Name.Variable */
-.highlight .ow { color: #004461; font-weight: bold } /* Operator.Word */
-.highlight .pm { color: #000000; font-weight: bold } /* Punctuation.Marker */
-.highlight .w { color: #f8f8f8; text-decoration: underline } /* Text.Whitespace */
-.highlight .mb { color: #990000 } /* Literal.Number.Bin */
-.highlight .mf { color: #990000 } /* Literal.Number.Float */
-.highlight .mh { color: #990000 } /* Literal.Number.Hex */
-.highlight .mi { color: #990000 } /* Literal.Number.Integer */
-.highlight .mo { color: #990000 } /* Literal.Number.Oct */
-.highlight .sa { color: #4e9a06 } /* Literal.String.Affix */
-.highlight .sb { color: #4e9a06 } /* Literal.String.Backtick */
-.highlight .sc { color: #4e9a06 } /* Literal.String.Char */
-.highlight .dl { color: #4e9a06 } /* Literal.String.Delimiter */
-.highlight .sd { color: #8f5902; font-style: italic } /* Literal.String.Doc */
-.highlight .s2 { color: #4e9a06 } /* Literal.String.Double */
-.highlight .se { color: #4e9a06 } /* Literal.String.Escape */
-.highlight .sh { color: #4e9a06 } /* Literal.String.Heredoc */
-.highlight .si { color: #4e9a06 } /* Literal.String.Interpol */
-.highlight .sx { color: #4e9a06 } /* Literal.String.Other */
-.highlight .sr { color: #4e9a06 } /* Literal.String.Regex */
-.highlight .s1 { color: #4e9a06 } /* Literal.String.Single */
-.highlight .ss { color: #4e9a06 } /* Literal.String.Symbol */
-.highlight .bp { color: #3465a4 } /* Name.Builtin.Pseudo */
-.highlight .fm { color: #000000 } /* Name.Function.Magic */
-.highlight .vc { color: #000000 } /* Name.Variable.Class */
-.highlight .vg { color: #000000 } /* Name.Variable.Global */
-.highlight .vi { color: #000000 } /* Name.Variable.Instance */
-.highlight .vm { color: #000000 } /* Name.Variable.Magic */
-.highlight .il { color: #990000 } /* Literal.Number.Integer.Long */
+.highlight .gt { color: #0044DD } /* Generic.Traceback */
+.highlight .kc { color: #008000; font-weight: bold } /* Keyword.Constant */
+.highlight .kd { color: #008000; font-weight: bold } /* Keyword.Declaration */
+.highlight .kn { color: #008000; font-weight: bold } /* Keyword.Namespace */
+.highlight .kp { color: #008000 } /* Keyword.Pseudo */
+.highlight .kr { color: #008000; font-weight: bold } /* Keyword.Reserved */
+.highlight .kt { color: #B00040 } /* Keyword.Type */
+.highlight .m { color: #666666 } /* Literal.Number */
+.highlight .s { color: #BA2121 } /* Literal.String */
+.highlight .na { color: #687822 } /* Name.Attribute */
+.highlight .nb { color: #008000 } /* Name.Builtin */
+.highlight .nc { color: #0000FF; font-weight: bold } /* Name.Class */
+.highlight .no { color: #880000 } /* Name.Constant */
+.highlight .nd { color: #AA22FF } /* Name.Decorator */
+.highlight .ni { color: #717171; font-weight: bold } /* Name.Entity */
+.highlight .ne { color: #CB3F38; font-weight: bold } /* Name.Exception */
+.highlight .nf { color: #0000FF } /* Name.Function */
+.highlight .nl { color: #767600 } /* Name.Label */
+.highlight .nn { color: #0000FF; font-weight: bold } /* Name.Namespace */
+.highlight .nt { color: #008000; font-weight: bold } /* Name.Tag */
+.highlight .nv { color: #19177C } /* Name.Variable */
+.highlight .ow { color: #AA22FF; font-weight: bold } /* Operator.Word */
+.highlight .w { color: #bbbbbb } /* Text.Whitespace */
+.highlight .mb { color: #666666 } /* Literal.Number.Bin */
+.highlight .mf { color: #666666 } /* Literal.Number.Float */
+.highlight .mh { color: #666666 } /* Literal.Number.Hex */
+.highlight .mi { color: #666666 } /* Literal.Number.Integer */
+.highlight .mo { color: #666666 } /* Literal.Number.Oct */
+.highlight .sa { color: #BA2121 } /* Literal.String.Affix */
+.highlight .sb { color: #BA2121 } /* Literal.String.Backtick */
+.highlight .sc { color: #BA2121 } /* Literal.String.Char */
+.highlight .dl { color: #BA2121 } /* Literal.String.Delimiter */
+.highlight .sd { color: #BA2121; font-style: italic } /* Literal.String.Doc */
+.highlight .s2 { color: #BA2121 } /* Literal.String.Double */
+.highlight .se { color: #AA5D1F; font-weight: bold } /* Literal.String.Escape */
+.highlight .sh { color: #BA2121 } /* Literal.String.Heredoc */
+.highlight .si { color: #A45A77; font-weight: bold } /* Literal.String.Interpol */
+.highlight .sx { color: #008000 } /* Literal.String.Other */
+.highlight .sr { color: #A45A77 } /* Literal.String.Regex */
+.highlight .s1 { color: #BA2121 } /* Literal.String.Single */
+.highlight .ss { color: #19177C } /* Literal.String.Symbol */
+.highlight .bp { color: #008000 } /* Name.Builtin.Pseudo */
+.highlight .fm { color: #0000FF } /* Name.Function.Magic */
+.highlight .vc { color: #19177C } /* Name.Variable.Class */
+.highlight .vg { color: #19177C } /* Name.Variable.Global */
+.highlight .vi { color: #19177C } /* Name.Variable.Instance */
+.highlight .vm { color: #19177C } /* Name.Variable.Magic */
+.highlight .il { color: #666666 } /* Literal.Number.Integer.Long */
```

### Comparing `sound_source_id-0.0.2/sound_source_id/doc/_build/html/_static/searchtools.js` & `sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/doc/_build/html/_static/sphinx_highlight.js` & `sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/doc/_build/html/_static/underscore.js` & `sound_source_id-0.0.3/sound_source_id/doc/_build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/doc/_build/html/experiment_setup.html` & `sound_source_id-0.0.3/sound_source_id/doc/_build/html/experiment_setup.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,85 @@
-
 <!DOCTYPE html>
-
-<html lang="en">
-  <head>
-    <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
-
-    <title>Parameters file &#8212; sound_source_id 0.0.1 documentation</title>
-    <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
-    <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
-    <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
-    <script src="_static/jquery.js"></script>
-    <script src="_static/underscore.js"></script>
-    <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
-    <script src="_static/doctools.js"></script>
-    <script src="_static/sphinx_highlight.js"></script>
+<html class="writer-html5" lang="en" >
+<head>
+  <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
+
+  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
+  <title>Parameters file &mdash; sound_source_id 0.0.3 documentation</title>
+      <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
+      <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
+  
+        <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
+        <script src="_static/jquery.js"></script>
+        <script src="_static/underscore.js"></script>
+        <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
+        <script src="_static/doctools.js"></script>
+        <script src="_static/sphinx_highlight.js"></script>
+    <script src="_static/js/theme.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
-    <link rel="prev" title="Installation" href="installation.html" />
-   
-  <link rel="stylesheet" href="_static/custom.css" type="text/css" />
-  
-  
-  <meta name="viewport" content="width=device-width, initial-scale=0.9, maximum-scale=0.9" />
+    <link rel="prev" title="Installation" href="installation.html" /> 
+</head>
 
-  </head><body>
-  
+<body class="wy-body-for-nav"> 
+  <div class="wy-grid-for-nav">
+    <nav data-toggle="wy-nav-shift" class="wy-nav-side">
+      <div class="wy-side-scroll">
+        <div class="wy-side-nav-search" >
 
-    <div class="document">
-      <div class="documentwrapper">
-        <div class="bodywrapper">
           
+          
+          <a href="index.html" class="icon icon-home">
+            sound_source_id
+          </a>
+              <div class="version">
+                0.0.3
+              </div>
+<div role="search">
+  <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
+    <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
+    <input type="hidden" name="check_keywords" value="yes" />
+    <input type="hidden" name="area" value="default" />
+  </form>
+</div>
+        </div><div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
+              <p class="caption" role="heading"><span class="caption-text">Contents:</span></p>
+<ul class="current">
+<li class="toctree-l1"><a class="reference internal" href="intro.html"><code class="docutils literal notranslate"><span class="pre">sound_source_id</span></code></a></li>
+<li class="toctree-l1"><a class="reference internal" href="installation.html">Installation</a></li>
+<li class="toctree-l1 current"><a class="current reference internal" href="#">Parameters file</a></li>
+<li class="toctree-l1"><a class="reference internal" href="#stimulation-file">Stimulation file</a></li>
+</ul>
+
+        </div>
+      </div>
+    </nav>
 
-          <div class="body" role="main">
-            
+    <section data-toggle="wy-nav-shift" class="wy-nav-content-wrap"><nav class="wy-nav-top" aria-label="Mobile navigation menu" >
+          <i data-toggle="wy-nav-top" class="fa fa-bars"></i>
+          <a href="index.html">sound_source_id</a>
+      </nav>
+
+      <div class="wy-nav-content">
+        <div class="rst-content">
+          <div role="navigation" aria-label="Page navigation">
+  <ul class="wy-breadcrumbs">
+      <li><a href="index.html" class="icon icon-home" aria-label="Home"></a></li>
+      <li class="breadcrumb-item active">Parameters file</li>
+      <li class="wy-breadcrumbs-aside">
+            <a href="_sources/experiment_setup.rst.txt" rel="nofollow"> View page source</a>
+      </li>
+  </ul>
+  <hr/>
+</div>
+          <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
+           <div itemprop="articleBody">
+             
   <section id="parameters-file">
-<span id="sec-experiment-setup"></span><h1>Parameters file<a class="headerlink" href="#parameters-file" title="Permalink to this heading">¶</a></h1>
+<span id="sec-experiment-setup"></span><h1>Parameters file<a class="headerlink" href="#parameters-file" title="Permalink to this heading"></a></h1>
 <p>The settings for a test are stored in a parameters file (which is a simple text file). An example parameters file is shown below:</p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="n">angles</span> <span class="p">:</span> <span class="o">-</span><span class="mi">70</span><span class="p">,</span> <span class="o">-</span><span class="mi">60</span><span class="p">,</span> <span class="o">-</span><span class="mi">50</span><span class="p">,</span> <span class="o">-</span><span class="mi">40</span><span class="p">,</span> <span class="o">-</span><span class="mi">30</span><span class="p">,</span> <span class="o">-</span><span class="mi">20</span><span class="p">,</span> <span class="o">-</span><span class="mi">10</span><span class="p">,</span> <span class="mi">0</span><span class="p">,</span> <span class="mi">10</span><span class="p">,</span> <span class="mi">20</span><span class="p">,</span> <span class="mi">30</span><span class="p">,</span> <span class="mi">40</span><span class="p">,</span> <span class="mi">50</span><span class="p">,</span> <span class="mi">60</span><span class="p">,</span> <span class="mi">70</span>
 <span class="n">labels</span> <span class="p">:</span> <span class="mi">1</span><span class="p">,</span> <span class="mi">2</span><span class="p">,</span> <span class="mi">3</span><span class="p">,</span> <span class="mi">4</span><span class="p">,</span> <span class="mi">5</span><span class="p">,</span> <span class="mi">6</span><span class="p">,</span> <span class="mi">7</span><span class="p">,</span> <span class="mi">8</span><span class="p">,</span> <span class="mi">9</span><span class="p">,</span> <span class="mi">10</span><span class="p">,</span> <span class="mi">11</span><span class="p">,</span> <span class="mi">12</span><span class="p">,</span> <span class="mi">13</span><span class="p">,</span> <span class="mi">14</span><span class="p">,</span> <span class="mi">15</span>
 <span class="n">channels</span> <span class="p">:</span> <span class="mi">1</span><span class="p">,</span> <span class="mi">2</span><span class="p">,</span> <span class="mi">3</span><span class="p">,</span> <span class="mi">4</span><span class="p">,</span> <span class="mi">5</span><span class="p">,</span> <span class="mi">6</span><span class="p">,</span> <span class="mi">7</span><span class="p">,</span> <span class="mi">8</span><span class="p">,</span> <span class="mi">9</span><span class="p">,</span> <span class="mi">10</span><span class="p">,</span> <span class="mi">11</span><span class="p">,</span> <span class="mi">12</span><span class="p">,</span> <span class="mi">13</span><span class="p">,</span> <span class="mi">14</span><span class="p">,</span> <span class="mi">15</span>
 <span class="n">n_chan</span> <span class="p">:</span> <span class="mi">15</span>
 <span class="n">n_blocks</span> <span class="p">:</span> <span class="mi">1</span>
 <span class="n">stim_list_file</span> <span class="p">:</span> <span class="n">stim_list</span><span class="o">.</span><span class="n">csv</span>
@@ -60,100 +100,59 @@
 <li><p><cite>randomize</cite>: if <cite>true</cite> the stim_list_file will be shuffled before each block repetition</p></li>
 <li><p><cite>demo_stim</cite>: the path to the WAV file to be used for the demo</p></li>
 <li><p><cite>demo_stim_lev</cite>: the sound level (in dB SPL) to be used for the demo</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="stimulation-file">
-<h1>Stimulation file<a class="headerlink" href="#stimulation-file" title="Permalink to this heading">¶</a></h1>
+<h1>Stimulation file<a class="headerlink" href="#stimulation-file" title="Permalink to this heading"></a></h1>
 <p>Stimulation files specify the stimuli that will be played on each trial of the test. Figure <a class="reference internal" href="#fig-stim-file"><span class="std std-ref">Example stimulation file.</span></a> shows an example stimulation file.</p>
 <figure class="align-default" id="id1">
 <span id="fig-stim-file"></span><a class="reference internal image-reference" href="_images/stim_file.png"><img alt="Example stimulation file" src="_images/stim_file.png" style="width: 248.0px; height: 67.5px;" /></a>
 <figcaption>
-<p><span class="caption-text">Example stimulation file.</span><a class="headerlink" href="#id1" title="Permalink to this image">¶</a></p>
+<p><span class="caption-text">Example stimulation file.</span><a class="headerlink" href="#id1" title="Permalink to this image"></a></p>
 </figcaption>
 </figure>
 <p>Each row of the file represents a trial. Stimulation files contain the following columns:</p>
 <blockquote>
 <div><ul class="simple">
 <li><p><cite>angle</cite>: the angle at which the sound will be presented (stimuli will be sent to the corresponding soundcard channel as specified in the parameters file)</p></li>
 <li><p><cite>sound_file</cite>: the path (relative or absolute) to the WAV file to be played</p></li>
 <li><p><cite>condition</cite>: an optional label specifying the experimental condition</p></li>
-<li><p><cite>level</cite>: the <cite>base</cite> sound level (in dB SPL) at which the sound will be presented (this assumes that <cite>pyloc</cite> has been correctly calibrated)</p></li>
+<li><p><cite>level</cite>: the <cite>base</cite> sound level (in dB SPL) at which the sound will be presented (this assumes that <cite>sound_source_id</cite> has been correctly calibrated)</p></li>
 <li><p><cite>roving</cite>: a level rove, actual sound level will be euqual to the base level plus a value drawn from a random uniform distribution between +/- the roving level</p></li>
 <li><p><cite>feedback</cite>: if <cite>true</cite>, feedback will be given to the listener at the end of each trial</p></li>
 </ul>
 </div></blockquote>
 </section>
 
 
+           </div>
           </div>
-          
-        </div>
-      </div>
-      <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
-        <div class="sphinxsidebarwrapper">
-<h1 class="logo"><a href="index.html">sound_source_id</a></h1>
-
-
-
-
-
-
-
-
-<h3>Navigation</h3>
-<p class="caption" role="heading"><span class="caption-text">Contents:</span></p>
-<ul class="current">
-<li class="toctree-l1"><a class="reference internal" href="intro.html"><code class="docutils literal notranslate"><span class="pre">sound_source_id</span></code></a></li>
-<li class="toctree-l1"><a class="reference internal" href="installation.html">Installation</a></li>
-<li class="toctree-l1 current"><a class="current reference internal" href="#">Parameters file</a></li>
-<li class="toctree-l1"><a class="reference internal" href="#stimulation-file">Stimulation file</a></li>
-</ul>
-
-<div class="relations">
-<h3>Related Topics</h3>
-<ul>
-  <li><a href="index.html">Documentation overview</a><ul>
-      <li>Previous: <a href="installation.html" title="previous chapter">Installation</a></li>
-  </ul></li>
-</ul>
-</div>
-<div id="searchbox" style="display: none" role="search">
-  <h3 id="searchlabel">Quick search</h3>
-    <div class="searchformwrapper">
-    <form class="search" action="search.html" method="get">
-      <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
-      <input type="submit" value="Go" />
-    </form>
+          <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
+        <a href="installation.html" class="btn btn-neutral float-left" title="Installation" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
     </div>
-</div>
-<script>document.getElementById('searchbox').style.display = "block"</script>
-
-
-
-
-
 
+  <hr/>
 
+  <div role="contentinfo">
+    <p>&#169; Copyright 2022-2023, Samuele Carcagno.</p>
+  </div>
+
+  Built with <a href="https://www.sphinx-doc.org/">Sphinx</a> using a
+    <a href="https://github.com/readthedocs/sphinx_rtd_theme">theme</a>
+    provided by <a href="https://readthedocs.org">Read the Docs</a>.
+   
 
+</footer>
         </div>
       </div>
-      <div class="clearer"></div>
-    </div>
-    <div class="footer">
-      &copy;2022-2023, Samuele Carcagno.
-      
-      |
-      Powered by <a href="http://sphinx-doc.org/">Sphinx 5.3.0</a>
-      &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.12</a>
-      
-      |
-      <a href="_sources/experiment_setup.rst.txt"
-          rel="nofollow">Page source</a>
-    </div>
-
-    
+    </section>
+  </div>
+  <script>
+      jQuery(function () {
+          SphinxRtdTheme.Navigation.enable(true);
+      });
+  </script> 
 
-    
-  </body>
+</body>
 </html>
```

#### html2text {}

```diff
@@ -1,16 +1,25 @@
 
 
 
 
 
-
-
-
-****** Parameters fileÂ¶ ******
+sound_source_id
+0.0.3
+[q                   ]
+Contents:
+    * sound_source_id
+    * Installation
+    * Parameters_file
+    * Stimulation_file
+   sound_source_id
+    * Parameters file
+    * View_page_source
+===============================================================================
+****** Parameters fileï ******
 The settings for a test are stored in a parameters file (which is a simple text
 file). An example parameters file is shown below:
 angles : -70, -60, -50, -40, -30, -20, -10, 0, 10, 20, 30, 40, 50, 60, 70
 labels : 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15
 channels : 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15
 n_chan : 15
 n_blocks : 1
@@ -33,44 +42,34 @@
            containing the stimulation list (see below)
          * randomize: iftruethe stim_list_file will be shuffled before
            each block repetition
          * demo_stim: the path to the WAV file to be used for the demo
          * demo_stim_lev: the sound level (in dB SPL) to be used for the
            demo
 
-****** Stimulation fileÂ¶ ******
+****** Stimulation fileï ******
 Stimulation files specify the stimuli that will be played on each trial of the
 test. Figure Example_stimulation_file. shows an example stimulation file.
  [Example_stimulation_file]
-Example stimulation file.Â¶
+Example stimulation file.ï
 
 Each row of the file represents a trial. Stimulation files contain the
 following columns:
          * angle: the angle at which the sound will be presented (stimuli
            will be sent to the corresponding soundcard channel as
            specified in the parameters file)
          * sound_file: the path (relative or absolute) to the WAV file to
            be played
          * condition: an optional label specifying the experimental
            condition
          * level: thebasesound level (in dB SPL) at which the sound will
-           be presented (this assumes thatpylochas been correctly
-           calibrated)
+           be presented (this assumes thatsound_source_idhas been
+           correctly calibrated)
          * roving: a level rove, actual sound level will be euqual to the
            base level plus a value drawn from a random uniform
            distribution between +/- the roving level
          * feedback: iftrue, feedback will be given to the listener at the
            end of each trial
-****** sound_source_id ******
-**** Navigation ****
-Contents:
-    * sound_source_id
-    * Installation
-    * Parameters_file
-    * Stimulation_file
-**** Related Topics ****
-    * Documentation_overview
-          o Previous: Installation
-**** Quick search ****
-[q                   ] [Go]
-©2022-2023, Samuele Carcagno. | Powered by Sphinx_5.3.0 & Alabaster_0.7.12 |
-Page_source
+Previous
+===============================================================================
+© Copyright 2022-2023, Samuele Carcagno.
+Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `sound_source_id-0.0.2/sound_source_id/doc/_build/html/index.html` & `sound_source_id-0.0.3/sound_source_id/doc/_build/html/index.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,129 +1,128 @@
-
 <!DOCTYPE html>
-
-<html lang="en">
-  <head>
-    <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
-
-    <title>Welcome to sound_source_id’s documentation! &#8212; sound_source_id 0.0.1 documentation</title>
-    <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
-    <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
-    <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
-    <script src="_static/jquery.js"></script>
-    <script src="_static/underscore.js"></script>
-    <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
-    <script src="_static/doctools.js"></script>
-    <script src="_static/sphinx_highlight.js"></script>
+<html class="writer-html5" lang="en" >
+<head>
+  <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
+
+  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
+  <title>Welcome to sound_source_id’s documentation! &mdash; sound_source_id 0.0.3 documentation</title>
+      <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
+      <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
+  
+        <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
+        <script src="_static/jquery.js"></script>
+        <script src="_static/underscore.js"></script>
+        <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
+        <script src="_static/doctools.js"></script>
+        <script src="_static/sphinx_highlight.js"></script>
+    <script src="_static/js/theme.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
-    <link rel="next" title="sound_source_id" href="intro.html" />
-   
-  <link rel="stylesheet" href="_static/custom.css" type="text/css" />
-  
-  
-  <meta name="viewport" content="width=device-width, initial-scale=0.9, maximum-scale=0.9" />
+    <link rel="next" title="sound_source_id" href="intro.html" /> 
+</head>
 
-  </head><body>
-  
+<body class="wy-body-for-nav"> 
+  <div class="wy-grid-for-nav">
+    <nav data-toggle="wy-nav-shift" class="wy-nav-side">
+      <div class="wy-side-scroll">
+        <div class="wy-side-nav-search" >
 
-    <div class="document">
-      <div class="documentwrapper">
-        <div class="bodywrapper">
           
+          
+          <a href="#" class="icon icon-home">
+            sound_source_id
+          </a>
+              <div class="version">
+                0.0.3
+              </div>
+<div role="search">
+  <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
+    <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
+    <input type="hidden" name="check_keywords" value="yes" />
+    <input type="hidden" name="area" value="default" />
+  </form>
+</div>
+        </div><div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
+              <p class="caption" role="heading"><span class="caption-text">Contents:</span></p>
+<ul>
+<li class="toctree-l1"><a class="reference internal" href="intro.html"><code class="docutils literal notranslate"><span class="pre">sound_source_id</span></code></a></li>
+<li class="toctree-l1"><a class="reference internal" href="installation.html">Installation</a></li>
+<li class="toctree-l1"><a class="reference internal" href="experiment_setup.html">Parameters file</a></li>
+<li class="toctree-l1"><a class="reference internal" href="experiment_setup.html#stimulation-file">Stimulation file</a></li>
+</ul>
 
-          <div class="body" role="main">
-            
+        </div>
+      </div>
+    </nav>
+
+    <section data-toggle="wy-nav-shift" class="wy-nav-content-wrap"><nav class="wy-nav-top" aria-label="Mobile navigation menu" >
+          <i data-toggle="wy-nav-top" class="fa fa-bars"></i>
+          <a href="#">sound_source_id</a>
+      </nav>
+
+      <div class="wy-nav-content">
+        <div class="rst-content">
+          <div role="navigation" aria-label="Page navigation">
+  <ul class="wy-breadcrumbs">
+      <li><a href="#" class="icon icon-home" aria-label="Home"></a></li>
+      <li class="breadcrumb-item active">Welcome to sound_source_id’s documentation!</li>
+      <li class="wy-breadcrumbs-aside">
+            <a href="_sources/index.rst.txt" rel="nofollow"> View page source</a>
+      </li>
+  </ul>
+  <hr/>
+</div>
+          <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
+           <div itemprop="articleBody">
+             
   <section id="welcome-to-sound-source-id-s-documentation">
-<h1>Welcome to sound_source_id’s documentation!<a class="headerlink" href="#welcome-to-sound-source-id-s-documentation" title="Permalink to this heading">¶</a></h1>
+<h1>Welcome to sound_source_id’s documentation!<a class="headerlink" href="#welcome-to-sound-source-id-s-documentation" title="Permalink to this heading"></a></h1>
 <div class="toctree-wrapper compound">
 <p class="caption" role="heading"><span class="caption-text">Contents:</span></p>
 <ul>
 <li class="toctree-l1"><a class="reference internal" href="intro.html"><code class="docutils literal notranslate"><span class="pre">sound_source_id</span></code></a></li>
 <li class="toctree-l1"><a class="reference internal" href="installation.html">Installation</a></li>
 <li class="toctree-l1"><a class="reference internal" href="experiment_setup.html">Parameters file</a></li>
 <li class="toctree-l1"><a class="reference internal" href="experiment_setup.html#stimulation-file">Stimulation file</a></li>
 </ul>
 </div>
 </section>
 <section id="indices-and-tables">
-<h1>Indices and tables<a class="headerlink" href="#indices-and-tables" title="Permalink to this heading">¶</a></h1>
+<h1>Indices and tables<a class="headerlink" href="#indices-and-tables" title="Permalink to this heading"></a></h1>
 <ul class="simple">
 <li><p><a class="reference internal" href="genindex.html"><span class="std std-ref">Index</span></a></p></li>
 <li><p><a class="reference internal" href="py-modindex.html"><span class="std std-ref">Module Index</span></a></p></li>
 <li><p><a class="reference internal" href="search.html"><span class="std std-ref">Search Page</span></a></p></li>
 </ul>
 </section>
 
 
+           </div>
           </div>
-          
-        </div>
-      </div>
-      <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
-        <div class="sphinxsidebarwrapper">
-<h1 class="logo"><a href="#">sound_source_id</a></h1>
-
-
-
-
-
-
-
-
-<h3>Navigation</h3>
-<p class="caption" role="heading"><span class="caption-text">Contents:</span></p>
-<ul>
-<li class="toctree-l1"><a class="reference internal" href="intro.html"><code class="docutils literal notranslate"><span class="pre">sound_source_id</span></code></a></li>
-<li class="toctree-l1"><a class="reference internal" href="installation.html">Installation</a></li>
-<li class="toctree-l1"><a class="reference internal" href="experiment_setup.html">Parameters file</a></li>
-<li class="toctree-l1"><a class="reference internal" href="experiment_setup.html#stimulation-file">Stimulation file</a></li>
-</ul>
-
-<div class="relations">
-<h3>Related Topics</h3>
-<ul>
-  <li><a href="#">Documentation overview</a><ul>
-      <li>Next: <a href="intro.html" title="next chapter"><code class="docutils literal notranslate"><span class="pre">sound_source_id</span></code></a></li>
-  </ul></li>
-</ul>
-</div>
-<div id="searchbox" style="display: none" role="search">
-  <h3 id="searchlabel">Quick search</h3>
-    <div class="searchformwrapper">
-    <form class="search" action="search.html" method="get">
-      <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
-      <input type="submit" value="Go" />
-    </form>
+          <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
+        <a href="intro.html" class="btn btn-neutral float-right" title="sound_source_id" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
     </div>
-</div>
-<script>document.getElementById('searchbox').style.display = "block"</script>
-
-
-
-
-
 
+  <hr/>
 
+  <div role="contentinfo">
+    <p>&#169; Copyright 2022-2023, Samuele Carcagno.</p>
+  </div>
+
+  Built with <a href="https://www.sphinx-doc.org/">Sphinx</a> using a
+    <a href="https://github.com/readthedocs/sphinx_rtd_theme">theme</a>
+    provided by <a href="https://readthedocs.org">Read the Docs</a>.
+   
 
+</footer>
         </div>
       </div>
-      <div class="clearer"></div>
-    </div>
-    <div class="footer">
-      &copy;2022-2023, Samuele Carcagno.
-      
-      |
-      Powered by <a href="http://sphinx-doc.org/">Sphinx 5.3.0</a>
-      &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.12</a>
-      
-      |
-      <a href="_sources/index.rst.txt"
-          rel="nofollow">Page source</a>
-    </div>
-
-    
+    </section>
+  </div>
+  <script>
+      jQuery(function () {
+          SphinxRtdTheme.Navigation.enable(true);
+      });
+  </script> 
 
-    
-  </body>
+</body>
 </html>
```

#### html2text {}

```diff
@@ -1,33 +1,32 @@
 
 
 
 
 
-
-
-
-****** Welcome to sound_source_idâs documentation!Â¶ ******
+sound_source_id
+0.0.3
+[q                   ]
 Contents:
     * sound_source_id
     * Installation
     * Parameters_file
     * Stimulation_file
-
-****** Indices and tablesÂ¶ ******
-    * Index
-    * Module_Index
-    * Search_Page
-****** sound_source_id ******
-**** Navigation ****
+   sound_source_id
+    * Welcome to sound_source_idâs documentation!
+    * View_page_source
+===============================================================================
+****** Welcome to sound_source_idâs documentation!ï ******
 Contents:
     * sound_source_id
     * Installation
     * Parameters_file
     * Stimulation_file
-**** Related Topics ****
-    * Documentation_overview
-          o Next: sound_source_id
-**** Quick search ****
-[q                   ] [Go]
-©2022-2023, Samuele Carcagno. | Powered by Sphinx_5.3.0 & Alabaster_0.7.12 |
-Page_source
+
+****** Indices and tablesï ******
+    * Index
+    * Module_Index
+    * Search_Page
+Next
+===============================================================================
+© Copyright 2022-2023, Samuele Carcagno.
+Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `sound_source_id-0.0.2/sound_source_id/doc/_build/html/installation.html` & `sound_source_id-0.0.3/sound_source_id/doc/_build/html/installation.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,86 @@
-
 <!DOCTYPE html>
-
-<html lang="en">
-  <head>
-    <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
-
-    <title>Installation &#8212; sound_source_id 0.0.1 documentation</title>
-    <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
-    <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
-    <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
-    <script src="_static/jquery.js"></script>
-    <script src="_static/underscore.js"></script>
-    <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
-    <script src="_static/doctools.js"></script>
-    <script src="_static/sphinx_highlight.js"></script>
+<html class="writer-html5" lang="en" >
+<head>
+  <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
+
+  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
+  <title>Installation &mdash; sound_source_id 0.0.3 documentation</title>
+      <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
+      <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
+  
+        <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
+        <script src="_static/jquery.js"></script>
+        <script src="_static/underscore.js"></script>
+        <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
+        <script src="_static/doctools.js"></script>
+        <script src="_static/sphinx_highlight.js"></script>
+    <script src="_static/js/theme.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Parameters file" href="experiment_setup.html" />
-    <link rel="prev" title="sound_source_id" href="intro.html" />
-   
-  <link rel="stylesheet" href="_static/custom.css" type="text/css" />
-  
-  
-  <meta name="viewport" content="width=device-width, initial-scale=0.9, maximum-scale=0.9" />
+    <link rel="prev" title="sound_source_id" href="intro.html" /> 
+</head>
 
-  </head><body>
-  
+<body class="wy-body-for-nav"> 
+  <div class="wy-grid-for-nav">
+    <nav data-toggle="wy-nav-shift" class="wy-nav-side">
+      <div class="wy-side-scroll">
+        <div class="wy-side-nav-search" >
 
-    <div class="document">
-      <div class="documentwrapper">
-        <div class="bodywrapper">
           
+          
+          <a href="index.html" class="icon icon-home">
+            sound_source_id
+          </a>
+              <div class="version">
+                0.0.3
+              </div>
+<div role="search">
+  <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
+    <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
+    <input type="hidden" name="check_keywords" value="yes" />
+    <input type="hidden" name="area" value="default" />
+  </form>
+</div>
+        </div><div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
+              <p class="caption" role="heading"><span class="caption-text">Contents:</span></p>
+<ul class="current">
+<li class="toctree-l1"><a class="reference internal" href="intro.html"><code class="docutils literal notranslate"><span class="pre">sound_source_id</span></code></a></li>
+<li class="toctree-l1 current"><a class="current reference internal" href="#">Installation</a></li>
+<li class="toctree-l1"><a class="reference internal" href="experiment_setup.html">Parameters file</a></li>
+<li class="toctree-l1"><a class="reference internal" href="experiment_setup.html#stimulation-file">Stimulation file</a></li>
+</ul>
+
+        </div>
+      </div>
+    </nav>
 
-          <div class="body" role="main">
-            
+    <section data-toggle="wy-nav-shift" class="wy-nav-content-wrap"><nav class="wy-nav-top" aria-label="Mobile navigation menu" >
+          <i data-toggle="wy-nav-top" class="fa fa-bars"></i>
+          <a href="index.html">sound_source_id</a>
+      </nav>
+
+      <div class="wy-nav-content">
+        <div class="rst-content">
+          <div role="navigation" aria-label="Page navigation">
+  <ul class="wy-breadcrumbs">
+      <li><a href="index.html" class="icon icon-home" aria-label="Home"></a></li>
+      <li class="breadcrumb-item active">Installation</li>
+      <li class="wy-breadcrumbs-aside">
+            <a href="_sources/installation.rst.txt" rel="nofollow"> View page source</a>
+      </li>
+  </ul>
+  <hr/>
+</div>
+          <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
+           <div itemprop="articleBody">
+             
   <section id="installation">
-<span id="sec-installation"></span><h1>Installation<a class="headerlink" href="#installation" title="Permalink to this heading">¶</a></h1>
+<span id="sec-installation"></span><h1>Installation<a class="headerlink" href="#installation" title="Permalink to this heading"></a></h1>
 <p><code class="docutils literal notranslate"><span class="pre">sound_source_id</span></code> has been successfully installed and used on Linux and Windows. It should also work on Mac platforms, but this has not been tested. <code class="docutils literal notranslate"><span class="pre">sound_source_id</span></code> is written in Python and can be installed via pip:</p>
 <div class="highlight-bash notranslate"><div class="highlight"><pre><span></span>pip<span class="w"> </span>install<span class="w"> </span>sound_source_id
 </pre></div>
 </div>
 <p><code class="docutils literal notranslate"><span class="pre">sound_source_id</span></code> depends on a few Python modules including:</p>
 <blockquote>
 <div><ul class="simple">
@@ -68,79 +108,38 @@
 <div><ul class="simple">
 <li><p><a class="reference external" href="https://sox.sourceforge.net/">https://sox.sourceforge.net/</a></p></li>
 </ul>
 </div></blockquote>
 </section>
 
 
+           </div>
           </div>
-          
-        </div>
-      </div>
-      <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
-        <div class="sphinxsidebarwrapper">
-<h1 class="logo"><a href="index.html">sound_source_id</a></h1>
-
-
-
-
-
-
-
-
-<h3>Navigation</h3>
-<p class="caption" role="heading"><span class="caption-text">Contents:</span></p>
-<ul class="current">
-<li class="toctree-l1"><a class="reference internal" href="intro.html"><code class="docutils literal notranslate"><span class="pre">sound_source_id</span></code></a></li>
-<li class="toctree-l1 current"><a class="current reference internal" href="#">Installation</a></li>
-<li class="toctree-l1"><a class="reference internal" href="experiment_setup.html">Parameters file</a></li>
-<li class="toctree-l1"><a class="reference internal" href="experiment_setup.html#stimulation-file">Stimulation file</a></li>
-</ul>
-
-<div class="relations">
-<h3>Related Topics</h3>
-<ul>
-  <li><a href="index.html">Documentation overview</a><ul>
-      <li>Previous: <a href="intro.html" title="previous chapter"><code class="docutils literal notranslate"><span class="pre">sound_source_id</span></code></a></li>
-      <li>Next: <a href="experiment_setup.html" title="next chapter">Parameters file</a></li>
-  </ul></li>
-</ul>
-</div>
-<div id="searchbox" style="display: none" role="search">
-  <h3 id="searchlabel">Quick search</h3>
-    <div class="searchformwrapper">
-    <form class="search" action="search.html" method="get">
-      <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
-      <input type="submit" value="Go" />
-    </form>
+          <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
+        <a href="intro.html" class="btn btn-neutral float-left" title="sound_source_id" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
+        <a href="experiment_setup.html" class="btn btn-neutral float-right" title="Parameters file" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
     </div>
-</div>
-<script>document.getElementById('searchbox').style.display = "block"</script>
-
-
-
-
-
 
+  <hr/>
 
+  <div role="contentinfo">
+    <p>&#169; Copyright 2022-2023, Samuele Carcagno.</p>
+  </div>
+
+  Built with <a href="https://www.sphinx-doc.org/">Sphinx</a> using a
+    <a href="https://github.com/readthedocs/sphinx_rtd_theme">theme</a>
+    provided by <a href="https://readthedocs.org">Read the Docs</a>.
+   
 
+</footer>
         </div>
       </div>
-      <div class="clearer"></div>
-    </div>
-    <div class="footer">
-      &copy;2022-2023, Samuele Carcagno.
-      
-      |
-      Powered by <a href="http://sphinx-doc.org/">Sphinx 5.3.0</a>
-      &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.12</a>
-      
-      |
-      <a href="_sources/installation.rst.txt"
-          rel="nofollow">Page source</a>
-    </div>
-
-    
+    </section>
+  </div>
+  <script>
+      jQuery(function () {
+          SphinxRtdTheme.Navigation.enable(true);
+      });
+  </script> 
 
-    
-  </body>
+</body>
 </html>
```

#### html2text {}

```diff
@@ -1,17 +1,26 @@
 
 
 
 
 
 
-
-
-
-****** InstallationÂ¶ ******
+sound_source_id
+0.0.3
+[q                   ]
+Contents:
+    * sound_source_id
+    * Installation
+    * Parameters_file
+    * Stimulation_file
+   sound_source_id
+    * Installation
+    * View_page_source
+===============================================================================
+****** Installationï ******
 sound_source_id has been successfully installed and used on Linux and Windows.
 It should also work on Mac platforms, but this has not been tested.
 sound_source_id is written in Python and can be installed via pip:
 pip install sound_source_id
 sound_source_id depends on a few Python modules including:
          * PyQt5
          * numpy
@@ -31,22 +40,11 @@
 above command matches the one you used when you installed the application.
 Sound can be played with either PyAudio, or SoX on Windows. On Linux
 pyalsaaudio can be also used. Depending on how you want sound to be played, you
 need to install:
          * pyalsaaudio https://pypi.org/project/pyalsaaudio/
 or SoX:
          * https://sox.sourceforge.net/
-****** sound_source_id ******
-**** Navigation ****
-Contents:
-    * sound_source_id
-    * Installation
-    * Parameters_file
-    * Stimulation_file
-**** Related Topics ****
-    * Documentation_overview
-          o Previous: sound_source_id
-          o Next: Parameters_file
-**** Quick search ****
-[q                   ] [Go]
-©2022-2023, Samuele Carcagno. | Powered by Sphinx_5.3.0 & Alabaster_0.7.12 |
-Page_source
+Previous Next
+===============================================================================
+© Copyright 2022-2023, Samuele Carcagno.
+Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `sound_source_id-0.0.2/sound_source_id/doc/_build/html/intro.html` & `sound_source_id-0.0.3/sound_source_id/doc/_build/html/intro.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,121 +1,120 @@
-
 <!DOCTYPE html>
-
-<html lang="en">
-  <head>
-    <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
-
-    <title>sound_source_id &#8212; sound_source_id 0.0.1 documentation</title>
-    <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
-    <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
-    <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
-    <script src="_static/jquery.js"></script>
-    <script src="_static/underscore.js"></script>
-    <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
-    <script src="_static/doctools.js"></script>
-    <script src="_static/sphinx_highlight.js"></script>
+<html class="writer-html5" lang="en" >
+<head>
+  <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
+
+  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
+  <title>sound_source_id &mdash; sound_source_id 0.0.3 documentation</title>
+      <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
+      <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
+  
+        <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
+        <script src="_static/jquery.js"></script>
+        <script src="_static/underscore.js"></script>
+        <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
+        <script src="_static/doctools.js"></script>
+        <script src="_static/sphinx_highlight.js"></script>
+    <script src="_static/js/theme.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Installation" href="installation.html" />
-    <link rel="prev" title="Welcome to sound_source_id’s documentation!" href="index.html" />
-   
-  <link rel="stylesheet" href="_static/custom.css" type="text/css" />
-  
-  
-  <meta name="viewport" content="width=device-width, initial-scale=0.9, maximum-scale=0.9" />
+    <link rel="prev" title="Welcome to sound_source_id’s documentation!" href="index.html" /> 
+</head>
 
-  </head><body>
-  
+<body class="wy-body-for-nav"> 
+  <div class="wy-grid-for-nav">
+    <nav data-toggle="wy-nav-shift" class="wy-nav-side">
+      <div class="wy-side-scroll">
+        <div class="wy-side-nav-search" >
 
-    <div class="document">
-      <div class="documentwrapper">
-        <div class="bodywrapper">
           
+          
+          <a href="index.html" class="icon icon-home">
+            sound_source_id
+          </a>
+              <div class="version">
+                0.0.3
+              </div>
+<div role="search">
+  <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
+    <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
+    <input type="hidden" name="check_keywords" value="yes" />
+    <input type="hidden" name="area" value="default" />
+  </form>
+</div>
+        </div><div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
+              <p class="caption" role="heading"><span class="caption-text">Contents:</span></p>
+<ul class="current">
+<li class="toctree-l1 current"><a class="current reference internal" href="#"><code class="docutils literal notranslate"><span class="pre">sound_source_id</span></code></a></li>
+<li class="toctree-l1"><a class="reference internal" href="installation.html">Installation</a></li>
+<li class="toctree-l1"><a class="reference internal" href="experiment_setup.html">Parameters file</a></li>
+<li class="toctree-l1"><a class="reference internal" href="experiment_setup.html#stimulation-file">Stimulation file</a></li>
+</ul>
+
+        </div>
+      </div>
+    </nav>
 
-          <div class="body" role="main">
-            
+    <section data-toggle="wy-nav-shift" class="wy-nav-content-wrap"><nav class="wy-nav-top" aria-label="Mobile navigation menu" >
+          <i data-toggle="wy-nav-top" class="fa fa-bars"></i>
+          <a href="index.html">sound_source_id</a>
+      </nav>
+
+      <div class="wy-nav-content">
+        <div class="rst-content">
+          <div role="navigation" aria-label="Page navigation">
+  <ul class="wy-breadcrumbs">
+      <li><a href="index.html" class="icon icon-home" aria-label="Home"></a></li>
+      <li class="breadcrumb-item active"><code class="docutils literal notranslate"><span class="pre">sound_source_id</span></code></li>
+      <li class="wy-breadcrumbs-aside">
+            <a href="_sources/intro.rst.txt" rel="nofollow"> View page source</a>
+      </li>
+  </ul>
+  <hr/>
+</div>
+          <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
+           <div itemprop="articleBody">
+             
   <section id="sound-source-id">
-<h1><code class="docutils literal notranslate"><span class="pre">sound_source_id</span></code><a class="headerlink" href="#sound-source-id" title="Permalink to this heading">¶</a></h1>
+<h1><code class="docutils literal notranslate"><span class="pre">sound_source_id</span></code><a class="headerlink" href="#sound-source-id" title="Permalink to this heading"></a></h1>
 <p><code class="docutils literal notranslate"><span class="pre">sound_source_id</span></code> is program for testing static sound localization. The interface is shown in Figure <a class="reference internal" href="#fig-sound-source-id-screenshot"><span class="std std-ref">Screenshot of the sound_source_id interface.</span></a>.</p>
 <figure class="align-default" id="id1">
 <span id="fig-sound-source-id-screenshot"></span><a class="reference internal image-reference" href="_images/sound_source_id_screenshot.png"><img alt="Screenshot of the ``sound_source_id`` interface." src="_images/sound_source_id_screenshot.png" style="width: 624.0px; height: 311.5px;" /></a>
 <figcaption>
-<p><span class="caption-text">Screenshot of the <code class="docutils literal notranslate"><span class="pre">sound_source_id</span></code> interface.</span><a class="headerlink" href="#id1" title="Permalink to this image">¶</a></p>
+<p><span class="caption-text">Screenshot of the <code class="docutils literal notranslate"><span class="pre">sound_source_id</span></code> interface.</span><a class="headerlink" href="#id1" title="Permalink to this image"></a></p>
 </figcaption>
 </figure>
 </section>
 
 
+           </div>
           </div>
-          
-        </div>
-      </div>
-      <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
-        <div class="sphinxsidebarwrapper">
-<h1 class="logo"><a href="index.html">sound_source_id</a></h1>
-
-
-
-
-
-
-
-
-<h3>Navigation</h3>
-<p class="caption" role="heading"><span class="caption-text">Contents:</span></p>
-<ul class="current">
-<li class="toctree-l1 current"><a class="current reference internal" href="#"><code class="docutils literal notranslate"><span class="pre">sound_source_id</span></code></a></li>
-<li class="toctree-l1"><a class="reference internal" href="installation.html">Installation</a></li>
-<li class="toctree-l1"><a class="reference internal" href="experiment_setup.html">Parameters file</a></li>
-<li class="toctree-l1"><a class="reference internal" href="experiment_setup.html#stimulation-file">Stimulation file</a></li>
-</ul>
-
-<div class="relations">
-<h3>Related Topics</h3>
-<ul>
-  <li><a href="index.html">Documentation overview</a><ul>
-      <li>Previous: <a href="index.html" title="previous chapter">Welcome to sound_source_id’s documentation!</a></li>
-      <li>Next: <a href="installation.html" title="next chapter">Installation</a></li>
-  </ul></li>
-</ul>
-</div>
-<div id="searchbox" style="display: none" role="search">
-  <h3 id="searchlabel">Quick search</h3>
-    <div class="searchformwrapper">
-    <form class="search" action="search.html" method="get">
-      <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
-      <input type="submit" value="Go" />
-    </form>
+          <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
+        <a href="index.html" class="btn btn-neutral float-left" title="Welcome to sound_source_id’s documentation!" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
+        <a href="installation.html" class="btn btn-neutral float-right" title="Installation" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
     </div>
-</div>
-<script>document.getElementById('searchbox').style.display = "block"</script>
-
-
-
-
-
 
+  <hr/>
 
+  <div role="contentinfo">
+    <p>&#169; Copyright 2022-2023, Samuele Carcagno.</p>
+  </div>
+
+  Built with <a href="https://www.sphinx-doc.org/">Sphinx</a> using a
+    <a href="https://github.com/readthedocs/sphinx_rtd_theme">theme</a>
+    provided by <a href="https://readthedocs.org">Read the Docs</a>.
+   
 
+</footer>
         </div>
       </div>
-      <div class="clearer"></div>
-    </div>
-    <div class="footer">
-      &copy;2022-2023, Samuele Carcagno.
-      
-      |
-      Powered by <a href="http://sphinx-doc.org/">Sphinx 5.3.0</a>
-      &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.12</a>
-      
-      |
-      <a href="_sources/intro.rst.txt"
-          rel="nofollow">Page source</a>
-    </div>
-
-    
+    </section>
+  </div>
+  <script>
+      jQuery(function () {
+          SphinxRtdTheme.Navigation.enable(true);
+      });
+  </script> 
 
-    
-  </body>
+</body>
 </html>
```

#### html2text {}

```diff
@@ -1,30 +1,28 @@
 
 
 
 
 
 
-
-
-
-****** sound_source_idÂ¶ ******
-sound_source_id is program for testing static sound localization. The interface
-is shown in Figure Screenshot_of_the_sound_source_id_interface..
- [Screenshot_of_the_``sound_source_id``_interface.]
-Screenshot of the sound_source_id interface.Â¶
-
-****** sound_source_id ******
-**** Navigation ****
+sound_source_id
+0.0.3
+[q                   ]
 Contents:
     * sound_source_id
     * Installation
     * Parameters_file
     * Stimulation_file
-**** Related Topics ****
-    * Documentation_overview
-          o Previous: Welcome_to_sound_source_idâs_documentation!
-          o Next: Installation
-**** Quick search ****
-[q                   ] [Go]
-©2022-2023, Samuele Carcagno. | Powered by Sphinx_5.3.0 & Alabaster_0.7.12 |
-Page_source
+   sound_source_id
+    * sound_source_id
+    * View_page_source
+===============================================================================
+****** sound_source_idï ******
+sound_source_id is program for testing static sound localization. The interface
+is shown in Figure Screenshot_of_the_sound_source_id_interface..
+ [Screenshot_of_the_``sound_source_id``_interface.]
+Screenshot of the sound_source_id interface.ï
+
+Previous Next
+===============================================================================
+© Copyright 2022-2023, Samuele Carcagno.
+Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `sound_source_id-0.0.2/sound_source_id/doc/_build/html/search.html` & `sound_source_id-0.0.3/sound_source_id/doc/_build/html/search.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,128 +1,124 @@
-
 <!DOCTYPE html>
-
-<html lang="en">
-  <head>
-    <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Search &#8212; sound_source_id 0.0.1 documentation</title>
-    <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
-    <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
+<html class="writer-html5" lang="en" >
+<head>
+  <meta charset="utf-8" />
+  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
+  <title>Search &mdash; sound_source_id 0.0.3 documentation</title>
+      <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
+      <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
     
-    <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
-    <script src="_static/jquery.js"></script>
-    <script src="_static/underscore.js"></script>
-    <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
-    <script src="_static/doctools.js"></script>
-    <script src="_static/sphinx_highlight.js"></script>
+  
+        <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
+        <script src="_static/jquery.js"></script>
+        <script src="_static/underscore.js"></script>
+        <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
+        <script src="_static/doctools.js"></script>
+        <script src="_static/sphinx_highlight.js"></script>
+    <script src="_static/js/theme.js"></script>
     <script src="_static/searchtools.js"></script>
     <script src="_static/language_data.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
-    <link rel="search" title="Search" href="#" />
-  <script src="searchindex.js" defer></script>
-  
-   
-  <link rel="stylesheet" href="_static/custom.css" type="text/css" />
-  
-  
-  <meta name="viewport" content="width=device-width, initial-scale=0.9, maximum-scale=0.9" />
-
+    <link rel="search" title="Search" href="#" /> 
+</head>
 
-  </head><body>
-  
+<body class="wy-body-for-nav"> 
+  <div class="wy-grid-for-nav">
+    <nav data-toggle="wy-nav-shift" class="wy-nav-side">
+      <div class="wy-side-scroll">
+        <div class="wy-side-nav-search" >
 
-    <div class="document">
-      <div class="documentwrapper">
-        <div class="bodywrapper">
           
-
-          <div class="body" role="main">
-            
-  <h1 id="search-documentation">Search</h1>
-  
-  <noscript>
-  <div class="admonition warning">
-  <p>
-    Please activate JavaScript to enable the search
-    functionality.
-  </p>
-  </div>
-  </noscript>
-  
-  
-  <p>
-    Searching for multiple words only shows matches that contain
-    all words.
-  </p>
-  
-  
-  <form action="" method="get">
-    <input type="text" name="q" aria-labelledby="search-documentation" value="" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
-    <input type="submit" value="search" />
-    <span id="search-progress" style="padding-left: 10px"></span>
-  </form>
-  
-  
-  
-  <div id="search-results">
-  
-  </div>
-  
-
-          </div>
           
-        </div>
-      </div>
-      <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
-        <div class="sphinxsidebarwrapper">
-<h1 class="logo"><a href="index.html">sound_source_id</a></h1>
-
-
-
-
-
-
-
-
-<h3>Navigation</h3>
-<p class="caption" role="heading"><span class="caption-text">Contents:</span></p>
+          <a href="index.html" class="icon icon-home">
+            sound_source_id
+          </a>
+              <div class="version">
+                0.0.3
+              </div>
+<div role="search">
+  <form id="rtd-search-form" class="wy-form" action="#" method="get">
+    <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
+    <input type="hidden" name="check_keywords" value="yes" />
+    <input type="hidden" name="area" value="default" />
+  </form>
+</div>
+        </div><div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
+              <p class="caption" role="heading"><span class="caption-text">Contents:</span></p>
 <ul>
 <li class="toctree-l1"><a class="reference internal" href="intro.html"><code class="docutils literal notranslate"><span class="pre">sound_source_id</span></code></a></li>
 <li class="toctree-l1"><a class="reference internal" href="installation.html">Installation</a></li>
 <li class="toctree-l1"><a class="reference internal" href="experiment_setup.html">Parameters file</a></li>
 <li class="toctree-l1"><a class="reference internal" href="experiment_setup.html#stimulation-file">Stimulation file</a></li>
 </ul>
 
-<div class="relations">
-<h3>Related Topics</h3>
-<ul>
-  <li><a href="index.html">Documentation overview</a><ul>
-  </ul></li>
-</ul>
-</div>
-
+        </div>
+      </div>
+    </nav>
 
+    <section data-toggle="wy-nav-shift" class="wy-nav-content-wrap"><nav class="wy-nav-top" aria-label="Mobile navigation menu" >
+          <i data-toggle="wy-nav-top" class="fa fa-bars"></i>
+          <a href="index.html">sound_source_id</a>
+      </nav>
+
+      <div class="wy-nav-content">
+        <div class="rst-content">
+          <div role="navigation" aria-label="Page navigation">
+  <ul class="wy-breadcrumbs">
+      <li><a href="index.html" class="icon icon-home" aria-label="Home"></a></li>
+      <li class="breadcrumb-item active">Search</li>
+      <li class="wy-breadcrumbs-aside">
+      </li>
+  </ul>
+  <hr/>
+</div>
+          <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
+           <div itemprop="articleBody">
+             
+  <noscript>
+  <div id="fallback" class="admonition warning">
+    <p class="last">
+      Please activate JavaScript to enable the search functionality.
+    </p>
+  </div>
+  </noscript>
 
+  
+  <div id="search-results">
+  
+  </div>
 
+           </div>
+          </div>
+          <footer>
 
+  <hr/>
 
+  <div role="contentinfo">
+    <p>&#169; Copyright 2022-2023, Samuele Carcagno.</p>
+  </div>
 
+  Built with <a href="https://www.sphinx-doc.org/">Sphinx</a> using a
+    <a href="https://github.com/readthedocs/sphinx_rtd_theme">theme</a>
+    provided by <a href="https://readthedocs.org">Read the Docs</a>.
+   
 
+</footer>
         </div>
       </div>
-      <div class="clearer"></div>
-    </div>
-    <div class="footer">
-      &copy;2022-2023, Samuele Carcagno.
-      
-      |
-      Powered by <a href="http://sphinx-doc.org/">Sphinx 5.3.0</a>
-      &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.12</a>
-      
-    </div>
+    </section>
+  </div>
+  <script>
+      jQuery(function () {
+          SphinxRtdTheme.Navigation.enable(true);
+      });
+  </script>
+  <script>
+    jQuery(function() { Search.loadIndex("searchindex.js"); });
+  </script>
+  
+  <script id="searchindexloader"></script>
+   
 
-    
 
-    
-  </body>
+</body>
 </html>
```

#### html2text {}

```diff
@@ -1,21 +1,20 @@
 
 
 
 
-
-
-
-****** Search ******
-Please activate JavaScript to enable the search functionality.
-Searching for multiple words only shows matches that contain all words.
-[q                   ] [search]
-****** sound_source_id ******
-**** Navigation ****
+sound_source_id
+0.0.3
+[q                   ]
 Contents:
     * sound_source_id
     * Installation
     * Parameters_file
     * Stimulation_file
-**** Related Topics ****
-    * Documentation_overview
-©2022-2023, Samuele Carcagno. | Powered by Sphinx_5.3.0 & Alabaster_0.7.12
+   sound_source_id
+    * Search
+===============================================================================
+Please activate JavaScript to enable the search functionality.
+
+===============================================================================
+© Copyright 2022-2023, Samuele Carcagno.
+Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `sound_source_id-0.0.2/sound_source_id/doc/_build/html/searchindex.js` & `sound_source_id-0.0.3/sound_source_id/doc/_build/html/searchindex.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -113,15 +113,15 @@
         "sent": 0,
         "sound_fil": 0,
         "condit": 0,
         "option": 0,
         "experiment": 0,
         "base": 0,
         "assum": 0,
-        "pyloc": 0,
+        "pyloc": [],
         "ha": [0, 2],
         "been": [0, 2],
         "correctli": 0,
         "calibr": 0,
         "rove": 0,
         "actual": 0,
         "euqual": 0,
@@ -213,15 +213,15 @@
         "click": [],
         "rather": [],
         "than": [],
         "static": 3,
         "local": 3,
         "interfac": 3,
         "screenshot": 3,
-        "sound_source_id": 2,
+        "sound_source_id": [0, 2],
         "path_to_sound_source_id": [],
         "via": 2,
         "pip": 2,
         "mai": 2,
         "dependeci": 2,
         "through": 2,
         "conda": 2,
@@ -290,16 +290,16 @@
         ],
         "Contents:": [
             [1, null]
         ],
         "Indices and tables": [
             [1, "indices-and-tables"]
         ],
-        "sound_source_id": [
-            [3, "sound-source-id"]
-        ],
         "Installation": [
             [2, "installation"]
+        ],
+        "sound_source_id": [
+            [3, "sound-source-id"]
         ]
     },
     "indexentries": {}
 })
```

### Comparing `sound_source_id-0.0.2/sound_source_id/doc/_build/latex/sound_source_id.pdf` & `sound_source_id-0.0.3/sound_source_id/doc/_build/latex/sound_source_id.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 12% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,13 +1,13 @@
 sound_source_id
-Release 0.0.1
+Release 0.0.3
 
 Samuele Carcagno
 
-Jun 03, 2023
+Jun 05, 2023
 
 CONTENTS:
 
 1
 
 sound_source_id
 
@@ -50,15 +50,15 @@
 sound_source_id is program for testing static sound localization. The interface is shown in Figure Screenshot of the
 sound_source_id interface..
 
 Fig. 1: Screenshot of the sound_source_id interface.
 
 1
 
-sound_source_id, Release 0.0.1
+sound_source_id, Release 0.0.3
 
 2
 
 Chapter 1. sound_source_id
 
 CHAPTER
 
@@ -88,15 +88,15 @@
 on how you want sound to be played, you need to install:
 • pyalsaaudio https://pypi.org/project/pyalsaaudio/
 or SoX:
 • https://sox.sourceforge.net/
 
 3
 
-sound_source_id, Release 0.0.1
+sound_source_id, Release 0.0.3
 
 4
 
 Chapter 2. Installation
 
 CHAPTER
 
@@ -125,15 +125,15 @@
 • stim_list_file: the path (absolute or relative) to the file containing the stimulation list (see below)
 • randomize: if true the stim_list_file will be shuffled before each block repetition
 • demo_stim: the path to the WAV file to be used for the demo
 • demo_stim_lev: the sound level (in dB SPL) to be used for the demo
 
 5
 
-sound_source_id, Release 0.0.1
+sound_source_id, Release 0.0.3
 
 6
 
 Chapter 3. Parameters file
 
 CHAPTER
 
@@ -146,23 +146,23 @@
 
 Fig. 1: Example stimulation file.
 Each row of the file represents a trial. Stimulation files contain the following columns:
 • angle: the angle at which the sound will be presented (stimuli will be sent to the corresponding soundcard channel
 as specified in the parameters file)
 • sound_file: the path (relative or absolute) to the WAV file to be played
 • condition: an optional label specifying the experimental condition
-• level: the base sound level (in dB SPL) at which the sound will be presented (this assumes that pyloc has been
-correctly calibrated)
+• level: the base sound level (in dB SPL) at which the sound will be presented (this assumes that sound_source_id
+has been correctly calibrated)
 • roving: a level rove, actual sound level will be euqual to the base level plus a value drawn from a random uniform
 distribution between +/- the roving level
 • feedback: if true, feedback will be given to the listener at the end of each trial
 
 7
 
-sound_source_id, Release 0.0.1
+sound_source_id, Release 0.0.3
 
 8
 
 Chapter 4. Stimulation file
 
 CHAPTER
```

### Comparing `sound_source_id-0.0.2/sound_source_id/doc/conf.py` & `sound_source_id-0.0.3/sound_source_id/doc/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 author = 'Samuele Carcagno'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = "0.0.2"
+version = "0.0.3"
 # The full version, including alpha/beta/rc tags.
-release = "0.0.2"
+release = "0.0.3"
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
@@ -48,13 +48,13 @@
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'alabaster'
+html_theme = 'sphinx_rtd_theme'
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ['_static']
```

### Comparing `sound_source_id-0.0.2/sound_source_id/doc/experiment_setup.rst` & `sound_source_id-0.0.3/sound_source_id/doc/experiment_setup.rst`

 * *Files 4% similar despite different names*

```diff
@@ -45,10 +45,10 @@
    Example stimulation file.
 
 Each row of the file represents a trial. Stimulation files contain the following columns:
 
   - `angle`: the angle at which the sound will be presented (stimuli will be sent to the corresponding soundcard channel as specified in the parameters file)
   - `sound_file`: the path (relative or absolute) to the WAV file to be played
   - `condition`: an optional label specifying the experimental condition
-  - `level`: the `base` sound level (in dB SPL) at which the sound will be presented (this assumes that `pyloc` has been correctly calibrated)
+  - `level`: the `base` sound level (in dB SPL) at which the sound will be presented (this assumes that `sound_source_id` has been correctly calibrated)
   - `roving`: a level rove, actual sound level will be euqual to the base level plus a value drawn from a random uniform distribution between +/- the roving level
   - `feedback`: if `true`, feedback will be given to the listener at the end of each trial
```

### Comparing `sound_source_id-0.0.2/sound_source_id/doc/installation.rst` & `sound_source_id-0.0.3/sound_source_id/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/doc/make.bat` & `sound_source_id-0.0.3/sound_source_id/doc/make.bat`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/global_parameters.py` & `sound_source_id-0.0.3/sound_source_id/global_parameters.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/icons/point-right.ico` & `sound_source_id-0.0.3/sound_source_id/icons/point-right.ico`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise1.wav` & `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise1.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise10.wav` & `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise10.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise11.wav` & `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise11.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise12.wav` & `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise12.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise13.wav` & `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise13.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise14.wav` & `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise14.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise15.wav` & `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise15.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise16.wav` & `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise16.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise17.wav` & `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise17.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise18.wav` & `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise18.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise19.wav` & `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise19.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise2.wav` & `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise2.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise20.wav` & `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise20.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise21.wav` & `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise21.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise22.wav` & `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise22.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise23.wav` & `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise23.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise24.wav` & `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise24.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise25.wav` & `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise25.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise26.wav` & `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise26.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise27.wav` & `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise27.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise28.wav` & `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise28.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise29.wav` & `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise29.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise3.wav` & `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise3.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise30.wav` & `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise30.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise4.wav` & `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise4.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise5.wav` & `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise5.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise6.wav` & `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise6.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise7.wav` & `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise7.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise8.wav` & `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise8.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/prm_files/pink_noises/noise9.wav` & `sound_source_id-0.0.3/sound_source_id/prm_files/pink_noises/noise9.wav`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/prm_files/stim_list.csv` & `sound_source_id-0.0.3/sound_source_id/prm_files/stim_list.csv`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/pyqtver.py` & `sound_source_id-0.0.3/sound_source_id/pyqtver.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/qrc_resources.py` & `sound_source_id-0.0.3/sound_source_id/qrc_resources.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/scipy_wav.py` & `sound_source_id-0.0.3/sound_source_id/scipy_wav.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/sndlib.py` & `sound_source_id-0.0.3/sound_source_id/sndlib.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/wavpy.py` & `sound_source_id-0.0.3/sound_source_id/wavpy.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id/wavpy_sndf.py` & `sound_source_id-0.0.3/sound_source_id/wavpy_sndf.py`

 * *Files identical despite different names*

### Comparing `sound_source_id-0.0.2/sound_source_id.egg-info/PKG-INFO` & `sound_source_id-0.0.3/sound_source_id.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sound-source-id
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python application for running sound localization experiments
 Author-email: Samuele Carcagno <sam.carcagno@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `sound_source_id-0.0.2/sound_source_id.egg-info/SOURCES.txt` & `sound_source_id-0.0.3/sound_source_id.egg-info/SOURCES.txt`

 * *Files identical despite different names*

