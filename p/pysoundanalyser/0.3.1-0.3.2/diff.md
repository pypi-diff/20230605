# Comparing `tmp/pysoundanalyser-0.3.1.tar.gz` & `tmp/pysoundanalyser-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysoundanalyser-0.3.1.tar", last modified: Sun Jun  4 05:19:13 2023, max compression
+gzip compressed data, was "pysoundanalyser-0.3.2.tar", last modified: Mon Jun  5 08:15:05 2023, max compression
```

## Comparing `pysoundanalyser-0.3.1.tar` & `pysoundanalyser-0.3.2.tar`

### file list

```diff
@@ -1,216 +1,162 @@
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-04 05:19:13.930760 pysoundanalyser-0.3.1/
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)    35147 2010-06-04 09:15:48.000000 pysoundanalyser-0.3.1/COPYING.txt
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)      183 2015-11-13 01:18:22.000000 pysoundanalyser-0.3.1/CREDITS.txt
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)       71 2015-09-08 22:01:46.000000 pysoundanalyser-0.3.1/INSTALL.txt
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)      696 2023-06-03 16:00:04.000000 pysoundanalyser-0.3.1/MANIFEST.in
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    42068 2023-06-04 05:19:13.930760 pysoundanalyser-0.3.1/PKG-INFO
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)      370 2022-07-18 13:01:39.000000 pysoundanalyser-0.3.1/README.md
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-04 05:19:12.761739 pysoundanalyser-0.3.1/icons/
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)    16622 2011-11-01 10:05:06.000000 pysoundanalyser-0.3.1/icons/exit.svg
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)    24750 2012-04-19 09:34:44.000000 pysoundanalyser-0.3.1/icons/johnny_automatic_crashing_wave.ico
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    45168 2015-09-29 11:52:50.000000 pysoundanalyser-0.3.1/icons/johnny_automatic_crashing_wave.png
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)    14143 2010-05-31 11:23:42.000000 pysoundanalyser-0.3.1/icons/johnny_automatic_crashing_wave.svg
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-04 05:19:12.824741 pysoundanalyser-0.3.1/prep-release/
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-04 05:19:12.867741 pysoundanalyser-0.3.1/prep-release/debian/
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)     9879 2020-05-28 09:36:16.000000 pysoundanalyser-0.3.1/prep-release/debian/changelog
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)        2 2012-12-17 22:35:36.000000 pysoundanalyser-0.3.1/prep-release/debian/compat
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)      849 2015-09-21 10:20:50.000000 pysoundanalyser-0.3.1/prep-release/debian/control
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)     1101 2013-02-08 13:13:12.000000 pysoundanalyser-0.3.1/prep-release/debian/copyright
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)        5 2013-02-08 11:05:31.000000 pysoundanalyser-0.3.1/prep-release/debian/docs
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)       71 2013-02-08 13:42:44.000000 pysoundanalyser-0.3.1/prep-release/debian/links
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)      745 2013-02-08 11:36:14.000000 pysoundanalyser-0.3.1/prep-release/debian/rules
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-04 05:19:12.676738 pysoundanalyser-0.3.1/prep-release/launchpad/
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-04 05:19:12.914742 pysoundanalyser-0.3.1/prep-release/launchpad/debian/
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)    10985 2020-05-28 13:40:27.000000 pysoundanalyser-0.3.1/prep-release/launchpad/debian/changelog
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)        2 2012-12-17 22:35:36.000000 pysoundanalyser-0.3.1/prep-release/launchpad/debian/compat
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)     1077 2020-05-28 13:40:20.000000 pysoundanalyser-0.3.1/prep-release/launchpad/debian/control
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)     1101 2013-02-08 13:13:12.000000 pysoundanalyser-0.3.1/prep-release/launchpad/debian/copyright
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)        5 2013-02-08 11:05:31.000000 pysoundanalyser-0.3.1/prep-release/launchpad/debian/docs
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)       71 2013-02-08 13:42:44.000000 pysoundanalyser-0.3.1/prep-release/launchpad/debian/links
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)      745 2013-02-08 11:36:14.000000 pysoundanalyser-0.3.1/prep-release/launchpad/debian/rules
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)     2171 2020-05-28 13:36:12.000000 pysoundanalyser-0.3.1/prep-release/launchpad_build.py
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)     3051 2015-10-13 17:39:53.000000 pysoundanalyser-0.3.1/prep-release/make_deb.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)        1 2023-06-04 05:18:34.000000 pysoundanalyser-0.3.1/prep-release/minor_minor_number.txt
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)      178 2022-09-23 15:23:28.000000 pysoundanalyser-0.3.1/prep-release/mkupdate_pyqt5.sh
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     1122 2023-06-03 15:25:11.000000 pysoundanalyser-0.3.1/prep-release/mkupdate_pyqt6.sh
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     1185 2023-06-03 15:23:52.000000 pysoundanalyser-0.3.1/prep-release/pysoundanalyser.pro
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    77407 2023-06-03 15:43:28.000000 pysoundanalyser-0.3.1/prep-release/pysoundanalyser_de.ts
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    77407 2023-06-03 15:43:28.000000 pysoundanalyser-0.3.1/prep-release/pysoundanalyser_el.ts
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    77435 2023-06-03 15:43:28.000000 pysoundanalyser-0.3.1/prep-release/pysoundanalyser_en_GB.ts
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    77407 2023-06-03 15:43:28.000000 pysoundanalyser-0.3.1/prep-release/pysoundanalyser_es.ts
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    79000 2023-06-03 15:43:28.000000 pysoundanalyser-0.3.1/prep-release/pysoundanalyser_fr.ts
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    93371 2023-06-03 15:43:28.000000 pysoundanalyser-0.3.1/prep-release/pysoundanalyser_it.ts
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    77424 2023-06-03 15:43:28.000000 pysoundanalyser-0.3.1/prep-release/pysoundanalyser_ru.ts
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     2654 2023-06-03 15:24:35.000000 pysoundanalyser-0.3.1/prep-release/release.py
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      937 2023-05-20 14:38:46.000000 pysoundanalyser-0.3.1/prep-release/switch_pyqt5.py
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      937 2023-05-20 14:37:31.000000 pysoundanalyser-0.3.1/prep-release/switch_pyqt6.py
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     2875 2019-02-12 09:45:06.000000 pysoundanalyser-0.3.1/prep-release/uploadToWebsite.py
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     1527 2023-06-04 05:18:34.000000 pysoundanalyser-0.3.1/pyproject.toml
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-04 05:19:13.004744 pysoundanalyser-0.3.1/pysoundanalyser/
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)        0 2008-10-28 02:30:54.000000 pysoundanalyser-0.3.1/pysoundanalyser/__init__.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    80415 2023-06-03 15:22:30.000000 pysoundanalyser-0.3.1/pysoundanalyser/__main__.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)      107 2023-06-04 05:18:34.000000 pysoundanalyser-0.3.1/pysoundanalyser/_version_info.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    13121 2023-05-20 15:42:12.000000 pysoundanalyser-0.3.1/pysoundanalyser/audio_manager.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    11329 2023-05-20 15:31:32.000000 pysoundanalyser-0.3.1/pysoundanalyser/dialog_apply_filter.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     1993 2023-05-08 21:53:20.000000 pysoundanalyser-0.3.1/pysoundanalyser/dialog_change_channel.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     4556 2023-05-20 15:31:53.000000 pysoundanalyser-0.3.1/pysoundanalyser/dialog_concatenate.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     2832 2023-05-20 15:32:08.000000 pysoundanalyser-0.3.1/pysoundanalyser/dialog_cut.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    24487 2023-05-20 17:31:33.000000 pysoundanalyser-0.3.1/pysoundanalyser/dialog_edit_preferences.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     5932 2023-05-20 15:32:35.000000 pysoundanalyser-0.3.1/pysoundanalyser/dialog_generate_noise.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     8214 2023-05-20 15:41:21.000000 pysoundanalyser-0.3.1/pysoundanalyser/dialog_generate_sinusoid.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    34378 2023-05-20 15:32:58.000000 pysoundanalyser-0.3.1/pysoundanalyser/dialog_generate_sound.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     6397 2023-05-20 15:33:11.000000 pysoundanalyser-0.3.1/pysoundanalyser/dialog_get_font.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     3684 2023-05-20 15:33:26.000000 pysoundanalyser-0.3.1/pysoundanalyser/dialog_resample.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     3287 2023-05-08 21:46:08.000000 pysoundanalyser-0.3.1/pysoundanalyser/dialog_save_sound.py
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-04 05:19:13.026744 pysoundanalyser-0.3.1/pysoundanalyser/doc/
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     6798 2015-09-27 14:16:12.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/Makefile
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-04 05:19:12.678738 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-04 05:19:13.041744 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      230 2019-02-12 13:02:01.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/.buildinfo
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-04 05:19:13.070745 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_sources/
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-04 05:19:13.071745 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_sources/_themes/
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     4140 2013-11-05 23:17:09.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_sources/_themes/README.txt
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      492 2015-10-02 01:14:58.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_sources/index.txt
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     9116 2015-10-02 01:25:42.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_sources/installation.txt
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      776 2015-10-02 01:14:16.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_sources/intro.txt
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     2919 2015-10-11 12:56:35.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_sources/user_interface.txt
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-04 05:19:13.462752 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_static/
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      673 2016-11-23 13:34:54.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_static/ajax-loader.gif
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     9740 2019-02-12 13:02:01.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_static/basic.css
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     3500 2016-12-11 08:42:43.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_static/comment-bright.png
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     3578 2016-12-11 08:42:43.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_static/comment-close.png
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     3445 2016-12-11 08:42:43.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_static/comment.png
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-04 05:19:13.464752 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_static/css/
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     2992 2013-11-05 23:17:09.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_static/css/badge_only.css
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    85310 2013-11-07 20:43:01.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_static/css/theme.css
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     4040 2015-09-28 09:22:00.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_static/default.css
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     8166 2019-02-12 13:02:01.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_static/doctools.js
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      347 2016-12-11 08:42:43.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_static/down-pressed.png
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      347 2016-12-11 08:42:43.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_static/down.png
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      358 2016-12-11 08:42:43.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_static/file.png
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-04 05:19:13.471752 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_static/font/
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    37405 2013-11-04 18:50:23.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_static/font/fontawesome_webfont.eot
--rw-rwsr--   0 sam       (1000) extdrive  (1777)   197829 2013-11-04 18:50:23.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_static/font/fontawesome_webfont.svg
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    79076 2013-11-04 18:50:23.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_static/font/fontawesome_webfont.ttf
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    43572 2013-11-04 18:50:23.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_static/font/fontawesome_webfont.woff
--rw-rwsr--   0 sam       (1000) extdrive  (1777)   282766 2015-03-10 21:52:53.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_static/jquery-1.11.1.js
--rw-rwsr--   0 sam       (1000) extdrive  (1777)   267180 2016-12-11 15:18:53.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_static/jquery.js
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-04 05:19:13.472752 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_static/js/
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      709 2013-11-04 18:50:23.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_static/js/theme.js
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      173 2016-12-11 08:42:43.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_static/minus.png
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      173 2016-12-11 08:42:43.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_static/plus.png
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     4395 2019-02-12 13:02:01.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_static/pygments.css
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    24991 2019-02-12 13:02:01.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_static/searchtools.js
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     4803 2015-09-28 09:22:00.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_static/sidebar.js
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    35168 2015-03-10 21:52:53.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_static/underscore-1.3.1.js
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    52919 2015-04-02 15:32:01.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_static/underscore.js
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      345 2016-12-11 08:42:43.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_static/up-pressed.png
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      345 2016-12-11 08:42:43.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_static/up.png
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    25351 2016-11-23 13:34:54.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_static/websupport.js
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-04 05:19:13.473752 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_themes/
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    12474 2019-02-12 13:02:01.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_themes/README.html
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     4010 2019-02-12 13:02:01.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/genindex.html
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     6091 2019-02-12 13:02:01.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/index.html
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    23011 2019-02-12 13:02:01.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/installation.html
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     5857 2019-02-12 13:02:01.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/intro.html
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      409 2019-02-12 13:02:01.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/objects.inv
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     4426 2019-02-12 13:02:01.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/search.html
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     4934 2019-02-12 13:02:01.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/searchindex.js
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     9932 2019-02-12 13:02:01.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/user_interface.html
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-04 05:19:13.474752 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/latex/
--rw-rwsr--   0 sam       (1000) extdrive  (1777)   135313 2020-05-28 09:35:28.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/latex/pysoundanalyser.pdf
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-04 05:19:13.563753 pysoundanalyser-0.3.1/pysoundanalyser/doc/_themes/
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     1078 2013-10-23 20:03:11.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_themes/LICENSE
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      360 2013-11-04 22:53:08.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_themes/MANIFEST.in
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     5940 2013-11-07 20:43:24.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_themes/PKG-INFO
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     4140 2013-11-05 23:17:09.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_themes/README.rst
--rw-rwsr--   0 sam       (1000) extdrive  (1777)       12 2013-11-04 18:50:23.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_themes/requirements.txt
--rw-rwsr--   0 sam       (1000) extdrive  (1777)       59 2013-11-07 20:43:24.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_themes/setup.cfg
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     1313 2013-11-04 23:11:48.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_themes/setup.py
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-04 05:19:13.846758 pysoundanalyser-0.3.1/pysoundanalyser/doc/_themes/sphinx_rtd_theme/
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      371 2013-11-07 20:43:12.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_themes/sphinx_rtd_theme/__init__.py
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      408 2013-11-04 18:50:23.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_themes/sphinx_rtd_theme/breadcrumbs.html
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     1166 2013-11-05 23:17:09.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_themes/sphinx_rtd_theme/footer.html
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     4512 2013-11-05 23:49:34.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_themes/sphinx_rtd_theme/layout.html
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     7341 2013-11-04 18:50:23.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_themes/sphinx_rtd_theme/layout_old.html
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     1533 2013-11-04 18:50:23.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_themes/sphinx_rtd_theme/search.html
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      249 2013-11-04 18:50:23.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_themes/sphinx_rtd_theme/searchbox.html
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-04 05:19:12.679738 pysoundanalyser-0.3.1/pysoundanalyser/doc/_themes/sphinx_rtd_theme/static/
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-04 05:19:13.851759 pysoundanalyser-0.3.1/pysoundanalyser/doc/_themes/sphinx_rtd_theme/static/css/
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     2992 2013-11-05 23:17:09.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_themes/sphinx_rtd_theme/static/css/badge_only.css
--rw-rwsr--   0 sam       (1000) extdrive  (1777)    85310 2013-11-07 20:43:01.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_themes/sphinx_rtd_theme/static/css/theme.css
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-04 05:19:13.885759 pysoundanalyser-0.3.1/pysoundanalyser/doc/_themes/sphinx_rtd_theme/static/font/
--rwxrwsr-x   0 sam       (1000) extdrive  (1777)    37405 2013-11-04 18:50:23.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_themes/sphinx_rtd_theme/static/font/fontawesome_webfont.eot
--rwxrwsr-x   0 sam       (1000) extdrive  (1777)   197829 2013-11-04 18:50:23.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_themes/sphinx_rtd_theme/static/font/fontawesome_webfont.svg
--rwxrwsr-x   0 sam       (1000) extdrive  (1777)    79076 2013-11-04 18:50:23.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_themes/sphinx_rtd_theme/static/font/fontawesome_webfont.ttf
--rwxrwsr-x   0 sam       (1000) extdrive  (1777)    43572 2013-11-04 18:50:23.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_themes/sphinx_rtd_theme/static/font/fontawesome_webfont.woff
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-04 05:19:13.886759 pysoundanalyser-0.3.1/pysoundanalyser/doc/_themes/sphinx_rtd_theme/static/js/
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      709 2013-11-04 18:50:23.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_themes/sphinx_rtd_theme/static/js/theme.js
--rw-rwsr--   0 sam       (1000) extdrive  (1777)       99 2013-11-04 18:50:23.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_themes/sphinx_rtd_theme/theme.conf
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     1194 2013-11-04 19:43:38.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_themes/sphinx_rtd_theme/versions.html
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-04 05:19:13.850758 pysoundanalyser-0.3.1/pysoundanalyser/doc/_themes/sphinx_rtd_theme.egg-info/
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     5940 2013-11-07 20:43:24.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_themes/sphinx_rtd_theme.egg-info/PKG-INFO
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      898 2013-11-07 20:43:24.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_themes/sphinx_rtd_theme.egg-info/SOURCES.txt
--rw-rwsr--   0 sam       (1000) extdrive  (1777)        1 2013-11-07 20:43:24.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_themes/sphinx_rtd_theme.egg-info/dependency_links.txt
--rw-rwsr--   0 sam       (1000) extdrive  (1777)        1 2013-11-04 00:23:45.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_themes/sphinx_rtd_theme.egg-info/not-zip-safe
--rw-rwsr--   0 sam       (1000) extdrive  (1777)       11 2013-11-07 20:43:24.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_themes/sphinx_rtd_theme.egg-info/requires.txt
--rw-rwsr--   0 sam       (1000) extdrive  (1777)       17 2013-11-07 20:43:24.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/_themes/sphinx_rtd_theme.egg-info/top_level.txt
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    10721 2023-06-04 05:18:34.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/conf.py
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      492 2015-10-02 01:14:58.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/index.rst
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     1277 2023-06-04 05:16:14.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/installation.rst
--rw-rwsr--   0 sam       (1000) extdrive  (1777)      776 2015-10-02 01:14:16.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/intro.rst
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     6719 2015-09-27 14:16:12.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/make.bat
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-04 05:19:13.922760 pysoundanalyser-0.3.1/pysoundanalyser/doc/manual/
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)      795 2013-02-19 12:34:49.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/manual/intro.aux
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)      125 2013-02-08 23:15:43.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/manual/intro.tex
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)      461 2013-02-19 12:34:49.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/manual/pysoundanalyser_manual.aux
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)        0 2013-02-19 12:34:49.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/manual/pysoundanalyser_manual.idx
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)    15637 2013-02-19 12:34:49.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/manual/pysoundanalyser_manual.log
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)       94 2013-02-19 12:34:49.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/manual/pysoundanalyser_manual.out
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)    63703 2013-02-19 12:34:49.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/manual/pysoundanalyser_manual.pdf
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)     2083 2013-02-19 12:34:51.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/manual/pysoundanalyser_manual.tex
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)      297 2013-02-19 12:34:49.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/manual/pysoundanalyser_manual.toc
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)      752 2013-02-08 23:16:03.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/manual/texput.log
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)      638 2013-02-19 12:34:49.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/manual/titlepage.aux
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)     1248 2013-02-08 23:15:26.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/manual/titlepage.tex
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)     1021 2013-02-19 12:34:49.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/manual/user_interface.aux
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)     2038 2013-02-08 23:16:00.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/manual/user_interface.tex
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)      103 2015-09-27 14:19:28.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/mkdoc.sh
--rw-rwsr--   0 sam       (1000) extdrive  (1777)     2919 2015-10-11 12:56:35.000000 pysoundanalyser-0.3.1/pysoundanalyser/doc/user_interface.rst
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    11077 2023-05-21 07:35:18.000000 pysoundanalyser-0.3.1/pysoundanalyser/global_parameters.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)       41 2023-06-03 15:43:28.000000 pysoundanalyser-0.3.1/pysoundanalyser/pyqtver.py
--rw-rw-r--   0 sam       (1000) extdrive  (1777)   108155 2023-06-03 15:43:28.000000 pysoundanalyser-0.3.1/pysoundanalyser/qrc_resources.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     1296 2023-04-30 11:36:30.000000 pysoundanalyser-0.3.1/pysoundanalyser/random_id.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)   171752 2023-04-30 11:36:45.000000 pysoundanalyser-0.3.1/pysoundanalyser/sndlib.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     1598 2023-04-30 11:36:57.000000 pysoundanalyser-0.3.1/pysoundanalyser/threaded_plotters.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     1432 2023-04-30 11:37:09.000000 pysoundanalyser-0.3.1/pysoundanalyser/utilities_open_manual.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    10331 2023-05-20 14:57:23.000000 pysoundanalyser-0.3.1/pysoundanalyser/utility_functions.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    10419 2023-05-09 07:48:46.000000 pysoundanalyser-0.3.1/pysoundanalyser/wavpy.py
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     2953 2023-05-08 10:12:35.000000 pysoundanalyser-0.3.1/pysoundanalyser/wavpy_sndf.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     7514 2023-05-20 15:34:46.000000 pysoundanalyser-0.3.1/pysoundanalyser/win_acf_plot.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     9305 2023-05-20 15:34:59.000000 pysoundanalyser-0.3.1/pysoundanalyser/win_autocorrelogram_plot.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    20600 2023-05-20 15:35:22.000000 pysoundanalyser-0.3.1/pysoundanalyser/win_generic_plot.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    11904 2023-05-20 15:35:37.000000 pysoundanalyser-0.3.1/pysoundanalyser/win_spectrogram_plot.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     8447 2023-05-20 15:35:51.000000 pysoundanalyser-0.3.1/pysoundanalyser/win_spectrum_plot.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     5635 2023-05-20 15:36:13.000000 pysoundanalyser-0.3.1/pysoundanalyser/win_waveform_plot.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)      397 2023-06-04 05:18:34.000000 pysoundanalyser-0.3.1/pysoundanalyser.desktop
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-04 05:19:13.006744 pysoundanalyser-0.3.1/pysoundanalyser.egg-info/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    42068 2023-06-04 05:19:12.000000 pysoundanalyser-0.3.1/pysoundanalyser.egg-info/PKG-INFO
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     7958 2023-06-04 05:19:12.000000 pysoundanalyser-0.3.1/pysoundanalyser.egg-info/SOURCES.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)        1 2023-06-04 05:19:12.000000 pysoundanalyser-0.3.1/pysoundanalyser.egg-info/dependency_links.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       62 2023-06-04 05:19:12.000000 pysoundanalyser-0.3.1/pysoundanalyser.egg-info/entry_points.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       86 2023-06-04 05:19:12.000000 pysoundanalyser-0.3.1/pysoundanalyser.egg-info/requires.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       16 2023-06-04 05:19:12.000000 pysoundanalyser-0.3.1/pysoundanalyser.egg-info/top_level.txt
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)      547 2013-02-19 11:18:49.000000 pysoundanalyser-0.3.1/resources.qrc
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-04 05:19:13.923760 pysoundanalyser-0.3.1/scripts/
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)       94 2015-10-11 12:48:00.000000 pysoundanalyser-0.3.1/scripts/pysoundanalyser-launcher.bat
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       38 2023-06-04 05:19:13.930760 pysoundanalyser-0.3.1/setup.cfg
-drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-04 05:19:13.928760 pysoundanalyser-0.3.1/translations/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       16 2023-06-03 15:43:32.000000 pysoundanalyser-0.3.1/translations/pysoundanalyser_de.qm
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       16 2023-06-03 15:43:32.000000 pysoundanalyser-0.3.1/translations/pysoundanalyser_el.qm
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      122 2023-06-03 15:43:32.000000 pysoundanalyser-0.3.1/translations/pysoundanalyser_en_GB.qm
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       16 2023-06-03 15:43:32.000000 pysoundanalyser-0.3.1/translations/pysoundanalyser_es.qm
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      235 2023-06-03 15:43:32.000000 pysoundanalyser-0.3.1/translations/pysoundanalyser_fr.qm
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    28965 2023-06-03 15:43:32.000000 pysoundanalyser-0.3.1/translations/pysoundanalyser_it.qm
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)    17558 2013-02-19 23:27:27.000000 pysoundanalyser-0.3.1/translations/pysoundanalyser_it_IT.qm
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       44 2023-06-03 15:43:32.000000 pysoundanalyser-0.3.1/translations/pysoundanalyser_ru.qm
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:15:05.422191 pysoundanalyser-0.3.2/
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    35147 2010-06-04 09:15:48.000000 pysoundanalyser-0.3.2/COPYING.txt
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)      183 2015-11-13 01:18:22.000000 pysoundanalyser-0.3.2/CREDITS.txt
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)       71 2015-09-08 22:01:46.000000 pysoundanalyser-0.3.2/INSTALL.txt
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)      696 2023-06-03 16:00:04.000000 pysoundanalyser-0.3.2/MANIFEST.in
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    42068 2023-06-05 08:15:05.422191 pysoundanalyser-0.3.2/PKG-INFO
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)      370 2022-07-18 13:01:39.000000 pysoundanalyser-0.3.2/README.md
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:15:05.176185 pysoundanalyser-0.3.2/icons/
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    16622 2011-11-01 10:05:06.000000 pysoundanalyser-0.3.2/icons/exit.svg
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    24750 2012-04-19 09:34:44.000000 pysoundanalyser-0.3.2/icons/johnny_automatic_crashing_wave.ico
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)    45168 2015-09-29 11:52:50.000000 pysoundanalyser-0.3.2/icons/johnny_automatic_crashing_wave.png
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    14143 2010-05-31 11:23:42.000000 pysoundanalyser-0.3.2/icons/johnny_automatic_crashing_wave.svg
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:15:05.208185 pysoundanalyser-0.3.2/prep-release/
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:15:05.259187 pysoundanalyser-0.3.2/prep-release/debian/
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     9879 2020-05-28 09:36:16.000000 pysoundanalyser-0.3.2/prep-release/debian/changelog
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)        2 2012-12-17 22:35:36.000000 pysoundanalyser-0.3.2/prep-release/debian/compat
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)      849 2015-09-21 10:20:50.000000 pysoundanalyser-0.3.2/prep-release/debian/control
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     1101 2013-02-08 13:13:12.000000 pysoundanalyser-0.3.2/prep-release/debian/copyright
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)        5 2013-02-08 11:05:31.000000 pysoundanalyser-0.3.2/prep-release/debian/docs
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)       71 2013-02-08 13:42:44.000000 pysoundanalyser-0.3.2/prep-release/debian/links
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)      745 2013-02-08 11:36:14.000000 pysoundanalyser-0.3.2/prep-release/debian/rules
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:15:03.694146 pysoundanalyser-0.3.2/prep-release/launchpad/
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:15:05.357189 pysoundanalyser-0.3.2/prep-release/launchpad/debian/
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    10985 2020-05-28 13:40:27.000000 pysoundanalyser-0.3.2/prep-release/launchpad/debian/changelog
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)        2 2012-12-17 22:35:36.000000 pysoundanalyser-0.3.2/prep-release/launchpad/debian/compat
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     1077 2020-05-28 13:40:20.000000 pysoundanalyser-0.3.2/prep-release/launchpad/debian/control
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     1101 2013-02-08 13:13:12.000000 pysoundanalyser-0.3.2/prep-release/launchpad/debian/copyright
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)        5 2013-02-08 11:05:31.000000 pysoundanalyser-0.3.2/prep-release/launchpad/debian/docs
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)       71 2013-02-08 13:42:44.000000 pysoundanalyser-0.3.2/prep-release/launchpad/debian/links
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)      745 2013-02-08 11:36:14.000000 pysoundanalyser-0.3.2/prep-release/launchpad/debian/rules
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     2171 2020-05-28 13:36:12.000000 pysoundanalyser-0.3.2/prep-release/launchpad_build.py
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)     3051 2015-10-13 17:39:53.000000 pysoundanalyser-0.3.2/prep-release/make_deb.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)        1 2023-06-05 08:12:44.000000 pysoundanalyser-0.3.2/prep-release/minor_minor_number.txt
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)      178 2022-09-23 15:23:28.000000 pysoundanalyser-0.3.2/prep-release/mkupdate_pyqt5.sh
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     1122 2023-06-03 15:25:11.000000 pysoundanalyser-0.3.2/prep-release/mkupdate_pyqt6.sh
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     1185 2023-06-03 15:23:52.000000 pysoundanalyser-0.3.2/prep-release/pysoundanalyser.pro
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    77407 2023-06-03 15:43:28.000000 pysoundanalyser-0.3.2/prep-release/pysoundanalyser_de.ts
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    77407 2023-06-03 15:43:28.000000 pysoundanalyser-0.3.2/prep-release/pysoundanalyser_el.ts
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    77435 2023-06-03 15:43:28.000000 pysoundanalyser-0.3.2/prep-release/pysoundanalyser_en_GB.ts
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    77407 2023-06-03 15:43:28.000000 pysoundanalyser-0.3.2/prep-release/pysoundanalyser_es.ts
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    79000 2023-06-03 15:43:28.000000 pysoundanalyser-0.3.2/prep-release/pysoundanalyser_fr.ts
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    93371 2023-06-03 15:43:28.000000 pysoundanalyser-0.3.2/prep-release/pysoundanalyser_it.ts
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    77424 2023-06-03 15:43:28.000000 pysoundanalyser-0.3.2/prep-release/pysoundanalyser_ru.ts
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     2652 2023-06-05 08:14:40.000000 pysoundanalyser-0.3.2/prep-release/release.py
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      937 2023-05-20 14:38:46.000000 pysoundanalyser-0.3.2/prep-release/switch_pyqt5.py
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      937 2023-05-20 14:37:31.000000 pysoundanalyser-0.3.2/prep-release/switch_pyqt6.py
+-rw-rwsr--   0 sam       (1000) extdrive  (1777)     2875 2019-02-12 09:45:06.000000 pysoundanalyser-0.3.2/prep-release/uploadToWebsite.py
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     1527 2023-06-05 08:12:44.000000 pysoundanalyser-0.3.2/pyproject.toml
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:15:05.382190 pysoundanalyser-0.3.2/pysoundanalyser/
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)        0 2008-10-28 02:30:54.000000 pysoundanalyser-0.3.2/pysoundanalyser/__init__.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    80415 2023-06-03 15:22:30.000000 pysoundanalyser-0.3.2/pysoundanalyser/__main__.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)      107 2023-06-05 08:12:44.000000 pysoundanalyser-0.3.2/pysoundanalyser/_version_info.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    13121 2023-05-20 15:42:12.000000 pysoundanalyser-0.3.2/pysoundanalyser/audio_manager.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    11329 2023-05-20 15:31:32.000000 pysoundanalyser-0.3.2/pysoundanalyser/dialog_apply_filter.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     1993 2023-05-08 21:53:20.000000 pysoundanalyser-0.3.2/pysoundanalyser/dialog_change_channel.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     4556 2023-05-20 15:31:53.000000 pysoundanalyser-0.3.2/pysoundanalyser/dialog_concatenate.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     2832 2023-05-20 15:32:08.000000 pysoundanalyser-0.3.2/pysoundanalyser/dialog_cut.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    24487 2023-05-20 17:31:33.000000 pysoundanalyser-0.3.2/pysoundanalyser/dialog_edit_preferences.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     5932 2023-05-20 15:32:35.000000 pysoundanalyser-0.3.2/pysoundanalyser/dialog_generate_noise.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     8214 2023-05-20 15:41:21.000000 pysoundanalyser-0.3.2/pysoundanalyser/dialog_generate_sinusoid.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    34378 2023-05-20 15:32:58.000000 pysoundanalyser-0.3.2/pysoundanalyser/dialog_generate_sound.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     6397 2023-05-20 15:33:11.000000 pysoundanalyser-0.3.2/pysoundanalyser/dialog_get_font.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     3684 2023-05-20 15:33:26.000000 pysoundanalyser-0.3.2/pysoundanalyser/dialog_resample.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     3287 2023-05-08 21:46:08.000000 pysoundanalyser-0.3.2/pysoundanalyser/dialog_save_sound.py
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:15:05.386190 pysoundanalyser-0.3.2/pysoundanalyser/doc/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      634 2023-06-04 19:54:36.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/Makefile
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:15:03.696147 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:15:05.389190 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      230 2023-06-05 08:13:40.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/.buildinfo
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:15:05.391190 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_sources/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      503 2023-06-04 19:56:26.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_sources/index.rst.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     1277 2023-06-04 05:16:14.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_sources/installation.rst.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      776 2015-10-02 01:14:16.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_sources/intro.rst.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     2919 2015-10-11 12:56:35.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_sources/user_interface.rst.txt
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:15:05.400190 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4418 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    11185 2023-06-04 19:56:48.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/alabaster.css
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     1128 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/alert_info_32.png
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      944 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/alert_warning_32.png
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       78 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/background_b01.png
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    14810 2023-06-05 08:13:40.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/basic.css
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       82 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/bg-page.png
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     9827 2023-06-04 20:00:44.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/bizstyle.css
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     1145 2023-06-04 20:00:44.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/bizstyle.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      165 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/bullet_orange.png
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      107 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/contents.png
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:15:05.401190 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/css/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     3303 2023-02-08 21:25:43.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/css/badge_only.css
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)   138354 2023-02-08 21:25:43.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/css/theme.css
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    14940 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/css3-mediaqueries.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       42 2017-05-15 18:58:47.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/custom.css
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4472 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/doctools.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      420 2023-06-05 08:13:40.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/documentation_options.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      286 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/file.png
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4787 2021-06-13 20:25:40.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/forkme_right_darkblue_121621.png
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     6714 2023-06-04 19:58:28.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/haiku.css
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)   289782 2022-08-29 08:27:59.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/jquery.js
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:15:05.401190 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/js/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     9478 2023-02-08 21:25:43.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/js/theme.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4758 2023-06-05 08:13:40.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/language_data.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       90 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/minus.png
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      120 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/navigation.png
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       90 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/plus.png
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4819 2023-06-05 08:13:40.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/pygments.css
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    18747 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/searchtools.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     5097 2023-03-29 08:31:27.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/sphinx_highlight.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     6263 2023-06-04 20:00:19.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/sphinxdoc.css
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    68416 2022-06-02 12:39:04.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/underscore.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     3668 2023-06-05 08:13:40.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/genindex.html
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     5481 2023-06-05 08:13:40.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/index.html
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     6262 2023-06-05 08:13:40.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/installation.html
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     5815 2023-06-05 08:13:40.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/intro.html
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      351 2023-06-05 08:13:40.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/objects.inv
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4067 2023-06-05 08:13:40.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/search.html
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4231 2023-06-05 08:13:40.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/searchindex.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     9618 2023-06-05 08:13:40.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/user_interface.html
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:15:05.402190 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/latex/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)   144787 2023-06-05 08:13:42.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/latex/pysoundanalyser.pdf
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      989 2023-06-05 08:13:31.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/conf.py
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      503 2023-06-04 19:56:26.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/index.rst
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     1277 2023-06-04 05:16:14.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/installation.rst
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      776 2015-10-02 01:14:16.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/intro.rst
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      800 2023-06-04 19:54:36.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/make.bat
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)      103 2015-09-27 14:19:28.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/mkdoc.sh
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     2919 2015-10-11 12:56:35.000000 pysoundanalyser-0.3.2/pysoundanalyser/doc/user_interface.rst
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    11077 2023-05-21 07:35:18.000000 pysoundanalyser-0.3.2/pysoundanalyser/global_parameters.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)       41 2023-06-04 19:54:17.000000 pysoundanalyser-0.3.2/pysoundanalyser/pyqtver.py
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)   108155 2023-06-03 15:43:28.000000 pysoundanalyser-0.3.2/pysoundanalyser/qrc_resources.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     1296 2023-04-30 11:36:30.000000 pysoundanalyser-0.3.2/pysoundanalyser/random_id.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)   171752 2023-04-30 11:36:45.000000 pysoundanalyser-0.3.2/pysoundanalyser/sndlib.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     1598 2023-04-30 11:36:57.000000 pysoundanalyser-0.3.2/pysoundanalyser/threaded_plotters.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     1432 2023-04-30 11:37:09.000000 pysoundanalyser-0.3.2/pysoundanalyser/utilities_open_manual.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    10331 2023-05-20 14:57:23.000000 pysoundanalyser-0.3.2/pysoundanalyser/utility_functions.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    10419 2023-05-09 07:48:46.000000 pysoundanalyser-0.3.2/pysoundanalyser/wavpy.py
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     2953 2023-05-08 10:12:35.000000 pysoundanalyser-0.3.2/pysoundanalyser/wavpy_sndf.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     7514 2023-05-20 15:34:46.000000 pysoundanalyser-0.3.2/pysoundanalyser/win_acf_plot.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     9305 2023-05-20 15:34:59.000000 pysoundanalyser-0.3.2/pysoundanalyser/win_autocorrelogram_plot.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    20600 2023-05-20 15:35:22.000000 pysoundanalyser-0.3.2/pysoundanalyser/win_generic_plot.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    11904 2023-05-20 15:35:37.000000 pysoundanalyser-0.3.2/pysoundanalyser/win_spectrogram_plot.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     8447 2023-05-20 15:35:51.000000 pysoundanalyser-0.3.2/pysoundanalyser/win_spectrum_plot.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     5635 2023-05-20 15:36:13.000000 pysoundanalyser-0.3.2/pysoundanalyser/win_waveform_plot.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)      397 2023-06-05 08:12:44.000000 pysoundanalyser-0.3.2/pysoundanalyser.desktop
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:15:05.384190 pysoundanalyser-0.3.2/pysoundanalyser.egg-info/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    42068 2023-06-05 08:15:03.000000 pysoundanalyser-0.3.2/pysoundanalyser.egg-info/PKG-INFO
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     5590 2023-06-05 08:15:03.000000 pysoundanalyser-0.3.2/pysoundanalyser.egg-info/SOURCES.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)        1 2023-06-05 08:15:03.000000 pysoundanalyser-0.3.2/pysoundanalyser.egg-info/dependency_links.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       62 2023-06-05 08:15:03.000000 pysoundanalyser-0.3.2/pysoundanalyser.egg-info/entry_points.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       86 2023-06-05 08:15:03.000000 pysoundanalyser-0.3.2/pysoundanalyser.egg-info/requires.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       16 2023-06-05 08:15:03.000000 pysoundanalyser-0.3.2/pysoundanalyser.egg-info/top_level.txt
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)      547 2013-02-19 11:18:49.000000 pysoundanalyser-0.3.2/resources.qrc
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:15:05.403190 pysoundanalyser-0.3.2/scripts/
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)       94 2015-10-11 12:48:00.000000 pysoundanalyser-0.3.2/scripts/pysoundanalyser-launcher.bat
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       38 2023-06-05 08:15:05.422191 pysoundanalyser-0.3.2/setup.cfg
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2023-06-05 08:15:05.421191 pysoundanalyser-0.3.2/translations/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       16 2023-06-03 15:43:32.000000 pysoundanalyser-0.3.2/translations/pysoundanalyser_de.qm
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       16 2023-06-03 15:43:32.000000 pysoundanalyser-0.3.2/translations/pysoundanalyser_el.qm
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      122 2023-06-03 15:43:32.000000 pysoundanalyser-0.3.2/translations/pysoundanalyser_en_GB.qm
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       16 2023-06-03 15:43:32.000000 pysoundanalyser-0.3.2/translations/pysoundanalyser_es.qm
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      235 2023-06-03 15:43:32.000000 pysoundanalyser-0.3.2/translations/pysoundanalyser_fr.qm
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    28965 2023-06-03 15:43:32.000000 pysoundanalyser-0.3.2/translations/pysoundanalyser_it.qm
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)    17558 2013-02-19 23:27:27.000000 pysoundanalyser-0.3.2/translations/pysoundanalyser_it_IT.qm
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       44 2023-06-03 15:43:32.000000 pysoundanalyser-0.3.2/translations/pysoundanalyser_ru.qm
```

### Comparing `pysoundanalyser-0.3.1/COPYING.txt` & `pysoundanalyser-0.3.2/COPYING.txt`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/MANIFEST.in` & `pysoundanalyser-0.3.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/PKG-INFO` & `pysoundanalyser-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysoundanalyser
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python program for visualizing short sounds (waveform, spectrum, etc...)
 Author-email: Samuele Carcagno <sam.carcagno@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pysoundanalyser-0.3.1/icons/exit.svg` & `pysoundanalyser-0.3.2/icons/exit.svg`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/icons/johnny_automatic_crashing_wave.ico` & `pysoundanalyser-0.3.2/icons/johnny_automatic_crashing_wave.ico`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/icons/johnny_automatic_crashing_wave.png` & `pysoundanalyser-0.3.2/icons/johnny_automatic_crashing_wave.png`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/icons/johnny_automatic_crashing_wave.svg` & `pysoundanalyser-0.3.2/icons/johnny_automatic_crashing_wave.svg`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/prep-release/debian/changelog` & `pysoundanalyser-0.3.2/prep-release/debian/changelog`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/prep-release/debian/control` & `pysoundanalyser-0.3.2/prep-release/debian/control`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/prep-release/debian/copyright` & `pysoundanalyser-0.3.2/prep-release/debian/copyright`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/prep-release/debian/rules` & `pysoundanalyser-0.3.2/prep-release/debian/rules`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/prep-release/launchpad/debian/changelog` & `pysoundanalyser-0.3.2/prep-release/launchpad/debian/changelog`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/prep-release/launchpad/debian/control` & `pysoundanalyser-0.3.2/prep-release/launchpad/debian/control`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/prep-release/launchpad/debian/copyright` & `pysoundanalyser-0.3.2/prep-release/launchpad/debian/copyright`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/prep-release/launchpad/debian/rules` & `pysoundanalyser-0.3.2/prep-release/launchpad/debian/rules`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/prep-release/launchpad_build.py` & `pysoundanalyser-0.3.2/prep-release/launchpad_build.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/prep-release/make_deb.py` & `pysoundanalyser-0.3.2/prep-release/make_deb.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/prep-release/mkupdate_pyqt6.sh` & `pysoundanalyser-0.3.2/prep-release/mkupdate_pyqt6.sh`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/prep-release/pysoundanalyser.pro` & `pysoundanalyser-0.3.2/prep-release/pysoundanalyser.pro`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/prep-release/pysoundanalyser_de.ts` & `pysoundanalyser-0.3.2/prep-release/pysoundanalyser_de.ts`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/prep-release/pysoundanalyser_el.ts` & `pysoundanalyser-0.3.2/prep-release/pysoundanalyser_el.ts`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/prep-release/pysoundanalyser_en_GB.ts` & `pysoundanalyser-0.3.2/prep-release/pysoundanalyser_en_GB.ts`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/prep-release/pysoundanalyser_es.ts` & `pysoundanalyser-0.3.2/prep-release/pysoundanalyser_es.ts`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/prep-release/pysoundanalyser_fr.ts` & `pysoundanalyser-0.3.2/prep-release/pysoundanalyser_fr.ts`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/prep-release/pysoundanalyser_it.ts` & `pysoundanalyser-0.3.2/prep-release/pysoundanalyser_it.ts`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/prep-release/pysoundanalyser_ru.ts` & `pysoundanalyser-0.3.2/prep-release/pysoundanalyser_ru.ts`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/prep-release/release.py` & `pysoundanalyser-0.3.2/prep-release/release.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,17 +56,17 @@
 
 
     f = open('pysoundanalyser/doc/conf.py', 'r')
     ln = f.readlines()
     f.close()
     for i in range(len(ln)):
         if ln[i].strip().split('=')[0].strip() == "version":
-            ln[i] = 'version = "' + gittag +'",\n'
+            ln[i] = 'version = "' + gittag +'"\n'
         if ln[i].strip().split('=')[0].strip() == "release":
-            ln[i] = 'release = "' + gittag + '",\n'
+            ln[i] = 'release = "' + gittag + '"\n'
 
     f = open('pysoundanalyser/doc/conf.py', 'w')
     f.writelines(ln)
     f.close()
 
     f = open('pysoundanalyser.desktop', 'r')
     ln = f.readlines()
```

### Comparing `pysoundanalyser-0.3.1/prep-release/switch_pyqt5.py` & `pysoundanalyser-0.3.2/prep-release/switch_pyqt5.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/prep-release/switch_pyqt6.py` & `pysoundanalyser-0.3.2/prep-release/switch_pyqt6.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/prep-release/uploadToWebsite.py` & `pysoundanalyser-0.3.2/prep-release/uploadToWebsite.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/pyproject.toml` & `pysoundanalyser-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pysoundanalyser"
-    version="0.3.1"
+    version="0.3.2"
 
 authors = [
   { name="Samuele Carcagno", email="sam.carcagno@gmail.com" },
 ]
 description = "Python program for visualizing short sounds (waveform, spectrum, etc...)"
 license = {file = "COPYING.txt"}
 readme = "README.md"
```

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/__main__.py` & `pysoundanalyser-0.3.2/pysoundanalyser/__main__.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/audio_manager.py` & `pysoundanalyser-0.3.2/pysoundanalyser/audio_manager.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/dialog_apply_filter.py` & `pysoundanalyser-0.3.2/pysoundanalyser/dialog_apply_filter.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/dialog_change_channel.py` & `pysoundanalyser-0.3.2/pysoundanalyser/dialog_change_channel.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/dialog_concatenate.py` & `pysoundanalyser-0.3.2/pysoundanalyser/dialog_concatenate.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/dialog_cut.py` & `pysoundanalyser-0.3.2/pysoundanalyser/dialog_cut.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/dialog_edit_preferences.py` & `pysoundanalyser-0.3.2/pysoundanalyser/dialog_edit_preferences.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/dialog_generate_noise.py` & `pysoundanalyser-0.3.2/pysoundanalyser/dialog_generate_noise.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/dialog_generate_sinusoid.py` & `pysoundanalyser-0.3.2/pysoundanalyser/dialog_generate_sinusoid.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/dialog_generate_sound.py` & `pysoundanalyser-0.3.2/pysoundanalyser/dialog_generate_sound.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/dialog_get_font.py` & `pysoundanalyser-0.3.2/pysoundanalyser/dialog_get_font.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/dialog_resample.py` & `pysoundanalyser-0.3.2/pysoundanalyser/dialog_resample.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/dialog_save_sound.py` & `pysoundanalyser-0.3.2/pysoundanalyser/dialog_save_sound.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_sources/intro.txt` & `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_sources/intro.rst.txt`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_sources/user_interface.txt` & `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_sources/user_interface.rst.txt`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_static/css/badge_only.css` & `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/css/badge_only.css`

 * *Files 16% similar despite different names*

```diff
@@ -1 +1 @@
-.font-smooth,.icon:before{-webkit-font-smoothing:antialiased}.clearfix{*zoom:1}.clearfix:before,.clearfix:after{display:table;content:""}.clearfix:after{clear:both}@font-face{font-family:fontawesome-webfont;font-weight:normal;font-style:normal;src:url("../font/fontawesome_webfont.eot");src:url("../font/fontawesome_webfont.eot?#iefix") format("embedded-opentype"),url("../font/fontawesome_webfont.woff") format("woff"),url("../font/fontawesome_webfont.ttf") format("truetype"),url("../font/fontawesome_webfont.svg#fontawesome-webfont") format("svg")}.icon:before{display:inline-block;font-family:fontawesome-webfont;font-style:normal;font-weight:normal;line-height:1;text-decoration:inherit}a .icon{display:inline-block;text-decoration:inherit}li .icon{display:inline-block}li .icon-large:before,li .icon-large:before{width:1.875em}ul.icons{list-style-type:none;margin-left:2em;text-indent:-0.8em}ul.icons li .icon{width:0.8em}ul.icons li .icon-large:before,ul.icons li .icon-large:before{vertical-align:baseline}.icon-book:before{content:"\f02d"}.icon-caret-down:before{content:"\f0d7"}.icon-caret-up:before{content:"\f0d8"}.icon-caret-left:before{content:"\f0d9"}.icon-caret-right:before{content:"\f0da"}.rst-versions{position:fixed;bottom:0;left:0;width:300px;color:#fcfcfc;background:#1f1d1d;border-top:solid 10px #343131;font-family:"Lato","proxima-nova","Helvetica Neue",Arial,sans-serif;z-index:400}.rst-versions a{color:#2980b9;text-decoration:none}.rst-versions .rst-badge-small{display:none}.rst-versions .rst-current-version{padding:12px;background-color:#272525;display:block;text-align:right;font-size:90%;cursor:pointer;color:#27ae60;*zoom:1}.rst-versions .rst-current-version:before,.rst-versions .rst-current-version:after{display:table;content:""}.rst-versions .rst-current-version:after{clear:both}.rst-versions .rst-current-version .icon{color:#fcfcfc}.rst-versions .rst-current-version .icon-book{float:left}.rst-versions .rst-current-version.rst-out-of-date{background-color:#e74c3c;color:#fff}.rst-versions.shift-up .rst-other-versions{display:block}.rst-versions .rst-other-versions{font-size:90%;padding:12px;color:gray;display:none}.rst-versions .rst-other-versions hr{display:block;height:1px;border:0;margin:20px 0;padding:0;border-top:solid 1px #413d3d}.rst-versions .rst-other-versions dd{display:inline-block;margin:0}.rst-versions .rst-other-versions dd a{display:inline-block;padding:6px;color:#fcfcfc}.rst-versions.rst-badge{width:auto;bottom:20px;right:20px;left:auto;border:none;max-width:300px}.rst-versions.rst-badge .icon-book{float:none}.rst-versions.rst-badge.shift-up .rst-current-version{text-align:right}.rst-versions.rst-badge.shift-up .rst-current-version .icon-book{float:left}.rst-versions.rst-badge .rst-current-version{width:auto;height:30px;line-height:30px;padding:0 6px;display:block;text-align:center}@media screen and (max-width: 768px){.rst-versions{width:85%;display:none}.rst-versions.shift{display:block}img{width:100%;height:auto}}
+﻿.clearfix{*zoom:1}.clearfix:before,.clearfix:after{display:table;content:""}.clearfix:after{clear:both}@font-face{font-family:FontAwesome;font-style:normal;font-weight:normal;src:url("../fonts/fontawesome-webfont.eot?#iefix") format("embedded-opentype"),url("../fonts/fontawesome-webfont.woff2") format("woff2"),url("../fonts/fontawesome-webfont.woff") format("woff"),url("../fonts/fontawesome-webfont.ttf") format("truetype"),url("../fonts/fontawesome-webfont.svg#FontAwesome") format("svg")}.fa:before{display:inline-block;font-family:FontAwesome;font-style:normal;font-weight:normal;line-height:1;text-decoration:inherit}a .fa{display:inline-block;text-decoration:inherit}li .fa{display:inline-block}li .fa-large:before,li .fa-large:before{width:1.875em}ul.fas{list-style-type:none;margin-left:2em;text-indent:-0.8em}ul.fas li .fa{width:.8em}ul.fas li .fa-large:before,ul.fas li .fa-large:before{vertical-align:baseline}.fa-book:before{content:""}.icon-book:before{content:""}.fa-caret-down:before{content:""}.icon-caret-down:before{content:""}.fa-caret-up:before{content:""}.icon-caret-up:before{content:""}.fa-caret-left:before{content:""}.icon-caret-left:before{content:""}.fa-caret-right:before{content:""}.icon-caret-right:before{content:""}.rst-versions{position:fixed;bottom:0;left:0;width:300px;color:#fcfcfc;background:#1f1d1d;font-family:"Lato","proxima-nova","Helvetica Neue",Arial,sans-serif;z-index:400}.rst-versions a{color:#2980B9;text-decoration:none}.rst-versions .rst-badge-small{display:none}.rst-versions .rst-current-version{padding:12px;background-color:#272525;display:block;text-align:right;font-size:90%;cursor:pointer;color:#27AE60}.rst-versions .rst-current-version::after{clear:both;content:"";display:block}.rst-versions .rst-current-version .fa{color:#fcfcfc}.rst-versions .rst-current-version .fa-book{float:left}.rst-versions .rst-current-version .icon-book{float:left}.rst-versions .rst-current-version.rst-out-of-date{background-color:#E74C3C;color:#fff}.rst-versions .rst-current-version.rst-active-old-version{background-color:#F1C40F;color:#000}.rst-versions.shift-up{height:auto;max-height:100%;overflow-y:scroll}.rst-versions.shift-up .rst-other-versions{display:block}.rst-versions .rst-other-versions{font-size:90%;padding:12px;color:gray;display:none}.rst-versions .rst-other-versions hr{display:block;height:1px;border:0;margin:20px 0;padding:0;border-top:solid 1px #413d3d}.rst-versions .rst-other-versions dd{display:inline-block;margin:0}.rst-versions .rst-other-versions dd a{display:inline-block;padding:6px;color:#fcfcfc}.rst-versions.rst-badge{width:auto;bottom:20px;right:20px;left:auto;border:none;max-width:300px;max-height:90%}.rst-versions.rst-badge .icon-book{float:none;line-height:30px}.rst-versions.rst-badge .fa-book{float:none;line-height:30px}.rst-versions.rst-badge.shift-up .rst-current-version{text-align:right}.rst-versions.rst-badge.shift-up .rst-current-version .fa-book{float:left}.rst-versions.rst-badge.shift-up .rst-current-version .icon-book{float:left}.rst-versions.rst-badge>.rst-current-version{width:auto;height:30px;line-height:30px;padding:0 6px;display:block;text-align:center}@media screen and (max-width: 768px){.rst-versions{width:85%;display:none}.rst-versions.shift{display:block}}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_static/jquery-1.11.1.js` & `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/jquery.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,143 +1,212 @@
 /*!
- * jQuery JavaScript Library v1.11.1
- * http://jquery.com/
+ * jQuery JavaScript Library v3.6.1
+ * https://jquery.com/
  *
  * Includes Sizzle.js
- * http://sizzlejs.com/
+ * https://sizzlejs.com/
  *
- * Copyright 2005, 2014 jQuery Foundation, Inc. and other contributors
+ * Copyright OpenJS Foundation and other contributors
  * Released under the MIT license
- * http://jquery.org/license
- *
- * Date: 2014-05-01T17:42Z
+ * https://jquery.org/license
  */
-
 (function(global, factory) {
 
+    "use strict";
+
     if (typeof module === "object" && typeof module.exports === "object") {
-        // For CommonJS and CommonJS-like environments where a proper window is present,
-        // execute the factory and get jQuery
-        // For environments that do not inherently posses a window with a document
-        // (such as Node.js), expose a jQuery-making factory as module.exports
-        // This accentuates the need for the creation of a real window
+
+        // For CommonJS and CommonJS-like environments where a proper `window`
+        // is present, execute the factory and get jQuery.
+        // For environments that do not have a `window` with a `document`
+        // (such as Node.js), expose a factory as module.exports.
+        // This accentuates the need for the creation of a real `window`.
         // e.g. var jQuery = require("jquery")(window);
-        // See ticket #14549 for more info
+        // See ticket trac-14549 for more info.
         module.exports = global.document ?
             factory(global, true) :
             function(w) {
                 if (!w.document) {
                     throw new Error("jQuery requires a window with a document");
                 }
                 return factory(w);
             };
     } else {
         factory(global);
     }
 
     // Pass this if window is not defined yet
-}(typeof window !== "undefined" ? window : this, function(window, noGlobal) {
+})(typeof window !== "undefined" ? window : this, function(window, noGlobal) {
 
-    // Can't do this because several apps including ASP.NET trace
-    // the stack via arguments.caller.callee and Firefox dies if
-    // you try to trace through "use strict" call chains. (#13335)
-    // Support: Firefox 18+
-    //
+    // Edge <= 12 - 13+, Firefox <=18 - 45+, IE 10 - 11, Safari 5.1 - 9+, iOS 6 - 9.1
+    // throw exceptions when non-strict code (e.g., ASP.NET 4.5) accesses strict mode
+    // arguments.callee.caller (trac-13335). But as of jQuery 3.0 (2016), strict mode should be common
+    // enough that all such attempts are guarded in a try block.
+    "use strict";
+
+    var arr = [];
 
-    var deletedIds = [];
+    var getProto = Object.getPrototypeOf;
 
-    var slice = deletedIds.slice;
+    var slice = arr.slice;
+
+    var flat = arr.flat ? function(array) {
+        return arr.flat.call(array);
+    } : function(array) {
+        return arr.concat.apply([], array);
+    };
 
-    var concat = deletedIds.concat;
 
-    var push = deletedIds.push;
+    var push = arr.push;
 
-    var indexOf = deletedIds.indexOf;
+    var indexOf = arr.indexOf;
 
     var class2type = {};
 
     var toString = class2type.toString;
 
     var hasOwn = class2type.hasOwnProperty;
 
+    var fnToString = hasOwn.toString;
+
+    var ObjectFunctionString = fnToString.call(Object);
+
     var support = {};
 
+    var isFunction = function isFunction(obj) {
+
+        // Support: Chrome <=57, Firefox <=52
+        // In some browsers, typeof returns "function" for HTML <object> elements
+        // (i.e., `typeof document.createElement( "object" ) === "function"`).
+        // We don't want to classify *any* DOM node as a function.
+        // Support: QtWeb <=3.8.5, WebKit <=534.34, wkhtmltopdf tool <=0.12.5
+        // Plus for old WebKit, typeof returns "function" for HTML collections
+        // (e.g., `typeof document.getElementsByTagName("div") === "function"`). (gh-4756)
+        return typeof obj === "function" && typeof obj.nodeType !== "number" &&
+            typeof obj.item !== "function";
+    };
+
+
+    var isWindow = function isWindow(obj) {
+        return obj != null && obj === obj.window;
+    };
+
+
+    var document = window.document;
+
+
+
+    var preservedScriptAttributes = {
+        type: true,
+        src: true,
+        nonce: true,
+        noModule: true
+    };
+
+    function DOMEval(code, node, doc) {
+        doc = doc || document;
+
+        var i, val,
+            script = doc.createElement("script");
+
+        script.text = code;
+        if (node) {
+            for (i in preservedScriptAttributes) {
+
+                // Support: Firefox 64+, Edge 18+
+                // Some browsers don't support the "nonce" property on scripts.
+                // On the other hand, just using `getAttribute` is not enough as
+                // the `nonce` attribute is reset to an empty string whenever it
+                // becomes browsing-context connected.
+                // See https://github.com/whatwg/html/issues/2369
+                // See https://html.spec.whatwg.org/#nonce-attributes
+                // The `node.getAttribute` check was added for the sake of
+                // `jQuery.globalEval` so that it can fake a nonce-containing node
+                // via an object.
+                val = node[i] || node.getAttribute && node.getAttribute(i);
+                if (val) {
+                    script.setAttribute(i, val);
+                }
+            }
+        }
+        doc.head.appendChild(script).parentNode.removeChild(script);
+    }
+
+
+    function toType(obj) {
+        if (obj == null) {
+            return obj + "";
+        }
+
+        // Support: Android <=2.3 only (functionish RegExp)
+        return typeof obj === "object" || typeof obj === "function" ?
+            class2type[toString.call(obj)] || "object" :
+            typeof obj;
+    }
+    /* global Symbol */
+    // Defining this global in .eslintrc.json would create a danger of using the global
+    // unguarded in another place, it seems safer to define global only for this module
+
 
 
     var
-        version = "1.11.1",
+        version = "3.6.1",
 
         // Define a local copy of jQuery
         jQuery = function(selector, context) {
+
             // The jQuery object is actually just the init constructor 'enhanced'
             // Need init if jQuery is called (just allow error to be thrown if not included)
             return new jQuery.fn.init(selector, context);
-        },
-
-        // Support: Android<4.1, IE<9
-        // Make sure we trim BOM and NBSP
-        rtrim = /^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g,
-
-        // Matches dashed string for camelizing
-        rmsPrefix = /^-ms-/,
-        rdashAlpha = /-([\da-z])/gi,
-
-        // Used by jQuery.camelCase as callback to replace()
-        fcamelCase = function(all, letter) {
-            return letter.toUpperCase();
         };
 
     jQuery.fn = jQuery.prototype = {
+
         // The current version of jQuery being used
         jquery: version,
 
         constructor: jQuery,
 
-        // Start with an empty selector
-        selector: "",
-
         // The default length of a jQuery object is 0
         length: 0,
 
         toArray: function() {
             return slice.call(this);
         },
 
         // Get the Nth element in the matched element set OR
         // Get the whole matched element set as a clean array
         get: function(num) {
-            return num != null ?
 
-                // Return just the one element from the set
-                (num < 0 ? this[num + this.length] : this[num]) :
+            // Return all the elements in a clean array
+            if (num == null) {
+                return slice.call(this);
+            }
 
-                // Return all the elements in a clean array
-                slice.call(this);
+            // Return just the one element from the set
+            return num < 0 ? this[num + this.length] : this[num];
         },
 
         // Take an array of elements and push it onto the stack
         // (returning the new matched element set)
         pushStack: function(elems) {
 
             // Build a new jQuery matched element set
             var ret = jQuery.merge(this.constructor(), elems);
 
             // Add the old object onto the stack (as a reference)
             ret.prevObject = this;
-            ret.context = this.context;
 
             // Return the newly-formed element set
             return ret;
         },
 
         // Execute a callback for every element in the matched set.
-        // (You can seed the arguments with an array of args, but this is
-        // only used internally.)
-        each: function(callback, args) {
-            return jQuery.each(this, callback, args);
+        each: function(callback) {
+            return jQuery.each(this, callback);
         },
 
         map: function(callback) {
             return this.pushStack(jQuery.map(this, function(elem, i) {
                 return callback.call(elem, i, elem);
             }));
         },
@@ -150,80 +219,99 @@
             return this.eq(0);
         },
 
         last: function() {
             return this.eq(-1);
         },
 
+        even: function() {
+            return this.pushStack(jQuery.grep(this, function(_elem, i) {
+                return (i + 1) % 2;
+            }));
+        },
+
+        odd: function() {
+            return this.pushStack(jQuery.grep(this, function(_elem, i) {
+                return i % 2;
+            }));
+        },
+
         eq: function(i) {
             var len = this.length,
                 j = +i + (i < 0 ? len : 0);
             return this.pushStack(j >= 0 && j < len ? [this[j]] : []);
         },
 
         end: function() {
-            return this.prevObject || this.constructor(null);
+            return this.prevObject || this.constructor();
         },
 
         // For internal use only.
         // Behaves like an Array's method, not like a jQuery method.
         push: push,
-        sort: deletedIds.sort,
-        splice: deletedIds.splice
+        sort: arr.sort,
+        splice: arr.splice
     };
 
     jQuery.extend = jQuery.fn.extend = function() {
-        var src, copyIsArray, copy, name, options, clone,
+        var options, name, src, copy, copyIsArray, clone,
             target = arguments[0] || {},
             i = 1,
             length = arguments.length,
             deep = false;
 
         // Handle a deep copy situation
         if (typeof target === "boolean") {
             deep = target;
 
-            // skip the boolean and the target
+            // Skip the boolean and the target
             target = arguments[i] || {};
             i++;
         }
 
         // Handle case when target is a string or something (possible in deep copy)
-        if (typeof target !== "object" && !jQuery.isFunction(target)) {
+        if (typeof target !== "object" && !isFunction(target)) {
             target = {};
         }
 
-        // extend jQuery itself if only one argument is passed
+        // Extend jQuery itself if only one argument is passed
         if (i === length) {
             target = this;
             i--;
         }
 
         for (; i < length; i++) {
+
             // Only deal with non-null/undefined values
             if ((options = arguments[i]) != null) {
+
                 // Extend the base object
                 for (name in options) {
-                    src = target[name];
                     copy = options[name];
 
+                    // Prevent Object.prototype pollution
                     // Prevent never-ending loop
-                    if (target === copy) {
+                    if (name === "__proto__" || target === copy) {
                         continue;
                     }
 
                     // Recurse if we're merging plain objects or arrays
-                    if (deep && copy && (jQuery.isPlainObject(copy) || (copyIsArray = jQuery.isArray(copy)))) {
-                        if (copyIsArray) {
-                            copyIsArray = false;
-                            clone = src && jQuery.isArray(src) ? src : [];
-
+                    if (deep && copy && (jQuery.isPlainObject(copy) ||
+                            (copyIsArray = Array.isArray(copy)))) {
+                        src = target[name];
+
+                        // Ensure proper type for the source value
+                        if (copyIsArray && !Array.isArray(src)) {
+                            clone = [];
+                        } else if (!copyIsArray && !jQuery.isPlainObject(src)) {
+                            clone = {};
                         } else {
-                            clone = src && jQuery.isPlainObject(src) ? src : {};
+                            clone = src;
                         }
+                        copyIsArray = false;
 
                         // Never move original objects, clone them
                         target[name] = jQuery.extend(deep, clone, copy);
 
                         // Don't bring in undefined values
                     } else if (copy !== undefined) {
                         target[name] = copy;
@@ -233,238 +321,116 @@
         }
 
         // Return the modified object
         return target;
     };
 
     jQuery.extend({
+
         // Unique for each copy of jQuery on the page
         expando: "jQuery" + (version + Math.random()).replace(/\D/g, ""),
 
         // Assume jQuery is ready without the ready module
         isReady: true,
 
         error: function(msg) {
             throw new Error(msg);
         },
 
         noop: function() {},
 
-        // See test/unit/core.js for details concerning isFunction.
-        // Since version 1.3, DOM methods and functions like alert
-        // aren't supported. They return false on IE (#2968).
-        isFunction: function(obj) {
-            return jQuery.type(obj) === "function";
-        },
-
-        isArray: Array.isArray || function(obj) {
-            return jQuery.type(obj) === "array";
-        },
-
-        isWindow: function(obj) {
-            /* jshint eqeqeq: false */
-            return obj != null && obj == obj.window;
-        },
-
-        isNumeric: function(obj) {
-            // parseFloat NaNs numeric-cast false positives (null|true|false|"")
-            // ...but misinterprets leading-number strings, particularly hex literals ("0x...")
-            // subtraction forces infinities to NaN
-            return !jQuery.isArray(obj) && obj - parseFloat(obj) >= 0;
-        },
-
-        isEmptyObject: function(obj) {
-            var name;
-            for (name in obj) {
-                return false;
-            }
-            return true;
-        },
-
         isPlainObject: function(obj) {
-            var key;
+            var proto, Ctor;
 
-            // Must be an Object.
-            // Because of IE, we also have to check the presence of the constructor property.
-            // Make sure that DOM nodes and window objects don't pass through, as well
-            if (!obj || jQuery.type(obj) !== "object" || obj.nodeType || jQuery.isWindow(obj)) {
+            // Detect obvious negatives
+            // Use toString instead of jQuery.type to catch host objects
+            if (!obj || toString.call(obj) !== "[object Object]") {
                 return false;
             }
 
-            try {
-                // Not own constructor property must be Object
-                if (obj.constructor &&
-                    !hasOwn.call(obj, "constructor") &&
-                    !hasOwn.call(obj.constructor.prototype, "isPrototypeOf")) {
-                    return false;
-                }
-            } catch (e) {
-                // IE8,9 Will throw exceptions on certain host objects #9897
-                return false;
-            }
+            proto = getProto(obj);
 
-            // Support: IE<9
-            // Handle iteration over inherited properties before own properties.
-            if (support.ownLast) {
-                for (key in obj) {
-                    return hasOwn.call(obj, key);
-                }
+            // Objects with no prototype (e.g., `Object.create( null )`) are plain
+            if (!proto) {
+                return true;
             }
 
-            // Own properties are enumerated firstly, so to speed up,
-            // if last one is own, then all properties are own.
-            for (key in obj) {}
-
-            return key === undefined || hasOwn.call(obj, key);
+            // Objects with prototype are plain iff they were constructed by a global Object function
+            Ctor = hasOwn.call(proto, "constructor") && proto.constructor;
+            return typeof Ctor === "function" && fnToString.call(Ctor) === ObjectFunctionString;
         },
 
-        type: function(obj) {
-            if (obj == null) {
-                return obj + "";
-            }
-            return typeof obj === "object" || typeof obj === "function" ?
-                class2type[toString.call(obj)] || "object" :
-                typeof obj;
-        },
+        isEmptyObject: function(obj) {
+            var name;
 
-        // Evaluates a script in a global context
-        // Workarounds based on findings by Jim Driscoll
-        // http://weblogs.java.net/blog/driscoll/archive/2009/09/08/eval-javascript-global-context
-        globalEval: function(data) {
-            if (data && jQuery.trim(data)) {
-                // We use execScript on Internet Explorer
-                // We use an anonymous function so that context is window
-                // rather than jQuery in Firefox
-                (window.execScript || function(data) {
-                    window["eval"].call(window, data);
-                })(data);
+            for (name in obj) {
+                return false;
             }
+            return true;
         },
 
-        // Convert dashed to camelCase; used by the css and data modules
-        // Microsoft forgot to hump their vendor prefix (#9572)
-        camelCase: function(string) {
-            return string.replace(rmsPrefix, "ms-").replace(rdashAlpha, fcamelCase);
-        },
-
-        nodeName: function(elem, name) {
-            return elem.nodeName && elem.nodeName.toLowerCase() === name.toLowerCase();
+        // Evaluates a script in a provided context; falls back to the global one
+        // if not specified.
+        globalEval: function(code, options, doc) {
+            DOMEval(code, {
+                nonce: options && options.nonce
+            }, doc);
         },
 
-        // args is for internal usage only
-        each: function(obj, callback, args) {
-            var value,
-                i = 0,
-                length = obj.length,
-                isArray = isArraylike(obj);
-
-            if (args) {
-                if (isArray) {
-                    for (; i < length; i++) {
-                        value = callback.apply(obj[i], args);
+        each: function(obj, callback) {
+            var length, i = 0;
 
-                        if (value === false) {
-                            break;
-                        }
-                    }
-                } else {
-                    for (i in obj) {
-                        value = callback.apply(obj[i], args);
-
-                        if (value === false) {
-                            break;
-                        }
+            if (isArrayLike(obj)) {
+                length = obj.length;
+                for (; i < length; i++) {
+                    if (callback.call(obj[i], i, obj[i]) === false) {
+                        break;
                     }
                 }
-
-                // A special, fast, case for the most common use of each
             } else {
-                if (isArray) {
-                    for (; i < length; i++) {
-                        value = callback.call(obj[i], i, obj[i]);
-
-                        if (value === false) {
-                            break;
-                        }
-                    }
-                } else {
-                    for (i in obj) {
-                        value = callback.call(obj[i], i, obj[i]);
-
-                        if (value === false) {
-                            break;
-                        }
+                for (i in obj) {
+                    if (callback.call(obj[i], i, obj[i]) === false) {
+                        break;
                     }
                 }
             }
 
             return obj;
         },
 
-        // Support: Android<4.1, IE<9
-        trim: function(text) {
-            return text == null ?
-                "" :
-                (text + "").replace(rtrim, "");
-        },
-
         // results is for internal usage only
         makeArray: function(arr, results) {
             var ret = results || [];
 
             if (arr != null) {
-                if (isArraylike(Object(arr))) {
+                if (isArrayLike(Object(arr))) {
                     jQuery.merge(ret,
                         typeof arr === "string" ? [arr] : arr
                     );
                 } else {
                     push.call(ret, arr);
                 }
             }
 
             return ret;
         },
 
         inArray: function(elem, arr, i) {
-            var len;
-
-            if (arr) {
-                if (indexOf) {
-                    return indexOf.call(arr, elem, i);
-                }
-
-                len = arr.length;
-                i = i ? i < 0 ? Math.max(0, len + i) : i : 0;
-
-                for (; i < len; i++) {
-                    // Skip accessing in sparse arrays
-                    if (i in arr && arr[i] === elem) {
-                        return i;
-                    }
-                }
-            }
-
-            return -1;
+            return arr == null ? -1 : indexOf.call(arr, elem, i);
         },
 
+        // Support: Android <=4.0 only, PhantomJS 1 only
+        // push.apply(_, arraylike) throws on ancient WebKit
         merge: function(first, second) {
             var len = +second.length,
                 j = 0,
                 i = first.length;
 
-            while (j < len) {
-                first[i++] = second[j++];
-            }
-
-            // Support: IE<9
-            // Workaround casting of .length to NaN on otherwise arraylike objects (e.g., NodeLists)
-            if (len !== len) {
-                while (second[j] !== undefined) {
-                    first[i++] = second[j++];
-                }
+            for (; j < len; j++) {
+                first[i++] = second[j];
             }
 
             first.length = i;
 
             return first;
         },
 
@@ -485,22 +451,21 @@
             }
 
             return matches;
         },
 
         // arg is for internal usage only
         map: function(elems, callback, arg) {
-            var value,
+            var length, value,
                 i = 0,
-                length = elems.length,
-                isArray = isArraylike(elems),
                 ret = [];
 
             // Go through the array, translating each of the items to their new values
-            if (isArray) {
+            if (isArrayLike(elems)) {
+                length = elems.length;
                 for (; i < length; i++) {
                     value = callback(elems[i], i, arg);
 
                     if (value != null) {
                         ret.push(value);
                     }
                 }
@@ -513,91 +478,63 @@
                     if (value != null) {
                         ret.push(value);
                     }
                 }
             }
 
             // Flatten any nested arrays
-            return concat.apply([], ret);
+            return flat(ret);
         },
 
         // A global GUID counter for objects
         guid: 1,
 
-        // Bind a function to a context, optionally partially applying any
-        // arguments.
-        proxy: function(fn, context) {
-            var args, proxy, tmp;
-
-            if (typeof context === "string") {
-                tmp = fn[context];
-                context = fn;
-                fn = tmp;
-            }
-
-            // Quick check to determine if target is callable, in the spec
-            // this throws a TypeError, but we will just return undefined.
-            if (!jQuery.isFunction(fn)) {
-                return undefined;
-            }
-
-            // Simulated bind
-            args = slice.call(arguments, 2);
-            proxy = function() {
-                return fn.apply(context || this, args.concat(slice.call(arguments)));
-            };
-
-            // Set the guid of unique handler to the same of original handler, so it can be removed
-            proxy.guid = fn.guid = fn.guid || jQuery.guid++;
-
-            return proxy;
-        },
-
-        now: function() {
-            return +(new Date());
-        },
-
         // jQuery.support is not used in Core but other projects attach their
         // properties to it so it needs to exist.
         support: support
     });
 
+    if (typeof Symbol === "function") {
+        jQuery.fn[Symbol.iterator] = arr[Symbol.iterator];
+    }
+
     // Populate the class2type map
-    jQuery.each("Boolean Number String Function Array Date RegExp Object Error".split(" "), function(i, name) {
-        class2type["[object " + name + "]"] = name.toLowerCase();
-    });
+    jQuery.each("Boolean Number String Function Array Date RegExp Object Error Symbol".split(" "),
+        function(_i, name) {
+            class2type["[object " + name + "]"] = name.toLowerCase();
+        });
 
-    function isArraylike(obj) {
-        var length = obj.length,
-            type = jQuery.type(obj);
+    function isArrayLike(obj) {
 
-        if (type === "function" || jQuery.isWindow(obj)) {
-            return false;
-        }
+        // Support: real iOS 8.2 only (not reproducible in simulator)
+        // `in` check used to prevent JIT error (gh-2145)
+        // hasOwn isn't used here due to false negatives
+        // regarding Nodelist length in IE
+        var length = !!obj && "length" in obj && obj.length,
+            type = toType(obj);
 
-        if (obj.nodeType === 1 && length) {
-            return true;
+        if (isFunction(obj) || isWindow(obj)) {
+            return false;
         }
 
         return type === "array" || length === 0 ||
             typeof length === "number" && length > 0 && (length - 1) in obj;
     }
     var Sizzle =
         /*!
-         * Sizzle CSS Selector Engine v1.10.19
-         * http://sizzlejs.com/
+         * Sizzle CSS Selector Engine v2.3.6
+         * https://sizzlejs.com/
          *
-         * Copyright 2013 jQuery Foundation, Inc. and other contributors
+         * Copyright JS Foundation and other contributors
          * Released under the MIT license
-         * http://jquery.org/license
+         * https://js.foundation/
          *
-         * Date: 2014-04-18
+         * Date: 2021-02-16
          */
         (function(window) {
-
             var i,
                 support,
                 Expr,
                 getText,
                 isXML,
                 tokenize,
                 compile,
@@ -613,287 +550,374 @@
                 documentIsHTML,
                 rbuggyQSA,
                 rbuggyMatches,
                 matches,
                 contains,
 
                 // Instance-specific data
-                expando = "sizzle" + -(new Date()),
+                expando = "sizzle" + 1 * new Date(),
                 preferredDoc = window.document,
                 dirruns = 0,
                 done = 0,
                 classCache = createCache(),
                 tokenCache = createCache(),
                 compilerCache = createCache(),
+                nonnativeSelectorCache = createCache(),
                 sortOrder = function(a, b) {
                     if (a === b) {
                         hasDuplicate = true;
                     }
                     return 0;
                 },
 
-                // General-purpose constants
-                strundefined = typeof undefined,
-                MAX_NEGATIVE = 1 << 31,
-
                 // Instance methods
                 hasOwn = ({}).hasOwnProperty,
                 arr = [],
                 pop = arr.pop,
-                push_native = arr.push,
+                pushNative = arr.push,
                 push = arr.push,
                 slice = arr.slice,
-                // Use a stripped-down indexOf if we can't use a native one
-                indexOf = arr.indexOf || function(elem) {
+
+                // Use a stripped-down indexOf as it's faster than native
+                // https://jsperf.com/thor-indexof-vs-for/5
+                indexOf = function(list, elem) {
                     var i = 0,
-                        len = this.length;
+                        len = list.length;
                     for (; i < len; i++) {
-                        if (this[i] === elem) {
+                        if (list[i] === elem) {
                             return i;
                         }
                     }
                     return -1;
                 },
 
-                booleans = "checked|selected|async|autofocus|autoplay|controls|defer|disabled|hidden|ismap|loop|multiple|open|readonly|required|scoped",
+                booleans = "checked|selected|async|autofocus|autoplay|controls|defer|disabled|hidden|" +
+                "ismap|loop|multiple|open|readonly|required|scoped",
 
                 // Regular expressions
 
-                // Whitespace characters http://www.w3.org/TR/css3-selectors/#whitespace
+                // http://www.w3.org/TR/css3-selectors/#whitespace
                 whitespace = "[\\x20\\t\\r\\n\\f]",
-                // http://www.w3.org/TR/css3-syntax/#characters
-                characterEncoding = "(?:\\\\.|[\\w-]|[^\\x00-\\xa0])+",
 
-                // Loosely modeled on CSS identifier characters
-                // An unquoted value should be a CSS identifier http://www.w3.org/TR/css3-selectors/#attribute-selectors
-                // Proper syntax: http://www.w3.org/TR/CSS21/syndata.html#value-def-identifier
-                identifier = characterEncoding.replace("w", "w#"),
+                // https://www.w3.org/TR/css-syntax-3/#ident-token-diagram
+                identifier = "(?:\\\\[\\da-fA-F]{1,6}" + whitespace +
+                "?|\\\\[^\\r\\n\\f]|[\\w-]|[^\0-\\x7f])+",
 
                 // Attribute selectors: http://www.w3.org/TR/selectors/#attribute-selectors
-                attributes = "\\[" + whitespace + "*(" + characterEncoding + ")(?:" + whitespace +
+                attributes = "\\[" + whitespace + "*(" + identifier + ")(?:" + whitespace +
+
                 // Operator (capture 2)
                 "*([*^$|!~]?=)" + whitespace +
-                // "Attribute values must be CSS identifiers [capture 5] or strings [capture 3 or capture 4]"
-                "*(?:'((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\"|(" + identifier + "))|)" + whitespace +
-                "*\\]",
 
-                pseudos = ":(" + characterEncoding + ")(?:\\((" +
+                // "Attribute values must be CSS identifiers [capture 5]
+                // or strings [capture 3 or capture 4]"
+                "*(?:'((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\"|(" + identifier + "))|)" +
+                whitespace + "*\\]",
+
+                pseudos = ":(" + identifier + ")(?:\\((" +
+
                 // To reduce the number of selectors needing tokenize in the preFilter, prefer arguments:
                 // 1. quoted (capture 3; capture 4 or capture 5)
                 "('((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\")|" +
+
                 // 2. simple (capture 6)
                 "((?:\\\\.|[^\\\\()[\\]]|" + attributes + ")*)|" +
+
                 // 3. anything else (capture 2)
                 ".*" +
                 ")\\)|)",
 
                 // Leading and non-escaped trailing whitespace, capturing some non-whitespace characters preceding the latter
-                rtrim = new RegExp("^" + whitespace + "+|((?:^|[^\\\\])(?:\\\\.)*)" + whitespace + "+$", "g"),
+                rwhitespace = new RegExp(whitespace + "+", "g"),
+                rtrim = new RegExp("^" + whitespace + "+|((?:^|[^\\\\])(?:\\\\.)*)" +
+                    whitespace + "+$", "g"),
 
                 rcomma = new RegExp("^" + whitespace + "*," + whitespace + "*"),
-                rcombinators = new RegExp("^" + whitespace + "*([>+~]|" + whitespace + ")" + whitespace + "*"),
-
-                rattributeQuotes = new RegExp("=" + whitespace + "*([^\\]'\"]*?)" + whitespace + "*\\]", "g"),
+                rcombinators = new RegExp("^" + whitespace + "*([>+~]|" + whitespace + ")" + whitespace +
+                    "*"),
+                rdescend = new RegExp(whitespace + "|>"),
 
                 rpseudo = new RegExp(pseudos),
                 ridentifier = new RegExp("^" + identifier + "$"),
 
                 matchExpr = {
-                    "ID": new RegExp("^#(" + characterEncoding + ")"),
-                    "CLASS": new RegExp("^\\.(" + characterEncoding + ")"),
-                    "TAG": new RegExp("^(" + characterEncoding.replace("w", "w*") + ")"),
+                    "ID": new RegExp("^#(" + identifier + ")"),
+                    "CLASS": new RegExp("^\\.(" + identifier + ")"),
+                    "TAG": new RegExp("^(" + identifier + "|[*])"),
                     "ATTR": new RegExp("^" + attributes),
                     "PSEUDO": new RegExp("^" + pseudos),
-                    "CHILD": new RegExp("^:(only|first|last|nth|nth-last)-(child|of-type)(?:\\(" + whitespace +
-                        "*(even|odd|(([+-]|)(\\d*)n|)" + whitespace + "*(?:([+-]|)" + whitespace +
-                        "*(\\d+)|))" + whitespace + "*\\)|)", "i"),
+                    "CHILD": new RegExp("^:(only|first|last|nth|nth-last)-(child|of-type)(?:\\(" +
+                        whitespace + "*(even|odd|(([+-]|)(\\d*)n|)" + whitespace + "*(?:([+-]|)" +
+                        whitespace + "*(\\d+)|))" + whitespace + "*\\)|)", "i"),
                     "bool": new RegExp("^(?:" + booleans + ")$", "i"),
+
                     // For use in libraries implementing .is()
                     // We use this for POS matching in `select`
-                    "needsContext": new RegExp("^" + whitespace + "*[>+~]|:(even|odd|eq|gt|lt|nth|first|last)(?:\\(" +
-                        whitespace + "*((?:-\\d)?\\d*)" + whitespace + "*\\)|)(?=[^-]|$)", "i")
+                    "needsContext": new RegExp("^" + whitespace +
+                        "*[>+~]|:(even|odd|eq|gt|lt|nth|first|last)(?:\\(" + whitespace +
+                        "*((?:-\\d)?\\d*)" + whitespace + "*\\)|)(?=[^-]|$)", "i")
                 },
 
+                rhtml = /HTML$/i,
                 rinputs = /^(?:input|select|textarea|button)$/i,
                 rheader = /^h\d$/i,
 
                 rnative = /^[^{]+\{\s*\[native \w/,
 
                 // Easily-parseable/retrievable ID or TAG or CLASS selectors
                 rquickExpr = /^(?:#([\w-]+)|(\w+)|\.([\w-]+))$/,
 
                 rsibling = /[+~]/,
-                rescape = /'|\\/g,
 
-                // CSS escapes http://www.w3.org/TR/CSS21/syndata.html#escaped-characters
-                runescape = new RegExp("\\\\([\\da-f]{1,6}" + whitespace + "?|(" + whitespace + ")|.)", "ig"),
-                funescape = function(_, escaped, escapedWhitespace) {
-                    var high = "0x" + escaped - 0x10000;
-                    // NaN means non-codepoint
-                    // Support: Firefox<24
-                    // Workaround erroneous numeric interpretation of +"0x"
-                    return high !== high || escapedWhitespace ?
-                        escaped :
+                // CSS escapes
+                // http://www.w3.org/TR/CSS21/syndata.html#escaped-characters
+                runescape = new RegExp("\\\\[\\da-fA-F]{1,6}" + whitespace + "?|\\\\([^\\r\\n\\f])", "g"),
+                funescape = function(escape, nonHex) {
+                    var high = "0x" + escape.slice(1) - 0x10000;
+
+                    return nonHex ?
+
+                        // Strip the backslash prefix from a non-hex escape sequence
+                        nonHex :
+
+                        // Replace a hexadecimal escape sequence with the encoded Unicode code point
+                        // Support: IE <=11+
+                        // For values outside the Basic Multilingual Plane (BMP), manually construct a
+                        // surrogate pair
                         high < 0 ?
-                        // BMP codepoint
                         String.fromCharCode(high + 0x10000) :
-                        // Supplemental Plane codepoint (surrogate pair)
                         String.fromCharCode(high >> 10 | 0xD800, high & 0x3FF | 0xDC00);
-                };
+                },
+
+                // CSS string/identifier serialization
+                // https://drafts.csswg.org/cssom/#common-serializing-idioms
+                rcssescape = /([\0-\x1f\x7f]|^-?\d)|^-$|[^\0-\x1f\x7f-\uFFFF\w-]/g,
+                fcssescape = function(ch, asCodePoint) {
+                    if (asCodePoint) {
+
+                        // U+0000 NULL becomes U+FFFD REPLACEMENT CHARACTER
+                        if (ch === "\0") {
+                            return "\uFFFD";
+                        }
+
+                        // Control characters and (dependent upon position) numbers get escaped as code points
+                        return ch.slice(0, -1) + "\\" +
+                            ch.charCodeAt(ch.length - 1).toString(16) + " ";
+                    }
+
+                    // Other potentially-special ASCII characters get backslash-escaped
+                    return "\\" + ch;
+                },
+
+                // Used for iframes
+                // See setDocument()
+                // Removing the function wrapper causes a "Permission Denied"
+                // error in IE
+                unloadHandler = function() {
+                    setDocument();
+                },
+
+                inDisabledFieldset = addCombinator(
+                    function(elem) {
+                        return elem.disabled === true && elem.nodeName.toLowerCase() === "fieldset";
+                    }, {
+                        dir: "parentNode",
+                        next: "legend"
+                    }
+                );
 
             // Optimize for push.apply( _, NodeList )
             try {
                 push.apply(
                     (arr = slice.call(preferredDoc.childNodes)),
                     preferredDoc.childNodes
                 );
+
                 // Support: Android<4.0
                 // Detect silently failing push.apply
+                // eslint-disable-next-line no-unused-expressions
                 arr[preferredDoc.childNodes.length].nodeType;
             } catch (e) {
                 push = {
                     apply: arr.length ?
 
                         // Leverage slice if possible
                         function(target, els) {
-                            push_native.apply(target, slice.call(els));
+                            pushNative.apply(target, slice.call(els));
                         } :
 
                         // Support: IE<9
                         // Otherwise append directly
                         function(target, els) {
                             var j = target.length,
                                 i = 0;
+
                             // Can't trust NodeList.length
                             while ((target[j++] = els[i++])) {}
                             target.length = j - 1;
                         }
                 };
             }
 
             function Sizzle(selector, context, results, seed) {
-                var match, elem, m, nodeType,
-                    // QSA vars
-                    i, groups, old, nid, newContext, newSelector;
+                var m, i, elem, nid, match, groups, newSelector,
+                    newContext = context && context.ownerDocument,
 
-                if ((context ? context.ownerDocument || context : preferredDoc) !== document) {
-                    setDocument(context);
-                }
+                    // nodeType defaults to 9, since context defaults to document
+                    nodeType = context ? context.nodeType : 9;
 
-                context = context || document;
                 results = results || [];
 
-                if (!selector || typeof selector !== "string") {
+                // Return early from calls with invalid selector or context
+                if (typeof selector !== "string" || !selector ||
+                    nodeType !== 1 && nodeType !== 9 && nodeType !== 11) {
+
                     return results;
                 }
 
-                if ((nodeType = context.nodeType) !== 1 && nodeType !== 9) {
-                    return [];
-                }
+                // Try to shortcut find operations (as opposed to filters) in HTML documents
+                if (!seed) {
+                    setDocument(context);
+                    context = context || document;
 
-                if (documentIsHTML && !seed) {
+                    if (documentIsHTML) {
 
-                    // Shortcuts
-                    if ((match = rquickExpr.exec(selector))) {
-                        // Speed-up: Sizzle("#ID")
-                        if ((m = match[1])) {
-                            if (nodeType === 9) {
-                                elem = context.getElementById(m);
-                                // Check parentNode to catch when Blackberry 4.6 returns
-                                // nodes that are no longer in the document (jQuery #6963)
-                                if (elem && elem.parentNode) {
-                                    // Handle the case where IE, Opera, and Webkit return items
-                                    // by name instead of ID
-                                    if (elem.id === m) {
-                                        results.push(elem);
+                        // If the selector is sufficiently simple, try using a "get*By*" DOM method
+                        // (excepting DocumentFragment context, where the methods don't exist)
+                        if (nodeType !== 11 && (match = rquickExpr.exec(selector))) {
+
+                            // ID selector
+                            if ((m = match[1])) {
+
+                                // Document context
+                                if (nodeType === 9) {
+                                    if ((elem = context.getElementById(m))) {
+
+                                        // Support: IE, Opera, Webkit
+                                        // TODO: identify versions
+                                        // getElementById can match elements by name instead of ID
+                                        if (elem.id === m) {
+                                            results.push(elem);
+                                            return results;
+                                        }
+                                    } else {
                                         return results;
                                     }
+
+                                    // Element context
                                 } else {
-                                    return results;
-                                }
-                            } else {
-                                // Context is not a document
-                                if (context.ownerDocument && (elem = context.ownerDocument.getElementById(m)) &&
-                                    contains(context, elem) && elem.id === m) {
-                                    results.push(elem);
-                                    return results;
-                                }
-                            }
 
-                            // Speed-up: Sizzle("TAG")
-                        } else if (match[2]) {
-                            push.apply(results, context.getElementsByTagName(selector));
-                            return results;
+                                    // Support: IE, Opera, Webkit
+                                    // TODO: identify versions
+                                    // getElementById can match elements by name instead of ID
+                                    if (newContext && (elem = newContext.getElementById(m)) &&
+                                        contains(context, elem) &&
+                                        elem.id === m) {
 
-                            // Speed-up: Sizzle(".CLASS")
-                        } else if ((m = match[3]) && support.getElementsByClassName && context.getElementsByClassName) {
-                            push.apply(results, context.getElementsByClassName(m));
-                            return results;
-                        }
-                    }
+                                        results.push(elem);
+                                        return results;
+                                    }
+                                }
 
-                    // QSA path
-                    if (support.qsa && (!rbuggyQSA || !rbuggyQSA.test(selector))) {
-                        nid = old = expando;
-                        newContext = context;
-                        newSelector = nodeType === 9 && selector;
-
-                        // qSA works strangely on Element-rooted queries
-                        // We can work around this by specifying an extra ID on the root
-                        // and working up from there (Thanks to Andrew Dupont for the technique)
-                        // IE 8 doesn't work on object elements
-                        if (nodeType === 1 && context.nodeName.toLowerCase() !== "object") {
-                            groups = tokenize(selector);
+                                // Type selector
+                            } else if (match[2]) {
+                                push.apply(results, context.getElementsByTagName(selector));
+                                return results;
 
-                            if ((old = context.getAttribute("id"))) {
-                                nid = old.replace(rescape, "\\$&");
-                            } else {
-                                context.setAttribute("id", nid);
-                            }
-                            nid = "[id='" + nid + "'] ";
+                                // Class selector
+                            } else if ((m = match[3]) && support.getElementsByClassName &&
+                                context.getElementsByClassName) {
 
-                            i = groups.length;
-                            while (i--) {
-                                groups[i] = nid + toSelector(groups[i]);
+                                push.apply(results, context.getElementsByClassName(m));
+                                return results;
                             }
-                            newContext = rsibling.test(selector) && testContext(context.parentNode) || context;
-                            newSelector = groups.join(",");
                         }
 
-                        if (newSelector) {
+                        // Take advantage of querySelectorAll
+                        if (support.qsa &&
+                            !nonnativeSelectorCache[selector + " "] &&
+                            (!rbuggyQSA || !rbuggyQSA.test(selector)) &&
+
+                            // Support: IE 8 only
+                            // Exclude object elements
+                            (nodeType !== 1 || context.nodeName.toLowerCase() !== "object")) {
+
+                            newSelector = selector;
+                            newContext = context;
+
+                            // qSA considers elements outside a scoping root when evaluating child or
+                            // descendant combinators, which is not what we want.
+                            // In such cases, we work around the behavior by prefixing every selector in the
+                            // list with an ID selector referencing the scope context.
+                            // The technique has to be used as well when a leading combinator is used
+                            // as such selectors are not recognized by querySelectorAll.
+                            // Thanks to Andrew Dupont for this technique.
+                            if (nodeType === 1 &&
+                                (rdescend.test(selector) || rcombinators.test(selector))) {
+
+                                // Expand context for sibling selectors
+                                newContext = rsibling.test(selector) && testContext(context.parentNode) ||
+                                    context;
+
+                                // We can use :scope instead of the ID hack if the browser
+                                // supports it & if we're not changing the context.
+                                if (newContext !== context || !support.scope) {
+
+                                    // Capture the context ID, setting it first if necessary
+                                    if ((nid = context.getAttribute("id"))) {
+                                        nid = nid.replace(rcssescape, fcssescape);
+                                    } else {
+                                        context.setAttribute("id", (nid = expando));
+                                    }
+                                }
+
+                                // Prefix every selector in the list
+                                groups = tokenize(selector);
+                                i = groups.length;
+                                while (i--) {
+                                    groups[i] = (nid ? "#" + nid : ":scope") + " " +
+                                        toSelector(groups[i]);
+                                }
+                                newSelector = groups.join(",");
+                            }
+
                             try {
                                 push.apply(results,
                                     newContext.querySelectorAll(newSelector)
                                 );
                                 return results;
-                            } catch (qsaError) {} finally {
-                                if (!old) {
+                            } catch (qsaError) {
+                                nonnativeSelectorCache(selector, true);
+                            } finally {
+                                if (nid === expando) {
                                     context.removeAttribute("id");
                                 }
                             }
                         }
                     }
                 }
 
                 // All others
                 return select(selector.replace(rtrim, "$1"), context, results, seed);
             }
 
             /**
              * Create key-value caches of limited size
-             * @returns {Function(string, Object)} Returns the Object data after storing it on itself with
+             * @returns {function(string, object)} Returns the Object data after storing it on itself with
              *	property name the (space-suffixed) string and (if the cache is larger than Expr.cacheLength)
              *	deleting the oldest entry
              */
             function createCache() {
                 var keys = [];
 
                 function cache(key, value) {
+
                     // Use (key + " ") to avoid collision with native prototype properties (see Issue #157)
                     if (keys.push(key + " ") > Expr.cacheLength) {
+
                         // Only keep the most recent entries
                         delete cache[keys.shift()];
                     }
                     return (cache[key + " "] = value);
                 }
                 return cache;
             }
@@ -905,41 +929,43 @@
             function markFunction(fn) {
                 fn[expando] = true;
                 return fn;
             }
 
             /**
              * Support testing using an element
-             * @param {Function} fn Passed the created div and expects a boolean result
+             * @param {Function} fn Passed the created element and returns a boolean result
              */
             function assert(fn) {
-                var div = document.createElement("div");
+                var el = document.createElement("fieldset");
 
                 try {
-                    return !!fn(div);
+                    return !!fn(el);
                 } catch (e) {
                     return false;
                 } finally {
+
                     // Remove from its parent by default
-                    if (div.parentNode) {
-                        div.parentNode.removeChild(div);
+                    if (el.parentNode) {
+                        el.parentNode.removeChild(el);
                     }
+
                     // release memory in IE
-                    div = null;
+                    el = null;
                 }
             }
 
             /**
              * Adds the same handler for all of the specified attrs
              * @param {String} attrs Pipe-separated list of attributes
              * @param {Function} handler The method that will be applied
              */
             function addHandle(attrs, handler) {
                 var arr = attrs.split("|"),
-                    i = attrs.length;
+                    i = arr.length;
 
                 while (i--) {
                     Expr.attrHandle[arr[i]] = handler;
                 }
             }
 
             /**
@@ -947,16 +973,15 @@
              * @param {Element} a
              * @param {Element} b
              * @returns {Number} Returns less than 0 if a precedes b, greater than 0 if a follows b
              */
             function siblingCheck(a, b) {
                 var cur = b && a,
                     diff = cur && a.nodeType === 1 && b.nodeType === 1 &&
-                    (~b.sourceIndex || MAX_NEGATIVE) -
-                    (~a.sourceIndex || MAX_NEGATIVE);
+                    a.sourceIndex - b.sourceIndex;
 
                 // Use IE sourceIndex if available on both nodes
                 if (diff) {
                     return diff;
                 }
 
                 // Check if b follows a
@@ -990,14 +1015,70 @@
                 return function(elem) {
                     var name = elem.nodeName.toLowerCase();
                     return (name === "input" || name === "button") && elem.type === type;
                 };
             }
 
             /**
+             * Returns a function to use in pseudos for :enabled/:disabled
+             * @param {Boolean} disabled true for :disabled; false for :enabled
+             */
+            function createDisabledPseudo(disabled) {
+
+                // Known :disabled false positives: fieldset[disabled] > legend:nth-of-type(n+2) :can-disable
+                return function(elem) {
+
+                    // Only certain elements can match :enabled or :disabled
+                    // https://html.spec.whatwg.org/multipage/scripting.html#selector-enabled
+                    // https://html.spec.whatwg.org/multipage/scripting.html#selector-disabled
+                    if ("form" in elem) {
+
+                        // Check for inherited disabledness on relevant non-disabled elements:
+                        // * listed form-associated elements in a disabled fieldset
+                        //   https://html.spec.whatwg.org/multipage/forms.html#category-listed
+                        //   https://html.spec.whatwg.org/multipage/forms.html#concept-fe-disabled
+                        // * option elements in a disabled optgroup
+                        //   https://html.spec.whatwg.org/multipage/forms.html#concept-option-disabled
+                        // All such elements have a "form" property.
+                        if (elem.parentNode && elem.disabled === false) {
+
+                            // Option elements defer to a parent optgroup if present
+                            if ("label" in elem) {
+                                if ("label" in elem.parentNode) {
+                                    return elem.parentNode.disabled === disabled;
+                                } else {
+                                    return elem.disabled === disabled;
+                                }
+                            }
+
+                            // Support: IE 6 - 11
+                            // Use the isDisabled shortcut property to check for disabled fieldset ancestors
+                            return elem.isDisabled === disabled ||
+
+                                // Where there is no isDisabled, check manually
+                                /* jshint -W018 */
+                                elem.isDisabled !== !disabled &&
+                                inDisabledFieldset(elem) === disabled;
+                        }
+
+                        return elem.disabled === disabled;
+
+                        // Try to winnow out elements that can't be disabled before trusting the disabled property.
+                        // Some victims get caught in our net (label, legend, menu, track), but it shouldn't
+                        // even exist on them, let alone have a boolean value.
+                    } else if ("label" in elem) {
+                        return elem.disabled === disabled;
+                    }
+
+                    // Remaining elements are neither :enabled nor :disabled
+                    return false;
+                };
+            }
+
+            /**
              * Returns a function to use in pseudos for positionals
              * @param {Function} fn
              */
             function createPositionalPseudo(fn) {
                 return markFunction(function(argument) {
                     argument = +argument;
                     return markFunction(function(seed, matches) {
@@ -1017,152 +1098,193 @@
 
             /**
              * Checks a node for validity as a Sizzle context
              * @param {Element|Object=} context
              * @returns {Element|Object|Boolean} The input node if acceptable, otherwise a falsy value
              */
             function testContext(context) {
-                return context && typeof context.getElementsByTagName !== strundefined && context;
+                return context && typeof context.getElementsByTagName !== "undefined" && context;
             }
 
             // Expose support vars for convenience
             support = Sizzle.support = {};
 
             /**
              * Detects XML nodes
              * @param {Element|Object} elem An element or a document
              * @returns {Boolean} True iff elem is a non-HTML XML node
              */
             isXML = Sizzle.isXML = function(elem) {
-                // documentElement is verified for cases where it doesn't yet exist
-                // (such as loading iframes in IE - #4833)
-                var documentElement = elem && (elem.ownerDocument || elem).documentElement;
-                return documentElement ? documentElement.nodeName !== "HTML" : false;
+                var namespace = elem && elem.namespaceURI,
+                    docElem = elem && (elem.ownerDocument || elem).documentElement;
+
+                // Support: IE <=8
+                // Assume HTML when documentElement doesn't yet exist, such as inside loading iframes
+                // https://bugs.jquery.com/ticket/4833
+                return !rhtml.test(namespace || docElem && docElem.nodeName || "HTML");
             };
 
             /**
              * Sets document-related variables once based on the current document
              * @param {Element|Object} [doc] An element or document object to use to set the document
              * @returns {Object} Returns the current document
              */
             setDocument = Sizzle.setDocument = function(node) {
-                var hasCompare,
-                    doc = node ? node.ownerDocument || node : preferredDoc,
-                    parent = doc.defaultView;
+                var hasCompare, subWindow,
+                    doc = node ? node.ownerDocument || node : preferredDoc;
 
-                // If no document and documentElement is available, return
-                if (doc === document || doc.nodeType !== 9 || !doc.documentElement) {
+                // Return early if doc is invalid or already selected
+                // Support: IE 11+, Edge 17 - 18+
+                // IE/Edge sometimes throw a "Permission denied" error when strict-comparing
+                // two documents; shallow comparisons work.
+                // eslint-disable-next-line eqeqeq
+                if (doc == document || doc.nodeType !== 9 || !doc.documentElement) {
                     return document;
                 }
 
-                // Set our document
+                // Update global variables
                 document = doc;
-                docElem = doc.documentElement;
-
-                // Support tests
-                documentIsHTML = !isXML(doc);
+                docElem = document.documentElement;
+                documentIsHTML = !isXML(document);
 
-                // Support: IE>8
-                // If iframe document is assigned to "document" variable and if iframe has been reloaded,
-                // IE will throw "permission denied" error when accessing "document" variable, see jQuery #13936
-                // IE6-8 do not support the defaultView property so parent will be undefined
-                if (parent && parent !== parent.top) {
-                    // IE11 does not have attachEvent, so all must suffer
-                    if (parent.addEventListener) {
-                        parent.addEventListener("unload", function() {
-                            setDocument();
-                        }, false);
-                    } else if (parent.attachEvent) {
-                        parent.attachEvent("onunload", function() {
-                            setDocument();
-                        });
+                // Support: IE 9 - 11+, Edge 12 - 18+
+                // Accessing iframe documents after unload throws "permission denied" errors (jQuery #13936)
+                // Support: IE 11+, Edge 17 - 18+
+                // IE/Edge sometimes throw a "Permission denied" error when strict-comparing
+                // two documents; shallow comparisons work.
+                // eslint-disable-next-line eqeqeq
+                if (preferredDoc != document &&
+                    (subWindow = document.defaultView) && subWindow.top !== subWindow) {
+
+                    // Support: IE 11, Edge
+                    if (subWindow.addEventListener) {
+                        subWindow.addEventListener("unload", unloadHandler, false);
+
+                        // Support: IE 9 - 10 only
+                    } else if (subWindow.attachEvent) {
+                        subWindow.attachEvent("onunload", unloadHandler);
                     }
                 }
 
+                // Support: IE 8 - 11+, Edge 12 - 18+, Chrome <=16 - 25 only, Firefox <=3.6 - 31 only,
+                // Safari 4 - 5 only, Opera <=11.6 - 12.x only
+                // IE/Edge & older browsers don't support the :scope pseudo-class.
+                // Support: Safari 6.0 only
+                // Safari 6.0 supports :scope but it's an alias of :root there.
+                support.scope = assert(function(el) {
+                    docElem.appendChild(el).appendChild(document.createElement("div"));
+                    return typeof el.querySelectorAll !== "undefined" &&
+                        !el.querySelectorAll(":scope fieldset div").length;
+                });
+
                 /* Attributes
                 ---------------------------------------------------------------------- */
 
                 // Support: IE<8
-                // Verify that getAttribute really returns attributes and not properties (excepting IE8 booleans)
-                support.attributes = assert(function(div) {
-                    div.className = "i";
-                    return !div.getAttribute("className");
+                // Verify that getAttribute really returns attributes and not properties
+                // (excepting IE8 booleans)
+                support.attributes = assert(function(el) {
+                    el.className = "i";
+                    return !el.getAttribute("className");
                 });
 
                 /* getElement(s)By*
                 ---------------------------------------------------------------------- */
 
                 // Check if getElementsByTagName("*") returns only elements
-                support.getElementsByTagName = assert(function(div) {
-                    div.appendChild(doc.createComment(""));
-                    return !div.getElementsByTagName("*").length;
+                support.getElementsByTagName = assert(function(el) {
+                    el.appendChild(document.createComment(""));
+                    return !el.getElementsByTagName("*").length;
                 });
 
-                // Check if getElementsByClassName can be trusted
-                support.getElementsByClassName = rnative.test(doc.getElementsByClassName) && assert(function(div) {
-                    div.innerHTML = "<div class='a'></div><div class='a i'></div>";
-
-                    // Support: Safari<4
-                    // Catch class over-caching
-                    div.firstChild.className = "i";
-                    // Support: Opera<10
-                    // Catch gEBCN failure to find non-leading classes
-                    return div.getElementsByClassName("i").length === 2;
-                });
+                // Support: IE<9
+                support.getElementsByClassName = rnative.test(document.getElementsByClassName);
 
                 // Support: IE<10
                 // Check if getElementById returns elements by name
-                // The broken getElementById methods don't pick up programatically-set names,
+                // The broken getElementById methods don't pick up programmatically-set names,
                 // so use a roundabout getElementsByName test
-                support.getById = assert(function(div) {
-                    docElem.appendChild(div).id = expando;
-                    return !doc.getElementsByName || !doc.getElementsByName(expando).length;
+                support.getById = assert(function(el) {
+                    docElem.appendChild(el).id = expando;
+                    return !document.getElementsByName || !document.getElementsByName(expando).length;
                 });
 
-                // ID find and filter
+                // ID filter and find
                 if (support.getById) {
-                    Expr.find["ID"] = function(id, context) {
-                        if (typeof context.getElementById !== strundefined && documentIsHTML) {
-                            var m = context.getElementById(id);
-                            // Check parentNode to catch when Blackberry 4.6 returns
-                            // nodes that are no longer in the document #6963
-                            return m && m.parentNode ? [m] : [];
-                        }
-                    };
                     Expr.filter["ID"] = function(id) {
                         var attrId = id.replace(runescape, funescape);
                         return function(elem) {
                             return elem.getAttribute("id") === attrId;
                         };
                     };
+                    Expr.find["ID"] = function(id, context) {
+                        if (typeof context.getElementById !== "undefined" && documentIsHTML) {
+                            var elem = context.getElementById(id);
+                            return elem ? [elem] : [];
+                        }
+                    };
                 } else {
-                    // Support: IE6/7
-                    // getElementById is not reliable as a find shortcut
-                    delete Expr.find["ID"];
-
                     Expr.filter["ID"] = function(id) {
                         var attrId = id.replace(runescape, funescape);
                         return function(elem) {
-                            var node = typeof elem.getAttributeNode !== strundefined && elem.getAttributeNode("id");
+                            var node = typeof elem.getAttributeNode !== "undefined" &&
+                                elem.getAttributeNode("id");
                             return node && node.value === attrId;
                         };
                     };
+
+                    // Support: IE 6 - 7 only
+                    // getElementById is not reliable as a find shortcut
+                    Expr.find["ID"] = function(id, context) {
+                        if (typeof context.getElementById !== "undefined" && documentIsHTML) {
+                            var node, i, elems,
+                                elem = context.getElementById(id);
+
+                            if (elem) {
+
+                                // Verify the id attribute
+                                node = elem.getAttributeNode("id");
+                                if (node && node.value === id) {
+                                    return [elem];
+                                }
+
+                                // Fall back on getElementsByName
+                                elems = context.getElementsByName(id);
+                                i = 0;
+                                while ((elem = elems[i++])) {
+                                    node = elem.getAttributeNode("id");
+                                    if (node && node.value === id) {
+                                        return [elem];
+                                    }
+                                }
+                            }
+
+                            return [];
+                        }
+                    };
                 }
 
                 // Tag
                 Expr.find["TAG"] = support.getElementsByTagName ?
                     function(tag, context) {
-                        if (typeof context.getElementsByTagName !== strundefined) {
+                        if (typeof context.getElementsByTagName !== "undefined") {
                             return context.getElementsByTagName(tag);
+
+                            // DocumentFragment nodes don't have gEBTN
+                        } else if (support.qsa) {
+                            return context.querySelectorAll(tag);
                         }
                     } :
+
                     function(tag, context) {
                         var elem,
                             tmp = [],
                             i = 0,
+
+                            // By happy coincidence, a (broken) gEBTN appears on DocumentFragment nodes too
                             results = context.getElementsByTagName(tag);
 
                         // Filter out possible comments
                         if (tag === "*") {
                             while ((elem = results[i++])) {
                                 if (elem.nodeType === 1) {
                                     tmp.push(elem);
@@ -1172,15 +1294,15 @@
                             return tmp;
                         }
                         return results;
                     };
 
                 // Class
                 Expr.find["CLASS"] = support.getElementsByClassName && function(className, context) {
-                    if (typeof context.getElementsByClassName !== strundefined && documentIsHTML) {
+                    if (typeof context.getElementsByClassName !== "undefined" && documentIsHTML) {
                         return context.getElementsByClassName(className);
                     }
                 };
 
                 /* QSA/matchesSelector
                 ---------------------------------------------------------------------- */
 
@@ -1189,102 +1311,150 @@
                 // matchesSelector(:active) reports false when true (IE9/Opera 11.5)
                 rbuggyMatches = [];
 
                 // qSa(:focus) reports false when true (Chrome 21)
                 // We allow this because of a bug in IE8/9 that throws an error
                 // whenever `document.activeElement` is accessed on an iframe
                 // So, we allow :focus to pass through QSA all the time to avoid the IE error
-                // See http://bugs.jquery.com/ticket/13378
+                // See https://bugs.jquery.com/ticket/13378
                 rbuggyQSA = [];
 
-                if ((support.qsa = rnative.test(doc.querySelectorAll))) {
+                if ((support.qsa = rnative.test(document.querySelectorAll))) {
+
                     // Build QSA regex
                     // Regex strategy adopted from Diego Perini
-                    assert(function(div) {
+                    assert(function(el) {
+
+                        var input;
+
                         // Select is set to empty string on purpose
                         // This is to test IE's treatment of not explicitly
                         // setting a boolean content attribute,
                         // since its presence should be enough
-                        // http://bugs.jquery.com/ticket/12359
-                        div.innerHTML = "<select msallowclip=''><option selected=''></option></select>";
+                        // https://bugs.jquery.com/ticket/12359
+                        docElem.appendChild(el).innerHTML = "<a id='" + expando + "'></a>" +
+                            "<select id='" + expando + "-\r\\' msallowcapture=''>" +
+                            "<option selected=''></option></select>";
 
                         // Support: IE8, Opera 11-12.16
                         // Nothing should be selected when empty strings follow ^= or $= or *=
                         // The test attribute must be unknown in Opera but "safe" for WinRT
-                        // http://msdn.microsoft.com/en-us/library/ie/hh465388.aspx#attribute_section
-                        if (div.querySelectorAll("[msallowclip^='']").length) {
+                        // https://msdn.microsoft.com/en-us/library/ie/hh465388.aspx#attribute_section
+                        if (el.querySelectorAll("[msallowcapture^='']").length) {
                             rbuggyQSA.push("[*^$]=" + whitespace + "*(?:''|\"\")");
                         }
 
                         // Support: IE8
                         // Boolean attributes and "value" are not treated correctly
-                        if (!div.querySelectorAll("[selected]").length) {
+                        if (!el.querySelectorAll("[selected]").length) {
                             rbuggyQSA.push("\\[" + whitespace + "*(?:value|" + booleans + ")");
                         }
 
+                        // Support: Chrome<29, Android<4.4, Safari<7.0+, iOS<7.0+, PhantomJS<1.9.8+
+                        if (!el.querySelectorAll("[id~=" + expando + "-]").length) {
+                            rbuggyQSA.push("~=");
+                        }
+
+                        // Support: IE 11+, Edge 15 - 18+
+                        // IE 11/Edge don't find elements on a `[name='']` query in some cases.
+                        // Adding a temporary attribute to the document before the selection works
+                        // around the issue.
+                        // Interestingly, IE 10 & older don't seem to have the issue.
+                        input = document.createElement("input");
+                        input.setAttribute("name", "");
+                        el.appendChild(input);
+                        if (!el.querySelectorAll("[name='']").length) {
+                            rbuggyQSA.push("\\[" + whitespace + "*name" + whitespace + "*=" +
+                                whitespace + "*(?:''|\"\")");
+                        }
+
                         // Webkit/Opera - :checked should return selected option elements
                         // http://www.w3.org/TR/2011/REC-css3-selectors-20110929/#checked
                         // IE8 throws error here and will not see later tests
-                        if (!div.querySelectorAll(":checked").length) {
+                        if (!el.querySelectorAll(":checked").length) {
                             rbuggyQSA.push(":checked");
                         }
+
+                        // Support: Safari 8+, iOS 8+
+                        // https://bugs.webkit.org/show_bug.cgi?id=136851
+                        // In-page `selector#id sibling-combinator selector` fails
+                        if (!el.querySelectorAll("a#" + expando + "+*").length) {
+                            rbuggyQSA.push(".#.+[+~]");
+                        }
+
+                        // Support: Firefox <=3.6 - 5 only
+                        // Old Firefox doesn't throw on a badly-escaped identifier.
+                        el.querySelectorAll("\\\f");
+                        rbuggyQSA.push("[\\r\\n\\f]");
                     });
 
-                    assert(function(div) {
+                    assert(function(el) {
+                        el.innerHTML = "<a href='' disabled='disabled'></a>" +
+                            "<select disabled='disabled'><option/></select>";
+
                         // Support: Windows 8 Native Apps
                         // The type and name attributes are restricted during .innerHTML assignment
-                        var input = doc.createElement("input");
+                        var input = document.createElement("input");
                         input.setAttribute("type", "hidden");
-                        div.appendChild(input).setAttribute("name", "D");
+                        el.appendChild(input).setAttribute("name", "D");
 
                         // Support: IE8
                         // Enforce case-sensitivity of name attribute
-                        if (div.querySelectorAll("[name=d]").length) {
+                        if (el.querySelectorAll("[name=d]").length) {
                             rbuggyQSA.push("name" + whitespace + "*[*^$|!~]?=");
                         }
 
                         // FF 3.5 - :enabled/:disabled and hidden elements (hidden elements are still enabled)
                         // IE8 throws error here and will not see later tests
-                        if (!div.querySelectorAll(":enabled").length) {
+                        if (el.querySelectorAll(":enabled").length !== 2) {
+                            rbuggyQSA.push(":enabled", ":disabled");
+                        }
+
+                        // Support: IE9-11+
+                        // IE's :disabled selector does not pick up the children of disabled fieldsets
+                        docElem.appendChild(el).disabled = true;
+                        if (el.querySelectorAll(":disabled").length !== 2) {
                             rbuggyQSA.push(":enabled", ":disabled");
                         }
 
+                        // Support: Opera 10 - 11 only
                         // Opera 10-11 does not throw on post-comma invalid pseudos
-                        div.querySelectorAll("*,:x");
+                        el.querySelectorAll("*,:x");
                         rbuggyQSA.push(",.*:");
                     });
                 }
 
                 if ((support.matchesSelector = rnative.test((matches = docElem.matches ||
                         docElem.webkitMatchesSelector ||
                         docElem.mozMatchesSelector ||
                         docElem.oMatchesSelector ||
                         docElem.msMatchesSelector)))) {
 
-                    assert(function(div) {
+                    assert(function(el) {
+
                         // Check to see if it's possible to do matchesSelector
                         // on a disconnected node (IE 9)
-                        support.disconnectedMatch = matches.call(div, "div");
+                        support.disconnectedMatch = matches.call(el, "*");
 
                         // This should fail with an exception
                         // Gecko does not error, returns false instead
-                        matches.call(div, "[s!='']:x");
+                        matches.call(el, "[s!='']:x");
                         rbuggyMatches.push("!=", pseudos);
                     });
                 }
 
                 rbuggyQSA = rbuggyQSA.length && new RegExp(rbuggyQSA.join("|"));
                 rbuggyMatches = rbuggyMatches.length && new RegExp(rbuggyMatches.join("|"));
 
                 /* Contains
                 ---------------------------------------------------------------------- */
                 hasCompare = rnative.test(docElem.compareDocumentPosition);
 
                 // Element contains another
-                // Purposefully does not implement inclusive descendent
+                // Purposefully self-exclusive
                 // As in, an element does not contain itself
                 contains = hasCompare || rnative.test(docElem.contains) ?
                     function(a, b) {
                         var adown = a.nodeType === 9 ? a.documentElement : a,
                             bup = b && b.parentNode;
                         return a === bup || !!(bup && bup.nodeType === 1 && (
                             adown.contains ?
@@ -1319,41 +1489,57 @@
                         // Sort on method existence if only one input has compareDocumentPosition
                         var compare = !a.compareDocumentPosition - !b.compareDocumentPosition;
                         if (compare) {
                             return compare;
                         }
 
                         // Calculate position if both inputs belong to the same document
-                        compare = (a.ownerDocument || a) === (b.ownerDocument || b) ?
+                        // Support: IE 11+, Edge 17 - 18+
+                        // IE/Edge sometimes throw a "Permission denied" error when strict-comparing
+                        // two documents; shallow comparisons work.
+                        // eslint-disable-next-line eqeqeq
+                        compare = (a.ownerDocument || a) == (b.ownerDocument || b) ?
                             a.compareDocumentPosition(b) :
 
                             // Otherwise we know they are disconnected
                             1;
 
                         // Disconnected nodes
                         if (compare & 1 ||
                             (!support.sortDetached && b.compareDocumentPosition(a) === compare)) {
 
                             // Choose the first element that is related to our preferred document
-                            if (a === doc || a.ownerDocument === preferredDoc && contains(preferredDoc, a)) {
+                            // Support: IE 11+, Edge 17 - 18+
+                            // IE/Edge sometimes throw a "Permission denied" error when strict-comparing
+                            // two documents; shallow comparisons work.
+                            // eslint-disable-next-line eqeqeq
+                            if (a == document || a.ownerDocument == preferredDoc &&
+                                contains(preferredDoc, a)) {
                                 return -1;
                             }
-                            if (b === doc || b.ownerDocument === preferredDoc && contains(preferredDoc, b)) {
+
+                            // Support: IE 11+, Edge 17 - 18+
+                            // IE/Edge sometimes throw a "Permission denied" error when strict-comparing
+                            // two documents; shallow comparisons work.
+                            // eslint-disable-next-line eqeqeq
+                            if (b == document || b.ownerDocument == preferredDoc &&
+                                contains(preferredDoc, b)) {
                                 return 1;
                             }
 
                             // Maintain original order
                             return sortInput ?
-                                (indexOf.call(sortInput, a) - indexOf.call(sortInput, b)) :
+                                (indexOf(sortInput, a) - indexOf(sortInput, b)) :
                                 0;
                         }
 
                         return compare & 4 ? -1 : 1;
                     } :
                     function(a, b) {
+
                         // Exit early if the nodes are identical
                         if (a === b) {
                             hasDuplicate = true;
                             return 0;
                         }
 
                         var cur,
@@ -1361,20 +1547,26 @@
                             aup = a.parentNode,
                             bup = b.parentNode,
                             ap = [a],
                             bp = [b];
 
                         // Parentless nodes are either documents or disconnected
                         if (!aup || !bup) {
-                            return a === doc ? -1 :
-                                b === doc ? 1 :
+
+                            // Support: IE 11+, Edge 17 - 18+
+                            // IE/Edge sometimes throw a "Permission denied" error when strict-comparing
+                            // two documents; shallow comparisons work.
+                            /* eslint-disable eqeqeq */
+                            return a == document ? -1 :
+                                b == document ? 1 :
+                                /* eslint-enable eqeqeq */
                                 aup ? -1 :
                                 bup ? 1 :
                                 sortInput ?
-                                (indexOf.call(sortInput, a) - indexOf.call(sortInput, b)) :
+                                (indexOf(sortInput, a) - indexOf(sortInput, b)) :
                                 0;
 
                             // If the nodes are siblings, we can do a quick check
                         } else if (aup === bup) {
                             return siblingCheck(a, b);
                         }
 
@@ -1390,88 +1582,107 @@
 
                         // Walk down the tree looking for a discrepancy
                         while (ap[i] === bp[i]) {
                             i++;
                         }
 
                         return i ?
+
                             // Do a sibling check if the nodes have a common ancestor
                             siblingCheck(ap[i], bp[i]) :
 
                             // Otherwise nodes in our document sort first
-                            ap[i] === preferredDoc ? -1 :
-                            bp[i] === preferredDoc ? 1 :
+                            // Support: IE 11+, Edge 17 - 18+
+                            // IE/Edge sometimes throw a "Permission denied" error when strict-comparing
+                            // two documents; shallow comparisons work.
+                            /* eslint-disable eqeqeq */
+                            ap[i] == preferredDoc ? -1 :
+                            bp[i] == preferredDoc ? 1 :
+                            /* eslint-enable eqeqeq */
                             0;
                     };
 
-                return doc;
+                return document;
             };
 
             Sizzle.matches = function(expr, elements) {
                 return Sizzle(expr, null, null, elements);
             };
 
             Sizzle.matchesSelector = function(elem, expr) {
-                // Set document vars if needed
-                if ((elem.ownerDocument || elem) !== document) {
-                    setDocument(elem);
-                }
-
-                // Make sure that attribute selectors are quoted
-                expr = expr.replace(rattributeQuotes, "='$1']");
+                setDocument(elem);
 
                 if (support.matchesSelector && documentIsHTML &&
+                    !nonnativeSelectorCache[expr + " "] &&
                     (!rbuggyMatches || !rbuggyMatches.test(expr)) &&
                     (!rbuggyQSA || !rbuggyQSA.test(expr))) {
 
                     try {
                         var ret = matches.call(elem, expr);
 
                         // IE 9's matchesSelector returns false on disconnected nodes
                         if (ret || support.disconnectedMatch ||
+
                             // As well, disconnected nodes are said to be in a document
                             // fragment in IE 9
                             elem.document && elem.document.nodeType !== 11) {
                             return ret;
                         }
-                    } catch (e) {}
+                    } catch (e) {
+                        nonnativeSelectorCache(expr, true);
+                    }
                 }
 
                 return Sizzle(expr, document, null, [elem]).length > 0;
             };
 
             Sizzle.contains = function(context, elem) {
+
                 // Set document vars if needed
-                if ((context.ownerDocument || context) !== document) {
+                // Support: IE 11+, Edge 17 - 18+
+                // IE/Edge sometimes throw a "Permission denied" error when strict-comparing
+                // two documents; shallow comparisons work.
+                // eslint-disable-next-line eqeqeq
+                if ((context.ownerDocument || context) != document) {
                     setDocument(context);
                 }
                 return contains(context, elem);
             };
 
             Sizzle.attr = function(elem, name) {
+
                 // Set document vars if needed
-                if ((elem.ownerDocument || elem) !== document) {
+                // Support: IE 11+, Edge 17 - 18+
+                // IE/Edge sometimes throw a "Permission denied" error when strict-comparing
+                // two documents; shallow comparisons work.
+                // eslint-disable-next-line eqeqeq
+                if ((elem.ownerDocument || elem) != document) {
                     setDocument(elem);
                 }
 
                 var fn = Expr.attrHandle[name.toLowerCase()],
+
                     // Don't get fooled by Object.prototype properties (jQuery #13807)
                     val = fn && hasOwn.call(Expr.attrHandle, name.toLowerCase()) ?
                     fn(elem, name, !documentIsHTML) :
                     undefined;
 
                 return val !== undefined ?
                     val :
                     support.attributes || !documentIsHTML ?
                     elem.getAttribute(name) :
                     (val = elem.getAttributeNode(name)) && val.specified ?
                     val.value :
                     null;
             };
 
+            Sizzle.escape = function(sel) {
+                return (sel + "").replace(rcssescape, fcssescape);
+            };
+
             Sizzle.error = function(msg) {
                 throw new Error("Syntax error, unrecognized expression: " + msg);
             };
 
             /**
              * Document sorting and removing duplicates
              * @param {ArrayLike} results
@@ -1512,33 +1723,38 @@
             getText = Sizzle.getText = function(elem) {
                 var node,
                     ret = "",
                     i = 0,
                     nodeType = elem.nodeType;
 
                 if (!nodeType) {
+
                     // If no nodeType, this is expected to be an array
                     while ((node = elem[i++])) {
+
                         // Do not traverse comment nodes
                         ret += getText(node);
                     }
                 } else if (nodeType === 1 || nodeType === 9 || nodeType === 11) {
+
                     // Use textContent for elements
                     // innerText usage removed for consistency of new lines (jQuery #11153)
                     if (typeof elem.textContent === "string") {
                         return elem.textContent;
                     } else {
+
                         // Traverse its children
                         for (elem = elem.firstChild; elem; elem = elem.nextSibling) {
                             ret += getText(elem);
                         }
                     }
                 } else if (nodeType === 3 || nodeType === 4) {
                     return elem.nodeValue;
                 }
+
                 // Do not include comment or processing instruction nodes
 
                 return ret;
             };
 
             Expr = Sizzle.selectors = {
 
@@ -1571,45 +1787,50 @@
                 },
 
                 preFilter: {
                     "ATTR": function(match) {
                         match[1] = match[1].replace(runescape, funescape);
 
                         // Move the given value to match[3] whether quoted or unquoted
-                        match[3] = (match[3] || match[4] || match[5] || "").replace(runescape, funescape);
+                        match[3] = (match[3] || match[4] ||
+                            match[5] || "").replace(runescape, funescape);
 
                         if (match[2] === "~=") {
                             match[3] = " " + match[3] + " ";
                         }
 
                         return match.slice(0, 4);
                     },
 
                     "CHILD": function(match) {
+
                         /* matches from matchExpr["CHILD"]
                         	1 type (only|nth|...)
                         	2 what (child|of-type)
                         	3 argument (even|odd|\d*|\d*n([+-]\d+)?|...)
                         	4 xn-component of xn+y argument ([+-]?\d*n|)
                         	5 sign of xn-component
                         	6 x of xn-component
                         	7 sign of y-component
                         	8 y of y-component
                         */
                         match[1] = match[1].toLowerCase();
 
                         if (match[1].slice(0, 3) === "nth") {
+
                             // nth-* requires argument
                             if (!match[3]) {
                                 Sizzle.error(match[0]);
                             }
 
                             // numeric x and y parameters for Expr.filter.CHILD
                             // remember that false/true cast respectively to 0/1
-                            match[4] = +(match[4] ? match[5] + (match[6] || 1) : 2 * (match[3] === "even" || match[3] === "odd"));
+                            match[4] = +(match[4] ?
+                                match[5] + (match[6] || 1) :
+                                2 * (match[3] === "even" || match[3] === "odd"));
                             match[5] = +((match[7] + match[8]) || match[3] === "odd");
 
                             // other types prohibit arguments
                         } else if (match[3]) {
                             Sizzle.error(match[0]);
                         }
 
@@ -1626,16 +1847,18 @@
 
                         // Accept quoted arguments as-is
                         if (match[3]) {
                             match[2] = match[4] || match[5] || "";
 
                             // Strip excess characters from unquoted arguments
                         } else if (unquoted && rpseudo.test(unquoted) &&
+
                             // Get excess from tokenize (recursively)
                             (excess = tokenize(unquoted, true)) &&
+
                             // advance to the next closing parenthesis
                             (excess = unquoted.indexOf(")", unquoted.length - excess) - unquoted.length)) {
 
                             // excess is a negative index
                             match[0] = match[0].slice(0, excess);
                             match[2] = unquoted.slice(0, excess);
                         }
@@ -1658,18 +1881,25 @@
                             };
                     },
 
                     "CLASS": function(className) {
                         var pattern = classCache[className + " "];
 
                         return pattern ||
-                            (pattern = new RegExp("(^|" + whitespace + ")" + className + "(" + whitespace + "|$)")) &&
-                            classCache(className, function(elem) {
-                                return pattern.test(typeof elem.className === "string" && elem.className || typeof elem.getAttribute !== strundefined && elem.getAttribute("class") || "");
-                            });
+                            (pattern = new RegExp("(^|" + whitespace +
+                                ")" + className + "(" + whitespace + "|$)")) && classCache(
+                                className,
+                                function(elem) {
+                                    return pattern.test(
+                                        typeof elem.className === "string" && elem.className ||
+                                        typeof elem.getAttribute !== "undefined" &&
+                                        elem.getAttribute("class") ||
+                                        ""
+                                    );
+                                });
                     },
 
                     "ATTR": function(name, operator, check) {
                         return function(elem) {
                             var result = Sizzle.attr(elem, name);
 
                             if (result == null) {
@@ -1677,115 +1907,165 @@
                             }
                             if (!operator) {
                                 return true;
                             }
 
                             result += "";
 
+                            /* eslint-disable max-len */
+
                             return operator === "=" ? result === check :
                                 operator === "!=" ? result !== check :
                                 operator === "^=" ? check && result.indexOf(check) === 0 :
                                 operator === "*=" ? check && result.indexOf(check) > -1 :
                                 operator === "$=" ? check && result.slice(-check.length) === check :
-                                operator === "~=" ? (" " + result + " ").indexOf(check) > -1 :
+                                operator === "~=" ? (" " + result.replace(rwhitespace, " ") + " ").indexOf(check) > -1 :
                                 operator === "|=" ? result === check || result.slice(0, check.length + 1) === check + "-" :
                                 false;
+                            /* eslint-enable max-len */
+
                         };
                     },
 
-                    "CHILD": function(type, what, argument, first, last) {
+                    "CHILD": function(type, what, _argument, first, last) {
                         var simple = type.slice(0, 3) !== "nth",
                             forward = type.slice(-4) !== "last",
                             ofType = what === "of-type";
 
                         return first === 1 && last === 0 ?
 
                             // Shortcut for :nth-*(n)
                             function(elem) {
                                 return !!elem.parentNode;
                             } :
 
-                            function(elem, context, xml) {
-                                var cache, outerCache, node, diff, nodeIndex, start,
+                            function(elem, _context, xml) {
+                                var cache, uniqueCache, outerCache, node, nodeIndex, start,
                                     dir = simple !== forward ? "nextSibling" : "previousSibling",
                                     parent = elem.parentNode,
                                     name = ofType && elem.nodeName.toLowerCase(),
-                                    useCache = !xml && !ofType;
+                                    useCache = !xml && !ofType,
+                                    diff = false;
 
                                 if (parent) {
 
                                     // :(first|last|only)-(child|of-type)
                                     if (simple) {
                                         while (dir) {
                                             node = elem;
                                             while ((node = node[dir])) {
-                                                if (ofType ? node.nodeName.toLowerCase() === name : node.nodeType === 1) {
+                                                if (ofType ?
+                                                    node.nodeName.toLowerCase() === name :
+                                                    node.nodeType === 1) {
+
                                                     return false;
                                                 }
                                             }
+
                                             // Reverse direction for :only-* (if we haven't yet done so)
                                             start = dir = type === "only" && !start && "nextSibling";
                                         }
                                         return true;
                                     }
 
                                     start = [forward ? parent.firstChild : parent.lastChild];
 
                                     // non-xml :nth-child(...) stores cache data on `parent`
                                     if (forward && useCache) {
+
                                         // Seek `elem` from a previously-cached index
-                                        outerCache = parent[expando] || (parent[expando] = {});
-                                        cache = outerCache[type] || [];
+
+                                        // ...in a gzip-friendly way
+                                        node = parent;
+                                        outerCache = node[expando] || (node[expando] = {});
+
+                                        // Support: IE <9 only
+                                        // Defend against cloned attroperties (jQuery gh-1709)
+                                        uniqueCache = outerCache[node.uniqueID] ||
+                                            (outerCache[node.uniqueID] = {});
+
+                                        cache = uniqueCache[type] || [];
                                         nodeIndex = cache[0] === dirruns && cache[1];
-                                        diff = cache[0] === dirruns && cache[2];
+                                        diff = nodeIndex && cache[2];
                                         node = nodeIndex && parent.childNodes[nodeIndex];
 
                                         while ((node = ++nodeIndex && node && node[dir] ||
 
                                                 // Fallback to seeking `elem` from the start
                                                 (diff = nodeIndex = 0) || start.pop())) {
 
                                             // When found, cache indexes on `parent` and break
                                             if (node.nodeType === 1 && ++diff && node === elem) {
-                                                outerCache[type] = [dirruns, nodeIndex, diff];
+                                                uniqueCache[type] = [dirruns, nodeIndex, diff];
                                                 break;
                                             }
                                         }
 
+                                    } else {
+
                                         // Use previously-cached element index if available
-                                    } else if (useCache && (cache = (elem[expando] || (elem[expando] = {}))[type]) && cache[0] === dirruns) {
-                                        diff = cache[1];
+                                        if (useCache) {
 
-                                        // xml :nth-child(...) or :nth-last-child(...) or :nth(-last)?-of-type(...)
-                                    } else {
-                                        // Use the same loop as above to seek `elem` from the start
-                                        while ((node = ++nodeIndex && node && node[dir] ||
-                                                (diff = nodeIndex = 0) || start.pop())) {
+                                            // ...in a gzip-friendly way
+                                            node = elem;
+                                            outerCache = node[expando] || (node[expando] = {});
 
-                                            if ((ofType ? node.nodeName.toLowerCase() === name : node.nodeType === 1) && ++diff) {
-                                                // Cache the index of each encountered element
-                                                if (useCache) {
-                                                    (node[expando] || (node[expando] = {}))[type] = [dirruns, diff];
-                                                }
+                                            // Support: IE <9 only
+                                            // Defend against cloned attroperties (jQuery gh-1709)
+                                            uniqueCache = outerCache[node.uniqueID] ||
+                                                (outerCache[node.uniqueID] = {});
+
+                                            cache = uniqueCache[type] || [];
+                                            nodeIndex = cache[0] === dirruns && cache[1];
+                                            diff = nodeIndex;
+                                        }
 
-                                                if (node === elem) {
-                                                    break;
+                                        // xml :nth-child(...)
+                                        // or :nth-last-child(...) or :nth(-last)?-of-type(...)
+                                        if (diff === false) {
+
+                                            // Use the same loop as above to seek `elem` from the start
+                                            while ((node = ++nodeIndex && node && node[dir] ||
+                                                    (diff = nodeIndex = 0) || start.pop())) {
+
+                                                if ((ofType ?
+                                                        node.nodeName.toLowerCase() === name :
+                                                        node.nodeType === 1) &&
+                                                    ++diff) {
+
+                                                    // Cache the index of each encountered element
+                                                    if (useCache) {
+                                                        outerCache = node[expando] ||
+                                                            (node[expando] = {});
+
+                                                        // Support: IE <9 only
+                                                        // Defend against cloned attroperties (jQuery gh-1709)
+                                                        uniqueCache = outerCache[node.uniqueID] ||
+                                                            (outerCache[node.uniqueID] = {});
+
+                                                        uniqueCache[type] = [dirruns, diff];
+                                                    }
+
+                                                    if (node === elem) {
+                                                        break;
+                                                    }
                                                 }
                                             }
                                         }
                                     }
 
                                     // Incorporate the offset, then check against cycle size
                                     diff -= last;
                                     return diff === first || (diff % first === 0 && diff / first >= 0);
                                 }
                             };
                     },
 
                     "PSEUDO": function(pseudo, argument) {
+
                         // pseudo-class names are case-insensitive
                         // http://www.w3.org/TR/selectors/#pseudo-classes
                         // Prioritize by case sensitivity in case custom pseudos are added with uppercase letters
                         // Remember that setFilters inherits from pseudos
                         var args,
                             fn = Expr.pseudos[pseudo] || Expr.setFilters[pseudo.toLowerCase()] ||
                             Sizzle.error("unsupported pseudo: " + pseudo);
@@ -1802,77 +2082,84 @@
                             args = [pseudo, pseudo, "", argument];
                             return Expr.setFilters.hasOwnProperty(pseudo.toLowerCase()) ?
                                 markFunction(function(seed, matches) {
                                     var idx,
                                         matched = fn(seed, argument),
                                         i = matched.length;
                                     while (i--) {
-                                        idx = indexOf.call(seed, matched[i]);
+                                        idx = indexOf(seed, matched[i]);
                                         seed[idx] = !(matches[idx] = matched[i]);
                                     }
                                 }) :
                                 function(elem) {
                                     return fn(elem, 0, args);
                                 };
                         }
 
                         return fn;
                     }
                 },
 
                 pseudos: {
+
                     // Potentially complex pseudos
                     "not": markFunction(function(selector) {
+
                         // Trim the selector passed to compile
                         // to avoid treating leading and trailing
                         // spaces as combinators
                         var input = [],
                             results = [],
                             matcher = compile(selector.replace(rtrim, "$1"));
 
                         return matcher[expando] ?
-                            markFunction(function(seed, matches, context, xml) {
+                            markFunction(function(seed, matches, _context, xml) {
                                 var elem,
                                     unmatched = matcher(seed, null, xml, []),
                                     i = seed.length;
 
                                 // Match elements unmatched by `matcher`
                                 while (i--) {
                                     if ((elem = unmatched[i])) {
                                         seed[i] = !(matches[i] = elem);
                                     }
                                 }
                             }) :
-                            function(elem, context, xml) {
+                            function(elem, _context, xml) {
                                 input[0] = elem;
                                 matcher(input, null, xml, results);
+
+                                // Don't keep the element (issue #299)
+                                input[0] = null;
                                 return !results.pop();
                             };
                     }),
 
                     "has": markFunction(function(selector) {
                         return function(elem) {
                             return Sizzle(selector, elem).length > 0;
                         };
                     }),
 
                     "contains": markFunction(function(text) {
+                        text = text.replace(runescape, funescape);
                         return function(elem) {
-                            return (elem.textContent || elem.innerText || getText(elem)).indexOf(text) > -1;
+                            return (elem.textContent || getText(elem)).indexOf(text) > -1;
                         };
                     }),
 
                     // "Whether an element is represented by a :lang() selector
                     // is based solely on the element's language value
                     // being equal to the identifier C,
                     // or beginning with the identifier C immediately followed by "-".
                     // The matching of C against the element's language value is performed case-insensitively.
                     // The identifier C does not have to be a valid language name."
                     // http://www.w3.org/TR/selectors/#lang-pseudo
                     "lang": markFunction(function(lang) {
+
                         // lang value must be a valid identifier
                         if (!ridentifier.test(lang || "")) {
                             Sizzle.error("unsupported lang: " + lang);
                         }
                         lang = lang.replace(runescape, funescape).toLowerCase();
                         return function(elem) {
                             var elemLang;
@@ -1896,45 +2183,47 @@
                     },
 
                     "root": function(elem) {
                         return elem === docElem;
                     },
 
                     "focus": function(elem) {
-                        return elem === document.activeElement && (!document.hasFocus || document.hasFocus()) && !!(elem.type || elem.href || ~elem.tabIndex);
+                        return elem === document.activeElement &&
+                            (!document.hasFocus || document.hasFocus()) &&
+                            !!(elem.type || elem.href || ~elem.tabIndex);
                     },
 
                     // Boolean properties
-                    "enabled": function(elem) {
-                        return elem.disabled === false;
-                    },
-
-                    "disabled": function(elem) {
-                        return elem.disabled === true;
-                    },
+                    "enabled": createDisabledPseudo(false),
+                    "disabled": createDisabledPseudo(true),
 
                     "checked": function(elem) {
+
                         // In CSS3, :checked should return both checked and selected elements
                         // http://www.w3.org/TR/2011/REC-css3-selectors-20110929/#checked
                         var nodeName = elem.nodeName.toLowerCase();
-                        return (nodeName === "input" && !!elem.checked) || (nodeName === "option" && !!elem.selected);
+                        return (nodeName === "input" && !!elem.checked) ||
+                            (nodeName === "option" && !!elem.selected);
                     },
 
                     "selected": function(elem) {
+
                         // Accessing this property makes selected-by-default
                         // options in Safari work properly
                         if (elem.parentNode) {
+                            // eslint-disable-next-line no-unused-expressions
                             elem.parentNode.selectedIndex;
                         }
 
                         return elem.selected === true;
                     },
 
                     // Contents
                     "empty": function(elem) {
+
                         // http://www.w3.org/TR/selectors/#empty-pseudo
                         // :empty is negated by element (1) or content nodes (text: 3; cdata: 4; entity ref: 5),
                         //   but not by others (comment: 8; processing instruction: 7; etc.)
                         // nodeType < 6 works because attributes (2) do not appear as children
                         for (elem = elem.firstChild; elem; elem = elem.nextSibling) {
                             if (elem.nodeType < 6) {
                                 return false;
@@ -1964,27 +2253,28 @@
                     "text": function(elem) {
                         var attr;
                         return elem.nodeName.toLowerCase() === "input" &&
                             elem.type === "text" &&
 
                             // Support: IE<8
                             // New HTML5 attribute values (e.g., "search") appear with elem.type === "text"
-                            ((attr = elem.getAttribute("type")) == null || attr.toLowerCase() === "text");
+                            ((attr = elem.getAttribute("type")) == null ||
+                                attr.toLowerCase() === "text");
                     },
 
                     // Position-in-collection
                     "first": createPositionalPseudo(function() {
                         return [0];
                     }),
 
-                    "last": createPositionalPseudo(function(matchIndexes, length) {
+                    "last": createPositionalPseudo(function(_matchIndexes, length) {
                         return [length - 1];
                     }),
 
-                    "eq": createPositionalPseudo(function(matchIndexes, length, argument) {
+                    "eq": createPositionalPseudo(function(_matchIndexes, length, argument) {
                         return [argument < 0 ? argument + length : argument];
                     }),
 
                     "even": createPositionalPseudo(function(matchIndexes, length) {
                         var i = 0;
                         for (; i < length; i += 2) {
                             matchIndexes.push(i);
@@ -1997,15 +2287,19 @@
                         for (; i < length; i += 2) {
                             matchIndexes.push(i);
                         }
                         return matchIndexes;
                     }),
 
                     "lt": createPositionalPseudo(function(matchIndexes, length, argument) {
-                        var i = argument < 0 ? argument + length : argument;
+                        var i = argument < 0 ?
+                            argument + length :
+                            argument > length ?
+                            length :
+                            argument;
                         for (; --i >= 0;) {
                             matchIndexes.push(i);
                         }
                         return matchIndexes;
                     }),
 
                     "gt": createPositionalPseudo(function(matchIndexes, length, argument) {
@@ -2056,27 +2350,29 @@
                 preFilters = Expr.preFilter;
 
                 while (soFar) {
 
                     // Comma and first run
                     if (!matched || (match = rcomma.exec(soFar))) {
                         if (match) {
+
                             // Don't consume trailing commas as valid
                             soFar = soFar.slice(match[0].length) || soFar;
                         }
                         groups.push((tokens = []));
                     }
 
                     matched = false;
 
                     // Combinators
                     if ((match = rcombinators.exec(soFar))) {
                         matched = match.shift();
                         tokens.push({
                             value: matched,
+
                             // Cast descendant combinators to space
                             type: match[0].replace(rtrim, " ")
                         });
                         soFar = soFar.slice(matched.length);
                     }
 
                     // Filters
@@ -2101,14 +2397,15 @@
                 // Return the length of the invalid excess
                 // if we're just parsing
                 // Otherwise, throw an error or return tokens
                 return parseOnly ?
                     soFar.length :
                     soFar ?
                     Sizzle.error(selector) :
+
                     // Cache the tokens
                     tokenCache(selector, groups).slice(0);
             };
 
             function toSelector(tokens) {
                 var i = 0,
                     len = tokens.length,
@@ -2117,62 +2414,76 @@
                     selector += tokens[i].value;
                 }
                 return selector;
             }
 
             function addCombinator(matcher, combinator, base) {
                 var dir = combinator.dir,
-                    checkNonElements = base && dir === "parentNode",
+                    skip = combinator.next,
+                    key = skip || dir,
+                    checkNonElements = base && key === "parentNode",
                     doneName = done++;
 
                 return combinator.first ?
+
                     // Check against closest ancestor/preceding element
                     function(elem, context, xml) {
                         while ((elem = elem[dir])) {
                             if (elem.nodeType === 1 || checkNonElements) {
                                 return matcher(elem, context, xml);
                             }
                         }
+                        return false;
                     } :
 
                     // Check against all ancestor/preceding elements
                     function(elem, context, xml) {
-                        var oldCache, outerCache,
+                        var oldCache, uniqueCache, outerCache,
                             newCache = [dirruns, doneName];
 
-                        // We can't set arbitrary data on XML nodes, so they don't benefit from dir caching
+                        // We can't set arbitrary data on XML nodes, so they don't benefit from combinator caching
                         if (xml) {
                             while ((elem = elem[dir])) {
                                 if (elem.nodeType === 1 || checkNonElements) {
                                     if (matcher(elem, context, xml)) {
                                         return true;
                                     }
                                 }
                             }
                         } else {
                             while ((elem = elem[dir])) {
                                 if (elem.nodeType === 1 || checkNonElements) {
                                     outerCache = elem[expando] || (elem[expando] = {});
-                                    if ((oldCache = outerCache[dir]) &&
+
+                                    // Support: IE <9 only
+                                    // Defend against cloned attroperties (jQuery gh-1709)
+                                    uniqueCache = outerCache[elem.uniqueID] ||
+                                        (outerCache[elem.uniqueID] = {});
+
+                                    if (skip && skip === elem.nodeName.toLowerCase()) {
+                                        elem = elem[dir] || elem;
+                                    } else if ((oldCache = uniqueCache[key]) &&
                                         oldCache[0] === dirruns && oldCache[1] === doneName) {
 
                                         // Assign to newCache so results back-propagate to previous elements
                                         return (newCache[2] = oldCache[2]);
                                     } else {
+
                                         // Reuse newcache so results back-propagate to previous elements
-                                        outerCache[dir] = newCache;
+                                        uniqueCache[key] = newCache;
 
                                         // A match means we're done; a fail means we have to keep checking
                                         if ((newCache[2] = matcher(elem, context, xml))) {
                                             return true;
                                         }
                                     }
                                 }
                             }
                         }
+                        return false;
                     };
             }
 
             function elementMatcher(matchers) {
                 return matchers.length > 1 ?
                     function(elem, context, xml) {
                         var i = matchers.length;
@@ -2226,22 +2537,27 @@
                 return markFunction(function(seed, results, context, xml) {
                     var temp, i, elem,
                         preMap = [],
                         postMap = [],
                         preexisting = results.length,
 
                         // Get initial elements from seed or context
-                        elems = seed || multipleContexts(selector || "*", context.nodeType ? [context] : context, []),
+                        elems = seed || multipleContexts(
+                            selector || "*",
+                            context.nodeType ? [context] : context,
+                            []
+                        ),
 
                         // Prefilter to get matcher input, preserving a map for seed-results synchronization
                         matcherIn = preFilter && (seed || !selector) ?
                         condense(elems, preMap, preFilter, context, xml) :
                         elems,
 
                         matcherOut = matcher ?
+
                         // If we have a postFinder, or filtered seed, or non-seed postFilter or preexisting results,
                         postFinder || (seed ? preFilter : preexisting || postFilter) ?
 
                         // ...intermediate processing is necessary
                         [] :
 
                         // ...otherwise use results directly
@@ -2266,31 +2582,33 @@
                             }
                         }
                     }
 
                     if (seed) {
                         if (postFinder || preFilter) {
                             if (postFinder) {
+
                                 // Get the final matcherOut by condensing this intermediate into postFinder contexts
                                 temp = [];
                                 i = matcherOut.length;
                                 while (i--) {
                                     if ((elem = matcherOut[i])) {
+
                                         // Restore matcherIn since elem is not yet a final match
                                         temp.push((matcherIn[i] = elem));
                                     }
                                 }
                                 postFinder(null, (matcherOut = []), temp, xml);
                             }
 
                             // Move matched elements from seed to results to keep them synchronized
                             i = matcherOut.length;
                             while (i--) {
                                 if ((elem = matcherOut[i]) &&
-                                    (temp = postFinder ? indexOf.call(seed, elem) : preMap[i]) > -1) {
+                                    (temp = postFinder ? indexOf(seed, elem) : preMap[i]) > -1) {
 
                                     seed[temp] = !(results[temp] = elem);
                                 }
                             }
                         }
 
                         // Add elements to results, through postFinder if defined
@@ -2317,43 +2635,51 @@
                     i = leadingRelative ? 1 : 0,
 
                     // The foundational matcher ensures that elements are reachable from top-level context(s)
                     matchContext = addCombinator(function(elem) {
                         return elem === checkContext;
                     }, implicitRelative, true),
                     matchAnyContext = addCombinator(function(elem) {
-                        return indexOf.call(checkContext, elem) > -1;
+                        return indexOf(checkContext, elem) > -1;
                     }, implicitRelative, true),
                     matchers = [function(elem, context, xml) {
-                        return (!leadingRelative && (xml || context !== outermostContext)) || (
+                        var ret = (!leadingRelative && (xml || context !== outermostContext)) || (
                             (checkContext = context).nodeType ?
                             matchContext(elem, context, xml) :
                             matchAnyContext(elem, context, xml));
+
+                        // Avoid hanging onto element (issue #299)
+                        checkContext = null;
+                        return ret;
                     }];
 
                 for (; i < len; i++) {
                     if ((matcher = Expr.relative[tokens[i].type])) {
                         matchers = [addCombinator(elementMatcher(matchers), matcher)];
                     } else {
                         matcher = Expr.filter[tokens[i].type].apply(null, tokens[i].matches);
 
                         // Return special upon seeing a positional matcher
                         if (matcher[expando]) {
+
                             // Find the next relative operator (if any) for proper handling
                             j = ++i;
                             for (; j < len; j++) {
                                 if (Expr.relative[tokens[j].type]) {
                                     break;
                                 }
                             }
                             return setMatcher(
                                 i > 1 && elementMatcher(matchers),
                                 i > 1 && toSelector(
+
                                     // If the preceding token was a descendant combinator, insert an implicit any-element `*`
-                                    tokens.slice(0, i - 1).concat({
+                                    tokens
+                                    .slice(0, i - 1)
+                                    .concat({
                                         value: tokens[i - 2].type === " " ? "*" : ""
                                     })
                                 ).replace(rtrim, "$1"),
                                 matcher,
                                 i < j && matcherFromTokens(tokens.slice(i, j)),
                                 j < len && matcherFromTokens((tokens = tokens.slice(j))),
                                 j < len && toSelector(tokens)
@@ -2372,65 +2698,91 @@
                     superMatcher = function(seed, context, xml, results, outermost) {
                         var elem, j, matcher,
                             matchedCount = 0,
                             i = "0",
                             unmatched = seed && [],
                             setMatched = [],
                             contextBackup = outermostContext,
+
                             // We must always have either seed elements or outermost context
                             elems = seed || byElement && Expr.find["TAG"]("*", outermost),
+
                             // Use integer dirruns iff this is the outermost matcher
                             dirrunsUnique = (dirruns += contextBackup == null ? 1 : Math.random() || 0.1),
                             len = elems.length;
 
                         if (outermost) {
-                            outermostContext = context !== document && context;
+
+                            // Support: IE 11+, Edge 17 - 18+
+                            // IE/Edge sometimes throw a "Permission denied" error when strict-comparing
+                            // two documents; shallow comparisons work.
+                            // eslint-disable-next-line eqeqeq
+                            outermostContext = context == document || context || outermost;
                         }
 
                         // Add elements passing elementMatchers directly to results
-                        // Keep `i` a string if there are no elements so `matchedCount` will be "00" below
                         // Support: IE<9, Safari
                         // Tolerate NodeList properties (IE: "length"; Safari: <number>) matching elements by id
                         for (; i !== len && (elem = elems[i]) != null; i++) {
                             if (byElement && elem) {
                                 j = 0;
+
+                                // Support: IE 11+, Edge 17 - 18+
+                                // IE/Edge sometimes throw a "Permission denied" error when strict-comparing
+                                // two documents; shallow comparisons work.
+                                // eslint-disable-next-line eqeqeq
+                                if (!context && elem.ownerDocument != document) {
+                                    setDocument(elem);
+                                    xml = !documentIsHTML;
+                                }
                                 while ((matcher = elementMatchers[j++])) {
-                                    if (matcher(elem, context, xml)) {
+                                    if (matcher(elem, context || document, xml)) {
                                         results.push(elem);
                                         break;
                                     }
                                 }
                                 if (outermost) {
                                     dirruns = dirrunsUnique;
                                 }
                             }
 
                             // Track unmatched elements for set filters
                             if (bySet) {
+
                                 // They will have gone through all possible matchers
                                 if ((elem = !matcher && elem)) {
                                     matchedCount--;
                                 }
 
                                 // Lengthen the array for every element, matched or not
                                 if (seed) {
                                     unmatched.push(elem);
                                 }
                             }
                         }
 
-                        // Apply set filters to unmatched elements
+                        // `i` is now the count of elements visited above, and adding it to `matchedCount`
+                        // makes the latter nonnegative.
                         matchedCount += i;
+
+                        // Apply set filters to unmatched elements
+                        // NOTE: This can be skipped if there are no unmatched elements (i.e., `matchedCount`
+                        // equals `i`), unless we didn't visit _any_ elements in the above loop because we have
+                        // no element matchers and no seed.
+                        // Incrementing an initially-string "0" `i` allows `i` to remain a string only in that
+                        // case, which will result in a "00" `matchedCount` that differs from `i` but is also
+                        // numerically zero.
                         if (bySet && i !== matchedCount) {
                             j = 0;
                             while ((matcher = setMatchers[j++])) {
                                 matcher(unmatched, setMatched, context, xml);
                             }
 
                             if (seed) {
+
                                 // Reintegrate element matches to eliminate the need for sorting
                                 if (matchedCount > 0) {
                                     while (i--) {
                                         if (!(unmatched[i] || setMatched[i])) {
                                             setMatched[i] = pop.call(results);
                                         }
                                     }
@@ -2468,14 +2820,15 @@
             compile = Sizzle.compile = function(selector, match /* Internal Use Only */ ) {
                 var i,
                     setMatchers = [],
                     elementMatchers = [],
                     cached = compilerCache[selector + " "];
 
                 if (!cached) {
+
                     // Generate a function of recursive functions that can be used to check each element
                     if (!match) {
                         match = tokenize(selector);
                     }
                     i = match.length;
                     while (i--) {
                         cached = matcherFromTokens(match[i]);
@@ -2483,15 +2836,18 @@
                             setMatchers.push(cached);
                         } else {
                             elementMatchers.push(cached);
                         }
                     }
 
                     // Cache the compiled function
-                    cached = compilerCache(selector, matcherFromGroupMatchers(elementMatchers, setMatchers));
+                    cached = compilerCache(
+                        selector,
+                        matcherFromGroupMatchers(elementMatchers, setMatchers)
+                    );
 
                     // Save selector and tokenization
                     cached.selector = selector;
                 }
                 return cached;
             };
 
@@ -2507,24 +2863,25 @@
             select = Sizzle.select = function(selector, context, results, seed) {
                 var i, tokens, token, type, find,
                     compiled = typeof selector === "function" && selector,
                     match = !seed && tokenize((selector = compiled.selector || selector));
 
                 results = results || [];
 
-                // Try to minimize operations if there is no seed and only one group
+                // Try to minimize operations if there is only one selector in the list and no seed
+                // (the latter of which guarantees us context)
                 if (match.length === 1) {
 
-                    // Take a shortcut and set the context if the root selector is an ID
+                    // Reduce context if the leading compound selector is an ID
                     tokens = match[0] = match[0].slice(0);
                     if (tokens.length > 2 && (token = tokens[0]).type === "ID" &&
-                        support.getById && context.nodeType === 9 && documentIsHTML &&
-                        Expr.relative[tokens[1].type]) {
+                        context.nodeType === 9 && documentIsHTML && Expr.relative[tokens[1].type]) {
 
-                        context = (Expr.find["ID"](token.matches[0].replace(runescape, funescape), context) || [])[0];
+                        context = (Expr.find["ID"](token.matches[0]
+                            .replace(runescape, funescape), context) || [])[0];
                         if (!context) {
                             return results;
 
                             // Precompiled matchers will still verify ancestry, so step up a level
                         } else if (compiled) {
                             context = context.parentNode;
                         }
@@ -2538,18 +2895,20 @@
                         token = tokens[i];
 
                         // Abort if we hit a combinator
                         if (Expr.relative[(type = token.type)]) {
                             break;
                         }
                         if ((find = Expr.find[type])) {
+
                             // Search, expanding context for leading sibling combinators
                             if ((seed = find(
                                     token.matches[0].replace(runescape, funescape),
-                                    rsibling.test(tokens[0].type) && testContext(context.parentNode) || context
+                                    rsibling.test(tokens[0].type) && testContext(context.parentNode) ||
+                                    context
                                 ))) {
 
                                 // If seed is empty or no tokens remain, we can return early
                                 tokens.splice(i, 1);
                                 selector = seed.length && toSelector(tokens);
                                 if (!selector) {
                                     push.apply(results, seed);
@@ -2565,70 +2924,71 @@
                 // Compile and execute a filtering function if one is not provided
                 // Provide `match` to avoid retokenization if we modified the selector above
                 (compiled || compile(selector, match))(
                     seed,
                     context,
                     !documentIsHTML,
                     results,
-                    rsibling.test(selector) && testContext(context.parentNode) || context
+                    !context || rsibling.test(selector) && testContext(context.parentNode) || context
                 );
                 return results;
             };
 
             // One-time assignments
 
             // Sort stability
             support.sortStable = expando.split("").sort(sortOrder).join("") === expando;
 
-            // Support: Chrome<14
+            // Support: Chrome 14-35+
             // Always assume duplicates if they aren't passed to the comparison function
             support.detectDuplicates = !!hasDuplicate;
 
             // Initialize against the default document
             setDocument();
 
             // Support: Webkit<537.32 - Safari 6.0.3/Chrome 25 (fixed in Chrome 27)
             // Detached nodes confoundingly follow *each other*
-            support.sortDetached = assert(function(div1) {
+            support.sortDetached = assert(function(el) {
+
                 // Should return 1, but returns 4 (following)
-                return div1.compareDocumentPosition(document.createElement("div")) & 1;
+                return el.compareDocumentPosition(document.createElement("fieldset")) & 1;
             });
 
             // Support: IE<8
             // Prevent attribute/property "interpolation"
-            // http://msdn.microsoft.com/en-us/library/ms536429%28VS.85%29.aspx
-            if (!assert(function(div) {
-                    div.innerHTML = "<a href='#'></a>";
-                    return div.firstChild.getAttribute("href") === "#";
+            // https://msdn.microsoft.com/en-us/library/ms536429%28VS.85%29.aspx
+            if (!assert(function(el) {
+                    el.innerHTML = "<a href='#'></a>";
+                    return el.firstChild.getAttribute("href") === "#";
                 })) {
                 addHandle("type|href|height|width", function(elem, name, isXML) {
                     if (!isXML) {
                         return elem.getAttribute(name, name.toLowerCase() === "type" ? 1 : 2);
                     }
                 });
             }
 
             // Support: IE<9
             // Use defaultValue in place of getAttribute("value")
-            if (!support.attributes || !assert(function(div) {
-                    div.innerHTML = "<input/>";
-                    div.firstChild.setAttribute("value", "");
-                    return div.firstChild.getAttribute("value") === "";
+            if (!support.attributes || !assert(function(el) {
+                    el.innerHTML = "<input/>";
+                    el.firstChild.setAttribute("value", "");
+                    return el.firstChild.getAttribute("value") === "";
                 })) {
-                addHandle("value", function(elem, name, isXML) {
+                addHandle("value", function(elem, _name, isXML) {
                     if (!isXML && elem.nodeName.toLowerCase() === "input") {
                         return elem.defaultValue;
                     }
                 });
             }
 
             // Support: IE<9
             // Use getAttributeNode to fetch booleans when getAttribute lies
-            if (!assert(function(div) {
-                    return div.getAttribute("disabled") == null;
+            if (!assert(function(el) {
+                    return el.getAttribute("disabled") == null;
                 })) {
                 addHandle(booleans, function(elem, name, isXML) {
                     var val;
                     if (!isXML) {
                         return elem[name] === true ? name.toLowerCase() :
                             (val = elem.getAttributeNode(name)) && val.specified ?
                             val.value :
@@ -2641,99 +3001,133 @@
 
         })(window);
 
 
 
     jQuery.find = Sizzle;
     jQuery.expr = Sizzle.selectors;
+
+    // Deprecated
     jQuery.expr[":"] = jQuery.expr.pseudos;
-    jQuery.unique = Sizzle.uniqueSort;
+    jQuery.uniqueSort = jQuery.unique = Sizzle.uniqueSort;
     jQuery.text = Sizzle.getText;
     jQuery.isXMLDoc = Sizzle.isXML;
     jQuery.contains = Sizzle.contains;
+    jQuery.escapeSelector = Sizzle.escape;
+
 
 
 
+    var dir = function(elem, dir, until) {
+        var matched = [],
+            truncate = until !== undefined;
+
+        while ((elem = elem[dir]) && elem.nodeType !== 9) {
+            if (elem.nodeType === 1) {
+                if (truncate && jQuery(elem).is(until)) {
+                    break;
+                }
+                matched.push(elem);
+            }
+        }
+        return matched;
+    };
+
+
+    var siblings = function(n, elem) {
+        var matched = [];
+
+        for (; n; n = n.nextSibling) {
+            if (n.nodeType === 1 && n !== elem) {
+                matched.push(n);
+            }
+        }
+
+        return matched;
+    };
+
+
     var rneedsContext = jQuery.expr.match.needsContext;
 
-    var rsingleTag = (/^<(\w+)\s*\/?>(?:<\/\1>|)$/);
 
 
+    function nodeName(elem, name) {
+
+        return elem.nodeName && elem.nodeName.toLowerCase() === name.toLowerCase();
+
+    }
+    var rsingleTag = (/^<([a-z][^\/\0>:\x20\t\r\n\f]*)[\x20\t\r\n\f]*\/?>(?:<\/\1>|)$/i);
+
 
-    var risSimple = /^.[^:#\[\.,]*$/;
 
     // Implement the identical functionality for filter and not
     function winnow(elements, qualifier, not) {
-        if (jQuery.isFunction(qualifier)) {
+        if (isFunction(qualifier)) {
             return jQuery.grep(elements, function(elem, i) {
-                /* jshint -W018 */
                 return !!qualifier.call(elem, i, elem) !== not;
             });
-
         }
 
+        // Single element
         if (qualifier.nodeType) {
             return jQuery.grep(elements, function(elem) {
                 return (elem === qualifier) !== not;
             });
-
         }
 
-        if (typeof qualifier === "string") {
-            if (risSimple.test(qualifier)) {
-                return jQuery.filter(qualifier, elements, not);
-            }
-
-            qualifier = jQuery.filter(qualifier, elements);
+        // Arraylike of elements (jQuery, arguments, Array)
+        if (typeof qualifier !== "string") {
+            return jQuery.grep(elements, function(elem) {
+                return (indexOf.call(qualifier, elem) > -1) !== not;
+            });
         }
 
-        return jQuery.grep(elements, function(elem) {
-            return (jQuery.inArray(elem, qualifier) >= 0) !== not;
-        });
+        // Filtered directly for both simple and complex selectors
+        return jQuery.filter(qualifier, elements, not);
     }
 
     jQuery.filter = function(expr, elems, not) {
         var elem = elems[0];
 
         if (not) {
             expr = ":not(" + expr + ")";
         }
 
-        return elems.length === 1 && elem.nodeType === 1 ?
-            jQuery.find.matchesSelector(elem, expr) ? [elem] : [] :
-            jQuery.find.matches(expr, jQuery.grep(elems, function(elem) {
-                return elem.nodeType === 1;
-            }));
+        if (elems.length === 1 && elem.nodeType === 1) {
+            return jQuery.find.matchesSelector(elem, expr) ? [elem] : [];
+        }
+
+        return jQuery.find.matches(expr, jQuery.grep(elems, function(elem) {
+            return elem.nodeType === 1;
+        }));
     };
 
     jQuery.fn.extend({
         find: function(selector) {
-            var i,
-                ret = [],
-                self = this,
-                len = self.length;
+            var i, ret,
+                len = this.length,
+                self = this;
 
             if (typeof selector !== "string") {
                 return this.pushStack(jQuery(selector).filter(function() {
                     for (i = 0; i < len; i++) {
                         if (jQuery.contains(self[i], this)) {
                             return true;
                         }
                     }
                 }));
             }
 
+            ret = this.pushStack([]);
+
             for (i = 0; i < len; i++) {
                 jQuery.find(selector, self[i], ret);
             }
 
-            // Needed because $( selector, context ) becomes $( context ).find( selector )
-            ret = this.pushStack(len > 1 ? jQuery.unique(ret) : ret);
-            ret.selector = this.selector ? this.selector + " " + selector : selector;
-            return ret;
+            return len > 1 ? jQuery.uniqueSort(ret) : ret;
         },
         filter: function(selector) {
             return this.pushStack(winnow(this, selector || [], false));
         },
         not: function(selector) {
             return this.pushStack(winnow(this, selector || [], true));
         },
@@ -2754,60 +3148,66 @@
 
     // Initialize a jQuery object
 
 
     // A central reference to the root jQuery(document)
     var rootjQuery,
 
-        // Use the correct document accordingly with window argument (sandbox)
-        document = window.document,
-
         // A simple way to check for HTML strings
-        // Prioritize #id over <tag> to avoid XSS via location.hash (#9521)
-        // Strict HTML recognition (#11290: must start with <)
-        rquickExpr = /^(?:\s*(<[\w\W]+>)[^>]*|#([\w-]*))$/,
+        // Prioritize #id over <tag> to avoid XSS via location.hash (trac-9521)
+        // Strict HTML recognition (trac-11290: must start with <)
+        // Shortcut simple #id case for speed
+        rquickExpr = /^(?:\s*(<[\w\W]+>)[^>]*|#([\w-]+))$/,
 
-        init = jQuery.fn.init = function(selector, context) {
+        init = jQuery.fn.init = function(selector, context, root) {
             var match, elem;
 
             // HANDLE: $(""), $(null), $(undefined), $(false)
             if (!selector) {
                 return this;
             }
 
+            // Method init() accepts an alternate rootjQuery
+            // so migrate can support jQuery.sub (gh-2101)
+            root = root || rootjQuery;
+
             // Handle HTML strings
             if (typeof selector === "string") {
-                if (selector.charAt(0) === "<" && selector.charAt(selector.length - 1) === ">" && selector.length >= 3) {
+                if (selector[0] === "<" &&
+                    selector[selector.length - 1] === ">" &&
+                    selector.length >= 3) {
+
                     // Assume that strings that start and end with <> are HTML and skip the regex check
                     match = [null, selector, null];
 
                 } else {
                     match = rquickExpr.exec(selector);
                 }
 
                 // Match html or make sure no context is specified for #id
                 if (match && (match[1] || !context)) {
 
                     // HANDLE: $(html) -> $(array)
                     if (match[1]) {
                         context = context instanceof jQuery ? context[0] : context;
 
-                        // scripts is true for back-compat
+                        // Option to run scripts is true for back-compat
                         // Intentionally let the error be thrown if parseHTML is not present
                         jQuery.merge(this, jQuery.parseHTML(
                             match[1],
                             context && context.nodeType ? context.ownerDocument || context : document,
                             true
                         ));
 
                         // HANDLE: $(html, props)
                         if (rsingleTag.test(match[1]) && jQuery.isPlainObject(context)) {
                             for (match in context) {
+
                                 // Properties of context are called as methods if possible
-                                if (jQuery.isFunction(this[match])) {
+                                if (isFunction(this[match])) {
                                     this[match](context[match]);
 
                                     // ...and otherwise set as attributes
                                 } else {
                                     this.attr(match, context[match]);
                                 }
                             }
@@ -2815,273 +3215,246 @@
 
                         return this;
 
                         // HANDLE: $(#id)
                     } else {
                         elem = document.getElementById(match[2]);
 
-                        // Check parentNode to catch when Blackberry 4.6 returns
-                        // nodes that are no longer in the document #6963
-                        if (elem && elem.parentNode) {
-                            // Handle the case where IE and Opera return items
-                            // by name instead of ID
-                            if (elem.id !== match[2]) {
-                                return rootjQuery.find(selector);
-                            }
+                        if (elem) {
 
-                            // Otherwise, we inject the element directly into the jQuery object
-                            this.length = 1;
+                            // Inject the element directly into the jQuery object
                             this[0] = elem;
+                            this.length = 1;
                         }
-
-                        this.context = document;
-                        this.selector = selector;
                         return this;
                     }
 
                     // HANDLE: $(expr, $(...))
                 } else if (!context || context.jquery) {
-                    return (context || rootjQuery).find(selector);
+                    return (context || root).find(selector);
 
                     // HANDLE: $(expr, context)
                     // (which is just equivalent to: $(context).find(expr)
                 } else {
                     return this.constructor(context).find(selector);
                 }
 
                 // HANDLE: $(DOMElement)
             } else if (selector.nodeType) {
-                this.context = this[0] = selector;
+                this[0] = selector;
                 this.length = 1;
                 return this;
 
                 // HANDLE: $(function)
                 // Shortcut for document ready
-            } else if (jQuery.isFunction(selector)) {
-                return typeof rootjQuery.ready !== "undefined" ?
-                    rootjQuery.ready(selector) :
+            } else if (isFunction(selector)) {
+                return root.ready !== undefined ?
+                    root.ready(selector) :
+
                     // Execute immediately if ready is not present
                     selector(jQuery);
             }
 
-            if (selector.selector !== undefined) {
-                this.selector = selector.selector;
-                this.context = selector.context;
-            }
-
             return jQuery.makeArray(selector, this);
         };
 
     // Give the init function the jQuery prototype for later instantiation
     init.prototype = jQuery.fn;
 
     // Initialize central reference
     rootjQuery = jQuery(document);
 
 
     var rparentsprev = /^(?:parents|prev(?:Until|All))/,
-        // methods guaranteed to produce a unique set when starting from a unique set
+
+        // Methods guaranteed to produce a unique set when starting from a unique set
         guaranteedUnique = {
             children: true,
             contents: true,
             next: true,
             prev: true
         };
 
-    jQuery.extend({
-        dir: function(elem, dir, until) {
-            var matched = [],
-                cur = elem[dir];
-
-            while (cur && cur.nodeType !== 9 && (until === undefined || cur.nodeType !== 1 || !jQuery(cur).is(until))) {
-                if (cur.nodeType === 1) {
-                    matched.push(cur);
-                }
-                cur = cur[dir];
-            }
-            return matched;
-        },
-
-        sibling: function(n, elem) {
-            var r = [];
-
-            for (; n; n = n.nextSibling) {
-                if (n.nodeType === 1 && n !== elem) {
-                    r.push(n);
-                }
-            }
-
-            return r;
-        }
-    });
-
     jQuery.fn.extend({
         has: function(target) {
-            var i,
-                targets = jQuery(target, this),
-                len = targets.length;
+            var targets = jQuery(target, this),
+                l = targets.length;
 
             return this.filter(function() {
-                for (i = 0; i < len; i++) {
+                var i = 0;
+                for (; i < l; i++) {
                     if (jQuery.contains(this, targets[i])) {
                         return true;
                     }
                 }
             });
         },
 
         closest: function(selectors, context) {
             var cur,
                 i = 0,
                 l = this.length,
                 matched = [],
-                pos = rneedsContext.test(selectors) || typeof selectors !== "string" ?
-                jQuery(selectors, context || this.context) :
-                0;
-
-            for (; i < l; i++) {
-                for (cur = this[i]; cur && cur !== context; cur = cur.parentNode) {
-                    // Always skip document fragments
-                    if (cur.nodeType < 11 && (pos ?
-                            pos.index(cur) > -1 :
-
-                            // Don't pass non-elements to Sizzle
-                            cur.nodeType === 1 &&
-                            jQuery.find.matchesSelector(cur, selectors))) {
+                targets = typeof selectors !== "string" && jQuery(selectors);
 
-                        matched.push(cur);
-                        break;
+            // Positional selectors never match, since there's no _selection_ context
+            if (!rneedsContext.test(selectors)) {
+                for (; i < l; i++) {
+                    for (cur = this[i]; cur && cur !== context; cur = cur.parentNode) {
+
+                        // Always skip document fragments
+                        if (cur.nodeType < 11 && (targets ?
+                                targets.index(cur) > -1 :
+
+                                // Don't pass non-elements to Sizzle
+                                cur.nodeType === 1 &&
+                                jQuery.find.matchesSelector(cur, selectors))) {
+
+                            matched.push(cur);
+                            break;
+                        }
                     }
                 }
             }
 
-            return this.pushStack(matched.length > 1 ? jQuery.unique(matched) : matched);
+            return this.pushStack(matched.length > 1 ? jQuery.uniqueSort(matched) : matched);
         },
 
-        // Determine the position of an element within
-        // the matched set of elements
+        // Determine the position of an element within the set
         index: function(elem) {
 
             // No argument, return index in parent
             if (!elem) {
                 return (this[0] && this[0].parentNode) ? this.first().prevAll().length : -1;
             }
 
-            // index in selector
+            // Index in selector
             if (typeof elem === "string") {
-                return jQuery.inArray(this[0], jQuery(elem));
+                return indexOf.call(jQuery(elem), this[0]);
             }
 
             // Locate the position of the desired element
-            return jQuery.inArray(
+            return indexOf.call(this,
+
                 // If it receives a jQuery object, the first element is used
-                elem.jquery ? elem[0] : elem, this);
+                elem.jquery ? elem[0] : elem
+            );
         },
 
         add: function(selector, context) {
             return this.pushStack(
-                jQuery.unique(
+                jQuery.uniqueSort(
                     jQuery.merge(this.get(), jQuery(selector, context))
                 )
             );
         },
 
         addBack: function(selector) {
             return this.add(selector == null ?
                 this.prevObject : this.prevObject.filter(selector)
             );
         }
     });
 
     function sibling(cur, dir) {
-        do {
-            cur = cur[dir];
-        } while (cur && cur.nodeType !== 1);
-
+        while ((cur = cur[dir]) && cur.nodeType !== 1) {}
         return cur;
     }
 
     jQuery.each({
         parent: function(elem) {
             var parent = elem.parentNode;
             return parent && parent.nodeType !== 11 ? parent : null;
         },
         parents: function(elem) {
-            return jQuery.dir(elem, "parentNode");
+            return dir(elem, "parentNode");
         },
-        parentsUntil: function(elem, i, until) {
-            return jQuery.dir(elem, "parentNode", until);
+        parentsUntil: function(elem, _i, until) {
+            return dir(elem, "parentNode", until);
         },
         next: function(elem) {
             return sibling(elem, "nextSibling");
         },
         prev: function(elem) {
             return sibling(elem, "previousSibling");
         },
         nextAll: function(elem) {
-            return jQuery.dir(elem, "nextSibling");
+            return dir(elem, "nextSibling");
         },
         prevAll: function(elem) {
-            return jQuery.dir(elem, "previousSibling");
+            return dir(elem, "previousSibling");
         },
-        nextUntil: function(elem, i, until) {
-            return jQuery.dir(elem, "nextSibling", until);
+        nextUntil: function(elem, _i, until) {
+            return dir(elem, "nextSibling", until);
         },
-        prevUntil: function(elem, i, until) {
-            return jQuery.dir(elem, "previousSibling", until);
+        prevUntil: function(elem, _i, until) {
+            return dir(elem, "previousSibling", until);
         },
         siblings: function(elem) {
-            return jQuery.sibling((elem.parentNode || {}).firstChild, elem);
+            return siblings((elem.parentNode || {}).firstChild, elem);
         },
         children: function(elem) {
-            return jQuery.sibling(elem.firstChild);
+            return siblings(elem.firstChild);
         },
         contents: function(elem) {
-            return jQuery.nodeName(elem, "iframe") ?
-                elem.contentDocument || elem.contentWindow.document :
-                jQuery.merge([], elem.childNodes);
+            if (elem.contentDocument != null &&
+
+                // Support: IE 11+
+                // <object> elements with no `data` attribute has an object
+                // `contentDocument` with a `null` prototype.
+                getProto(elem.contentDocument)) {
+
+                return elem.contentDocument;
+            }
+
+            // Support: IE 9 - 11 only, iOS 7 only, Android Browser <=4.3 only
+            // Treat the template element as a regular one in browsers that
+            // don't support it.
+            if (nodeName(elem, "template")) {
+                elem = elem.content || elem;
+            }
+
+            return jQuery.merge([], elem.childNodes);
         }
     }, function(name, fn) {
         jQuery.fn[name] = function(until, selector) {
-            var ret = jQuery.map(this, fn, until);
+            var matched = jQuery.map(this, fn, until);
 
             if (name.slice(-5) !== "Until") {
                 selector = until;
             }
 
             if (selector && typeof selector === "string") {
-                ret = jQuery.filter(selector, ret);
+                matched = jQuery.filter(selector, matched);
             }
 
             if (this.length > 1) {
+
                 // Remove duplicates
                 if (!guaranteedUnique[name]) {
-                    ret = jQuery.unique(ret);
+                    jQuery.uniqueSort(matched);
                 }
 
                 // Reverse order for parents* and prev-derivatives
                 if (rparentsprev.test(name)) {
-                    ret = ret.reverse();
+                    matched.reverse();
                 }
             }
 
-            return this.pushStack(ret);
+            return this.pushStack(matched);
         };
     });
-    var rnotwhite = (/\S+/g);
-
+    var rnothtmlwhite = (/[^\x20\t\r\n\f]+/g);
 
 
-    // String to Object options format cache
-    var optionsCache = {};
 
-    // Convert String-formatted options into Object-formatted ones and store in cache
+    // Convert String-formatted options into Object-formatted ones
     function createOptions(options) {
-        var object = optionsCache[options] = {};
-        jQuery.each(options.match(rnotwhite) || [], function(_, flag) {
+        var object = {};
+        jQuery.each(options.match(rnothtmlwhite) || [], function(_, flag) {
             object[flag] = true;
         });
         return object;
     }
 
     /*
      * Create a callback list using the following parameters:
@@ -3106,247 +3479,532 @@
      *
      */
     jQuery.Callbacks = function(options) {
 
         // Convert options from String-formatted to Object-formatted if needed
         // (we check in cache first)
         options = typeof options === "string" ?
-            (optionsCache[options] || createOptions(options)) :
+            createOptions(options) :
             jQuery.extend({}, options);
 
         var // Flag to know if list is currently firing
             firing,
-            // Last fire value (for non-forgettable lists)
+
+            // Last fire value for non-forgettable lists
             memory,
+
             // Flag to know if list was already fired
             fired,
-            // End of the loop when firing
-            firingLength,
-            // Index of currently firing callback (modified by remove if needed)
-            firingIndex,
-            // First callback to fire (used internally by add and fireWith)
-            firingStart,
+
+            // Flag to prevent firing
+            locked,
+
             // Actual callback list
             list = [],
-            // Stack of fire calls for repeatable lists
-            stack = !options.once && [],
+
+            // Queue of execution data for repeatable lists
+            queue = [],
+
+            // Index of currently firing callback (modified by add/remove as needed)
+            firingIndex = -1,
+
             // Fire callbacks
-            fire = function(data) {
-                memory = options.memory && data;
-                fired = true;
-                firingIndex = firingStart || 0;
-                firingStart = 0;
-                firingLength = list.length;
-                firing = true;
-                for (; list && firingIndex < firingLength; firingIndex++) {
-                    if (list[firingIndex].apply(data[0], data[1]) === false && options.stopOnFalse) {
-                        memory = false; // To prevent further calls using add
-                        break;
+            fire = function() {
+
+                // Enforce single-firing
+                locked = locked || options.once;
+
+                // Execute callbacks for all pending executions,
+                // respecting firingIndex overrides and runtime changes
+                fired = firing = true;
+                for (; queue.length; firingIndex = -1) {
+                    memory = queue.shift();
+                    while (++firingIndex < list.length) {
+
+                        // Run callback and check for early termination
+                        if (list[firingIndex].apply(memory[0], memory[1]) === false &&
+                            options.stopOnFalse) {
+
+                            // Jump to end and forget the data so .add doesn't re-fire
+                            firingIndex = list.length;
+                            memory = false;
+                        }
                     }
                 }
+
+                // Forget the data if we're done with it
+                if (!options.memory) {
+                    memory = false;
+                }
+
                 firing = false;
-                if (list) {
-                    if (stack) {
-                        if (stack.length) {
-                            fire(stack.shift());
-                        }
-                    } else if (memory) {
+
+                // Clean up if we're done firing for good
+                if (locked) {
+
+                    // Keep an empty list if we have data for future add calls
+                    if (memory) {
                         list = [];
+
+                        // Otherwise, this object is spent
                     } else {
-                        self.disable();
+                        list = "";
                     }
                 }
             },
+
             // Actual Callbacks object
             self = {
+
                 // Add a callback or a collection of callbacks to the list
                 add: function() {
                     if (list) {
-                        // First, we save the current length
-                        var start = list.length;
+
+                        // If we have memory from a past run, we should fire after adding
+                        if (memory && !firing) {
+                            firingIndex = list.length - 1;
+                            queue.push(memory);
+                        }
+
                         (function add(args) {
                             jQuery.each(args, function(_, arg) {
-                                var type = jQuery.type(arg);
-                                if (type === "function") {
+                                if (isFunction(arg)) {
                                     if (!options.unique || !self.has(arg)) {
                                         list.push(arg);
                                     }
-                                } else if (arg && arg.length && type !== "string") {
+                                } else if (arg && arg.length && toType(arg) !== "string") {
+
                                     // Inspect recursively
                                     add(arg);
                                 }
                             });
                         })(arguments);
-                        // Do we need to add the callbacks to the
-                        // current firing batch?
-                        if (firing) {
-                            firingLength = list.length;
-                            // With memory, if we're not firing then
-                            // we should call right away
-                        } else if (memory) {
-                            firingStart = start;
-                            fire(memory);
+
+                        if (memory && !firing) {
+                            fire();
                         }
                     }
                     return this;
                 },
+
                 // Remove a callback from the list
                 remove: function() {
-                    if (list) {
-                        jQuery.each(arguments, function(_, arg) {
-                            var index;
-                            while ((index = jQuery.inArray(arg, list, index)) > -1) {
-                                list.splice(index, 1);
-                                // Handle firing indexes
-                                if (firing) {
-                                    if (index <= firingLength) {
-                                        firingLength--;
-                                    }
-                                    if (index <= firingIndex) {
-                                        firingIndex--;
-                                    }
-                                }
+                    jQuery.each(arguments, function(_, arg) {
+                        var index;
+                        while ((index = jQuery.inArray(arg, list, index)) > -1) {
+                            list.splice(index, 1);
+
+                            // Handle firing indexes
+                            if (index <= firingIndex) {
+                                firingIndex--;
                             }
-                        });
-                    }
+                        }
+                    });
                     return this;
                 },
+
                 // Check if a given callback is in the list.
                 // If no argument is given, return whether or not list has callbacks attached.
                 has: function(fn) {
-                    return fn ? jQuery.inArray(fn, list) > -1 : !!(list && list.length);
+                    return fn ?
+                        jQuery.inArray(fn, list) > -1 :
+                        list.length > 0;
                 },
+
                 // Remove all callbacks from the list
                 empty: function() {
-                    list = [];
-                    firingLength = 0;
+                    if (list) {
+                        list = [];
+                    }
                     return this;
                 },
-                // Have the list do nothing anymore
+
+                // Disable .fire and .add
+                // Abort any current/pending executions
+                // Clear all callbacks and values
                 disable: function() {
-                    list = stack = memory = undefined;
+                    locked = queue = [];
+                    list = memory = "";
                     return this;
                 },
-                // Is it disabled?
                 disabled: function() {
                     return !list;
                 },
-                // Lock the list in its current state
+
+                // Disable .fire
+                // Also disable .add unless we have memory (since it would have no effect)
+                // Abort any pending executions
                 lock: function() {
-                    stack = undefined;
-                    if (!memory) {
-                        self.disable();
+                    locked = queue = [];
+                    if (!memory && !firing) {
+                        list = memory = "";
                     }
                     return this;
                 },
-                // Is it locked?
                 locked: function() {
-                    return !stack;
+                    return !!locked;
                 },
+
                 // Call all callbacks with the given context and arguments
                 fireWith: function(context, args) {
-                    if (list && (!fired || stack)) {
+                    if (!locked) {
                         args = args || [];
                         args = [context, args.slice ? args.slice() : args];
-                        if (firing) {
-                            stack.push(args);
-                        } else {
-                            fire(args);
+                        queue.push(args);
+                        if (!firing) {
+                            fire();
                         }
                     }
                     return this;
                 },
+
                 // Call all the callbacks with the given arguments
                 fire: function() {
                     self.fireWith(this, arguments);
                     return this;
                 },
+
                 // To know if the callbacks have already been called at least once
                 fired: function() {
                     return !!fired;
                 }
             };
 
         return self;
     };
 
 
+    function Identity(v) {
+        return v;
+    }
+
+    function Thrower(ex) {
+        throw ex;
+    }
+
+    function adoptValue(value, resolve, reject, noValue) {
+        var method;
+
+        try {
+
+            // Check for promise aspect first to privilege synchronous behavior
+            if (value && isFunction((method = value.promise))) {
+                method.call(value).done(resolve).fail(reject);
+
+                // Other thenables
+            } else if (value && isFunction((method = value.then))) {
+                method.call(value, resolve, reject);
+
+                // Other non-thenables
+            } else {
+
+                // Control `resolve` arguments by letting Array#slice cast boolean `noValue` to integer:
+                // * false: [ value ].slice( 0 ) => resolve( value )
+                // * true: [ value ].slice( 1 ) => resolve()
+                resolve.apply(undefined, [value].slice(noValue));
+            }
+
+            // For Promises/A+, convert exceptions into rejections
+            // Since jQuery.when doesn't unwrap thenables, we can skip the extra checks appearing in
+            // Deferred#then to conditionally suppress rejection.
+        } catch (value) {
+
+            // Support: Android 4.0 only
+            // Strict mode functions invoked without .call/.apply get global-object context
+            reject.apply(undefined, [value]);
+        }
+    }
+
     jQuery.extend({
 
         Deferred: function(func) {
             var tuples = [
-                    // action, add listener, listener list, final state
-                    ["resolve", "done", jQuery.Callbacks("once memory"), "resolved"],
-                    ["reject", "fail", jQuery.Callbacks("once memory"), "rejected"],
-                    ["notify", "progress", jQuery.Callbacks("memory")]
+
+                    // action, add listener, callbacks,
+                    // ... .then handlers, argument index, [final state]
+                    ["notify", "progress", jQuery.Callbacks("memory"),
+                        jQuery.Callbacks("memory"), 2
+                    ],
+                    ["resolve", "done", jQuery.Callbacks("once memory"),
+                        jQuery.Callbacks("once memory"), 0, "resolved"
+                    ],
+                    ["reject", "fail", jQuery.Callbacks("once memory"),
+                        jQuery.Callbacks("once memory"), 1, "rejected"
+                    ]
                 ],
                 state = "pending",
                 promise = {
                     state: function() {
                         return state;
                     },
                     always: function() {
                         deferred.done(arguments).fail(arguments);
                         return this;
                     },
-                    then: function( /* fnDone, fnFail, fnProgress */ ) {
+                    "catch": function(fn) {
+                        return promise.then(null, fn);
+                    },
+
+                    // Keep pipe for back-compat
+                    pipe: function( /* fnDone, fnFail, fnProgress */ ) {
                         var fns = arguments;
+
                         return jQuery.Deferred(function(newDefer) {
-                            jQuery.each(tuples, function(i, tuple) {
-                                var fn = jQuery.isFunction(fns[i]) && fns[i];
-                                // deferred[ done | fail | progress ] for forwarding actions to newDefer
+                            jQuery.each(tuples, function(_i, tuple) {
+
+                                // Map tuples (progress, done, fail) to arguments (done, fail, progress)
+                                var fn = isFunction(fns[tuple[4]]) && fns[tuple[4]];
+
+                                // deferred.progress(function() { bind to newDefer or newDefer.notify })
+                                // deferred.done(function() { bind to newDefer or newDefer.resolve })
+                                // deferred.fail(function() { bind to newDefer or newDefer.reject })
                                 deferred[tuple[1]](function() {
                                     var returned = fn && fn.apply(this, arguments);
-                                    if (returned && jQuery.isFunction(returned.promise)) {
+                                    if (returned && isFunction(returned.promise)) {
                                         returned.promise()
+                                            .progress(newDefer.notify)
                                             .done(newDefer.resolve)
-                                            .fail(newDefer.reject)
-                                            .progress(newDefer.notify);
+                                            .fail(newDefer.reject);
                                     } else {
-                                        newDefer[tuple[0] + "With"](this === promise ? newDefer.promise() : this, fn ? [returned] : arguments);
+                                        newDefer[tuple[0] + "With"](
+                                            this,
+                                            fn ? [returned] : arguments
+                                        );
                                     }
                                 });
                             });
                             fns = null;
                         }).promise();
                     },
+                    then: function(onFulfilled, onRejected, onProgress) {
+                        var maxDepth = 0;
+
+                        function resolve(depth, deferred, handler, special) {
+                            return function() {
+                                var that = this,
+                                    args = arguments,
+                                    mightThrow = function() {
+                                        var returned, then;
+
+                                        // Support: Promises/A+ section 2.3.3.3.3
+                                        // https://promisesaplus.com/#point-59
+                                        // Ignore double-resolution attempts
+                                        if (depth < maxDepth) {
+                                            return;
+                                        }
+
+                                        returned = handler.apply(that, args);
+
+                                        // Support: Promises/A+ section 2.3.1
+                                        // https://promisesaplus.com/#point-48
+                                        if (returned === deferred.promise()) {
+                                            throw new TypeError("Thenable self-resolution");
+                                        }
+
+                                        // Support: Promises/A+ sections 2.3.3.1, 3.5
+                                        // https://promisesaplus.com/#point-54
+                                        // https://promisesaplus.com/#point-75
+                                        // Retrieve `then` only once
+                                        then = returned &&
+
+                                            // Support: Promises/A+ section 2.3.4
+                                            // https://promisesaplus.com/#point-64
+                                            // Only check objects and functions for thenability
+                                            (typeof returned === "object" ||
+                                                typeof returned === "function") &&
+                                            returned.then;
+
+                                        // Handle a returned thenable
+                                        if (isFunction(then)) {
+
+                                            // Special processors (notify) just wait for resolution
+                                            if (special) {
+                                                then.call(
+                                                    returned,
+                                                    resolve(maxDepth, deferred, Identity, special),
+                                                    resolve(maxDepth, deferred, Thrower, special)
+                                                );
+
+                                                // Normal processors (resolve) also hook into progress
+                                            } else {
+
+                                                // ...and disregard older resolution values
+                                                maxDepth++;
+
+                                                then.call(
+                                                    returned,
+                                                    resolve(maxDepth, deferred, Identity, special),
+                                                    resolve(maxDepth, deferred, Thrower, special),
+                                                    resolve(maxDepth, deferred, Identity,
+                                                        deferred.notifyWith)
+                                                );
+                                            }
+
+                                            // Handle all other returned values
+                                        } else {
+
+                                            // Only substitute handlers pass on context
+                                            // and multiple values (non-spec behavior)
+                                            if (handler !== Identity) {
+                                                that = undefined;
+                                                args = [returned];
+                                            }
+
+                                            // Process the value(s)
+                                            // Default process is resolve
+                                            (special || deferred.resolveWith)(that, args);
+                                        }
+                                    },
+
+                                    // Only normal processors (resolve) catch and reject exceptions
+                                    process = special ?
+                                    mightThrow :
+                                    function() {
+                                        try {
+                                            mightThrow();
+                                        } catch (e) {
+
+                                            if (jQuery.Deferred.exceptionHook) {
+                                                jQuery.Deferred.exceptionHook(e,
+                                                    process.stackTrace);
+                                            }
+
+                                            // Support: Promises/A+ section 2.3.3.3.4.1
+                                            // https://promisesaplus.com/#point-61
+                                            // Ignore post-resolution exceptions
+                                            if (depth + 1 >= maxDepth) {
+
+                                                // Only substitute handlers pass on context
+                                                // and multiple values (non-spec behavior)
+                                                if (handler !== Thrower) {
+                                                    that = undefined;
+                                                    args = [e];
+                                                }
+
+                                                deferred.rejectWith(that, args);
+                                            }
+                                        }
+                                    };
+
+                                // Support: Promises/A+ section 2.3.3.3.1
+                                // https://promisesaplus.com/#point-57
+                                // Re-resolve promises immediately to dodge false rejection from
+                                // subsequent errors
+                                if (depth) {
+                                    process();
+                                } else {
+
+                                    // Call an optional hook to record the stack, in case of exception
+                                    // since it's otherwise lost when execution goes async
+                                    if (jQuery.Deferred.getStackHook) {
+                                        process.stackTrace = jQuery.Deferred.getStackHook();
+                                    }
+                                    window.setTimeout(process);
+                                }
+                            };
+                        }
+
+                        return jQuery.Deferred(function(newDefer) {
+
+                            // progress_handlers.add( ... )
+                            tuples[0][3].add(
+                                resolve(
+                                    0,
+                                    newDefer,
+                                    isFunction(onProgress) ?
+                                    onProgress :
+                                    Identity,
+                                    newDefer.notifyWith
+                                )
+                            );
+
+                            // fulfilled_handlers.add( ... )
+                            tuples[1][3].add(
+                                resolve(
+                                    0,
+                                    newDefer,
+                                    isFunction(onFulfilled) ?
+                                    onFulfilled :
+                                    Identity
+                                )
+                            );
+
+                            // rejected_handlers.add( ... )
+                            tuples[2][3].add(
+                                resolve(
+                                    0,
+                                    newDefer,
+                                    isFunction(onRejected) ?
+                                    onRejected :
+                                    Thrower
+                                )
+                            );
+                        }).promise();
+                    },
+
                     // Get a promise for this deferred
                     // If obj is provided, the promise aspect is added to the object
                     promise: function(obj) {
                         return obj != null ? jQuery.extend(obj, promise) : promise;
                     }
                 },
                 deferred = {};
 
-            // Keep pipe for back-compat
-            promise.pipe = promise.then;
-
             // Add list-specific methods
             jQuery.each(tuples, function(i, tuple) {
                 var list = tuple[2],
-                    stateString = tuple[3];
+                    stateString = tuple[5];
 
-                // promise[ done | fail | progress ] = list.add
+                // promise.progress = list.add
+                // promise.done = list.add
+                // promise.fail = list.add
                 promise[tuple[1]] = list.add;
 
                 // Handle state
                 if (stateString) {
-                    list.add(function() {
-                        // state = [ resolved | rejected ]
-                        state = stateString;
+                    list.add(
+                        function() {
+
+                            // state = "resolved" (i.e., fulfilled)
+                            // state = "rejected"
+                            state = stateString;
+                        },
+
+                        // rejected_callbacks.disable
+                        // fulfilled_callbacks.disable
+                        tuples[3 - i][2].disable,
+
+                        // rejected_handlers.disable
+                        // fulfilled_handlers.disable
+                        tuples[3 - i][3].disable,
 
-                        // [ reject_list | resolve_list ].disable; progress_list.lock
-                    }, tuples[i ^ 1][2].disable, tuples[2][2].lock);
+                        // progress_callbacks.lock
+                        tuples[0][2].lock,
+
+                        // progress_handlers.lock
+                        tuples[0][3].lock
+                    );
                 }
 
-                // deferred[ resolve | reject | notify ]
+                // progress_handlers.fire
+                // fulfilled_handlers.fire
+                // rejected_handlers.fire
+                list.add(tuple[3].fire);
+
+                // deferred.notify = function() { deferred.notifyWith(...) }
+                // deferred.resolve = function() { deferred.resolveWith(...) }
+                // deferred.reject = function() { deferred.rejectWith(...) }
                 deferred[tuple[0]] = function() {
-                    deferred[tuple[0] + "With"](this === deferred ? promise : this, arguments);
+                    deferred[tuple[0] + "With"](this === deferred ? undefined : this, arguments);
                     return this;
                 };
+
+                // deferred.notifyWith = list.fireWith
+                // deferred.resolveWith = list.fireWith
+                // deferred.rejectWith = list.fireWith
                 deferred[tuple[0] + "With"] = list.fireWith;
             });
 
             // Make the deferred a promise
             promise.promise(deferred);
 
             // Call given func if any
@@ -3355,645 +4013,595 @@
             }
 
             // All done!
             return deferred;
         },
 
         // Deferred helper
-        when: function(subordinate /* , ..., subordinateN */ ) {
-            var i = 0,
-                resolveValues = slice.call(arguments),
-                length = resolveValues.length,
+        when: function(singleValue) {
+            var
 
-                // the count of uncompleted subordinates
-                remaining = length !== 1 || (subordinate && jQuery.isFunction(subordinate.promise)) ? length : 0,
+                // count of uncompleted subordinates
+                remaining = arguments.length,
 
-                // the master Deferred. If resolveValues consist of only a single Deferred, just use that.
-                deferred = remaining === 1 ? subordinate : jQuery.Deferred(),
+                // count of unprocessed arguments
+                i = remaining,
 
-                // Update function for both resolve and progress values
-                updateFunc = function(i, contexts, values) {
-                    return function(value) {
-                        contexts[i] = this;
-                        values[i] = arguments.length > 1 ? slice.call(arguments) : value;
-                        if (values === progressValues) {
-                            deferred.notifyWith(contexts, values);
+                // subordinate fulfillment data
+                resolveContexts = Array(i),
+                resolveValues = slice.call(arguments),
 
-                        } else if (!(--remaining)) {
-                            deferred.resolveWith(contexts, values);
+                // the primary Deferred
+                primary = jQuery.Deferred(),
+
+                // subordinate callback factory
+                updateFunc = function(i) {
+                    return function(value) {
+                        resolveContexts[i] = this;
+                        resolveValues[i] = arguments.length > 1 ? slice.call(arguments) : value;
+                        if (!(--remaining)) {
+                            primary.resolveWith(resolveContexts, resolveValues);
                         }
                     };
-                },
+                };
 
-                progressValues, progressContexts, resolveContexts;
+            // Single- and empty arguments are adopted like Promise.resolve
+            if (remaining <= 1) {
+                adoptValue(singleValue, primary.done(updateFunc(i)).resolve, primary.reject,
+                    !remaining);
 
-            // add listeners to Deferred subordinates; treat others as resolved
-            if (length > 1) {
-                progressValues = new Array(length);
-                progressContexts = new Array(length);
-                resolveContexts = new Array(length);
-                for (; i < length; i++) {
-                    if (resolveValues[i] && jQuery.isFunction(resolveValues[i].promise)) {
-                        resolveValues[i].promise()
-                            .done(updateFunc(i, resolveContexts, resolveValues))
-                            .fail(deferred.reject)
-                            .progress(updateFunc(i, progressContexts, progressValues));
-                    } else {
-                        --remaining;
-                    }
+                // Use .then() to unwrap secondary thenables (cf. gh-3000)
+                if (primary.state() === "pending" ||
+                    isFunction(resolveValues[i] && resolveValues[i].then)) {
+
+                    return primary.then();
                 }
             }
 
-            // if we're not waiting on anything, resolve the master
-            if (!remaining) {
-                deferred.resolveWith(resolveContexts, resolveValues);
+            // Multiple arguments are aggregated like Promise.all array elements
+            while (i--) {
+                adoptValue(resolveValues[i], updateFunc(i), primary.reject);
             }
 
-            return deferred.promise();
+            return primary.promise();
         }
     });
 
 
+    // These usually indicate a programmer mistake during development,
+    // warn about them ASAP rather than swallowing them by default.
+    var rerrorNames = /^(Eval|Internal|Range|Reference|Syntax|Type|URI)Error$/;
+
+    jQuery.Deferred.exceptionHook = function(error, stack) {
+
+        // Support: IE 8 - 9 only
+        // Console exists when dev tools are open, which can happen at any time
+        if (window.console && window.console.warn && error && rerrorNames.test(error.name)) {
+            window.console.warn("jQuery.Deferred exception: " + error.message, error.stack, stack);
+        }
+    };
+
+
+
+
+    jQuery.readyException = function(error) {
+        window.setTimeout(function() {
+            throw error;
+        });
+    };
+
+
+
+
     // The deferred used on DOM ready
-    var readyList;
+    var readyList = jQuery.Deferred();
 
     jQuery.fn.ready = function(fn) {
-        // Add the callback
-        jQuery.ready.promise().done(fn);
+
+        readyList
+            .then(fn)
+
+            // Wrap jQuery.readyException in a function so that the lookup
+            // happens at the time of error handling instead of callback
+            // registration.
+            .catch(function(error) {
+                jQuery.readyException(error);
+            });
 
         return this;
     };
 
     jQuery.extend({
+
         // Is the DOM ready to be used? Set to true once it occurs.
         isReady: false,
 
         // A counter to track how many items to wait for before
-        // the ready event fires. See #6781
+        // the ready event fires. See trac-6781
         readyWait: 1,
 
-        // Hold (or release) the ready event
-        holdReady: function(hold) {
-            if (hold) {
-                jQuery.readyWait++;
-            } else {
-                jQuery.ready(true);
-            }
-        },
-
         // Handle when the DOM is ready
         ready: function(wait) {
 
             // Abort if there are pending holds or we're already ready
             if (wait === true ? --jQuery.readyWait : jQuery.isReady) {
                 return;
             }
 
-            // Make sure body exists, at least, in case IE gets a little overzealous (ticket #5443).
-            if (!document.body) {
-                return setTimeout(jQuery.ready);
-            }
-
             // Remember that the DOM is ready
             jQuery.isReady = true;
 
             // If a normal DOM Ready event fired, decrement, and wait if need be
             if (wait !== true && --jQuery.readyWait > 0) {
                 return;
             }
 
             // If there are functions bound, to execute
             readyList.resolveWith(document, [jQuery]);
-
-            // Trigger any bound ready events
-            if (jQuery.fn.triggerHandler) {
-                jQuery(document).triggerHandler("ready");
-                jQuery(document).off("ready");
-            }
         }
     });
 
-    /**
-     * Clean-up method for dom ready events
-     */
-    function detach() {
-        if (document.addEventListener) {
-            document.removeEventListener("DOMContentLoaded", completed, false);
-            window.removeEventListener("load", completed, false);
-
-        } else {
-            document.detachEvent("onreadystatechange", completed);
-            window.detachEvent("onload", completed);
-        }
-    }
+    jQuery.ready.then = readyList.then;
 
-    /**
-     * The ready event handler and self cleanup method
-     */
+    // The ready event handler and self cleanup method
     function completed() {
-        // readyState === "complete" is good enough for us to call the dom ready in oldIE
-        if (document.addEventListener || event.type === "load" || document.readyState === "complete") {
-            detach();
-            jQuery.ready();
-        }
+        document.removeEventListener("DOMContentLoaded", completed);
+        window.removeEventListener("load", completed);
+        jQuery.ready();
     }
 
-    jQuery.ready.promise = function(obj) {
-        if (!readyList) {
-
-            readyList = jQuery.Deferred();
-
-            // Catch cases where $(document).ready() is called after the browser event has already occurred.
-            // we once tried to use readyState "interactive" here, but it caused issues like the one
-            // discovered by ChrisS here: http://bugs.jquery.com/ticket/12282#comment:15
-            if (document.readyState === "complete") {
-                // Handle it asynchronously to allow scripts the opportunity to delay ready
-                setTimeout(jQuery.ready);
-
-                // Standards-based browsers support DOMContentLoaded
-            } else if (document.addEventListener) {
-                // Use the handy event callback
-                document.addEventListener("DOMContentLoaded", completed, false);
+    // Catch cases where $(document).ready() is called
+    // after the browser event has already occurred.
+    // Support: IE <=9 - 10 only
+    // Older IE sometimes signals "interactive" too soon
+    if (document.readyState === "complete" ||
+        (document.readyState !== "loading" && !document.documentElement.doScroll)) {
 
-                // A fallback to window.onload, that will always work
-                window.addEventListener("load", completed, false);
+        // Handle it asynchronously to allow scripts the opportunity to delay ready
+        window.setTimeout(jQuery.ready);
 
-                // If IE event model is used
-            } else {
-                // Ensure firing before onload, maybe late but safe also for iframes
-                document.attachEvent("onreadystatechange", completed);
+    } else {
 
-                // A fallback to window.onload, that will always work
-                window.attachEvent("onload", completed);
+        // Use the handy event callback
+        document.addEventListener("DOMContentLoaded", completed);
 
-                // If IE and not a frame
-                // continually check to see if the document is ready
-                var top = false;
+        // A fallback to window.onload, that will always work
+        window.addEventListener("load", completed);
+    }
 
-                try {
-                    top = window.frameElement == null && document.documentElement;
-                } catch (e) {}
 
-                if (top && top.doScroll) {
-                    (function doScrollCheck() {
-                        if (!jQuery.isReady) {
 
-                            try {
-                                // Use the trick by Diego Perini
-                                // http://javascript.nwbox.com/IEContentLoaded/
-                                top.doScroll("left");
-                            } catch (e) {
-                                return setTimeout(doScrollCheck, 50);
-                            }
 
-                            // detach all dom ready events
-                            detach();
+    // Multifunctional method to get and set values of a collection
+    // The value/s can optionally be executed if it's a function
+    var access = function(elems, fn, key, value, chainable, emptyGet, raw) {
+        var i = 0,
+            len = elems.length,
+            bulk = key == null;
 
-                            // and execute any waiting functions
-                            jQuery.ready();
-                        }
-                    })();
-                }
+        // Sets many values
+        if (toType(key) === "object") {
+            chainable = true;
+            for (i in key) {
+                access(elems, fn, i, key[i], true, emptyGet, raw);
             }
-        }
-        return readyList.promise(obj);
-    };
-
-
-    var strundefined = typeof undefined;
 
+            // Sets one value
+        } else if (value !== undefined) {
+            chainable = true;
 
+            if (!isFunction(value)) {
+                raw = true;
+            }
 
-    // Support: IE<9
-    // Iteration over object's inherited properties before its own
-    var i;
-    for (i in jQuery(support)) {
-        break;
-    }
-    support.ownLast = i !== "0";
+            if (bulk) {
 
-    // Note: most support tests are defined in their respective modules.
-    // false until the test is run
-    support.inlineBlockNeedsLayout = false;
+                // Bulk operations run against the entire set
+                if (raw) {
+                    fn.call(elems, value);
+                    fn = null;
 
-    // Execute ASAP in case we need to set body.style.zoom
-    jQuery(function() {
-        // Minified: var a,b,c,d
-        var val, div, body, container;
+                    // ...except when executing function values
+                } else {
+                    bulk = fn;
+                    fn = function(elem, _key, value) {
+                        return bulk.call(jQuery(elem), value);
+                    };
+                }
+            }
 
-        body = document.getElementsByTagName("body")[0];
-        if (!body || !body.style) {
-            // Return for frameset docs that don't have a body
-            return;
+            if (fn) {
+                for (; i < len; i++) {
+                    fn(
+                        elems[i], key, raw ?
+                        value :
+                        value.call(elems[i], i, fn(elems[i], key))
+                    );
+                }
+            }
         }
 
-        // Setup
-        div = document.createElement("div");
-        container = document.createElement("div");
-        container.style.cssText = "position:absolute;border:0;width:0;height:0;top:0;left:-9999px";
-        body.appendChild(container).appendChild(div);
+        if (chainable) {
+            return elems;
+        }
 
-        if (typeof div.style.zoom !== strundefined) {
-            // Support: IE<8
-            // Check if natively block-level elements act like inline-block
-            // elements when setting their display to 'inline' and giving
-            // them layout
-            div.style.cssText = "display:inline;margin:0;border:0;padding:1px;width:1px;zoom:1";
-
-            support.inlineBlockNeedsLayout = val = div.offsetWidth === 3;
-            if (val) {
-                // Prevent IE 6 from affecting layout for positioned elements #11048
-                // Prevent IE from shrinking the body in IE 7 mode #12869
-                // Support: IE<8
-                body.style.zoom = 1;
-            }
+        // Gets
+        if (bulk) {
+            return fn.call(elems);
         }
 
-        body.removeChild(container);
-    });
+        return len ? fn(elems[0], key) : emptyGet;
+    };
 
 
+    // Matches dashed string for camelizing
+    var rmsPrefix = /^-ms-/,
+        rdashAlpha = /-([a-z])/g;
+
+    // Used by camelCase as callback to replace()
+    function fcamelCase(_all, letter) {
+        return letter.toUpperCase();
+    }
+
+    // Convert dashed to camelCase; used by the css and data modules
+    // Support: IE <=9 - 11, Edge 12 - 15
+    // Microsoft forgot to hump their vendor prefix (trac-9572)
+    function camelCase(string) {
+        return string.replace(rmsPrefix, "ms-").replace(rdashAlpha, fcamelCase);
+    }
+    var acceptData = function(owner) {
+
+        // Accepts only:
+        //  - Node
+        //    - Node.ELEMENT_NODE
+        //    - Node.DOCUMENT_NODE
+        //  - Object
+        //    - Any
+        return owner.nodeType === 1 || owner.nodeType === 9 || !(+owner.nodeType);
+    };
 
 
-    (function() {
-        var div = document.createElement("div");
 
-        // Execute the test only if not already executed in another module.
-        if (support.deleteExpando == null) {
-            // Support: IE<9
-            support.deleteExpando = true;
-            try {
-                delete div.test;
-            } catch (e) {
-                support.deleteExpando = false;
-            }
-        }
 
-        // Null elements to avoid leaks in IE.
-        div = null;
-    })();
+    function Data() {
+        this.expando = jQuery.expando + Data.uid++;
+    }
 
+    Data.uid = 1;
 
-    /**
-     * Determines whether an object can have data
-     */
-    jQuery.acceptData = function(elem) {
-        var noData = jQuery.noData[(elem.nodeName + " ").toLowerCase()],
-            nodeType = +elem.nodeType || 1;
-
-        // Do not set data on non-element DOM nodes because it will not be cleared (#8335).
-        return nodeType !== 1 && nodeType !== 9 ?
-            false :
+    Data.prototype = {
 
-            // Nodes accept data unless otherwise specified; rejection can be conditional
-            !noData || noData !== true && elem.getAttribute("classid") === noData;
-    };
+        cache: function(owner) {
 
+            // Check if the owner object already has a cache
+            var value = owner[this.expando];
 
-    var rbrace = /^(?:\{[\w\W]*\}|\[[\w\W]*\])$/,
-        rmultiDash = /([A-Z])/g;
+            // If not, create one
+            if (!value) {
+                value = {};
 
-    function dataAttr(elem, key, data) {
-        // If nothing was found internally, try to fetch any
-        // data from the HTML5 data-* attribute
-        if (data === undefined && elem.nodeType === 1) {
+                // We can accept data for non-element nodes in modern browsers,
+                // but we should not, see trac-8335.
+                // Always return an empty object.
+                if (acceptData(owner)) {
 
-            var name = "data-" + key.replace(rmultiDash, "-$1").toLowerCase();
+                    // If it is a node unlikely to be stringify-ed or looped over
+                    // use plain assignment
+                    if (owner.nodeType) {
+                        owner[this.expando] = value;
 
-            data = elem.getAttribute(name);
+                        // Otherwise secure it in a non-enumerable property
+                        // configurable must be true to allow the property to be
+                        // deleted when data is removed
+                    } else {
+                        Object.defineProperty(owner, this.expando, {
+                            value: value,
+                            configurable: true
+                        });
+                    }
+                }
+            }
 
-            if (typeof data === "string") {
-                try {
-                    data = data === "true" ? true :
-                        data === "false" ? false :
-                        data === "null" ? null :
-                        // Only convert to a number if it doesn't change the string
-                        +data + "" === data ? +data :
-                        rbrace.test(data) ? jQuery.parseJSON(data) :
-                        data;
-                } catch (e) {}
+            return value;
+        },
+        set: function(owner, data, value) {
+            var prop,
+                cache = this.cache(owner);
 
-                // Make sure we set the data so it isn't changed later
-                jQuery.data(elem, key, data);
+            // Handle: [ owner, key, value ] args
+            // Always use camelCase key (gh-2257)
+            if (typeof data === "string") {
+                cache[camelCase(data)] = value;
 
+                // Handle: [ owner, { properties } ] args
             } else {
-                data = undefined;
-            }
-        }
-
-        return data;
-    }
 
-    // checks a cache object for emptiness
-    function isEmptyDataObject(obj) {
-        var name;
-        for (name in obj) {
+                // Copy the properties one-by-one to the cache object
+                for (prop in data) {
+                    cache[camelCase(prop)] = data[prop];
+                }
+            }
+            return cache;
+        },
+        get: function(owner, key) {
+            return key === undefined ?
+                this.cache(owner) :
+
+                // Always use camelCase key (gh-2257)
+                owner[this.expando] && owner[this.expando][camelCase(key)];
+        },
+        access: function(owner, key, value) {
+
+            // In cases where either:
+            //
+            //   1. No key was specified
+            //   2. A string key was specified, but no value provided
+            //
+            // Take the "read" path and allow the get method to determine
+            // which value to return, respectively either:
+            //
+            //   1. The entire cache object
+            //   2. The data stored at the key
+            //
+            if (key === undefined ||
+                ((key && typeof key === "string") && value === undefined)) {
+
+                return this.get(owner, key);
+            }
+
+            // When the key is not a string, or both a key and value
+            // are specified, set or extend (existing objects) with either:
+            //
+            //   1. An object of properties
+            //   2. A key and value
+            //
+            this.set(owner, key, value);
+
+            // Since the "set" path can have two possible entry points
+            // return the expected data based on which path was taken[*]
+            return value !== undefined ? value : key;
+        },
+        remove: function(owner, key) {
+            var i,
+                cache = owner[this.expando];
 
-            // if the public data object is empty, the private is still empty
-            if (name === "data" && jQuery.isEmptyObject(obj[name])) {
-                continue;
-            }
-            if (name !== "toJSON") {
-                return false;
+            if (cache === undefined) {
+                return;
             }
-        }
-
-        return true;
-    }
 
-    function internalData(elem, name, data, pvt /* Internal Use Only */ ) {
-        if (!jQuery.acceptData(elem)) {
-            return;
-        }
+            if (key !== undefined) {
 
-        var ret, thisCache,
-            internalKey = jQuery.expando,
+                // Support array or space separated string of keys
+                if (Array.isArray(key)) {
 
-            // We have to handle DOM nodes and JS objects differently because IE6-7
-            // can't GC object references properly across the DOM-JS boundary
-            isNode = elem.nodeType,
-
-            // Only DOM nodes need the global jQuery cache; JS object data is
-            // attached directly to the object so GC can occur automatically
-            cache = isNode ? jQuery.cache : elem,
-
-            // Only defining an ID for JS objects if its cache already exists allows
-            // the code to shortcut on the same path as a DOM node with no cache
-            id = isNode ? elem[internalKey] : elem[internalKey] && internalKey;
-
-        // Avoid doing any more work than we need to when trying to get data on an
-        // object that has no data at all
-        if ((!id || !cache[id] || (!pvt && !cache[id].data)) && data === undefined && typeof name === "string") {
-            return;
-        }
+                    // If key is an array of keys...
+                    // We always set camelCase keys, so remove that.
+                    key = key.map(camelCase);
+                } else {
+                    key = camelCase(key);
 
-        if (!id) {
-            // Only DOM nodes need a new unique ID for each element since their data
-            // ends up in the global cache
-            if (isNode) {
-                id = elem[internalKey] = deletedIds.pop() || jQuery.guid++;
-            } else {
-                id = internalKey;
-            }
-        }
+                    // If a key with the spaces exists, use it.
+                    // Otherwise, create an array by matching non-whitespace
+                    key = key in cache ? [key] :
+                        (key.match(rnothtmlwhite) || []);
+                }
 
-        if (!cache[id]) {
-            // Avoid exposing jQuery metadata on plain JS objects when the object
-            // is serialized using JSON.stringify
-            cache[id] = isNode ? {} : {
-                toJSON: jQuery.noop
-            };
-        }
+                i = key.length;
 
-        // An object can be passed to jQuery.data instead of a key/value pair; this gets
-        // shallow copied over onto the existing cache
-        if (typeof name === "object" || typeof name === "function") {
-            if (pvt) {
-                cache[id] = jQuery.extend(cache[id], name);
-            } else {
-                cache[id].data = jQuery.extend(cache[id].data, name);
+                while (i--) {
+                    delete cache[key[i]];
+                }
             }
-        }
 
-        thisCache = cache[id];
+            // Remove the expando if there's no more data
+            if (key === undefined || jQuery.isEmptyObject(cache)) {
 
-        // jQuery data() is stored in a separate object inside the object's internal data
-        // cache in order to avoid key collisions between internal data and user-defined
-        // data.
-        if (!pvt) {
-            if (!thisCache.data) {
-                thisCache.data = {};
+                // Support: Chrome <=35 - 45
+                // Webkit & Blink performance suffers when deleting properties
+                // from DOM nodes, so set to undefined instead
+                // https://bugs.chromium.org/p/chromium/issues/detail?id=378607 (bug restricted)
+                if (owner.nodeType) {
+                    owner[this.expando] = undefined;
+                } else {
+                    delete owner[this.expando];
+                }
             }
-
-            thisCache = thisCache.data;
-        }
-
-        if (data !== undefined) {
-            thisCache[jQuery.camelCase(name)] = data;
+        },
+        hasData: function(owner) {
+            var cache = owner[this.expando];
+            return cache !== undefined && !jQuery.isEmptyObject(cache);
         }
+    };
+    var dataPriv = new Data();
 
-        // Check for both converted-to-camel and non-converted data property names
-        // If a data property was specified
-        if (typeof name === "string") {
+    var dataUser = new Data();
 
-            // First Try to find as-is property data
-            ret = thisCache[name];
 
-            // Test for null|undefined property data
-            if (ret == null) {
 
-                // Try to find the camelCased property
-                ret = thisCache[jQuery.camelCase(name)];
-            }
-        } else {
-            ret = thisCache;
-        }
+    //	Implementation Summary
+    //
+    //	1. Enforce API surface and semantic compatibility with 1.9.x branch
+    //	2. Improve the module's maintainability by reducing the storage
+    //		paths to a single mechanism.
+    //	3. Use the same single mechanism to support "private" and "user" data.
+    //	4. _Never_ expose "private" data to user code (TODO: Drop _data, _removeData)
+    //	5. Avoid exposing implementation details on user objects (eg. expando properties)
+    //	6. Provide a clear path for implementation upgrade to WeakMap in 2014
 
-        return ret;
-    }
+    var rbrace = /^(?:\{[\w\W]*\}|\[[\w\W]*\])$/,
+        rmultiDash = /[A-Z]/g;
 
-    function internalRemoveData(elem, name, pvt) {
-        if (!jQuery.acceptData(elem)) {
-            return;
+    function getData(data) {
+        if (data === "true") {
+            return true;
         }
 
-        var thisCache, i,
-            isNode = elem.nodeType,
-
-            // See jQuery.data for more information
-            cache = isNode ? jQuery.cache : elem,
-            id = isNode ? elem[jQuery.expando] : jQuery.expando;
-
-        // If there is already no cache entry for this object, there is no
-        // purpose in continuing
-        if (!cache[id]) {
-            return;
+        if (data === "false") {
+            return false;
         }
 
-        if (name) {
-
-            thisCache = pvt ? cache[id] : cache[id].data;
+        if (data === "null") {
+            return null;
+        }
 
-            if (thisCache) {
+        // Only convert to a number if it doesn't change the string
+        if (data === +data + "") {
+            return +data;
+        }
 
-                // Support array or space separated string names for data keys
-                if (!jQuery.isArray(name)) {
+        if (rbrace.test(data)) {
+            return JSON.parse(data);
+        }
 
-                    // try the string as a key before any manipulation
-                    if (name in thisCache) {
-                        name = [name];
-                    } else {
+        return data;
+    }
 
-                        // split the camel cased version by spaces unless a key with the spaces exists
-                        name = jQuery.camelCase(name);
-                        if (name in thisCache) {
-                            name = [name];
-                        } else {
-                            name = name.split(" ");
-                        }
-                    }
-                } else {
-                    // If "name" is an array of keys...
-                    // When data is initially created, via ("key", "val") signature,
-                    // keys will be converted to camelCase.
-                    // Since there is no way to tell _how_ a key was added, remove
-                    // both plain key and camelCase key. #12786
-                    // This will only penalize the array argument path.
-                    name = name.concat(jQuery.map(name, jQuery.camelCase));
-                }
+    function dataAttr(elem, key, data) {
+        var name;
 
-                i = name.length;
-                while (i--) {
-                    delete thisCache[name[i]];
-                }
+        // If nothing was found internally, try to fetch any
+        // data from the HTML5 data-* attribute
+        if (data === undefined && elem.nodeType === 1) {
+            name = "data-" + key.replace(rmultiDash, "-$&").toLowerCase();
+            data = elem.getAttribute(name);
 
-                // If there is no data left in the cache, we want to continue
-                // and let the cache object itself get destroyed
-                if (pvt ? !isEmptyDataObject(thisCache) : !jQuery.isEmptyObject(thisCache)) {
-                    return;
-                }
-            }
-        }
+            if (typeof data === "string") {
+                try {
+                    data = getData(data);
+                } catch (e) {}
 
-        // See jQuery.data for more information
-        if (!pvt) {
-            delete cache[id].data;
-
-            // Don't destroy the parent cache unless the internal data object
-            // had been the only thing left in it
-            if (!isEmptyDataObject(cache[id])) {
-                return;
+                // Make sure we set the data so it isn't changed later
+                dataUser.set(elem, key, data);
+            } else {
+                data = undefined;
             }
         }
-
-        // Destroy the cache
-        if (isNode) {
-            jQuery.cleanData([elem], true);
-
-            // Use delete when supported for expandos or `cache` is not a window per isWindow (#10080)
-            /* jshint eqeqeq: false */
-        } else if (support.deleteExpando || cache != cache.window) {
-            /* jshint eqeqeq: true */
-            delete cache[id];
-
-            // When all else fails, null
-        } else {
-            cache[id] = null;
-        }
+        return data;
     }
 
     jQuery.extend({
-        cache: {},
-
-        // The following elements (space-suffixed to avoid Object.prototype collisions)
-        // throw uncatchable exceptions if you attempt to set expando properties
-        noData: {
-            "applet ": true,
-            "embed ": true,
-            // ...but Flash objects (which have this classid) *can* handle expandos
-            "object ": "clsid:D27CDB6E-AE6D-11cf-96B8-444553540000"
-        },
-
         hasData: function(elem) {
-            elem = elem.nodeType ? jQuery.cache[elem[jQuery.expando]] : elem[jQuery.expando];
-            return !!elem && !isEmptyDataObject(elem);
+            return dataUser.hasData(elem) || dataPriv.hasData(elem);
         },
 
         data: function(elem, name, data) {
-            return internalData(elem, name, data);
+            return dataUser.access(elem, name, data);
         },
 
         removeData: function(elem, name) {
-            return internalRemoveData(elem, name);
+            dataUser.remove(elem, name);
         },
 
-        // For internal use only.
+        // TODO: Now that all calls to _data and _removeData have been replaced
+        // with direct calls to dataPriv methods, these can be deprecated.
         _data: function(elem, name, data) {
-            return internalData(elem, name, data, true);
+            return dataPriv.access(elem, name, data);
         },
 
         _removeData: function(elem, name) {
-            return internalRemoveData(elem, name, true);
+            dataPriv.remove(elem, name);
         }
     });
 
     jQuery.fn.extend({
         data: function(key, value) {
             var i, name, data,
                 elem = this[0],
                 attrs = elem && elem.attributes;
 
-            // Special expections of .data basically thwart jQuery.access,
-            // so implement the relevant behavior ourselves
-
             // Gets all values
             if (key === undefined) {
                 if (this.length) {
-                    data = jQuery.data(elem);
+                    data = dataUser.get(elem);
 
-                    if (elem.nodeType === 1 && !jQuery._data(elem, "parsedAttrs")) {
+                    if (elem.nodeType === 1 && !dataPriv.get(elem, "hasDataAttrs")) {
                         i = attrs.length;
                         while (i--) {
 
-                            // Support: IE11+
-                            // The attrs elements can be null (#14894)
+                            // Support: IE 11 only
+                            // The attrs elements can be null (trac-14894)
                             if (attrs[i]) {
                                 name = attrs[i].name;
                                 if (name.indexOf("data-") === 0) {
-                                    name = jQuery.camelCase(name.slice(5));
+                                    name = camelCase(name.slice(5));
                                     dataAttr(elem, name, data[name]);
                                 }
                             }
                         }
-                        jQuery._data(elem, "parsedAttrs", true);
+                        dataPriv.set(elem, "hasDataAttrs", true);
                     }
                 }
 
                 return data;
             }
 
             // Sets multiple values
             if (typeof key === "object") {
                 return this.each(function() {
-                    jQuery.data(this, key);
+                    dataUser.set(this, key);
                 });
             }
 
-            return arguments.length > 1 ?
+            return access(this, function(value) {
+                var data;
+
+                // The calling jQuery object (element matches) is not empty
+                // (and therefore has an element appears at this[ 0 ]) and the
+                // `value` parameter was not undefined. An empty jQuery object
+                // will result in `undefined` for elem = this[ 0 ] which will
+                // throw an exception if an attempt to read a data cache is made.
+                if (elem && value === undefined) {
+
+                    // Attempt to get data from the cache
+                    // The key will always be camelCased in Data
+                    data = dataUser.get(elem, key);
+                    if (data !== undefined) {
+                        return data;
+                    }
+
+                    // Attempt to "discover" the data in
+                    // HTML5 custom data-* attrs
+                    data = dataAttr(elem, key);
+                    if (data !== undefined) {
+                        return data;
+                    }
+
+                    // We tried really hard, but the data doesn't exist.
+                    return;
+                }
 
-                // Sets one value
+                // Set the data...
                 this.each(function() {
-                    jQuery.data(this, key, value);
-                }) :
 
-                // Gets one value
-                // Try to fetch any internally stored data first
-                elem ? dataAttr(elem, key, jQuery.data(elem, key)) : undefined;
+                    // We always store the camelCased key
+                    dataUser.set(this, key, value);
+                });
+            }, null, value, arguments.length > 1, null, true);
         },
 
         removeData: function(key) {
             return this.each(function() {
-                jQuery.removeData(this, key);
+                dataUser.remove(this, key);
             });
         }
     });
 
 
     jQuery.extend({
         queue: function(elem, type, data) {
             var queue;
 
             if (elem) {
                 type = (type || "fx") + "queue";
-                queue = jQuery._data(elem, type);
+                queue = dataPriv.get(elem, type);
 
                 // Speed up dequeue by getting out quickly if this is just a lookup
                 if (data) {
-                    if (!queue || jQuery.isArray(data)) {
-                        queue = jQuery._data(elem, type, jQuery.makeArray(data));
+                    if (!queue || Array.isArray(data)) {
+                        queue = dataPriv.access(elem, type, jQuery.makeArray(data));
                     } else {
                         queue.push(data);
                     }
                 }
                 return queue || [];
             }
         },
@@ -4019,31 +4627,30 @@
 
                 // Add a progress sentinel to prevent the fx queue from being
                 // automatically dequeued
                 if (type === "fx") {
                     queue.unshift("inprogress");
                 }
 
-                // clear up the last queue stop function
+                // Clear up the last queue stop function
                 delete hooks.stop;
                 fn.call(elem, next, hooks);
             }
 
             if (!startLength && hooks) {
                 hooks.empty.fire();
             }
         },
 
-        // not intended for public consumption - generates a queueHooks object, or returns the current one
+        // Not public - generate a queueHooks object, or return the current one
         _queueHooks: function(elem, type) {
             var key = type + "queueHooks";
-            return jQuery._data(elem, key) || jQuery._data(elem, key, {
+            return dataPriv.get(elem, key) || dataPriv.access(elem, key, {
                 empty: jQuery.Callbacks("once memory").add(function() {
-                    jQuery._removeData(elem, type + "queue");
-                    jQuery._removeData(elem, key);
+                    dataPriv.remove(elem, [type + "queue", key]);
                 })
             });
         }
     });
 
     jQuery.fn.extend({
         queue: function(type, data) {
@@ -4060,15 +4667,15 @@
             }
 
             return data === undefined ?
                 this :
                 this.each(function() {
                     var queue = jQuery.queue(this, type, data);
 
-                    // ensure a hooks for this queue
+                    // Ensure a hooks for this queue
                     jQuery._queueHooks(this, type);
 
                     if (type === "fx" && queue[0] !== "inprogress") {
                         jQuery.dequeue(this, type);
                     }
                 });
         },
@@ -4076,14 +4683,15 @@
             return this.each(function() {
                 jQuery.dequeue(this, type);
             });
         },
         clearQueue: function(type) {
             return this.queue(type || "fx", []);
         },
+
         // Get a promise resolved when queues of a certain type
         // are emptied (fx is the type by default)
         promise: function(type, obj) {
             var tmp,
                 count = 1,
                 defer = jQuery.Deferred(),
                 elements = this,
@@ -4097,256 +4705,572 @@
             if (typeof type !== "string") {
                 obj = type;
                 type = undefined;
             }
             type = type || "fx";
 
             while (i--) {
-                tmp = jQuery._data(elements[i], type + "queueHooks");
+                tmp = dataPriv.get(elements[i], type + "queueHooks");
                 if (tmp && tmp.empty) {
                     count++;
                     tmp.empty.add(resolve);
                 }
             }
             resolve();
             return defer.promise(obj);
         }
     });
     var pnum = (/[+-]?(?:\d*\.|)\d+(?:[eE][+-]?\d+|)/).source;
 
+    var rcssNum = new RegExp("^(?:([+-])=|)(" + pnum + ")([a-z%]*)$", "i");
+
+
     var cssExpand = ["Top", "Right", "Bottom", "Left"];
 
-    var isHidden = function(elem, el) {
-        // isHidden might be called from jQuery#filter function;
+    var documentElement = document.documentElement;
+
+
+
+    var isAttached = function(elem) {
+            return jQuery.contains(elem.ownerDocument, elem);
+        },
+        composed = {
+            composed: true
+        };
+
+    // Support: IE 9 - 11+, Edge 12 - 18+, iOS 10.0 - 10.2 only
+    // Check attachment across shadow DOM boundaries when possible (gh-3504)
+    // Support: iOS 10.0-10.2 only
+    // Early iOS 10 versions support `attachShadow` but not `getRootNode`,
+    // leading to errors. We need to check for `getRootNode`.
+    if (documentElement.getRootNode) {
+        isAttached = function(elem) {
+            return jQuery.contains(elem.ownerDocument, elem) ||
+                elem.getRootNode(composed) === elem.ownerDocument;
+        };
+    }
+    var isHiddenWithinTree = function(elem, el) {
+
+        // isHiddenWithinTree might be called from jQuery#filter function;
         // in that case, element will be second argument
         elem = el || elem;
-        return jQuery.css(elem, "display") === "none" || !jQuery.contains(elem.ownerDocument, elem);
+
+        // Inline style trumps all
+        return elem.style.display === "none" ||
+            elem.style.display === "" &&
+
+            // Otherwise, check computed style
+            // Support: Firefox <=43 - 45
+            // Disconnected elements can have computed display: none, so first confirm that elem is
+            // in the document.
+            isAttached(elem) &&
+
+            jQuery.css(elem, "display") === "none";
     };
 
 
 
-    // Multifunctional method to get and set values of a collection
-    // The value/s can optionally be executed if it's a function
-    var access = jQuery.access = function(elems, fn, key, value, chainable, emptyGet, raw) {
-        var i = 0,
-            length = elems.length,
-            bulk = key == null;
+    function adjustCSS(elem, prop, valueParts, tween) {
+        var adjusted, scale,
+            maxIterations = 20,
+            currentValue = tween ?
+            function() {
+                return tween.cur();
+            } :
+            function() {
+                return jQuery.css(elem, prop, "");
+            },
+            initial = currentValue(),
+            unit = valueParts && valueParts[3] || (jQuery.cssNumber[prop] ? "" : "px"),
+
+            // Starting value computation is required for potential unit mismatches
+            initialInUnit = elem.nodeType &&
+            (jQuery.cssNumber[prop] || unit !== "px" && +initial) &&
+            rcssNum.exec(jQuery.css(elem, prop));
+
+        if (initialInUnit && initialInUnit[3] !== unit) {
+
+            // Support: Firefox <=54
+            // Halve the iteration target value to prevent interference from CSS upper bounds (gh-2144)
+            initial = initial / 2;
+
+            // Trust units reported by jQuery.css
+            unit = unit || initialInUnit[3];
+
+            // Iteratively approximate from a nonzero starting point
+            initialInUnit = +initial || 1;
+
+            while (maxIterations--) {
+
+                // Evaluate and update our best guess (doubling guesses that zero out).
+                // Finish if the scale equals or crosses 1 (making the old*new product non-positive).
+                jQuery.style(elem, prop, initialInUnit + unit);
+                if ((1 - scale) * (1 - (scale = currentValue() / initial || 0.5)) <= 0) {
+                    maxIterations = 0;
+                }
+                initialInUnit = initialInUnit / scale;
 
-        // Sets many values
-        if (jQuery.type(key) === "object") {
-            chainable = true;
-            for (i in key) {
-                jQuery.access(elems, fn, i, key[i], true, emptyGet, raw);
             }
 
-            // Sets one value
-        } else if (value !== undefined) {
-            chainable = true;
+            initialInUnit = initialInUnit * 2;
+            jQuery.style(elem, prop, initialInUnit + unit);
 
-            if (!jQuery.isFunction(value)) {
-                raw = true;
+            // Make sure we update the tween properties later on
+            valueParts = valueParts || [];
+        }
+
+        if (valueParts) {
+            initialInUnit = +initialInUnit || +initial || 0;
+
+            // Apply relative offset (+=/-=) if specified
+            adjusted = valueParts[1] ?
+                initialInUnit + (valueParts[1] + 1) * valueParts[2] :
+                +valueParts[2];
+            if (tween) {
+                tween.unit = unit;
+                tween.start = initialInUnit;
+                tween.end = adjusted;
             }
+        }
+        return adjusted;
+    }
 
-            if (bulk) {
-                // Bulk operations run against the entire set
-                if (raw) {
-                    fn.call(elems, value);
-                    fn = null;
 
-                    // ...except when executing function values
-                } else {
-                    bulk = fn;
-                    fn = function(elem, key, value) {
-                        return bulk.call(jQuery(elem), value);
-                    };
-                }
+    var defaultDisplayMap = {};
+
+    function getDefaultDisplay(elem) {
+        var temp,
+            doc = elem.ownerDocument,
+            nodeName = elem.nodeName,
+            display = defaultDisplayMap[nodeName];
+
+        if (display) {
+            return display;
+        }
+
+        temp = doc.body.appendChild(doc.createElement(nodeName));
+        display = jQuery.css(temp, "display");
+
+        temp.parentNode.removeChild(temp);
+
+        if (display === "none") {
+            display = "block";
+        }
+        defaultDisplayMap[nodeName] = display;
+
+        return display;
+    }
+
+    function showHide(elements, show) {
+        var display, elem,
+            values = [],
+            index = 0,
+            length = elements.length;
+
+        // Determine new display value for elements that need to change
+        for (; index < length; index++) {
+            elem = elements[index];
+            if (!elem.style) {
+                continue;
             }
 
-            if (fn) {
-                for (; i < length; i++) {
-                    fn(elems[i], key, raw ? value : value.call(elems[i], i, fn(elems[i], key)));
+            display = elem.style.display;
+            if (show) {
+
+                // Since we force visibility upon cascade-hidden elements, an immediate (and slow)
+                // check is required in this first loop unless we have a nonempty display value (either
+                // inline or about-to-be-restored)
+                if (display === "none") {
+                    values[index] = dataPriv.get(elem, "display") || null;
+                    if (!values[index]) {
+                        elem.style.display = "";
+                    }
+                }
+                if (elem.style.display === "" && isHiddenWithinTree(elem)) {
+                    values[index] = getDefaultDisplay(elem);
                 }
+            } else {
+                if (display !== "none") {
+                    values[index] = "none";
+
+                    // Remember what we're overwriting
+                    dataPriv.set(elem, "display", display);
+                }
+            }
+        }
+
+        // Set the display of the elements in a second loop to avoid constant reflow
+        for (index = 0; index < length; index++) {
+            if (values[index] != null) {
+                elements[index].style.display = values[index];
             }
         }
 
-        return chainable ?
-            elems :
+        return elements;
+    }
 
-            // Gets
-            bulk ?
-            fn.call(elems) :
-            length ? fn(elems[0], key) : emptyGet;
-    };
+    jQuery.fn.extend({
+        show: function() {
+            return showHide(this, true);
+        },
+        hide: function() {
+            return showHide(this);
+        },
+        toggle: function(state) {
+            if (typeof state === "boolean") {
+                return state ? this.show() : this.hide();
+            }
+
+            return this.each(function() {
+                if (isHiddenWithinTree(this)) {
+                    jQuery(this).show();
+                } else {
+                    jQuery(this).hide();
+                }
+            });
+        }
+    });
     var rcheckableType = (/^(?:checkbox|radio)$/i);
 
+    var rtagName = (/<([a-z][^\/\0>\x20\t\r\n\f]*)/i);
 
+    var rscriptType = (/^$|^module$|\/(?:java|ecma)script/i);
 
-    (function() {
-        // Minified: var a,b,c
-        var input = document.createElement("input"),
-            div = document.createElement("div"),
-            fragment = document.createDocumentFragment();
 
-        // Setup
-        div.innerHTML = "  <link/><table></table><a href='/a'>a</a><input type='checkbox'/>";
 
-        // IE strips leading whitespace when .innerHTML is used
-        support.leadingWhitespace = div.firstChild.nodeType === 3;
+    (function() {
+        var fragment = document.createDocumentFragment(),
+            div = fragment.appendChild(document.createElement("div")),
+            input = document.createElement("input");
+
+        // Support: Android 4.0 - 4.3 only
+        // Check state lost if the name is set (trac-11217)
+        // Support: Windows Web Apps (WWA)
+        // `name` and `type` must use .setAttribute for WWA (trac-14901)
+        input.setAttribute("type", "radio");
+        input.setAttribute("checked", "checked");
+        input.setAttribute("name", "t");
 
-        // Make sure that tbody elements aren't automatically inserted
-        // IE will insert them into empty tables
-        support.tbody = !div.getElementsByTagName("tbody").length;
-
-        // Make sure that link elements get serialized correctly by innerHTML
-        // This requires a wrapper element in IE
-        support.htmlSerialize = !!div.getElementsByTagName("link").length;
-
-        // Makes sure cloning an html5 element does not cause problems
-        // Where outerHTML is undefined, this still works
-        support.html5Clone =
-            document.createElement("nav").cloneNode(true).outerHTML !== "<:nav></:nav>";
+        div.appendChild(input);
 
-        // Check if a disconnected checkbox will retain its checked
-        // value of true after appended to the DOM (IE6/7)
-        input.type = "checkbox";
-        input.checked = true;
-        fragment.appendChild(input);
-        support.appendChecked = input.checked;
+        // Support: Android <=4.1 only
+        // Older WebKit doesn't clone checked state correctly in fragments
+        support.checkClone = div.cloneNode(true).cloneNode(true).lastChild.checked;
 
+        // Support: IE <=11 only
         // Make sure textarea (and checkbox) defaultValue is properly cloned
-        // Support: IE6-IE11+
         div.innerHTML = "<textarea>x</textarea>";
         support.noCloneChecked = !!div.cloneNode(true).lastChild.defaultValue;
 
-        // #11217 - WebKit loses check when the name is after the checked attribute
-        fragment.appendChild(div);
-        div.innerHTML = "<input type='radio' checked='checked' name='t'/>";
+        // Support: IE <=9 only
+        // IE <=9 replaces <option> tags with their contents when inserted outside of
+        // the select element.
+        div.innerHTML = "<option></option>";
+        support.option = !!div.lastChild;
+    })();
 
-        // Support: Safari 5.1, iOS 5.1, Android 4.x, Android 2.3
-        // old WebKit doesn't clone checked state correctly in fragments
-        support.checkClone = div.cloneNode(true).cloneNode(true).lastChild.checked;
 
-        // Support: IE<9
-        // Opera does not clone events (and typeof div.attachEvent === undefined).
-        // IE9-10 clones events bound via attachEvent, but they don't trigger with .click()
-        support.noCloneEvent = true;
-        if (div.attachEvent) {
-            div.attachEvent("onclick", function() {
-                support.noCloneEvent = false;
-            });
+    // We have to close these tags to support XHTML (trac-13200)
+    var wrapMap = {
+
+        // XHTML parsers do not magically insert elements in the
+        // same way that tag soup parsers do. So we cannot shorten
+        // this by omitting <tbody> or other required elements.
+        thead: [1, "<table>", "</table>"],
+        col: [2, "<table><colgroup>", "</colgroup></table>"],
+        tr: [2, "<table><tbody>", "</tbody></table>"],
+        td: [3, "<table><tbody><tr>", "</tr></tbody></table>"],
+
+        _default: [0, "", ""]
+    };
+
+    wrapMap.tbody = wrapMap.tfoot = wrapMap.colgroup = wrapMap.caption = wrapMap.thead;
+    wrapMap.th = wrapMap.td;
+
+    // Support: IE <=9 only
+    if (!support.option) {
+        wrapMap.optgroup = wrapMap.option = [1, "<select multiple='multiple'>", "</select>"];
+    }
 
-            div.cloneNode(true).click();
+
+    function getAll(context, tag) {
+
+        // Support: IE <=9 - 11 only
+        // Use typeof to avoid zero-argument method invocation on host objects (trac-15151)
+        var ret;
+
+        if (typeof context.getElementsByTagName !== "undefined") {
+            ret = context.getElementsByTagName(tag || "*");
+
+        } else if (typeof context.querySelectorAll !== "undefined") {
+            ret = context.querySelectorAll(tag || "*");
+
+        } else {
+            ret = [];
         }
 
-        // Execute the test only if not already executed in another module.
-        if (support.deleteExpando == null) {
-            // Support: IE<9
-            support.deleteExpando = true;
-            try {
-                delete div.test;
-            } catch (e) {
-                support.deleteExpando = false;
+        if (tag === undefined || tag && nodeName(context, tag)) {
+            return jQuery.merge([context], ret);
+        }
+
+        return ret;
+    }
+
+
+    // Mark scripts as having already been evaluated
+    function setGlobalEval(elems, refElements) {
+        var i = 0,
+            l = elems.length;
+
+        for (; i < l; i++) {
+            dataPriv.set(
+                elems[i],
+                "globalEval",
+                !refElements || dataPriv.get(refElements[i], "globalEval")
+            );
+        }
+    }
+
+
+    var rhtml = /<|&#?\w+;/;
+
+    function buildFragment(elems, context, scripts, selection, ignored) {
+        var elem, tmp, tag, wrap, attached, j,
+            fragment = context.createDocumentFragment(),
+            nodes = [],
+            i = 0,
+            l = elems.length;
+
+        for (; i < l; i++) {
+            elem = elems[i];
+
+            if (elem || elem === 0) {
+
+                // Add nodes directly
+                if (toType(elem) === "object") {
+
+                    // Support: Android <=4.0 only, PhantomJS 1 only
+                    // push.apply(_, arraylike) throws on ancient WebKit
+                    jQuery.merge(nodes, elem.nodeType ? [elem] : elem);
+
+                    // Convert non-html into a text node
+                } else if (!rhtml.test(elem)) {
+                    nodes.push(context.createTextNode(elem));
+
+                    // Convert html into DOM nodes
+                } else {
+                    tmp = tmp || fragment.appendChild(context.createElement("div"));
+
+                    // Deserialize a standard representation
+                    tag = (rtagName.exec(elem) || ["", ""])[1].toLowerCase();
+                    wrap = wrapMap[tag] || wrapMap._default;
+                    tmp.innerHTML = wrap[1] + jQuery.htmlPrefilter(elem) + wrap[2];
+
+                    // Descend through wrappers to the right content
+                    j = wrap[0];
+                    while (j--) {
+                        tmp = tmp.lastChild;
+                    }
+
+                    // Support: Android <=4.0 only, PhantomJS 1 only
+                    // push.apply(_, arraylike) throws on ancient WebKit
+                    jQuery.merge(nodes, tmp.childNodes);
+
+                    // Remember the top-level container
+                    tmp = fragment.firstChild;
+
+                    // Ensure the created nodes are orphaned (trac-12392)
+                    tmp.textContent = "";
+                }
             }
         }
-    })();
 
+        // Remove wrapper from fragment
+        fragment.textContent = "";
 
-    (function() {
-        var i, eventName,
-            div = document.createElement("div");
+        i = 0;
+        while ((elem = nodes[i++])) {
+
+            // Skip elements already in the context collection (trac-4087)
+            if (selection && jQuery.inArray(elem, selection) > -1) {
+                if (ignored) {
+                    ignored.push(elem);
+                }
+                continue;
+            }
+
+            attached = isAttached(elem);
+
+            // Append to fragment
+            tmp = getAll(fragment.appendChild(elem), "script");
+
+            // Preserve script evaluation history
+            if (attached) {
+                setGlobalEval(tmp);
+            }
 
-        // Support: IE<9 (lack submit/change bubble), Firefox 23+ (lack focusin event)
-        for (i in {
-                submit: true,
-                change: true,
-                focusin: true
-            }) {
-            eventName = "on" + i;
-
-            if (!(support[i + "Bubbles"] = eventName in window)) {
-                // Beware of CSP restrictions (https://developer.mozilla.org/en/Security/CSP)
-                div.setAttribute(eventName, "t");
-                support[i + "Bubbles"] = div.attributes[eventName].expando === false;
+            // Capture executables
+            if (scripts) {
+                j = 0;
+                while ((elem = tmp[j++])) {
+                    if (rscriptType.test(elem.type || "")) {
+                        scripts.push(elem);
+                    }
+                }
             }
         }
 
-        // Null elements to avoid leaks in IE.
-        div = null;
-    })();
+        return fragment;
+    }
 
 
-    var rformElems = /^(?:input|select|textarea)$/i,
-        rkeyEvent = /^key/,
-        rmouseEvent = /^(?:mouse|pointer|contextmenu)|click/,
-        rfocusMorph = /^(?:focusinfocus|focusoutblur)$/,
-        rtypenamespace = /^([^.]*)(?:\.(.+)|)$/;
+    var rtypenamespace = /^([^.]*)(?:\.(.+)|)/;
 
     function returnTrue() {
         return true;
     }
 
     function returnFalse() {
         return false;
     }
 
+    // Support: IE <=9 - 11+
+    // focus() and blur() are asynchronous, except when they are no-op.
+    // So expect focus to be synchronous when the element is already active,
+    // and blur to be synchronous when the element is not already active.
+    // (focus and blur are always synchronous in other supported browsers,
+    // this just defines when we can count on it).
+    function expectSync(elem, type) {
+        return (elem === safeActiveElement()) === (type === "focus");
+    }
+
+    // Support: IE <=9 only
+    // Accessing document.activeElement can throw unexpectedly
+    // https://bugs.jquery.com/ticket/13393
     function safeActiveElement() {
         try {
             return document.activeElement;
         } catch (err) {}
     }
 
+    function on(elem, types, selector, data, fn, one) {
+        var origFn, type;
+
+        // Types can be a map of types/handlers
+        if (typeof types === "object") {
+
+            // ( types-Object, selector, data )
+            if (typeof selector !== "string") {
+
+                // ( types-Object, data )
+                data = data || selector;
+                selector = undefined;
+            }
+            for (type in types) {
+                on(elem, type, selector, data, types[type], one);
+            }
+            return elem;
+        }
+
+        if (data == null && fn == null) {
+
+            // ( types, fn )
+            fn = selector;
+            data = selector = undefined;
+        } else if (fn == null) {
+            if (typeof selector === "string") {
+
+                // ( types, selector, fn )
+                fn = data;
+                data = undefined;
+            } else {
+
+                // ( types, data, fn )
+                fn = data;
+                data = selector;
+                selector = undefined;
+            }
+        }
+        if (fn === false) {
+            fn = returnFalse;
+        } else if (!fn) {
+            return elem;
+        }
+
+        if (one === 1) {
+            origFn = fn;
+            fn = function(event) {
+
+                // Can use an empty set, since event contains the info
+                jQuery().off(event);
+                return origFn.apply(this, arguments);
+            };
+
+            // Use same guid so caller can remove using origFn
+            fn.guid = origFn.guid || (origFn.guid = jQuery.guid++);
+        }
+        return elem.each(function() {
+            jQuery.event.add(this, types, fn, data, selector);
+        });
+    }
+
     /*
      * Helper functions for managing events -- not part of the public interface.
      * Props to Dean Edwards' addEvent library for many of the ideas.
      */
     jQuery.event = {
 
         global: {},
 
         add: function(elem, types, handler, data, selector) {
-            var tmp, events, t, handleObjIn,
-                special, eventHandle, handleObj,
-                handlers, type, namespaces, origType,
-                elemData = jQuery._data(elem);
 
-            // Don't attach events to noData or text/comment nodes (but allow plain objects)
-            if (!elemData) {
+            var handleObjIn, eventHandle, tmp,
+                events, t, handleObj,
+                special, handlers, type, namespaces, origType,
+                elemData = dataPriv.get(elem);
+
+            // Only attach events to objects that accept data
+            if (!acceptData(elem)) {
                 return;
             }
 
             // Caller can pass in an object of custom data in lieu of the handler
             if (handler.handler) {
                 handleObjIn = handler;
                 handler = handleObjIn.handler;
                 selector = handleObjIn.selector;
             }
 
+            // Ensure that invalid selectors throw exceptions at attach time
+            // Evaluate against documentElement in case elem is a non-element node (e.g., document)
+            if (selector) {
+                jQuery.find.matchesSelector(documentElement, selector);
+            }
+
             // Make sure that the handler has a unique ID, used to find/remove it later
             if (!handler.guid) {
                 handler.guid = jQuery.guid++;
             }
 
             // Init the element's event structure and main handler, if this is the first
             if (!(events = elemData.events)) {
-                events = elemData.events = {};
+                events = elemData.events = Object.create(null);
             }
             if (!(eventHandle = elemData.handle)) {
                 eventHandle = elemData.handle = function(e) {
+
                     // Discard the second event of a jQuery.event.trigger() and
                     // when an event is called after a page has unloaded
-                    return typeof jQuery !== strundefined && (!e || jQuery.event.triggered !== e.type) ?
-                        jQuery.event.dispatch.apply(eventHandle.elem, arguments) :
-                        undefined;
+                    return typeof jQuery !== "undefined" && jQuery.event.triggered !== e.type ?
+                        jQuery.event.dispatch.apply(elem, arguments) : undefined;
                 };
-                // Add elem as a property of the handle fn to prevent a memory leak with IE non-native events
-                eventHandle.elem = elem;
             }
 
             // Handle multiple events separated by a space
-            types = (types || "").match(rnotwhite) || [""];
+            types = (types || "").match(rnothtmlwhite) || [""];
             t = types.length;
             while (t--) {
                 tmp = rtypenamespace.exec(types[t]) || [];
                 type = origType = tmp[1];
                 namespaces = (tmp[2] || "").split(".").sort();
 
                 // There *must* be a type, no attaching namespace-only handlers
@@ -4376,22 +5300,20 @@
                 }, handleObjIn);
 
                 // Init the event handler queue if we're the first
                 if (!(handlers = events[type])) {
                     handlers = events[type] = [];
                     handlers.delegateCount = 0;
 
-                    // Only use addEventListener/attachEvent if the special events handler returns false
-                    if (!special.setup || special.setup.call(elem, data, namespaces, eventHandle) === false) {
-                        // Bind the global event handler to the element
-                        if (elem.addEventListener) {
-                            elem.addEventListener(type, eventHandle, false);
+                    // Only use addEventListener if the special events handler returns false
+                    if (!special.setup ||
+                        special.setup.call(elem, data, namespaces, eventHandle) === false) {
 
-                        } else if (elem.attachEvent) {
-                            elem.attachEvent("on" + type, eventHandle);
+                        if (elem.addEventListener) {
+                            elem.addEventListener(type, eventHandle);
                         }
                     }
                 }
 
                 if (special.add) {
                     special.add.call(elem, handleObj);
 
@@ -4407,32 +5329,30 @@
                     handlers.push(handleObj);
                 }
 
                 // Keep track of which events have ever been used, for event optimization
                 jQuery.event.global[type] = true;
             }
 
-            // Nullify elem to prevent memory leaks in IE
-            elem = null;
         },
 
         // Detach an event or set of events from an element
         remove: function(elem, types, handler, selector, mappedTypes) {
-            var j, handleObj, tmp,
-                origCount, t, events,
-                special, handlers, type,
-                namespaces, origType,
-                elemData = jQuery.hasData(elem) && jQuery._data(elem);
+
+            var j, origCount, tmp,
+                events, t, handleObj,
+                special, handlers, type, namespaces, origType,
+                elemData = dataPriv.hasData(elem) && dataPriv.get(elem);
 
             if (!elemData || !(events = elemData.events)) {
                 return;
             }
 
             // Once for each type.namespace in types; type may be omitted
-            types = (types || "").match(rnotwhite) || [""];
+            types = (types || "").match(rnothtmlwhite) || [""];
             t = types.length;
             while (t--) {
                 tmp = rtypenamespace.exec(types[t]) || [];
                 type = origType = tmp[1];
                 namespaces = (tmp[2] || "").split(".").sort();
 
                 // Unbind all events (on this namespace, if provided) for the element
@@ -4442,207 +5362,77 @@
                     }
                     continue;
                 }
 
                 special = jQuery.event.special[type] || {};
                 type = (selector ? special.delegateType : special.bindType) || type;
                 handlers = events[type] || [];
-                tmp = tmp[2] && new RegExp("(^|\\.)" + namespaces.join("\\.(?:.*\\.|)") + "(\\.|$)");
+                tmp = tmp[2] &&
+                    new RegExp("(^|\\.)" + namespaces.join("\\.(?:.*\\.|)") + "(\\.|$)");
 
                 // Remove matching events
                 origCount = j = handlers.length;
                 while (j--) {
                     handleObj = handlers[j];
 
                     if ((mappedTypes || origType === handleObj.origType) &&
                         (!handler || handler.guid === handleObj.guid) &&
                         (!tmp || tmp.test(handleObj.namespace)) &&
-                        (!selector || selector === handleObj.selector || selector === "**" && handleObj.selector)) {
+                        (!selector || selector === handleObj.selector ||
+                            selector === "**" && handleObj.selector)) {
                         handlers.splice(j, 1);
 
                         if (handleObj.selector) {
                             handlers.delegateCount--;
                         }
                         if (special.remove) {
                             special.remove.call(elem, handleObj);
                         }
                     }
                 }
 
                 // Remove generic event handler if we removed something and no more handlers exist
                 // (avoids potential for endless recursion during removal of special event handlers)
                 if (origCount && !handlers.length) {
-                    if (!special.teardown || special.teardown.call(elem, namespaces, elemData.handle) === false) {
+                    if (!special.teardown ||
+                        special.teardown.call(elem, namespaces, elemData.handle) === false) {
+
                         jQuery.removeEvent(elem, type, elemData.handle);
                     }
 
                     delete events[type];
                 }
             }
 
-            // Remove the expando if it's no longer used
+            // Remove data and the expando if it's no longer used
             if (jQuery.isEmptyObject(events)) {
-                delete elemData.handle;
-
-                // removeData also checks for emptiness and clears the expando if empty
-                // so use it instead of delete
-                jQuery._removeData(elem, "events");
+                dataPriv.remove(elem, "handle events");
             }
         },
 
-        trigger: function(event, data, elem, onlyHandlers) {
-            var handle, ontype, cur,
-                bubbleType, special, tmp, i,
-                eventPath = [elem || document],
-                type = hasOwn.call(event, "type") ? event.type : event,
-                namespaces = hasOwn.call(event, "namespace") ? event.namespace.split(".") : [];
-
-            cur = tmp = elem = elem || document;
+        dispatch: function(nativeEvent) {
 
-            // Don't do events on text and comment nodes
-            if (elem.nodeType === 3 || elem.nodeType === 8) {
-                return;
-            }
-
-            // focus/blur morphs to focusin/out; ensure we're not firing them right now
-            if (rfocusMorph.test(type + jQuery.event.triggered)) {
-                return;
-            }
+            var i, j, ret, matched, handleObj, handlerQueue,
+                args = new Array(arguments.length),
 
-            if (type.indexOf(".") >= 0) {
-                // Namespaced trigger; create a regexp to match event type in handle()
-                namespaces = type.split(".");
-                type = namespaces.shift();
-                namespaces.sort();
-            }
-            ontype = type.indexOf(":") < 0 && "on" + type;
+                // Make a writable jQuery.Event from the native event object
+                event = jQuery.event.fix(nativeEvent),
 
-            // Caller can pass in a jQuery.Event object, Object, or just an event type string
-            event = event[jQuery.expando] ?
-                event :
-                new jQuery.Event(type, typeof event === "object" && event);
-
-            // Trigger bitmask: & 1 for native handlers; & 2 for jQuery (always true)
-            event.isTrigger = onlyHandlers ? 2 : 3;
-            event.namespace = namespaces.join(".");
-            event.namespace_re = event.namespace ?
-                new RegExp("(^|\\.)" + namespaces.join("\\.(?:.*\\.|)") + "(\\.|$)") :
-                null;
-
-            // Clean up the event in case it is being reused
-            event.result = undefined;
-            if (!event.target) {
-                event.target = elem;
-            }
-
-            // Clone any incoming data and prepend the event, creating the handler arg list
-            data = data == null ? [event] :
-                jQuery.makeArray(data, [event]);
-
-            // Allow special events to draw outside the lines
-            special = jQuery.event.special[type] || {};
-            if (!onlyHandlers && special.trigger && special.trigger.apply(elem, data) === false) {
-                return;
-            }
-
-            // Determine event propagation path in advance, per W3C events spec (#9951)
-            // Bubble up to document, then to window; watch for a global ownerDocument var (#9724)
-            if (!onlyHandlers && !special.noBubble && !jQuery.isWindow(elem)) {
-
-                bubbleType = special.delegateType || type;
-                if (!rfocusMorph.test(bubbleType + type)) {
-                    cur = cur.parentNode;
-                }
-                for (; cur; cur = cur.parentNode) {
-                    eventPath.push(cur);
-                    tmp = cur;
-                }
-
-                // Only add window if we got to document (e.g., not plain obj or detached DOM)
-                if (tmp === (elem.ownerDocument || document)) {
-                    eventPath.push(tmp.defaultView || tmp.parentWindow || window);
-                }
-            }
-
-            // Fire handlers on the event path
-            i = 0;
-            while ((cur = eventPath[i++]) && !event.isPropagationStopped()) {
-
-                event.type = i > 1 ?
-                    bubbleType :
-                    special.bindType || type;
-
-                // jQuery handler
-                handle = (jQuery._data(cur, "events") || {})[event.type] && jQuery._data(cur, "handle");
-                if (handle) {
-                    handle.apply(cur, data);
-                }
-
-                // Native handler
-                handle = ontype && cur[ontype];
-                if (handle && handle.apply && jQuery.acceptData(cur)) {
-                    event.result = handle.apply(cur, data);
-                    if (event.result === false) {
-                        event.preventDefault();
-                    }
-                }
-            }
-            event.type = type;
-
-            // If nobody prevented the default action, do it now
-            if (!onlyHandlers && !event.isDefaultPrevented()) {
-
-                if ((!special._default || special._default.apply(eventPath.pop(), data) === false) &&
-                    jQuery.acceptData(elem)) {
-
-                    // Call a native DOM method on the target with the same name name as the event.
-                    // Can't use an .isFunction() check here because IE6/7 fails that test.
-                    // Don't do default actions on window, that's where global variables be (#6170)
-                    if (ontype && elem[type] && !jQuery.isWindow(elem)) {
-
-                        // Don't re-trigger an onFOO event when we call its FOO() method
-                        tmp = elem[ontype];
-
-                        if (tmp) {
-                            elem[ontype] = null;
-                        }
-
-                        // Prevent re-triggering of the same event, since we already bubbled it above
-                        jQuery.event.triggered = type;
-                        try {
-                            elem[type]();
-                        } catch (e) {
-                            // IE<9 dies on focus/blur to hidden element (#1486,#12518)
-                            // only reproducible on winXP IE8 native, not IE9 in IE8 mode
-                        }
-                        jQuery.event.triggered = undefined;
-
-                        if (tmp) {
-                            elem[ontype] = tmp;
-                        }
-                    }
-                }
-            }
-
-            return event.result;
-        },
-
-        dispatch: function(event) {
-
-            // Make a writable jQuery.Event from the native event object
-            event = jQuery.event.fix(event);
-
-            var i, ret, handleObj, matched, j,
-                handlerQueue = [],
-                args = slice.call(arguments),
-                handlers = (jQuery._data(this, "events") || {})[event.type] || [],
+                handlers = (
+                    dataPriv.get(this, "events") || Object.create(null)
+                )[event.type] || [],
                 special = jQuery.event.special[event.type] || {};
 
             // Use the fix-ed jQuery.Event rather than the (read-only) native event
             args[0] = event;
+
+            for (i = 1; i < arguments.length; i++) {
+                args[i] = arguments[i];
+            }
+
             event.delegateTarget = this;
 
             // Call the preDispatch hook for the mapped type, and let it bail if desired
             if (special.preDispatch && special.preDispatch.call(this, event) === false) {
                 return;
             }
 
@@ -4651,25 +5441,27 @@
 
             // Run delegates first; they may want to stop propagation beneath us
             i = 0;
             while ((matched = handlerQueue[i++]) && !event.isPropagationStopped()) {
                 event.currentTarget = matched.elem;
 
                 j = 0;
-                while ((handleObj = matched.handlers[j++]) && !event.isImmediatePropagationStopped()) {
+                while ((handleObj = matched.handlers[j++]) &&
+                    !event.isImmediatePropagationStopped()) {
 
-                    // Triggered event must either 1) have no namespace, or
-                    // 2) have namespace(s) a subset or equal to those in the bound event (both can have no namespace).
-                    if (!event.namespace_re || event.namespace_re.test(handleObj.namespace)) {
+                    // If the event is namespaced, then each handler is only invoked if it is
+                    // specially universal or its namespaces are a superset of the event's.
+                    if (!event.rnamespace || handleObj.namespace === false ||
+                        event.rnamespace.test(handleObj.namespace)) {
 
                         event.handleObj = handleObj;
                         event.data = handleObj.data;
 
-                        ret = ((jQuery.event.special[handleObj.origType] || {}).handle || handleObj.handler)
-                            .apply(matched.elem, args);
+                        ret = ((jQuery.event.special[handleObj.origType] || {}).handle ||
+                            handleObj.handler).apply(matched.elem, args);
 
                         if (ret !== undefined) {
                             if ((event.result = ret) === false) {
                                 event.preventDefault();
                                 event.stopPropagation();
                             }
                         }
@@ -4682,356 +5474,446 @@
                 special.postDispatch.call(this, event);
             }
 
             return event.result;
         },
 
         handlers: function(event, handlers) {
-            var sel, handleObj, matches, i,
+            var i, handleObj, sel, matchedHandlers, matchedSelectors,
                 handlerQueue = [],
                 delegateCount = handlers.delegateCount,
                 cur = event.target;
 
             // Find delegate handlers
-            // Black-hole SVG <use> instance trees (#13180)
-            // Avoid non-left-click bubbling in Firefox (#3861)
-            if (delegateCount && cur.nodeType && (!event.button || event.type !== "click")) {
-
-                /* jshint eqeqeq: false */
-                for (; cur != this; cur = cur.parentNode || this) {
-                    /* jshint eqeqeq: true */
-
-                    // Don't check non-elements (#13208)
-                    // Don't process clicks on disabled elements (#6911, #8165, #11382, #11764)
-                    if (cur.nodeType === 1 && (cur.disabled !== true || event.type !== "click")) {
-                        matches = [];
+            if (delegateCount &&
+
+                // Support: IE <=9
+                // Black-hole SVG <use> instance trees (trac-13180)
+                cur.nodeType &&
+
+                // Support: Firefox <=42
+                // Suppress spec-violating clicks indicating a non-primary pointer button (trac-3861)
+                // https://www.w3.org/TR/DOM-Level-3-Events/#event-type-click
+                // Support: IE 11 only
+                // ...but not arrow key "clicks" of radio inputs, which can have `button` -1 (gh-2343)
+                !(event.type === "click" && event.button >= 1)) {
+
+                for (; cur !== this; cur = cur.parentNode || this) {
+
+                    // Don't check non-elements (trac-13208)
+                    // Don't process clicks on disabled elements (trac-6911, trac-8165, trac-11382, trac-11764)
+                    if (cur.nodeType === 1 && !(event.type === "click" && cur.disabled === true)) {
+                        matchedHandlers = [];
+                        matchedSelectors = {};
                         for (i = 0; i < delegateCount; i++) {
                             handleObj = handlers[i];
 
-                            // Don't conflict with Object.prototype properties (#13203)
+                            // Don't conflict with Object.prototype properties (trac-13203)
                             sel = handleObj.selector + " ";
 
-                            if (matches[sel] === undefined) {
-                                matches[sel] = handleObj.needsContext ?
-                                    jQuery(sel, this).index(cur) >= 0 :
+                            if (matchedSelectors[sel] === undefined) {
+                                matchedSelectors[sel] = handleObj.needsContext ?
+                                    jQuery(sel, this).index(cur) > -1 :
                                     jQuery.find(sel, this, null, [cur]).length;
                             }
-                            if (matches[sel]) {
-                                matches.push(handleObj);
+                            if (matchedSelectors[sel]) {
+                                matchedHandlers.push(handleObj);
                             }
                         }
-                        if (matches.length) {
+                        if (matchedHandlers.length) {
                             handlerQueue.push({
                                 elem: cur,
-                                handlers: matches
+                                handlers: matchedHandlers
                             });
                         }
                     }
                 }
             }
 
             // Add the remaining (directly-bound) handlers
+            cur = this;
             if (delegateCount < handlers.length) {
                 handlerQueue.push({
-                    elem: this,
+                    elem: cur,
                     handlers: handlers.slice(delegateCount)
                 });
             }
 
             return handlerQueue;
         },
 
-        fix: function(event) {
-            if (event[jQuery.expando]) {
-                return event;
-            }
-
-            // Create a writable copy of the event object and normalize some properties
-            var i, prop, copy,
-                type = event.type,
-                originalEvent = event,
-                fixHook = this.fixHooks[type];
-
-            if (!fixHook) {
-                this.fixHooks[type] = fixHook =
-                    rmouseEvent.test(type) ? this.mouseHooks :
-                    rkeyEvent.test(type) ? this.keyHooks : {};
-            }
-            copy = fixHook.props ? this.props.concat(fixHook.props) : this.props;
-
-            event = new jQuery.Event(originalEvent);
-
-            i = copy.length;
-            while (i--) {
-                prop = copy[i];
-                event[prop] = originalEvent[prop];
-            }
-
-            // Support: IE<9
-            // Fix target property (#1925)
-            if (!event.target) {
-                event.target = originalEvent.srcElement || document;
-            }
-
-            // Support: Chrome 23+, Safari?
-            // Target should not be a text node (#504, #13143)
-            if (event.target.nodeType === 3) {
-                event.target = event.target.parentNode;
-            }
-
-            // Support: IE<9
-            // For mouse/key events, metaKey==false if it's undefined (#3368, #11328)
-            event.metaKey = !!event.metaKey;
-
-            return fixHook.filter ? fixHook.filter(event, originalEvent) : event;
-        },
-
-        // Includes some event props shared by KeyEvent and MouseEvent
-        props: "altKey bubbles cancelable ctrlKey currentTarget eventPhase metaKey relatedTarget shiftKey target timeStamp view which".split(" "),
-
-        fixHooks: {},
-
-        keyHooks: {
-            props: "char charCode key keyCode".split(" "),
-            filter: function(event, original) {
+        addProp: function(name, hook) {
+            Object.defineProperty(jQuery.Event.prototype, name, {
+                enumerable: true,
+                configurable: true,
+
+                get: isFunction(hook) ?
+                    function() {
+                        if (this.originalEvent) {
+                            return hook(this.originalEvent);
+                        }
+                    } : function() {
+                        if (this.originalEvent) {
+                            return this.originalEvent[name];
+                        }
+                    },
 
-                // Add which for key events
-                if (event.which == null) {
-                    event.which = original.charCode != null ? original.charCode : original.keyCode;
+                set: function(value) {
+                    Object.defineProperty(this, name, {
+                        enumerable: true,
+                        configurable: true,
+                        writable: true,
+                        value: value
+                    });
                 }
-
-                return event;
-            }
+            });
         },
 
-        mouseHooks: {
-            props: "button buttons clientX clientY fromElement offsetX offsetY pageX pageY screenX screenY toElement".split(" "),
-            filter: function(event, original) {
-                var body, eventDoc, doc,
-                    button = original.button,
-                    fromElement = original.fromElement;
-
-                // Calculate pageX/Y if missing and clientX/Y available
-                if (event.pageX == null && original.clientX != null) {
-                    eventDoc = event.target.ownerDocument || document;
-                    doc = eventDoc.documentElement;
-                    body = eventDoc.body;
-
-                    event.pageX = original.clientX + (doc && doc.scrollLeft || body && body.scrollLeft || 0) - (doc && doc.clientLeft || body && body.clientLeft || 0);
-                    event.pageY = original.clientY + (doc && doc.scrollTop || body && body.scrollTop || 0) - (doc && doc.clientTop || body && body.clientTop || 0);
-                }
-
-                // Add relatedTarget, if necessary
-                if (!event.relatedTarget && fromElement) {
-                    event.relatedTarget = fromElement === event.target ? original.toElement : fromElement;
-                }
-
-                // Add which for click: 1 === left; 2 === middle; 3 === right
-                // Note: button is not normalized, so don't use it
-                if (!event.which && button !== undefined) {
-                    event.which = (button & 1 ? 1 : (button & 2 ? 3 : (button & 4 ? 2 : 0)));
-                }
-
-                return event;
-            }
+        fix: function(originalEvent) {
+            return originalEvent[jQuery.expando] ?
+                originalEvent :
+                new jQuery.Event(originalEvent);
         },
 
         special: {
             load: {
+
                 // Prevent triggered image.load events from bubbling to window.load
                 noBubble: true
             },
-            focus: {
-                // Fire native event if possible so blur/focus sequence is correct
-                trigger: function() {
-                    if (this !== safeActiveElement() && this.focus) {
-                        try {
-                            this.focus();
-                            return false;
-                        } catch (e) {
-                            // Support: IE<9
-                            // If we error on focus to hidden element (#1486, #12518),
-                            // let .trigger() run the handlers
-                        }
-                    }
-                },
-                delegateType: "focusin"
-            },
-            blur: {
-                trigger: function() {
-                    if (this === safeActiveElement() && this.blur) {
-                        this.blur();
-                        return false;
+            click: {
+
+                // Utilize native event to ensure correct state for checkable inputs
+                setup: function(data) {
+
+                    // For mutual compressibility with _default, replace `this` access with a local var.
+                    // `|| data` is dead code meant only to preserve the variable through minification.
+                    var el = this || data;
+
+                    // Claim the first handler
+                    if (rcheckableType.test(el.type) &&
+                        el.click && nodeName(el, "input")) {
+
+                        // dataPriv.set( el, "click", ... )
+                        leverageNative(el, "click", returnTrue);
                     }
+
+                    // Return false to allow normal processing in the caller
+                    return false;
                 },
-                delegateType: "focusout"
-            },
-            click: {
-                // For checkbox, fire native event so checked state will be right
-                trigger: function() {
-                    if (jQuery.nodeName(this, "input") && this.type === "checkbox" && this.click) {
-                        this.click();
-                        return false;
+                trigger: function(data) {
+
+                    // For mutual compressibility with _default, replace `this` access with a local var.
+                    // `|| data` is dead code meant only to preserve the variable through minification.
+                    var el = this || data;
+
+                    // Force setup before triggering a click
+                    if (rcheckableType.test(el.type) &&
+                        el.click && nodeName(el, "input")) {
+
+                        leverageNative(el, "click");
                     }
+
+                    // Return non-false to allow normal event-path propagation
+                    return true;
                 },
 
-                // For cross-browser consistency, don't fire native .click() on links
+                // For cross-browser consistency, suppress native .click() on links
+                // Also prevent it if we're currently inside a leveraged native-event stack
                 _default: function(event) {
-                    return jQuery.nodeName(event.target, "a");
+                    var target = event.target;
+                    return rcheckableType.test(target.type) &&
+                        target.click && nodeName(target, "input") &&
+                        dataPriv.get(target, "click") ||
+                        nodeName(target, "a");
                 }
             },
 
             beforeunload: {
                 postDispatch: function(event) {
 
                     // Support: Firefox 20+
                     // Firefox doesn't alert if the returnValue field is not set.
                     if (event.result !== undefined && event.originalEvent) {
                         event.originalEvent.returnValue = event.result;
                     }
                 }
             }
-        },
-
-        simulate: function(type, elem, event, bubble) {
-            // Piggyback on a donor event to simulate a different one.
-            // Fake originalEvent to avoid donor's stopPropagation, but if the
-            // simulated event prevents default then we do the same on the donor.
-            var e = jQuery.extend(
-                new jQuery.Event(),
-                event, {
-                    type: type,
-                    isSimulated: true,
-                    originalEvent: {}
-                }
-            );
-            if (bubble) {
-                jQuery.event.trigger(e, null, elem);
-            } else {
-                jQuery.event.dispatch.call(elem, e);
-            }
-            if (e.isDefaultPrevented()) {
-                event.preventDefault();
-            }
         }
     };
 
-    jQuery.removeEvent = document.removeEventListener ?
-        function(elem, type, handle) {
-            if (elem.removeEventListener) {
-                elem.removeEventListener(type, handle, false);
+    // Ensure the presence of an event listener that handles manually-triggered
+    // synthetic events by interrupting progress until reinvoked in response to
+    // *native* events that it fires directly, ensuring that state changes have
+    // already occurred before other listeners are invoked.
+    function leverageNative(el, type, expectSync) {
+
+        // Missing expectSync indicates a trigger call, which must force setup through jQuery.event.add
+        if (!expectSync) {
+            if (dataPriv.get(el, type) === undefined) {
+                jQuery.event.add(el, type, returnTrue);
             }
-        } :
-        function(elem, type, handle) {
-            var name = "on" + type;
+            return;
+        }
 
-            if (elem.detachEvent) {
+        // Register the controller as a special universal handler for all event namespaces
+        dataPriv.set(el, type, false);
+        jQuery.event.add(el, type, {
+            namespace: false,
+            handler: function(event) {
+                var notAsync, result,
+                    saved = dataPriv.get(this, type);
+
+                if ((event.isTrigger & 1) && this[type]) {
+
+                    // Interrupt processing of the outer synthetic .trigger()ed event
+                    // Saved data should be false in such cases, but might be a leftover capture object
+                    // from an async native handler (gh-4350)
+                    if (!saved.length) {
+
+                        // Store arguments for use when handling the inner native event
+                        // There will always be at least one argument (an event object), so this array
+                        // will not be confused with a leftover capture object.
+                        saved = slice.call(arguments);
+                        dataPriv.set(this, type, saved);
+
+                        // Trigger the native event and capture its result
+                        // Support: IE <=9 - 11+
+                        // focus() and blur() are asynchronous
+                        notAsync = expectSync(this, type);
+                        this[type]();
+                        result = dataPriv.get(this, type);
+                        if (saved !== result || notAsync) {
+                            dataPriv.set(this, type, false);
+                        } else {
+                            result = {};
+                        }
+                        if (saved !== result) {
 
-                // #8545, #7054, preventing memory leaks for custom events in IE6-8
-                // detachEvent needed property on element, by name of that event, to properly expose it to GC
-                if (typeof elem[name] === strundefined) {
-                    elem[name] = null;
-                }
+                            // Cancel the outer synthetic event
+                            event.stopImmediatePropagation();
+                            event.preventDefault();
+
+                            // Support: Chrome 86+
+                            // In Chrome, if an element having a focusout handler is blurred by
+                            // clicking outside of it, it invokes the handler synchronously. If
+                            // that handler calls `.remove()` on the element, the data is cleared,
+                            // leaving `result` undefined. We need to guard against this.
+                            return result && result.value;
+                        }
+
+                        // If this is an inner synthetic event for an event with a bubbling surrogate
+                        // (focus or blur), assume that the surrogate already propagated from triggering the
+                        // native event and prevent that from happening again here.
+                        // This technically gets the ordering wrong w.r.t. to `.trigger()` (in which the
+                        // bubbling surrogate propagates *after* the non-bubbling base), but that seems
+                        // less bad than duplication.
+                    } else if ((jQuery.event.special[type] || {}).delegateType) {
+                        event.stopPropagation();
+                    }
+
+                    // If this is a native event triggered above, everything is now in order
+                    // Fire an inner synthetic event with the original arguments
+                } else if (saved.length) {
+
+                    // ...and capture the result
+                    dataPriv.set(this, type, {
+                        value: jQuery.event.trigger(
+
+                            // Support: IE <=9 - 11+
+                            // Extend with the prototype to reset the above stopImmediatePropagation()
+                            jQuery.extend(saved[0], jQuery.Event.prototype),
+                            saved.slice(1),
+                            this
+                        )
+                    });
 
-                elem.detachEvent(name, handle);
+                    // Abort handling of the native event
+                    event.stopImmediatePropagation();
+                }
             }
-        };
+        });
+    }
+
+    jQuery.removeEvent = function(elem, type, handle) {
+
+        // This "if" is needed for plain objects
+        if (elem.removeEventListener) {
+            elem.removeEventListener(type, handle);
+        }
+    };
 
     jQuery.Event = function(src, props) {
+
         // Allow instantiation without the 'new' keyword
         if (!(this instanceof jQuery.Event)) {
             return new jQuery.Event(src, props);
         }
 
         // Event object
         if (src && src.type) {
             this.originalEvent = src;
             this.type = src.type;
 
             // Events bubbling up the document may have been marked as prevented
             // by a handler lower down the tree; reflect the correct value.
             this.isDefaultPrevented = src.defaultPrevented ||
                 src.defaultPrevented === undefined &&
-                // Support: IE < 9, Android < 4.0
+
+                // Support: Android <=2.3 only
                 src.returnValue === false ?
                 returnTrue :
                 returnFalse;
 
+            // Create target properties
+            // Support: Safari <=6 - 7 only
+            // Target should not be a text node (trac-504, trac-13143)
+            this.target = (src.target && src.target.nodeType === 3) ?
+                src.target.parentNode :
+                src.target;
+
+            this.currentTarget = src.currentTarget;
+            this.relatedTarget = src.relatedTarget;
+
             // Event type
         } else {
             this.type = src;
         }
 
         // Put explicitly provided properties onto the event object
         if (props) {
             jQuery.extend(this, props);
         }
 
         // Create a timestamp if incoming event doesn't have one
-        this.timeStamp = src && src.timeStamp || jQuery.now();
+        this.timeStamp = src && src.timeStamp || Date.now();
 
         // Mark it as fixed
         this[jQuery.expando] = true;
     };
 
     // jQuery.Event is based on DOM3 Events as specified by the ECMAScript Language Binding
-    // http://www.w3.org/TR/2003/WD-DOM-Level-3-Events-20030331/ecma-script-binding.html
+    // https://www.w3.org/TR/2003/WD-DOM-Level-3-Events-20030331/ecma-script-binding.html
     jQuery.Event.prototype = {
+        constructor: jQuery.Event,
         isDefaultPrevented: returnFalse,
         isPropagationStopped: returnFalse,
         isImmediatePropagationStopped: returnFalse,
+        isSimulated: false,
 
         preventDefault: function() {
             var e = this.originalEvent;
 
             this.isDefaultPrevented = returnTrue;
-            if (!e) {
-                return;
-            }
 
-            // If preventDefault exists, run it on the original event
-            if (e.preventDefault) {
+            if (e && !this.isSimulated) {
                 e.preventDefault();
-
-                // Support: IE
-                // Otherwise set the returnValue property of the original event to false
-            } else {
-                e.returnValue = false;
             }
         },
         stopPropagation: function() {
             var e = this.originalEvent;
 
             this.isPropagationStopped = returnTrue;
-            if (!e) {
-                return;
-            }
-            // If stopPropagation exists, run it on the original event
-            if (e.stopPropagation) {
+
+            if (e && !this.isSimulated) {
                 e.stopPropagation();
             }
-
-            // Support: IE
-            // Set the cancelBubble property of the original event to true
-            e.cancelBubble = true;
         },
         stopImmediatePropagation: function() {
             var e = this.originalEvent;
 
             this.isImmediatePropagationStopped = returnTrue;
 
-            if (e && e.stopImmediatePropagation) {
+            if (e && !this.isSimulated) {
                 e.stopImmediatePropagation();
             }
 
             this.stopPropagation();
         }
     };
 
+    // Includes all common event props including KeyEvent and MouseEvent specific props
+    jQuery.each({
+        altKey: true,
+        bubbles: true,
+        cancelable: true,
+        changedTouches: true,
+        ctrlKey: true,
+        detail: true,
+        eventPhase: true,
+        metaKey: true,
+        pageX: true,
+        pageY: true,
+        shiftKey: true,
+        view: true,
+        "char": true,
+        code: true,
+        charCode: true,
+        key: true,
+        keyCode: true,
+        button: true,
+        buttons: true,
+        clientX: true,
+        clientY: true,
+        offsetX: true,
+        offsetY: true,
+        pointerId: true,
+        pointerType: true,
+        screenX: true,
+        screenY: true,
+        targetTouches: true,
+        toElement: true,
+        touches: true,
+        which: true
+    }, jQuery.event.addProp);
+
+    jQuery.each({
+        focus: "focusin",
+        blur: "focusout"
+    }, function(type, delegateType) {
+        jQuery.event.special[type] = {
+
+            // Utilize native event if possible so blur/focus sequence is correct
+            setup: function() {
+
+                // Claim the first handler
+                // dataPriv.set( this, "focus", ... )
+                // dataPriv.set( this, "blur", ... )
+                leverageNative(this, type, expectSync);
+
+                // Return false to allow normal processing in the caller
+                return false;
+            },
+            trigger: function() {
+
+                // Force setup before trigger
+                leverageNative(this, type);
+
+                // Return non-false to allow normal event-path propagation
+                return true;
+            },
+
+            // Suppress native focus or blur if we're currently inside
+            // a leveraged native-event stack
+            _default: function(event) {
+                return dataPriv.get(event.target, type);
+            },
+
+            delegateType: delegateType
+        };
+    });
+
     // Create mouseenter/leave events using mouseover/out and event-time checks
+    // so that event delegation works in jQuery.
+    // Do the same for pointerenter/pointerleave and pointerover/pointerout
+    //
+    // Support: Safari 7 only
+    // Safari sends mouseenter too often; see:
+    // https://bugs.chromium.org/p/chromium/issues/detail?id=470258
+    // for the description of the bug (it existed in older Chrome versions as well).
     jQuery.each({
         mouseenter: "mouseover",
         mouseleave: "mouseout",
         pointerenter: "pointerover",
         pointerleave: "pointerout"
     }, function(orig, fix) {
         jQuery.event.special[orig] = {
@@ -5040,812 +5922,429 @@
 
             handle: function(event) {
                 var ret,
                     target = this,
                     related = event.relatedTarget,
                     handleObj = event.handleObj;
 
-                // For mousenter/leave call the handler if related is outside the target.
+                // For mouseenter/leave call the handler if related is outside the target.
                 // NB: No relatedTarget if the mouse left/entered the browser window
                 if (!related || (related !== target && !jQuery.contains(target, related))) {
                     event.type = handleObj.origType;
                     ret = handleObj.handler.apply(this, arguments);
                     event.type = fix;
                 }
                 return ret;
             }
         };
     });
 
-    // IE submit delegation
-    if (!support.submitBubbles) {
-
-        jQuery.event.special.submit = {
-            setup: function() {
-                // Only need this for delegated form submit events
-                if (jQuery.nodeName(this, "form")) {
-                    return false;
-                }
-
-                // Lazy-add a submit handler when a descendant form may potentially be submitted
-                jQuery.event.add(this, "click._submit keypress._submit", function(e) {
-                    // Node name check avoids a VML-related crash in IE (#9807)
-                    var elem = e.target,
-                        form = jQuery.nodeName(elem, "input") || jQuery.nodeName(elem, "button") ? elem.form : undefined;
-                    if (form && !jQuery._data(form, "submitBubbles")) {
-                        jQuery.event.add(form, "submit._submit", function(event) {
-                            event._submit_bubble = true;
-                        });
-                        jQuery._data(form, "submitBubbles", true);
-                    }
-                });
-                // return undefined since we don't need an event listener
-            },
-
-            postDispatch: function(event) {
-                // If form was submitted by the user, bubble the event up the tree
-                if (event._submit_bubble) {
-                    delete event._submit_bubble;
-                    if (this.parentNode && !event.isTrigger) {
-                        jQuery.event.simulate("submit", this.parentNode, event, true);
-                    }
-                }
-            },
-
-            teardown: function() {
-                // Only need this for delegated form submit events
-                if (jQuery.nodeName(this, "form")) {
-                    return false;
-                }
-
-                // Remove delegated handlers; cleanData eventually reaps submit handlers attached above
-                jQuery.event.remove(this, "._submit");
-            }
-        };
-    }
-
-    // IE change delegation and checkbox/radio fix
-    if (!support.changeBubbles) {
-
-        jQuery.event.special.change = {
-
-            setup: function() {
-
-                if (rformElems.test(this.nodeName)) {
-                    // IE doesn't fire change on a check/radio until blur; trigger it on click
-                    // after a propertychange. Eat the blur-change in special.change.handle.
-                    // This still fires onchange a second time for check/radio after blur.
-                    if (this.type === "checkbox" || this.type === "radio") {
-                        jQuery.event.add(this, "propertychange._change", function(event) {
-                            if (event.originalEvent.propertyName === "checked") {
-                                this._just_changed = true;
-                            }
-                        });
-                        jQuery.event.add(this, "click._change", function(event) {
-                            if (this._just_changed && !event.isTrigger) {
-                                this._just_changed = false;
-                            }
-                            // Allow triggered, simulated change events (#11500)
-                            jQuery.event.simulate("change", this, event, true);
-                        });
-                    }
-                    return false;
-                }
-                // Delegated event; lazy-add a change handler on descendant inputs
-                jQuery.event.add(this, "beforeactivate._change", function(e) {
-                    var elem = e.target;
-
-                    if (rformElems.test(elem.nodeName) && !jQuery._data(elem, "changeBubbles")) {
-                        jQuery.event.add(elem, "change._change", function(event) {
-                            if (this.parentNode && !event.isSimulated && !event.isTrigger) {
-                                jQuery.event.simulate("change", this.parentNode, event, true);
-                            }
-                        });
-                        jQuery._data(elem, "changeBubbles", true);
-                    }
-                });
-            },
-
-            handle: function(event) {
-                var elem = event.target;
-
-                // Swallow native change events from checkbox/radio, we already triggered them above
-                if (this !== elem || event.isSimulated || event.isTrigger || (elem.type !== "radio" && elem.type !== "checkbox")) {
-                    return event.handleObj.handler.apply(this, arguments);
-                }
-            },
-
-            teardown: function() {
-                jQuery.event.remove(this, "._change");
-
-                return !rformElems.test(this.nodeName);
-            }
-        };
-    }
-
-    // Create "bubbling" focus and blur events
-    if (!support.focusinBubbles) {
-        jQuery.each({
-            focus: "focusin",
-            blur: "focusout"
-        }, function(orig, fix) {
-
-            // Attach a single capturing handler on the document while someone wants focusin/focusout
-            var handler = function(event) {
-                jQuery.event.simulate(fix, event.target, jQuery.event.fix(event), true);
-            };
-
-            jQuery.event.special[fix] = {
-                setup: function() {
-                    var doc = this.ownerDocument || this,
-                        attaches = jQuery._data(doc, fix);
-
-                    if (!attaches) {
-                        doc.addEventListener(orig, handler, true);
-                    }
-                    jQuery._data(doc, fix, (attaches || 0) + 1);
-                },
-                teardown: function() {
-                    var doc = this.ownerDocument || this,
-                        attaches = jQuery._data(doc, fix) - 1;
-
-                    if (!attaches) {
-                        doc.removeEventListener(orig, handler, true);
-                        jQuery._removeData(doc, fix);
-                    } else {
-                        jQuery._data(doc, fix, attaches);
-                    }
-                }
-            };
-        });
-    }
-
     jQuery.fn.extend({
 
-        on: function(types, selector, data, fn, /*INTERNAL*/ one) {
-            var type, origFn;
-
-            // Types can be a map of types/handlers
-            if (typeof types === "object") {
-                // ( types-Object, selector, data )
-                if (typeof selector !== "string") {
-                    // ( types-Object, data )
-                    data = data || selector;
-                    selector = undefined;
-                }
-                for (type in types) {
-                    this.on(type, selector, data, types[type], one);
-                }
-                return this;
-            }
-
-            if (data == null && fn == null) {
-                // ( types, fn )
-                fn = selector;
-                data = selector = undefined;
-            } else if (fn == null) {
-                if (typeof selector === "string") {
-                    // ( types, selector, fn )
-                    fn = data;
-                    data = undefined;
-                } else {
-                    // ( types, data, fn )
-                    fn = data;
-                    data = selector;
-                    selector = undefined;
-                }
-            }
-            if (fn === false) {
-                fn = returnFalse;
-            } else if (!fn) {
-                return this;
-            }
-
-            if (one === 1) {
-                origFn = fn;
-                fn = function(event) {
-                    // Can use an empty set, since event contains the info
-                    jQuery().off(event);
-                    return origFn.apply(this, arguments);
-                };
-                // Use same guid so caller can remove using origFn
-                fn.guid = origFn.guid || (origFn.guid = jQuery.guid++);
-            }
-            return this.each(function() {
-                jQuery.event.add(this, types, fn, data, selector);
-            });
+        on: function(types, selector, data, fn) {
+            return on(this, types, selector, data, fn);
         },
         one: function(types, selector, data, fn) {
-            return this.on(types, selector, data, fn, 1);
+            return on(this, types, selector, data, fn, 1);
         },
         off: function(types, selector, fn) {
             var handleObj, type;
             if (types && types.preventDefault && types.handleObj) {
+
                 // ( event )  dispatched jQuery.Event
                 handleObj = types.handleObj;
                 jQuery(types.delegateTarget).off(
-                    handleObj.namespace ? handleObj.origType + "." + handleObj.namespace : handleObj.origType,
+                    handleObj.namespace ?
+                    handleObj.origType + "." + handleObj.namespace :
+                    handleObj.origType,
                     handleObj.selector,
                     handleObj.handler
                 );
                 return this;
             }
             if (typeof types === "object") {
+
                 // ( types-object [, selector] )
                 for (type in types) {
                     this.off(type, selector, types[type]);
                 }
                 return this;
             }
             if (selector === false || typeof selector === "function") {
+
                 // ( types [, fn] )
                 fn = selector;
                 selector = undefined;
             }
             if (fn === false) {
                 fn = returnFalse;
             }
             return this.each(function() {
                 jQuery.event.remove(this, types, fn, selector);
             });
-        },
-
-        trigger: function(type, data) {
-            return this.each(function() {
-                jQuery.event.trigger(type, data, this);
-            });
-        },
-        triggerHandler: function(type, data) {
-            var elem = this[0];
-            if (elem) {
-                return jQuery.event.trigger(type, data, elem, true);
-            }
         }
     });
 
 
-    function createSafeFragment(document) {
-        var list = nodeNames.split("|"),
-            safeFrag = document.createDocumentFragment();
-
-        if (safeFrag.createElement) {
-            while (list.length) {
-                safeFrag.createElement(
-                    list.pop()
-                );
-            }
-        }
-        return safeFrag;
-    }
+    var
+
+        // Support: IE <=10 - 11, Edge 12 - 13 only
+        // In IE/Edge using regex groups here causes severe slowdowns.
+        // See https://connect.microsoft.com/IE/feedback/details/1736512/
+        rnoInnerhtml = /<script|<style|<link/i,
 
-    var nodeNames = "abbr|article|aside|audio|bdi|canvas|data|datalist|details|figcaption|figure|footer|" +
-        "header|hgroup|mark|meter|nav|output|progress|section|summary|time|video",
-        rinlinejQuery = / jQuery\d+="(?:null|\d+)"/g,
-        rnoshimcache = new RegExp("<(?:" + nodeNames + ")[\\s/>]", "i"),
-        rleadingWhitespace = /^\s+/,
-        rxhtmlTag = /<(?!area|br|col|embed|hr|img|input|link|meta|param)(([\w:]+)[^>]*)\/>/gi,
-        rtagName = /<([\w:]+)/,
-        rtbody = /<tbody/i,
-        rhtml = /<|&#?\w+;/,
-        rnoInnerhtml = /<(?:script|style|link)/i,
         // checked="checked" or checked
         rchecked = /checked\s*(?:[^=]|=\s*.checked.)/i,
-        rscriptType = /^$|\/(?:java|ecma)script/i,
-        rscriptTypeMasked = /^true\/(.*)/,
-        rcleanScript = /^\s*<!(?:\[CDATA\[|--)|(?:\]\]|--)>\s*$/g,
-
-        // We have to close these tags to support XHTML (#13200)
-        wrapMap = {
-            option: [1, "<select multiple='multiple'>", "</select>"],
-            legend: [1, "<fieldset>", "</fieldset>"],
-            area: [1, "<map>", "</map>"],
-            param: [1, "<object>", "</object>"],
-            thead: [1, "<table>", "</table>"],
-            tr: [2, "<table><tbody>", "</tbody></table>"],
-            col: [2, "<table><tbody></tbody><colgroup>", "</colgroup></table>"],
-            td: [3, "<table><tbody><tr>", "</tr></tbody></table>"],
-
-            // IE6-8 can't serialize link, script, style, or any html5 (NoScope) tags,
-            // unless wrapped in a div with non-breaking characters in front of it.
-            _default: support.htmlSerialize ? [0, "", ""] : [1, "X<div>", "</div>"]
-        },
-        safeFragment = createSafeFragment(document),
-        fragmentDiv = safeFragment.appendChild(document.createElement("div"));
 
-    wrapMap.optgroup = wrapMap.option;
-    wrapMap.tbody = wrapMap.tfoot = wrapMap.colgroup = wrapMap.caption = wrapMap.thead;
-    wrapMap.th = wrapMap.td;
-
-    function getAll(context, tag) {
-        var elems, elem,
-            i = 0,
-            found = typeof context.getElementsByTagName !== strundefined ? context.getElementsByTagName(tag || "*") :
-            typeof context.querySelectorAll !== strundefined ? context.querySelectorAll(tag || "*") :
-            undefined;
-
-        if (!found) {
-            for (found = [], elems = context.childNodes || context;
-                (elem = elems[i]) != null; i++) {
-                if (!tag || jQuery.nodeName(elem, tag)) {
-                    found.push(elem);
-                } else {
-                    jQuery.merge(found, getAll(elem, tag));
-                }
-            }
-        }
+        rcleanScript = /^\s*<!\[CDATA\[|\]\]>\s*$/g;
 
-        return tag === undefined || tag && jQuery.nodeName(context, tag) ?
-            jQuery.merge([context], found) :
-            found;
-    }
+    // Prefer a tbody over its parent table for containing new rows
+    function manipulationTarget(elem, content) {
+        if (nodeName(elem, "table") &&
+            nodeName(content.nodeType !== 11 ? content : content.firstChild, "tr")) {
 
-    // Used in buildFragment, fixes the defaultChecked property
-    function fixDefaultChecked(elem) {
-        if (rcheckableType.test(elem.type)) {
-            elem.defaultChecked = elem.checked;
+            return jQuery(elem).children("tbody")[0] || elem;
         }
-    }
 
-    // Support: IE<8
-    // Manipulating tables requires a tbody
-    function manipulationTarget(elem, content) {
-        return jQuery.nodeName(elem, "table") &&
-            jQuery.nodeName(content.nodeType !== 11 ? content : content.firstChild, "tr") ?
-
-            elem.getElementsByTagName("tbody")[0] ||
-            elem.appendChild(elem.ownerDocument.createElement("tbody")) :
-            elem;
+        return elem;
     }
 
     // Replace/restore the type attribute of script elements for safe DOM manipulation
     function disableScript(elem) {
-        elem.type = (jQuery.find.attr(elem, "type") !== null) + "/" + elem.type;
+        elem.type = (elem.getAttribute("type") !== null) + "/" + elem.type;
         return elem;
     }
 
     function restoreScript(elem) {
-        var match = rscriptTypeMasked.exec(elem.type);
-        if (match) {
-            elem.type = match[1];
+        if ((elem.type || "").slice(0, 5) === "true/") {
+            elem.type = elem.type.slice(5);
         } else {
             elem.removeAttribute("type");
         }
-        return elem;
-    }
 
-    // Mark scripts as having already been evaluated
-    function setGlobalEval(elems, refElements) {
-        var elem,
-            i = 0;
-        for (;
-            (elem = elems[i]) != null; i++) {
-            jQuery._data(elem, "globalEval", !refElements || jQuery._data(refElements[i], "globalEval"));
-        }
+        return elem;
     }
 
     function cloneCopyEvent(src, dest) {
+        var i, l, type, pdataOld, udataOld, udataCur, events;
 
-        if (dest.nodeType !== 1 || !jQuery.hasData(src)) {
+        if (dest.nodeType !== 1) {
             return;
         }
 
-        var type, i, l,
-            oldData = jQuery._data(src),
-            curData = jQuery._data(dest, oldData),
-            events = oldData.events;
+        // 1. Copy private data: events, handlers, etc.
+        if (dataPriv.hasData(src)) {
+            pdataOld = dataPriv.get(src);
+            events = pdataOld.events;
 
-        if (events) {
-            delete curData.handle;
-            curData.events = {};
+            if (events) {
+                dataPriv.remove(dest, "handle events");
 
-            for (type in events) {
-                for (i = 0, l = events[type].length; i < l; i++) {
-                    jQuery.event.add(dest, type, events[type][i]);
+                for (type in events) {
+                    for (i = 0, l = events[type].length; i < l; i++) {
+                        jQuery.event.add(dest, type, events[type][i]);
+                    }
                 }
             }
         }
 
-        // make the cloned public data object a copy from the original
-        if (curData.data) {
-            curData.data = jQuery.extend({}, curData.data);
+        // 2. Copy user data
+        if (dataUser.hasData(src)) {
+            udataOld = dataUser.access(src);
+            udataCur = jQuery.extend({}, udataOld);
+
+            dataUser.set(dest, udataCur);
         }
     }
 
-    function fixCloneNodeIssues(src, dest) {
-        var nodeName, e, data;
+    // Fix IE bugs, see support tests
+    function fixInput(src, dest) {
+        var nodeName = dest.nodeName.toLowerCase();
 
-        // We do not need to do anything for non-Elements
-        if (dest.nodeType !== 1) {
-            return;
-        }
+        // Fails to persist the checked state of a cloned checkbox or radio button.
+        if (nodeName === "input" && rcheckableType.test(src.type)) {
+            dest.checked = src.checked;
 
-        nodeName = dest.nodeName.toLowerCase();
+            // Fails to return the selected option to the default selected state when cloning options
+        } else if (nodeName === "input" || nodeName === "textarea") {
+            dest.defaultValue = src.defaultValue;
+        }
+    }
 
-        // IE6-8 copies events bound via attachEvent when using cloneNode.
-        if (!support.noCloneEvent && dest[jQuery.expando]) {
-            data = jQuery._data(dest);
+    function domManip(collection, args, callback, ignored) {
 
-            for (e in data.events) {
-                jQuery.removeEvent(dest, e, data.handle);
-            }
+        // Flatten any nested arrays
+        args = flat(args);
 
-            // Event data gets referenced instead of copied if the expando gets copied too
-            dest.removeAttribute(jQuery.expando);
+        var fragment, first, scripts, hasScripts, node, doc,
+            i = 0,
+            l = collection.length,
+            iNoClone = l - 1,
+            value = args[0],
+            valueIsFunction = isFunction(value);
+
+        // We can't cloneNode fragments that contain checked, in WebKit
+        if (valueIsFunction ||
+            (l > 1 && typeof value === "string" &&
+                !support.checkClone && rchecked.test(value))) {
+            return collection.each(function(index) {
+                var self = collection.eq(index);
+                if (valueIsFunction) {
+                    args[0] = value.call(this, index, self.html());
+                }
+                domManip(self, args, callback, ignored);
+            });
         }
 
-        // IE blanks contents when cloning scripts, and tries to evaluate newly-set text
-        if (nodeName === "script" && dest.text !== src.text) {
-            disableScript(dest).text = src.text;
-            restoreScript(dest);
+        if (l) {
+            fragment = buildFragment(args, collection[0].ownerDocument, false, collection, ignored);
+            first = fragment.firstChild;
 
-            // IE6-10 improperly clones children of object elements using classid.
-            // IE10 throws NoModificationAllowedError if parent is null, #12132.
-        } else if (nodeName === "object") {
-            if (dest.parentNode) {
-                dest.outerHTML = src.outerHTML;
+            if (fragment.childNodes.length === 1) {
+                fragment = first;
             }
 
-            // This path appears unavoidable for IE9. When cloning an object
-            // element in IE9, the outerHTML strategy above is not sufficient.
-            // If the src has innerHTML and the destination does not,
-            // copy the src.innerHTML into the dest.innerHTML. #10324
-            if (support.html5Clone && (src.innerHTML && !jQuery.trim(dest.innerHTML))) {
-                dest.innerHTML = src.innerHTML;
-            }
+            // Require either new content or an interest in ignored elements to invoke the callback
+            if (first || ignored) {
+                scripts = jQuery.map(getAll(fragment, "script"), disableScript);
+                hasScripts = scripts.length;
 
-        } else if (nodeName === "input" && rcheckableType.test(src.type)) {
-            // IE6-8 fails to persist the checked state of a cloned checkbox
-            // or radio button. Worse, IE6-7 fail to give the cloned element
-            // a checked appearance if the defaultChecked value isn't also set
+                // Use the original fragment for the last item
+                // instead of the first because it can end up
+                // being emptied incorrectly in certain situations (trac-8070).
+                for (; i < l; i++) {
+                    node = fragment;
 
-            dest.defaultChecked = dest.checked = src.checked;
+                    if (i !== iNoClone) {
+                        node = jQuery.clone(node, true, true);
 
-            // IE6-7 get confused and end up setting the value of a cloned
-            // checkbox/radio button to an empty string instead of "on"
-            if (dest.value !== src.value) {
-                dest.value = src.value;
-            }
+                        // Keep references to cloned scripts for later restoration
+                        if (hasScripts) {
 
-            // IE6-8 fails to return the selected option to the default selected
-            // state when cloning options
-        } else if (nodeName === "option") {
-            dest.defaultSelected = dest.selected = src.defaultSelected;
+                            // Support: Android <=4.0 only, PhantomJS 1 only
+                            // push.apply(_, arraylike) throws on ancient WebKit
+                            jQuery.merge(scripts, getAll(node, "script"));
+                        }
+                    }
 
-            // IE6-8 fails to set the defaultValue to the correct value when
-            // cloning other types of input fields
-        } else if (nodeName === "input" || nodeName === "textarea") {
-            dest.defaultValue = src.defaultValue;
+                    callback.call(collection[i], node, i);
+                }
+
+                if (hasScripts) {
+                    doc = scripts[scripts.length - 1].ownerDocument;
+
+                    // Reenable scripts
+                    jQuery.map(scripts, restoreScript);
+
+                    // Evaluate executable scripts on first document insertion
+                    for (i = 0; i < hasScripts; i++) {
+                        node = scripts[i];
+                        if (rscriptType.test(node.type || "") &&
+                            !dataPriv.access(node, "globalEval") &&
+                            jQuery.contains(doc, node)) {
+
+                            if (node.src && (node.type || "").toLowerCase() !== "module") {
+
+                                // Optional AJAX dependency, but won't run scripts if not present
+                                if (jQuery._evalUrl && !node.noModule) {
+                                    jQuery._evalUrl(node.src, {
+                                        nonce: node.nonce || node.getAttribute("nonce")
+                                    }, doc);
+                                }
+                            } else {
+
+                                // Unwrap a CDATA section containing script contents. This shouldn't be
+                                // needed as in XML documents they're already not visible when
+                                // inspecting element contents and in HTML documents they have no
+                                // meaning but we're preserving that logic for backwards compatibility.
+                                // This will be removed completely in 4.0. See gh-4904.
+                                DOMEval(node.textContent.replace(rcleanScript, ""), node, doc);
+                            }
+                        }
+                    }
+                }
+            }
         }
+
+        return collection;
     }
 
-    jQuery.extend({
-        clone: function(elem, dataAndEvents, deepDataAndEvents) {
-            var destElements, node, clone, i, srcElements,
-                inPage = jQuery.contains(elem.ownerDocument, elem);
+    function remove(elem, selector, keepData) {
+        var node,
+            nodes = selector ? jQuery.filter(selector, elem) : elem,
+            i = 0;
 
-            if (support.html5Clone || jQuery.isXMLDoc(elem) || !rnoshimcache.test("<" + elem.nodeName + ">")) {
-                clone = elem.cloneNode(true);
+        for (;
+            (node = nodes[i]) != null; i++) {
+            if (!keepData && node.nodeType === 1) {
+                jQuery.cleanData(getAll(node));
+            }
 
-                // IE<=8 does not properly clone detached, unknown element nodes
-            } else {
-                fragmentDiv.innerHTML = elem.outerHTML;
-                fragmentDiv.removeChild(clone = fragmentDiv.firstChild);
+            if (node.parentNode) {
+                if (keepData && isAttached(node)) {
+                    setGlobalEval(getAll(node, "script"));
+                }
+                node.parentNode.removeChild(node);
             }
+        }
+
+        return elem;
+    }
+
+    jQuery.extend({
+        htmlPrefilter: function(html) {
+            return html;
+        },
 
-            if ((!support.noCloneEvent || !support.noCloneChecked) &&
-                (elem.nodeType === 1 || elem.nodeType === 11) && !jQuery.isXMLDoc(elem)) {
+        clone: function(elem, dataAndEvents, deepDataAndEvents) {
+            var i, l, srcElements, destElements,
+                clone = elem.cloneNode(true),
+                inPage = isAttached(elem);
+
+            // Fix IE cloning issues
+            if (!support.noCloneChecked && (elem.nodeType === 1 || elem.nodeType === 11) &&
+                !jQuery.isXMLDoc(elem)) {
 
-                // We eschew Sizzle here for performance reasons: http://jsperf.com/getall-vs-sizzle/2
+                // We eschew Sizzle here for performance reasons: https://jsperf.com/getall-vs-sizzle/2
                 destElements = getAll(clone);
                 srcElements = getAll(elem);
 
-                // Fix all IE cloning issues
-                for (i = 0;
-                    (node = srcElements[i]) != null; ++i) {
-                    // Ensure that the destination node is not null; Fixes #9587
-                    if (destElements[i]) {
-                        fixCloneNodeIssues(node, destElements[i]);
-                    }
+                for (i = 0, l = srcElements.length; i < l; i++) {
+                    fixInput(srcElements[i], destElements[i]);
                 }
             }
 
             // Copy the events from the original to the clone
             if (dataAndEvents) {
                 if (deepDataAndEvents) {
                     srcElements = srcElements || getAll(elem);
                     destElements = destElements || getAll(clone);
 
-                    for (i = 0;
-                        (node = srcElements[i]) != null; i++) {
-                        cloneCopyEvent(node, destElements[i]);
+                    for (i = 0, l = srcElements.length; i < l; i++) {
+                        cloneCopyEvent(srcElements[i], destElements[i]);
                     }
                 } else {
                     cloneCopyEvent(elem, clone);
                 }
             }
 
             // Preserve script evaluation history
             destElements = getAll(clone, "script");
             if (destElements.length > 0) {
                 setGlobalEval(destElements, !inPage && getAll(elem, "script"));
             }
 
-            destElements = srcElements = node = null;
-
             // Return the cloned set
             return clone;
         },
 
-        buildFragment: function(elems, context, scripts, selection) {
-            var j, elem, contains,
-                tmp, tag, tbody, wrap,
-                l = elems.length,
-
-                // Ensure a safe fragment
-                safe = createSafeFragment(context),
-
-                nodes = [],
+        cleanData: function(elems) {
+            var data, elem, type,
+                special = jQuery.event.special,
                 i = 0;
 
-            for (; i < l; i++) {
-                elem = elems[i];
-
-                if (elem || elem === 0) {
-
-                    // Add nodes directly
-                    if (jQuery.type(elem) === "object") {
-                        jQuery.merge(nodes, elem.nodeType ? [elem] : elem);
-
-                        // Convert non-html into a text node
-                    } else if (!rhtml.test(elem)) {
-                        nodes.push(context.createTextNode(elem));
-
-                        // Convert html into DOM nodes
-                    } else {
-                        tmp = tmp || safe.appendChild(context.createElement("div"));
-
-                        // Deserialize a standard representation
-                        tag = (rtagName.exec(elem) || ["", ""])[1].toLowerCase();
-                        wrap = wrapMap[tag] || wrapMap._default;
-
-                        tmp.innerHTML = wrap[1] + elem.replace(rxhtmlTag, "<$1></$2>") + wrap[2];
-
-                        // Descend through wrappers to the right content
-                        j = wrap[0];
-                        while (j--) {
-                            tmp = tmp.lastChild;
-                        }
-
-                        // Manually add leading whitespace removed by IE
-                        if (!support.leadingWhitespace && rleadingWhitespace.test(elem)) {
-                            nodes.push(context.createTextNode(rleadingWhitespace.exec(elem)[0]));
-                        }
-
-                        // Remove IE's autoinserted <tbody> from table fragments
-                        if (!support.tbody) {
-
-                            // String was a <table>, *may* have spurious <tbody>
-                            elem = tag === "table" && !rtbody.test(elem) ?
-                                tmp.firstChild :
-
-                                // String was a bare <thead> or <tfoot>
-                                wrap[1] === "<table>" && !rtbody.test(elem) ?
-                                tmp :
-                                0;
-
-                            j = elem && elem.childNodes.length;
-                            while (j--) {
-                                if (jQuery.nodeName((tbody = elem.childNodes[j]), "tbody") && !tbody.childNodes.length) {
-                                    elem.removeChild(tbody);
-                                }
-                            }
-                        }
-
-                        jQuery.merge(nodes, tmp.childNodes);
-
-                        // Fix #12392 for WebKit and IE > 9
-                        tmp.textContent = "";
-
-                        // Fix #12392 for oldIE
-                        while (tmp.firstChild) {
-                            tmp.removeChild(tmp.firstChild);
-                        }
-
-                        // Remember the top-level container for proper cleanup
-                        tmp = safe.lastChild;
-                    }
-                }
-            }
-
-            // Fix #11356: Clear elements from fragment
-            if (tmp) {
-                safe.removeChild(tmp);
-            }
-
-            // Reset defaultChecked for any radios and checkboxes
-            // about to be appended to the DOM in IE 6/7 (#8060)
-            if (!support.appendChecked) {
-                jQuery.grep(getAll(nodes, "input"), fixDefaultChecked);
-            }
-
-            i = 0;
-            while ((elem = nodes[i++])) {
-
-                // #4087 - If origin and destination elements are the same, and this is
-                // that element, do not do anything
-                if (selection && jQuery.inArray(elem, selection) !== -1) {
-                    continue;
-                }
-
-                contains = jQuery.contains(elem.ownerDocument, elem);
-
-                // Append to fragment
-                tmp = getAll(safe.appendChild(elem), "script");
-
-                // Preserve script evaluation history
-                if (contains) {
-                    setGlobalEval(tmp);
-                }
-
-                // Capture executables
-                if (scripts) {
-                    j = 0;
-                    while ((elem = tmp[j++])) {
-                        if (rscriptType.test(elem.type || "")) {
-                            scripts.push(elem);
-                        }
-                    }
-                }
-            }
-
-            tmp = null;
-
-            return safe;
-        },
-
-        cleanData: function(elems, /* internal */ acceptData) {
-            var elem, type, id, data,
-                i = 0,
-                internalKey = jQuery.expando,
-                cache = jQuery.cache,
-                deleteExpando = support.deleteExpando,
-                special = jQuery.event.special;
-
             for (;
-                (elem = elems[i]) != null; i++) {
-                if (acceptData || jQuery.acceptData(elem)) {
-
-                    id = elem[internalKey];
-                    data = id && cache[id];
-
-                    if (data) {
+                (elem = elems[i]) !== undefined; i++) {
+                if (acceptData(elem)) {
+                    if ((data = elem[dataPriv.expando])) {
                         if (data.events) {
                             for (type in data.events) {
                                 if (special[type]) {
                                     jQuery.event.remove(elem, type);
 
                                     // This is a shortcut to avoid jQuery.event.remove's overhead
                                 } else {
                                     jQuery.removeEvent(elem, type, data.handle);
                                 }
                             }
                         }
 
-                        // Remove cache only if it was not already removed by jQuery.event.remove
-                        if (cache[id]) {
-
-                            delete cache[id];
-
-                            // IE does not allow us to delete expando properties from nodes,
-                            // nor does it have a removeAttribute function on Document nodes;
-                            // we must handle all of these cases
-                            if (deleteExpando) {
-                                delete elem[internalKey];
-
-                            } else if (typeof elem.removeAttribute !== strundefined) {
-                                elem.removeAttribute(internalKey);
-
-                            } else {
-                                elem[internalKey] = null;
-                            }
-
-                            deletedIds.push(id);
-                        }
+                        // Support: Chrome <=35 - 45+
+                        // Assign undefined instead of using delete, see Data#remove
+                        elem[dataPriv.expando] = undefined;
+                    }
+                    if (elem[dataUser.expando]) {
+
+                        // Support: Chrome <=35 - 45+
+                        // Assign undefined instead of using delete, see Data#remove
+                        elem[dataUser.expando] = undefined;
                     }
                 }
             }
         }
     });
 
     jQuery.fn.extend({
+        detach: function(selector) {
+            return remove(this, selector, true);
+        },
+
+        remove: function(selector) {
+            return remove(this, selector);
+        },
+
         text: function(value) {
             return access(this, function(value) {
                 return value === undefined ?
                     jQuery.text(this) :
-                    this.empty().append((this[0] && this[0].ownerDocument || document).createTextNode(value));
+                    this.empty().each(function() {
+                        if (this.nodeType === 1 || this.nodeType === 11 || this.nodeType === 9) {
+                            this.textContent = value;
+                        }
+                    });
             }, null, value, arguments.length);
         },
 
         append: function() {
-            return this.domManip(arguments, function(elem) {
+            return domManip(this, arguments, function(elem) {
                 if (this.nodeType === 1 || this.nodeType === 11 || this.nodeType === 9) {
                     var target = manipulationTarget(this, elem);
                     target.appendChild(elem);
                 }
             });
         },
 
         prepend: function() {
-            return this.domManip(arguments, function(elem) {
+            return domManip(this, arguments, function(elem) {
                 if (this.nodeType === 1 || this.nodeType === 11 || this.nodeType === 9) {
                     var target = manipulationTarget(this, elem);
                     target.insertBefore(elem, target.firstChild);
                 }
             });
         },
 
         before: function() {
-            return this.domManip(arguments, function(elem) {
+            return domManip(this, arguments, function(elem) {
                 if (this.parentNode) {
                     this.parentNode.insertBefore(elem, this);
                 }
             });
         },
 
         after: function() {
-            return this.domManip(arguments, function(elem) {
+            return domManip(this, arguments, function(elem) {
                 if (this.parentNode) {
                     this.parentNode.insertBefore(elem, this.nextSibling);
                 }
             });
         },
 
-        remove: function(selector, keepData /* Internal Use Only */ ) {
-            var elem,
-                elems = selector ? jQuery.filter(selector, this) : this,
-                i = 0;
-
-            for (;
-                (elem = elems[i]) != null; i++) {
-
-                if (!keepData && elem.nodeType === 1) {
-                    jQuery.cleanData(getAll(elem));
-                }
-
-                if (elem.parentNode) {
-                    if (keepData && jQuery.contains(elem.ownerDocument, elem)) {
-                        setGlobalEval(getAll(elem, "script"));
-                    }
-                    elem.parentNode.removeChild(elem);
-                }
-            }
-
-            return this;
-        },
-
         empty: function() {
             var elem,
                 i = 0;
 
             for (;
                 (elem = this[i]) != null; i++) {
-                // Remove element nodes and prevent memory leaks
                 if (elem.nodeType === 1) {
-                    jQuery.cleanData(getAll(elem, false));
-                }
 
-                // Remove any remaining nodes
-                while (elem.firstChild) {
-                    elem.removeChild(elem.firstChild);
-                }
+                    // Prevent memory leaks
+                    jQuery.cleanData(getAll(elem, false));
 
-                // If this is a select, ensure that it displays empty (#12336)
-                // Support: IE<9
-                if (elem.options && jQuery.nodeName(elem, "select")) {
-                    elem.options.length = 0;
+                    // Remove any remaining nodes
+                    elem.textContent = "";
                 }
             }
 
             return this;
         },
 
         clone: function(dataAndEvents, deepDataAndEvents) {
@@ -5859,32 +6358,29 @@
 
         html: function(value) {
             return access(this, function(value) {
                 var elem = this[0] || {},
                     i = 0,
                     l = this.length;
 
-                if (value === undefined) {
-                    return elem.nodeType === 1 ?
-                        elem.innerHTML.replace(rinlinejQuery, "") :
-                        undefined;
+                if (value === undefined && elem.nodeType === 1) {
+                    return elem.innerHTML;
                 }
 
                 // See if we can take a shortcut and just use innerHTML
                 if (typeof value === "string" && !rnoInnerhtml.test(value) &&
-                    (support.htmlSerialize || !rnoshimcache.test(value)) &&
-                    (support.leadingWhitespace || !rleadingWhitespace.test(value)) &&
                     !wrapMap[(rtagName.exec(value) || ["", ""])[1].toLowerCase()]) {
 
-                    value = value.replace(rxhtmlTag, "<$1></$2>");
+                    value = jQuery.htmlPrefilter(value);
 
                     try {
                         for (; i < l; i++) {
-                            // Remove element nodes and prevent memory leaks
                             elem = this[i] || {};
+
+                            // Remove element nodes and prevent memory leaks
                             if (elem.nodeType === 1) {
                                 jQuery.cleanData(getAll(elem, false));
                                 elem.innerHTML = value;
                             }
                         }
 
                         elem = 0;
@@ -5896,975 +6392,786 @@
                 if (elem) {
                     this.empty().append(value);
                 }
             }, null, value, arguments.length);
         },
 
         replaceWith: function() {
-            var arg = arguments[0];
-
-            // Make the changes, replacing each context element with the new content
-            this.domManip(arguments, function(elem) {
-                arg = this.parentNode;
-
-                jQuery.cleanData(getAll(this));
-
-                if (arg) {
-                    arg.replaceChild(elem, this);
-                }
-            });
-
-            // Force removal if there was no new content (e.g., from empty arguments)
-            return arg && (arg.length || arg.nodeType) ? this : this.remove();
-        },
-
-        detach: function(selector) {
-            return this.remove(selector, true);
-        },
-
-        domManip: function(args, callback) {
-
-            // Flatten any nested arrays
-            args = concat.apply([], args);
-
-            var first, node, hasScripts,
-                scripts, doc, fragment,
-                i = 0,
-                l = this.length,
-                set = this,
-                iNoClone = l - 1,
-                value = args[0],
-                isFunction = jQuery.isFunction(value);
-
-            // We can't cloneNode fragments that contain checked, in WebKit
-            if (isFunction ||
-                (l > 1 && typeof value === "string" &&
-                    !support.checkClone && rchecked.test(value))) {
-                return this.each(function(index) {
-                    var self = set.eq(index);
-                    if (isFunction) {
-                        args[0] = value.call(this, index, self.html());
-                    }
-                    self.domManip(args, callback);
-                });
-            }
-
-            if (l) {
-                fragment = jQuery.buildFragment(args, this[0].ownerDocument, false, this);
-                first = fragment.firstChild;
-
-                if (fragment.childNodes.length === 1) {
-                    fragment = first;
-                }
+            var ignored = [];
 
-                if (first) {
-                    scripts = jQuery.map(getAll(fragment, "script"), disableScript);
-                    hasScripts = scripts.length;
+            // Make the changes, replacing each non-ignored context element with the new content
+            return domManip(this, arguments, function(elem) {
+                var parent = this.parentNode;
 
-                    // Use the original fragment for the last item instead of the first because it can end up
-                    // being emptied incorrectly in certain situations (#8070).
-                    for (; i < l; i++) {
-                        node = fragment;
-
-                        if (i !== iNoClone) {
-                            node = jQuery.clone(node, true, true);
-
-                            // Keep references to cloned scripts for later restoration
-                            if (hasScripts) {
-                                jQuery.merge(scripts, getAll(node, "script"));
-                            }
-                        }
-
-                        callback.call(this[i], node, i);
-                    }
-
-                    if (hasScripts) {
-                        doc = scripts[scripts.length - 1].ownerDocument;
-
-                        // Reenable scripts
-                        jQuery.map(scripts, restoreScript);
-
-                        // Evaluate executable scripts on first document insertion
-                        for (i = 0; i < hasScripts; i++) {
-                            node = scripts[i];
-                            if (rscriptType.test(node.type || "") &&
-                                !jQuery._data(node, "globalEval") && jQuery.contains(doc, node)) {
-
-                                if (node.src) {
-                                    // Optional AJAX dependency, but won't run scripts if not present
-                                    if (jQuery._evalUrl) {
-                                        jQuery._evalUrl(node.src);
-                                    }
-                                } else {
-                                    jQuery.globalEval((node.text || node.textContent || node.innerHTML || "").replace(rcleanScript, ""));
-                                }
-                            }
-                        }
+                if (jQuery.inArray(this, ignored) < 0) {
+                    jQuery.cleanData(getAll(this));
+                    if (parent) {
+                        parent.replaceChild(elem, this);
                     }
-
-                    // Fix #11809: Avoid leaking memory
-                    fragment = first = null;
                 }
-            }
 
-            return this;
+                // Force callback invocation
+            }, ignored);
         }
     });
 
     jQuery.each({
         appendTo: "append",
         prependTo: "prepend",
         insertBefore: "before",
         insertAfter: "after",
         replaceAll: "replaceWith"
     }, function(name, original) {
         jQuery.fn[name] = function(selector) {
             var elems,
-                i = 0,
                 ret = [],
                 insert = jQuery(selector),
-                last = insert.length - 1;
+                last = insert.length - 1,
+                i = 0;
 
             for (; i <= last; i++) {
                 elems = i === last ? this : this.clone(true);
                 jQuery(insert[i])[original](elems);
 
-                // Modern browsers can apply jQuery collections as arrays, but oldIE needs a .get()
+                // Support: Android <=4.0 only, PhantomJS 1 only
+                // .get() because push.apply(_, arraylike) throws on ancient WebKit
                 push.apply(ret, elems.get());
             }
 
             return this.pushStack(ret);
         };
     });
+    var rnumnonpx = new RegExp("^(" + pnum + ")(?!px)[a-z%]+$", "i");
 
+    var rcustomProp = /^--/;
 
-    var iframe,
-        elemdisplay = {};
 
-    /**
-     * Retrieve the actual display of a element
-     * @param {String} name nodeName of the element
-     * @param {Object} doc Document object
-     */
-    // Called only from within defaultDisplay
-    function actualDisplay(name, doc) {
-        var style,
-            elem = jQuery(doc.createElement(name)).appendTo(doc.body),
-
-            // getDefaultComputedStyle might be reliably used only on attached element
-            display = window.getDefaultComputedStyle && (style = window.getDefaultComputedStyle(elem[0])) ?
-
-            // Use of this method is a temporary fix (more like optmization) until something better comes along,
-            // since it was removed from specification and supported only in FF
-            style.display : jQuery.css(elem[0], "display");
-
-        // We don't have any data stored on the element,
-        // so use "detach" method as fast way to get rid of the element
-        elem.detach();
+    var getStyles = function(elem) {
 
-        return display;
-    }
+        // Support: IE <=11 only, Firefox <=30 (trac-15098, trac-14150)
+        // IE throws on elements created in popups
+        // FF meanwhile throws on frame elements through "defaultView.getComputedStyle"
+        var view = elem.ownerDocument.defaultView;
 
-    /**
-     * Try to determine the default display value of an element
-     * @param {String} nodeName
-     */
-    function defaultDisplay(nodeName) {
-        var doc = document,
-            display = elemdisplay[nodeName];
+        if (!view || !view.opener) {
+            view = window;
+        }
 
-        if (!display) {
-            display = actualDisplay(nodeName, doc);
+        return view.getComputedStyle(elem);
+    };
 
-            // If the simple way fails, read from inside an iframe
-            if (display === "none" || !display) {
+    var swap = function(elem, options, callback) {
+        var ret, name,
+            old = {};
 
-                // Use the already-created iframe if possible
-                iframe = (iframe || jQuery("<iframe frameborder='0' width='0' height='0'/>")).appendTo(doc.documentElement);
+        // Remember the old values, and insert the new ones
+        for (name in options) {
+            old[name] = elem.style[name];
+            elem.style[name] = options[name];
+        }
 
-                // Always write a new HTML skeleton so Webkit and Firefox don't choke on reuse
-                doc = (iframe[0].contentWindow || iframe[0].contentDocument).document;
+        ret = callback.call(elem);
 
-                // Support: IE
-                doc.write();
-                doc.close();
+        // Revert the old values
+        for (name in options) {
+            elem.style[name] = old[name];
+        }
 
-                display = actualDisplay(nodeName, doc);
-                iframe.detach();
-            }
+        return ret;
+    };
 
-            // Store the correct default display
-            elemdisplay[nodeName] = display;
-        }
 
-        return display;
-    }
+    var rboxStyle = new RegExp(cssExpand.join("|"), "i");
 
+    var whitespace = "[\\x20\\t\\r\\n\\f]";
 
-    (function() {
-        var shrinkWrapBlocksVal;
 
-        support.shrinkWrapBlocks = function() {
-            if (shrinkWrapBlocksVal != null) {
-                return shrinkWrapBlocksVal;
-            }
+    var rtrimCSS = new RegExp(
+        "^" + whitespace + "+|((?:^|[^\\\\])(?:\\\\.)*)" + whitespace + "+$",
+        "g"
+    );
 
-            // Will be changed later if needed.
-            shrinkWrapBlocksVal = false;
 
-            // Minified: var b,c,d
-            var div, body, container;
 
-            body = document.getElementsByTagName("body")[0];
-            if (!body || !body.style) {
-                // Test fired too early or in an unsupported environment, exit.
-                return;
-            }
 
-            // Setup
-            div = document.createElement("div");
-            container = document.createElement("div");
-            container.style.cssText = "position:absolute;border:0;width:0;height:0;top:0;left:-9999px";
-            body.appendChild(container).appendChild(div);
-
-            // Support: IE6
-            // Check if elements with layout shrink-wrap their children
-            if (typeof div.style.zoom !== strundefined) {
-                // Reset CSS: box-sizing; display; margin; border
-                div.style.cssText =
-                    // Support: Firefox<29, Android 2.3
-                    // Vendor-prefix box-sizing
-                    "-webkit-box-sizing:content-box;-moz-box-sizing:content-box;" +
-                    "box-sizing:content-box;display:block;margin:0;border:0;" +
-                    "padding:1px;width:1px;zoom:1";
-                div.appendChild(document.createElement("div")).style.width = "5px";
-                shrinkWrapBlocksVal = div.offsetWidth !== 3;
-            }
+    (function() {
 
-            body.removeChild(container);
+        // Executing both pixelPosition & boxSizingReliable tests require only one layout
+        // so they're executed at the same time to save the second computation.
+        function computeStyleTests() {
 
-            return shrinkWrapBlocksVal;
-        };
+            // This is a singleton, we need to execute it only once
+            if (!div) {
+                return;
+            }
 
-    })();
-    var rmargin = (/^margin/);
+            container.style.cssText = "position:absolute;left:-11111px;width:60px;" +
+                "margin-top:1px;padding:0;border:0";
+            div.style.cssText =
+                "position:relative;display:block;box-sizing:border-box;overflow:scroll;" +
+                "margin:auto;border:1px;padding:1px;" +
+                "width:60%;top:1%";
+            documentElement.appendChild(container).appendChild(div);
 
-    var rnumnonpx = new RegExp("^(" + pnum + ")(?!px)[a-z%]+$", "i");
+            var divStyle = window.getComputedStyle(div);
+            pixelPositionVal = divStyle.top !== "1%";
 
+            // Support: Android 4.0 - 4.3 only, Firefox <=3 - 44
+            reliableMarginLeftVal = roundPixelMeasures(divStyle.marginLeft) === 12;
 
+            // Support: Android 4.0 - 4.3 only, Safari <=9.1 - 10.1, iOS <=7.0 - 9.3
+            // Some styles come back with percentage values, even though they shouldn't
+            div.style.right = "60%";
+            pixelBoxStylesVal = roundPixelMeasures(divStyle.right) === 36;
 
-    var getStyles, curCSS,
-        rposition = /^(top|right|bottom|left)$/;
+            // Support: IE 9 - 11 only
+            // Detect misreporting of content dimensions for box-sizing:border-box elements
+            boxSizingReliableVal = roundPixelMeasures(divStyle.width) === 36;
 
-    if (window.getComputedStyle) {
-        getStyles = function(elem) {
-            return elem.ownerDocument.defaultView.getComputedStyle(elem, null);
-        };
+            // Support: IE 9 only
+            // Detect overflow:scroll screwiness (gh-3699)
+            // Support: Chrome <=64
+            // Don't get tricked when zoom affects offsetWidth (gh-4029)
+            div.style.position = "absolute";
+            scrollboxSizeVal = roundPixelMeasures(div.offsetWidth / 3) === 12;
 
-        curCSS = function(elem, name, computed) {
-            var width, minWidth, maxWidth, ret,
-                style = elem.style;
+            documentElement.removeChild(container);
 
-            computed = computed || getStyles(elem);
+            // Nullify the div so it wouldn't be stored in the memory and
+            // it will also be a sign that checks already performed
+            div = null;
+        }
 
-            // getPropertyValue is only needed for .css('filter') in IE9, see #12537
-            ret = computed ? computed.getPropertyValue(name) || computed[name] : undefined;
+        function roundPixelMeasures(measure) {
+            return Math.round(parseFloat(measure));
+        }
 
-            if (computed) {
+        var pixelPositionVal, boxSizingReliableVal, scrollboxSizeVal, pixelBoxStylesVal,
+            reliableTrDimensionsVal, reliableMarginLeftVal,
+            container = document.createElement("div"),
+            div = document.createElement("div");
 
-                if (ret === "" && !jQuery.contains(elem.ownerDocument, elem)) {
-                    ret = jQuery.style(elem, name);
-                }
+        // Finish early in limited (non-browser) environments
+        if (!div.style) {
+            return;
+        }
 
-                // A tribute to the "awesome hack by Dean Edwards"
-                // Chrome < 17 and Safari 5.0 uses "computed value" instead of "used value" for margin-right
-                // Safari 5.1.7 (at least) returns percentage for a larger set of values, but width seems to be reliably pixels
-                // this is against the CSSOM draft spec: http://dev.w3.org/csswg/cssom/#resolved-values
-                if (rnumnonpx.test(ret) && rmargin.test(name)) {
+        // Support: IE <=9 - 11 only
+        // Style of cloned element affects source element cloned (trac-8908)
+        div.style.backgroundClip = "content-box";
+        div.cloneNode(true).style.backgroundClip = "";
+        support.clearCloneStyle = div.style.backgroundClip === "content-box";
 
-                    // Remember the original values
-                    width = style.width;
-                    minWidth = style.minWidth;
-                    maxWidth = style.maxWidth;
+        jQuery.extend(support, {
+            boxSizingReliable: function() {
+                computeStyleTests();
+                return boxSizingReliableVal;
+            },
+            pixelBoxStyles: function() {
+                computeStyleTests();
+                return pixelBoxStylesVal;
+            },
+            pixelPosition: function() {
+                computeStyleTests();
+                return pixelPositionVal;
+            },
+            reliableMarginLeft: function() {
+                computeStyleTests();
+                return reliableMarginLeftVal;
+            },
+            scrollboxSize: function() {
+                computeStyleTests();
+                return scrollboxSizeVal;
+            },
 
-                    // Put in the new values to get a computed value out
-                    style.minWidth = style.maxWidth = style.width = ret;
-                    ret = computed.width;
+            // Support: IE 9 - 11+, Edge 15 - 18+
+            // IE/Edge misreport `getComputedStyle` of table rows with width/height
+            // set in CSS while `offset*` properties report correct values.
+            // Behavior in IE 9 is more subtle than in newer versions & it passes
+            // some versions of this test; make sure not to make it pass there!
+            //
+            // Support: Firefox 70+
+            // Only Firefox includes border widths
+            // in computed dimensions. (gh-4529)
+            reliableTrDimensions: function() {
+                var table, tr, trChild, trStyle;
+                if (reliableTrDimensionsVal == null) {
+                    table = document.createElement("table");
+                    tr = document.createElement("tr");
+                    trChild = document.createElement("div");
+
+                    table.style.cssText = "position:absolute;left:-11111px;border-collapse:separate";
+                    tr.style.cssText = "border:1px solid";
+
+                    // Support: Chrome 86+
+                    // Height set through cssText does not get applied.
+                    // Computed height then comes back as 0.
+                    tr.style.height = "1px";
+                    trChild.style.height = "9px";
+
+                    // Support: Android 8 Chrome 86+
+                    // In our bodyBackground.html iframe,
+                    // display for all div elements is set to "inline",
+                    // which causes a problem only in Android 8 Chrome 86.
+                    // Ensuring the div is display: block
+                    // gets around this issue.
+                    trChild.style.display = "block";
+
+                    documentElement
+                        .appendChild(table)
+                        .appendChild(tr)
+                        .appendChild(trChild);
+
+                    trStyle = window.getComputedStyle(tr);
+                    reliableTrDimensionsVal = (parseInt(trStyle.height, 10) +
+                        parseInt(trStyle.borderTopWidth, 10) +
+                        parseInt(trStyle.borderBottomWidth, 10)) === tr.offsetHeight;
 
-                    // Revert the changed values
-                    style.width = width;
-                    style.minWidth = minWidth;
-                    style.maxWidth = maxWidth;
+                    documentElement.removeChild(table);
                 }
+                return reliableTrDimensionsVal;
             }
+        });
+    })();
 
-            // Support: IE
-            // IE returns zIndex value as an integer.
-            return ret === undefined ?
-                ret :
-                ret + "";
-        };
-    } else if (document.documentElement.currentStyle) {
-        getStyles = function(elem) {
-            return elem.currentStyle;
-        };
-
-        curCSS = function(elem, name, computed) {
-            var left, rs, rsLeft, ret,
-                style = elem.style;
-
-            computed = computed || getStyles(elem);
-            ret = computed ? computed[name] : undefined;
 
-            // Avoid setting ret to empty string here
-            // so we don't default to auto
-            if (ret == null && style && style[name]) {
-                ret = style[name];
-            }
-
-            // From the awesome hack by Dean Edwards
-            // http://erik.eae.net/archives/2007/07/27/18.54.15/#comment-102291
-
-            // If we're not dealing with a regular pixel number
-            // but a number that has a weird ending, we need to convert it to pixels
-            // but not position css attributes, as those are proportional to the parent element instead
-            // and we can't measure the parent instead because it might trigger a "stacking dolls" problem
-            if (rnumnonpx.test(ret) && !rposition.test(name)) {
+    function curCSS(elem, name, computed) {
+        var width, minWidth, maxWidth, ret,
+            isCustomProp = rcustomProp.test(name),
+
+            // Support: Firefox 51+
+            // Retrieving style before computed somehow
+            // fixes an issue with getting wrong values
+            // on detached elements
+            style = elem.style;
+
+        computed = computed || getStyles(elem);
+
+        // getPropertyValue is needed for:
+        //   .css('filter') (IE 9 only, trac-12537)
+        //   .css('--customProperty) (gh-3144)
+        if (computed) {
+            ret = computed.getPropertyValue(name) || computed[name];
+
+            // trim whitespace for custom property (issue gh-4926)
+            if (isCustomProp) {
+
+                // rtrim treats U+000D CARRIAGE RETURN and U+000C FORM FEED
+                // as whitespace while CSS does not, but this is not a problem
+                // because CSS preprocessing replaces them with U+000A LINE FEED
+                // (which *is* CSS whitespace)
+                // https://www.w3.org/TR/css-syntax-3/#input-preprocessing
+                ret = ret.replace(rtrimCSS, "$1");
+            }
+
+            if (ret === "" && !isAttached(elem)) {
+                ret = jQuery.style(elem, name);
+            }
+
+            // A tribute to the "awesome hack by Dean Edwards"
+            // Android Browser returns percentage for some values,
+            // but width seems to be reliably pixels.
+            // This is against the CSSOM draft spec:
+            // https://drafts.csswg.org/cssom/#resolved-values
+            if (!support.pixelBoxStyles() && rnumnonpx.test(ret) && rboxStyle.test(name)) {
 
                 // Remember the original values
-                left = style.left;
-                rs = elem.runtimeStyle;
-                rsLeft = rs && rs.left;
+                width = style.width;
+                minWidth = style.minWidth;
+                maxWidth = style.maxWidth;
 
                 // Put in the new values to get a computed value out
-                if (rsLeft) {
-                    rs.left = elem.currentStyle.left;
-                }
-                style.left = name === "fontSize" ? "1em" : ret;
-                ret = style.pixelLeft + "px";
+                style.minWidth = style.maxWidth = style.width = ret;
+                ret = computed.width;
 
                 // Revert the changed values
-                style.left = left;
-                if (rsLeft) {
-                    rs.left = rsLeft;
-                }
+                style.width = width;
+                style.minWidth = minWidth;
+                style.maxWidth = maxWidth;
             }
+        }
 
-            // Support: IE
+        return ret !== undefined ?
+
+            // Support: IE <=9 - 11 only
             // IE returns zIndex value as an integer.
-            return ret === undefined ?
-                ret :
-                ret + "" || "auto";
-        };
+            ret + "" :
+            ret;
     }
 
 
-
-
     function addGetHookIf(conditionFn, hookFn) {
+
         // Define the hook, we'll check on the first run if it's really needed.
         return {
             get: function() {
-                var condition = conditionFn();
-
-                if (condition == null) {
-                    // The test was not ready at this point; screw the hook this time
-                    // but check again when needed next time.
-                    return;
-                }
+                if (conditionFn()) {
 
-                if (condition) {
-                    // Hook not needed (or it's not possible to use it due to missing dependency),
-                    // remove it.
-                    // Since there are no other hooks for marginRight, remove the whole object.
+                    // Hook not needed (or it's not possible to use it due
+                    // to missing dependency), remove it.
                     delete this.get;
                     return;
                 }
 
                 // Hook needed; redefine it so that the support test is not executed again.
-
                 return (this.get = hookFn).apply(this, arguments);
             }
         };
     }
 
 
-    (function() {
-        // Minified: var b,c,d,e,f,g, h,i
-        var div, style, a, pixelPositionVal, boxSizingReliableVal,
-            reliableHiddenOffsetsVal, reliableMarginRightVal;
-
-        // Setup
-        div = document.createElement("div");
-        div.innerHTML = "  <link/><table></table><a href='/a'>a</a><input type='checkbox'/>";
-        a = div.getElementsByTagName("a")[0];
-        style = a && a.style;
-
-        // Finish early in limited (non-browser) environments
-        if (!style) {
-            return;
-        }
-
-        style.cssText = "float:left;opacity:.5";
-
-        // Support: IE<9
-        // Make sure that element opacity exists (as opposed to filter)
-        support.opacity = style.opacity === "0.5";
-
-        // Verify style float existence
-        // (IE uses styleFloat instead of cssFloat)
-        support.cssFloat = !!style.cssFloat;
-
-        div.style.backgroundClip = "content-box";
-        div.cloneNode(true).style.backgroundClip = "";
-        support.clearCloneStyle = div.style.backgroundClip === "content-box";
-
-        // Support: Firefox<29, Android 2.3
-        // Vendor-prefix box-sizing
-        support.boxSizing = style.boxSizing === "" || style.MozBoxSizing === "" ||
-            style.WebkitBoxSizing === "";
-
-        jQuery.extend(support, {
-            reliableHiddenOffsets: function() {
-                if (reliableHiddenOffsetsVal == null) {
-                    computeStyleTests();
-                }
-                return reliableHiddenOffsetsVal;
-            },
-
-            boxSizingReliable: function() {
-                if (boxSizingReliableVal == null) {
-                    computeStyleTests();
-                }
-                return boxSizingReliableVal;
-            },
-
-            pixelPosition: function() {
-                if (pixelPositionVal == null) {
-                    computeStyleTests();
-                }
-                return pixelPositionVal;
-            },
-
-            // Support: Android 2.3
-            reliableMarginRight: function() {
-                if (reliableMarginRightVal == null) {
-                    computeStyleTests();
-                }
-                return reliableMarginRightVal;
-            }
-        });
-
-        function computeStyleTests() {
-            // Minified: var b,c,d,j
-            var div, body, container, contents;
-
-            body = document.getElementsByTagName("body")[0];
-            if (!body || !body.style) {
-                // Test fired too early or in an unsupported environment, exit.
-                return;
-            }
+    var cssPrefixes = ["Webkit", "Moz", "ms"],
+        emptyStyle = document.createElement("div").style,
+        vendorProps = {};
 
-            // Setup
-            div = document.createElement("div");
-            container = document.createElement("div");
-            container.style.cssText = "position:absolute;border:0;width:0;height:0;top:0;left:-9999px";
-            body.appendChild(container).appendChild(div);
+    // Return a vendor-prefixed property or undefined
+    function vendorPropName(name) {
 
-            div.style.cssText =
-                // Support: Firefox<29, Android 2.3
-                // Vendor-prefix box-sizing
-                "-webkit-box-sizing:border-box;-moz-box-sizing:border-box;" +
-                "box-sizing:border-box;display:block;margin-top:1%;top:1%;" +
-                "border:1px;padding:1px;width:4px;position:absolute";
+        // Check for vendor prefixed names
+        var capName = name[0].toUpperCase() + name.slice(1),
+            i = cssPrefixes.length;
 
-            // Support: IE<9
-            // Assume reasonable values in the absence of getComputedStyle
-            pixelPositionVal = boxSizingReliableVal = false;
-            reliableMarginRightVal = true;
-
-            // Check for getComputedStyle so that this code is not run in IE<9.
-            if (window.getComputedStyle) {
-                pixelPositionVal = (window.getComputedStyle(div, null) || {}).top !== "1%";
-                boxSizingReliableVal =
-                    (window.getComputedStyle(div, null) || {
-                        width: "4px"
-                    }).width === "4px";
-
-                // Support: Android 2.3
-                // Div with explicit width and no margin-right incorrectly
-                // gets computed margin-right based on width of container (#3333)
-                // WebKit Bug 13343 - getComputedStyle returns wrong value for margin-right
-                contents = div.appendChild(document.createElement("div"));
-
-                // Reset CSS: box-sizing; display; margin; border; padding
-                contents.style.cssText = div.style.cssText =
-                    // Support: Firefox<29, Android 2.3
-                    // Vendor-prefix box-sizing
-                    "-webkit-box-sizing:content-box;-moz-box-sizing:content-box;" +
-                    "box-sizing:content-box;display:block;margin:0;border:0;padding:0";
-                contents.style.marginRight = contents.style.width = "0";
-                div.style.width = "1px";
-
-                reliableMarginRightVal = !parseFloat((window.getComputedStyle(contents, null) || {}).marginRight);
-            }
-
-            // Support: IE8
-            // Check if table cells still have offsetWidth/Height when they are set
-            // to display:none and there are still other visible table cells in a
-            // table row; if so, offsetWidth/Height are not reliable for use when
-            // determining if an element has been hidden directly using
-            // display:none (it is still safe to use offsets if a parent element is
-            // hidden; don safety goggles and see bug #4512 for more information).
-            div.innerHTML = "<table><tr><td></td><td>t</td></tr></table>";
-            contents = div.getElementsByTagName("td");
-            contents[0].style.cssText = "margin:0;border:0;padding:0;display:none";
-            reliableHiddenOffsetsVal = contents[0].offsetHeight === 0;
-            if (reliableHiddenOffsetsVal) {
-                contents[0].style.display = "";
-                contents[1].style.display = "none";
-                reliableHiddenOffsetsVal = contents[0].offsetHeight === 0;
+        while (i--) {
+            name = cssPrefixes[i] + capName;
+            if (name in emptyStyle) {
+                return name;
             }
-
-            body.removeChild(container);
         }
+    }
 
-    })();
-
-
-    // A method for quickly swapping in/out CSS properties to get correct calculations.
-    jQuery.swap = function(elem, options, callback, args) {
-        var ret, name,
-            old = {};
+    // Return a potentially-mapped jQuery.cssProps or vendor prefixed property
+    function finalPropName(name) {
+        var final = jQuery.cssProps[name] || vendorProps[name];
 
-        // Remember the old values, and insert the new ones
-        for (name in options) {
-            old[name] = elem.style[name];
-            elem.style[name] = options[name];
+        if (final) {
+            return final;
         }
-
-        ret = callback.apply(elem, args || []);
-
-        // Revert the old values
-        for (name in options) {
-            elem.style[name] = old[name];
+        if (name in emptyStyle) {
+            return name;
         }
-
-        return ret;
-    };
+        return vendorProps[name] = vendorPropName(name) || name;
+    }
 
 
     var
-        ralpha = /alpha\([^)]*\)/i,
-        ropacity = /opacity\s*=\s*([^)]*)/,
 
-        // swappable if display is none or starts with table except "table", "table-cell", or "table-caption"
-        // see here for display values: https://developer.mozilla.org/en-US/docs/CSS/display
+        // Swappable if display is none or starts with table
+        // except "table", "table-cell", or "table-caption"
+        // See here for display values: https://developer.mozilla.org/en-US/docs/CSS/display
         rdisplayswap = /^(none|table(?!-c[ea]).+)/,
-        rnumsplit = new RegExp("^(" + pnum + ")(.*)$", "i"),
-        rrelNum = new RegExp("^([+-])=(" + pnum + ")", "i"),
-
         cssShow = {
             position: "absolute",
             visibility: "hidden",
             display: "block"
         },
         cssNormalTransform = {
             letterSpacing: "0",
             fontWeight: "400"
-        },
+        };
 
-        cssPrefixes = ["Webkit", "O", "Moz", "ms"];
+    function setPositiveNumber(_elem, value, subtract) {
 
+        // Any relative (+/-) values have already been
+        // normalized at this point
+        var matches = rcssNum.exec(value);
+        return matches ?
 
-    // return a css property mapped to a potentially vendor prefixed property
-    function vendorPropName(style, name) {
+            // Guard against undefined "subtract", e.g., when used as in cssHooks
+            Math.max(0, matches[2] - (subtract || 0)) + (matches[3] || "px") :
+            value;
+    }
 
-        // shortcut for names that are not vendor prefixed
-        if (name in style) {
-            return name;
+    function boxModelAdjustment(elem, dimension, box, isBorderBox, styles, computedVal) {
+        var i = dimension === "width" ? 1 : 0,
+            extra = 0,
+            delta = 0;
+
+        // Adjustment may not be necessary
+        if (box === (isBorderBox ? "border" : "content")) {
+            return 0;
         }
 
-        // check for vendor prefixed names
-        var capName = name.charAt(0).toUpperCase() + name.slice(1),
-            origName = name,
-            i = cssPrefixes.length;
+        for (; i < 4; i += 2) {
 
-        while (i--) {
-            name = cssPrefixes[i] + capName;
-            if (name in style) {
-                return name;
+            // Both box models exclude margin
+            if (box === "margin") {
+                delta += jQuery.css(elem, box + cssExpand[i], true, styles);
             }
-        }
 
-        return origName;
-    }
+            // If we get here with a content-box, we're seeking "padding" or "border" or "margin"
+            if (!isBorderBox) {
 
-    function showHide(elements, show) {
-        var display, elem, hidden,
-            values = [],
-            index = 0,
-            length = elements.length;
+                // Add padding
+                delta += jQuery.css(elem, "padding" + cssExpand[i], true, styles);
 
-        for (; index < length; index++) {
-            elem = elements[index];
-            if (!elem.style) {
-                continue;
-            }
+                // For "border" or "margin", add border
+                if (box !== "padding") {
+                    delta += jQuery.css(elem, "border" + cssExpand[i] + "Width", true, styles);
 
-            values[index] = jQuery._data(elem, "olddisplay");
-            display = elem.style.display;
-            if (show) {
-                // Reset the inline display of this element to learn if it is
-                // being hidden by cascaded rules or not
-                if (!values[index] && display === "none") {
-                    elem.style.display = "";
+                    // But still keep track of it otherwise
+                } else {
+                    extra += jQuery.css(elem, "border" + cssExpand[i] + "Width", true, styles);
                 }
 
-                // Set elements which have been overridden with display: none
-                // in a stylesheet to whatever the default browser style is
-                // for such an element
-                if (elem.style.display === "" && isHidden(elem)) {
-                    values[index] = jQuery._data(elem, "olddisplay", defaultDisplay(elem.nodeName));
-                }
+                // If we get here with a border-box (content + padding + border), we're seeking "content" or
+                // "padding" or "margin"
             } else {
-                hidden = isHidden(elem);
 
-                if (display && display !== "none" || !hidden) {
-                    jQuery._data(elem, "olddisplay", hidden ? display : jQuery.css(elem, "display"));
+                // For "content", subtract padding
+                if (box === "content") {
+                    delta -= jQuery.css(elem, "padding" + cssExpand[i], true, styles);
                 }
-            }
-        }
 
-        // Set the display of most of the elements in a second loop
-        // to avoid the constant reflow
-        for (index = 0; index < length; index++) {
-            elem = elements[index];
-            if (!elem.style) {
-                continue;
-            }
-            if (!show || elem.style.display === "none" || elem.style.display === "") {
-                elem.style.display = show ? values[index] || "" : "none";
+                // For "content" or "padding", subtract border
+                if (box !== "margin") {
+                    delta -= jQuery.css(elem, "border" + cssExpand[i] + "Width", true, styles);
+                }
             }
         }
 
-        return elements;
-    }
+        // Account for positive content-box scroll gutter when requested by providing computedVal
+        if (!isBorderBox && computedVal >= 0) {
 
-    function setPositiveNumber(elem, value, subtract) {
-        var matches = rnumsplit.exec(value);
-        return matches ?
-            // Guard against undefined "subtract", e.g., when used as in cssHooks
-            Math.max(0, matches[1] - (subtract || 0)) + (matches[2] || "px") :
-            value;
-    }
+            // offsetWidth/offsetHeight is a rounded sum of content, padding, scroll gutter, and border
+            // Assuming integer scroll gutter, subtract the rest and round down
+            delta += Math.max(0, Math.ceil(
+                elem["offset" + dimension[0].toUpperCase() + dimension.slice(1)] -
+                computedVal -
+                delta -
+                extra -
+                0.5
 
-    function augmentWidthOrHeight(elem, name, extra, isBorderBox, styles) {
-        var i = extra === (isBorderBox ? "border" : "content") ?
-            // If we already have the right measurement, avoid augmentation
-            4 :
-            // Otherwise initialize for horizontal or vertical properties
-            name === "width" ? 1 : 0,
+                // If offsetWidth/offsetHeight is unknown, then we can't determine content-box scroll gutter
+                // Use an explicit zero to avoid NaN (gh-3964)
+            )) || 0;
+        }
 
-            val = 0;
+        return delta;
+    }
 
-        for (; i < 4; i += 2) {
-            // both box models exclude margin, so add it if we want it
-            if (extra === "margin") {
-                val += jQuery.css(elem, extra + cssExpand[i], true, styles);
-            }
+    function getWidthOrHeight(elem, dimension, extra) {
 
-            if (isBorderBox) {
-                // border-box includes padding, so remove it if we want content
-                if (extra === "content") {
-                    val -= jQuery.css(elem, "padding" + cssExpand[i], true, styles);
-                }
+        // Start with computed style
+        var styles = getStyles(elem),
 
-                // at this point, extra isn't border nor margin, so remove border
-                if (extra !== "margin") {
-                    val -= jQuery.css(elem, "border" + cssExpand[i] + "Width", true, styles);
-                }
-            } else {
-                // at this point, extra isn't content, so add padding
-                val += jQuery.css(elem, "padding" + cssExpand[i], true, styles);
+            // To avoid forcing a reflow, only fetch boxSizing if we need it (gh-4322).
+            // Fake content-box until we know it's needed to know the true value.
+            boxSizingNeeded = !support.boxSizingReliable() || extra,
+            isBorderBox = boxSizingNeeded &&
+            jQuery.css(elem, "boxSizing", false, styles) === "border-box",
+            valueIsBorderBox = isBorderBox,
 
-                // at this point, extra isn't content nor padding, so add border
-                if (extra !== "padding") {
-                    val += jQuery.css(elem, "border" + cssExpand[i] + "Width", true, styles);
-                }
+            val = curCSS(elem, dimension, styles),
+            offsetProp = "offset" + dimension[0].toUpperCase() + dimension.slice(1);
+
+        // Support: Firefox <=54
+        // Return a confounding non-pixel value or feign ignorance, as appropriate.
+        if (rnumnonpx.test(val)) {
+            if (!extra) {
+                return val;
             }
+            val = "auto";
         }
 
-        return val;
-    }
 
-    function getWidthOrHeight(elem, name, extra) {
+        // Support: IE 9 - 11 only
+        // Use offsetWidth/offsetHeight for when box sizing is unreliable.
+        // In those cases, the computed value can be trusted to be border-box.
+        if ((!support.boxSizingReliable() && isBorderBox ||
 
-        // Start with offset property, which is equivalent to the border-box value
-        var valueIsBorderBox = true,
-            val = name === "width" ? elem.offsetWidth : elem.offsetHeight,
-            styles = getStyles(elem),
-            isBorderBox = support.boxSizing && jQuery.css(elem, "boxSizing", false, styles) === "border-box";
+                // Support: IE 10 - 11+, Edge 15 - 18+
+                // IE/Edge misreport `getComputedStyle` of table rows with width/height
+                // set in CSS while `offset*` properties report correct values.
+                // Interestingly, in some cases IE 9 doesn't suffer from this issue.
+                !support.reliableTrDimensions() && nodeName(elem, "tr") ||
 
-        // some non-html elements return undefined for offsetWidth, so check for null/undefined
-        // svg - https://bugzilla.mozilla.org/show_bug.cgi?id=649285
-        // MathML - https://bugzilla.mozilla.org/show_bug.cgi?id=491668
-        if (val <= 0 || val == null) {
-            // Fall back to computed then uncomputed css if necessary
-            val = curCSS(elem, name, styles);
-            if (val < 0 || val == null) {
-                val = elem.style[name];
-            }
+                // Fall back to offsetWidth/offsetHeight when value is "auto"
+                // This happens for inline elements with no explicit setting (gh-3571)
+                val === "auto" ||
 
-            // Computed unit is not pixels. Stop here and return.
-            if (rnumnonpx.test(val)) {
-                return val;
-            }
+                // Support: Android <=4.1 - 4.3 only
+                // Also use offsetWidth/offsetHeight for misreported inline dimensions (gh-3602)
+                !parseFloat(val) && jQuery.css(elem, "display", false, styles) === "inline") &&
+
+            // Make sure the element is visible & connected
+            elem.getClientRects().length) {
 
-            // we need the check for style in case a browser which returns unreliable values
-            // for getComputedStyle silently falls back to the reliable elem.style
-            valueIsBorderBox = isBorderBox && (support.boxSizingReliable() || val === elem.style[name]);
+            isBorderBox = jQuery.css(elem, "boxSizing", false, styles) === "border-box";
 
-            // Normalize "", auto, and prepare for extra
-            val = parseFloat(val) || 0;
+            // Where available, offsetWidth/offsetHeight approximate border box dimensions.
+            // Where not available (e.g., SVG), assume unreliable box-sizing and interpret the
+            // retrieved value as a content box dimension.
+            valueIsBorderBox = offsetProp in elem;
+            if (valueIsBorderBox) {
+                val = elem[offsetProp];
+            }
         }
 
-        // use the active box-sizing model to add/subtract irrelevant styles
+        // Normalize "" and auto
+        val = parseFloat(val) || 0;
+
+        // Adjust for the element's box model
         return (val +
-            augmentWidthOrHeight(
+            boxModelAdjustment(
                 elem,
-                name,
+                dimension,
                 extra || (isBorderBox ? "border" : "content"),
                 valueIsBorderBox,
-                styles
+                styles,
+
+                // Provide the current computed size to request scroll gutter calculation (gh-3589)
+                val
             )
         ) + "px";
     }
 
     jQuery.extend({
+
         // Add in style property hooks for overriding the default
         // behavior of getting and setting a style property
         cssHooks: {
             opacity: {
                 get: function(elem, computed) {
                     if (computed) {
+
                         // We should always get a number back from opacity
                         var ret = curCSS(elem, "opacity");
                         return ret === "" ? "1" : ret;
                     }
                 }
             }
         },
 
         // Don't automatically add "px" to these possibly-unitless properties
         cssNumber: {
+            "animationIterationCount": true,
             "columnCount": true,
             "fillOpacity": true,
             "flexGrow": true,
             "flexShrink": true,
             "fontWeight": true,
+            "gridArea": true,
+            "gridColumn": true,
+            "gridColumnEnd": true,
+            "gridColumnStart": true,
+            "gridRow": true,
+            "gridRowEnd": true,
+            "gridRowStart": true,
             "lineHeight": true,
             "opacity": true,
             "order": true,
             "orphans": true,
             "widows": true,
             "zIndex": true,
             "zoom": true
         },
 
         // Add in properties whose names you wish to fix before
         // setting or getting the value
-        cssProps: {
-            // normalize float css property
-            "float": support.cssFloat ? "cssFloat" : "styleFloat"
-        },
+        cssProps: {},
 
         // Get and set the style property on a DOM Node
         style: function(elem, name, value, extra) {
+
             // Don't set styles on text and comment nodes
             if (!elem || elem.nodeType === 3 || elem.nodeType === 8 || !elem.style) {
                 return;
             }
 
             // Make sure that we're working with the right name
             var ret, type, hooks,
-                origName = jQuery.camelCase(name),
+                origName = camelCase(name),
+                isCustomProp = rcustomProp.test(name),
                 style = elem.style;
 
-            name = jQuery.cssProps[origName] || (jQuery.cssProps[origName] = vendorPropName(style, origName));
+            // Make sure that we're working with the right name. We don't
+            // want to query the value if it is a CSS custom property
+            // since they are user-defined.
+            if (!isCustomProp) {
+                name = finalPropName(origName);
+            }
 
-            // gets hook for the prefixed version
-            // followed by the unprefixed version
+            // Gets hook for the prefixed version, then unprefixed version
             hooks = jQuery.cssHooks[name] || jQuery.cssHooks[origName];
 
             // Check if we're setting a value
             if (value !== undefined) {
                 type = typeof value;
 
-                // convert relative number strings (+= or -=) to relative numbers. #7345
-                if (type === "string" && (ret = rrelNum.exec(value))) {
-                    value = (ret[1] + 1) * ret[2] + parseFloat(jQuery.css(elem, name));
-                    // Fixes bug #9237
+                // Convert "+=" or "-=" to relative numbers (trac-7345)
+                if (type === "string" && (ret = rcssNum.exec(value)) && ret[1]) {
+                    value = adjustCSS(elem, name, ret);
+
+                    // Fixes bug trac-9237
                     type = "number";
                 }
 
-                // Make sure that null and NaN values aren't set. See: #7116
+                // Make sure that null and NaN values aren't set (trac-7116)
                 if (value == null || value !== value) {
                     return;
                 }
 
-                // If a number was passed in, add 'px' to the (except for certain CSS properties)
-                if (type === "number" && !jQuery.cssNumber[origName]) {
-                    value += "px";
+                // If a number was passed in, add the unit (except for certain CSS properties)
+                // The isCustomProp check can be removed in jQuery 4.0 when we only auto-append
+                // "px" to a few hardcoded values.
+                if (type === "number" && !isCustomProp) {
+                    value += ret && ret[3] || (jQuery.cssNumber[origName] ? "" : "px");
                 }
 
-                // Fixes #8908, it can be done more correctly by specifing setters in cssHooks,
-                // but it would mean to define eight (for every problematic property) identical functions
+                // background-* props affect original clone's values
                 if (!support.clearCloneStyle && value === "" && name.indexOf("background") === 0) {
                     style[name] = "inherit";
                 }
 
                 // If a hook was provided, use that value, otherwise just set the specified value
-                if (!hooks || !("set" in hooks) || (value = hooks.set(elem, value, extra)) !== undefined) {
+                if (!hooks || !("set" in hooks) ||
+                    (value = hooks.set(elem, value, extra)) !== undefined) {
 
-                    // Support: IE
-                    // Swallow errors from 'invalid' CSS values (#5509)
-                    try {
+                    if (isCustomProp) {
+                        style.setProperty(name, value);
+                    } else {
                         style[name] = value;
-                    } catch (e) {}
+                    }
                 }
 
             } else {
+
                 // If a hook was provided get the non-computed value from there
-                if (hooks && "get" in hooks && (ret = hooks.get(elem, false, extra)) !== undefined) {
+                if (hooks && "get" in hooks &&
+                    (ret = hooks.get(elem, false, extra)) !== undefined) {
+
                     return ret;
                 }
 
                 // Otherwise just get the value from the style object
                 return style[name];
             }
         },
 
         css: function(elem, name, extra, styles) {
-            var num, val, hooks,
-                origName = jQuery.camelCase(name);
-
-            // Make sure that we're working with the right name
-            name = jQuery.cssProps[origName] || (jQuery.cssProps[origName] = vendorPropName(elem.style, origName));
+            var val, num, hooks,
+                origName = camelCase(name),
+                isCustomProp = rcustomProp.test(name);
+
+            // Make sure that we're working with the right name. We don't
+            // want to modify the value if it is a CSS custom property
+            // since they are user-defined.
+            if (!isCustomProp) {
+                name = finalPropName(origName);
+            }
 
-            // gets hook for the prefixed version
-            // followed by the unprefixed version
+            // Try prefixed name followed by the unprefixed name
             hooks = jQuery.cssHooks[name] || jQuery.cssHooks[origName];
 
             // If a hook was provided get the computed value from there
             if (hooks && "get" in hooks) {
                 val = hooks.get(elem, true, extra);
             }
 
             // Otherwise, if a way to get the computed value exists, use that
             if (val === undefined) {
                 val = curCSS(elem, name, styles);
             }
 
-            //convert "normal" to computed value
+            // Convert "normal" to computed value
             if (val === "normal" && name in cssNormalTransform) {
                 val = cssNormalTransform[name];
             }
 
-            // Return, converting to number if forced or a qualifier was provided and val looks numeric
+            // Make numeric if forced or a qualifier was provided and val looks numeric
             if (extra === "" || extra) {
                 num = parseFloat(val);
-                return extra === true || jQuery.isNumeric(num) ? num || 0 : val;
+                return extra === true || isFinite(num) ? num || 0 : val;
             }
+
             return val;
         }
     });
 
-    jQuery.each(["height", "width"], function(i, name) {
-        jQuery.cssHooks[name] = {
+    jQuery.each(["height", "width"], function(_i, dimension) {
+        jQuery.cssHooks[dimension] = {
             get: function(elem, computed, extra) {
                 if (computed) {
-                    // certain elements can have dimension info if we invisibly show them
-                    // however, it must have a current display style that would benefit from this
-                    return rdisplayswap.test(jQuery.css(elem, "display")) && elem.offsetWidth === 0 ?
-                        jQuery.swap(elem, cssShow, function() {
-                            return getWidthOrHeight(elem, name, extra);
+
+                    // Certain elements can have dimension info if we invisibly show them
+                    // but it must have a current display style that would benefit
+                    return rdisplayswap.test(jQuery.css(elem, "display")) &&
+
+                        // Support: Safari 8+
+                        // Table columns in Safari have non-zero offsetWidth & zero
+                        // getBoundingClientRect().width unless display is changed.
+                        // Support: IE <=11 only
+                        // Running getBoundingClientRect on a disconnected node
+                        // in IE throws an error.
+                        (!elem.getClientRects().length || !elem.getBoundingClientRect().width) ?
+                        swap(elem, cssShow, function() {
+                            return getWidthOrHeight(elem, dimension, extra);
                         }) :
-                        getWidthOrHeight(elem, name, extra);
+                        getWidthOrHeight(elem, dimension, extra);
                 }
             },
 
             set: function(elem, value, extra) {
-                var styles = extra && getStyles(elem);
-                return setPositiveNumber(elem, value, extra ?
-                    augmentWidthOrHeight(
+                var matches,
+                    styles = getStyles(elem),
+
+                    // Only read styles.position if the test has a chance to fail
+                    // to avoid forcing a reflow.
+                    scrollboxSizeBuggy = !support.scrollboxSize() &&
+                    styles.position === "absolute",
+
+                    // To avoid forcing a reflow, only fetch boxSizing if we need it (gh-3991)
+                    boxSizingNeeded = scrollboxSizeBuggy || extra,
+                    isBorderBox = boxSizingNeeded &&
+                    jQuery.css(elem, "boxSizing", false, styles) === "border-box",
+                    subtract = extra ?
+                    boxModelAdjustment(
                         elem,
-                        name,
+                        dimension,
                         extra,
-                        support.boxSizing && jQuery.css(elem, "boxSizing", false, styles) === "border-box",
+                        isBorderBox,
                         styles
-                    ) : 0
-                );
-            }
-        };
-    });
+                    ) :
+                    0;
 
-    if (!support.opacity) {
-        jQuery.cssHooks.opacity = {
-            get: function(elem, computed) {
-                // IE uses filters for opacity
-                return ropacity.test((computed && elem.currentStyle ? elem.currentStyle.filter : elem.style.filter) || "") ?
-                    (0.01 * parseFloat(RegExp.$1)) + "" :
-                    computed ? "1" : "";
-            },
+                // Account for unreliable border-box dimensions by comparing offset* to computed and
+                // faking a content-box to get border and padding (gh-3699)
+                if (isBorderBox && scrollboxSizeBuggy) {
+                    subtract -= Math.ceil(
+                        elem["offset" + dimension[0].toUpperCase() + dimension.slice(1)] -
+                        parseFloat(styles[dimension]) -
+                        boxModelAdjustment(elem, dimension, "border", false, styles) -
+                        0.5
+                    );
+                }
 
-            set: function(elem, value) {
-                var style = elem.style,
-                    currentStyle = elem.currentStyle,
-                    opacity = jQuery.isNumeric(value) ? "alpha(opacity=" + value * 100 + ")" : "",
-                    filter = currentStyle && currentStyle.filter || style.filter || "";
-
-                // IE has trouble with opacity if it does not have layout
-                // Force it by setting the zoom level
-                style.zoom = 1;
-
-                // if setting opacity to 1, and no other filters exist - attempt to remove filter attribute #6652
-                // if value === "", then remove inline opacity #12685
-                if ((value >= 1 || value === "") &&
-                    jQuery.trim(filter.replace(ralpha, "")) === "" &&
-                    style.removeAttribute) {
-
-                    // Setting style.filter to null, "" & " " still leave "filter:" in the cssText
-                    // if "filter:" is present at all, clearType is disabled, we want to avoid this
-                    // style.removeAttribute is IE Only, but so apparently is this code path...
-                    style.removeAttribute("filter");
-
-                    // if there is no filter style applied in a css rule or unset inline opacity, we are done
-                    if (value === "" || currentStyle && !currentStyle.filter) {
-                        return;
-                    }
+                // Convert to pixels if value adjustment is needed
+                if (subtract && (matches = rcssNum.exec(value)) &&
+                    (matches[3] || "px") !== "px") {
+
+                    elem.style[dimension] = value;
+                    value = jQuery.css(elem, dimension);
                 }
 
-                // otherwise, set new filter values
-                style.filter = ralpha.test(filter) ?
-                    filter.replace(ralpha, opacity) :
-                    filter + " " + opacity;
+                return setPositiveNumber(elem, value, subtract);
             }
         };
-    }
+    });
 
-    jQuery.cssHooks.marginRight = addGetHookIf(support.reliableMarginRight,
+    jQuery.cssHooks.marginLeft = addGetHookIf(support.reliableMarginLeft,
         function(elem, computed) {
             if (computed) {
-                // WebKit Bug 13343 - getComputedStyle returns wrong value for margin-right
-                // Work around by temporarily setting element display to inline-block
-                return jQuery.swap(elem, {
-                        "display": "inline-block"
-                    },
-                    curCSS, [elem, "marginRight"]);
+                return (parseFloat(curCSS(elem, "marginLeft")) ||
+                    elem.getBoundingClientRect().left -
+                    swap(elem, {
+                        marginLeft: 0
+                    }, function() {
+                        return elem.getBoundingClientRect().left;
+                    })
+                ) + "px";
             }
         }
     );
 
     // These hooks are used by animate to expand properties
     jQuery.each({
         margin: "",
@@ -6872,87 +7179,68 @@
         border: "Width"
     }, function(prefix, suffix) {
         jQuery.cssHooks[prefix + suffix] = {
             expand: function(value) {
                 var i = 0,
                     expanded = {},
 
-                    // assumes a single number if not a string
+                    // Assumes a single number if not a string
                     parts = typeof value === "string" ? value.split(" ") : [value];
 
                 for (; i < 4; i++) {
                     expanded[prefix + cssExpand[i] + suffix] =
                         parts[i] || parts[i - 2] || parts[0];
                 }
 
                 return expanded;
             }
         };
 
-        if (!rmargin.test(prefix)) {
+        if (prefix !== "margin") {
             jQuery.cssHooks[prefix + suffix].set = setPositiveNumber;
         }
     });
 
     jQuery.fn.extend({
         css: function(name, value) {
             return access(this, function(elem, name, value) {
                 var styles, len,
                     map = {},
                     i = 0;
 
-                if (jQuery.isArray(name)) {
+                if (Array.isArray(name)) {
                     styles = getStyles(elem);
                     len = name.length;
 
                     for (; i < len; i++) {
                         map[name[i]] = jQuery.css(elem, name[i], false, styles);
                     }
 
                     return map;
                 }
 
                 return value !== undefined ?
                     jQuery.style(elem, name, value) :
                     jQuery.css(elem, name);
             }, name, value, arguments.length > 1);
-        },
-        show: function() {
-            return showHide(this, true);
-        },
-        hide: function() {
-            return showHide(this);
-        },
-        toggle: function(state) {
-            if (typeof state === "boolean") {
-                return state ? this.show() : this.hide();
-            }
-
-            return this.each(function() {
-                if (isHidden(this)) {
-                    jQuery(this).show();
-                } else {
-                    jQuery(this).hide();
-                }
-            });
         }
     });
 
 
     function Tween(elem, options, prop, end, easing) {
         return new Tween.prototype.init(elem, options, prop, end, easing);
     }
     jQuery.Tween = Tween;
 
     Tween.prototype = {
         constructor: Tween,
         init: function(elem, options, prop, end, easing, unit) {
             this.elem = elem;
             this.prop = prop;
-            this.easing = easing || "swing";
+            this.easing = easing || jQuery.easing._default;
             this.options = options;
             this.start = this.now = this.cur();
             this.end = end;
             this.unit = unit || (jQuery.cssNumber[prop] ? "" : "px");
         },
         cur: function() {
             var hooks = Tween.propHooks[this.prop];
@@ -6990,144 +7278,111 @@
     Tween.prototype.init.prototype = Tween.prototype;
 
     Tween.propHooks = {
         _default: {
             get: function(tween) {
                 var result;
 
-                if (tween.elem[tween.prop] != null &&
-                    (!tween.elem.style || tween.elem.style[tween.prop] == null)) {
+                // Use a property on the element directly when it is not a DOM element,
+                // or when there is no matching style property that exists.
+                if (tween.elem.nodeType !== 1 ||
+                    tween.elem[tween.prop] != null && tween.elem.style[tween.prop] == null) {
                     return tween.elem[tween.prop];
                 }
 
-                // passing an empty string as a 3rd parameter to .css will automatically
-                // attempt a parseFloat and fallback to a string if the parse fails
-                // so, simple values such as "10px" are parsed to Float.
-                // complex values such as "rotate(1rad)" are returned as is.
+                // Passing an empty string as a 3rd parameter to .css will automatically
+                // attempt a parseFloat and fallback to a string if the parse fails.
+                // Simple values such as "10px" are parsed to Float;
+                // complex values such as "rotate(1rad)" are returned as-is.
                 result = jQuery.css(tween.elem, tween.prop, "");
+
                 // Empty strings, null, undefined and "auto" are converted to 0.
                 return !result || result === "auto" ? 0 : result;
             },
             set: function(tween) {
-                // use step hook for back compat - use cssHook if its there - use .style if its
-                // available and use plain properties where available
+
+                // Use step hook for back compat.
+                // Use cssHook if its there.
+                // Use .style if available and use plain properties where available.
                 if (jQuery.fx.step[tween.prop]) {
                     jQuery.fx.step[tween.prop](tween);
-                } else if (tween.elem.style && (tween.elem.style[jQuery.cssProps[tween.prop]] != null || jQuery.cssHooks[tween.prop])) {
+                } else if (tween.elem.nodeType === 1 && (
+                        jQuery.cssHooks[tween.prop] ||
+                        tween.elem.style[finalPropName(tween.prop)] != null)) {
                     jQuery.style(tween.elem, tween.prop, tween.now + tween.unit);
                 } else {
                     tween.elem[tween.prop] = tween.now;
                 }
             }
         }
     };
 
-    // Support: IE <=9
+    // Support: IE <=9 only
     // Panic based approach to setting things on disconnected nodes
-
     Tween.propHooks.scrollTop = Tween.propHooks.scrollLeft = {
         set: function(tween) {
             if (tween.elem.nodeType && tween.elem.parentNode) {
                 tween.elem[tween.prop] = tween.now;
             }
         }
     };
 
     jQuery.easing = {
         linear: function(p) {
             return p;
         },
         swing: function(p) {
             return 0.5 - Math.cos(p * Math.PI) / 2;
-        }
+        },
+        _default: "swing"
     };
 
     jQuery.fx = Tween.prototype.init;
 
-    // Back Compat <1.8 extension point
+    // Back compat <1.8 extension point
     jQuery.fx.step = {};
 
 
 
 
     var
-        fxNow, timerId,
+        fxNow, inProgress,
         rfxtypes = /^(?:toggle|show|hide)$/,
-        rfxnum = new RegExp("^(?:([+-])=|)(" + pnum + ")([a-z%]*)$", "i"),
-        rrun = /queueHooks$/,
-        animationPrefilters = [defaultPrefilter],
-        tweeners = {
-            "*": [function(prop, value) {
-                var tween = this.createTween(prop, value),
-                    target = tween.cur(),
-                    parts = rfxnum.exec(value),
-                    unit = parts && parts[3] || (jQuery.cssNumber[prop] ? "" : "px"),
-
-                    // Starting value computation is required for potential unit mismatches
-                    start = (jQuery.cssNumber[prop] || unit !== "px" && +target) &&
-                    rfxnum.exec(jQuery.css(tween.elem, prop)),
-                    scale = 1,
-                    maxIterations = 20;
-
-                if (start && start[3] !== unit) {
-                    // Trust units reported by jQuery.css
-                    unit = unit || start[3];
-
-                    // Make sure we update the tween properties later on
-                    parts = parts || [];
-
-                    // Iteratively approximate from a nonzero starting point
-                    start = +target || 1;
-
-                    do {
-                        // If previous iteration zeroed out, double until we get *something*
-                        // Use a string for doubling factor so we don't accidentally see scale as unchanged below
-                        scale = scale || ".5";
-
-                        // Adjust and apply
-                        start = start / scale;
-                        jQuery.style(tween.elem, prop, start + unit);
-
-                        // Update scale, tolerating zero or NaN from tween.cur()
-                        // And breaking the loop if scale is unchanged or perfect, or if we've just had enough
-                    } while (scale !== (scale = tween.cur() / target) && scale !== 1 && --maxIterations);
-                }
-
-                // Update tween properties
-                if (parts) {
-                    start = tween.start = +start || +target || 0;
-                    tween.unit = unit;
-                    // If a +=/-= token was provided, we're doing a relative animation
-                    tween.end = parts[1] ?
-                        start + (parts[1] + 1) * parts[2] :
-                        +parts[2];
-                }
+        rrun = /queueHooks$/;
 
-                return tween;
-            }]
-        };
+    function schedule() {
+        if (inProgress) {
+            if (document.hidden === false && window.requestAnimationFrame) {
+                window.requestAnimationFrame(schedule);
+            } else {
+                window.setTimeout(schedule, jQuery.fx.interval);
+            }
+
+            jQuery.fx.tick();
+        }
+    }
 
     // Animations created synchronously will run synchronously
     function createFxNow() {
-        setTimeout(function() {
+        window.setTimeout(function() {
             fxNow = undefined;
         });
-        return (fxNow = jQuery.now());
+        return (fxNow = Date.now());
     }
 
     // Generate parameters to create a standard animation
     function genFx(type, includeWidth) {
         var which,
+            i = 0,
             attrs = {
                 height: type
-            },
-            i = 0;
+            };
 
-        // if we include width, step value is 1 to do all cssExpand values,
-        // if we don't include width, step value is 2 to skip over Left and Right
+        // If we include width, step value is 1 to do all cssExpand values,
+        // otherwise step value is 2 to skip over Left and Right
         includeWidth = includeWidth ? 1 : 0;
         for (; i < 4; i += 2 - includeWidth) {
             which = cssExpand[i];
             attrs["margin" + which] = attrs["padding" + which] = type;
         }
 
         if (includeWidth) {
@@ -7135,193 +7390,225 @@
         }
 
         return attrs;
     }
 
     function createTween(value, prop, animation) {
         var tween,
-            collection = (tweeners[prop] || []).concat(tweeners["*"]),
+            collection = (Animation.tweeners[prop] || []).concat(Animation.tweeners["*"]),
             index = 0,
             length = collection.length;
         for (; index < length; index++) {
             if ((tween = collection[index].call(animation, prop, value))) {
 
-                // we're done with this property
+                // We're done with this property
                 return tween;
             }
         }
     }
 
     function defaultPrefilter(elem, props, opts) {
-        /* jshint validthis: true */
-        var prop, value, toggle, tween, hooks, oldfire, display, checkDisplay,
+        var prop, value, toggle, hooks, oldfire, propTween, restoreDisplay, display,
+            isBox = "width" in props || "height" in props,
             anim = this,
             orig = {},
             style = elem.style,
-            hidden = elem.nodeType && isHidden(elem),
-            dataShow = jQuery._data(elem, "fxshow");
+            hidden = elem.nodeType && isHiddenWithinTree(elem),
+            dataShow = dataPriv.get(elem, "fxshow");
 
-        // handle queue: false promises
+        // Queue-skipping animations hijack the fx hooks
         if (!opts.queue) {
             hooks = jQuery._queueHooks(elem, "fx");
             if (hooks.unqueued == null) {
                 hooks.unqueued = 0;
                 oldfire = hooks.empty.fire;
                 hooks.empty.fire = function() {
                     if (!hooks.unqueued) {
                         oldfire();
                     }
                 };
             }
             hooks.unqueued++;
 
             anim.always(function() {
-                // doing this makes sure that the complete handler will be called
-                // before this completes
+
+                // Ensure the complete handler is called before this completes
                 anim.always(function() {
                     hooks.unqueued--;
                     if (!jQuery.queue(elem, "fx").length) {
                         hooks.empty.fire();
                     }
                 });
             });
         }
 
-        // height/width overflow pass
-        if (elem.nodeType === 1 && ("height" in props || "width" in props)) {
-            // Make sure that nothing sneaks out
-            // Record all 3 overflow attributes because IE does not
-            // change the overflow attribute when overflowX and
-            // overflowY are set to the same value
-            opts.overflow = [style.overflow, style.overflowX, style.overflowY];
-
-            // Set display property to inline-block for height/width
-            // animations on inline elements that are having width/height animated
-            display = jQuery.css(elem, "display");
-
-            // Test default display if display is currently "none"
-            checkDisplay = display === "none" ?
-                jQuery._data(elem, "olddisplay") || defaultDisplay(elem.nodeName) : display;
-
-            if (checkDisplay === "inline" && jQuery.css(elem, "float") === "none") {
-
-                // inline-level elements accept inline-block;
-                // block-level elements need to be inline with layout
-                if (!support.inlineBlockNeedsLayout || defaultDisplay(elem.nodeName) === "inline") {
-                    style.display = "inline-block";
-                } else {
-                    style.zoom = 1;
-                }
-            }
-        }
-
-        if (opts.overflow) {
-            style.overflow = "hidden";
-            if (!support.shrinkWrapBlocks()) {
-                anim.always(function() {
-                    style.overflow = opts.overflow[0];
-                    style.overflowX = opts.overflow[1];
-                    style.overflowY = opts.overflow[2];
-                });
-            }
-        }
-
-        // show/hide pass
+        // Detect show/hide animations
         for (prop in props) {
             value = props[prop];
-            if (rfxtypes.exec(value)) {
+            if (rfxtypes.test(value)) {
                 delete props[prop];
                 toggle = toggle || value === "toggle";
                 if (value === (hidden ? "hide" : "show")) {
 
-                    // If there is dataShow left over from a stopped hide or show and we are going to proceed with show, we should pretend to be hidden
+                    // Pretend to be hidden if this is a "show" and
+                    // there is still data from a stopped show/hide
                     if (value === "show" && dataShow && dataShow[prop] !== undefined) {
                         hidden = true;
+
+                        // Ignore all other no-op show/hide data
                     } else {
                         continue;
                     }
                 }
                 orig[prop] = dataShow && dataShow[prop] || jQuery.style(elem, prop);
-
-                // Any non-fx value stops us from restoring the original display value
-            } else {
-                display = undefined;
             }
         }
 
-        if (!jQuery.isEmptyObject(orig)) {
-            if (dataShow) {
-                if ("hidden" in dataShow) {
-                    hidden = dataShow.hidden;
-                }
-            } else {
-                dataShow = jQuery._data(elem, "fxshow", {});
-            }
+        // Bail out if this is a no-op like .hide().hide()
+        propTween = !jQuery.isEmptyObject(props);
+        if (!propTween && jQuery.isEmptyObject(orig)) {
+            return;
+        }
+
+        // Restrict "overflow" and "display" styles during box animations
+        if (isBox && elem.nodeType === 1) {
+
+            // Support: IE <=9 - 11, Edge 12 - 15
+            // Record all 3 overflow attributes because IE does not infer the shorthand
+            // from identically-valued overflowX and overflowY and Edge just mirrors
+            // the overflowX value there.
+            opts.overflow = [style.overflow, style.overflowX, style.overflowY];
 
-            // store state if its toggle - enables .stop().toggle() to "reverse"
-            if (toggle) {
-                dataShow.hidden = !hidden;
+            // Identify a display type, preferring old show/hide data over the CSS cascade
+            restoreDisplay = dataShow && dataShow.display;
+            if (restoreDisplay == null) {
+                restoreDisplay = dataPriv.get(elem, "display");
             }
-            if (hidden) {
-                jQuery(elem).show();
-            } else {
-                anim.done(function() {
-                    jQuery(elem).hide();
-                });
+            display = jQuery.css(elem, "display");
+            if (display === "none") {
+                if (restoreDisplay) {
+                    display = restoreDisplay;
+                } else {
+
+                    // Get nonempty value(s) by temporarily forcing visibility
+                    showHide([elem], true);
+                    restoreDisplay = elem.style.display || restoreDisplay;
+                    display = jQuery.css(elem, "display");
+                    showHide([elem]);
+                }
             }
-            anim.done(function() {
-                var prop;
-                jQuery._removeData(elem, "fxshow");
-                for (prop in orig) {
-                    jQuery.style(elem, prop, orig[prop]);
+
+            // Animate inline elements as inline-block
+            if (display === "inline" || display === "inline-block" && restoreDisplay != null) {
+                if (jQuery.css(elem, "float") === "none") {
+
+                    // Restore the original display value at the end of pure show/hide animations
+                    if (!propTween) {
+                        anim.done(function() {
+                            style.display = restoreDisplay;
+                        });
+                        if (restoreDisplay == null) {
+                            display = style.display;
+                            restoreDisplay = display === "none" ? "" : display;
+                        }
+                    }
+                    style.display = "inline-block";
                 }
+            }
+        }
+
+        if (opts.overflow) {
+            style.overflow = "hidden";
+            anim.always(function() {
+                style.overflow = opts.overflow[0];
+                style.overflowX = opts.overflow[1];
+                style.overflowY = opts.overflow[2];
             });
-            for (prop in orig) {
-                tween = createTween(hidden ? dataShow[prop] : 0, prop, anim);
+        }
 
-                if (!(prop in dataShow)) {
-                    dataShow[prop] = tween.start;
-                    if (hidden) {
-                        tween.end = tween.start;
-                        tween.start = prop === "width" || prop === "height" ? 1 : 0;
+        // Implement show/hide animations
+        propTween = false;
+        for (prop in orig) {
+
+            // General show/hide setup for this element animation
+            if (!propTween) {
+                if (dataShow) {
+                    if ("hidden" in dataShow) {
+                        hidden = dataShow.hidden;
                     }
+                } else {
+                    dataShow = dataPriv.access(elem, "fxshow", {
+                        display: restoreDisplay
+                    });
                 }
+
+                // Store hidden/visible for toggle so `.stop().toggle()` "reverses"
+                if (toggle) {
+                    dataShow.hidden = !hidden;
+                }
+
+                // Show elements before animating them
+                if (hidden) {
+                    showHide([elem], true);
+                }
+
+                /* eslint-disable no-loop-func */
+
+                anim.done(function() {
+
+                    /* eslint-enable no-loop-func */
+
+                    // The final step of a "hide" animation is actually hiding the element
+                    if (!hidden) {
+                        showHide([elem]);
+                    }
+                    dataPriv.remove(elem, "fxshow");
+                    for (prop in orig) {
+                        jQuery.style(elem, prop, orig[prop]);
+                    }
+                });
             }
 
-            // If this is a noop like .hide().hide(), restore an overwritten display value
-        } else if ((display === "none" ? defaultDisplay(elem.nodeName) : display) === "inline") {
-            style.display = display;
+            // Per-property setup
+            propTween = createTween(hidden ? dataShow[prop] : 0, prop, anim);
+            if (!(prop in dataShow)) {
+                dataShow[prop] = propTween.start;
+                if (hidden) {
+                    propTween.end = propTween.start;
+                    propTween.start = 0;
+                }
+            }
         }
     }
 
     function propFilter(props, specialEasing) {
         var index, name, easing, value, hooks;
 
         // camelCase, specialEasing and expand cssHook pass
         for (index in props) {
-            name = jQuery.camelCase(index);
+            name = camelCase(index);
             easing = specialEasing[name];
             value = props[index];
-            if (jQuery.isArray(value)) {
+            if (Array.isArray(value)) {
                 easing = value[1];
                 value = props[index] = value[0];
             }
 
             if (index !== name) {
                 props[name] = value;
                 delete props[index];
             }
 
             hooks = jQuery.cssHooks[name];
             if (hooks && "expand" in hooks) {
                 value = hooks.expand(value);
                 delete props[name];
 
-                // not quite $.extend, this wont overwrite keys already present.
-                // also - reusing 'index' from above because we have the correct "name"
+                // Not quite $.extend, this won't overwrite existing keys.
+                // Reusing 'index' because we have the correct "name"
                 for (index in value) {
                     if (!(index in props)) {
                         props[index] = value[index];
                         specialEasing[index] = easing;
                     }
                 }
             } else {
@@ -7330,200 +7617,244 @@
         }
     }
 
     function Animation(elem, properties, options) {
         var result,
             stopped,
             index = 0,
-            length = animationPrefilters.length,
+            length = Animation.prefilters.length,
             deferred = jQuery.Deferred().always(function() {
-                // don't match elem in the :animated selector
+
+                // Don't match elem in the :animated selector
                 delete tick.elem;
             }),
             tick = function() {
                 if (stopped) {
                     return false;
                 }
                 var currentTime = fxNow || createFxNow(),
                     remaining = Math.max(0, animation.startTime + animation.duration - currentTime),
-                    // archaic crash bug won't allow us to use 1 - ( 0.5 || 0 ) (#12497)
+
+                    // Support: Android 2.3 only
+                    // Archaic crash bug won't allow us to use `1 - ( 0.5 || 0 )` (trac-12497)
                     temp = remaining / animation.duration || 0,
                     percent = 1 - temp,
                     index = 0,
                     length = animation.tweens.length;
 
                 for (; index < length; index++) {
                     animation.tweens[index].run(percent);
                 }
 
                 deferred.notifyWith(elem, [animation, percent, remaining]);
 
+                // If there's more to do, yield
                 if (percent < 1 && length) {
                     return remaining;
-                } else {
-                    deferred.resolveWith(elem, [animation]);
-                    return false;
                 }
+
+                // If this was an empty animation, synthesize a final progress notification
+                if (!length) {
+                    deferred.notifyWith(elem, [animation, 1, 0]);
+                }
+
+                // Resolve the animation and report its conclusion
+                deferred.resolveWith(elem, [animation]);
+                return false;
             },
             animation = deferred.promise({
                 elem: elem,
                 props: jQuery.extend({}, properties),
                 opts: jQuery.extend(true, {
-                    specialEasing: {}
+                    specialEasing: {},
+                    easing: jQuery.easing._default
                 }, options),
                 originalProperties: properties,
                 originalOptions: options,
                 startTime: fxNow || createFxNow(),
                 duration: options.duration,
                 tweens: [],
                 createTween: function(prop, end) {
                     var tween = jQuery.Tween(elem, animation.opts, prop, end,
                         animation.opts.specialEasing[prop] || animation.opts.easing);
                     animation.tweens.push(tween);
                     return tween;
                 },
                 stop: function(gotoEnd) {
                     var index = 0,
-                        // if we are going to the end, we want to run all the tweens
+
+                        // If we are going to the end, we want to run all the tweens
                         // otherwise we skip this part
                         length = gotoEnd ? animation.tweens.length : 0;
                     if (stopped) {
                         return this;
                     }
                     stopped = true;
                     for (; index < length; index++) {
                         animation.tweens[index].run(1);
                     }
 
-                    // resolve when we played the last frame
-                    // otherwise, reject
+                    // Resolve when we played the last frame; otherwise, reject
                     if (gotoEnd) {
+                        deferred.notifyWith(elem, [animation, 1, 0]);
                         deferred.resolveWith(elem, [animation, gotoEnd]);
                     } else {
                         deferred.rejectWith(elem, [animation, gotoEnd]);
                     }
                     return this;
                 }
             }),
             props = animation.props;
 
         propFilter(props, animation.opts.specialEasing);
 
         for (; index < length; index++) {
-            result = animationPrefilters[index].call(animation, elem, props, animation.opts);
+            result = Animation.prefilters[index].call(animation, elem, props, animation.opts);
             if (result) {
+                if (isFunction(result.stop)) {
+                    jQuery._queueHooks(animation.elem, animation.opts.queue).stop =
+                        result.stop.bind(result);
+                }
                 return result;
             }
         }
 
         jQuery.map(props, createTween, animation);
 
-        if (jQuery.isFunction(animation.opts.start)) {
+        if (isFunction(animation.opts.start)) {
             animation.opts.start.call(elem, animation);
         }
 
+        // Attach callbacks from options
+        animation
+            .progress(animation.opts.progress)
+            .done(animation.opts.done, animation.opts.complete)
+            .fail(animation.opts.fail)
+            .always(animation.opts.always);
+
         jQuery.fx.timer(
             jQuery.extend(tick, {
                 elem: elem,
                 anim: animation,
                 queue: animation.opts.queue
             })
         );
 
-        // attach callbacks from options
-        return animation.progress(animation.opts.progress)
-            .done(animation.opts.done, animation.opts.complete)
-            .fail(animation.opts.fail)
-            .always(animation.opts.always);
+        return animation;
     }
 
     jQuery.Animation = jQuery.extend(Animation, {
+
+        tweeners: {
+            "*": [function(prop, value) {
+                var tween = this.createTween(prop, value);
+                adjustCSS(tween.elem, prop, rcssNum.exec(value), tween);
+                return tween;
+            }]
+        },
+
         tweener: function(props, callback) {
-            if (jQuery.isFunction(props)) {
+            if (isFunction(props)) {
                 callback = props;
                 props = ["*"];
             } else {
-                props = props.split(" ");
+                props = props.match(rnothtmlwhite);
             }
 
             var prop,
                 index = 0,
                 length = props.length;
 
             for (; index < length; index++) {
                 prop = props[index];
-                tweeners[prop] = tweeners[prop] || [];
-                tweeners[prop].unshift(callback);
+                Animation.tweeners[prop] = Animation.tweeners[prop] || [];
+                Animation.tweeners[prop].unshift(callback);
             }
         },
 
+        prefilters: [defaultPrefilter],
+
         prefilter: function(callback, prepend) {
             if (prepend) {
-                animationPrefilters.unshift(callback);
+                Animation.prefilters.unshift(callback);
             } else {
-                animationPrefilters.push(callback);
+                Animation.prefilters.push(callback);
             }
         }
     });
 
     jQuery.speed = function(speed, easing, fn) {
         var opt = speed && typeof speed === "object" ? jQuery.extend({}, speed) : {
             complete: fn || !fn && easing ||
-                jQuery.isFunction(speed) && speed,
+                isFunction(speed) && speed,
             duration: speed,
-            easing: fn && easing || easing && !jQuery.isFunction(easing) && easing
+            easing: fn && easing || easing && !isFunction(easing) && easing
         };
 
-        opt.duration = jQuery.fx.off ? 0 : typeof opt.duration === "number" ? opt.duration :
-            opt.duration in jQuery.fx.speeds ? jQuery.fx.speeds[opt.duration] : jQuery.fx.speeds._default;
+        // Go to the end state if fx are off
+        if (jQuery.fx.off) {
+            opt.duration = 0;
+
+        } else {
+            if (typeof opt.duration !== "number") {
+                if (opt.duration in jQuery.fx.speeds) {
+                    opt.duration = jQuery.fx.speeds[opt.duration];
+
+                } else {
+                    opt.duration = jQuery.fx.speeds._default;
+                }
+            }
+        }
 
-        // normalize opt.queue - true/undefined/null -> "fx"
+        // Normalize opt.queue - true/undefined/null -> "fx"
         if (opt.queue == null || opt.queue === true) {
             opt.queue = "fx";
         }
 
         // Queueing
         opt.old = opt.complete;
 
         opt.complete = function() {
-            if (jQuery.isFunction(opt.old)) {
+            if (isFunction(opt.old)) {
                 opt.old.call(this);
             }
 
             if (opt.queue) {
                 jQuery.dequeue(this, opt.queue);
             }
         };
 
         return opt;
     };
 
     jQuery.fn.extend({
         fadeTo: function(speed, to, easing, callback) {
 
-            // show any hidden elements after setting opacity to 0
-            return this.filter(isHidden).css("opacity", 0).show()
+            // Show any hidden elements after setting opacity to 0
+            return this.filter(isHiddenWithinTree).css("opacity", 0).show()
 
-                // animate to the value specified
+                // Animate to the value specified
                 .end().animate({
                     opacity: to
                 }, speed, easing, callback);
         },
         animate: function(prop, speed, easing, callback) {
             var empty = jQuery.isEmptyObject(prop),
                 optall = jQuery.speed(speed, easing, callback),
                 doAnimation = function() {
+
                     // Operate on a copy of prop so per-property easing won't be lost
                     var anim = Animation(this, jQuery.extend({}, prop), optall);
 
                     // Empty animations, or finishing resolves immediately
-                    if (empty || jQuery._data(this, "finish")) {
+                    if (empty || dataPriv.get(this, "finish")) {
                         anim.stop(true);
                     }
                 };
+
             doAnimation.finish = doAnimation;
 
             return empty || optall.queue === false ?
                 this.each(doAnimation) :
                 this.queue(optall.queue, doAnimation);
         },
         stop: function(type, clearQueue, gotoEnd) {
@@ -7534,96 +7865,98 @@
             };
 
             if (typeof type !== "string") {
                 gotoEnd = clearQueue;
                 clearQueue = type;
                 type = undefined;
             }
-            if (clearQueue && type !== false) {
+            if (clearQueue) {
                 this.queue(type || "fx", []);
             }
 
             return this.each(function() {
                 var dequeue = true,
                     index = type != null && type + "queueHooks",
                     timers = jQuery.timers,
-                    data = jQuery._data(this);
+                    data = dataPriv.get(this);
 
                 if (index) {
                     if (data[index] && data[index].stop) {
                         stopQueue(data[index]);
                     }
                 } else {
                     for (index in data) {
                         if (data[index] && data[index].stop && rrun.test(index)) {
                             stopQueue(data[index]);
                         }
                     }
                 }
 
                 for (index = timers.length; index--;) {
-                    if (timers[index].elem === this && (type == null || timers[index].queue === type)) {
+                    if (timers[index].elem === this &&
+                        (type == null || timers[index].queue === type)) {
+
                         timers[index].anim.stop(gotoEnd);
                         dequeue = false;
                         timers.splice(index, 1);
                     }
                 }
 
-                // start the next in the queue if the last step wasn't forced
-                // timers currently will call their complete callbacks, which will dequeue
-                // but only if they were gotoEnd
+                // Start the next in the queue if the last step wasn't forced.
+                // Timers currently will call their complete callbacks, which
+                // will dequeue but only if they were gotoEnd.
                 if (dequeue || !gotoEnd) {
                     jQuery.dequeue(this, type);
                 }
             });
         },
         finish: function(type) {
             if (type !== false) {
                 type = type || "fx";
             }
             return this.each(function() {
                 var index,
-                    data = jQuery._data(this),
+                    data = dataPriv.get(this),
                     queue = data[type + "queue"],
                     hooks = data[type + "queueHooks"],
                     timers = jQuery.timers,
                     length = queue ? queue.length : 0;
 
-                // enable finishing flag on private data
+                // Enable finishing flag on private data
                 data.finish = true;
 
-                // empty the queue first
+                // Empty the queue first
                 jQuery.queue(this, type, []);
 
                 if (hooks && hooks.stop) {
                     hooks.stop.call(this, true);
                 }
 
-                // look for any active animations, and finish them
+                // Look for any active animations, and finish them
                 for (index = timers.length; index--;) {
                     if (timers[index].elem === this && timers[index].queue === type) {
                         timers[index].anim.stop(true);
                         timers.splice(index, 1);
                     }
                 }
 
-                // look for any animations in the old queue and finish them
+                // Look for any animations in the old queue and finish them
                 for (index = 0; index < length; index++) {
                     if (queue[index] && queue[index].finish) {
                         queue[index].finish.call(this);
                     }
                 }
 
-                // turn off finishing flag
+                // Turn off finishing flag
                 delete data.finish;
             });
         }
     });
 
-    jQuery.each(["toggle", "show", "hide"], function(i, name) {
+    jQuery.each(["toggle", "show", "hide"], function(_i, name) {
         var cssFn = jQuery.fn[name];
         jQuery.fn[name] = function(speed, easing, callback) {
             return speed == null || typeof speed === "boolean" ?
                 cssFn.apply(this, arguments) :
                 this.animate(genFx(name, true), speed, easing, callback);
         };
     });
@@ -7647,313 +7980,102 @@
             return this.animate(props, speed, easing, callback);
         };
     });
 
     jQuery.timers = [];
     jQuery.fx.tick = function() {
         var timer,
-            timers = jQuery.timers,
-            i = 0;
+            i = 0,
+            timers = jQuery.timers;
 
-        fxNow = jQuery.now();
+        fxNow = Date.now();
 
         for (; i < timers.length; i++) {
             timer = timers[i];
-            // Checks the timer has not already been removed
+
+            // Run the timer and safely remove it when done (allowing for external removal)
             if (!timer() && timers[i] === timer) {
                 timers.splice(i--, 1);
             }
         }
 
         if (!timers.length) {
             jQuery.fx.stop();
         }
         fxNow = undefined;
     };
 
     jQuery.fx.timer = function(timer) {
         jQuery.timers.push(timer);
-        if (timer()) {
-            jQuery.fx.start();
-        } else {
-            jQuery.timers.pop();
-        }
+        jQuery.fx.start();
     };
 
     jQuery.fx.interval = 13;
-
     jQuery.fx.start = function() {
-        if (!timerId) {
-            timerId = setInterval(jQuery.fx.tick, jQuery.fx.interval);
+        if (inProgress) {
+            return;
         }
+
+        inProgress = true;
+        schedule();
     };
 
     jQuery.fx.stop = function() {
-        clearInterval(timerId);
-        timerId = null;
+        inProgress = null;
     };
 
     jQuery.fx.speeds = {
         slow: 600,
         fast: 200,
+
         // Default speed
         _default: 400
     };
 
 
     // Based off of the plugin by Clint Helfers, with permission.
-    // http://blindsignals.com/index.php/2009/07/jquery-delay/
     jQuery.fn.delay = function(time, type) {
         time = jQuery.fx ? jQuery.fx.speeds[time] || time : time;
         type = type || "fx";
 
         return this.queue(type, function(next, hooks) {
-            var timeout = setTimeout(next, time);
+            var timeout = window.setTimeout(next, time);
             hooks.stop = function() {
-                clearTimeout(timeout);
+                window.clearTimeout(timeout);
             };
         });
     };
 
 
     (function() {
-        // Minified: var a,b,c,d,e
-        var input, div, select, a, opt;
+        var input = document.createElement("input"),
+            select = document.createElement("select"),
+            opt = select.appendChild(document.createElement("option"));
 
-        // Setup
-        div = document.createElement("div");
-        div.setAttribute("className", "t");
-        div.innerHTML = "  <link/><table></table><a href='/a'>a</a><input type='checkbox'/>";
-        a = div.getElementsByTagName("a")[0];
-
-        // First batch of tests.
-        select = document.createElement("select");
-        opt = select.appendChild(document.createElement("option"));
-        input = div.getElementsByTagName("input")[0];
-
-        a.style.cssText = "top:1px";
-
-        // Test setAttribute on camelCase class. If it works, we need attrFixes when doing get/setAttribute (ie6/7)
-        support.getSetAttribute = div.className !== "t";
-
-        // Get the style information from getAttribute
-        // (IE uses .cssText instead)
-        support.style = /top/.test(a.getAttribute("style"));
-
-        // Make sure that URLs aren't manipulated
-        // (IE normalizes it by default)
-        support.hrefNormalized = a.getAttribute("href") === "/a";
+        input.type = "checkbox";
 
-        // Check the default checkbox/radio value ("" on WebKit; "on" elsewhere)
-        support.checkOn = !!input.value;
+        // Support: Android <=4.3 only
+        // Default value for a checkbox should be "on"
+        support.checkOn = input.value !== "";
 
-        // Make sure that a selected-by-default option has a working selected property.
-        // (WebKit defaults to false instead of true, IE too, if it's in an optgroup)
+        // Support: IE <=11 only
+        // Must access selectedIndex to make default options select
         support.optSelected = opt.selected;
 
-        // Tests for enctype support on a form (#6743)
-        support.enctype = !!document.createElement("form").enctype;
-
-        // Make sure that the options inside disabled selects aren't marked as disabled
-        // (WebKit marks them as disabled)
-        select.disabled = true;
-        support.optDisabled = !opt.disabled;
-
-        // Support: IE8 only
-        // Check if we can trust getAttribute("value")
+        // Support: IE <=11 only
+        // An input loses its value after becoming a radio
         input = document.createElement("input");
-        input.setAttribute("value", "");
-        support.input = input.getAttribute("value") === "";
-
-        // Check if an input maintains its value after becoming a radio
         input.value = "t";
-        input.setAttribute("type", "radio");
+        input.type = "radio";
         support.radioValue = input.value === "t";
     })();
 
 
-    var rreturn = /\r/g;
-
-    jQuery.fn.extend({
-        val: function(value) {
-            var hooks, ret, isFunction,
-                elem = this[0];
-
-            if (!arguments.length) {
-                if (elem) {
-                    hooks = jQuery.valHooks[elem.type] || jQuery.valHooks[elem.nodeName.toLowerCase()];
-
-                    if (hooks && "get" in hooks && (ret = hooks.get(elem, "value")) !== undefined) {
-                        return ret;
-                    }
-
-                    ret = elem.value;
-
-                    return typeof ret === "string" ?
-                        // handle most common string cases
-                        ret.replace(rreturn, "") :
-                        // handle cases where value is null/undef or number
-                        ret == null ? "" : ret;
-                }
-
-                return;
-            }
-
-            isFunction = jQuery.isFunction(value);
-
-            return this.each(function(i) {
-                var val;
-
-                if (this.nodeType !== 1) {
-                    return;
-                }
-
-                if (isFunction) {
-                    val = value.call(this, i, jQuery(this).val());
-                } else {
-                    val = value;
-                }
-
-                // Treat null/undefined as ""; convert numbers to string
-                if (val == null) {
-                    val = "";
-                } else if (typeof val === "number") {
-                    val += "";
-                } else if (jQuery.isArray(val)) {
-                    val = jQuery.map(val, function(value) {
-                        return value == null ? "" : value + "";
-                    });
-                }
-
-                hooks = jQuery.valHooks[this.type] || jQuery.valHooks[this.nodeName.toLowerCase()];
-
-                // If set returns undefined, fall back to normal setting
-                if (!hooks || !("set" in hooks) || hooks.set(this, val, "value") === undefined) {
-                    this.value = val;
-                }
-            });
-        }
-    });
-
-    jQuery.extend({
-        valHooks: {
-            option: {
-                get: function(elem) {
-                    var val = jQuery.find.attr(elem, "value");
-                    return val != null ?
-                        val :
-                        // Support: IE10-11+
-                        // option.text throws exceptions (#14686, #14858)
-                        jQuery.trim(jQuery.text(elem));
-                }
-            },
-            select: {
-                get: function(elem) {
-                    var value, option,
-                        options = elem.options,
-                        index = elem.selectedIndex,
-                        one = elem.type === "select-one" || index < 0,
-                        values = one ? null : [],
-                        max = one ? index + 1 : options.length,
-                        i = index < 0 ?
-                        max :
-                        one ? index : 0;
-
-                    // Loop through all the selected options
-                    for (; i < max; i++) {
-                        option = options[i];
-
-                        // oldIE doesn't update selected after form reset (#2551)
-                        if ((option.selected || i === index) &&
-                            // Don't return options that are disabled or in a disabled optgroup
-                            (support.optDisabled ? !option.disabled : option.getAttribute("disabled") === null) &&
-                            (!option.parentNode.disabled || !jQuery.nodeName(option.parentNode, "optgroup"))) {
-
-                            // Get the specific value for the option
-                            value = jQuery(option).val();
-
-                            // We don't need an array for one selects
-                            if (one) {
-                                return value;
-                            }
-
-                            // Multi-Selects return an array
-                            values.push(value);
-                        }
-                    }
-
-                    return values;
-                },
-
-                set: function(elem, value) {
-                    var optionSet, option,
-                        options = elem.options,
-                        values = jQuery.makeArray(value),
-                        i = options.length;
-
-                    while (i--) {
-                        option = options[i];
-
-                        if (jQuery.inArray(jQuery.valHooks.option.get(option), values) >= 0) {
-
-                            // Support: IE6
-                            // When new option element is added to select box we need to
-                            // force reflow of newly added node in order to workaround delay
-                            // of initialization properties
-                            try {
-                                option.selected = optionSet = true;
-
-                            } catch (_) {
-
-                                // Will be executed only in IE6
-                                option.scrollHeight;
-                            }
-
-                        } else {
-                            option.selected = false;
-                        }
-                    }
-
-                    // Force browsers to behave consistently when non-matching value is set
-                    if (!optionSet) {
-                        elem.selectedIndex = -1;
-                    }
-
-                    return options;
-                }
-            }
-        }
-    });
-
-    // Radios and checkboxes getter/setter
-    jQuery.each(["radio", "checkbox"], function() {
-        jQuery.valHooks[this] = {
-            set: function(elem, value) {
-                if (jQuery.isArray(value)) {
-                    return (elem.checked = jQuery.inArray(jQuery(elem).val(), value) >= 0);
-                }
-            }
-        };
-        if (!support.checkOn) {
-            jQuery.valHooks[this].get = function(elem) {
-                // Support: Webkit
-                // "" is returned instead of "on" if a value isn't specified
-                return elem.getAttribute("value") === null ? "on" : elem.value;
-            };
-        }
-    });
-
-
-
-
-    var nodeHook, boolHook,
-        attrHandle = jQuery.expr.attrHandle,
-        ruseDefault = /^(?:checked|selected)$/i,
-        getSetAttribute = support.getSetAttribute,
-        getSetInput = support.input;
+    var boolHook,
+        attrHandle = jQuery.expr.attrHandle;
 
     jQuery.fn.extend({
         attr: function(name, value) {
             return access(this, jQuery.attr, name, value, arguments.length > 1);
         },
 
         removeAttr: function(name) {
@@ -7961,360 +8083,242 @@
                 jQuery.removeAttr(this, name);
             });
         }
     });
 
     jQuery.extend({
         attr: function(elem, name, value) {
-            var hooks, ret,
+            var ret, hooks,
                 nType = elem.nodeType;
 
-            // don't get/set attributes on text, comment and attribute nodes
-            if (!elem || nType === 3 || nType === 8 || nType === 2) {
+            // Don't get/set attributes on text, comment and attribute nodes
+            if (nType === 3 || nType === 8 || nType === 2) {
                 return;
             }
 
             // Fallback to prop when attributes are not supported
-            if (typeof elem.getAttribute === strundefined) {
+            if (typeof elem.getAttribute === "undefined") {
                 return jQuery.prop(elem, name, value);
             }
 
-            // All attributes are lowercase
+            // Attribute hooks are determined by the lowercase version
             // Grab necessary hook if one is defined
             if (nType !== 1 || !jQuery.isXMLDoc(elem)) {
-                name = name.toLowerCase();
-                hooks = jQuery.attrHooks[name] ||
-                    (jQuery.expr.match.bool.test(name) ? boolHook : nodeHook);
+                hooks = jQuery.attrHooks[name.toLowerCase()] ||
+                    (jQuery.expr.match.bool.test(name) ? boolHook : undefined);
             }
 
             if (value !== undefined) {
-
                 if (value === null) {
                     jQuery.removeAttr(elem, name);
+                    return;
+                }
 
-                } else if (hooks && "set" in hooks && (ret = hooks.set(elem, value, name)) !== undefined) {
+                if (hooks && "set" in hooks &&
+                    (ret = hooks.set(elem, value, name)) !== undefined) {
                     return ret;
-
-                } else {
-                    elem.setAttribute(name, value + "");
-                    return value;
                 }
 
-            } else if (hooks && "get" in hooks && (ret = hooks.get(elem, name)) !== null) {
-                return ret;
-
-            } else {
-                ret = jQuery.find.attr(elem, name);
-
-                // Non-existent attributes return null, we normalize to undefined
-                return ret == null ?
-                    undefined :
-                    ret;
+                elem.setAttribute(name, value + "");
+                return value;
             }
-        },
-
-        removeAttr: function(elem, value) {
-            var name, propName,
-                i = 0,
-                attrNames = value && value.match(rnotwhite);
-
-            if (attrNames && elem.nodeType === 1) {
-                while ((name = attrNames[i++])) {
-                    propName = jQuery.propFix[name] || name;
 
-                    // Boolean attributes get special treatment (#10870)
-                    if (jQuery.expr.match.bool.test(name)) {
-                        // Set corresponding property to false
-                        if (getSetInput && getSetAttribute || !ruseDefault.test(name)) {
-                            elem[propName] = false;
-                            // Support: IE<9
-                            // Also clear defaultChecked/defaultSelected (if appropriate)
-                        } else {
-                            elem[jQuery.camelCase("default-" + name)] =
-                                elem[propName] = false;
-                        }
+            if (hooks && "get" in hooks && (ret = hooks.get(elem, name)) !== null) {
+                return ret;
+            }
 
-                        // See #9699 for explanation of this approach (setting first, then removal)
-                    } else {
-                        jQuery.attr(elem, name, "");
-                    }
+            ret = jQuery.find.attr(elem, name);
 
-                    elem.removeAttribute(getSetAttribute ? name : propName);
-                }
-            }
+            // Non-existent attributes return null, we normalize to undefined
+            return ret == null ? undefined : ret;
         },
 
         attrHooks: {
             type: {
                 set: function(elem, value) {
-                    if (!support.radioValue && value === "radio" && jQuery.nodeName(elem, "input")) {
-                        // Setting the type on a radio button after the value resets the value in IE6-9
-                        // Reset value to default in case type is set after value during creation
+                    if (!support.radioValue && value === "radio" &&
+                        nodeName(elem, "input")) {
                         var val = elem.value;
                         elem.setAttribute("type", value);
                         if (val) {
                             elem.value = val;
                         }
                         return value;
                     }
                 }
             }
+        },
+
+        removeAttr: function(elem, value) {
+            var name,
+                i = 0,
+
+                // Attribute names can contain non-HTML whitespace characters
+                // https://html.spec.whatwg.org/multipage/syntax.html#attributes-2
+                attrNames = value && value.match(rnothtmlwhite);
+
+            if (attrNames && elem.nodeType === 1) {
+                while ((name = attrNames[i++])) {
+                    elem.removeAttribute(name);
+                }
+            }
         }
     });
 
-    // Hook for boolean attributes
+    // Hooks for boolean attributes
     boolHook = {
         set: function(elem, value, name) {
             if (value === false) {
+
                 // Remove boolean attributes when set to false
                 jQuery.removeAttr(elem, name);
-            } else if (getSetInput && getSetAttribute || !ruseDefault.test(name)) {
-                // IE<8 needs the *property* name
-                elem.setAttribute(!getSetAttribute && jQuery.propFix[name] || name, name);
-
-                // Use defaultChecked and defaultSelected for oldIE
             } else {
-                elem[jQuery.camelCase("default-" + name)] = elem[name] = true;
+                elem.setAttribute(name, name);
             }
-
             return name;
         }
     };
 
-    // Retrieve booleans specially
-    jQuery.each(jQuery.expr.match.bool.source.match(/\w+/g), function(i, name) {
-
+    jQuery.each(jQuery.expr.match.bool.source.match(/\w+/g), function(_i, name) {
         var getter = attrHandle[name] || jQuery.find.attr;
 
-        attrHandle[name] = getSetInput && getSetAttribute || !ruseDefault.test(name) ?
-            function(elem, name, isXML) {
-                var ret, handle;
-                if (!isXML) {
-                    // Avoid an infinite loop by temporarily removing this function from the getter
-                    handle = attrHandle[name];
-                    attrHandle[name] = ret;
-                    ret = getter(elem, name, isXML) != null ?
-                        name.toLowerCase() :
-                        null;
-                    attrHandle[name] = handle;
-                }
-                return ret;
-            } :
-            function(elem, name, isXML) {
-                if (!isXML) {
-                    return elem[jQuery.camelCase("default-" + name)] ?
-                        name.toLowerCase() :
-                        null;
-                }
-            };
-    });
-
-    // fix oldIE attroperties
-    if (!getSetInput || !getSetAttribute) {
-        jQuery.attrHooks.value = {
-            set: function(elem, value, name) {
-                if (jQuery.nodeName(elem, "input")) {
-                    // Does not return so that setAttribute is also used
-                    elem.defaultValue = value;
-                } else {
-                    // Use nodeHook if defined (#1954); otherwise setAttribute is fine
-                    return nodeHook && nodeHook.set(elem, value, name);
-                }
-            }
-        };
-    }
-
-    // IE6/7 do not support getting/setting some attributes with get/setAttribute
-    if (!getSetAttribute) {
-
-        // Use this for any attribute in IE6/7
-        // This fixes almost every IE6/7 issue
-        nodeHook = {
-            set: function(elem, value, name) {
-                // Set the existing or create a new attribute node
-                var ret = elem.getAttributeNode(name);
-                if (!ret) {
-                    elem.setAttributeNode(
-                        (ret = elem.ownerDocument.createAttribute(name))
-                    );
-                }
-
-                ret.value = value += "";
-
-                // Break association with cloned elements by also using setAttribute (#9646)
-                if (name === "value" || value === elem.getAttribute(name)) {
-                    return value;
-                }
-            }
-        };
-
-        // Some attributes are constructed with empty-string values when not defined
-        attrHandle.id = attrHandle.name = attrHandle.coords =
-            function(elem, name, isXML) {
-                var ret;
-                if (!isXML) {
-                    return (ret = elem.getAttributeNode(name)) && ret.value !== "" ?
-                        ret.value :
-                        null;
-                }
-            };
-
-        // Fixing value retrieval on a button requires this module
-        jQuery.valHooks.button = {
-            get: function(elem, name) {
-                var ret = elem.getAttributeNode(name);
-                if (ret && ret.specified) {
-                    return ret.value;
-                }
-            },
-            set: nodeHook.set
-        };
-
-        // Set contenteditable to false on removals(#10429)
-        // Setting to empty string throws an error as an invalid value
-        jQuery.attrHooks.contenteditable = {
-            set: function(elem, value, name) {
-                nodeHook.set(elem, value === "" ? false : value, name);
-            }
-        };
-
-        // Set width and height to auto instead of 0 on empty string( Bug #8150 )
-        // This is for removals
-        jQuery.each(["width", "height"], function(i, name) {
-            jQuery.attrHooks[name] = {
-                set: function(elem, value) {
-                    if (value === "") {
-                        elem.setAttribute(name, "auto");
-                        return value;
-                    }
-                }
-            };
-        });
-    }
-
-    if (!support.style) {
-        jQuery.attrHooks.style = {
-            get: function(elem) {
-                // Return undefined in the case of empty string
-                // Note: IE uppercases css property names, but if we were to .toLowerCase()
-                // .cssText, that would destroy case senstitivity in URL's, like in "background"
-                return elem.style.cssText || undefined;
-            },
-            set: function(elem, value) {
-                return (elem.style.cssText = value + "");
+        attrHandle[name] = function(elem, name, isXML) {
+            var ret, handle,
+                lowercaseName = name.toLowerCase();
+
+            if (!isXML) {
+
+                // Avoid an infinite loop by temporarily removing this function from the getter
+                handle = attrHandle[lowercaseName];
+                attrHandle[lowercaseName] = ret;
+                ret = getter(elem, name, isXML) != null ?
+                    lowercaseName :
+                    null;
+                attrHandle[lowercaseName] = handle;
             }
+            return ret;
         };
-    }
+    });
 
 
 
 
-    var rfocusable = /^(?:input|select|textarea|button|object)$/i,
+    var rfocusable = /^(?:input|select|textarea|button)$/i,
         rclickable = /^(?:a|area)$/i;
 
     jQuery.fn.extend({
         prop: function(name, value) {
             return access(this, jQuery.prop, name, value, arguments.length > 1);
         },
 
         removeProp: function(name) {
-            name = jQuery.propFix[name] || name;
             return this.each(function() {
-                // try/catch handles cases where IE balks (such as removing a property on window)
-                try {
-                    this[name] = undefined;
-                    delete this[name];
-                } catch (e) {}
+                delete this[jQuery.propFix[name] || name];
             });
         }
     });
 
     jQuery.extend({
-        propFix: {
-            "for": "htmlFor",
-            "class": "className"
-        },
-
         prop: function(elem, name, value) {
-            var ret, hooks, notxml,
+            var ret, hooks,
                 nType = elem.nodeType;
 
-            // don't get/set properties on text, comment and attribute nodes
-            if (!elem || nType === 3 || nType === 8 || nType === 2) {
+            // Don't get/set properties on text, comment and attribute nodes
+            if (nType === 3 || nType === 8 || nType === 2) {
                 return;
             }
 
-            notxml = nType !== 1 || !jQuery.isXMLDoc(elem);
+            if (nType !== 1 || !jQuery.isXMLDoc(elem)) {
 
-            if (notxml) {
                 // Fix name and attach hooks
                 name = jQuery.propFix[name] || name;
                 hooks = jQuery.propHooks[name];
             }
 
             if (value !== undefined) {
-                return hooks && "set" in hooks && (ret = hooks.set(elem, value, name)) !== undefined ?
-                    ret :
-                    (elem[name] = value);
+                if (hooks && "set" in hooks &&
+                    (ret = hooks.set(elem, value, name)) !== undefined) {
+                    return ret;
+                }
 
-            } else {
-                return hooks && "get" in hooks && (ret = hooks.get(elem, name)) !== null ?
-                    ret :
-                    elem[name];
+                return (elem[name] = value);
+            }
+
+            if (hooks && "get" in hooks && (ret = hooks.get(elem, name)) !== null) {
+                return ret;
             }
+
+            return elem[name];
         },
 
         propHooks: {
             tabIndex: {
                 get: function(elem) {
-                    // elem.tabIndex doesn't always return the correct value when it hasn't been explicitly set
-                    // http://fluidproject.org/blog/2008/01/09/getting-setting-and-removing-tabindex-values-with-javascript/
-                    // Use proper attribute retrieval(#12072)
+
+                    // Support: IE <=9 - 11 only
+                    // elem.tabIndex doesn't always return the
+                    // correct value when it hasn't been explicitly set
+                    // Use proper attribute retrieval (trac-12072)
                     var tabindex = jQuery.find.attr(elem, "tabindex");
 
-                    return tabindex ?
-                        parseInt(tabindex, 10) :
-                        rfocusable.test(elem.nodeName) || rclickable.test(elem.nodeName) && elem.href ?
-                        0 :
-                        -1;
+                    if (tabindex) {
+                        return parseInt(tabindex, 10);
+                    }
+
+                    if (
+                        rfocusable.test(elem.nodeName) ||
+                        rclickable.test(elem.nodeName) &&
+                        elem.href
+                    ) {
+                        return 0;
+                    }
+
+                    return -1;
                 }
             }
+        },
+
+        propFix: {
+            "for": "htmlFor",
+            "class": "className"
         }
     });
 
-    // Some attributes require a special call on IE
-    // http://msdn.microsoft.com/en-us/library/ms536429%28VS.85%29.aspx
-    if (!support.hrefNormalized) {
-        // href/src property should get the full normalized URL (#10299/#12915)
-        jQuery.each(["href", "src"], function(i, name) {
-            jQuery.propHooks[name] = {
-                get: function(elem) {
-                    return elem.getAttribute(name, 4);
-                }
-            };
-        });
-    }
-
-    // Support: Safari, IE9+
-    // mis-reports the default selected property of an option
-    // Accessing the parent's selectedIndex property fixes it
+    // Support: IE <=11 only
+    // Accessing the selectedIndex property
+    // forces the browser to respect setting selected
+    // on the option
+    // The getter ensures a default option is selected
+    // when in an optgroup
+    // eslint rule "no-unused-expressions" is disabled for this code
+    // since it considers such accessions noop
     if (!support.optSelected) {
         jQuery.propHooks.selected = {
             get: function(elem) {
+
+                /* eslint no-unused-expressions: "off" */
+
                 var parent = elem.parentNode;
+                if (parent && parent.parentNode) {
+                    parent.parentNode.selectedIndex;
+                }
+                return null;
+            },
+            set: function(elem) {
+
+                /* eslint no-unused-expressions: "off" */
 
+                var parent = elem.parentNode;
                 if (parent) {
                     parent.selectedIndex;
 
-                    // Make sure that it also works with optgroups, see #5701
                     if (parent.parentNode) {
                         parent.parentNode.selectedIndex;
                     }
                 }
-                return null;
             }
         };
     }
 
     jQuery.each([
         "tabIndex",
         "readOnly",
@@ -8326,300 +8330,791 @@
         "useMap",
         "frameBorder",
         "contentEditable"
     ], function() {
         jQuery.propFix[this.toLowerCase()] = this;
     });
 
-    // IE6/7 call enctype encoding
-    if (!support.enctype) {
-        jQuery.propFix.enctype = "encoding";
-    }
 
 
 
+    // Strip and collapse whitespace according to HTML spec
+    // https://infra.spec.whatwg.org/#strip-and-collapse-ascii-whitespace
+    function stripAndCollapse(value) {
+        var tokens = value.match(rnothtmlwhite) || [];
+        return tokens.join(" ");
+    }
+
 
-    var rclass = /[\t\r\n\f]/g;
+    function getClass(elem) {
+        return elem.getAttribute && elem.getAttribute("class") || "";
+    }
+
+    function classesToArray(value) {
+        if (Array.isArray(value)) {
+            return value;
+        }
+        if (typeof value === "string") {
+            return value.match(rnothtmlwhite) || [];
+        }
+        return [];
+    }
 
     jQuery.fn.extend({
         addClass: function(value) {
-            var classes, elem, cur, clazz, j, finalValue,
-                i = 0,
-                len = this.length,
-                proceed = typeof value === "string" && value;
+            var classNames, cur, curValue, className, i, finalValue;
 
-            if (jQuery.isFunction(value)) {
+            if (isFunction(value)) {
                 return this.each(function(j) {
-                    jQuery(this).addClass(value.call(this, j, this.className));
+                    jQuery(this).addClass(value.call(this, j, getClass(this)));
                 });
             }
 
-            if (proceed) {
-                // The disjunction here is for better compressibility (see removeClass)
-                classes = (value || "").match(rnotwhite) || [];
+            classNames = classesToArray(value);
 
-                for (; i < len; i++) {
-                    elem = this[i];
-                    cur = elem.nodeType === 1 && (elem.className ?
-                        (" " + elem.className + " ").replace(rclass, " ") :
-                        " "
-                    );
+            if (classNames.length) {
+                return this.each(function() {
+                    curValue = getClass(this);
+                    cur = this.nodeType === 1 && (" " + stripAndCollapse(curValue) + " ");
 
                     if (cur) {
-                        j = 0;
-                        while ((clazz = classes[j++])) {
-                            if (cur.indexOf(" " + clazz + " ") < 0) {
-                                cur += clazz + " ";
+                        for (i = 0; i < classNames.length; i++) {
+                            className = classNames[i];
+                            if (cur.indexOf(" " + className + " ") < 0) {
+                                cur += className + " ";
                             }
                         }
 
-                        // only assign if different to avoid unneeded rendering.
-                        finalValue = jQuery.trim(cur);
-                        if (elem.className !== finalValue) {
-                            elem.className = finalValue;
+                        // Only assign if different to avoid unneeded rendering.
+                        finalValue = stripAndCollapse(cur);
+                        if (curValue !== finalValue) {
+                            this.setAttribute("class", finalValue);
                         }
                     }
-                }
+                });
             }
 
             return this;
         },
 
         removeClass: function(value) {
-            var classes, elem, cur, clazz, j, finalValue,
-                i = 0,
-                len = this.length,
-                proceed = arguments.length === 0 || typeof value === "string" && value;
+            var classNames, cur, curValue, className, i, finalValue;
 
-            if (jQuery.isFunction(value)) {
+            if (isFunction(value)) {
                 return this.each(function(j) {
-                    jQuery(this).removeClass(value.call(this, j, this.className));
+                    jQuery(this).removeClass(value.call(this, j, getClass(this)));
                 });
             }
-            if (proceed) {
-                classes = (value || "").match(rnotwhite) || [];
 
-                for (; i < len; i++) {
-                    elem = this[i];
+            if (!arguments.length) {
+                return this.attr("class", "");
+            }
+
+            classNames = classesToArray(value);
+
+            if (classNames.length) {
+                return this.each(function() {
+                    curValue = getClass(this);
+
                     // This expression is here for better compressibility (see addClass)
-                    cur = elem.nodeType === 1 && (elem.className ?
-                        (" " + elem.className + " ").replace(rclass, " ") :
-                        ""
-                    );
+                    cur = this.nodeType === 1 && (" " + stripAndCollapse(curValue) + " ");
 
                     if (cur) {
-                        j = 0;
-                        while ((clazz = classes[j++])) {
+                        for (i = 0; i < classNames.length; i++) {
+                            className = classNames[i];
+
                             // Remove *all* instances
-                            while (cur.indexOf(" " + clazz + " ") >= 0) {
-                                cur = cur.replace(" " + clazz + " ", " ");
+                            while (cur.indexOf(" " + className + " ") > -1) {
+                                cur = cur.replace(" " + className + " ", " ");
                             }
                         }
 
-                        // only assign if different to avoid unneeded rendering.
-                        finalValue = value ? jQuery.trim(cur) : "";
-                        if (elem.className !== finalValue) {
-                            elem.className = finalValue;
+                        // Only assign if different to avoid unneeded rendering.
+                        finalValue = stripAndCollapse(cur);
+                        if (curValue !== finalValue) {
+                            this.setAttribute("class", finalValue);
                         }
                     }
-                }
+                });
             }
 
             return this;
         },
 
         toggleClass: function(value, stateVal) {
-            var type = typeof value;
-
-            if (typeof stateVal === "boolean" && type === "string") {
-                return stateVal ? this.addClass(value) : this.removeClass(value);
-            }
+            var classNames, className, i, self,
+                type = typeof value,
+                isValidValue = type === "string" || Array.isArray(value);
 
-            if (jQuery.isFunction(value)) {
+            if (isFunction(value)) {
                 return this.each(function(i) {
-                    jQuery(this).toggleClass(value.call(this, i, this.className, stateVal), stateVal);
+                    jQuery(this).toggleClass(
+                        value.call(this, i, getClass(this), stateVal),
+                        stateVal
+                    );
                 });
             }
 
+            if (typeof stateVal === "boolean" && isValidValue) {
+                return stateVal ? this.addClass(value) : this.removeClass(value);
+            }
+
+            classNames = classesToArray(value);
+
             return this.each(function() {
-                if (type === "string") {
-                    // toggle individual class names
-                    var className,
-                        i = 0,
-                        self = jQuery(this),
-                        classNames = value.match(rnotwhite) || [];
+                if (isValidValue) {
 
-                    while ((className = classNames[i++])) {
-                        // check each className given, space separated list
+                    // Toggle individual class names
+                    self = jQuery(this);
+
+                    for (i = 0; i < classNames.length; i++) {
+                        className = classNames[i];
+
+                        // Check each className given, space separated list
                         if (self.hasClass(className)) {
                             self.removeClass(className);
                         } else {
                             self.addClass(className);
                         }
                     }
 
                     // Toggle whole class name
-                } else if (type === strundefined || type === "boolean") {
-                    if (this.className) {
-                        // store className if set
-                        jQuery._data(this, "__className__", this.className);
+                } else if (value === undefined || type === "boolean") {
+                    className = getClass(this);
+                    if (className) {
+
+                        // Store className if set
+                        dataPriv.set(this, "__className__", className);
                     }
 
-                    // If the element has a class name or if we're passed "false",
+                    // If the element has a class name or if we're passed `false`,
                     // then remove the whole classname (if there was one, the above saved it).
                     // Otherwise bring back whatever was previously saved (if anything),
                     // falling back to the empty string if nothing was stored.
-                    this.className = this.className || value === false ? "" : jQuery._data(this, "__className__") || "";
+                    if (this.setAttribute) {
+                        this.setAttribute("class",
+                            className || value === false ?
+                            "" :
+                            dataPriv.get(this, "__className__") || ""
+                        );
+                    }
                 }
             });
         },
 
         hasClass: function(selector) {
-            var className = " " + selector + " ",
-                i = 0,
-                l = this.length;
-            for (; i < l; i++) {
-                if (this[i].nodeType === 1 && (" " + this[i].className + " ").replace(rclass, " ").indexOf(className) >= 0) {
+            var className, elem,
+                i = 0;
+
+            className = " " + selector + " ";
+            while ((elem = this[i++])) {
+                if (elem.nodeType === 1 &&
+                    (" " + stripAndCollapse(getClass(elem)) + " ").indexOf(className) > -1) {
                     return true;
                 }
             }
 
             return false;
         }
     });
 
 
 
 
-    // Return jQuery for attributes-only inclusion
+    var rreturn = /\r/g;
 
+    jQuery.fn.extend({
+        val: function(value) {
+            var hooks, ret, valueIsFunction,
+                elem = this[0];
 
-    jQuery.each(("blur focus focusin focusout load resize scroll unload click dblclick " +
-        "mousedown mouseup mousemove mouseover mouseout mouseenter mouseleave " +
-        "change select submit keydown keypress keyup error contextmenu").split(" "), function(i, name) {
-
-        // Handle event binding
-        jQuery.fn[name] = function(data, fn) {
-            return arguments.length > 0 ?
-                this.on(name, null, data, fn) :
-                this.trigger(name);
-        };
-    });
+            if (!arguments.length) {
+                if (elem) {
+                    hooks = jQuery.valHooks[elem.type] ||
+                        jQuery.valHooks[elem.nodeName.toLowerCase()];
 
-    jQuery.fn.extend({
-        hover: function(fnOver, fnOut) {
-            return this.mouseenter(fnOver).mouseleave(fnOut || fnOver);
-        },
+                    if (hooks &&
+                        "get" in hooks &&
+                        (ret = hooks.get(elem, "value")) !== undefined
+                    ) {
+                        return ret;
+                    }
 
-        bind: function(types, data, fn) {
-            return this.on(types, null, data, fn);
-        },
-        unbind: function(types, fn) {
-            return this.off(types, null, fn);
-        },
+                    ret = elem.value;
 
-        delegate: function(selector, types, data, fn) {
-            return this.on(types, selector, data, fn);
-        },
-        undelegate: function(selector, types, fn) {
-            // ( namespace ) or ( selector, types [, fn] )
-            return arguments.length === 1 ? this.off(selector, "**") : this.off(types, selector || "**", fn);
+                    // Handle most common string cases
+                    if (typeof ret === "string") {
+                        return ret.replace(rreturn, "");
+                    }
+
+                    // Handle cases where value is null/undef or number
+                    return ret == null ? "" : ret;
+                }
+
+                return;
+            }
+
+            valueIsFunction = isFunction(value);
+
+            return this.each(function(i) {
+                var val;
+
+                if (this.nodeType !== 1) {
+                    return;
+                }
+
+                if (valueIsFunction) {
+                    val = value.call(this, i, jQuery(this).val());
+                } else {
+                    val = value;
+                }
+
+                // Treat null/undefined as ""; convert numbers to string
+                if (val == null) {
+                    val = "";
+
+                } else if (typeof val === "number") {
+                    val += "";
+
+                } else if (Array.isArray(val)) {
+                    val = jQuery.map(val, function(value) {
+                        return value == null ? "" : value + "";
+                    });
+                }
+
+                hooks = jQuery.valHooks[this.type] || jQuery.valHooks[this.nodeName.toLowerCase()];
+
+                // If set returns undefined, fall back to normal setting
+                if (!hooks || !("set" in hooks) || hooks.set(this, val, "value") === undefined) {
+                    this.value = val;
+                }
+            });
         }
     });
 
+    jQuery.extend({
+        valHooks: {
+            option: {
+                get: function(elem) {
 
-    var nonce = jQuery.now();
+                    var val = jQuery.find.attr(elem, "value");
+                    return val != null ?
+                        val :
 
-    var rquery = (/\?/);
+                        // Support: IE <=10 - 11 only
+                        // option.text throws exceptions (trac-14686, trac-14858)
+                        // Strip and collapse whitespace
+                        // https://html.spec.whatwg.org/#strip-and-collapse-whitespace
+                        stripAndCollapse(jQuery.text(elem));
+                }
+            },
+            select: {
+                get: function(elem) {
+                    var value, option, i,
+                        options = elem.options,
+                        index = elem.selectedIndex,
+                        one = elem.type === "select-one",
+                        values = one ? null : [],
+                        max = one ? index + 1 : options.length;
+
+                    if (index < 0) {
+                        i = max;
+
+                    } else {
+                        i = one ? index : 0;
+                    }
 
+                    // Loop through all the selected options
+                    for (; i < max; i++) {
+                        option = options[i];
 
+                        // Support: IE <=9 only
+                        // IE8-9 doesn't update selected after form reset (trac-2551)
+                        if ((option.selected || i === index) &&
 
-    var rvalidtokens = /(,)|(\[|{)|(}|])|"(?:[^"\\\r\n]|\\["\\\/bfnrt]|\\u[\da-fA-F]{4})*"\s*:?|true|false|null|-?(?!0\d)\d+(?:\.\d+|)(?:[eE][+-]?\d+|)/g;
+                            // Don't return options that are disabled or in a disabled optgroup
+                            !option.disabled &&
+                            (!option.parentNode.disabled ||
+                                !nodeName(option.parentNode, "optgroup"))) {
 
-    jQuery.parseJSON = function(data) {
-        // Attempt to parse using the native JSON parser first
-        if (window.JSON && window.JSON.parse) {
-            // Support: Android 2.3
-            // Workaround failure to string-cast null input
-            return window.JSON.parse(data + "");
+                            // Get the specific value for the option
+                            value = jQuery(option).val();
+
+                            // We don't need an array for one selects
+                            if (one) {
+                                return value;
+                            }
+
+                            // Multi-Selects return an array
+                            values.push(value);
+                        }
+                    }
+
+                    return values;
+                },
+
+                set: function(elem, value) {
+                    var optionSet, option,
+                        options = elem.options,
+                        values = jQuery.makeArray(value),
+                        i = options.length;
+
+                    while (i--) {
+                        option = options[i];
+
+                        /* eslint-disable no-cond-assign */
+
+                        if (option.selected =
+                            jQuery.inArray(jQuery.valHooks.option.get(option), values) > -1
+                        ) {
+                            optionSet = true;
+                        }
+
+                        /* eslint-enable no-cond-assign */
+                    }
+
+                    // Force browsers to behave consistently when non-matching value is set
+                    if (!optionSet) {
+                        elem.selectedIndex = -1;
+                    }
+                    return values;
+                }
+            }
         }
+    });
+
+    // Radios and checkboxes getter/setter
+    jQuery.each(["radio", "checkbox"], function() {
+        jQuery.valHooks[this] = {
+            set: function(elem, value) {
+                if (Array.isArray(value)) {
+                    return (elem.checked = jQuery.inArray(jQuery(elem).val(), value) > -1);
+                }
+            }
+        };
+        if (!support.checkOn) {
+            jQuery.valHooks[this].get = function(elem) {
+                return elem.getAttribute("value") === null ? "on" : elem.value;
+            };
+        }
+    });
+
+
+
+
+    // Return jQuery for attributes-only inclusion
+
+
+    support.focusin = "onfocusin" in window;
+
+
+    var rfocusMorph = /^(?:focusinfocus|focusoutblur)$/,
+        stopPropagationCallback = function(e) {
+            e.stopPropagation();
+        };
+
+    jQuery.extend(jQuery.event, {
+
+        trigger: function(event, data, elem, onlyHandlers) {
+
+            var i, cur, tmp, bubbleType, ontype, handle, special, lastElement,
+                eventPath = [elem || document],
+                type = hasOwn.call(event, "type") ? event.type : event,
+                namespaces = hasOwn.call(event, "namespace") ? event.namespace.split(".") : [];
+
+            cur = lastElement = tmp = elem = elem || document;
+
+            // Don't do events on text and comment nodes
+            if (elem.nodeType === 3 || elem.nodeType === 8) {
+                return;
+            }
+
+            // focus/blur morphs to focusin/out; ensure we're not firing them right now
+            if (rfocusMorph.test(type + jQuery.event.triggered)) {
+                return;
+            }
+
+            if (type.indexOf(".") > -1) {
+
+                // Namespaced trigger; create a regexp to match event type in handle()
+                namespaces = type.split(".");
+                type = namespaces.shift();
+                namespaces.sort();
+            }
+            ontype = type.indexOf(":") < 0 && "on" + type;
+
+            // Caller can pass in a jQuery.Event object, Object, or just an event type string
+            event = event[jQuery.expando] ?
+                event :
+                new jQuery.Event(type, typeof event === "object" && event);
+
+            // Trigger bitmask: & 1 for native handlers; & 2 for jQuery (always true)
+            event.isTrigger = onlyHandlers ? 2 : 3;
+            event.namespace = namespaces.join(".");
+            event.rnamespace = event.namespace ?
+                new RegExp("(^|\\.)" + namespaces.join("\\.(?:.*\\.|)") + "(\\.|$)") :
+                null;
+
+            // Clean up the event in case it is being reused
+            event.result = undefined;
+            if (!event.target) {
+                event.target = elem;
+            }
+
+            // Clone any incoming data and prepend the event, creating the handler arg list
+            data = data == null ? [event] :
+                jQuery.makeArray(data, [event]);
+
+            // Allow special events to draw outside the lines
+            special = jQuery.event.special[type] || {};
+            if (!onlyHandlers && special.trigger && special.trigger.apply(elem, data) === false) {
+                return;
+            }
+
+            // Determine event propagation path in advance, per W3C events spec (trac-9951)
+            // Bubble up to document, then to window; watch for a global ownerDocument var (trac-9724)
+            if (!onlyHandlers && !special.noBubble && !isWindow(elem)) {
+
+                bubbleType = special.delegateType || type;
+                if (!rfocusMorph.test(bubbleType + type)) {
+                    cur = cur.parentNode;
+                }
+                for (; cur; cur = cur.parentNode) {
+                    eventPath.push(cur);
+                    tmp = cur;
+                }
 
-        var requireNonComma,
-            depth = null,
-            str = jQuery.trim(data + "");
+                // Only add window if we got to document (e.g., not plain obj or detached DOM)
+                if (tmp === (elem.ownerDocument || document)) {
+                    eventPath.push(tmp.defaultView || tmp.parentWindow || window);
+                }
+            }
 
-        // Guard against invalid (and possibly dangerous) input by ensuring that nothing remains
-        // after removing valid tokens
-        return str && !jQuery.trim(str.replace(rvalidtokens, function(token, comma, open, close) {
+            // Fire handlers on the event path
+            i = 0;
+            while ((cur = eventPath[i++]) && !event.isPropagationStopped()) {
+                lastElement = cur;
+                event.type = i > 1 ?
+                    bubbleType :
+                    special.bindType || type;
 
-                // Force termination if we see a misplaced comma
-                if (requireNonComma && comma) {
-                    depth = 0;
+                // jQuery handler
+                handle = (dataPriv.get(cur, "events") || Object.create(null))[event.type] &&
+                    dataPriv.get(cur, "handle");
+                if (handle) {
+                    handle.apply(cur, data);
                 }
 
-                // Perform no more replacements after returning to outermost depth
-                if (depth === 0) {
-                    return token;
+                // Native handler
+                handle = ontype && cur[ontype];
+                if (handle && handle.apply && acceptData(cur)) {
+                    event.result = handle.apply(cur, data);
+                    if (event.result === false) {
+                        event.preventDefault();
+                    }
                 }
+            }
+            event.type = type;
+
+            // If nobody prevented the default action, do it now
+            if (!onlyHandlers && !event.isDefaultPrevented()) {
+
+                if ((!special._default ||
+                        special._default.apply(eventPath.pop(), data) === false) &&
+                    acceptData(elem)) {
+
+                    // Call a native DOM method on the target with the same name as the event.
+                    // Don't do default actions on window, that's where global variables be (trac-6170)
+                    if (ontype && isFunction(elem[type]) && !isWindow(elem)) {
+
+                        // Don't re-trigger an onFOO event when we call its FOO() method
+                        tmp = elem[ontype];
+
+                        if (tmp) {
+                            elem[ontype] = null;
+                        }
+
+                        // Prevent re-triggering of the same event, since we already bubbled it above
+                        jQuery.event.triggered = type;
+
+                        if (event.isPropagationStopped()) {
+                            lastElement.addEventListener(type, stopPropagationCallback);
+                        }
 
-                // Commas must not follow "[", "{", or ","
-                requireNonComma = open || comma;
+                        elem[type]();
 
-                // Determine new depth
-                // array/object open ("[" or "{"): depth += true - false (increment)
-                // array/object close ("]" or "}"): depth += false - true (decrement)
-                // other cases ("," or primitive): depth += true - true (numeric cast)
-                depth += !close - !open;
+                        if (event.isPropagationStopped()) {
+                            lastElement.removeEventListener(type, stopPropagationCallback);
+                        }
 
-                // Remove this token
-                return "";
-            })) ?
-            (Function("return " + str))() :
-            jQuery.error("Invalid JSON: " + data);
+                        jQuery.event.triggered = undefined;
+
+                        if (tmp) {
+                            elem[ontype] = tmp;
+                        }
+                    }
+                }
+            }
+
+            return event.result;
+        },
+
+        // Piggyback on a donor event to simulate a different one
+        // Used only for `focus(in | out)` events
+        simulate: function(type, elem, event) {
+            var e = jQuery.extend(
+                new jQuery.Event(),
+                event, {
+                    type: type,
+                    isSimulated: true
+                }
+            );
+
+            jQuery.event.trigger(e, null, elem);
+        }
+
+    });
+
+    jQuery.fn.extend({
+
+        trigger: function(type, data) {
+            return this.each(function() {
+                jQuery.event.trigger(type, data, this);
+            });
+        },
+        triggerHandler: function(type, data) {
+            var elem = this[0];
+            if (elem) {
+                return jQuery.event.trigger(type, data, elem, true);
+            }
+        }
+    });
+
+
+    // Support: Firefox <=44
+    // Firefox doesn't have focus(in | out) events
+    // Related ticket - https://bugzilla.mozilla.org/show_bug.cgi?id=687787
+    //
+    // Support: Chrome <=48 - 49, Safari <=9.0 - 9.1
+    // focus(in | out) events fire after focus & blur events,
+    // which is spec violation - http://www.w3.org/TR/DOM-Level-3-Events/#events-focusevent-event-order
+    // Related ticket - https://bugs.chromium.org/p/chromium/issues/detail?id=449857
+    if (!support.focusin) {
+        jQuery.each({
+            focus: "focusin",
+            blur: "focusout"
+        }, function(orig, fix) {
+
+            // Attach a single capturing handler on the document while someone wants focusin/focusout
+            var handler = function(event) {
+                jQuery.event.simulate(fix, event.target, jQuery.event.fix(event));
+            };
+
+            jQuery.event.special[fix] = {
+                setup: function() {
+
+                    // Handle: regular nodes (via `this.ownerDocument`), window
+                    // (via `this.document`) & document (via `this`).
+                    var doc = this.ownerDocument || this.document || this,
+                        attaches = dataPriv.access(doc, fix);
+
+                    if (!attaches) {
+                        doc.addEventListener(orig, handler, true);
+                    }
+                    dataPriv.access(doc, fix, (attaches || 0) + 1);
+                },
+                teardown: function() {
+                    var doc = this.ownerDocument || this.document || this,
+                        attaches = dataPriv.access(doc, fix) - 1;
+
+                    if (!attaches) {
+                        doc.removeEventListener(orig, handler, true);
+                        dataPriv.remove(doc, fix);
+
+                    } else {
+                        dataPriv.access(doc, fix, attaches);
+                    }
+                }
+            };
+        });
+    }
+    var location = window.location;
+
+    var nonce = {
+        guid: Date.now()
     };
 
+    var rquery = (/\?/);
+
+
 
     // Cross-browser xml parsing
     jQuery.parseXML = function(data) {
-        var xml, tmp;
+        var xml, parserErrorElem;
         if (!data || typeof data !== "string") {
             return null;
         }
+
+        // Support: IE 9 - 11 only
+        // IE throws on parseFromString with invalid input.
         try {
-            if (window.DOMParser) { // Standard
-                tmp = new DOMParser();
-                xml = tmp.parseFromString(data, "text/xml");
-            } else { // IE
-                xml = new ActiveXObject("Microsoft.XMLDOM");
-                xml.async = "false";
-                xml.loadXML(data);
-            }
-        } catch (e) {
-            xml = undefined;
-        }
-        if (!xml || !xml.documentElement || xml.getElementsByTagName("parsererror").length) {
-            jQuery.error("Invalid XML: " + data);
+            xml = (new window.DOMParser()).parseFromString(data, "text/xml");
+        } catch (e) {}
+
+        parserErrorElem = xml && xml.getElementsByTagName("parsererror")[0];
+        if (!xml || parserErrorElem) {
+            jQuery.error("Invalid XML: " + (
+                parserErrorElem ?
+                jQuery.map(parserErrorElem.childNodes, function(el) {
+                    return el.textContent;
+                }).join("\n") :
+                data
+            ));
         }
         return xml;
     };
 
 
     var
-        // Document location
-        ajaxLocParts,
-        ajaxLocation,
+        rbracket = /\[\]$/,
+        rCRLF = /\r?\n/g,
+        rsubmitterTypes = /^(?:submit|button|image|reset|file)$/i,
+        rsubmittable = /^(?:input|select|textarea|keygen)/i;
+
+    function buildParams(prefix, obj, traditional, add) {
+        var name;
+
+        if (Array.isArray(obj)) {
+
+            // Serialize array item.
+            jQuery.each(obj, function(i, v) {
+                if (traditional || rbracket.test(prefix)) {
+
+                    // Treat each array item as a scalar.
+                    add(prefix, v);
+
+                } else {
+
+                    // Item is non-scalar (array or object), encode its numeric index.
+                    buildParams(
+                        prefix + "[" + (typeof v === "object" && v != null ? i : "") + "]",
+                        v,
+                        traditional,
+                        add
+                    );
+                }
+            });
+
+        } else if (!traditional && toType(obj) === "object") {
+
+            // Serialize object item.
+            for (name in obj) {
+                buildParams(prefix + "[" + name + "]", obj[name], traditional, add);
+            }
+
+        } else {
+
+            // Serialize scalar item.
+            add(prefix, obj);
+        }
+    }
+
+    // Serialize an array of form elements or a set of
+    // key/values into a query string
+    jQuery.param = function(a, traditional) {
+        var prefix,
+            s = [],
+            add = function(key, valueOrFunction) {
+
+                // If value is a function, invoke it and use its return value
+                var value = isFunction(valueOrFunction) ?
+                    valueOrFunction() :
+                    valueOrFunction;
+
+                s[s.length] = encodeURIComponent(key) + "=" +
+                    encodeURIComponent(value == null ? "" : value);
+            };
+
+        if (a == null) {
+            return "";
+        }
+
+        // If an array was passed in, assume that it is an array of form elements.
+        if (Array.isArray(a) || (a.jquery && !jQuery.isPlainObject(a))) {
+
+            // Serialize the form elements
+            jQuery.each(a, function() {
+                add(this.name, this.value);
+            });
+
+        } else {
+
+            // If traditional, encode the "old" way (the way 1.3.2 or older
+            // did it), otherwise encode params recursively.
+            for (prefix in a) {
+                buildParams(prefix, a[prefix], traditional, add);
+            }
+        }
+
+        // Return the resulting serialization
+        return s.join("&");
+    };
 
+    jQuery.fn.extend({
+        serialize: function() {
+            return jQuery.param(this.serializeArray());
+        },
+        serializeArray: function() {
+            return this.map(function() {
+
+                // Can add propHook for "elements" to filter or add form elements
+                var elements = jQuery.prop(this, "elements");
+                return elements ? jQuery.makeArray(elements) : this;
+            }).filter(function() {
+                var type = this.type;
+
+                // Use .is( ":disabled" ) so that fieldset[disabled] works
+                return this.name && !jQuery(this).is(":disabled") &&
+                    rsubmittable.test(this.nodeName) && !rsubmitterTypes.test(type) &&
+                    (this.checked || !rcheckableType.test(type));
+            }).map(function(_i, elem) {
+                var val = jQuery(this).val();
+
+                if (val == null) {
+                    return null;
+                }
+
+                if (Array.isArray(val)) {
+                    return jQuery.map(val, function(val) {
+                        return {
+                            name: elem.name,
+                            value: val.replace(rCRLF, "\r\n")
+                        };
+                    });
+                }
+
+                return {
+                    name: elem.name,
+                    value: val.replace(rCRLF, "\r\n")
+                };
+            }).get();
+        }
+    });
+
+
+    var
+        r20 = /%20/g,
         rhash = /#.*$/,
-        rts = /([?&])_=[^&]*/,
-        rheaders = /^(.*?):[ \t]*([^\r\n]*)\r?$/mg, // IE leaves an \r character at EOL
-        // #7653, #8125, #8152: local protocol detection
+        rantiCache = /([?&])_=[^&]*/,
+        rheaders = /^(.*?):[ \t]*([^\r\n]*)$/mg,
+
+        // trac-7653, trac-8125, trac-8152: local protocol detection
         rlocalProtocol = /^(?:about|app|app-storage|.+-extension|file|res|widget):$/,
         rnoContent = /^(?:GET|HEAD)$/,
         rprotocol = /^\/\//,
-        rurl = /^([\w.+-]+:)(?:\/\/(?:[^\/?#]*@|)([^\/?#:]*)(?::(\d+)|)|)/,
 
         /* Prefilters
          * 1) They are useful to introduce custom dataTypes (see ajax/jsonp.js for an example)
          * 2) These are called:
          *    - BEFORE asking for a transport
          *    - AFTER param serialization (s.data is a string if s.processData is true)
          * 3) key is the dataType
@@ -8631,52 +9126,44 @@
         /* Transports bindings
          * 1) key is the dataType
          * 2) the catchall symbol "*" can be used
          * 3) selection will start with transport dataType and THEN go to "*" if needed
          */
         transports = {},
 
-        // Avoid comment-prolog char sequence (#10098); must appease lint and evade compression
-        allTypes = "*/".concat("*");
+        // Avoid comment-prolog char sequence (trac-10098); must appease lint and evade compression
+        allTypes = "*/".concat("*"),
 
-    // #8138, IE may throw an exception when accessing
-    // a field from window.location if document.domain has been set
-    try {
-        ajaxLocation = location.href;
-    } catch (e) {
-        // Use the href attribute of an A element
-        // since IE will modify it given document.location
-        ajaxLocation = document.createElement("a");
-        ajaxLocation.href = "";
-        ajaxLocation = ajaxLocation.href;
-    }
+        // Anchor tag for parsing the document origin
+        originAnchor = document.createElement("a");
 
-    // Segment location into parts
-    ajaxLocParts = rurl.exec(ajaxLocation.toLowerCase()) || [];
+    originAnchor.href = location.href;
 
     // Base "constructor" for jQuery.ajaxPrefilter and jQuery.ajaxTransport
     function addToPrefiltersOrTransports(structure) {
 
         // dataTypeExpression is optional and defaults to "*"
         return function(dataTypeExpression, func) {
 
             if (typeof dataTypeExpression !== "string") {
                 func = dataTypeExpression;
                 dataTypeExpression = "*";
             }
 
             var dataType,
                 i = 0,
-                dataTypes = dataTypeExpression.toLowerCase().match(rnotwhite) || [];
+                dataTypes = dataTypeExpression.toLowerCase().match(rnothtmlwhite) || [];
+
+            if (isFunction(func)) {
 
-            if (jQuery.isFunction(func)) {
                 // For each dataType in the dataTypeExpression
                 while ((dataType = dataTypes[i++])) {
+
                     // Prepend if requested
-                    if (dataType.charAt(0) === "+") {
+                    if (dataType[0] === "+") {
                         dataType = dataType.slice(1) || "*";
                         (structure[dataType] = structure[dataType] || []).unshift(func);
 
                         // Otherwise append
                     } else {
                         (structure[dataType] = structure[dataType] || []).push(func);
                     }
@@ -8692,15 +9179,17 @@
             seekingTransport = (structure === transports);
 
         function inspect(dataType) {
             var selected;
             inspected[dataType] = true;
             jQuery.each(structure[dataType] || [], function(_, prefilterOrFactory) {
                 var dataTypeOrTransport = prefilterOrFactory(options, originalOptions, jqXHR);
-                if (typeof dataTypeOrTransport === "string" && !seekingTransport && !inspected[dataTypeOrTransport]) {
+                if (typeof dataTypeOrTransport === "string" &&
+                    !seekingTransport && !inspected[dataTypeOrTransport]) {
+
                     options.dataTypes.unshift(dataTypeOrTransport);
                     inspect(dataTypeOrTransport);
                     return false;
                 } else if (seekingTransport) {
                     return !(selected = dataTypeOrTransport);
                 }
             });
@@ -8708,17 +9197,17 @@
         }
 
         return inspect(options.dataTypes[0]) || !inspected["*"] && inspect("*");
     }
 
     // A special extend for ajax options
     // that takes "flat" options (not to be deep extended)
-    // Fixes #9887
+    // Fixes trac-9887
     function ajaxExtend(target, src) {
-        var deep, key,
+        var key, deep,
             flatOptions = jQuery.ajaxSettings.flatOptions || {};
 
         for (key in src) {
             if (src[key] !== undefined) {
                 (flatOptions[key] ? target : (deep || (deep = {})))[key] = src[key];
             }
         }
@@ -8730,15 +9219,16 @@
     }
 
     /* Handles responses to an ajax request:
      * - finds the right dataType (mediates between content-type and expected dataType)
      * - returns the corresponding response
      */
     function ajaxHandleResponses(s, jqXHR, responses) {
-        var firstDataType, ct, finalDataType, type,
+
+        var ct, type, finalDataType, firstDataType,
             contents = s.contents,
             dataTypes = s.dataTypes;
 
         // Remove auto dataType and get content-type in the process
         while (dataTypes[0] === "*") {
             dataTypes.shift();
             if (ct === undefined) {
@@ -8756,24 +9246,26 @@
             }
         }
 
         // Check to see if we have a response for the expected dataType
         if (dataTypes[0] in responses) {
             finalDataType = dataTypes[0];
         } else {
+
             // Try convertible dataTypes
             for (type in responses) {
                 if (!dataTypes[0] || s.converters[type + " " + dataTypes[0]]) {
                     finalDataType = type;
                     break;
                 }
                 if (!firstDataType) {
                     firstDataType = type;
                 }
             }
+
             // Or just use first one
             finalDataType = finalDataType || firstDataType;
         }
 
         // If we found a dataType
         // We add the dataType to the list if needed
         // and return the corresponding response
@@ -8787,14 +9279,15 @@
 
     /* Chain conversions given the request and the original response
      * Also sets the responseXXX fields on the jqXHR instance
      */
     function ajaxConvert(s, response, jqXHR, isSuccess) {
         var conv2, current, conv, tmp, prev,
             converters = {},
+
             // Work with a copy of dataTypes in case we need to modify it for conversion
             dataTypes = s.dataTypes.slice();
 
         // Create converters map with lowercased keys
         if (dataTypes[1]) {
             for (conv in s.converters) {
                 converters[conv.toLowerCase()] = s.converters[conv];
@@ -8839,14 +9332,15 @@
                             tmp = conv2.split(" ");
                             if (tmp[1] === current) {
 
                                 // If prev can be converted to accepted input
                                 conv = converters[prev + " " + tmp[0]] ||
                                     converters["* " + tmp[0]];
                                 if (conv) {
+
                                     // Condense equivalence converters
                                     if (conv === true) {
                                         conv = converters[conv2];
 
                                         // Otherwise, insert the intermediate dataType
                                     } else if (converters[conv2] !== true) {
                                         current = tmp[0];
@@ -8858,15 +9352,15 @@
                         }
                     }
 
                     // Apply converter (if not an equivalence)
                     if (conv !== true) {
 
                         // Unless errors are allowed to bubble, catch and return them
-                        if (conv && s["throws"]) {
+                        if (conv && s.throws) {
                             response = conv(response);
                         } else {
                             try {
                                 response = conv(response);
                             } catch (e) {
                                 return {
                                     state: "parsererror",
@@ -8891,21 +9385,22 @@
         active: 0,
 
         // Last-Modified header cache for next request
         lastModified: {},
         etag: {},
 
         ajaxSettings: {
-            url: ajaxLocation,
+            url: location.href,
             type: "GET",
-            isLocal: rlocalProtocol.test(ajaxLocParts[1]),
+            isLocal: rlocalProtocol.test(location.protocol),
             global: true,
             processData: true,
             async: true,
             contentType: "application/x-www-form-urlencoded; charset=UTF-8",
+
             /*
             timeout: 0,
             data: null,
             dataType: null,
             username: null,
             password: null,
             cache: null,
@@ -8919,17 +9414,17 @@
                 text: "text/plain",
                 html: "text/html",
                 xml: "application/xml, text/xml",
                 json: "application/json, text/javascript"
             },
 
             contents: {
-                xml: /xml/,
-                html: /html/,
-                json: /json/
+                xml: /\bxml\b/,
+                html: /\bhtml/,
+                json: /\bjson\b/
             },
 
             responseFields: {
                 xml: "responseXML",
                 text: "responseText",
                 json: "responseJSON"
             },
@@ -8941,15 +9436,15 @@
                 // Convert anything to text
                 "* text": String,
 
                 // Text to html (true = no transformation)
                 "text html": true,
 
                 // Evaluate text as a json expression
-                "text json": jQuery.parseJSON,
+                "text json": JSON.parse,
 
                 // Parse text as xml
                 "text xml": jQuery.parseXML
             },
 
             // For options that shouldn't be deep extended:
             // you can add your own custom options here if
@@ -8985,105 +9480,125 @@
                 options = url;
                 url = undefined;
             }
 
             // Force options to be an object
             options = options || {};
 
-            var // Cross-domain detection vars
-                parts,
-                // Loop variable
-                i,
+            var transport,
+
                 // URL without anti-cache param
                 cacheURL,
-                // Response headers as string
+
+                // Response headers
                 responseHeadersString,
+                responseHeaders,
+
                 // timeout handle
                 timeoutTimer,
 
+                // Url cleanup var
+                urlAnchor,
+
+                // Request state (becomes false upon send and true upon completion)
+                completed,
+
                 // To know if global events are to be dispatched
                 fireGlobals,
 
-                transport,
-                // Response headers
-                responseHeaders,
+                // Loop variable
+                i,
+
+                // uncached part of the url
+                uncached,
+
                 // Create the final options object
                 s = jQuery.ajaxSetup({}, options),
+
                 // Callbacks context
                 callbackContext = s.context || s,
+
                 // Context for global events is callbackContext if it is a DOM node or jQuery collection
-                globalEventContext = s.context && (callbackContext.nodeType || callbackContext.jquery) ?
+                globalEventContext = s.context &&
+                (callbackContext.nodeType || callbackContext.jquery) ?
                 jQuery(callbackContext) :
                 jQuery.event,
+
                 // Deferreds
                 deferred = jQuery.Deferred(),
                 completeDeferred = jQuery.Callbacks("once memory"),
+
                 // Status-dependent callbacks
                 statusCode = s.statusCode || {},
+
                 // Headers (they are sent all at once)
                 requestHeaders = {},
                 requestHeadersNames = {},
-                // The jqXHR state
-                state = 0,
+
                 // Default abort message
                 strAbort = "canceled",
+
                 // Fake xhr
                 jqXHR = {
                     readyState: 0,
 
                     // Builds headers hashtable if needed
                     getResponseHeader: function(key) {
                         var match;
-                        if (state === 2) {
+                        if (completed) {
                             if (!responseHeaders) {
                                 responseHeaders = {};
                                 while ((match = rheaders.exec(responseHeadersString))) {
-                                    responseHeaders[match[1].toLowerCase()] = match[2];
+                                    responseHeaders[match[1].toLowerCase() + " "] =
+                                        (responseHeaders[match[1].toLowerCase() + " "] || [])
+                                        .concat(match[2]);
                                 }
                             }
-                            match = responseHeaders[key.toLowerCase()];
+                            match = responseHeaders[key.toLowerCase() + " "];
                         }
-                        return match == null ? null : match;
+                        return match == null ? null : match.join(", ");
                     },
 
                     // Raw string
                     getAllResponseHeaders: function() {
-                        return state === 2 ? responseHeadersString : null;
+                        return completed ? responseHeadersString : null;
                     },
 
                     // Caches the header
                     setRequestHeader: function(name, value) {
-                        var lname = name.toLowerCase();
-                        if (!state) {
-                            name = requestHeadersNames[lname] = requestHeadersNames[lname] || name;
+                        if (completed == null) {
+                            name = requestHeadersNames[name.toLowerCase()] =
+                                requestHeadersNames[name.toLowerCase()] || name;
                             requestHeaders[name] = value;
                         }
                         return this;
                     },
 
                     // Overrides response content-type header
                     overrideMimeType: function(type) {
-                        if (!state) {
+                        if (completed == null) {
                             s.mimeType = type;
                         }
                         return this;
                     },
 
                     // Status-dependent callbacks
                     statusCode: function(map) {
                         var code;
                         if (map) {
-                            if (state < 2) {
+                            if (completed) {
+
+                                // Execute the appropriate callbacks
+                                jqXHR.always(map[jqXHR.status]);
+                            } else {
+
+                                // Lazy-add the new callbacks in a way that preserves old ones
                                 for (code in map) {
-                                    // Lazy-add the new callback in a way that preserves old ones
                                     statusCode[code] = [statusCode[code], map[code]];
                                 }
-                            } else {
-                                // Execute the appropriate callbacks
-                                jqXHR.always(map[jqXHR.status]);
                             }
                         }
                         return this;
                     },
 
                     // Cancel the request
                     abort: function(statusText) {
@@ -9093,91 +9608,112 @@
                         }
                         done(0, finalText);
                         return this;
                     }
                 };
 
             // Attach deferreds
-            deferred.promise(jqXHR).complete = completeDeferred.add;
-            jqXHR.success = jqXHR.done;
-            jqXHR.error = jqXHR.fail;
-
-            // Remove hash character (#7531: and string promotion)
-            // Add protocol if not provided (#5866: IE7 issue with protocol-less urls)
-            // Handle falsy url in the settings object (#10093: consistency with old signature)
+            deferred.promise(jqXHR);
+
+            // Add protocol if not provided (prefilters might expect it)
+            // Handle falsy url in the settings object (trac-10093: consistency with old signature)
             // We also use the url parameter if available
-            s.url = ((url || s.url || ajaxLocation) + "").replace(rhash, "").replace(rprotocol, ajaxLocParts[1] + "//");
+            s.url = ((url || s.url || location.href) + "")
+                .replace(rprotocol, location.protocol + "//");
 
-            // Alias method option to type as per ticket #12004
+            // Alias method option to type as per ticket trac-12004
             s.type = options.method || options.type || s.method || s.type;
 
             // Extract dataTypes list
-            s.dataTypes = jQuery.trim(s.dataType || "*").toLowerCase().match(rnotwhite) || [""];
+            s.dataTypes = (s.dataType || "*").toLowerCase().match(rnothtmlwhite) || [""];
 
-            // A cross-domain request is in order when we have a protocol:host:port mismatch
+            // A cross-domain request is in order when the origin doesn't match the current origin.
             if (s.crossDomain == null) {
-                parts = rurl.exec(s.url.toLowerCase());
-                s.crossDomain = !!(parts &&
-                    (parts[1] !== ajaxLocParts[1] || parts[2] !== ajaxLocParts[2] ||
-                        (parts[3] || (parts[1] === "http:" ? "80" : "443")) !==
-                        (ajaxLocParts[3] || (ajaxLocParts[1] === "http:" ? "80" : "443")))
-                );
+                urlAnchor = document.createElement("a");
+
+                // Support: IE <=8 - 11, Edge 12 - 15
+                // IE throws exception on accessing the href property if url is malformed,
+                // e.g. http://example.com:80x/
+                try {
+                    urlAnchor.href = s.url;
+
+                    // Support: IE <=8 - 11 only
+                    // Anchor's host property isn't correctly set when s.url is relative
+                    urlAnchor.href = urlAnchor.href;
+                    s.crossDomain = originAnchor.protocol + "//" + originAnchor.host !==
+                        urlAnchor.protocol + "//" + urlAnchor.host;
+                } catch (e) {
+
+                    // If there is an error parsing the URL, assume it is crossDomain,
+                    // it can be rejected by the transport if it is invalid
+                    s.crossDomain = true;
+                }
             }
 
             // Convert data if not already a string
             if (s.data && s.processData && typeof s.data !== "string") {
                 s.data = jQuery.param(s.data, s.traditional);
             }
 
             // Apply prefilters
             inspectPrefiltersOrTransports(prefilters, s, options, jqXHR);
 
             // If request was aborted inside a prefilter, stop there
-            if (state === 2) {
+            if (completed) {
                 return jqXHR;
             }
 
             // We can fire global events as of now if asked to
-            fireGlobals = s.global;
+            // Don't fire events if jQuery.event is undefined in an AMD-usage scenario (trac-15118)
+            fireGlobals = jQuery.event && s.global;
 
             // Watch for a new set of requests
             if (fireGlobals && jQuery.active++ === 0) {
                 jQuery.event.trigger("ajaxStart");
             }
 
             // Uppercase the type
             s.type = s.type.toUpperCase();
 
             // Determine if request has content
             s.hasContent = !rnoContent.test(s.type);
 
             // Save the URL in case we're toying with the If-Modified-Since
             // and/or If-None-Match header later on
-            cacheURL = s.url;
+            // Remove hash to simplify url manipulation
+            cacheURL = s.url.replace(rhash, "");
 
             // More options handling for requests with no content
             if (!s.hasContent) {
 
-                // If data is available, append data to url
-                if (s.data) {
-                    cacheURL = (s.url += (rquery.test(cacheURL) ? "&" : "?") + s.data);
-                    // #9682: remove data so that it's not used in an eventual retry
+                // Remember the hash so we can put it back
+                uncached = s.url.slice(cacheURL.length);
+
+                // If data is available and should be processed, append data to url
+                if (s.data && (s.processData || typeof s.data === "string")) {
+                    cacheURL += (rquery.test(cacheURL) ? "&" : "?") + s.data;
+
+                    // trac-9682: remove data so that it's not used in an eventual retry
                     delete s.data;
                 }
 
-                // Add anti-cache in url if needed
+                // Add or update anti-cache param if needed
                 if (s.cache === false) {
-                    s.url = rts.test(cacheURL) ?
-
-                        // If there is already a '_' parameter, set its value
-                        cacheURL.replace(rts, "$1_=" + nonce++) :
-
-                        // Otherwise add one to the end
-                        cacheURL + (rquery.test(cacheURL) ? "&" : "?") + "_=" + nonce++;
+                    cacheURL = cacheURL.replace(rantiCache, "$1");
+                    uncached = (rquery.test(cacheURL) ? "&" : "?") + "_=" + (nonce.guid++) +
+                        uncached;
                 }
+
+                // Put hash and anti-cache on the URL that will be requested (gh-1732)
+                s.url = cacheURL + uncached;
+
+                // Change '%20' to '+' if this is encoded form body content (gh-2658)
+            } else if (s.data && s.processData &&
+                (s.contentType || "").indexOf("application/x-www-form-urlencoded") === 0) {
+                s.data = s.data.replace(r20, "+");
             }
 
             // Set the If-Modified-Since and/or If-None-Match header, if in ifModified mode.
             if (s.ifModified) {
                 if (jQuery.lastModified[cacheURL]) {
                     jqXHR.setRequestHeader("If-Modified-Since", jQuery.lastModified[cacheURL]);
                 }
@@ -9191,91 +9727,96 @@
                 jqXHR.setRequestHeader("Content-Type", s.contentType);
             }
 
             // Set the Accepts header for the server, depending on the dataType
             jqXHR.setRequestHeader(
                 "Accept",
                 s.dataTypes[0] && s.accepts[s.dataTypes[0]] ?
-                s.accepts[s.dataTypes[0]] + (s.dataTypes[0] !== "*" ? ", " + allTypes + "; q=0.01" : "") :
+                s.accepts[s.dataTypes[0]] +
+                (s.dataTypes[0] !== "*" ? ", " + allTypes + "; q=0.01" : "") :
                 s.accepts["*"]
             );
 
             // Check for headers option
             for (i in s.headers) {
                 jqXHR.setRequestHeader(i, s.headers[i]);
             }
 
             // Allow custom headers/mimetypes and early abort
-            if (s.beforeSend && (s.beforeSend.call(callbackContext, jqXHR, s) === false || state === 2)) {
+            if (s.beforeSend &&
+                (s.beforeSend.call(callbackContext, jqXHR, s) === false || completed)) {
+
                 // Abort if not done already and return
                 return jqXHR.abort();
             }
 
-            // aborting is no longer a cancellation
+            // Aborting is no longer a cancellation
             strAbort = "abort";
 
             // Install callbacks on deferreds
-            for (i in {
-                    success: 1,
-                    error: 1,
-                    complete: 1
-                }) {
-                jqXHR[i](s[i]);
-            }
+            completeDeferred.add(s.complete);
+            jqXHR.done(s.success);
+            jqXHR.fail(s.error);
 
             // Get transport
             transport = inspectPrefiltersOrTransports(transports, s, options, jqXHR);
 
             // If no transport, we auto-abort
             if (!transport) {
                 done(-1, "No Transport");
             } else {
                 jqXHR.readyState = 1;
 
                 // Send global event
                 if (fireGlobals) {
                     globalEventContext.trigger("ajaxSend", [jqXHR, s]);
                 }
+
+                // If request was aborted inside ajaxSend, stop there
+                if (completed) {
+                    return jqXHR;
+                }
+
                 // Timeout
                 if (s.async && s.timeout > 0) {
-                    timeoutTimer = setTimeout(function() {
+                    timeoutTimer = window.setTimeout(function() {
                         jqXHR.abort("timeout");
                     }, s.timeout);
                 }
 
                 try {
-                    state = 1;
+                    completed = false;
                     transport.send(requestHeaders, done);
                 } catch (e) {
-                    // Propagate exception as error if not done
-                    if (state < 2) {
-                        done(-1, e);
-                        // Simply rethrow otherwise
-                    } else {
+
+                    // Rethrow post-completion exceptions
+                    if (completed) {
                         throw e;
                     }
+
+                    // Propagate others as results
+                    done(-1, e);
                 }
             }
 
             // Callback for when everything is done
             function done(status, nativeStatusText, responses, headers) {
                 var isSuccess, success, error, response, modified,
                     statusText = nativeStatusText;
 
-                // Called once
-                if (state === 2) {
+                // Ignore repeat invocations
+                if (completed) {
                     return;
                 }
 
-                // State is "done" now
-                state = 2;
+                completed = true;
 
                 // Clear timeout if it exists
                 if (timeoutTimer) {
-                    clearTimeout(timeoutTimer);
+                    window.clearTimeout(timeoutTimer);
                 }
 
                 // Dereference transport for early garbage collection
                 // (no matter how long the jqXHR object will be used)
                 transport = undefined;
 
                 // Cache response headers
@@ -9288,14 +9829,21 @@
                 isSuccess = status >= 200 && status < 300 || status === 304;
 
                 // Get response data
                 if (responses) {
                     response = ajaxHandleResponses(s, jqXHR, responses);
                 }
 
+                // Use a noop converter for missing script but not if jsonp
+                if (!isSuccess &&
+                    jQuery.inArray("script", s.dataTypes) > -1 &&
+                    jQuery.inArray("json", s.dataTypes) < 0) {
+                    s.converters["text script"] = function() {};
+                }
+
                 // Convert no matter what (that way responseXXX fields are always set)
                 response = ajaxConvert(s, response, jqXHR, isSuccess);
 
                 // If successful, handle type chaining
                 if (isSuccess) {
 
                     // Set the If-Modified-Since and/or If-None-Match header, if in ifModified mode.
@@ -9322,16 +9870,16 @@
                     } else {
                         statusText = response.state;
                         success = response.data;
                         error = response.error;
                         isSuccess = !error;
                     }
                 } else {
-                    // We extract error from statusText
-                    // then normalize statusText and status for non-aborts
+
+                    // Extract error from statusText and normalize for non-aborts
                     error = statusText;
                     if (status || !statusText) {
                         statusText = "error";
                         if (status < 0) {
                             status = 0;
                         }
                     }
@@ -9358,14 +9906,15 @@
                 }
 
                 // Complete
                 completeDeferred.fireWith(callbackContext, [jqXHR, statusText]);
 
                 if (fireGlobals) {
                     globalEventContext.trigger("ajaxComplete", [jqXHR, s]);
+
                     // Handle the global AJAX counter
                     if (!(--jQuery.active)) {
                         jQuery.event.trigger("ajaxStop");
                     }
                 }
             }
 
@@ -9377,85 +9926,101 @@
         },
 
         getScript: function(url, callback) {
             return jQuery.get(url, undefined, callback, "script");
         }
     });
 
-    jQuery.each(["get", "post"], function(i, method) {
+    jQuery.each(["get", "post"], function(_i, method) {
         jQuery[method] = function(url, data, callback, type) {
-            // shift arguments if data argument was omitted
-            if (jQuery.isFunction(data)) {
+
+            // Shift arguments if data argument was omitted
+            if (isFunction(data)) {
                 type = type || callback;
                 callback = data;
                 data = undefined;
             }
 
-            return jQuery.ajax({
+            // The url can be an options object (which then must have .url)
+            return jQuery.ajax(jQuery.extend({
                 url: url,
                 type: method,
                 dataType: type,
                 data: data,
                 success: callback
-            });
+            }, jQuery.isPlainObject(url) && url));
         };
     });
 
-    // Attach a bunch of functions for handling common AJAX events
-    jQuery.each(["ajaxStart", "ajaxStop", "ajaxComplete", "ajaxError", "ajaxSuccess", "ajaxSend"], function(i, type) {
-        jQuery.fn[type] = function(fn) {
-            return this.on(type, fn);
-        };
+    jQuery.ajaxPrefilter(function(s) {
+        var i;
+        for (i in s.headers) {
+            if (i.toLowerCase() === "content-type") {
+                s.contentType = s.headers[i] || "";
+            }
+        }
     });
 
 
-    jQuery._evalUrl = function(url) {
+    jQuery._evalUrl = function(url, options, doc) {
         return jQuery.ajax({
             url: url,
+
+            // Make this explicit, since user can override this through ajaxSetup (trac-11264)
             type: "GET",
             dataType: "script",
+            cache: true,
             async: false,
             global: false,
-            "throws": true
+
+            // Only evaluate the response if it is successful (gh-4126)
+            // dataFilter is not invoked for failure responses, so using it instead
+            // of the default converter is kludgy but it works.
+            converters: {
+                "text script": function() {}
+            },
+            dataFilter: function(response) {
+                jQuery.globalEval(response, options, doc);
+            }
         });
     };
 
 
     jQuery.fn.extend({
         wrapAll: function(html) {
-            if (jQuery.isFunction(html)) {
-                return this.each(function(i) {
-                    jQuery(this).wrapAll(html.call(this, i));
-                });
-            }
+            var wrap;
 
             if (this[0]) {
+                if (isFunction(html)) {
+                    html = html.call(this[0]);
+                }
+
                 // The elements to wrap the target around
-                var wrap = jQuery(html, this[0].ownerDocument).eq(0).clone(true);
+                wrap = jQuery(html, this[0].ownerDocument).eq(0).clone(true);
 
                 if (this[0].parentNode) {
                     wrap.insertBefore(this[0]);
                 }
 
                 wrap.map(function() {
                     var elem = this;
 
-                    while (elem.firstChild && elem.firstChild.nodeType === 1) {
-                        elem = elem.firstChild;
+                    while (elem.firstElementChild) {
+                        elem = elem.firstElementChild;
                     }
 
                     return elem;
                 }).append(this);
             }
 
             return this;
         },
 
         wrapInner: function(html) {
-            if (jQuery.isFunction(html)) {
+            if (isFunction(html)) {
                 return this.each(function(i) {
                     jQuery(this).wrapInner(html.call(this, i));
                 });
             }
 
             return this.each(function() {
                 var self = jQuery(this),
@@ -9467,425 +10032,268 @@
                 } else {
                     self.append(html);
                 }
             });
         },
 
         wrap: function(html) {
-            var isFunction = jQuery.isFunction(html);
+            var htmlIsFunction = isFunction(html);
 
             return this.each(function(i) {
-                jQuery(this).wrapAll(isFunction ? html.call(this, i) : html);
+                jQuery(this).wrapAll(htmlIsFunction ? html.call(this, i) : html);
             });
         },
 
-        unwrap: function() {
-            return this.parent().each(function() {
-                if (!jQuery.nodeName(this, "body")) {
-                    jQuery(this).replaceWith(this.childNodes);
-                }
-            }).end();
+        unwrap: function(selector) {
+            this.parent(selector).not("body").each(function() {
+                jQuery(this).replaceWith(this.childNodes);
+            });
+            return this;
         }
     });
 
 
-    jQuery.expr.filters.hidden = function(elem) {
-        // Support: Opera <= 12.12
-        // Opera reports offsetWidths and offsetHeights less than zero on some elements
-        return elem.offsetWidth <= 0 && elem.offsetHeight <= 0 ||
-            (!support.reliableHiddenOffsets() &&
-                ((elem.style && elem.style.display) || jQuery.css(elem, "display")) === "none");
+    jQuery.expr.pseudos.hidden = function(elem) {
+        return !jQuery.expr.pseudos.visible(elem);
     };
-
-    jQuery.expr.filters.visible = function(elem) {
-        return !jQuery.expr.filters.hidden(elem);
+    jQuery.expr.pseudos.visible = function(elem) {
+        return !!(elem.offsetWidth || elem.offsetHeight || elem.getClientRects().length);
     };
 
 
 
 
-    var r20 = /%20/g,
-        rbracket = /\[\]$/,
-        rCRLF = /\r?\n/g,
-        rsubmitterTypes = /^(?:submit|button|image|reset|file)$/i,
-        rsubmittable = /^(?:input|select|textarea|keygen)/i;
-
-    function buildParams(prefix, obj, traditional, add) {
-        var name;
-
-        if (jQuery.isArray(obj)) {
-            // Serialize array item.
-            jQuery.each(obj, function(i, v) {
-                if (traditional || rbracket.test(prefix)) {
-                    // Treat each array item as a scalar.
-                    add(prefix, v);
-
-                } else {
-                    // Item is non-scalar (array or object), encode its numeric index.
-                    buildParams(prefix + "[" + (typeof v === "object" ? i : "") + "]", v, traditional, add);
-                }
-            });
-
-        } else if (!traditional && jQuery.type(obj) === "object") {
-            // Serialize object item.
-            for (name in obj) {
-                buildParams(prefix + "[" + name + "]", obj[name], traditional, add);
-            }
-
-        } else {
-            // Serialize scalar item.
-            add(prefix, obj);
-        }
-    }
-
-    // Serialize an array of form elements or a set of
-    // key/values into a query string
-    jQuery.param = function(a, traditional) {
-        var prefix,
-            s = [],
-            add = function(key, value) {
-                // If value is a function, invoke it and return its value
-                value = jQuery.isFunction(value) ? value() : (value == null ? "" : value);
-                s[s.length] = encodeURIComponent(key) + "=" + encodeURIComponent(value);
-            };
-
-        // Set traditional to true for jQuery <= 1.3.2 behavior.
-        if (traditional === undefined) {
-            traditional = jQuery.ajaxSettings && jQuery.ajaxSettings.traditional;
-        }
-
-        // If an array was passed in, assume that it is an array of form elements.
-        if (jQuery.isArray(a) || (a.jquery && !jQuery.isPlainObject(a))) {
-            // Serialize the form elements
-            jQuery.each(a, function() {
-                add(this.name, this.value);
-            });
-
-        } else {
-            // If traditional, encode the "old" way (the way 1.3.2 or older
-            // did it), otherwise encode params recursively.
-            for (prefix in a) {
-                buildParams(prefix, a[prefix], traditional, add);
-            }
-        }
-
-        // Return the resulting serialization
-        return s.join("&").replace(r20, "+");
+    jQuery.ajaxSettings.xhr = function() {
+        try {
+            return new window.XMLHttpRequest();
+        } catch (e) {}
     };
 
-    jQuery.fn.extend({
-        serialize: function() {
-            return jQuery.param(this.serializeArray());
-        },
-        serializeArray: function() {
-            return this.map(function() {
-                    // Can add propHook for "elements" to filter or add form elements
-                    var elements = jQuery.prop(this, "elements");
-                    return elements ? jQuery.makeArray(elements) : this;
-                })
-                .filter(function() {
-                    var type = this.type;
-                    // Use .is(":disabled") so that fieldset[disabled] works
-                    return this.name && !jQuery(this).is(":disabled") &&
-                        rsubmittable.test(this.nodeName) && !rsubmitterTypes.test(type) &&
-                        (this.checked || !rcheckableType.test(type));
-                })
-                .map(function(i, elem) {
-                    var val = jQuery(this).val();
-
-                    return val == null ?
-                        null :
-                        jQuery.isArray(val) ?
-                        jQuery.map(val, function(val) {
-                            return {
-                                name: elem.name,
-                                value: val.replace(rCRLF, "\r\n")
-                            };
-                        }) : {
-                            name: elem.name,
-                            value: val.replace(rCRLF, "\r\n")
-                        };
-                }).get();
-        }
-    });
-
-
-    // Create the request object
-    // (This is still attached to ajaxSettings for backward compatibility)
-    jQuery.ajaxSettings.xhr = window.ActiveXObject !== undefined ?
-        // Support: IE6+
-        function() {
-
-            // XHR cannot access local files, always use ActiveX for that case
-            return !this.isLocal &&
-
-                // Support: IE7-8
-                // oldIE XHR does not support non-RFC2616 methods (#13240)
-                // See http://msdn.microsoft.com/en-us/library/ie/ms536648(v=vs.85).aspx
-                // and http://www.w3.org/Protocols/rfc2616/rfc2616-sec9.html#sec9
-                // Although this check for six methods instead of eight
-                // since IE also does not support "trace" and "connect"
-                /^(get|post|head|put|delete|options)$/i.test(this.type) &&
+    var xhrSuccessStatus = {
 
-                createStandardXHR() || createActiveXHR();
-        } :
-        // For all other browsers, use the standard XMLHttpRequest object
-        createStandardXHR;
+            // File protocol always yields status code 0, assume 200
+            0: 200,
 
-    var xhrId = 0,
-        xhrCallbacks = {},
+            // Support: IE <=9 only
+            // trac-1450: sometimes IE returns 1223 when it should be 204
+            1223: 204
+        },
         xhrSupported = jQuery.ajaxSettings.xhr();
 
-    // Support: IE<10
-    // Open requests must be manually aborted on unload (#5280)
-    if (window.ActiveXObject) {
-        jQuery(window).on("unload", function() {
-            for (var key in xhrCallbacks) {
-                xhrCallbacks[key](undefined, true);
-            }
-        });
-    }
-
-    // Determine support properties
     support.cors = !!xhrSupported && ("withCredentials" in xhrSupported);
-    xhrSupported = support.ajax = !!xhrSupported;
-
-    // Create transport if the browser can provide an xhr
-    if (xhrSupported) {
+    support.ajax = xhrSupported = !!xhrSupported;
 
-        jQuery.ajaxTransport(function(options) {
-            // Cross domain only allowed if supported through XMLHttpRequest
-            if (!options.crossDomain || support.cors) {
+    jQuery.ajaxTransport(function(options) {
+        var callback, errorCallback;
 
-                var callback;
+        // Cross domain only allowed if supported through XMLHttpRequest
+        if (support.cors || xhrSupported && !options.crossDomain) {
+            return {
+                send: function(headers, complete) {
+                    var i,
+                        xhr = options.xhr();
+
+                    xhr.open(
+                        options.type,
+                        options.url,
+                        options.async,
+                        options.username,
+                        options.password
+                    );
 
-                return {
-                    send: function(headers, complete) {
-                        var i,
-                            xhr = options.xhr(),
-                            id = ++xhrId;
-
-                        // Open the socket
-                        xhr.open(options.type, options.url, options.async, options.username, options.password);
-
-                        // Apply custom fields if provided
-                        if (options.xhrFields) {
-                            for (i in options.xhrFields) {
-                                xhr[i] = options.xhrFields[i];
-                            }
+                    // Apply custom fields if provided
+                    if (options.xhrFields) {
+                        for (i in options.xhrFields) {
+                            xhr[i] = options.xhrFields[i];
                         }
+                    }
 
-                        // Override mime type if needed
-                        if (options.mimeType && xhr.overrideMimeType) {
-                            xhr.overrideMimeType(options.mimeType);
-                        }
-
-                        // X-Requested-With header
-                        // For cross-domain requests, seeing as conditions for a preflight are
-                        // akin to a jigsaw puzzle, we simply never set it to be sure.
-                        // (it can always be set on a per-request basis or even using ajaxSetup)
-                        // For same-domain requests, won't change header if already provided.
-                        if (!options.crossDomain && !headers["X-Requested-With"]) {
-                            headers["X-Requested-With"] = "XMLHttpRequest";
-                        }
-
-                        // Set headers
-                        for (i in headers) {
-                            // Support: IE<9
-                            // IE's ActiveXObject throws a 'Type Mismatch' exception when setting
-                            // request header to a null-value.
-                            //
-                            // To keep consistent with other XHR implementations, cast the value
-                            // to string and ignore `undefined`.
-                            if (headers[i] !== undefined) {
-                                xhr.setRequestHeader(i, headers[i] + "");
-                            }
-                        }
+                    // Override mime type if needed
+                    if (options.mimeType && xhr.overrideMimeType) {
+                        xhr.overrideMimeType(options.mimeType);
+                    }
 
-                        // Do send the request
-                        // This may raise an exception which is actually
-                        // handled in jQuery.ajax (so no try/catch here)
-                        xhr.send((options.hasContent && options.data) || null);
-
-                        // Listener
-                        callback = function(_, isAbort) {
-                            var status, statusText, responses;
-
-                            // Was never called and is aborted or complete
-                            if (callback && (isAbort || xhr.readyState === 4)) {
-                                // Clean up
-                                delete xhrCallbacks[id];
-                                callback = undefined;
-                                xhr.onreadystatechange = jQuery.noop;
-
-                                // Abort manually if needed
-                                if (isAbort) {
-                                    if (xhr.readyState !== 4) {
-                                        xhr.abort();
-                                    }
-                                } else {
-                                    responses = {};
-                                    status = xhr.status;
+                    // X-Requested-With header
+                    // For cross-domain requests, seeing as conditions for a preflight are
+                    // akin to a jigsaw puzzle, we simply never set it to be sure.
+                    // (it can always be set on a per-request basis or even using ajaxSetup)
+                    // For same-domain requests, won't change header if already provided.
+                    if (!options.crossDomain && !headers["X-Requested-With"]) {
+                        headers["X-Requested-With"] = "XMLHttpRequest";
+                    }
 
-                                    // Support: IE<10
-                                    // Accessing binary-data responseText throws an exception
-                                    // (#11426)
-                                    if (typeof xhr.responseText === "string") {
-                                        responses.text = xhr.responseText;
-                                    }
+                    // Set headers
+                    for (i in headers) {
+                        xhr.setRequestHeader(i, headers[i]);
+                    }
 
-                                    // Firefox throws an exception when accessing
-                                    // statusText for faulty cross-domain requests
-                                    try {
-                                        statusText = xhr.statusText;
-                                    } catch (e) {
-                                        // We normalize with Webkit giving an empty statusText
-                                        statusText = "";
-                                    }
+                    // Callback
+                    callback = function(type) {
+                        return function() {
+                            if (callback) {
+                                callback = errorCallback = xhr.onload =
+                                    xhr.onerror = xhr.onabort = xhr.ontimeout =
+                                    xhr.onreadystatechange = null;
+
+                                if (type === "abort") {
+                                    xhr.abort();
+                                } else if (type === "error") {
 
-                                    // Filter status for non standard behaviors
+                                    // Support: IE <=9 only
+                                    // On a manual native abort, IE9 throws
+                                    // errors on any property access that is not readyState
+                                    if (typeof xhr.status !== "number") {
+                                        complete(0, "error");
+                                    } else {
+                                        complete(
 
-                                    // If the request is local and we have data: assume a success
-                                    // (success with no data won't get notified, that's the best we
-                                    // can do given current implementations)
-                                    if (!status && options.isLocal && !options.crossDomain) {
-                                        status = responses.text ? 200 : 404;
-                                        // IE - #1450: sometimes returns 1223 when it should be 204
-                                    } else if (status === 1223) {
-                                        status = 204;
+                                            // File: protocol always yields status 0; see trac-8605, trac-14207
+                                            xhr.status,
+                                            xhr.statusText
+                                        );
                                     }
+                                } else {
+                                    complete(
+                                        xhrSuccessStatus[xhr.status] || xhr.status,
+                                        xhr.statusText,
+
+                                        // Support: IE <=9 only
+                                        // IE9 has no XHR2 but throws on binary (trac-11426)
+                                        // For XHR2 non-text, let the caller handle it (gh-2498)
+                                        (xhr.responseType || "text") !== "text" ||
+                                        typeof xhr.responseText !== "string" ? {
+                                            binary: xhr.response
+                                        } : {
+                                            text: xhr.responseText
+                                        },
+                                        xhr.getAllResponseHeaders()
+                                    );
                                 }
                             }
+                        };
+                    };
+
+                    // Listen to events
+                    xhr.onload = callback();
+                    errorCallback = xhr.onerror = xhr.ontimeout = callback("error");
+
+                    // Support: IE 9 only
+                    // Use onreadystatechange to replace onabort
+                    // to handle uncaught aborts
+                    if (xhr.onabort !== undefined) {
+                        xhr.onabort = errorCallback;
+                    } else {
+                        xhr.onreadystatechange = function() {
 
-                            // Call complete if needed
-                            if (responses) {
-                                complete(status, statusText, responses, xhr.getAllResponseHeaders());
+                            // Check readyState before timeout as it changes
+                            if (xhr.readyState === 4) {
+
+                                // Allow onerror to be called first,
+                                // but that will not handle a native abort
+                                // Also, save errorCallback to a variable
+                                // as xhr.onerror cannot be accessed
+                                window.setTimeout(function() {
+                                    if (callback) {
+                                        errorCallback();
+                                    }
+                                });
                             }
                         };
+                    }
 
-                        if (!options.async) {
-                            // if we're in sync mode we fire the callback
-                            callback();
-                        } else if (xhr.readyState === 4) {
-                            // (IE6 & IE7) if it's in cache and has been
-                            // retrieved directly we need to fire the callback
-                            setTimeout(callback);
-                        } else {
-                            // Add to the list of active xhr callbacks
-                            xhr.onreadystatechange = xhrCallbacks[id] = callback;
-                        }
-                    },
+                    // Create the abort callback
+                    callback = callback("abort");
+
+                    try {
 
-                    abort: function() {
+                        // Do send the request (this may raise an exception)
+                        xhr.send(options.hasContent && options.data || null);
+                    } catch (e) {
+
+                        // trac-14683: Only rethrow if this hasn't been notified as an error yet
                         if (callback) {
-                            callback(undefined, true);
+                            throw e;
                         }
                     }
-                };
-            }
-        });
-    }
+                },
 
-    // Functions to create xhrs
-    function createStandardXHR() {
-        try {
-            return new window.XMLHttpRequest();
-        } catch (e) {}
-    }
+                abort: function() {
+                    if (callback) {
+                        callback();
+                    }
+                }
+            };
+        }
+    });
 
-    function createActiveXHR() {
-        try {
-            return new window.ActiveXObject("Microsoft.XMLHTTP");
-        } catch (e) {}
-    }
 
 
 
+    // Prevent auto-execution of scripts when no explicit dataType was provided (See gh-2432)
+    jQuery.ajaxPrefilter(function(s) {
+        if (s.crossDomain) {
+            s.contents.script = false;
+        }
+    });
 
     // Install script dataType
     jQuery.ajaxSetup({
         accepts: {
-            script: "text/javascript, application/javascript, application/ecmascript, application/x-ecmascript"
+            script: "text/javascript, application/javascript, " +
+                "application/ecmascript, application/x-ecmascript"
         },
         contents: {
-            script: /(?:java|ecma)script/
+            script: /\b(?:java|ecma)script\b/
         },
         converters: {
             "text script": function(text) {
                 jQuery.globalEval(text);
                 return text;
             }
         }
     });
 
-    // Handle cache's special case and global
+    // Handle cache's special case and crossDomain
     jQuery.ajaxPrefilter("script", function(s) {
         if (s.cache === undefined) {
             s.cache = false;
         }
         if (s.crossDomain) {
             s.type = "GET";
-            s.global = false;
         }
     });
 
     // Bind script tag hack transport
     jQuery.ajaxTransport("script", function(s) {
 
-        // This transport only deals with cross domain requests
-        if (s.crossDomain) {
-
-            var script,
-                head = document.head || jQuery("head")[0] || document.documentElement;
-
+        // This transport only deals with cross domain or forced-by-attrs requests
+        if (s.crossDomain || s.scriptAttrs) {
+            var script, callback;
             return {
-
-                send: function(_, callback) {
-
-                    script = document.createElement("script");
-
-                    script.async = true;
-
-                    if (s.scriptCharset) {
-                        script.charset = s.scriptCharset;
-                    }
-
-                    script.src = s.url;
-
-                    // Attach handlers for all browsers
-                    script.onload = script.onreadystatechange = function(_, isAbort) {
-
-                        if (isAbort || !script.readyState || /loaded|complete/.test(script.readyState)) {
-
-                            // Handle memory leak in IE
-                            script.onload = script.onreadystatechange = null;
-
-                            // Remove the script
-                            if (script.parentNode) {
-                                script.parentNode.removeChild(script);
+                send: function(_, complete) {
+                    script = jQuery("<script>")
+                        .attr(s.scriptAttrs || {})
+                        .prop({
+                            charset: s.scriptCharset,
+                            src: s.url
+                        })
+                        .on("load error", callback = function(evt) {
+                            script.remove();
+                            callback = null;
+                            if (evt) {
+                                complete(evt.type === "error" ? 404 : 200, evt.type);
                             }
+                        });
 
-                            // Dereference the script
-                            script = null;
-
-                            // Callback if not abort
-                            if (!isAbort) {
-                                callback(200, "success");
-                            }
-                        }
-                    };
-
-                    // Circumvent IE6 bugs with base elements (#2709 and #4378) by prepending
                     // Use native DOM manipulation to avoid our domManip AJAX trickery
-                    head.insertBefore(script, head.firstChild);
+                    document.head.appendChild(script[0]);
                 },
-
                 abort: function() {
-                    if (script) {
-                        script.onload(undefined, true);
+                    if (callback) {
+                        callback();
                     }
                 }
             };
         }
     });
 
 
@@ -9894,34 +10302,37 @@
     var oldCallbacks = [],
         rjsonp = /(=)\?(?=&|$)|\?\?/;
 
     // Default jsonp settings
     jQuery.ajaxSetup({
         jsonp: "callback",
         jsonpCallback: function() {
-            var callback = oldCallbacks.pop() || (jQuery.expando + "_" + (nonce++));
+            var callback = oldCallbacks.pop() || (jQuery.expando + "_" + (nonce.guid++));
             this[callback] = true;
             return callback;
         }
     });
 
     // Detect, normalize options and install callbacks for jsonp requests
     jQuery.ajaxPrefilter("json jsonp", function(s, originalSettings, jqXHR) {
 
         var callbackName, overwritten, responseContainer,
             jsonProp = s.jsonp !== false && (rjsonp.test(s.url) ?
                 "url" :
-                typeof s.data === "string" && !(s.contentType || "").indexOf("application/x-www-form-urlencoded") && rjsonp.test(s.data) && "data"
+                typeof s.data === "string" &&
+                (s.contentType || "")
+                .indexOf("application/x-www-form-urlencoded") === 0 &&
+                rjsonp.test(s.data) && "data"
             );
 
         // Handle iff the expected data type is "jsonp" or we have a parameter to set
         if (jsonProp || s.dataTypes[0] === "jsonp") {
 
             // Get callback name, remembering preexisting value associated with it
-            callbackName = s.jsonpCallback = jQuery.isFunction(s.jsonpCallback) ?
+            callbackName = s.jsonpCallback = isFunction(s.jsonpCallback) ?
                 s.jsonpCallback() :
                 s.jsonpCallback;
 
             // Insert callback into url or form data
             if (jsonProp) {
                 s[jsonProp] = s[jsonProp].replace(rjsonp, "$1" + callbackName);
             } else if (s.jsonp !== false) {
@@ -9932,106 +10343,139 @@
             s.converters["script json"] = function() {
                 if (!responseContainer) {
                     jQuery.error(callbackName + " was not called");
                 }
                 return responseContainer[0];
             };
 
-            // force json dataType
+            // Force json dataType
             s.dataTypes[0] = "json";
 
             // Install callback
             overwritten = window[callbackName];
             window[callbackName] = function() {
                 responseContainer = arguments;
             };
 
             // Clean-up function (fires after converters)
             jqXHR.always(function() {
-                // Restore preexisting value
-                window[callbackName] = overwritten;
+
+                // If previous value didn't exist - remove it
+                if (overwritten === undefined) {
+                    jQuery(window).removeProp(callbackName);
+
+                    // Otherwise restore preexisting value
+                } else {
+                    window[callbackName] = overwritten;
+                }
 
                 // Save back as free
                 if (s[callbackName]) {
-                    // make sure that re-using the options doesn't screw things around
+
+                    // Make sure that re-using the options doesn't screw things around
                     s.jsonpCallback = originalSettings.jsonpCallback;
 
-                    // save the callback name for future use
+                    // Save the callback name for future use
                     oldCallbacks.push(callbackName);
                 }
 
                 // Call if it was a function and we have a response
-                if (responseContainer && jQuery.isFunction(overwritten)) {
+                if (responseContainer && isFunction(overwritten)) {
                     overwritten(responseContainer[0]);
                 }
 
                 responseContainer = overwritten = undefined;
             });
 
             // Delegate to script
             return "script";
         }
     });
 
 
 
 
-    // data: string of html
-    // context (optional): If specified, the fragment will be created in this context, defaults to document
+    // Support: Safari 8 only
+    // In Safari 8 documents created via document.implementation.createHTMLDocument
+    // collapse sibling forms: the second one becomes a child of the first one.
+    // Because of that, this security measure has to be disabled in Safari 8.
+    // https://bugs.webkit.org/show_bug.cgi?id=137337
+    support.createHTMLDocument = (function() {
+        var body = document.implementation.createHTMLDocument("").body;
+        body.innerHTML = "<form></form><form></form>";
+        return body.childNodes.length === 2;
+    })();
+
+
+    // Argument "data" should be string of html
+    // context (optional): If specified, the fragment will be created in this context,
+    // defaults to document
     // keepScripts (optional): If true, will include scripts passed in the html string
     jQuery.parseHTML = function(data, context, keepScripts) {
-        if (!data || typeof data !== "string") {
-            return null;
+        if (typeof data !== "string") {
+            return [];
         }
         if (typeof context === "boolean") {
             keepScripts = context;
             context = false;
         }
-        context = context || document;
 
-        var parsed = rsingleTag.exec(data),
-            scripts = !keepScripts && [];
+        var base, parsed, scripts;
+
+        if (!context) {
+
+            // Stop scripts or inline event handlers from being executed immediately
+            // by using document.implementation
+            if (support.createHTMLDocument) {
+                context = document.implementation.createHTMLDocument("");
+
+                // Set the base href for the created document
+                // so any parsed elements with URLs
+                // are based on the document's URL (gh-2965)
+                base = context.createElement("base");
+                base.href = document.location.href;
+                context.head.appendChild(base);
+            } else {
+                context = document;
+            }
+        }
+
+        parsed = rsingleTag.exec(data);
+        scripts = !keepScripts && [];
 
         // Single tag
         if (parsed) {
             return [context.createElement(parsed[1])];
         }
 
-        parsed = jQuery.buildFragment([data], context, scripts);
+        parsed = buildFragment([data], context, scripts);
 
         if (scripts && scripts.length) {
             jQuery(scripts).remove();
         }
 
         return jQuery.merge([], parsed.childNodes);
     };
 
 
-    // Keep a copy of the old load method
-    var _load = jQuery.fn.load;
-
     /**
      * Load a url into a page
      */
     jQuery.fn.load = function(url, params, callback) {
-        if (typeof url !== "string" && _load) {
-            return _load.apply(this, arguments);
-        }
-
-        var selector, response, type,
+        var selector, type, response,
             self = this,
             off = url.indexOf(" ");
 
-        if (off >= 0) {
-            selector = jQuery.trim(url.slice(off, url.length));
+        if (off > -1) {
+            selector = stripAndCollapse(url.slice(off));
             url = url.slice(0, off);
         }
 
         // If it's a function
-        if (jQuery.isFunction(params)) {
+        if (isFunction(params)) {
 
             // We assume that it's the callback
             callback = params;
             params = undefined;
 
             // Otherwise, build a param string
         } else if (params && typeof params === "object") {
@@ -10039,16 +10483,18 @@
         }
 
         // If we have elements to modify, make the request
         if (self.length > 0) {
             jQuery.ajax({
                 url: url,
 
-                // if "type" variable is undefined, then "GET" method will be used
-                type: type,
+                // If "type" variable is undefined, then "GET" method will be used.
+                // Make value of this field explicit since
+                // user can override it through ajaxSetup method
+                type: type || "GET",
                 dataType: "html",
                 data: params
             }).done(function(responseText) {
 
                 // Save response for use in complete callback
                 response = arguments;
 
@@ -10057,228 +10503,252 @@
                     // If a selector was specified, locate the right elements in a dummy div
                     // Exclude scripts to avoid IE 'Permission Denied' errors
                     jQuery("<div>").append(jQuery.parseHTML(responseText)).find(selector) :
 
                     // Otherwise use the full result
                     responseText);
 
-            }).complete(callback && function(jqXHR, status) {
-                self.each(callback, response || [jqXHR.responseText, status, jqXHR]);
+                // If the request succeeds, this function gets "data", "status", "jqXHR"
+                // but they are ignored because response was set above.
+                // If it fails, this function gets "jqXHR", "status", "error"
+            }).always(callback && function(jqXHR, status) {
+                self.each(function() {
+                    callback.apply(this, response || [jqXHR.responseText, status, jqXHR]);
+                });
             });
         }
 
         return this;
     };
 
 
 
 
-    jQuery.expr.filters.animated = function(elem) {
+    jQuery.expr.pseudos.animated = function(elem) {
         return jQuery.grep(jQuery.timers, function(fn) {
             return elem === fn.elem;
         }).length;
     };
 
 
 
 
-
-    var docElem = window.document.documentElement;
-
-    /**
-     * Gets a window from an element
-     */
-    function getWindow(elem) {
-        return jQuery.isWindow(elem) ?
-            elem :
-            elem.nodeType === 9 ?
-            elem.defaultView || elem.parentWindow :
-            false;
-    }
-
     jQuery.offset = {
         setOffset: function(elem, options, i) {
             var curPosition, curLeft, curCSSTop, curTop, curOffset, curCSSLeft, calculatePosition,
                 position = jQuery.css(elem, "position"),
                 curElem = jQuery(elem),
                 props = {};
 
-            // set position first, in-case top/left are set even on static elem
+            // Set position first, in-case top/left are set even on static elem
             if (position === "static") {
                 elem.style.position = "relative";
             }
 
             curOffset = curElem.offset();
             curCSSTop = jQuery.css(elem, "top");
             curCSSLeft = jQuery.css(elem, "left");
             calculatePosition = (position === "absolute" || position === "fixed") &&
-                jQuery.inArray("auto", [curCSSTop, curCSSLeft]) > -1;
+                (curCSSTop + curCSSLeft).indexOf("auto") > -1;
 
-            // need to be able to calculate position if either top or left is auto and position is either absolute or fixed
+            // Need to be able to calculate position if either
+            // top or left is auto and position is either absolute or fixed
             if (calculatePosition) {
                 curPosition = curElem.position();
                 curTop = curPosition.top;
                 curLeft = curPosition.left;
+
             } else {
                 curTop = parseFloat(curCSSTop) || 0;
                 curLeft = parseFloat(curCSSLeft) || 0;
             }
 
-            if (jQuery.isFunction(options)) {
-                options = options.call(elem, i, curOffset);
+            if (isFunction(options)) {
+
+                // Use jQuery.extend here to allow modification of coordinates argument (gh-1848)
+                options = options.call(elem, i, jQuery.extend({}, curOffset));
             }
 
             if (options.top != null) {
                 props.top = (options.top - curOffset.top) + curTop;
             }
             if (options.left != null) {
                 props.left = (options.left - curOffset.left) + curLeft;
             }
 
             if ("using" in options) {
                 options.using.call(elem, props);
+
             } else {
                 curElem.css(props);
             }
         }
     };
 
     jQuery.fn.extend({
+
+        // offset() relates an element's border box to the document origin
         offset: function(options) {
+
+            // Preserve chaining for setter
             if (arguments.length) {
                 return options === undefined ?
                     this :
                     this.each(function(i) {
                         jQuery.offset.setOffset(this, options, i);
                     });
             }
 
-            var docElem, win,
-                box = {
-                    top: 0,
-                    left: 0
-                },
-                elem = this[0],
-                doc = elem && elem.ownerDocument;
+            var rect, win,
+                elem = this[0];
 
-            if (!doc) {
+            if (!elem) {
                 return;
             }
 
-            docElem = doc.documentElement;
-
-            // Make sure it's not a disconnected DOM node
-            if (!jQuery.contains(docElem, elem)) {
-                return box;
+            // Return zeros for disconnected and hidden (display: none) elements (gh-2310)
+            // Support: IE <=11 only
+            // Running getBoundingClientRect on a
+            // disconnected node in IE throws an error
+            if (!elem.getClientRects().length) {
+                return {
+                    top: 0,
+                    left: 0
+                };
             }
 
-            // If we don't have gBCR, just use 0,0 rather than error
-            // BlackBerry 5, iOS 3 (original iPhone)
-            if (typeof elem.getBoundingClientRect !== strundefined) {
-                box = elem.getBoundingClientRect();
-            }
-            win = getWindow(doc);
+            // Get document-relative position by adding viewport scroll to viewport-relative gBCR
+            rect = elem.getBoundingClientRect();
+            win = elem.ownerDocument.defaultView;
             return {
-                top: box.top + (win.pageYOffset || docElem.scrollTop) - (docElem.clientTop || 0),
-                left: box.left + (win.pageXOffset || docElem.scrollLeft) - (docElem.clientLeft || 0)
+                top: rect.top + win.pageYOffset,
+                left: rect.left + win.pageXOffset
             };
         },
 
+        // position() relates an element's margin box to its offset parent's padding box
+        // This corresponds to the behavior of CSS absolute positioning
         position: function() {
             if (!this[0]) {
                 return;
             }
 
-            var offsetParent, offset,
+            var offsetParent, offset, doc,
+                elem = this[0],
                 parentOffset = {
                     top: 0,
                     left: 0
-                },
-                elem = this[0];
+                };
 
-            // fixed elements are offset from window (parentOffset = {top:0, left: 0}, because it is its only offset parent
+            // position:fixed elements are offset from the viewport, which itself always has zero offset
             if (jQuery.css(elem, "position") === "fixed") {
-                // we assume that getBoundingClientRect is available when computed position is fixed
+
+                // Assume position:fixed implies availability of getBoundingClientRect
                 offset = elem.getBoundingClientRect();
-            } else {
-                // Get *real* offsetParent
-                offsetParent = this.offsetParent();
 
-                // Get correct offsets
+            } else {
                 offset = this.offset();
-                if (!jQuery.nodeName(offsetParent[0], "html")) {
-                    parentOffset = offsetParent.offset();
-                }
 
-                // Add offsetParent borders
-                parentOffset.top += jQuery.css(offsetParent[0], "borderTopWidth", true);
-                parentOffset.left += jQuery.css(offsetParent[0], "borderLeftWidth", true);
+                // Account for the *real* offset parent, which can be the document or its root element
+                // when a statically positioned element is identified
+                doc = elem.ownerDocument;
+                offsetParent = elem.offsetParent || doc.documentElement;
+                while (offsetParent &&
+                    (offsetParent === doc.body || offsetParent === doc.documentElement) &&
+                    jQuery.css(offsetParent, "position") === "static") {
+
+                    offsetParent = offsetParent.parentNode;
+                }
+                if (offsetParent && offsetParent !== elem && offsetParent.nodeType === 1) {
+
+                    // Incorporate borders into its offset, since they are outside its content origin
+                    parentOffset = jQuery(offsetParent).offset();
+                    parentOffset.top += jQuery.css(offsetParent, "borderTopWidth", true);
+                    parentOffset.left += jQuery.css(offsetParent, "borderLeftWidth", true);
+                }
             }
 
             // Subtract parent offsets and element margins
-            // note: when an element has margin: auto the offsetLeft and marginLeft
-            // are the same in Safari causing offset.left to incorrectly be 0
             return {
                 top: offset.top - parentOffset.top - jQuery.css(elem, "marginTop", true),
                 left: offset.left - parentOffset.left - jQuery.css(elem, "marginLeft", true)
             };
         },
 
+        // This method will return documentElement in the following cases:
+        // 1) For the element inside the iframe without offsetParent, this method will return
+        //    documentElement of the parent window
+        // 2) For the hidden or detached element
+        // 3) For body or html element, i.e. in case of the html node - it will return itself
+        //
+        // but those exceptions were never presented as a real life use-cases
+        // and might be considered as more preferable results.
+        //
+        // This logic, however, is not guaranteed and can change at any point in the future
         offsetParent: function() {
             return this.map(function() {
-                var offsetParent = this.offsetParent || docElem;
+                var offsetParent = this.offsetParent;
 
-                while (offsetParent && (!jQuery.nodeName(offsetParent, "html") && jQuery.css(offsetParent, "position") === "static")) {
+                while (offsetParent && jQuery.css(offsetParent, "position") === "static") {
                     offsetParent = offsetParent.offsetParent;
                 }
-                return offsetParent || docElem;
+
+                return offsetParent || documentElement;
             });
         }
     });
 
     // Create scrollLeft and scrollTop methods
     jQuery.each({
         scrollLeft: "pageXOffset",
         scrollTop: "pageYOffset"
     }, function(method, prop) {
-        var top = /Y/.test(prop);
+        var top = "pageYOffset" === prop;
 
         jQuery.fn[method] = function(val) {
             return access(this, function(elem, method, val) {
-                var win = getWindow(elem);
+
+                // Coalesce documents and windows
+                var win;
+                if (isWindow(elem)) {
+                    win = elem;
+                } else if (elem.nodeType === 9) {
+                    win = elem.defaultView;
+                }
 
                 if (val === undefined) {
-                    return win ? (prop in win) ? win[prop] :
-                        win.document.documentElement[method] :
-                        elem[method];
+                    return win ? win[prop] : elem[method];
                 }
 
                 if (win) {
                     win.scrollTo(
-                        !top ? val : jQuery(win).scrollLeft(),
-                        top ? val : jQuery(win).scrollTop()
+                        !top ? val : win.pageXOffset,
+                        top ? val : win.pageYOffset
                     );
 
                 } else {
                     elem[method] = val;
                 }
-            }, method, val, arguments.length, null);
+            }, method, val, arguments.length);
         };
     });
 
+    // Support: Safari <=7 - 9.1, Chrome <=37 - 49
     // Add the top/left cssHooks using jQuery.fn.position
     // Webkit bug: https://bugs.webkit.org/show_bug.cgi?id=29084
-    // getComputedStyle returns percent when specified for top/left/bottom/right
-    // rather than make the css module depend on the offset module, we just check for it here
-    jQuery.each(["top", "left"], function(i, prop) {
+    // Blink bug: https://bugs.chromium.org/p/chromium/issues/detail?id=589347
+    // getComputedStyle returns percent when specified for top/left/bottom/right;
+    // rather than make the css module depend on the offset module, just check for it here
+    jQuery.each(["top", "left"], function(_i, prop) {
         jQuery.cssHooks[prop] = addGetHookIf(support.pixelPosition,
             function(elem, computed) {
                 if (computed) {
                     computed = curCSS(elem, prop);
-                    // if curCSS returns percentage, fallback to offset
+
+                    // If curCSS returns percentage, fallback to offset
                     return rnumnonpx.test(computed) ?
                         jQuery(elem).position()[prop] + "px" :
                         computed;
                 }
             }
         );
     });
@@ -10290,61 +10760,189 @@
         Width: "width"
     }, function(name, type) {
         jQuery.each({
             padding: "inner" + name,
             content: type,
             "": "outer" + name
         }, function(defaultExtra, funcName) {
-            // margin is only for outerHeight, outerWidth
+
+            // Margin is only for outerHeight, outerWidth
             jQuery.fn[funcName] = function(margin, value) {
                 var chainable = arguments.length && (defaultExtra || typeof margin !== "boolean"),
                     extra = defaultExtra || (margin === true || value === true ? "margin" : "border");
 
                 return access(this, function(elem, type, value) {
                     var doc;
 
-                    if (jQuery.isWindow(elem)) {
-                        // As of 5/8/2012 this will yield incorrect results for Mobile Safari, but there
-                        // isn't a whole lot we can do. See pull request at this URL for discussion:
-                        // https://github.com/jquery/jquery/pull/764
-                        return elem.document.documentElement["client" + name];
+                    if (isWindow(elem)) {
+
+                        // $( window ).outerWidth/Height return w/h including scrollbars (gh-1729)
+                        return funcName.indexOf("outer") === 0 ?
+                            elem["inner" + name] :
+                            elem.document.documentElement["client" + name];
                     }
 
                     // Get document width or height
                     if (elem.nodeType === 9) {
                         doc = elem.documentElement;
 
-                        // Either scroll[Width/Height] or offset[Width/Height] or client[Width/Height], whichever is greatest
-                        // unfortunately, this causes bug #3838 in IE6/8 only, but there is currently no good, small way to fix it.
+                        // Either scroll[Width/Height] or offset[Width/Height] or client[Width/Height],
+                        // whichever is greatest
                         return Math.max(
                             elem.body["scroll" + name], doc["scroll" + name],
                             elem.body["offset" + name], doc["offset" + name],
                             doc["client" + name]
                         );
                     }
 
                     return value === undefined ?
+
                         // Get width or height on the element, requesting but not forcing parseFloat
                         jQuery.css(elem, type, extra) :
 
                         // Set width or height on the element
                         jQuery.style(elem, type, value, extra);
-                }, type, chainable ? margin : undefined, chainable, null);
+                }, type, chainable ? margin : undefined, chainable);
             };
         });
     });
 
 
-    // The number of elements contained in the matched element set
-    jQuery.fn.size = function() {
-        return this.length;
+    jQuery.each([
+        "ajaxStart",
+        "ajaxStop",
+        "ajaxComplete",
+        "ajaxError",
+        "ajaxSuccess",
+        "ajaxSend"
+    ], function(_i, type) {
+        jQuery.fn[type] = function(fn) {
+            return this.on(type, fn);
+        };
+    });
+
+
+
+
+    jQuery.fn.extend({
+
+        bind: function(types, data, fn) {
+            return this.on(types, null, data, fn);
+        },
+        unbind: function(types, fn) {
+            return this.off(types, null, fn);
+        },
+
+        delegate: function(selector, types, data, fn) {
+            return this.on(types, selector, data, fn);
+        },
+        undelegate: function(selector, types, fn) {
+
+            // ( namespace ) or ( selector, types [, fn] )
+            return arguments.length === 1 ?
+                this.off(selector, "**") :
+                this.off(types, selector || "**", fn);
+        },
+
+        hover: function(fnOver, fnOut) {
+            return this.mouseenter(fnOver).mouseleave(fnOut || fnOver);
+        }
+    });
+
+    jQuery.each(
+        ("blur focus focusin focusout resize scroll click dblclick " +
+            "mousedown mouseup mousemove mouseover mouseout mouseenter mouseleave " +
+            "change select submit keydown keypress keyup contextmenu").split(" "),
+        function(_i, name) {
+
+            // Handle event binding
+            jQuery.fn[name] = function(data, fn) {
+                return arguments.length > 0 ?
+                    this.on(name, null, data, fn) :
+                    this.trigger(name);
+            };
+        }
+    );
+
+
+
+
+    // Support: Android <=4.0 only
+    // Make sure we trim BOM and NBSP
+    // Require that the "whitespace run" starts from a non-whitespace
+    // to avoid O(N^2) behavior when the engine would try matching "\s+$" at each space position.
+    var rtrim = /^[\s\uFEFF\xA0]+|([^\s\uFEFF\xA0])[\s\uFEFF\xA0]+$/g;
+
+    // Bind a function to a context, optionally partially applying any
+    // arguments.
+    // jQuery.proxy is deprecated to promote standards (specifically Function#bind)
+    // However, it is not slated for removal any time soon
+    jQuery.proxy = function(fn, context) {
+        var tmp, args, proxy;
+
+        if (typeof context === "string") {
+            tmp = fn[context];
+            context = fn;
+            fn = tmp;
+        }
+
+        // Quick check to determine if target is callable, in the spec
+        // this throws a TypeError, but we will just return undefined.
+        if (!isFunction(fn)) {
+            return undefined;
+        }
+
+        // Simulated bind
+        args = slice.call(arguments, 2);
+        proxy = function() {
+            return fn.apply(context || this, args.concat(slice.call(arguments)));
+        };
+
+        // Set the guid of unique handler to the same of original handler, so it can be removed
+        proxy.guid = fn.guid = fn.guid || jQuery.guid++;
+
+        return proxy;
     };
 
-    jQuery.fn.andSelf = jQuery.fn.addBack;
+    jQuery.holdReady = function(hold) {
+        if (hold) {
+            jQuery.readyWait++;
+        } else {
+            jQuery.ready(true);
+        }
+    };
+    jQuery.isArray = Array.isArray;
+    jQuery.parseJSON = JSON.parse;
+    jQuery.nodeName = nodeName;
+    jQuery.isFunction = isFunction;
+    jQuery.isWindow = isWindow;
+    jQuery.camelCase = camelCase;
+    jQuery.type = toType;
+
+    jQuery.now = Date.now;
+
+    jQuery.isNumeric = function(obj) {
+
+        // As of jQuery 3.0, isNumeric is limited to
+        // strings and numbers (primitives or objects)
+        // that can be coerced to finite numbers (gh-2662)
+        var type = jQuery.type(obj);
+        return (type === "number" || type === "string") &&
 
+            // parseFloat NaNs numeric-cast false positives ("")
+            // ...but misinterprets leading-number strings, particularly hex literals ("0x...")
+            // subtraction forces infinities to NaN
+            !isNaN(obj - parseFloat(obj));
+    };
+
+    jQuery.trim = function(text) {
+        return text == null ?
+            "" :
+            (text + "").replace(rtrim, "$1");
+    };
 
 
 
     // Register as a named AMD module, since jQuery can be concatenated with other
     // files that may use define, but not via a proper concatenation script that
     // understands anonymous AMD modules. A named AMD is safest and most robust
     // way to register. Lowercase jquery is used because AMD module names are
@@ -10363,14 +10961,15 @@
         });
     }
 
 
 
 
     var
+
         // Map over jQuery in case of overwrite
         _jQuery = window.jQuery,
 
         // Map over the $ in case of overwrite
         _$ = window.$;
 
     jQuery.noConflict = function(deep) {
@@ -10381,20 +10980,19 @@
         if (deep && window.jQuery === jQuery) {
             window.jQuery = _jQuery;
         }
 
         return jQuery;
     };
 
-    // Expose jQuery and $ identifiers, even in
-    // AMD (#7102#comment:10, https://github.com/jquery/jquery/pull/557)
-    // and CommonJS for browser emulators (#13566)
-    if (typeof noGlobal === strundefined) {
+    // Expose jQuery and $ identifiers, even in AMD
+    // (trac-7102#comment:10, https://github.com/jquery/jquery/pull/557)
+    // and CommonJS for browser emulators (trac-13566)
+    if (typeof noGlobal === "undefined") {
         window.jQuery = window.$ = jQuery;
     }
 
 
 
 
     return jQuery;
-
-}));
+});
```

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_static/pygments.css` & `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/pygments.css`

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,74 @@
+pre { line-height: 125%; }
+td.linenos .normal { color: inherit; background-color: transparent; padding-left: 5px; padding-right: 5px; }
+span.linenos { color: inherit; background-color: transparent; padding-left: 5px; padding-right: 5px; }
+td.linenos .special { color: #000000; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
+span.linenos.special { color: #000000; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
 .highlight .hll { background-color: #ffffcc }
-.highlight  { background: #eeffcc; }
-.highlight .c { color: #408090; font-style: italic } /* Comment */
+.highlight { background: #f8f8f8; }
+.highlight .c { color: #3D7B7B; font-style: italic } /* Comment */
 .highlight .err { border: 1px solid #FF0000 } /* Error */
-.highlight .k { color: #007020; font-weight: bold } /* Keyword */
+.highlight .k { color: #008000; font-weight: bold } /* Keyword */
 .highlight .o { color: #666666 } /* Operator */
-.highlight .ch { color: #408090; font-style: italic } /* Comment.Hashbang */
-.highlight .cm { color: #408090; font-style: italic } /* Comment.Multiline */
-.highlight .cp { color: #007020 } /* Comment.Preproc */
-.highlight .cpf { color: #408090; font-style: italic } /* Comment.PreprocFile */
-.highlight .c1 { color: #408090; font-style: italic } /* Comment.Single */
-.highlight .cs { color: #408090; background-color: #fff0f0 } /* Comment.Special */
+.highlight .ch { color: #3D7B7B; font-style: italic } /* Comment.Hashbang */
+.highlight .cm { color: #3D7B7B; font-style: italic } /* Comment.Multiline */
+.highlight .cp { color: #9C6500 } /* Comment.Preproc */
+.highlight .cpf { color: #3D7B7B; font-style: italic } /* Comment.PreprocFile */
+.highlight .c1 { color: #3D7B7B; font-style: italic } /* Comment.Single */
+.highlight .cs { color: #3D7B7B; font-style: italic } /* Comment.Special */
 .highlight .gd { color: #A00000 } /* Generic.Deleted */
 .highlight .ge { font-style: italic } /* Generic.Emph */
-.highlight .gr { color: #FF0000 } /* Generic.Error */
+.highlight .gr { color: #E40000 } /* Generic.Error */
 .highlight .gh { color: #000080; font-weight: bold } /* Generic.Heading */
-.highlight .gi { color: #00A000 } /* Generic.Inserted */
-.highlight .go { color: #333333 } /* Generic.Output */
-.highlight .gp { color: #c65d09; font-weight: bold } /* Generic.Prompt */
+.highlight .gi { color: #008400 } /* Generic.Inserted */
+.highlight .go { color: #717171 } /* Generic.Output */
+.highlight .gp { color: #000080; font-weight: bold } /* Generic.Prompt */
 .highlight .gs { font-weight: bold } /* Generic.Strong */
 .highlight .gu { color: #800080; font-weight: bold } /* Generic.Subheading */
 .highlight .gt { color: #0044DD } /* Generic.Traceback */
-.highlight .kc { color: #007020; font-weight: bold } /* Keyword.Constant */
-.highlight .kd { color: #007020; font-weight: bold } /* Keyword.Declaration */
-.highlight .kn { color: #007020; font-weight: bold } /* Keyword.Namespace */
-.highlight .kp { color: #007020 } /* Keyword.Pseudo */
-.highlight .kr { color: #007020; font-weight: bold } /* Keyword.Reserved */
-.highlight .kt { color: #902000 } /* Keyword.Type */
-.highlight .m { color: #208050 } /* Literal.Number */
-.highlight .s { color: #4070a0 } /* Literal.String */
-.highlight .na { color: #4070a0 } /* Name.Attribute */
-.highlight .nb { color: #007020 } /* Name.Builtin */
-.highlight .nc { color: #0e84b5; font-weight: bold } /* Name.Class */
-.highlight .no { color: #60add5 } /* Name.Constant */
-.highlight .nd { color: #555555; font-weight: bold } /* Name.Decorator */
-.highlight .ni { color: #d55537; font-weight: bold } /* Name.Entity */
-.highlight .ne { color: #007020 } /* Name.Exception */
-.highlight .nf { color: #06287e } /* Name.Function */
-.highlight .nl { color: #002070; font-weight: bold } /* Name.Label */
-.highlight .nn { color: #0e84b5; font-weight: bold } /* Name.Namespace */
-.highlight .nt { color: #062873; font-weight: bold } /* Name.Tag */
-.highlight .nv { color: #bb60d5 } /* Name.Variable */
-.highlight .ow { color: #007020; font-weight: bold } /* Operator.Word */
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
 .highlight .w { color: #bbbbbb } /* Text.Whitespace */
-.highlight .mb { color: #208050 } /* Literal.Number.Bin */
-.highlight .mf { color: #208050 } /* Literal.Number.Float */
-.highlight .mh { color: #208050 } /* Literal.Number.Hex */
-.highlight .mi { color: #208050 } /* Literal.Number.Integer */
-.highlight .mo { color: #208050 } /* Literal.Number.Oct */
-.highlight .sa { color: #4070a0 } /* Literal.String.Affix */
-.highlight .sb { color: #4070a0 } /* Literal.String.Backtick */
-.highlight .sc { color: #4070a0 } /* Literal.String.Char */
-.highlight .dl { color: #4070a0 } /* Literal.String.Delimiter */
-.highlight .sd { color: #4070a0; font-style: italic } /* Literal.String.Doc */
-.highlight .s2 { color: #4070a0 } /* Literal.String.Double */
-.highlight .se { color: #4070a0; font-weight: bold } /* Literal.String.Escape */
-.highlight .sh { color: #4070a0 } /* Literal.String.Heredoc */
-.highlight .si { color: #70a0d0; font-style: italic } /* Literal.String.Interpol */
-.highlight .sx { color: #c65d09 } /* Literal.String.Other */
-.highlight .sr { color: #235388 } /* Literal.String.Regex */
-.highlight .s1 { color: #4070a0 } /* Literal.String.Single */
-.highlight .ss { color: #517918 } /* Literal.String.Symbol */
-.highlight .bp { color: #007020 } /* Name.Builtin.Pseudo */
-.highlight .fm { color: #06287e } /* Name.Function.Magic */
-.highlight .vc { color: #bb60d5 } /* Name.Variable.Class */
-.highlight .vg { color: #bb60d5 } /* Name.Variable.Global */
-.highlight .vi { color: #bb60d5 } /* Name.Variable.Instance */
-.highlight .vm { color: #bb60d5 } /* Name.Variable.Magic */
-.highlight .il { color: #208050 } /* Literal.Number.Integer.Long */
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

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/_static/underscore.js` & `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_static/underscore.js`

 * *Files 27% similar despite different names*

#### js-beautify {}

```diff
@@ -1,1173 +1,447 @@
-//     Underscore.js 1.8.3
-//     http://underscorejs.org
-//     (c) 2009-2015 Jeremy Ashkenas, DocumentCloud and Investigative Reporters & Editors
-//     Underscore may be freely distributed under the MIT license.
-
-(function() {
-
-    // Baseline setup
-    // --------------
+(function(global, factory) {
+    typeof exports === 'object' && typeof module !== 'undefined' ? module.exports = factory() :
+        typeof define === 'function' && define.amd ? define('underscore', factory) :
+        (global = typeof globalThis !== 'undefined' ? globalThis : global || self, (function() {
+            var current = global._;
+            var exports = global._ = factory();
+            exports.noConflict = function() {
+                global._ = current;
+                return exports;
+            };
+        }()));
+}(this, (function() {
+    //     Underscore.js 1.13.4
+    //     https://underscorejs.org
+    //     (c) 2009-2022 Jeremy Ashkenas, Julian Gonggrijp, and DocumentCloud and Investigative Reporters & Editors
+    //     Underscore may be freely distributed under the MIT license.
 
-    // Establish the root object, `window` in the browser, or `exports` on the server.
-    var root = this;
+    // Current version.
+    var VERSION = '1.13.4';
 
-    // Save the previous value of the `_` variable.
-    var previousUnderscore = root._;
+    // Establish the root object, `window` (`self`) in the browser, `global`
+    // on the server, or `this` in some virtual machines. We use `self`
+    // instead of `window` for `WebWorker` support.
+    var root = (typeof self == 'object' && self.self === self && self) ||
+        (typeof global == 'object' && global.global === global && global) ||
+        Function('return this')() || {};
 
     // Save bytes in the minified (but not gzipped) version:
     var ArrayProto = Array.prototype,
-        ObjProto = Object.prototype,
-        FuncProto = Function.prototype;
+        ObjProto = Object.prototype;
+    var SymbolProto = typeof Symbol !== 'undefined' ? Symbol.prototype : null;
 
     // Create quick reference variables for speed access to core prototypes.
-    var
-        push = ArrayProto.push,
+    var push = ArrayProto.push,
         slice = ArrayProto.slice,
         toString = ObjProto.toString,
         hasOwnProperty = ObjProto.hasOwnProperty;
 
-    // All **ECMAScript 5** native function implementations that we hope to use
+    // Modern feature detection.
+    var supportsArrayBuffer = typeof ArrayBuffer !== 'undefined',
+        supportsDataView = typeof DataView !== 'undefined';
+
+    // All **ECMAScript 5+** native function implementations that we hope to use
     // are declared here.
-    var
-        nativeIsArray = Array.isArray,
+    var nativeIsArray = Array.isArray,
         nativeKeys = Object.keys,
-        nativeBind = FuncProto.bind,
-        nativeCreate = Object.create;
-
-    // Naked function reference for surrogate-prototype-swapping.
-    var Ctor = function() {};
-
-    // Create a safe reference to the Underscore object for use below.
-    var _ = function(obj) {
-        if (obj instanceof _) return obj;
-        if (!(this instanceof _)) return new _(obj);
-        this._wrapped = obj;
-    };
-
-    // Export the Underscore object for **Node.js**, with
-    // backwards-compatibility for the old `require()` API. If we're in
-    // the browser, add `_` as a global object.
-    if (typeof exports !== 'undefined') {
-        if (typeof module !== 'undefined' && module.exports) {
-            exports = module.exports = _;
-        }
-        exports._ = _;
-    } else {
-        root._ = _;
-    }
-
-    // Current version.
-    _.VERSION = '1.8.3';
-
-    // Internal function that returns an efficient (for current engines) version
-    // of the passed-in callback, to be repeatedly applied in other Underscore
-    // functions.
-    var optimizeCb = function(func, context, argCount) {
-        if (context === void 0) return func;
-        switch (argCount == null ? 3 : argCount) {
-            case 1:
-                return function(value) {
-                    return func.call(context, value);
-                };
-            case 2:
-                return function(value, other) {
-                    return func.call(context, value, other);
-                };
-            case 3:
-                return function(value, index, collection) {
-                    return func.call(context, value, index, collection);
-                };
-            case 4:
-                return function(accumulator, value, index, collection) {
-                    return func.call(context, accumulator, value, index, collection);
-                };
-        }
-        return function() {
-            return func.apply(context, arguments);
-        };
-    };
-
-    // A mostly-internal function to generate callbacks that can be applied
-    // to each element in a collection, returning the desired result — either
-    // identity, an arbitrary callback, a property matcher, or a property accessor.
-    var cb = function(value, context, argCount) {
-        if (value == null) return _.identity;
-        if (_.isFunction(value)) return optimizeCb(value, context, argCount);
-        if (_.isObject(value)) return _.matcher(value);
-        return _.property(value);
-    };
-    _.iteratee = function(value, context) {
-        return cb(value, context, Infinity);
-    };
-
-    // An internal function for creating assigner functions.
-    var createAssigner = function(keysFunc, undefinedOnly) {
-        return function(obj) {
-            var length = arguments.length;
-            if (length < 2 || obj == null) return obj;
-            for (var index = 1; index < length; index++) {
-                var source = arguments[index],
-                    keys = keysFunc(source),
-                    l = keys.length;
-                for (var i = 0; i < l; i++) {
-                    var key = keys[i];
-                    if (!undefinedOnly || obj[key] === void 0) obj[key] = source[key];
-                }
-            }
-            return obj;
-        };
-    };
+        nativeCreate = Object.create,
+        nativeIsView = supportsArrayBuffer && ArrayBuffer.isView;
 
-    // An internal function for creating a new object that inherits from another.
-    var baseCreate = function(prototype) {
-        if (!_.isObject(prototype)) return {};
-        if (nativeCreate) return nativeCreate(prototype);
-        Ctor.prototype = prototype;
-        var result = new Ctor;
-        Ctor.prototype = null;
-        return result;
-    };
+    // Create references to these builtin functions because we override them.
+    var _isNaN = isNaN,
+        _isFinite = isFinite;
 
-    var property = function(key) {
-        return function(obj) {
-            return obj == null ? void 0 : obj[key];
-        };
-    };
+    // Keys in IE < 9 that won't be iterated by `for key in ...` and thus missed.
+    var hasEnumBug = !{
+        toString: null
+    }.propertyIsEnumerable('toString');
+    var nonEnumerableProps = ['valueOf', 'isPrototypeOf', 'toString',
+        'propertyIsEnumerable', 'hasOwnProperty', 'toLocaleString'
+    ];
 
-    // Helper for collection methods to determine whether a collection
-    // should be iterated as an array or as an object
-    // Related: http://people.mozilla.org/~jorendorff/es6-draft.html#sec-tolength
-    // Avoids a very nasty iOS 8 JIT bug on ARM-64. #2094
+    // The largest integer that can be represented exactly.
     var MAX_ARRAY_INDEX = Math.pow(2, 53) - 1;
-    var getLength = property('length');
-    var isArrayLike = function(collection) {
-        var length = getLength(collection);
-        return typeof length == 'number' && length >= 0 && length <= MAX_ARRAY_INDEX;
-    };
-
-    // Collection Functions
-    // --------------------
 
-    // The cornerstone, an `each` implementation, aka `forEach`.
-    // Handles raw objects in addition to array-likes. Treats all
-    // sparse array-likes as if they were dense.
-    _.each = _.forEach = function(obj, iteratee, context) {
-        iteratee = optimizeCb(iteratee, context);
-        var i, length;
-        if (isArrayLike(obj)) {
-            for (i = 0, length = obj.length; i < length; i++) {
-                iteratee(obj[i], i, obj);
-            }
-        } else {
-            var keys = _.keys(obj);
-            for (i = 0, length = keys.length; i < length; i++) {
-                iteratee(obj[keys[i]], keys[i], obj);
-            }
-        }
-        return obj;
-    };
-
-    // Return the results of applying the iteratee to each element.
-    _.map = _.collect = function(obj, iteratee, context) {
-        iteratee = cb(iteratee, context);
-        var keys = !isArrayLike(obj) && _.keys(obj),
-            length = (keys || obj).length,
-            results = Array(length);
-        for (var index = 0; index < length; index++) {
-            var currentKey = keys ? keys[index] : index;
-            results[index] = iteratee(obj[currentKey], currentKey, obj);
-        }
-        return results;
-    };
-
-    // Create a reducing function iterating left or right.
-    function createReduce(dir) {
-        // Optimized iterator function as using arguments.length
-        // in the main function will deoptimize the, see #1991.
-        function iterator(obj, iteratee, memo, keys, index, length) {
-            for (; index >= 0 && index < length; index += dir) {
-                var currentKey = keys ? keys[index] : index;
-                memo = iteratee(memo, obj[currentKey], currentKey, obj);
-            }
-            return memo;
-        }
-
-        return function(obj, iteratee, memo, context) {
-            iteratee = optimizeCb(iteratee, context, 4);
-            var keys = !isArrayLike(obj) && _.keys(obj),
-                length = (keys || obj).length,
-                index = dir > 0 ? 0 : length - 1;
-            // Determine the initial value if none is provided.
-            if (arguments.length < 3) {
-                memo = obj[keys ? keys[index] : index];
-                index += dir;
+    // Some functions take a variable number of arguments, or a few expected
+    // arguments at the beginning and then a variable number of values to operate
+    // on. This helper accumulates all remaining arguments past the function’s
+    // argument length (or an explicit `startIndex`), into an array that becomes
+    // the last argument. Similar to ES6’s "rest parameter".
+    function restArguments(func, startIndex) {
+        startIndex = startIndex == null ? func.length - 1 : +startIndex;
+        return function() {
+            var length = Math.max(arguments.length - startIndex, 0),
+                rest = Array(length),
+                index = 0;
+            for (; index < length; index++) {
+                rest[index] = arguments[index + startIndex];
+            }
+            switch (startIndex) {
+                case 0:
+                    return func.call(this, rest);
+                case 1:
+                    return func.call(this, arguments[0], rest);
+                case 2:
+                    return func.call(this, arguments[0], arguments[1], rest);
+            }
+            var args = Array(startIndex + 1);
+            for (index = 0; index < startIndex; index++) {
+                args[index] = arguments[index];
             }
-            return iterator(obj, iteratee, memo, keys, index, length);
+            args[startIndex] = rest;
+            return func.apply(this, args);
         };
     }
 
-    // **Reduce** builds up a single result from a list of values, aka `inject`,
-    // or `foldl`.
-    _.reduce = _.foldl = _.inject = createReduce(1);
-
-    // The right-associative version of reduce, also known as `foldr`.
-    _.reduceRight = _.foldr = createReduce(-1);
-
-    // Return the first value which passes a truth test. Aliased as `detect`.
-    _.find = _.detect = function(obj, predicate, context) {
-        var key;
-        if (isArrayLike(obj)) {
-            key = _.findIndex(obj, predicate, context);
-        } else {
-            key = _.findKey(obj, predicate, context);
-        }
-        if (key !== void 0 && key !== -1) return obj[key];
-    };
-
-    // Return all the elements that pass a truth test.
-    // Aliased as `select`.
-    _.filter = _.select = function(obj, predicate, context) {
-        var results = [];
-        predicate = cb(predicate, context);
-        _.each(obj, function(value, index, list) {
-            if (predicate(value, index, list)) results.push(value);
-        });
-        return results;
-    };
-
-    // Return all the elements for which a truth test fails.
-    _.reject = function(obj, predicate, context) {
-        return _.filter(obj, _.negate(cb(predicate)), context);
-    };
-
-    // Determine whether all of the elements match a truth test.
-    // Aliased as `all`.
-    _.every = _.all = function(obj, predicate, context) {
-        predicate = cb(predicate, context);
-        var keys = !isArrayLike(obj) && _.keys(obj),
-            length = (keys || obj).length;
-        for (var index = 0; index < length; index++) {
-            var currentKey = keys ? keys[index] : index;
-            if (!predicate(obj[currentKey], currentKey, obj)) return false;
-        }
-        return true;
-    };
-
-    // Determine if at least one element in the object matches a truth test.
-    // Aliased as `any`.
-    _.some = _.any = function(obj, predicate, context) {
-        predicate = cb(predicate, context);
-        var keys = !isArrayLike(obj) && _.keys(obj),
-            length = (keys || obj).length;
-        for (var index = 0; index < length; index++) {
-            var currentKey = keys ? keys[index] : index;
-            if (predicate(obj[currentKey], currentKey, obj)) return true;
-        }
-        return false;
-    };
-
-    // Determine if the array or object contains a given item (using `===`).
-    // Aliased as `includes` and `include`.
-    _.contains = _.includes = _.include = function(obj, item, fromIndex, guard) {
-        if (!isArrayLike(obj)) obj = _.values(obj);
-        if (typeof fromIndex != 'number' || guard) fromIndex = 0;
-        return _.indexOf(obj, item, fromIndex) >= 0;
-    };
-
-    // Invoke a method (with arguments) on every item in a collection.
-    _.invoke = function(obj, method) {
-        var args = slice.call(arguments, 2);
-        var isFunc = _.isFunction(method);
-        return _.map(obj, function(value) {
-            var func = isFunc ? method : value[method];
-            return func == null ? func : func.apply(value, args);
-        });
-    };
-
-    // Convenience version of a common use case of `map`: fetching a property.
-    _.pluck = function(obj, key) {
-        return _.map(obj, _.property(key));
-    };
-
-    // Convenience version of a common use case of `filter`: selecting only objects
-    // containing specific `key:value` pairs.
-    _.where = function(obj, attrs) {
-        return _.filter(obj, _.matcher(attrs));
-    };
-
-    // Convenience version of a common use case of `find`: getting the first object
-    // containing specific `key:value` pairs.
-    _.findWhere = function(obj, attrs) {
-        return _.find(obj, _.matcher(attrs));
-    };
-
-    // Return the maximum element (or element-based computation).
-    _.max = function(obj, iteratee, context) {
-        var result = -Infinity,
-            lastComputed = -Infinity,
-            value, computed;
-        if (iteratee == null && obj != null) {
-            obj = isArrayLike(obj) ? obj : _.values(obj);
-            for (var i = 0, length = obj.length; i < length; i++) {
-                value = obj[i];
-                if (value > result) {
-                    result = value;
-                }
-            }
-        } else {
-            iteratee = cb(iteratee, context);
-            _.each(obj, function(value, index, list) {
-                computed = iteratee(value, index, list);
-                if (computed > lastComputed || computed === -Infinity && result === -Infinity) {
-                    result = value;
-                    lastComputed = computed;
-                }
-            });
-        }
-        return result;
-    };
+    // Is a given variable an object?
+    function isObject(obj) {
+        var type = typeof obj;
+        return type === 'function' || (type === 'object' && !!obj);
+    }
 
-    // Return the minimum element (or element-based computation).
-    _.min = function(obj, iteratee, context) {
-        var result = Infinity,
-            lastComputed = Infinity,
-            value, computed;
-        if (iteratee == null && obj != null) {
-            obj = isArrayLike(obj) ? obj : _.values(obj);
-            for (var i = 0, length = obj.length; i < length; i++) {
-                value = obj[i];
-                if (value < result) {
-                    result = value;
-                }
-            }
-        } else {
-            iteratee = cb(iteratee, context);
-            _.each(obj, function(value, index, list) {
-                computed = iteratee(value, index, list);
-                if (computed < lastComputed || computed === Infinity && result === Infinity) {
-                    result = value;
-                    lastComputed = computed;
-                }
-            });
-        }
-        return result;
-    };
+    // Is a given value equal to null?
+    function isNull(obj) {
+        return obj === null;
+    }
 
-    // Shuffle a collection, using the modern version of the
-    // [Fisher-Yates shuffle](http://en.wikipedia.org/wiki/Fisher–Yates_shuffle).
-    _.shuffle = function(obj) {
-        var set = isArrayLike(obj) ? obj : _.values(obj);
-        var length = set.length;
-        var shuffled = Array(length);
-        for (var index = 0, rand; index < length; index++) {
-            rand = _.random(0, index);
-            if (rand !== index) shuffled[index] = shuffled[rand];
-            shuffled[rand] = set[index];
-        }
-        return shuffled;
-    };
+    // Is a given variable undefined?
+    function isUndefined(obj) {
+        return obj === void 0;
+    }
 
-    // Sample **n** random values from a collection.
-    // If **n** is not specified, returns a single random element.
-    // The internal `guard` argument allows it to work with `map`.
-    _.sample = function(obj, n, guard) {
-        if (n == null || guard) {
-            if (!isArrayLike(obj)) obj = _.values(obj);
-            return obj[_.random(obj.length - 1)];
-        }
-        return _.shuffle(obj).slice(0, Math.max(0, n));
-    };
+    // Is a given value a boolean?
+    function isBoolean(obj) {
+        return obj === true || obj === false || toString.call(obj) === '[object Boolean]';
+    }
 
-    // Sort the object's values by a criterion produced by an iteratee.
-    _.sortBy = function(obj, iteratee, context) {
-        iteratee = cb(iteratee, context);
-        return _.pluck(_.map(obj, function(value, index, list) {
-            return {
-                value: value,
-                index: index,
-                criteria: iteratee(value, index, list)
-            };
-        }).sort(function(left, right) {
-            var a = left.criteria;
-            var b = right.criteria;
-            if (a !== b) {
-                if (a > b || a === void 0) return 1;
-                if (a < b || b === void 0) return -1;
-            }
-            return left.index - right.index;
-        }), 'value');
-    };
+    // Is a given value a DOM element?
+    function isElement(obj) {
+        return !!(obj && obj.nodeType === 1);
+    }
 
-    // An internal function used for aggregate "group by" operations.
-    var group = function(behavior) {
-        return function(obj, iteratee, context) {
-            var result = {};
-            iteratee = cb(iteratee, context);
-            _.each(obj, function(value, index) {
-                var key = iteratee(value, index, obj);
-                behavior(result, value, key);
-            });
-            return result;
+    // Internal function for creating a `toString`-based type tester.
+    function tagTester(name) {
+        var tag = '[object ' + name + ']';
+        return function(obj) {
+            return toString.call(obj) === tag;
         };
-    };
-
-    // Groups the object's values by a criterion. Pass either a string attribute
-    // to group by, or a function that returns the criterion.
-    _.groupBy = group(function(result, value, key) {
-        if (_.has(result, key)) result[key].push(value);
-        else result[key] = [value];
-    });
-
-    // Indexes the object's values by a criterion, similar to `groupBy`, but for
-    // when you know that your index values will be unique.
-    _.indexBy = group(function(result, value, key) {
-        result[key] = value;
-    });
-
-    // Counts instances of an object that group by a certain criterion. Pass
-    // either a string attribute to count by, or a function that returns the
-    // criterion.
-    _.countBy = group(function(result, value, key) {
-        if (_.has(result, key)) result[key]++;
-        else result[key] = 1;
-    });
-
-    // Safely create a real, live array from anything iterable.
-    _.toArray = function(obj) {
-        if (!obj) return [];
-        if (_.isArray(obj)) return slice.call(obj);
-        if (isArrayLike(obj)) return _.map(obj, _.identity);
-        return _.values(obj);
-    };
-
-    // Return the number of elements in an object.
-    _.size = function(obj) {
-        if (obj == null) return 0;
-        return isArrayLike(obj) ? obj.length : _.keys(obj).length;
-    };
-
-    // Split a collection into two arrays: one whose elements all satisfy the given
-    // predicate, and one whose elements all do not satisfy the predicate.
-    _.partition = function(obj, predicate, context) {
-        predicate = cb(predicate, context);
-        var pass = [],
-            fail = [];
-        _.each(obj, function(value, key, obj) {
-            (predicate(value, key, obj) ? pass : fail).push(value);
-        });
-        return [pass, fail];
-    };
-
-    // Array Functions
-    // ---------------
-
-    // Get the first element of an array. Passing **n** will return the first N
-    // values in the array. Aliased as `head` and `take`. The **guard** check
-    // allows it to work with `_.map`.
-    _.first = _.head = _.take = function(array, n, guard) {
-        if (array == null) return void 0;
-        if (n == null || guard) return array[0];
-        return _.initial(array, array.length - n);
-    };
-
-    // Returns everything but the last entry of the array. Especially useful on
-    // the arguments object. Passing **n** will return all the values in
-    // the array, excluding the last N.
-    _.initial = function(array, n, guard) {
-        return slice.call(array, 0, Math.max(0, array.length - (n == null || guard ? 1 : n)));
-    };
-
-    // Get the last element of an array. Passing **n** will return the last N
-    // values in the array.
-    _.last = function(array, n, guard) {
-        if (array == null) return void 0;
-        if (n == null || guard) return array[array.length - 1];
-        return _.rest(array, Math.max(0, array.length - n));
-    };
+    }
 
-    // Returns everything but the first entry of the array. Aliased as `tail` and `drop`.
-    // Especially useful on the arguments object. Passing an **n** will return
-    // the rest N values in the array.
-    _.rest = _.tail = _.drop = function(array, n, guard) {
-        return slice.call(array, n == null || guard ? 1 : n);
-    };
+    var isString = tagTester('String');
 
-    // Trim out all falsy values from an array.
-    _.compact = function(array) {
-        return _.filter(array, _.identity);
-    };
+    var isNumber = tagTester('Number');
 
-    // Internal implementation of a recursive `flatten` function.
-    var flatten = function(input, shallow, strict, startIndex) {
-        var output = [],
-            idx = 0;
-        for (var i = startIndex || 0, length = getLength(input); i < length; i++) {
-            var value = input[i];
-            if (isArrayLike(value) && (_.isArray(value) || _.isArguments(value))) {
-                //flatten current level of array or arguments object
-                if (!shallow) value = flatten(value, shallow, strict);
-                var j = 0,
-                    len = value.length;
-                output.length += len;
-                while (j < len) {
-                    output[idx++] = value[j++];
-                }
-            } else if (!strict) {
-                output[idx++] = value;
-            }
-        }
-        return output;
-    };
+    var isDate = tagTester('Date');
 
-    // Flatten out an array, either recursively (by default), or just one level.
-    _.flatten = function(array, shallow) {
-        return flatten(array, shallow, false);
-    };
+    var isRegExp = tagTester('RegExp');
 
-    // Return a version of the array that does not contain the specified value(s).
-    _.without = function(array) {
-        return _.difference(array, slice.call(arguments, 1));
-    };
+    var isError = tagTester('Error');
 
-    // Produce a duplicate-free version of the array. If the array has already
-    // been sorted, you have the option of using a faster algorithm.
-    // Aliased as `unique`.
-    _.uniq = _.unique = function(array, isSorted, iteratee, context) {
-        if (!_.isBoolean(isSorted)) {
-            context = iteratee;
-            iteratee = isSorted;
-            isSorted = false;
-        }
-        if (iteratee != null) iteratee = cb(iteratee, context);
-        var result = [];
-        var seen = [];
-        for (var i = 0, length = getLength(array); i < length; i++) {
-            var value = array[i],
-                computed = iteratee ? iteratee(value, i, array) : value;
-            if (isSorted) {
-                if (!i || seen !== computed) result.push(value);
-                seen = computed;
-            } else if (iteratee) {
-                if (!_.contains(seen, computed)) {
-                    seen.push(computed);
-                    result.push(value);
-                }
-            } else if (!_.contains(result, value)) {
-                result.push(value);
-            }
-        }
-        return result;
-    };
+    var isSymbol = tagTester('Symbol');
 
-    // Produce an array that contains the union: each distinct element from all of
-    // the passed-in arrays.
-    _.union = function() {
-        return _.uniq(flatten(arguments, true, true));
-    };
+    var isArrayBuffer = tagTester('ArrayBuffer');
 
-    // Produce an array that contains every item shared between all the
-    // passed-in arrays.
-    _.intersection = function(array) {
-        var result = [];
-        var argsLength = arguments.length;
-        for (var i = 0, length = getLength(array); i < length; i++) {
-            var item = array[i];
-            if (_.contains(result, item)) continue;
-            for (var j = 1; j < argsLength; j++) {
-                if (!_.contains(arguments[j], item)) break;
-            }
-            if (j === argsLength) result.push(item);
-        }
-        return result;
-    };
-
-    // Take the difference between one array and a number of other arrays.
-    // Only the elements present in just the first array will remain.
-    _.difference = function(array) {
-        var rest = flatten(arguments, true, true, 1);
-        return _.filter(array, function(value) {
-            return !_.contains(rest, value);
-        });
-    };
-
-    // Zip together multiple lists into a single array -- elements that share
-    // an index go together.
-    _.zip = function() {
-        return _.unzip(arguments);
-    };
-
-    // Complement of _.zip. Unzip accepts an array of arrays and groups
-    // each array's elements on shared indices
-    _.unzip = function(array) {
-        var length = array && _.max(array, getLength).length || 0;
-        var result = Array(length);
-
-        for (var index = 0; index < length; index++) {
-            result[index] = _.pluck(array, index);
-        }
-        return result;
-    };
+    var isFunction = tagTester('Function');
 
-    // Converts lists into objects. Pass either a single array of `[key, value]`
-    // pairs, or two parallel arrays of the same length -- one of keys, and one of
-    // the corresponding values.
-    _.object = function(list, values) {
-        var result = {};
-        for (var i = 0, length = getLength(list); i < length; i++) {
-            if (values) {
-                result[list[i]] = values[i];
-            } else {
-                result[list[i][0]] = list[i][1];
-            }
-        }
-        return result;
-    };
-
-    // Generator function to create the findIndex and findLastIndex functions
-    function createPredicateIndexFinder(dir) {
-        return function(array, predicate, context) {
-            predicate = cb(predicate, context);
-            var length = getLength(array);
-            var index = dir > 0 ? 0 : length - 1;
-            for (; index >= 0 && index < length; index += dir) {
-                if (predicate(array[index], index, array)) return index;
-            }
-            return -1;
+    // Optimize `isFunction` if appropriate. Work around some `typeof` bugs in old
+    // v8, IE 11 (#1621), Safari 8 (#1929), and PhantomJS (#2236).
+    var nodelist = root.document && root.document.childNodes;
+    if (typeof /./ != 'function' && typeof Int8Array != 'object' && typeof nodelist != 'function') {
+        isFunction = function(obj) {
+            return typeof obj == 'function' || false;
         };
     }
 
-    // Returns the first index on an array-like that passes a predicate test
-    _.findIndex = createPredicateIndexFinder(1);
-    _.findLastIndex = createPredicateIndexFinder(-1);
+    var isFunction$1 = isFunction;
 
-    // Use a comparator function to figure out the smallest index at which
-    // an object should be inserted so as to maintain order. Uses binary search.
-    _.sortedIndex = function(array, obj, iteratee, context) {
-        iteratee = cb(iteratee, context, 1);
-        var value = iteratee(obj);
-        var low = 0,
-            high = getLength(array);
-        while (low < high) {
-            var mid = Math.floor((low + high) / 2);
-            if (iteratee(array[mid]) < value) low = mid + 1;
-            else high = mid;
-        }
-        return low;
-    };
+    var hasObjectTag = tagTester('Object');
 
-    // Generator function to create the indexOf and lastIndexOf functions
-    function createIndexFinder(dir, predicateFind, sortedIndex) {
-        return function(array, item, idx) {
-            var i = 0,
-                length = getLength(array);
-            if (typeof idx == 'number') {
-                if (dir > 0) {
-                    i = idx >= 0 ? idx : Math.max(idx + length, i);
-                } else {
-                    length = idx >= 0 ? Math.min(idx + 1, length) : idx + length + 1;
-                }
-            } else if (sortedIndex && idx && length) {
-                idx = sortedIndex(array, item);
-                return array[idx] === item ? idx : -1;
-            }
-            if (item !== item) {
-                idx = predicateFind(slice.call(array, i, length), _.isNaN);
-                return idx >= 0 ? idx + i : -1;
-            }
-            for (idx = dir > 0 ? i : length - 1; idx >= 0 && idx < length; idx += dir) {
-                if (array[idx] === item) return idx;
-            }
-            return -1;
-        };
+    // In IE 10 - Edge 13, `DataView` has string tag `'[object Object]'`.
+    // In IE 11, the most common among them, this problem also applies to
+    // `Map`, `WeakMap` and `Set`.
+    var hasStringTagBug = (
+            supportsDataView && hasObjectTag(new DataView(new ArrayBuffer(8)))
+        ),
+        isIE11 = (typeof Map !== 'undefined' && hasObjectTag(new Map));
+
+    var isDataView = tagTester('DataView');
+
+    // In IE 10 - Edge 13, we need a different heuristic
+    // to determine whether an object is a `DataView`.
+    function ie10IsDataView(obj) {
+        return obj != null && isFunction$1(obj.getInt8) && isArrayBuffer(obj.buffer);
     }
 
-    // Return the position of the first occurrence of an item in an array,
-    // or -1 if the item is not included in the array.
-    // If the array is large and already in sort order, pass `true`
-    // for **isSorted** to use binary search.
-    _.indexOf = createIndexFinder(1, _.findIndex, _.sortedIndex);
-    _.lastIndexOf = createIndexFinder(-1, _.findLastIndex);
-
-    // Generate an integer Array containing an arithmetic progression. A port of
-    // the native Python `range()` function. See
-    // [the Python documentation](http://docs.python.org/library/functions.html#range).
-    _.range = function(start, stop, step) {
-        if (stop == null) {
-            stop = start || 0;
-            start = 0;
-        }
-        step = step || 1;
-
-        var length = Math.max(Math.ceil((stop - start) / step), 0);
-        var range = Array(length);
-
-        for (var idx = 0; idx < length; idx++, start += step) {
-            range[idx] = start;
-        }
-
-        return range;
-    };
-
-    // Function (ahem) Functions
-    // ------------------
+    var isDataView$1 = (hasStringTagBug ? ie10IsDataView : isDataView);
 
-    // Determines whether to execute a function as a constructor
-    // or a normal function with the provided arguments
-    var executeBound = function(sourceFunc, boundFunc, context, callingContext, args) {
-        if (!(callingContext instanceof boundFunc)) return sourceFunc.apply(context, args);
-        var self = baseCreate(sourceFunc.prototype);
-        var result = sourceFunc.apply(self, args);
-        if (_.isObject(result)) return result;
-        return self;
-    };
+    // Is a given value an array?
+    // Delegates to ECMA5's native `Array.isArray`.
+    var isArray = nativeIsArray || tagTester('Array');
 
-    // Create a function bound to a given object (assigning `this`, and arguments,
-    // optionally). Delegates to **ECMAScript 5**'s native `Function.bind` if
-    // available.
-    _.bind = function(func, context) {
-        if (nativeBind && func.bind === nativeBind) return nativeBind.apply(func, slice.call(arguments, 1));
-        if (!_.isFunction(func)) throw new TypeError('Bind must be called on a function');
-        var args = slice.call(arguments, 2);
-        var bound = function() {
-            return executeBound(func, bound, context, this, args.concat(slice.call(arguments)));
-        };
-        return bound;
-    };
+    // Internal function to check whether `key` is an own property name of `obj`.
+    function has$1(obj, key) {
+        return obj != null && hasOwnProperty.call(obj, key);
+    }
 
-    // Partially apply a function by creating a version that has had some of its
-    // arguments pre-filled, without changing its dynamic `this` context. _ acts
-    // as a placeholder, allowing any combination of arguments to be pre-filled.
-    _.partial = function(func) {
-        var boundArgs = slice.call(arguments, 1);
-        var bound = function() {
-            var position = 0,
-                length = boundArgs.length;
-            var args = Array(length);
-            for (var i = 0; i < length; i++) {
-                args[i] = boundArgs[i] === _ ? arguments[position++] : boundArgs[i];
-            }
-            while (position < arguments.length) args.push(arguments[position++]);
-            return executeBound(func, bound, this, this, args);
-        };
-        return bound;
-    };
+    var isArguments = tagTester('Arguments');
 
-    // Bind a number of an object's methods to that object. Remaining arguments
-    // are the method names to be bound. Useful for ensuring that all callbacks
-    // defined on an object belong to it.
-    _.bindAll = function(obj) {
-        var i, length = arguments.length,
-            key;
-        if (length <= 1) throw new Error('bindAll must be passed function names');
-        for (i = 1; i < length; i++) {
-            key = arguments[i];
-            obj[key] = _.bind(obj[key], obj);
+    // Define a fallback version of the method in browsers (ahem, IE < 9), where
+    // there isn't any inspectable "Arguments" type.
+    (function() {
+        if (!isArguments(arguments)) {
+            isArguments = function(obj) {
+                return has$1(obj, 'callee');
+            };
         }
-        return obj;
-    };
+    }());
 
-    // Memoize an expensive function by storing its results.
-    _.memoize = function(func, hasher) {
-        var memoize = function(key) {
-            var cache = memoize.cache;
-            var address = '' + (hasher ? hasher.apply(this, arguments) : key);
-            if (!_.has(cache, address)) cache[address] = func.apply(this, arguments);
-            return cache[address];
-        };
-        memoize.cache = {};
-        return memoize;
-    };
+    var isArguments$1 = isArguments;
 
-    // Delays a function for the given number of milliseconds, and then calls
-    // it with the arguments supplied.
-    _.delay = function(func, wait) {
-        var args = slice.call(arguments, 2);
-        return setTimeout(function() {
-            return func.apply(null, args);
-        }, wait);
-    };
+    // Is a given object a finite number?
+    function isFinite$1(obj) {
+        return !isSymbol(obj) && _isFinite(obj) && !isNaN(parseFloat(obj));
+    }
 
-    // Defers a function, scheduling it to run after the current call stack has
-    // cleared.
-    _.defer = _.partial(_.delay, _, 1);
+    // Is the given value `NaN`?
+    function isNaN$1(obj) {
+        return isNumber(obj) && _isNaN(obj);
+    }
 
-    // Returns a function, that, when invoked, will only be triggered at most once
-    // during a given window of time. Normally, the throttled function will run
-    // as much as it can, without ever going more than once per `wait` duration;
-    // but if you'd like to disable the execution on the leading edge, pass
-    // `{leading: false}`. To disable execution on the trailing edge, ditto.
-    _.throttle = function(func, wait, options) {
-        var context, args, result;
-        var timeout = null;
-        var previous = 0;
-        if (!options) options = {};
-        var later = function() {
-            previous = options.leading === false ? 0 : _.now();
-            timeout = null;
-            result = func.apply(context, args);
-            if (!timeout) context = args = null;
-        };
+    // Predicate-generating function. Often useful outside of Underscore.
+    function constant(value) {
         return function() {
-            var now = _.now();
-            if (!previous && options.leading === false) previous = now;
-            var remaining = wait - (now - previous);
-            context = this;
-            args = arguments;
-            if (remaining <= 0 || remaining > wait) {
-                if (timeout) {
-                    clearTimeout(timeout);
-                    timeout = null;
-                }
-                previous = now;
-                result = func.apply(context, args);
-                if (!timeout) context = args = null;
-            } else if (!timeout && options.trailing !== false) {
-                timeout = setTimeout(later, remaining);
-            }
-            return result;
+            return value;
         };
-    };
-
-    // Returns a function, that, as long as it continues to be invoked, will not
-    // be triggered. The function will be called after it stops being called for
-    // N milliseconds. If `immediate` is passed, trigger the function on the
-    // leading edge, instead of the trailing.
-    _.debounce = function(func, wait, immediate) {
-        var timeout, args, context, timestamp, result;
+    }
 
-        var later = function() {
-            var last = _.now() - timestamp;
+    // Common internal logic for `isArrayLike` and `isBufferLike`.
+    function createSizePropertyCheck(getSizeProperty) {
+        return function(collection) {
+            var sizeProperty = getSizeProperty(collection);
+            return typeof sizeProperty == 'number' && sizeProperty >= 0 && sizeProperty <= MAX_ARRAY_INDEX;
+        }
+    }
 
-            if (last < wait && last >= 0) {
-                timeout = setTimeout(later, wait - last);
-            } else {
-                timeout = null;
-                if (!immediate) {
-                    result = func.apply(context, args);
-                    if (!timeout) context = args = null;
-                }
-            }
+    // Internal helper to generate a function to obtain property `key` from `obj`.
+    function shallowProperty(key) {
+        return function(obj) {
+            return obj == null ? void 0 : obj[key];
         };
+    }
 
-        return function() {
-            context = this;
-            args = arguments;
-            timestamp = _.now();
-            var callNow = immediate && !timeout;
-            if (!timeout) timeout = setTimeout(later, wait);
-            if (callNow) {
-                result = func.apply(context, args);
-                context = args = null;
-            }
-
-            return result;
-        };
-    };
+    // Internal helper to obtain the `byteLength` property of an object.
+    var getByteLength = shallowProperty('byteLength');
 
-    // Returns the first function passed as an argument to the second,
-    // allowing you to adjust arguments, run code before and after, and
-    // conditionally execute the original function.
-    _.wrap = function(func, wrapper) {
-        return _.partial(wrapper, func);
-    };
+    // Internal helper to determine whether we should spend extensive checks against
+    // `ArrayBuffer` et al.
+    var isBufferLike = createSizePropertyCheck(getByteLength);
+
+    // Is a given value a typed array?
+    var typedArrayPattern = /\[object ((I|Ui)nt(8|16|32)|Float(32|64)|Uint8Clamped|Big(I|Ui)nt64)Array\]/;
+
+    function isTypedArray(obj) {
+        // `ArrayBuffer.isView` is the most future-proof, so use it when available.
+        // Otherwise, fall back on the above regular expression.
+        return nativeIsView ? (nativeIsView(obj) && !isDataView$1(obj)) :
+            isBufferLike(obj) && typedArrayPattern.test(toString.call(obj));
+    }
 
-    // Returns a negated version of the passed-in predicate.
-    _.negate = function(predicate) {
-        return function() {
-            return !predicate.apply(this, arguments);
-        };
-    };
+    var isTypedArray$1 = supportsArrayBuffer ? isTypedArray : constant(false);
 
-    // Returns a function that is the composition of a list of functions, each
-    // consuming the return value of the function that follows.
-    _.compose = function() {
-        var args = arguments;
-        var start = args.length - 1;
-        return function() {
-            var i = start;
-            var result = args[start].apply(this, arguments);
-            while (i--) result = args[i].call(this, result);
-            return result;
-        };
-    };
+    // Internal helper to obtain the `length` property of an object.
+    var getLength = shallowProperty('length');
 
-    // Returns a function that will only be executed on and after the Nth call.
-    _.after = function(times, func) {
-        return function() {
-            if (--times < 1) {
-                return func.apply(this, arguments);
+    // Internal helper to create a simple lookup structure.
+    // `collectNonEnumProps` used to depend on `_.contains`, but this led to
+    // circular imports. `emulatedSet` is a one-off solution that only works for
+    // arrays of strings.
+    function emulatedSet(keys) {
+        var hash = {};
+        for (var l = keys.length, i = 0; i < l; ++i) hash[keys[i]] = true;
+        return {
+            contains: function(key) {
+                return hash[key] === true;
+            },
+            push: function(key) {
+                hash[key] = true;
+                return keys.push(key);
             }
         };
-    };
-
-    // Returns a function that will only be executed up to (but not including) the Nth call.
-    _.before = function(times, func) {
-        var memo;
-        return function() {
-            if (--times > 0) {
-                memo = func.apply(this, arguments);
-            }
-            if (times <= 1) func = null;
-            return memo;
-        };
-    };
-
-    // Returns a function that will be executed at most one time, no matter how
-    // often you call it. Useful for lazy initialization.
-    _.once = _.partial(_.before, 2);
-
-    // Object Functions
-    // ----------------
-
-    // Keys in IE < 9 that won't be iterated by `for key in ...` and thus missed.
-    var hasEnumBug = !{
-        toString: null
-    }.propertyIsEnumerable('toString');
-    var nonEnumerableProps = ['valueOf', 'isPrototypeOf', 'toString',
-        'propertyIsEnumerable', 'hasOwnProperty', 'toLocaleString'
-    ];
+    }
 
+    // Internal helper. Checks `keys` for the presence of keys in IE < 9 that won't
+    // be iterated by `for key in ...` and thus missed. Extends `keys` in place if
+    // needed.
     function collectNonEnumProps(obj, keys) {
+        keys = emulatedSet(keys);
         var nonEnumIdx = nonEnumerableProps.length;
         var constructor = obj.constructor;
-        var proto = (_.isFunction(constructor) && constructor.prototype) || ObjProto;
+        var proto = (isFunction$1(constructor) && constructor.prototype) || ObjProto;
 
         // Constructor is a special case.
         var prop = 'constructor';
-        if (_.has(obj, prop) && !_.contains(keys, prop)) keys.push(prop);
+        if (has$1(obj, prop) && !keys.contains(prop)) keys.push(prop);
 
         while (nonEnumIdx--) {
             prop = nonEnumerableProps[nonEnumIdx];
-            if (prop in obj && obj[prop] !== proto[prop] && !_.contains(keys, prop)) {
+            if (prop in obj && obj[prop] !== proto[prop] && !keys.contains(prop)) {
                 keys.push(prop);
             }
         }
     }
 
     // Retrieve the names of an object's own properties.
-    // Delegates to **ECMAScript 5**'s native `Object.keys`
-    _.keys = function(obj) {
-        if (!_.isObject(obj)) return [];
+    // Delegates to **ECMAScript 5**'s native `Object.keys`.
+    function keys(obj) {
+        if (!isObject(obj)) return [];
         if (nativeKeys) return nativeKeys(obj);
         var keys = [];
         for (var key in obj)
-            if (_.has(obj, key)) keys.push(key);
+            if (has$1(obj, key)) keys.push(key);
         // Ahem, IE < 9.
         if (hasEnumBug) collectNonEnumProps(obj, keys);
         return keys;
-    };
-
-    // Retrieve all the property names of an object.
-    _.allKeys = function(obj) {
-        if (!_.isObject(obj)) return [];
-        var keys = [];
-        for (var key in obj) keys.push(key);
-        // Ahem, IE < 9.
-        if (hasEnumBug) collectNonEnumProps(obj, keys);
-        return keys;
-    };
-
-    // Retrieve the values of an object's properties.
-    _.values = function(obj) {
-        var keys = _.keys(obj);
-        var length = keys.length;
-        var values = Array(length);
-        for (var i = 0; i < length; i++) {
-            values[i] = obj[keys[i]];
-        }
-        return values;
-    };
+    }
 
-    // Returns the results of applying the iteratee to each element of the object
-    // In contrast to _.map it returns an object
-    _.mapObject = function(obj, iteratee, context) {
-        iteratee = cb(iteratee, context);
-        var keys = _.keys(obj),
-            length = keys.length,
-            results = {},
-            currentKey;
-        for (var index = 0; index < length; index++) {
-            currentKey = keys[index];
-            results[currentKey] = iteratee(obj[currentKey], currentKey, obj);
-        }
-        return results;
-    };
+    // Is a given array, string, or object empty?
+    // An "empty" object has no enumerable own-properties.
+    function isEmpty(obj) {
+        if (obj == null) return true;
+        // Skip the more expensive `toString`-based type checks if `obj` has no
+        // `.length`.
+        var length = getLength(obj);
+        if (typeof length == 'number' && (
+                isArray(obj) || isString(obj) || isArguments$1(obj)
+            )) return length === 0;
+        return getLength(keys(obj)) === 0;
+    }
 
-    // Convert an object into a list of `[key, value]` pairs.
-    _.pairs = function(obj) {
-        var keys = _.keys(obj);
-        var length = keys.length;
-        var pairs = Array(length);
+    // Returns whether an object has a given set of `key:value` pairs.
+    function isMatch(object, attrs) {
+        var _keys = keys(attrs),
+            length = _keys.length;
+        if (object == null) return !length;
+        var obj = Object(object);
         for (var i = 0; i < length; i++) {
-            pairs[i] = [keys[i], obj[keys[i]]];
-        }
-        return pairs;
-    };
-
-    // Invert the keys and values of an object. The values must be serializable.
-    _.invert = function(obj) {
-        var result = {};
-        var keys = _.keys(obj);
-        for (var i = 0, length = keys.length; i < length; i++) {
-            result[obj[keys[i]]] = keys[i];
-        }
-        return result;
-    };
-
-    // Return a sorted list of the function names available on the object.
-    // Aliased as `methods`
-    _.functions = _.methods = function(obj) {
-        var names = [];
-        for (var key in obj) {
-            if (_.isFunction(obj[key])) names.push(key);
-        }
-        return names.sort();
-    };
-
-    // Extend a given object with all the properties in passed-in object(s).
-    _.extend = createAssigner(_.allKeys);
-
-    // Assigns a given object with all the own properties in the passed-in object(s)
-    // (https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object/assign)
-    _.extendOwn = _.assign = createAssigner(_.keys);
-
-    // Returns the first key on an object that passes a predicate test
-    _.findKey = function(obj, predicate, context) {
-        predicate = cb(predicate, context);
-        var keys = _.keys(obj),
-            key;
-        for (var i = 0, length = keys.length; i < length; i++) {
-            key = keys[i];
-            if (predicate(obj[key], key, obj)) return key;
-        }
-    };
-
-    // Return a copy of the object only containing the whitelisted properties.
-    _.pick = function(object, oiteratee, context) {
-        var result = {},
-            obj = object,
-            iteratee, keys;
-        if (obj == null) return result;
-        if (_.isFunction(oiteratee)) {
-            keys = _.allKeys(obj);
-            iteratee = optimizeCb(oiteratee, context);
-        } else {
-            keys = flatten(arguments, false, false, 1);
-            iteratee = function(value, key, obj) {
-                return key in obj;
-            };
-            obj = Object(obj);
-        }
-        for (var i = 0, length = keys.length; i < length; i++) {
-            var key = keys[i];
-            var value = obj[key];
-            if (iteratee(value, key, obj)) result[key] = value;
+            var key = _keys[i];
+            if (attrs[key] !== obj[key] || !(key in obj)) return false;
         }
-        return result;
-    };
+        return true;
+    }
 
-    // Return a copy of the object without the blacklisted properties.
-    _.omit = function(obj, iteratee, context) {
-        if (_.isFunction(iteratee)) {
-            iteratee = _.negate(iteratee);
-        } else {
-            var keys = _.map(flatten(arguments, false, false, 1), String);
-            iteratee = function(value, key) {
-                return !_.contains(keys, key);
-            };
-        }
-        return _.pick(obj, iteratee, context);
-    };
+    // If Underscore is called as a function, it returns a wrapped object that can
+    // be used OO-style. This wrapper holds altered versions of all functions added
+    // through `_.mixin`. Wrapped objects may be chained.
+    function _$1(obj) {
+        if (obj instanceof _$1) return obj;
+        if (!(this instanceof _$1)) return new _$1(obj);
+        this._wrapped = obj;
+    }
 
-    // Fill in a given object with default properties.
-    _.defaults = createAssigner(_.allKeys, true);
+    _$1.VERSION = VERSION;
 
-    // Creates an object that inherits from the given prototype object.
-    // If additional properties are provided then they will be added to the
-    // created object.
-    _.create = function(prototype, props) {
-        var result = baseCreate(prototype);
-        if (props) _.extendOwn(result, props);
-        return result;
+    // Extracts the result from a wrapped and chained object.
+    _$1.prototype.value = function() {
+        return this._wrapped;
     };
 
-    // Create a (shallow-cloned) duplicate of an object.
-    _.clone = function(obj) {
-        if (!_.isObject(obj)) return obj;
-        return _.isArray(obj) ? obj.slice() : _.extend({}, obj);
-    };
+    // Provide unwrapping proxies for some methods used in engine operations
+    // such as arithmetic and JSON stringification.
+    _$1.prototype.valueOf = _$1.prototype.toJSON = _$1.prototype.value;
 
-    // Invokes interceptor with the obj, and then returns obj.
-    // The primary purpose of this method is to "tap into" a method chain, in
-    // order to perform operations on intermediate results within the chain.
-    _.tap = function(obj, interceptor) {
-        interceptor(obj);
-        return obj;
+    _$1.prototype.toString = function() {
+        return String(this._wrapped);
     };
 
-    // Returns whether an object has a given set of `key:value` pairs.
-    _.isMatch = function(object, attrs) {
-        var keys = _.keys(attrs),
-            length = keys.length;
-        if (object == null) return !length;
-        var obj = Object(object);
-        for (var i = 0; i < length; i++) {
-            var key = keys[i];
-            if (attrs[key] !== obj[key] || !(key in obj)) return false;
-        }
-        return true;
-    };
+    // Internal function to wrap or shallow-copy an ArrayBuffer,
+    // typed array or DataView to a new view, reusing the buffer.
+    function toBufferView(bufferSource) {
+        return new Uint8Array(
+            bufferSource.buffer || bufferSource,
+            bufferSource.byteOffset || 0,
+            getByteLength(bufferSource)
+        );
+    }
 
+    // We use this string twice, so give it a name for minification.
+    var tagDataView = '[object DataView]';
 
-    // Internal recursive comparison function for `isEqual`.
-    var eq = function(a, b, aStack, bStack) {
+    // Internal recursive comparison function for `_.isEqual`.
+    function eq(a, b, aStack, bStack) {
         // Identical objects are equal. `0 === -0`, but they aren't identical.
-        // See the [Harmony `egal` proposal](http://wiki.ecmascript.org/doku.php?id=harmony:egal).
+        // See the [Harmony `egal` proposal](https://wiki.ecmascript.org/doku.php?id=harmony:egal).
         if (a === b) return a !== 0 || 1 / a === 1 / b;
-        // A strict comparison is necessary because `null == undefined`.
-        if (a == null || b == null) return a === b;
+        // `null` or `undefined` only equal to itself (strict comparison).
+        if (a == null || b == null) return false;
+        // `NaN`s are equivalent, but non-reflexive.
+        if (a !== a) return b !== b;
+        // Exhaust primitive checks
+        var type = typeof a;
+        if (type !== 'function' && type !== 'object' && typeof b != 'object') return false;
+        return deepEq(a, b, aStack, bStack);
+    }
+
+    // Internal recursive comparison function for `_.isEqual`.
+    function deepEq(a, b, aStack, bStack) {
         // Unwrap any wrapped objects.
-        if (a instanceof _) a = a._wrapped;
-        if (b instanceof _) b = b._wrapped;
+        if (a instanceof _$1) a = a._wrapped;
+        if (b instanceof _$1) b = b._wrapped;
         // Compare `[[Class]]` names.
         var className = toString.call(a);
         if (className !== toString.call(b)) return false;
+        // Work around a bug in IE 10 - Edge 13.
+        if (hasStringTagBug && className == '[object Object]' && isDataView$1(a)) {
+            if (!isDataView$1(b)) return false;
+            className = tagDataView;
+        }
         switch (className) {
-            // Strings, numbers, regular expressions, dates, and booleans are compared by value.
+            // These types are compared by value.
             case '[object RegExp]':
                 // RegExps are coerced to strings for comparison (Note: '' + /a/i === '/a/i')
             case '[object String]':
                 // Primitives and their corresponding object wrappers are equivalent; thus, `"5"` is
                 // equivalent to `new String("5")`.
                 return '' + a === '' + b;
             case '[object Number]':
                 // `NaN`s are equivalent, but non-reflexive.
-                // Object(NaN) is equivalent to NaN
+                // Object(NaN) is equivalent to NaN.
                 if (+a !== +a) return +b !== +b;
                 // An `egal` comparison is performed for other numeric values.
                 return +a === 0 ? 1 / +a === 1 / b : +a === +b;
             case '[object Date]':
             case '[object Boolean]':
                 // Coerce dates and booleans to numeric primitive values. Dates are compared by their
                 // millisecond representations. Note that invalid dates with millisecond representations
                 // of `NaN` are not equivalent.
                 return +a === +b;
+            case '[object Symbol]':
+                return SymbolProto.valueOf.call(a) === SymbolProto.valueOf.call(b);
+            case '[object ArrayBuffer]':
+            case tagDataView:
+                // Coerce to typed array so we can fall through.
+                return deepEq(toBufferView(a), toBufferView(b), aStack, bStack);
         }
 
         var areArrays = className === '[object Array]';
+        if (!areArrays && isTypedArray$1(a)) {
+            var byteLength = getByteLength(a);
+            if (byteLength !== getByteLength(b)) return false;
+            if (a.buffer === b.buffer && a.byteOffset === b.byteOffset) return true;
+            areArrays = true;
+        }
         if (!areArrays) {
             if (typeof a != 'object' || typeof b != 'object') return false;
 
             // Objects with different constructors are not equivalent, but `Object`s or `Array`s
             // from different frames are.
             var aCtor = a.constructor,
                 bCtor = b.constructor;
-            if (aCtor !== bCtor && !(_.isFunction(aCtor) && aCtor instanceof aCtor &&
-                    _.isFunction(bCtor) && bCtor instanceof bCtor) &&
+            if (aCtor !== bCtor && !(isFunction$1(aCtor) && aCtor instanceof aCtor &&
+                    isFunction$1(bCtor) && bCtor instanceof bCtor) &&
                 ('constructor' in a && 'constructor' in b)) {
                 return false;
             }
         }
         // Assume equality for cyclic structures. The algorithm for detecting cyclic
         // structures is adapted from ES 5.1 section 15.12.3, abstract operation `JO`.
 
@@ -1193,234 +467,409 @@
             if (length !== b.length) return false;
             // Deep compare the contents, ignoring non-numeric properties.
             while (length--) {
                 if (!eq(a[length], b[length], aStack, bStack)) return false;
             }
         } else {
             // Deep compare objects.
-            var keys = _.keys(a),
+            var _keys = keys(a),
                 key;
-            length = keys.length;
+            length = _keys.length;
             // Ensure that both objects contain the same number of properties before comparing deep equality.
-            if (_.keys(b).length !== length) return false;
+            if (keys(b).length !== length) return false;
             while (length--) {
                 // Deep compare each member
-                key = keys[length];
-                if (!(_.has(b, key) && eq(a[key], b[key], aStack, bStack))) return false;
+                key = _keys[length];
+                if (!(has$1(b, key) && eq(a[key], b[key], aStack, bStack))) return false;
             }
         }
         // Remove the first object from the stack of traversed objects.
         aStack.pop();
         bStack.pop();
         return true;
-    };
+    }
 
     // Perform a deep comparison to check if two objects are equal.
-    _.isEqual = function(a, b) {
+    function isEqual(a, b) {
         return eq(a, b);
-    };
+    }
 
-    // Is a given array, string, or object empty?
-    // An "empty" object has no enumerable own-properties.
-    _.isEmpty = function(obj) {
-        if (obj == null) return true;
-        if (isArrayLike(obj) && (_.isArray(obj) || _.isString(obj) || _.isArguments(obj))) return obj.length === 0;
-        return _.keys(obj).length === 0;
-    };
+    // Retrieve all the enumerable property names of an object.
+    function allKeys(obj) {
+        if (!isObject(obj)) return [];
+        var keys = [];
+        for (var key in obj) keys.push(key);
+        // Ahem, IE < 9.
+        if (hasEnumBug) collectNonEnumProps(obj, keys);
+        return keys;
+    }
 
-    // Is a given value a DOM element?
-    _.isElement = function(obj) {
-        return !!(obj && obj.nodeType === 1);
-    };
+    // Since the regular `Object.prototype.toString` type tests don't work for
+    // some types in IE 11, we use a fingerprinting heuristic instead, based
+    // on the methods. It's not great, but it's the best we got.
+    // The fingerprint method lists are defined below.
+    function ie11fingerprint(methods) {
+        var length = getLength(methods);
+        return function(obj) {
+            if (obj == null) return false;
+            // `Map`, `WeakMap` and `Set` have no enumerable keys.
+            var keys = allKeys(obj);
+            if (getLength(keys)) return false;
+            for (var i = 0; i < length; i++) {
+                if (!isFunction$1(obj[methods[i]])) return false;
+            }
+            // If we are testing against `WeakMap`, we need to ensure that
+            // `obj` doesn't have a `forEach` method in order to distinguish
+            // it from a regular `Map`.
+            return methods !== weakMapMethods || !isFunction$1(obj[forEachName]);
+        };
+    }
 
-    // Is a given value an array?
-    // Delegates to ECMA5's native Array.isArray
-    _.isArray = nativeIsArray || function(obj) {
-        return toString.call(obj) === '[object Array]';
-    };
+    // In the interest of compact minification, we write
+    // each string in the fingerprints only once.
+    var forEachName = 'forEach',
+        hasName = 'has',
+        commonInit = ['clear', 'delete'],
+        mapTail = ['get', hasName, 'set'];
+
+    // `Map`, `WeakMap` and `Set` each have slightly different
+    // combinations of the above sublists.
+    var mapMethods = commonInit.concat(forEachName, mapTail),
+        weakMapMethods = commonInit.concat(mapTail),
+        setMethods = ['add'].concat(commonInit, forEachName, hasName);
 
-    // Is a given variable an object?
-    _.isObject = function(obj) {
-        var type = typeof obj;
-        return type === 'function' || type === 'object' && !!obj;
-    };
+    var isMap = isIE11 ? ie11fingerprint(mapMethods) : tagTester('Map');
 
-    // Add some isType methods: isArguments, isFunction, isString, isNumber, isDate, isRegExp, isError.
-    _.each(['Arguments', 'Function', 'String', 'Number', 'Date', 'RegExp', 'Error'], function(name) {
-        _['is' + name] = function(obj) {
-            return toString.call(obj) === '[object ' + name + ']';
-        };
-    });
+    var isWeakMap = isIE11 ? ie11fingerprint(weakMapMethods) : tagTester('WeakMap');
 
-    // Define a fallback version of the method in browsers (ahem, IE < 9), where
-    // there isn't any inspectable "Arguments" type.
-    if (!_.isArguments(arguments)) {
-        _.isArguments = function(obj) {
-            return _.has(obj, 'callee');
-        };
+    var isSet = isIE11 ? ie11fingerprint(setMethods) : tagTester('Set');
+
+    var isWeakSet = tagTester('WeakSet');
+
+    // Retrieve the values of an object's properties.
+    function values(obj) {
+        var _keys = keys(obj);
+        var length = _keys.length;
+        var values = Array(length);
+        for (var i = 0; i < length; i++) {
+            values[i] = obj[_keys[i]];
+        }
+        return values;
     }
 
-    // Optimize `isFunction` if appropriate. Work around some typeof bugs in old v8,
-    // IE 11 (#1621), and in Safari 8 (#1929).
-    if (typeof /./ != 'function' && typeof Int8Array != 'object') {
-        _.isFunction = function(obj) {
-            return typeof obj == 'function' || false;
+    // Convert an object into a list of `[key, value]` pairs.
+    // The opposite of `_.object` with one argument.
+    function pairs(obj) {
+        var _keys = keys(obj);
+        var length = _keys.length;
+        var pairs = Array(length);
+        for (var i = 0; i < length; i++) {
+            pairs[i] = [_keys[i], obj[_keys[i]]];
+        }
+        return pairs;
+    }
+
+    // Invert the keys and values of an object. The values must be serializable.
+    function invert(obj) {
+        var result = {};
+        var _keys = keys(obj);
+        for (var i = 0, length = _keys.length; i < length; i++) {
+            result[obj[_keys[i]]] = _keys[i];
+        }
+        return result;
+    }
+
+    // Return a sorted list of the function names available on the object.
+    function functions(obj) {
+        var names = [];
+        for (var key in obj) {
+            if (isFunction$1(obj[key])) names.push(key);
+        }
+        return names.sort();
+    }
+
+    // An internal function for creating assigner functions.
+    function createAssigner(keysFunc, defaults) {
+        return function(obj) {
+            var length = arguments.length;
+            if (defaults) obj = Object(obj);
+            if (length < 2 || obj == null) return obj;
+            for (var index = 1; index < length; index++) {
+                var source = arguments[index],
+                    keys = keysFunc(source),
+                    l = keys.length;
+                for (var i = 0; i < l; i++) {
+                    var key = keys[i];
+                    if (!defaults || obj[key] === void 0) obj[key] = source[key];
+                }
+            }
+            return obj;
         };
     }
 
-    // Is a given object a finite number?
-    _.isFinite = function(obj) {
-        return isFinite(obj) && !isNaN(parseFloat(obj));
-    };
+    // Extend a given object with all the properties in passed-in object(s).
+    var extend = createAssigner(allKeys);
 
-    // Is the given value `NaN`? (NaN is the only number which does not equal itself).
-    _.isNaN = function(obj) {
-        return _.isNumber(obj) && obj !== +obj;
-    };
+    // Assigns a given object with all the own properties in the passed-in
+    // object(s).
+    // (https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object/assign)
+    var extendOwn = createAssigner(keys);
 
-    // Is a given value a boolean?
-    _.isBoolean = function(obj) {
-        return obj === true || obj === false || toString.call(obj) === '[object Boolean]';
-    };
+    // Fill in a given object with default properties.
+    var defaults = createAssigner(allKeys, true);
 
-    // Is a given value equal to null?
-    _.isNull = function(obj) {
-        return obj === null;
-    };
+    // Create a naked function reference for surrogate-prototype-swapping.
+    function ctor() {
+        return function() {};
+    }
 
-    // Is a given variable undefined?
-    _.isUndefined = function(obj) {
-        return obj === void 0;
-    };
+    // An internal function for creating a new object that inherits from another.
+    function baseCreate(prototype) {
+        if (!isObject(prototype)) return {};
+        if (nativeCreate) return nativeCreate(prototype);
+        var Ctor = ctor();
+        Ctor.prototype = prototype;
+        var result = new Ctor;
+        Ctor.prototype = null;
+        return result;
+    }
 
-    // Shortcut function for checking if an object has a given property directly
-    // on itself (in other words, not on a prototype).
-    _.has = function(obj, key) {
-        return obj != null && hasOwnProperty.call(obj, key);
-    };
+    // Creates an object that inherits from the given prototype object.
+    // If additional properties are provided then they will be added to the
+    // created object.
+    function create(prototype, props) {
+        var result = baseCreate(prototype);
+        if (props) extendOwn(result, props);
+        return result;
+    }
 
-    // Utility Functions
-    // -----------------
+    // Create a (shallow-cloned) duplicate of an object.
+    function clone(obj) {
+        if (!isObject(obj)) return obj;
+        return isArray(obj) ? obj.slice() : extend({}, obj);
+    }
 
-    // Run Underscore.js in *noConflict* mode, returning the `_` variable to its
-    // previous owner. Returns a reference to the Underscore object.
-    _.noConflict = function() {
-        root._ = previousUnderscore;
-        return this;
-    };
+    // Invokes `interceptor` with the `obj` and then returns `obj`.
+    // The primary purpose of this method is to "tap into" a method chain, in
+    // order to perform operations on intermediate results within the chain.
+    function tap(obj, interceptor) {
+        interceptor(obj);
+        return obj;
+    }
+
+    // Normalize a (deep) property `path` to array.
+    // Like `_.iteratee`, this function can be customized.
+    function toPath$1(path) {
+        return isArray(path) ? path : [path];
+    }
+    _$1.toPath = toPath$1;
+
+    // Internal wrapper for `_.toPath` to enable minification.
+    // Similar to `cb` for `_.iteratee`.
+    function toPath(path) {
+        return _$1.toPath(path);
+    }
+
+    // Internal function to obtain a nested property in `obj` along `path`.
+    function deepGet(obj, path) {
+        var length = path.length;
+        for (var i = 0; i < length; i++) {
+            if (obj == null) return void 0;
+            obj = obj[path[i]];
+        }
+        return length ? obj : void 0;
+    }
+
+    // Get the value of the (deep) property on `path` from `object`.
+    // If any property in `path` does not exist or if the value is
+    // `undefined`, return `defaultValue` instead.
+    // The `path` is normalized through `_.toPath`.
+    function get(object, path, defaultValue) {
+        var value = deepGet(object, toPath(path));
+        return isUndefined(value) ? defaultValue : value;
+    }
+
+    // Shortcut function for checking if an object has a given property directly on
+    // itself (in other words, not on a prototype). Unlike the internal `has`
+    // function, this public version can also traverse nested properties.
+    function has(obj, path) {
+        path = toPath(path);
+        var length = path.length;
+        for (var i = 0; i < length; i++) {
+            var key = path[i];
+            if (!has$1(obj, key)) return false;
+            obj = obj[key];
+        }
+        return !!length;
+    }
 
     // Keep the identity function around for default iteratees.
-    _.identity = function(value) {
+    function identity(value) {
         return value;
-    };
+    }
+
+    // Returns a predicate for checking whether an object has a given set of
+    // `key:value` pairs.
+    function matcher(attrs) {
+        attrs = extendOwn({}, attrs);
+        return function(obj) {
+            return isMatch(obj, attrs);
+        };
+    }
 
-    // Predicate-generating functions. Often useful outside of Underscore.
-    _.constant = function(value) {
+    // Creates a function that, when passed an object, will traverse that object’s
+    // properties down the given `path`, specified as an array of keys or indices.
+    function property(path) {
+        path = toPath(path);
+        return function(obj) {
+            return deepGet(obj, path);
+        };
+    }
+
+    // Internal function that returns an efficient (for current engines) version
+    // of the passed-in callback, to be repeatedly applied in other Underscore
+    // functions.
+    function optimizeCb(func, context, argCount) {
+        if (context === void 0) return func;
+        switch (argCount == null ? 3 : argCount) {
+            case 1:
+                return function(value) {
+                    return func.call(context, value);
+                };
+                // The 2-argument case is omitted because we’re not using it.
+            case 3:
+                return function(value, index, collection) {
+                    return func.call(context, value, index, collection);
+                };
+            case 4:
+                return function(accumulator, value, index, collection) {
+                    return func.call(context, accumulator, value, index, collection);
+                };
+        }
         return function() {
-            return value;
+            return func.apply(context, arguments);
         };
-    };
+    }
 
-    _.noop = function() {};
+    // An internal function to generate callbacks that can be applied to each
+    // element in a collection, returning the desired result — either `_.identity`,
+    // an arbitrary callback, a property matcher, or a property accessor.
+    function baseIteratee(value, context, argCount) {
+        if (value == null) return identity;
+        if (isFunction$1(value)) return optimizeCb(value, context, argCount);
+        if (isObject(value) && !isArray(value)) return matcher(value);
+        return property(value);
+    }
 
-    _.property = property;
+    // External wrapper for our callback generator. Users may customize
+    // `_.iteratee` if they want additional predicate/iteratee shorthand styles.
+    // This abstraction hides the internal-only `argCount` argument.
+    function iteratee(value, context) {
+        return baseIteratee(value, context, Infinity);
+    }
+    _$1.iteratee = iteratee;
 
-    // Generates a function for a given object that returns a given property.
-    _.propertyOf = function(obj) {
-        return obj == null ? function() {} : function(key) {
-            return obj[key];
-        };
-    };
+    // The function we call internally to generate a callback. It invokes
+    // `_.iteratee` if overridden, otherwise `baseIteratee`.
+    function cb(value, context, argCount) {
+        if (_$1.iteratee !== iteratee) return _$1.iteratee(value, context);
+        return baseIteratee(value, context, argCount);
+    }
 
-    // Returns a predicate for checking whether an object has a given set of
-    // `key:value` pairs.
-    _.matcher = _.matches = function(attrs) {
-        attrs = _.extendOwn({}, attrs);
-        return function(obj) {
-            return _.isMatch(obj, attrs);
+    // Returns the results of applying the `iteratee` to each element of `obj`.
+    // In contrast to `_.map` it returns an object.
+    function mapObject(obj, iteratee, context) {
+        iteratee = cb(iteratee, context);
+        var _keys = keys(obj),
+            length = _keys.length,
+            results = {};
+        for (var index = 0; index < length; index++) {
+            var currentKey = _keys[index];
+            results[currentKey] = iteratee(obj[currentKey], currentKey, obj);
+        }
+        return results;
+    }
+
+    // Predicate-generating function. Often useful outside of Underscore.
+    function noop() {}
+
+    // Generates a function for a given object that returns a given property.
+    function propertyOf(obj) {
+        if (obj == null) return noop;
+        return function(path) {
+            return get(obj, path);
         };
-    };
+    }
 
     // Run a function **n** times.
-    _.times = function(n, iteratee, context) {
+    function times(n, iteratee, context) {
         var accum = Array(Math.max(0, n));
         iteratee = optimizeCb(iteratee, context, 1);
         for (var i = 0; i < n; i++) accum[i] = iteratee(i);
         return accum;
-    };
+    }
 
-    // Return a random integer between min and max (inclusive).
-    _.random = function(min, max) {
+    // Return a random integer between `min` and `max` (inclusive).
+    function random(min, max) {
         if (max == null) {
             max = min;
             min = 0;
         }
         return min + Math.floor(Math.random() * (max - min + 1));
-    };
+    }
 
     // A (possibly faster) way to get the current timestamp as an integer.
-    _.now = Date.now || function() {
+    var now = Date.now || function() {
         return new Date().getTime();
     };
 
-    // List of HTML entities for escaping.
-    var escapeMap = {
-        '&': '&amp;',
-        '<': '&lt;',
-        '>': '&gt;',
-        '"': '&quot;',
-        "'": '&#x27;',
-        '`': '&#x60;'
-    };
-    var unescapeMap = _.invert(escapeMap);
-
-    // Functions for escaping and unescaping strings to/from HTML interpolation.
-    var createEscaper = function(map) {
+    // Internal helper to generate functions for escaping and unescaping strings
+    // to/from HTML interpolation.
+    function createEscaper(map) {
         var escaper = function(match) {
             return map[match];
         };
-        // Regexes for identifying a key that needs to be escaped
-        var source = '(?:' + _.keys(map).join('|') + ')';
+        // Regexes for identifying a key that needs to be escaped.
+        var source = '(?:' + keys(map).join('|') + ')';
         var testRegexp = RegExp(source);
         var replaceRegexp = RegExp(source, 'g');
         return function(string) {
             string = string == null ? '' : '' + string;
             return testRegexp.test(string) ? string.replace(replaceRegexp, escaper) : string;
         };
-    };
-    _.escape = createEscaper(escapeMap);
-    _.unescape = createEscaper(unescapeMap);
+    }
 
-    // If the value of the named `property` is a function then invoke it with the
-    // `object` as context; otherwise, return it.
-    _.result = function(object, property, fallback) {
-        var value = object == null ? void 0 : object[property];
-        if (value === void 0) {
-            value = fallback;
-        }
-        return _.isFunction(value) ? value.call(object) : value;
+    // Internal list of HTML entities for escaping.
+    var escapeMap = {
+        '&': '&amp;',
+        '<': '&lt;',
+        '>': '&gt;',
+        '"': '&quot;',
+        "'": '&#x27;',
+        '`': '&#x60;'
     };
 
-    // Generate a unique integer id (unique within the entire client session).
-    // Useful for temporary DOM ids.
-    var idCounter = 0;
-    _.uniqueId = function(prefix) {
-        var id = ++idCounter + '';
-        return prefix ? prefix + id : id;
-    };
+    // Function for escaping strings to HTML interpolation.
+    var _escape = createEscaper(escapeMap);
+
+    // Internal list of HTML entities for unescaping.
+    var unescapeMap = invert(escapeMap);
 
-    // By default, Underscore uses ERB-style template delimiters, change the
+    // Function for unescaping strings from HTML interpolation.
+    var _unescape = createEscaper(unescapeMap);
+
+    // By default, Underscore uses ERB-style template delimiters. Change the
     // following template settings to use alternative delimiters.
-    _.templateSettings = {
+    var templateSettings = _$1.templateSettings = {
         evaluate: /<%([\s\S]+?)%>/g,
         interpolate: /<%=([\s\S]+?)%>/g,
         escape: /<%-([\s\S]+?)%>/g
     };
 
-    // When customizing `templateSettings`, if you don't want to define an
+    // When customizing `_.templateSettings`, if you don't want to define an
     // interpolation, evaluation or escaping regex, we need one that is
     // guaranteed not to match.
     var noMatch = /(.)^/;
 
     // Certain characters need to be escaped so that they can be put into a
     // string literal.
     var escapes = {
@@ -1428,151 +877,1203 @@
         '\\': '\\',
         '\r': 'r',
         '\n': 'n',
         '\u2028': 'u2028',
         '\u2029': 'u2029'
     };
 
-    var escaper = /\\|'|\r|\n|\u2028|\u2029/g;
+    var escapeRegExp = /\\|'|\r|\n|\u2028|\u2029/g;
 
-    var escapeChar = function(match) {
+    function escapeChar(match) {
         return '\\' + escapes[match];
-    };
+    }
+
+    // In order to prevent third-party code injection through
+    // `_.templateSettings.variable`, we test it against the following regular
+    // expression. It is intentionally a bit more liberal than just matching valid
+    // identifiers, but still prevents possible loopholes through defaults or
+    // destructuring assignment.
+    var bareIdentifier = /^\s*(\w|\$)+\s*$/;
 
     // JavaScript micro-templating, similar to John Resig's implementation.
     // Underscore templating handles arbitrary delimiters, preserves whitespace,
     // and correctly escapes quotes within interpolated code.
     // NB: `oldSettings` only exists for backwards compatibility.
-    _.template = function(text, settings, oldSettings) {
+    function template(text, settings, oldSettings) {
         if (!settings && oldSettings) settings = oldSettings;
-        settings = _.defaults({}, settings, _.templateSettings);
+        settings = defaults({}, settings, _$1.templateSettings);
 
         // Combine delimiters into one regular expression via alternation.
         var matcher = RegExp([
             (settings.escape || noMatch).source,
             (settings.interpolate || noMatch).source,
             (settings.evaluate || noMatch).source
         ].join('|') + '|$', 'g');
 
         // Compile the template source, escaping string literals appropriately.
         var index = 0;
         var source = "__p+='";
         text.replace(matcher, function(match, escape, interpolate, evaluate, offset) {
-            source += text.slice(index, offset).replace(escaper, escapeChar);
+            source += text.slice(index, offset).replace(escapeRegExp, escapeChar);
             index = offset + match.length;
 
             if (escape) {
                 source += "'+\n((__t=(" + escape + "))==null?'':_.escape(__t))+\n'";
             } else if (interpolate) {
                 source += "'+\n((__t=(" + interpolate + "))==null?'':__t)+\n'";
             } else if (evaluate) {
                 source += "';\n" + evaluate + "\n__p+='";
             }
 
-            // Adobe VMs need the match returned to produce the correct offest.
+            // Adobe VMs need the match returned to produce the correct offset.
             return match;
         });
         source += "';\n";
 
-        // If a variable is not specified, place data values in local scope.
-        if (!settings.variable) source = 'with(obj||{}){\n' + source + '}\n';
+        var argument = settings.variable;
+        if (argument) {
+            // Insure against third-party code injection. (CVE-2021-23358)
+            if (!bareIdentifier.test(argument)) throw new Error(
+                'variable is not a bare identifier: ' + argument
+            );
+        } else {
+            // If a variable is not specified, place data values in local scope.
+            source = 'with(obj||{}){\n' + source + '}\n';
+            argument = 'obj';
+        }
 
         source = "var __t,__p='',__j=Array.prototype.join," +
             "print=function(){__p+=__j.call(arguments,'');};\n" +
             source + 'return __p;\n';
 
+        var render;
         try {
-            var render = new Function(settings.variable || 'obj', '_', source);
+            render = new Function(argument, '_', source);
         } catch (e) {
             e.source = source;
             throw e;
         }
 
         var template = function(data) {
-            return render.call(this, data, _);
+            return render.call(this, data, _$1);
         };
 
         // Provide the compiled source as a convenience for precompilation.
-        var argument = settings.variable || 'obj';
         template.source = 'function(' + argument + '){\n' + source + '}';
 
         return template;
-    };
+    }
+
+    // Traverses the children of `obj` along `path`. If a child is a function, it
+    // is invoked with its parent as context. Returns the value of the final
+    // child, or `fallback` if any child is undefined.
+    function result(obj, path, fallback) {
+        path = toPath(path);
+        var length = path.length;
+        if (!length) {
+            return isFunction$1(fallback) ? fallback.call(obj) : fallback;
+        }
+        for (var i = 0; i < length; i++) {
+            var prop = obj == null ? void 0 : obj[path[i]];
+            if (prop === void 0) {
+                prop = fallback;
+                i = length; // Ensure we don't continue iterating.
+            }
+            obj = isFunction$1(prop) ? prop.call(obj) : prop;
+        }
+        return obj;
+    }
 
-    // Add a "chain" function. Start chaining a wrapped Underscore object.
-    _.chain = function(obj) {
-        var instance = _(obj);
+    // Generate a unique integer id (unique within the entire client session).
+    // Useful for temporary DOM ids.
+    var idCounter = 0;
+
+    function uniqueId(prefix) {
+        var id = ++idCounter + '';
+        return prefix ? prefix + id : id;
+    }
+
+    // Start chaining a wrapped Underscore object.
+    function chain(obj) {
+        var instance = _$1(obj);
         instance._chain = true;
         return instance;
-    };
+    }
+
+    // Internal function to execute `sourceFunc` bound to `context` with optional
+    // `args`. Determines whether to execute a function as a constructor or as a
+    // normal function.
+    function executeBound(sourceFunc, boundFunc, context, callingContext, args) {
+        if (!(callingContext instanceof boundFunc)) return sourceFunc.apply(context, args);
+        var self = baseCreate(sourceFunc.prototype);
+        var result = sourceFunc.apply(self, args);
+        if (isObject(result)) return result;
+        return self;
+    }
+
+    // Partially apply a function by creating a version that has had some of its
+    // arguments pre-filled, without changing its dynamic `this` context. `_` acts
+    // as a placeholder by default, allowing any combination of arguments to be
+    // pre-filled. Set `_.partial.placeholder` for a custom placeholder argument.
+    var partial = restArguments(function(func, boundArgs) {
+        var placeholder = partial.placeholder;
+        var bound = function() {
+            var position = 0,
+                length = boundArgs.length;
+            var args = Array(length);
+            for (var i = 0; i < length; i++) {
+                args[i] = boundArgs[i] === placeholder ? arguments[position++] : boundArgs[i];
+            }
+            while (position < arguments.length) args.push(arguments[position++]);
+            return executeBound(func, bound, this, this, args);
+        };
+        return bound;
+    });
+
+    partial.placeholder = _$1;
+
+    // Create a function bound to a given object (assigning `this`, and arguments,
+    // optionally).
+    var bind = restArguments(function(func, context, args) {
+        if (!isFunction$1(func)) throw new TypeError('Bind must be called on a function');
+        var bound = restArguments(function(callArgs) {
+            return executeBound(func, bound, context, this, args.concat(callArgs));
+        });
+        return bound;
+    });
+
+    // Internal helper for collection methods to determine whether a collection
+    // should be iterated as an array or as an object.
+    // Related: https://people.mozilla.org/~jorendorff/es6-draft.html#sec-tolength
+    // Avoids a very nasty iOS 8 JIT bug on ARM-64. #2094
+    var isArrayLike = createSizePropertyCheck(getLength);
+
+    // Internal implementation of a recursive `flatten` function.
+    function flatten$1(input, depth, strict, output) {
+        output = output || [];
+        if (!depth && depth !== 0) {
+            depth = Infinity;
+        } else if (depth <= 0) {
+            return output.concat(input);
+        }
+        var idx = output.length;
+        for (var i = 0, length = getLength(input); i < length; i++) {
+            var value = input[i];
+            if (isArrayLike(value) && (isArray(value) || isArguments$1(value))) {
+                // Flatten current level of array or arguments object.
+                if (depth > 1) {
+                    flatten$1(value, depth - 1, strict, output);
+                    idx = output.length;
+                } else {
+                    var j = 0,
+                        len = value.length;
+                    while (j < len) output[idx++] = value[j++];
+                }
+            } else if (!strict) {
+                output[idx++] = value;
+            }
+        }
+        return output;
+    }
+
+    // Bind a number of an object's methods to that object. Remaining arguments
+    // are the method names to be bound. Useful for ensuring that all callbacks
+    // defined on an object belong to it.
+    var bindAll = restArguments(function(obj, keys) {
+        keys = flatten$1(keys, false, false);
+        var index = keys.length;
+        if (index < 1) throw new Error('bindAll must be passed function names');
+        while (index--) {
+            var key = keys[index];
+            obj[key] = bind(obj[key], obj);
+        }
+        return obj;
+    });
+
+    // Memoize an expensive function by storing its results.
+    function memoize(func, hasher) {
+        var memoize = function(key) {
+            var cache = memoize.cache;
+            var address = '' + (hasher ? hasher.apply(this, arguments) : key);
+            if (!has$1(cache, address)) cache[address] = func.apply(this, arguments);
+            return cache[address];
+        };
+        memoize.cache = {};
+        return memoize;
+    }
+
+    // Delays a function for the given number of milliseconds, and then calls
+    // it with the arguments supplied.
+    var delay = restArguments(function(func, wait, args) {
+        return setTimeout(function() {
+            return func.apply(null, args);
+        }, wait);
+    });
+
+    // Defers a function, scheduling it to run after the current call stack has
+    // cleared.
+    var defer = partial(delay, _$1, 1);
+
+    // Returns a function, that, when invoked, will only be triggered at most once
+    // during a given window of time. Normally, the throttled function will run
+    // as much as it can, without ever going more than once per `wait` duration;
+    // but if you'd like to disable the execution on the leading edge, pass
+    // `{leading: false}`. To disable execution on the trailing edge, ditto.
+    function throttle(func, wait, options) {
+        var timeout, context, args, result;
+        var previous = 0;
+        if (!options) options = {};
+
+        var later = function() {
+            previous = options.leading === false ? 0 : now();
+            timeout = null;
+            result = func.apply(context, args);
+            if (!timeout) context = args = null;
+        };
+
+        var throttled = function() {
+            var _now = now();
+            if (!previous && options.leading === false) previous = _now;
+            var remaining = wait - (_now - previous);
+            context = this;
+            args = arguments;
+            if (remaining <= 0 || remaining > wait) {
+                if (timeout) {
+                    clearTimeout(timeout);
+                    timeout = null;
+                }
+                previous = _now;
+                result = func.apply(context, args);
+                if (!timeout) context = args = null;
+            } else if (!timeout && options.trailing !== false) {
+                timeout = setTimeout(later, remaining);
+            }
+            return result;
+        };
+
+        throttled.cancel = function() {
+            clearTimeout(timeout);
+            previous = 0;
+            timeout = context = args = null;
+        };
+
+        return throttled;
+    }
+
+    // When a sequence of calls of the returned function ends, the argument
+    // function is triggered. The end of a sequence is defined by the `wait`
+    // parameter. If `immediate` is passed, the argument function will be
+    // triggered at the beginning of the sequence instead of at the end.
+    function debounce(func, wait, immediate) {
+        var timeout, previous, args, result, context;
+
+        var later = function() {
+            var passed = now() - previous;
+            if (wait > passed) {
+                timeout = setTimeout(later, wait - passed);
+            } else {
+                timeout = null;
+                if (!immediate) result = func.apply(context, args);
+                // This check is needed because `func` can recursively invoke `debounced`.
+                if (!timeout) args = context = null;
+            }
+        };
+
+        var debounced = restArguments(function(_args) {
+            context = this;
+            args = _args;
+            previous = now();
+            if (!timeout) {
+                timeout = setTimeout(later, wait);
+                if (immediate) result = func.apply(context, args);
+            }
+            return result;
+        });
+
+        debounced.cancel = function() {
+            clearTimeout(timeout);
+            timeout = args = context = null;
+        };
+
+        return debounced;
+    }
+
+    // Returns the first function passed as an argument to the second,
+    // allowing you to adjust arguments, run code before and after, and
+    // conditionally execute the original function.
+    function wrap(func, wrapper) {
+        return partial(wrapper, func);
+    }
+
+    // Returns a negated version of the passed-in predicate.
+    function negate(predicate) {
+        return function() {
+            return !predicate.apply(this, arguments);
+        };
+    }
+
+    // Returns a function that is the composition of a list of functions, each
+    // consuming the return value of the function that follows.
+    function compose() {
+        var args = arguments;
+        var start = args.length - 1;
+        return function() {
+            var i = start;
+            var result = args[start].apply(this, arguments);
+            while (i--) result = args[i].call(this, result);
+            return result;
+        };
+    }
+
+    // Returns a function that will only be executed on and after the Nth call.
+    function after(times, func) {
+        return function() {
+            if (--times < 1) {
+                return func.apply(this, arguments);
+            }
+        };
+    }
+
+    // Returns a function that will only be executed up to (but not including) the
+    // Nth call.
+    function before(times, func) {
+        var memo;
+        return function() {
+            if (--times > 0) {
+                memo = func.apply(this, arguments);
+            }
+            if (times <= 1) func = null;
+            return memo;
+        };
+    }
+
+    // Returns a function that will be executed at most one time, no matter how
+    // often you call it. Useful for lazy initialization.
+    var once = partial(before, 2);
+
+    // Returns the first key on an object that passes a truth test.
+    function findKey(obj, predicate, context) {
+        predicate = cb(predicate, context);
+        var _keys = keys(obj),
+            key;
+        for (var i = 0, length = _keys.length; i < length; i++) {
+            key = _keys[i];
+            if (predicate(obj[key], key, obj)) return key;
+        }
+    }
+
+    // Internal function to generate `_.findIndex` and `_.findLastIndex`.
+    function createPredicateIndexFinder(dir) {
+        return function(array, predicate, context) {
+            predicate = cb(predicate, context);
+            var length = getLength(array);
+            var index = dir > 0 ? 0 : length - 1;
+            for (; index >= 0 && index < length; index += dir) {
+                if (predicate(array[index], index, array)) return index;
+            }
+            return -1;
+        };
+    }
+
+    // Returns the first index on an array-like that passes a truth test.
+    var findIndex = createPredicateIndexFinder(1);
+
+    // Returns the last index on an array-like that passes a truth test.
+    var findLastIndex = createPredicateIndexFinder(-1);
+
+    // Use a comparator function to figure out the smallest index at which
+    // an object should be inserted so as to maintain order. Uses binary search.
+    function sortedIndex(array, obj, iteratee, context) {
+        iteratee = cb(iteratee, context, 1);
+        var value = iteratee(obj);
+        var low = 0,
+            high = getLength(array);
+        while (low < high) {
+            var mid = Math.floor((low + high) / 2);
+            if (iteratee(array[mid]) < value) low = mid + 1;
+            else high = mid;
+        }
+        return low;
+    }
+
+    // Internal function to generate the `_.indexOf` and `_.lastIndexOf` functions.
+    function createIndexFinder(dir, predicateFind, sortedIndex) {
+        return function(array, item, idx) {
+            var i = 0,
+                length = getLength(array);
+            if (typeof idx == 'number') {
+                if (dir > 0) {
+                    i = idx >= 0 ? idx : Math.max(idx + length, i);
+                } else {
+                    length = idx >= 0 ? Math.min(idx + 1, length) : idx + length + 1;
+                }
+            } else if (sortedIndex && idx && length) {
+                idx = sortedIndex(array, item);
+                return array[idx] === item ? idx : -1;
+            }
+            if (item !== item) {
+                idx = predicateFind(slice.call(array, i, length), isNaN$1);
+                return idx >= 0 ? idx + i : -1;
+            }
+            for (idx = dir > 0 ? i : length - 1; idx >= 0 && idx < length; idx += dir) {
+                if (array[idx] === item) return idx;
+            }
+            return -1;
+        };
+    }
+
+    // Return the position of the first occurrence of an item in an array,
+    // or -1 if the item is not included in the array.
+    // If the array is large and already in sort order, pass `true`
+    // for **isSorted** to use binary search.
+    var indexOf = createIndexFinder(1, findIndex, sortedIndex);
+
+    // Return the position of the last occurrence of an item in an array,
+    // or -1 if the item is not included in the array.
+    var lastIndexOf = createIndexFinder(-1, findLastIndex);
+
+    // Return the first value which passes a truth test.
+    function find(obj, predicate, context) {
+        var keyFinder = isArrayLike(obj) ? findIndex : findKey;
+        var key = keyFinder(obj, predicate, context);
+        if (key !== void 0 && key !== -1) return obj[key];
+    }
+
+    // Convenience version of a common use case of `_.find`: getting the first
+    // object containing specific `key:value` pairs.
+    function findWhere(obj, attrs) {
+        return find(obj, matcher(attrs));
+    }
+
+    // The cornerstone for collection functions, an `each`
+    // implementation, aka `forEach`.
+    // Handles raw objects in addition to array-likes. Treats all
+    // sparse array-likes as if they were dense.
+    function each(obj, iteratee, context) {
+        iteratee = optimizeCb(iteratee, context);
+        var i, length;
+        if (isArrayLike(obj)) {
+            for (i = 0, length = obj.length; i < length; i++) {
+                iteratee(obj[i], i, obj);
+            }
+        } else {
+            var _keys = keys(obj);
+            for (i = 0, length = _keys.length; i < length; i++) {
+                iteratee(obj[_keys[i]], _keys[i], obj);
+            }
+        }
+        return obj;
+    }
 
-    // OOP
-    // ---------------
-    // If Underscore is called as a function, it returns a wrapped object that
-    // can be used OO-style. This wrapper holds altered versions of all the
-    // underscore functions. Wrapped objects may be chained.
+    // Return the results of applying the iteratee to each element.
+    function map(obj, iteratee, context) {
+        iteratee = cb(iteratee, context);
+        var _keys = !isArrayLike(obj) && keys(obj),
+            length = (_keys || obj).length,
+            results = Array(length);
+        for (var index = 0; index < length; index++) {
+            var currentKey = _keys ? _keys[index] : index;
+            results[index] = iteratee(obj[currentKey], currentKey, obj);
+        }
+        return results;
+    }
+
+    // Internal helper to create a reducing function, iterating left or right.
+    function createReduce(dir) {
+        // Wrap code that reassigns argument variables in a separate function than
+        // the one that accesses `arguments.length` to avoid a perf hit. (#1991)
+        var reducer = function(obj, iteratee, memo, initial) {
+            var _keys = !isArrayLike(obj) && keys(obj),
+                length = (_keys || obj).length,
+                index = dir > 0 ? 0 : length - 1;
+            if (!initial) {
+                memo = obj[_keys ? _keys[index] : index];
+                index += dir;
+            }
+            for (; index >= 0 && index < length; index += dir) {
+                var currentKey = _keys ? _keys[index] : index;
+                memo = iteratee(memo, obj[currentKey], currentKey, obj);
+            }
+            return memo;
+        };
+
+        return function(obj, iteratee, memo, context) {
+            var initial = arguments.length >= 3;
+            return reducer(obj, optimizeCb(iteratee, context, 4), memo, initial);
+        };
+    }
+
+    // **Reduce** builds up a single result from a list of values, aka `inject`,
+    // or `foldl`.
+    var reduce = createReduce(1);
+
+    // The right-associative version of reduce, also known as `foldr`.
+    var reduceRight = createReduce(-1);
+
+    // Return all the elements that pass a truth test.
+    function filter(obj, predicate, context) {
+        var results = [];
+        predicate = cb(predicate, context);
+        each(obj, function(value, index, list) {
+            if (predicate(value, index, list)) results.push(value);
+        });
+        return results;
+    }
+
+    // Return all the elements for which a truth test fails.
+    function reject(obj, predicate, context) {
+        return filter(obj, negate(cb(predicate)), context);
+    }
+
+    // Determine whether all of the elements pass a truth test.
+    function every(obj, predicate, context) {
+        predicate = cb(predicate, context);
+        var _keys = !isArrayLike(obj) && keys(obj),
+            length = (_keys || obj).length;
+        for (var index = 0; index < length; index++) {
+            var currentKey = _keys ? _keys[index] : index;
+            if (!predicate(obj[currentKey], currentKey, obj)) return false;
+        }
+        return true;
+    }
+
+    // Determine if at least one element in the object passes a truth test.
+    function some(obj, predicate, context) {
+        predicate = cb(predicate, context);
+        var _keys = !isArrayLike(obj) && keys(obj),
+            length = (_keys || obj).length;
+        for (var index = 0; index < length; index++) {
+            var currentKey = _keys ? _keys[index] : index;
+            if (predicate(obj[currentKey], currentKey, obj)) return true;
+        }
+        return false;
+    }
+
+    // Determine if the array or object contains a given item (using `===`).
+    function contains(obj, item, fromIndex, guard) {
+        if (!isArrayLike(obj)) obj = values(obj);
+        if (typeof fromIndex != 'number' || guard) fromIndex = 0;
+        return indexOf(obj, item, fromIndex) >= 0;
+    }
+
+    // Invoke a method (with arguments) on every item in a collection.
+    var invoke = restArguments(function(obj, path, args) {
+        var contextPath, func;
+        if (isFunction$1(path)) {
+            func = path;
+        } else {
+            path = toPath(path);
+            contextPath = path.slice(0, -1);
+            path = path[path.length - 1];
+        }
+        return map(obj, function(context) {
+            var method = func;
+            if (!method) {
+                if (contextPath && contextPath.length) {
+                    context = deepGet(context, contextPath);
+                }
+                if (context == null) return void 0;
+                method = context[path];
+            }
+            return method == null ? method : method.apply(context, args);
+        });
+    });
+
+    // Convenience version of a common use case of `_.map`: fetching a property.
+    function pluck(obj, key) {
+        return map(obj, property(key));
+    }
+
+    // Convenience version of a common use case of `_.filter`: selecting only
+    // objects containing specific `key:value` pairs.
+    function where(obj, attrs) {
+        return filter(obj, matcher(attrs));
+    }
+
+    // Return the maximum element (or element-based computation).
+    function max(obj, iteratee, context) {
+        var result = -Infinity,
+            lastComputed = -Infinity,
+            value, computed;
+        if (iteratee == null || (typeof iteratee == 'number' && typeof obj[0] != 'object' && obj != null)) {
+            obj = isArrayLike(obj) ? obj : values(obj);
+            for (var i = 0, length = obj.length; i < length; i++) {
+                value = obj[i];
+                if (value != null && value > result) {
+                    result = value;
+                }
+            }
+        } else {
+            iteratee = cb(iteratee, context);
+            each(obj, function(v, index, list) {
+                computed = iteratee(v, index, list);
+                if (computed > lastComputed || (computed === -Infinity && result === -Infinity)) {
+                    result = v;
+                    lastComputed = computed;
+                }
+            });
+        }
+        return result;
+    }
+
+    // Return the minimum element (or element-based computation).
+    function min(obj, iteratee, context) {
+        var result = Infinity,
+            lastComputed = Infinity,
+            value, computed;
+        if (iteratee == null || (typeof iteratee == 'number' && typeof obj[0] != 'object' && obj != null)) {
+            obj = isArrayLike(obj) ? obj : values(obj);
+            for (var i = 0, length = obj.length; i < length; i++) {
+                value = obj[i];
+                if (value != null && value < result) {
+                    result = value;
+                }
+            }
+        } else {
+            iteratee = cb(iteratee, context);
+            each(obj, function(v, index, list) {
+                computed = iteratee(v, index, list);
+                if (computed < lastComputed || (computed === Infinity && result === Infinity)) {
+                    result = v;
+                    lastComputed = computed;
+                }
+            });
+        }
+        return result;
+    }
+
+    // Safely create a real, live array from anything iterable.
+    var reStrSymbol = /[^\ud800-\udfff]|[\ud800-\udbff][\udc00-\udfff]|[\ud800-\udfff]/g;
+
+    function toArray(obj) {
+        if (!obj) return [];
+        if (isArray(obj)) return slice.call(obj);
+        if (isString(obj)) {
+            // Keep surrogate pair characters together.
+            return obj.match(reStrSymbol);
+        }
+        if (isArrayLike(obj)) return map(obj, identity);
+        return values(obj);
+    }
+
+    // Sample **n** random values from a collection using the modern version of the
+    // [Fisher-Yates shuffle](https://en.wikipedia.org/wiki/Fisher–Yates_shuffle).
+    // If **n** is not specified, returns a single random element.
+    // The internal `guard` argument allows it to work with `_.map`.
+    function sample(obj, n, guard) {
+        if (n == null || guard) {
+            if (!isArrayLike(obj)) obj = values(obj);
+            return obj[random(obj.length - 1)];
+        }
+        var sample = toArray(obj);
+        var length = getLength(sample);
+        n = Math.max(Math.min(n, length), 0);
+        var last = length - 1;
+        for (var index = 0; index < n; index++) {
+            var rand = random(index, last);
+            var temp = sample[index];
+            sample[index] = sample[rand];
+            sample[rand] = temp;
+        }
+        return sample.slice(0, n);
+    }
+
+    // Shuffle a collection.
+    function shuffle(obj) {
+        return sample(obj, Infinity);
+    }
+
+    // Sort the object's values by a criterion produced by an iteratee.
+    function sortBy(obj, iteratee, context) {
+        var index = 0;
+        iteratee = cb(iteratee, context);
+        return pluck(map(obj, function(value, key, list) {
+            return {
+                value: value,
+                index: index++,
+                criteria: iteratee(value, key, list)
+            };
+        }).sort(function(left, right) {
+            var a = left.criteria;
+            var b = right.criteria;
+            if (a !== b) {
+                if (a > b || a === void 0) return 1;
+                if (a < b || b === void 0) return -1;
+            }
+            return left.index - right.index;
+        }), 'value');
+    }
+
+    // An internal function used for aggregate "group by" operations.
+    function group(behavior, partition) {
+        return function(obj, iteratee, context) {
+            var result = partition ? [
+                [],
+                []
+            ] : {};
+            iteratee = cb(iteratee, context);
+            each(obj, function(value, index) {
+                var key = iteratee(value, index, obj);
+                behavior(result, value, key);
+            });
+            return result;
+        };
+    }
+
+    // Groups the object's values by a criterion. Pass either a string attribute
+    // to group by, or a function that returns the criterion.
+    var groupBy = group(function(result, value, key) {
+        if (has$1(result, key)) result[key].push(value);
+        else result[key] = [value];
+    });
+
+    // Indexes the object's values by a criterion, similar to `_.groupBy`, but for
+    // when you know that your index values will be unique.
+    var indexBy = group(function(result, value, key) {
+        result[key] = value;
+    });
+
+    // Counts instances of an object that group by a certain criterion. Pass
+    // either a string attribute to count by, or a function that returns the
+    // criterion.
+    var countBy = group(function(result, value, key) {
+        if (has$1(result, key)) result[key]++;
+        else result[key] = 1;
+    });
+
+    // Split a collection into two arrays: one whose elements all pass the given
+    // truth test, and one whose elements all do not pass the truth test.
+    var partition = group(function(result, value, pass) {
+        result[pass ? 0 : 1].push(value);
+    }, true);
+
+    // Return the number of elements in a collection.
+    function size(obj) {
+        if (obj == null) return 0;
+        return isArrayLike(obj) ? obj.length : keys(obj).length;
+    }
+
+    // Internal `_.pick` helper function to determine whether `key` is an enumerable
+    // property name of `obj`.
+    function keyInObj(value, key, obj) {
+        return key in obj;
+    }
+
+    // Return a copy of the object only containing the allowed properties.
+    var pick = restArguments(function(obj, keys) {
+        var result = {},
+            iteratee = keys[0];
+        if (obj == null) return result;
+        if (isFunction$1(iteratee)) {
+            if (keys.length > 1) iteratee = optimizeCb(iteratee, keys[1]);
+            keys = allKeys(obj);
+        } else {
+            iteratee = keyInObj;
+            keys = flatten$1(keys, false, false);
+            obj = Object(obj);
+        }
+        for (var i = 0, length = keys.length; i < length; i++) {
+            var key = keys[i];
+            var value = obj[key];
+            if (iteratee(value, key, obj)) result[key] = value;
+        }
+        return result;
+    });
+
+    // Return a copy of the object without the disallowed properties.
+    var omit = restArguments(function(obj, keys) {
+        var iteratee = keys[0],
+            context;
+        if (isFunction$1(iteratee)) {
+            iteratee = negate(iteratee);
+            if (keys.length > 1) context = keys[1];
+        } else {
+            keys = map(flatten$1(keys, false, false), String);
+            iteratee = function(value, key) {
+                return !contains(keys, key);
+            };
+        }
+        return pick(obj, iteratee, context);
+    });
+
+    // Returns everything but the last entry of the array. Especially useful on
+    // the arguments object. Passing **n** will return all the values in
+    // the array, excluding the last N.
+    function initial(array, n, guard) {
+        return slice.call(array, 0, Math.max(0, array.length - (n == null || guard ? 1 : n)));
+    }
+
+    // Get the first element of an array. Passing **n** will return the first N
+    // values in the array. The **guard** check allows it to work with `_.map`.
+    function first(array, n, guard) {
+        if (array == null || array.length < 1) return n == null || guard ? void 0 : [];
+        if (n == null || guard) return array[0];
+        return initial(array, array.length - n);
+    }
+
+    // Returns everything but the first entry of the `array`. Especially useful on
+    // the `arguments` object. Passing an **n** will return the rest N values in the
+    // `array`.
+    function rest(array, n, guard) {
+        return slice.call(array, n == null || guard ? 1 : n);
+    }
+
+    // Get the last element of an array. Passing **n** will return the last N
+    // values in the array.
+    function last(array, n, guard) {
+        if (array == null || array.length < 1) return n == null || guard ? void 0 : [];
+        if (n == null || guard) return array[array.length - 1];
+        return rest(array, Math.max(0, array.length - n));
+    }
+
+    // Trim out all falsy values from an array.
+    function compact(array) {
+        return filter(array, Boolean);
+    }
+
+    // Flatten out an array, either recursively (by default), or up to `depth`.
+    // Passing `true` or `false` as `depth` means `1` or `Infinity`, respectively.
+    function flatten(array, depth) {
+        return flatten$1(array, depth, false);
+    }
+
+    // Take the difference between one array and a number of other arrays.
+    // Only the elements present in just the first array will remain.
+    var difference = restArguments(function(array, rest) {
+        rest = flatten$1(rest, true, true);
+        return filter(array, function(value) {
+            return !contains(rest, value);
+        });
+    });
+
+    // Return a version of the array that does not contain the specified value(s).
+    var without = restArguments(function(array, otherArrays) {
+        return difference(array, otherArrays);
+    });
+
+    // Produce a duplicate-free version of the array. If the array has already
+    // been sorted, you have the option of using a faster algorithm.
+    // The faster algorithm will not work with an iteratee if the iteratee
+    // is not a one-to-one function, so providing an iteratee will disable
+    // the faster algorithm.
+    function uniq(array, isSorted, iteratee, context) {
+        if (!isBoolean(isSorted)) {
+            context = iteratee;
+            iteratee = isSorted;
+            isSorted = false;
+        }
+        if (iteratee != null) iteratee = cb(iteratee, context);
+        var result = [];
+        var seen = [];
+        for (var i = 0, length = getLength(array); i < length; i++) {
+            var value = array[i],
+                computed = iteratee ? iteratee(value, i, array) : value;
+            if (isSorted && !iteratee) {
+                if (!i || seen !== computed) result.push(value);
+                seen = computed;
+            } else if (iteratee) {
+                if (!contains(seen, computed)) {
+                    seen.push(computed);
+                    result.push(value);
+                }
+            } else if (!contains(result, value)) {
+                result.push(value);
+            }
+        }
+        return result;
+    }
+
+    // Produce an array that contains the union: each distinct element from all of
+    // the passed-in arrays.
+    var union = restArguments(function(arrays) {
+        return uniq(flatten$1(arrays, true, true));
+    });
+
+    // Produce an array that contains every item shared between all the
+    // passed-in arrays.
+    function intersection(array) {
+        var result = [];
+        var argsLength = arguments.length;
+        for (var i = 0, length = getLength(array); i < length; i++) {
+            var item = array[i];
+            if (contains(result, item)) continue;
+            var j;
+            for (j = 1; j < argsLength; j++) {
+                if (!contains(arguments[j], item)) break;
+            }
+            if (j === argsLength) result.push(item);
+        }
+        return result;
+    }
+
+    // Complement of zip. Unzip accepts an array of arrays and groups
+    // each array's elements on shared indices.
+    function unzip(array) {
+        var length = (array && max(array, getLength).length) || 0;
+        var result = Array(length);
+
+        for (var index = 0; index < length; index++) {
+            result[index] = pluck(array, index);
+        }
+        return result;
+    }
+
+    // Zip together multiple lists into a single array -- elements that share
+    // an index go together.
+    var zip = restArguments(unzip);
+
+    // Converts lists into objects. Pass either a single array of `[key, value]`
+    // pairs, or two parallel arrays of the same length -- one of keys, and one of
+    // the corresponding values. Passing by pairs is the reverse of `_.pairs`.
+    function object(list, values) {
+        var result = {};
+        for (var i = 0, length = getLength(list); i < length; i++) {
+            if (values) {
+                result[list[i]] = values[i];
+            } else {
+                result[list[i][0]] = list[i][1];
+            }
+        }
+        return result;
+    }
+
+    // Generate an integer Array containing an arithmetic progression. A port of
+    // the native Python `range()` function. See
+    // [the Python documentation](https://docs.python.org/library/functions.html#range).
+    function range(start, stop, step) {
+        if (stop == null) {
+            stop = start || 0;
+            start = 0;
+        }
+        if (!step) {
+            step = stop < start ? -1 : 1;
+        }
+
+        var length = Math.max(Math.ceil((stop - start) / step), 0);
+        var range = Array(length);
+
+        for (var idx = 0; idx < length; idx++, start += step) {
+            range[idx] = start;
+        }
+
+        return range;
+    }
+
+    // Chunk a single array into multiple arrays, each containing `count` or fewer
+    // items.
+    function chunk(array, count) {
+        if (count == null || count < 1) return [];
+        var result = [];
+        var i = 0,
+            length = array.length;
+        while (i < length) {
+            result.push(slice.call(array, i, i += count));
+        }
+        return result;
+    }
 
     // Helper function to continue chaining intermediate results.
-    var result = function(instance, obj) {
-        return instance._chain ? _(obj).chain() : obj;
-    };
+    function chainResult(instance, obj) {
+        return instance._chain ? _$1(obj).chain() : obj;
+    }
 
     // Add your own custom functions to the Underscore object.
-    _.mixin = function(obj) {
-        _.each(_.functions(obj), function(name) {
-            var func = _[name] = obj[name];
-            _.prototype[name] = function() {
+    function mixin(obj) {
+        each(functions(obj), function(name) {
+            var func = _$1[name] = obj[name];
+            _$1.prototype[name] = function() {
                 var args = [this._wrapped];
                 push.apply(args, arguments);
-                return result(this, func.apply(_, args));
+                return chainResult(this, func.apply(_$1, args));
             };
         });
-    };
-
-    // Add all of the Underscore functions to the wrapper object.
-    _.mixin(_);
+        return _$1;
+    }
 
-    // Add all mutator Array functions to the wrapper.
-    _.each(['pop', 'push', 'reverse', 'shift', 'sort', 'splice', 'unshift'], function(name) {
+    // Add all mutator `Array` functions to the wrapper.
+    each(['pop', 'push', 'reverse', 'shift', 'sort', 'splice', 'unshift'], function(name) {
         var method = ArrayProto[name];
-        _.prototype[name] = function() {
+        _$1.prototype[name] = function() {
             var obj = this._wrapped;
-            method.apply(obj, arguments);
-            if ((name === 'shift' || name === 'splice') && obj.length === 0) delete obj[0];
-            return result(this, obj);
+            if (obj != null) {
+                method.apply(obj, arguments);
+                if ((name === 'shift' || name === 'splice') && obj.length === 0) {
+                    delete obj[0];
+                }
+            }
+            return chainResult(this, obj);
         };
     });
 
-    // Add all accessor Array functions to the wrapper.
-    _.each(['concat', 'join', 'slice'], function(name) {
+    // Add all accessor `Array` functions to the wrapper.
+    each(['concat', 'join', 'slice'], function(name) {
         var method = ArrayProto[name];
-        _.prototype[name] = function() {
-            return result(this, method.apply(this._wrapped, arguments));
+        _$1.prototype[name] = function() {
+            var obj = this._wrapped;
+            if (obj != null) obj = method.apply(obj, arguments);
+            return chainResult(this, obj);
         };
     });
 
-    // Extracts the result from a wrapped and chained object.
-    _.prototype.value = function() {
-        return this._wrapped;
+    // Named Exports
+
+    var allExports = {
+        __proto__: null,
+        VERSION: VERSION,
+        restArguments: restArguments,
+        isObject: isObject,
+        isNull: isNull,
+        isUndefined: isUndefined,
+        isBoolean: isBoolean,
+        isElement: isElement,
+        isString: isString,
+        isNumber: isNumber,
+        isDate: isDate,
+        isRegExp: isRegExp,
+        isError: isError,
+        isSymbol: isSymbol,
+        isArrayBuffer: isArrayBuffer,
+        isDataView: isDataView$1,
+        isArray: isArray,
+        isFunction: isFunction$1,
+        isArguments: isArguments$1,
+        isFinite: isFinite$1,
+        isNaN: isNaN$1,
+        isTypedArray: isTypedArray$1,
+        isEmpty: isEmpty,
+        isMatch: isMatch,
+        isEqual: isEqual,
+        isMap: isMap,
+        isWeakMap: isWeakMap,
+        isSet: isSet,
+        isWeakSet: isWeakSet,
+        keys: keys,
+        allKeys: allKeys,
+        values: values,
+        pairs: pairs,
+        invert: invert,
+        functions: functions,
+        methods: functions,
+        extend: extend,
+        extendOwn: extendOwn,
+        assign: extendOwn,
+        defaults: defaults,
+        create: create,
+        clone: clone,
+        tap: tap,
+        get: get,
+        has: has,
+        mapObject: mapObject,
+        identity: identity,
+        constant: constant,
+        noop: noop,
+        toPath: toPath$1,
+        property: property,
+        propertyOf: propertyOf,
+        matcher: matcher,
+        matches: matcher,
+        times: times,
+        random: random,
+        now: now,
+        escape: _escape,
+        unescape: _unescape,
+        templateSettings: templateSettings,
+        template: template,
+        result: result,
+        uniqueId: uniqueId,
+        chain: chain,
+        iteratee: iteratee,
+        partial: partial,
+        bind: bind,
+        bindAll: bindAll,
+        memoize: memoize,
+        delay: delay,
+        defer: defer,
+        throttle: throttle,
+        debounce: debounce,
+        wrap: wrap,
+        negate: negate,
+        compose: compose,
+        after: after,
+        before: before,
+        once: once,
+        findKey: findKey,
+        findIndex: findIndex,
+        findLastIndex: findLastIndex,
+        sortedIndex: sortedIndex,
+        indexOf: indexOf,
+        lastIndexOf: lastIndexOf,
+        find: find,
+        detect: find,
+        findWhere: findWhere,
+        each: each,
+        forEach: each,
+        map: map,
+        collect: map,
+        reduce: reduce,
+        foldl: reduce,
+        inject: reduce,
+        reduceRight: reduceRight,
+        foldr: reduceRight,
+        filter: filter,
+        select: filter,
+        reject: reject,
+        every: every,
+        all: every,
+        some: some,
+        any: some,
+        contains: contains,
+        includes: contains,
+        include: contains,
+        invoke: invoke,
+        pluck: pluck,
+        where: where,
+        max: max,
+        min: min,
+        shuffle: shuffle,
+        sample: sample,
+        sortBy: sortBy,
+        groupBy: groupBy,
+        indexBy: indexBy,
+        countBy: countBy,
+        partition: partition,
+        toArray: toArray,
+        size: size,
+        pick: pick,
+        omit: omit,
+        first: first,
+        head: first,
+        take: first,
+        initial: initial,
+        last: last,
+        rest: rest,
+        tail: rest,
+        drop: rest,
+        compact: compact,
+        flatten: flatten,
+        without: without,
+        uniq: uniq,
+        unique: uniq,
+        union: union,
+        intersection: intersection,
+        difference: difference,
+        unzip: unzip,
+        transpose: unzip,
+        zip: zip,
+        object: object,
+        range: range,
+        chunk: chunk,
+        mixin: mixin,
+        'default': _$1
     };
 
-    // Provide unwrapping proxy for some methods used in engine operations
-    // such as arithmetic and JSON stringification.
-    _.prototype.valueOf = _.prototype.toJSON = _.prototype.value;
+    // Default Export
 
-    _.prototype.toString = function() {
-        return '' + this._wrapped;
-    };
+    // Add all of the Underscore functions to the wrapper object.
+    var _ = mixin(allExports);
+    // Legacy Node.js API.
+    _._ = _;
 
-    // AMD registration happens at the end for compatibility with AMD loaders
-    // that may not enforce next-turn semantics on modules. Even though general
-    // practice for AMD registration is to be anonymous, underscore registers
-    // as a named module because, like jQuery, it is a base library that is
-    // popular enough to be bundled in a third party lib, but not be part of
-    // an AMD load request. Those cases could generate an error when an
-    // anonymous define() is called outside of a loader request.
-    if (typeof define === 'function' && define.amd) {
-        define('underscore', [], function() {
-            return _;
-        });
-    }
-}.call(this));
+    return _;
+
+})));
+//# sourceMappingURL=underscore-umd.js.map
```

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/index.html` & `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/index.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,166 +1,123 @@
-
-
 <!DOCTYPE html>
-<!--[if IE 8]><html class="no-js lt-ie9" lang="en" > <![endif]-->
-<!--[if gt IE 8]><!--> <html class="no-js" lang="en" > <!--<![endif]-->
+<html class="writer-html5" lang="en" >
 <head>
-  <meta charset="utf-8">
-  <meta name="viewport" content="width=device-width, initial-scale=1.0">
-  
-  <title>Welcome to pysoundanalyser’s documentation! &mdash; pysoundanalyser (&#39;0.2.39&#39;,) documentation</title>
-  
-
-  
-  
-
-  
-  <link href='https://fonts.googleapis.com/css?family=Lato:400,700|Roboto+Slab:400,700|Inconsolata:400,700' rel='stylesheet' type='text/css'>
-
-  
-  
-
-    <script type="text/javascript">
-      var DOCUMENTATION_OPTIONS = {
-        URL_ROOT:'./',
-        VERSION:'(&#39;0.2.39&#39;,)',
-        COLLAPSE_INDEX:false,
-        FILE_SUFFIX:'.html',
-        HAS_SOURCE:  true
-      };
-    </script>
-      <script type="text/javascript" src="_static/jquery.js"></script>
-      <script type="text/javascript" src="_static/underscore.js"></script>
-      <script type="text/javascript" src="_static/doctools.js"></script>
-      <script type="text/javascript" src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
-
-    
-
-  
-
-  
-  
-    <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
-    <script type="text/javascript" src="_static/js/theme.js"></script>
-  
-
-  
-        <link rel="index" title="Index"
-              href="genindex.html"/>
-        <link rel="search" title="Search" href="search.html"/>
-    <link rel="top" title="pysoundanalyser (&#39;0.2.39&#39;,) documentation" href="#"/>
-        <link rel="next" title="What is pysoundanalyser?" href="intro.html"/> 
-
-  <script src="//cdnjs.cloudflare.com/ajax/libs/modernizr/2.6.2/modernizr.min.js"></script>
+  <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
+  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
+  <title>Welcome to pysoundanalyser’s documentation! &mdash; pysoundanalyser 0.3.2 documentation</title>
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
+    <link rel="index" title="Index" href="genindex.html" />
+    <link rel="search" title="Search" href="search.html" />
+    <link rel="next" title="What is pysoundanalyser?" href="intro.html" /> 
 </head>
 
-<body class="wy-body-for-nav">
-
+<body class="wy-body-for-nav"> 
   <div class="wy-grid-for-nav">
-
-    
     <nav data-toggle="wy-nav-shift" class="wy-nav-side">
-      <div class="wy-side-nav-search">
-        <a href="#" class="icon icon-home"> pysoundanalyser</a>
-        <form class="wy-form" action="search.html" method="get">
-  <input type="text" name="q" placeholder="Search docs" />
-  <input type="hidden" name="check_keywords" value="yes" />
-  <input type="hidden" name="area" value="default" />
-</form>
-      </div>
+      <div class="wy-side-scroll">
+        <div class="wy-side-nav-search" >
 
-      <div class="wy-menu wy-menu-vertical" data-spy="affix">
-        
-        
-            <ul>
-<li class="toctree-l1"><a class="reference internal" href="intro.html">What is <code class="docutils literal"><span class="pre">pysoundanalyser</span></code>?</a></li>
-<li class="toctree-l1"><a class="reference internal" href="installation.html">Installation</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="installation.html#installation-on-linux">Installation on Linux</a></li>
-<li class="toctree-l2"><a class="reference internal" href="installation.html#installation-on-windows">Installation on Windows</a></li>
-<li class="toctree-l2"><a class="reference internal" href="installation.html#installation-on-the-mac">Installation on the Mac</a></li>
-<li class="toctree-l2"><a class="reference internal" href="installation.html#installation-from-source">Installation from source</a></li>
-</ul>
-</li>
+          
+          
+          <a href="#" class="icon icon-home">
+            pysoundanalyser
+          </a>
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
+<li class="toctree-l1"><a class="reference internal" href="intro.html">What is <code class="docutils literal notranslate"><span class="pre">pysoundanalyser</span></code>?</a></li>
+<li class="toctree-l1"><a class="reference internal" href="installation.html">Installation</a></li>
 <li class="toctree-l1"><a class="reference internal" href="user_interface.html">User Interface</a></li>
 </ul>
 
-        
+        </div>
       </div>
-      &nbsp;
     </nav>
 
-    <section data-toggle="wy-nav-shift" class="wy-nav-content-wrap">
-
-      
-      <nav class="wy-nav-top">
-        <i data-toggle="wy-nav-top" class="icon icon-reorder"></i>
-        <a href="/">pysoundanalyser</a>
+    <section data-toggle="wy-nav-shift" class="wy-nav-content-wrap"><nav class="wy-nav-top" aria-label="Mobile navigation menu" >
+          <i data-toggle="wy-nav-top" class="fa fa-bars"></i>
+          <a href="#">pysoundanalyser</a>
       </nav>
 
-
-      
       <div class="wy-nav-content">
         <div class="rst-content">
-          <ul class="wy-breadcrumbs">
-  <li><a href="#">Docs</a> &raquo;</li>
-  <li><a href="">Welcome to pysoundanalyser&#8217;s documentation!</a></li>
-  
-</ul>
-<hr/>
-
-          
-  <div class="section" id="welcome-to-pysoundanalyser-s-documentation">
-<h1>Welcome to pysoundanalyser&#8217;s documentation!<a class="headerlink" href="#welcome-to-pysoundanalyser-s-documentation" title="Permalink to this headline">¶</a></h1>
-<p>Contents:</p>
+          <div role="navigation" aria-label="Page navigation">
+  <ul class="wy-breadcrumbs">
+      <li><a href="#" class="icon icon-home" aria-label="Home"></a></li>
+      <li class="breadcrumb-item active">Welcome to pysoundanalyser’s documentation!</li>
+      <li class="wy-breadcrumbs-aside">
+            <a href="_sources/index.rst.txt" rel="nofollow"> View page source</a>
+      </li>
+  </ul>
+  <hr/>
+</div>
+          <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
+           <div itemprop="articleBody">
+             
+  <section id="welcome-to-pysoundanalyser-s-documentation">
+<h1>Welcome to pysoundanalyser’s documentation!<a class="headerlink" href="#welcome-to-pysoundanalyser-s-documentation" title="Permalink to this heading"></a></h1>
 <div class="toctree-wrapper compound">
+<p class="caption" role="heading"><span class="caption-text">Contents:</span></p>
 <ul>
-<li class="toctree-l1"><a class="reference internal" href="intro.html">What is <code class="docutils literal"><span class="pre">pysoundanalyser</span></code>?</a></li>
-<li class="toctree-l1"><a class="reference internal" href="installation.html">Installation</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="installation.html#installation-on-linux">Installation on Linux</a></li>
-<li class="toctree-l2"><a class="reference internal" href="installation.html#installation-on-windows">Installation on Windows</a></li>
-<li class="toctree-l2"><a class="reference internal" href="installation.html#installation-on-the-mac">Installation on the Mac</a></li>
-<li class="toctree-l2"><a class="reference internal" href="installation.html#installation-from-source">Installation from source</a></li>
-</ul>
-</li>
+<li class="toctree-l1"><a class="reference internal" href="intro.html">What is <code class="docutils literal notranslate"><span class="pre">pysoundanalyser</span></code>?</a></li>
+<li class="toctree-l1"><a class="reference internal" href="installation.html">Installation</a></li>
 <li class="toctree-l1"><a class="reference internal" href="user_interface.html">User Interface</a></li>
 </ul>
 </div>
-</div>
-<div class="section" id="indices-and-tables">
-<h1>Indices and tables<a class="headerlink" href="#indices-and-tables" title="Permalink to this headline">¶</a></h1>
+</section>
+<section id="indices-and-tables">
+<h1>Indices and tables<a class="headerlink" href="#indices-and-tables" title="Permalink to this heading"></a></h1>
 <ul class="simple">
-<li><a class="reference internal" href="genindex.html"><span class="std std-ref">Index</span></a></li>
-<li><a class="reference internal" href="py-modindex.html"><span class="std std-ref">Module Index</span></a></li>
-<li><a class="reference internal" href="search.html"><span class="std std-ref">Search Page</span></a></li>
+<li><p><a class="reference internal" href="genindex.html"><span class="std std-ref">Index</span></a></p></li>
+<li><p><a class="reference internal" href="py-modindex.html"><span class="std std-ref">Module Index</span></a></p></li>
+<li><p><a class="reference internal" href="search.html"><span class="std std-ref">Search Page</span></a></p></li>
 </ul>
-</div>
+</section>
 
 
-          <footer>
-  
-    <div class="rst-footer-buttons">
-      
-        <a href="intro.html" class="btn btn-neutral float-right" title="What is pysoundanalyser?"/>Next <span class="icon icon-circle-arrow-right"></span></a>
-      
-      
+           </div>
+          </div>
+          <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
+        <a href="intro.html" class="btn btn-neutral float-right" title="What is pysoundanalyser?" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
     </div>
-  
 
   <hr/>
 
-  <p>
-      &copy; Copyright 2010-2017, Samuele Carcagno.
-  </p>
+  <div role="contentinfo">
+    <p>&#169; Copyright 2010-2023, Samuele Carcagno.</p>
+  </div>
+
+  Built with <a href="https://www.sphinx-doc.org/">Sphinx</a> using a
+    <a href="https://github.com/readthedocs/sphinx_rtd_theme">theme</a>
+    provided by <a href="https://readthedocs.org">Read the Docs</a>.
+   
 
-  <a href="https://www.github.com/snide/sphinx_rtd_theme">Sphinx theme</a> provided by <a href="http://readthedocs.org">Read the Docs</a>
 </footer>
         </div>
       </div>
-
     </section>
-
   </div>
-  
+  <script>
+      jQuery(function () {
+          SphinxRtdTheme.Navigation.enable(true);
+      });
+  </script> 
 
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,38 +1,29 @@
 
 
 
 
 
-
-
-
 pysoundanalyser
 [q                   ]
+Contents:
     * What_is_pysoundanalyser?
     * Installation
-          o Installation_on_Linux
-          o Installation_on_Windows
-          o Installation_on_the_Mac
-          o Installation_from_source
     * User_Interface
-      pysoundanalyser
-    * Docs »
-    * Welcome to pysoundanalyser’s documentation!
+   pysoundanalyser
+    * Welcome to pysoundanalyserâs documentation!
+    * View_page_source
 ===============================================================================
-****** Welcome to pysoundanalyser’s documentation!Â¶ ******
+****** Welcome to pysoundanalyserâs documentation!ï ******
 Contents:
     * What_is_pysoundanalyser?
     * Installation
-          o Installation_on_Linux
-          o Installation_on_Windows
-          o Installation_on_the_Mac
-          o Installation_from_source
     * User_Interface
-****** Indices and tablesÂ¶ ******
+
+****** Indices and tablesï ******
     * Index
     * Module_Index
     * Search_Page
 Next
 ===============================================================================
-© Copyright 2010-2017, Samuele Carcagno.
-Sphinx_theme provided by Read_the_Docs
+© Copyright 2010-2023, Samuele Carcagno.
+Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/intro.html` & `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/intro.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,149 +1,111 @@
-
-
 <!DOCTYPE html>
-<!--[if IE 8]><html class="no-js lt-ie9" lang="en" > <![endif]-->
-<!--[if gt IE 8]><!--> <html class="no-js" lang="en" > <!--<![endif]-->
+<html class="writer-html5" lang="en" >
 <head>
-  <meta charset="utf-8">
-  <meta name="viewport" content="width=device-width, initial-scale=1.0">
-  
-  <title>What is pysoundanalyser? &mdash; pysoundanalyser (&#39;0.2.39&#39;,) documentation</title>
-  
-
-  
-  
-
-  
-  <link href='https://fonts.googleapis.com/css?family=Lato:400,700|Roboto+Slab:400,700|Inconsolata:400,700' rel='stylesheet' type='text/css'>
-
-  
-  
-
-    <script type="text/javascript">
-      var DOCUMENTATION_OPTIONS = {
-        URL_ROOT:'./',
-        VERSION:'(&#39;0.2.39&#39;,)',
-        COLLAPSE_INDEX:false,
-        FILE_SUFFIX:'.html',
-        HAS_SOURCE:  true
-      };
-    </script>
-      <script type="text/javascript" src="_static/jquery.js"></script>
-      <script type="text/javascript" src="_static/underscore.js"></script>
-      <script type="text/javascript" src="_static/doctools.js"></script>
-      <script type="text/javascript" src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
-
-    
-
-  
-
-  
-  
-    <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
-    <script type="text/javascript" src="_static/js/theme.js"></script>
-  
-
-  
-        <link rel="index" title="Index"
-              href="genindex.html"/>
-        <link rel="search" title="Search" href="search.html"/>
-    <link rel="top" title="pysoundanalyser (&#39;0.2.39&#39;,) documentation" href="index.html"/>
-        <link rel="next" title="Installation" href="installation.html"/>
-        <link rel="prev" title="Welcome to pysoundanalyser’s documentation!" href="index.html"/> 
-
-  <script src="//cdnjs.cloudflare.com/ajax/libs/modernizr/2.6.2/modernizr.min.js"></script>
+  <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
+  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
+  <title>What is pysoundanalyser? &mdash; pysoundanalyser 0.3.2 documentation</title>
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
+    <link rel="index" title="Index" href="genindex.html" />
+    <link rel="search" title="Search" href="search.html" />
+    <link rel="next" title="Installation" href="installation.html" />
+    <link rel="prev" title="Welcome to pysoundanalyser’s documentation!" href="index.html" /> 
 </head>
 
-<body class="wy-body-for-nav">
-
+<body class="wy-body-for-nav"> 
   <div class="wy-grid-for-nav">
-
-    
     <nav data-toggle="wy-nav-shift" class="wy-nav-side">
-      <div class="wy-side-nav-search">
-        <a href="index.html" class="icon icon-home"> pysoundanalyser</a>
-        <form class="wy-form" action="search.html" method="get">
-  <input type="text" name="q" placeholder="Search docs" />
-  <input type="hidden" name="check_keywords" value="yes" />
-  <input type="hidden" name="area" value="default" />
-</form>
-      </div>
+      <div class="wy-side-scroll">
+        <div class="wy-side-nav-search" >
 
-      <div class="wy-menu wy-menu-vertical" data-spy="affix">
-        
-        
-            <ul class="current">
-<li class="toctree-l1 current"><a class="current reference internal" href="#">What is <code class="docutils literal"><span class="pre">pysoundanalyser</span></code>?</a></li>
-<li class="toctree-l1"><a class="reference internal" href="installation.html">Installation</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="installation.html#installation-on-linux">Installation on Linux</a></li>
-<li class="toctree-l2"><a class="reference internal" href="installation.html#installation-on-windows">Installation on Windows</a></li>
-<li class="toctree-l2"><a class="reference internal" href="installation.html#installation-on-the-mac">Installation on the Mac</a></li>
-<li class="toctree-l2"><a class="reference internal" href="installation.html#installation-from-source">Installation from source</a></li>
-</ul>
-</li>
+          
+          
+          <a href="index.html" class="icon icon-home">
+            pysoundanalyser
+          </a>
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
+<li class="toctree-l1 current"><a class="current reference internal" href="#">What is <code class="docutils literal notranslate"><span class="pre">pysoundanalyser</span></code>?</a></li>
+<li class="toctree-l1"><a class="reference internal" href="installation.html">Installation</a></li>
 <li class="toctree-l1"><a class="reference internal" href="user_interface.html">User Interface</a></li>
 </ul>
 
-        
+        </div>
       </div>
-      &nbsp;
     </nav>
 
-    <section data-toggle="wy-nav-shift" class="wy-nav-content-wrap">
-
-      
-      <nav class="wy-nav-top">
-        <i data-toggle="wy-nav-top" class="icon icon-reorder"></i>
-        <a href="/">pysoundanalyser</a>
+    <section data-toggle="wy-nav-shift" class="wy-nav-content-wrap"><nav class="wy-nav-top" aria-label="Mobile navigation menu" >
+          <i data-toggle="wy-nav-top" class="fa fa-bars"></i>
+          <a href="index.html">pysoundanalyser</a>
       </nav>
 
-
-      
       <div class="wy-nav-content">
         <div class="rst-content">
-          <ul class="wy-breadcrumbs">
-  <li><a href="index.html">Docs</a> &raquo;</li>
-  <li><a href="">What is <code class="docutils literal"><span class="pre">pysoundanalyser</span></code>?</a></li>
-  
-</ul>
-<hr/>
-
-          
-  <div class="section" id="what-is-pysoundanalyser">
-<h1>What is <code class="docutils literal"><span class="pre">pysoundanalyser</span></code>?<a class="headerlink" href="#what-is-pysoundanalyser" title="Permalink to this headline">¶</a></h1>
-<p><code class="docutils literal"><span class="pre">pysoundanalyser</span></code> is an application which provides a graphical user interface to analyse short (in the range of seconds) wav files. I developed and use it mainly to quickly load and visualize the waveforms and the spectral content of sounds generated for psychoacoustics research. <code class="docutils literal"><span class="pre">pysoundanalyser</span></code> can also generate some types of sounds used in psychoacoustics research (e.g. pure tones, amplitude modulated tones, frequency modulated tones, different colors of noise, etc...).</p>
-<p>The repository of <code class="docutils literal"><span class="pre">pysoundanalyser</span></code> is hosted on <a class="reference external" href="https://github.com/sam81/pysoundanalyser">GitHub</a>. If you find bugs, please report them <a class="reference external" href="https://github.com/sam81/pysoundanalyser/issues">there</a>.</p>
+          <div role="navigation" aria-label="Page navigation">
+  <ul class="wy-breadcrumbs">
+      <li><a href="index.html" class="icon icon-home" aria-label="Home"></a></li>
+      <li class="breadcrumb-item active">What is <code class="docutils literal notranslate"><span class="pre">pysoundanalyser</span></code>?</li>
+      <li class="wy-breadcrumbs-aside">
+            <a href="_sources/intro.rst.txt" rel="nofollow"> View page source</a>
+      </li>
+  </ul>
+  <hr/>
 </div>
+          <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
+           <div itemprop="articleBody">
+             
+  <section id="what-is-pysoundanalyser">
+<h1>What is <code class="docutils literal notranslate"><span class="pre">pysoundanalyser</span></code>?<a class="headerlink" href="#what-is-pysoundanalyser" title="Permalink to this heading"></a></h1>
+<p><code class="docutils literal notranslate"><span class="pre">pysoundanalyser</span></code> is an application which provides a graphical user interface to analyse short (in the range of seconds) wav files. I developed and use it mainly to quickly load and visualize the waveforms and the spectral content of sounds generated for psychoacoustics research. <code class="docutils literal notranslate"><span class="pre">pysoundanalyser</span></code> can also generate some types of sounds used in psychoacoustics research (e.g. pure tones, amplitude modulated tones, frequency modulated tones, different colors of noise, etc…).</p>
+<p>The repository of <code class="docutils literal notranslate"><span class="pre">pysoundanalyser</span></code> is hosted on <a class="reference external" href="https://github.com/sam81/pysoundanalyser">GitHub</a>. If you find bugs, please report them <a class="reference external" href="https://github.com/sam81/pysoundanalyser/issues">there</a>.</p>
+</section>
 
 
-          <footer>
-  
-    <div class="rst-footer-buttons">
-      
-        <a href="installation.html" class="btn btn-neutral float-right" title="Installation"/>Next <span class="icon icon-circle-arrow-right"></span></a>
-      
-      
-        <a href="index.html" class="btn btn-neutral" title="Welcome to pysoundanalyser’s documentation!"><span class="icon icon-circle-arrow-left"></span> Previous</a>
-      
+           </div>
+          </div>
+          <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
+        <a href="index.html" class="btn btn-neutral float-left" title="Welcome to pysoundanalyser’s documentation!" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
+        <a href="installation.html" class="btn btn-neutral float-right" title="Installation" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
     </div>
-  
 
   <hr/>
 
-  <p>
-      &copy; Copyright 2010-2017, Samuele Carcagno.
-  </p>
+  <div role="contentinfo">
+    <p>&#169; Copyright 2010-2023, Samuele Carcagno.</p>
+  </div>
+
+  Built with <a href="https://www.sphinx-doc.org/">Sphinx</a> using a
+    <a href="https://github.com/readthedocs/sphinx_rtd_theme">theme</a>
+    provided by <a href="https://readthedocs.org">Read the Docs</a>.
+   
 
-  <a href="https://www.github.com/snide/sphinx_rtd_theme">Sphinx theme</a> provided by <a href="http://readthedocs.org">Read the Docs</a>
 </footer>
         </div>
       </div>
-
     </section>
-
   </div>
-  
+  <script>
+      jQuery(function () {
+          SphinxRtdTheme.Navigation.enable(true);
+      });
+  </script> 
 
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,36 +1,30 @@
 
 
 
 
 
 
-
-
-
 pysoundanalyser
 [q                   ]
+Contents:
     * What_is_pysoundanalyser?
     * Installation
-          o Installation_on_Linux
-          o Installation_on_Windows
-          o Installation_on_the_Mac
-          o Installation_from_source
     * User_Interface
-      pysoundanalyser
-    * Docs »
+   pysoundanalyser
     * What is pysoundanalyser?
+    * View_page_source
 ===============================================================================
-****** What is pysoundanalyser?Â¶ ******
+****** What is pysoundanalyser?ï ******
 pysoundanalyser is an application which provides a graphical user interface to
 analyse short (in the range of seconds) wav files. I developed and use it
 mainly to quickly load and visualize the waveforms and the spectral content of
 sounds generated for psychoacoustics research. pysoundanalyser can also
 generate some types of sounds used in psychoacoustics research (e.g. pure
 tones, amplitude modulated tones, frequency modulated tones, different colors
-of noise, etc...).
+of noise, etcâ¦).
 The repository of pysoundanalyser is hosted on GitHub. If you find bugs, please
 report them there.
-Next Previous
+Previous Next
 ===============================================================================
-© Copyright 2010-2017, Samuele Carcagno.
-Sphinx_theme provided by Read_the_Docs
+© Copyright 2010-2023, Samuele Carcagno.
+Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/doc/_build/html/user_interface.html` & `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/user_interface.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,195 +1,144 @@
-
-
 <!DOCTYPE html>
-<!--[if IE 8]><html class="no-js lt-ie9" lang="en" > <![endif]-->
-<!--[if gt IE 8]><!--> <html class="no-js" lang="en" > <!--<![endif]-->
+<html class="writer-html5" lang="en" >
 <head>
-  <meta charset="utf-8">
-  <meta name="viewport" content="width=device-width, initial-scale=1.0">
-  
-  <title>User Interface &mdash; pysoundanalyser (&#39;0.2.39&#39;,) documentation</title>
-  
-
-  
-  
-
-  
-  <link href='https://fonts.googleapis.com/css?family=Lato:400,700|Roboto+Slab:400,700|Inconsolata:400,700' rel='stylesheet' type='text/css'>
-
-  
-  
-
-    <script type="text/javascript">
-      var DOCUMENTATION_OPTIONS = {
-        URL_ROOT:'./',
-        VERSION:'(&#39;0.2.39&#39;,)',
-        COLLAPSE_INDEX:false,
-        FILE_SUFFIX:'.html',
-        HAS_SOURCE:  true
-      };
-    </script>
-      <script type="text/javascript" src="_static/jquery.js"></script>
-      <script type="text/javascript" src="_static/underscore.js"></script>
-      <script type="text/javascript" src="_static/doctools.js"></script>
-      <script type="text/javascript" src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
-
-    
-
-  
-
-  
-  
-    <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
-    <script type="text/javascript" src="_static/js/theme.js"></script>
-  
-
-  
-        <link rel="index" title="Index"
-              href="genindex.html"/>
-        <link rel="search" title="Search" href="search.html"/>
-    <link rel="top" title="pysoundanalyser (&#39;0.2.39&#39;,) documentation" href="index.html"/>
-        <link rel="prev" title="Installation" href="installation.html"/> 
-
-  <script src="//cdnjs.cloudflare.com/ajax/libs/modernizr/2.6.2/modernizr.min.js"></script>
+  <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
+  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
+  <title>User Interface &mdash; pysoundanalyser 0.3.2 documentation</title>
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
+    <link rel="index" title="Index" href="genindex.html" />
+    <link rel="search" title="Search" href="search.html" />
+    <link rel="prev" title="Installation" href="installation.html" /> 
 </head>
 
-<body class="wy-body-for-nav">
-
+<body class="wy-body-for-nav"> 
   <div class="wy-grid-for-nav">
-
-    
     <nav data-toggle="wy-nav-shift" class="wy-nav-side">
-      <div class="wy-side-nav-search">
-        <a href="index.html" class="icon icon-home"> pysoundanalyser</a>
-        <form class="wy-form" action="search.html" method="get">
-  <input type="text" name="q" placeholder="Search docs" />
-  <input type="hidden" name="check_keywords" value="yes" />
-  <input type="hidden" name="area" value="default" />
-</form>
-      </div>
+      <div class="wy-side-scroll">
+        <div class="wy-side-nav-search" >
 
-      <div class="wy-menu wy-menu-vertical" data-spy="affix">
-        
-        
-            <ul class="current">
-<li class="toctree-l1"><a class="reference internal" href="intro.html">What is <code class="docutils literal"><span class="pre">pysoundanalyser</span></code>?</a></li>
-<li class="toctree-l1"><a class="reference internal" href="installation.html">Installation</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="installation.html#installation-on-linux">Installation on Linux</a></li>
-<li class="toctree-l2"><a class="reference internal" href="installation.html#installation-on-windows">Installation on Windows</a></li>
-<li class="toctree-l2"><a class="reference internal" href="installation.html#installation-on-the-mac">Installation on the Mac</a></li>
-<li class="toctree-l2"><a class="reference internal" href="installation.html#installation-from-source">Installation from source</a></li>
-</ul>
-</li>
+          
+          
+          <a href="index.html" class="icon icon-home">
+            pysoundanalyser
+          </a>
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
+<li class="toctree-l1"><a class="reference internal" href="intro.html">What is <code class="docutils literal notranslate"><span class="pre">pysoundanalyser</span></code>?</a></li>
+<li class="toctree-l1"><a class="reference internal" href="installation.html">Installation</a></li>
 <li class="toctree-l1 current"><a class="current reference internal" href="#">User Interface</a></li>
 </ul>
 
-        
+        </div>
       </div>
-      &nbsp;
     </nav>
 
-    <section data-toggle="wy-nav-shift" class="wy-nav-content-wrap">
-
-      
-      <nav class="wy-nav-top">
-        <i data-toggle="wy-nav-top" class="icon icon-reorder"></i>
-        <a href="/">pysoundanalyser</a>
+    <section data-toggle="wy-nav-shift" class="wy-nav-content-wrap"><nav class="wy-nav-top" aria-label="Mobile navigation menu" >
+          <i data-toggle="wy-nav-top" class="fa fa-bars"></i>
+          <a href="index.html">pysoundanalyser</a>
       </nav>
 
-
-      
       <div class="wy-nav-content">
         <div class="rst-content">
-          <ul class="wy-breadcrumbs">
-  <li><a href="index.html">Docs</a> &raquo;</li>
-  <li><a href="">User Interface</a></li>
-  
-</ul>
-<hr/>
-
-          
-  <div class="section" id="user-interface">
-<span id="sec-user-interface"></span><h1>User Interface<a class="headerlink" href="#user-interface" title="Permalink to this headline">¶</a></h1>
+          <div role="navigation" aria-label="Page navigation">
+  <ul class="wy-breadcrumbs">
+      <li><a href="index.html" class="icon icon-home" aria-label="Home"></a></li>
+      <li class="breadcrumb-item active">User Interface</li>
+      <li class="wy-breadcrumbs-aside">
+            <a href="_sources/user_interface.rst.txt" rel="nofollow"> View page source</a>
+      </li>
+  </ul>
+  <hr/>
+</div>
+          <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
+           <div itemprop="articleBody">
+             
+  <section id="user-interface">
+<span id="sec-user-interface"></span><h1>User Interface<a class="headerlink" href="#user-interface" title="Permalink to this heading"></a></h1>
 <ul>
-<li><p class="first"><strong>Load Sound</strong> The <code class="docutils literal"><span class="pre">Load</span> <span class="pre">Sound</span></code> button allows you to load a wav file into the program. Currently only 16 and 32 bit wav files with one or two channels are supported. Note that the entire wav file is loaded in memory, this is fine and fast for wav files of short durations (tens of seconds), but longer sound files are going to consume huge amounts of RAM and may even halt your computer. If you need to work on long sound files, please use other software, like audacity.</p>
+<li><p><strong>Load Sound</strong> The <code class="docutils literal notranslate"><span class="pre">Load</span> <span class="pre">Sound</span></code> button allows you to load a wav file into the program. Currently only 16 and 32 bit wav files with one or two channels are supported. Note that the entire wav file is loaded in memory, this is fine and fast for wav files of short durations (tens of seconds), but longer sound files are going to consume huge amounts of RAM and may even halt your computer. If you need to work on long sound files, please use other software, like audacity.</p>
 <ul class="simple">
-<li><strong>Save As</strong> The <code class="docutils literal"><span class="pre">Save</span> <span class="pre">As</span></code> button allows you to save PSA sound objects as wav files. Currently it is only possible to save sounds as 16 or 32 bit wav files with one or two channels. If you choose a mono (1-channel) format, and multiple PSA sound objects have been selected for saving, they will be summed together before saving. If you choose a stereo (2-channels) format, &#8220;right&#8221; and &#8220;left&#8221; PSA sound objects will be saved to their respective channels in the wav file; if multiple &#8220;right&#8221; or &#8220;left&#8221; PSA sound objects have been selected, they will be summed before saving.</li>
+<li><p><strong>Save As</strong> The <code class="docutils literal notranslate"><span class="pre">Save</span> <span class="pre">As</span></code> button allows you to save PSA sound objects as wav files. Currently it is only possible to save sounds as 16 or 32 bit wav files with one or two channels. If you choose a mono (1-channel) format, and multiple PSA sound objects have been selected for saving, they will be summed together before saving. If you choose a stereo (2-channels) format, “right” and “left” PSA sound objects will be saved to their respective channels in the wav file; if multiple “right” or “left” PSA sound objects have been selected, they will be summed before saving.</p></li>
 </ul>
 </li>
-<li><p class="first"><strong>Clone Sound</strong></p>
-</li>
-<li><p class="first"><strong>Concatenate</strong></p>
-</li>
-<li><p class="first"><strong>Cut</strong> The <code class="docutils literal"><span class="pre">Cut</span></code> button allows you to remove segments of a sound waveform. The starting and ending points of the segments to be cut off can be specified in seconds, milliseconds, or sample numbers. When working with sample numbers, note that PSA indexing works exactly like numpy indexing. Examples:</p>
-<div class="highlight-python"><div class="highlight"><pre><span></span><span class="gp">&gt;&gt;&gt; </span><span class="kn">import</span> <span class="nn">numpy</span> <span class="kn">as</span> <span class="nn">np</span> <span class="c1">#import numpy</span>
+<li><p><strong>Clone Sound</strong></p></li>
+<li><p><strong>Concatenate</strong></p></li>
+<li><p><strong>Cut</strong> The <code class="docutils literal notranslate"><span class="pre">Cut</span></code> button allows you to remove segments of a sound waveform. The starting and ending points of the segments to be cut off can be specified in seconds, milliseconds, or sample numbers. When working with sample numbers, note that PSA indexing works exactly like numpy indexing. Examples:</p>
+<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="gp">&gt;&gt;&gt; </span><span class="kn">import</span> <span class="nn">numpy</span> <span class="k">as</span> <span class="nn">np</span> <span class="c1">#import numpy</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="n">sig</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">arange</span><span class="p">(</span><span class="mi">10</span><span class="p">)</span> <span class="c1">#generate a 10-elements array</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="n">x</span><span class="p">[</span><span class="mi">0</span><span class="p">:</span><span class="mi">5</span><span class="p">]</span> <span class="c1">#Select the first five samples, indexing starts from 0</span>
 <span class="go">array([0, 1, 2, 3, 4])</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="n">sig</span><span class="p">[</span><span class="mi">7</span><span class="p">:</span><span class="mi">10</span><span class="p">]</span> <span class="c1">#select last 3 samples</span>
 <span class="go">array([7, 8, 9])</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="n">sig</span><span class="p">[</span><span class="mi">1</span><span class="p">:</span><span class="mi">3</span><span class="p">]</span> <span class="c1">#select the second and third sample</span>
 <span class="go">array([1, 2])</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="n">sig</span><span class="p">[</span><span class="mi">1</span><span class="p">:</span><span class="mi">2</span><span class="p">]</span> <span class="c1">#select the second sample</span>
 <span class="go">array([1])</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="n">sig</span><span class="p">[</span><span class="mi">1</span><span class="p">:</span><span class="mi">1</span><span class="p">]</span> <span class="c1">#note that if the start and end point are the same nothing is selected</span>
 <span class="go">array([], dtype=int64)</span>
 </pre></div>
 </div>
 </li>
-<li><p class="first"><strong>Play</strong> The <code class="docutils literal"><span class="pre">Play</span></code> button allows playback of the currently selected sound.</p>
-</li>
-<li><p class="first"><strong>Plot Waveform</strong> The <code class="docutils literal"><span class="pre">Plot</span> <span class="pre">Wavform</span></code> button allows you to plot the waveform of the currently selected sound.</p>
-</li>
-<li><p class="first"><strong>Spectrum</strong> Plot the spectrum of the currently selected sound.</p>
-</li>
-<li><p class="first"><strong>Spectrogram</strong> Plot the spectrogram of the currently selected sound.</p>
-</li>
-<li><p class="first"><strong>Autocorrelation</strong> Plot the autocorrelation function of the currently selected sound.</p>
-</li>
-<li><p class="first"><strong>Autocorrelogram</strong> Plot the autocorrelogram of the currently selected sound.</p>
-</li>
-<li><p class="first"><strong>Level Difference</strong> Show the difference in level between two selected sounds.</p>
-</li>
-<li><p class="first"><strong>Scale</strong> Change the level of the currently selected sound.</p>
-</li>
-<li><p class="first"><strong>Resample</strong> Resample the currently selected sound.</p>
-</li>
-<li><p class="first"><strong>Rename</strong> Rename the currently selected sound.</p>
-</li>
-<li><p class="first"><strong>Remove</strong> Remove the currently selected sound from the workspace.</p>
-</li>
-<li><p class="first"><strong>Remove All</strong> Remove all sounds from the workspace.</p>
-</li>
+<li><p><strong>Play</strong> The <code class="docutils literal notranslate"><span class="pre">Play</span></code> button allows playback of the currently selected sound.</p></li>
+<li><p><strong>Plot Waveform</strong> The <code class="docutils literal notranslate"><span class="pre">Plot</span> <span class="pre">Wavform</span></code> button allows you to plot the waveform of the currently selected sound.</p></li>
+<li><p><strong>Spectrum</strong> Plot the spectrum of the currently selected sound.</p></li>
+<li><p><strong>Spectrogram</strong> Plot the spectrogram of the currently selected sound.</p></li>
+<li><p><strong>Autocorrelation</strong> Plot the autocorrelation function of the currently selected sound.</p></li>
+<li><p><strong>Autocorrelogram</strong> Plot the autocorrelogram of the currently selected sound.</p></li>
+<li><p><strong>Level Difference</strong> Show the difference in level between two selected sounds.</p></li>
+<li><p><strong>Scale</strong> Change the level of the currently selected sound.</p></li>
+<li><p><strong>Resample</strong> Resample the currently selected sound.</p></li>
+<li><p><strong>Rename</strong> Rename the currently selected sound.</p></li>
+<li><p><strong>Remove</strong> Remove the currently selected sound from the workspace.</p></li>
+<li><p><strong>Remove All</strong> Remove all sounds from the workspace.</p></li>
 </ul>
-</div>
+</section>
 
 
-          <footer>
-  
-    <div class="rst-footer-buttons">
-      
-      
-        <a href="installation.html" class="btn btn-neutral" title="Installation"><span class="icon icon-circle-arrow-left"></span> Previous</a>
-      
+           </div>
+          </div>
+          <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
+        <a href="installation.html" class="btn btn-neutral float-left" title="Installation" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
     </div>
-  
 
   <hr/>
 
-  <p>
-      &copy; Copyright 2010-2017, Samuele Carcagno.
-  </p>
+  <div role="contentinfo">
+    <p>&#169; Copyright 2010-2023, Samuele Carcagno.</p>
+  </div>
+
+  Built with <a href="https://www.sphinx-doc.org/">Sphinx</a> using a
+    <a href="https://github.com/readthedocs/sphinx_rtd_theme">theme</a>
+    provided by <a href="https://readthedocs.org">Read the Docs</a>.
+   
 
-  <a href="https://www.github.com/snide/sphinx_rtd_theme">Sphinx theme</a> provided by <a href="http://readthedocs.org">Read the Docs</a>
 </footer>
         </div>
       </div>
-
     </section>
-
   </div>
-  
+  <script>
+      jQuery(function () {
+          SphinxRtdTheme.Navigation.enable(true);
+      });
+  </script> 
 
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,45 +1,39 @@
 
 
 
 
 
-
-
-
 pysoundanalyser
 [q                   ]
+Contents:
     * What_is_pysoundanalyser?
     * Installation
-          o Installation_on_Linux
-          o Installation_on_Windows
-          o Installation_on_the_Mac
-          o Installation_from_source
     * User_Interface
-      pysoundanalyser
-    * Docs »
+   pysoundanalyser
     * User Interface
+    * View_page_source
 ===============================================================================
-****** User InterfaceÂ¶ ******
+****** User Interfaceï ******
     * Load Sound The Load Sound button allows you to load a wav file into the
       program. Currently only 16 and 32 bit wav files with one or two channels
       are supported. Note that the entire wav file is loaded in memory, this is
       fine and fast for wav files of short durations (tens of seconds), but
       longer sound files are going to consume huge amounts of RAM and may even
       halt your computer. If you need to work on long sound files, please use
       other software, like audacity.
           o Save As The Save As button allows you to save PSA sound objects as
             wav files. Currently it is only possible to save sounds as 16 or 32
             bit wav files with one or two channels. If you choose a mono (1-
             channel) format, and multiple PSA sound objects have been selected
             for saving, they will be summed together before saving. If you
-            choose a stereo (2-channels) format, “right” and “left” PSA sound
-            objects will be saved to their respective channels in the wav file;
-            if multiple “right” or “left” PSA sound objects have been selected,
-            they will be summed before saving.
+            choose a stereo (2-channels) format, ârightâ and âleftâ PSA
+            sound objects will be saved to their respective channels in the wav
+            file; if multiple ârightâ or âleftâ PSA sound objects have
+            been selected, they will be summed before saving.
     * Clone Sound
     * Concatenate
     * Cut The Cut button allows you to remove segments of a sound waveform. The
       starting and ending points of the segments to be cut off can be specified
       in seconds, milliseconds, or sample numbers. When working with sample
       numbers, note that PSA indexing works exactly like numpy indexing.
       Examples:
@@ -69,9 +63,9 @@
     * Scale Change the level of the currently selected sound.
     * Resample Resample the currently selected sound.
     * Rename Rename the currently selected sound.
     * Remove Remove the currently selected sound from the workspace.
     * Remove All Remove all sounds from the workspace.
 Previous
 ===============================================================================
-© Copyright 2010-2017, Samuele Carcagno.
-Sphinx_theme provided by Read_the_Docs
+© Copyright 2010-2023, Samuele Carcagno.
+Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/doc/installation.rst` & `pysoundanalyser-0.3.2/pysoundanalyser/doc/_build/html/_sources/installation.rst.txt`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/doc/intro.rst` & `pysoundanalyser-0.3.2/pysoundanalyser/doc/intro.rst`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/doc/user_interface.rst` & `pysoundanalyser-0.3.2/pysoundanalyser/doc/user_interface.rst`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/global_parameters.py` & `pysoundanalyser-0.3.2/pysoundanalyser/global_parameters.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/qrc_resources.py` & `pysoundanalyser-0.3.2/pysoundanalyser/qrc_resources.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/random_id.py` & `pysoundanalyser-0.3.2/pysoundanalyser/random_id.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/sndlib.py` & `pysoundanalyser-0.3.2/pysoundanalyser/sndlib.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/threaded_plotters.py` & `pysoundanalyser-0.3.2/pysoundanalyser/threaded_plotters.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/utilities_open_manual.py` & `pysoundanalyser-0.3.2/pysoundanalyser/utilities_open_manual.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/utility_functions.py` & `pysoundanalyser-0.3.2/pysoundanalyser/utility_functions.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/wavpy.py` & `pysoundanalyser-0.3.2/pysoundanalyser/wavpy.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/wavpy_sndf.py` & `pysoundanalyser-0.3.2/pysoundanalyser/wavpy_sndf.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/win_acf_plot.py` & `pysoundanalyser-0.3.2/pysoundanalyser/win_acf_plot.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/win_autocorrelogram_plot.py` & `pysoundanalyser-0.3.2/pysoundanalyser/win_autocorrelogram_plot.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/win_generic_plot.py` & `pysoundanalyser-0.3.2/pysoundanalyser/win_generic_plot.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/win_spectrogram_plot.py` & `pysoundanalyser-0.3.2/pysoundanalyser/win_spectrogram_plot.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/win_spectrum_plot.py` & `pysoundanalyser-0.3.2/pysoundanalyser/win_spectrum_plot.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser/win_waveform_plot.py` & `pysoundanalyser-0.3.2/pysoundanalyser/win_waveform_plot.py`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/pysoundanalyser.egg-info/PKG-INFO` & `pysoundanalyser-0.3.2/pysoundanalyser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysoundanalyser
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python program for visualizing short sounds (waveform, spectrum, etc...)
 Author-email: Samuele Carcagno <sam.carcagno@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pysoundanalyser-0.3.1/resources.qrc` & `pysoundanalyser-0.3.2/resources.qrc`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/translations/pysoundanalyser_it.qm` & `pysoundanalyser-0.3.2/translations/pysoundanalyser_it.qm`

 * *Files identical despite different names*

### Comparing `pysoundanalyser-0.3.1/translations/pysoundanalyser_it_IT.qm` & `pysoundanalyser-0.3.2/translations/pysoundanalyser_it_IT.qm`

 * *Files identical despite different names*

