# Comparing `tmp/petljadoc-1.3.1.tar.gz` & `tmp/petljadoc-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petljadoc-1.3.1.tar", last modified: Mon Apr 10 05:44:09 2023, max compression
+gzip compressed data, was "petljadoc-1.3.3.tar", last modified: Mon Jun  5 12:58:57 2023, max compression
```

## Comparing `petljadoc-1.3.1.tar` & `petljadoc-1.3.3.tar`

### file list

```diff
@@ -1,969 +1,969 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:09.215963 petljadoc-1.3.1/
--rw-rw-rw-   0        0        0     1084 2019-09-29 18:46:11.000000 petljadoc-1.3.1/LICENSE
--rw-rw-rw-   0        0        0      475 2022-11-20 11:14:54.000000 petljadoc-1.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2389 2023-04-10 05:44:09.215963 petljadoc-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1803 2022-11-06 13:07:30.000000 petljadoc-1.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.727090 petljadoc-1.3.1/petljadoc/
--rw-rw-rw-   0        0        0       67 2023-04-10 05:07:00.000000 petljadoc-1.3.1/petljadoc/__init__.py
--rw-rw-rw-   0        0        0       39 2020-12-07 14:32:36.000000 petljadoc-1.3.1/petljadoc/__main__.py
--rw-rw-rw-   0        0        0    43045 2023-03-06 12:31:02.000000 petljadoc-1.3.1/petljadoc/cli.py
--rw-rw-rw-   0        0        0    15820 2023-03-06 12:31:02.000000 petljadoc-1.3.1/petljadoc/course.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.546086 petljadoc-1.3.1/petljadoc/nb-templates/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.763088 petljadoc-1.3.1/petljadoc/nb-templates/classic2/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.864437 petljadoc-1.3.1/petljadoc/nb-templates/classic2/base/
--rw-rw-rw-   0        0        0     7752 2022-11-06 13:07:30.000000 petljadoc-1.3.1/petljadoc/nb-templates/classic2/base/base.html.j2
--rw-rw-rw-   0        0        0      220 2022-11-06 13:07:30.000000 petljadoc-1.3.1/petljadoc/nb-templates/classic2/base/celltags.j2
--rw-rw-rw-   0        0        0     1634 2022-11-06 13:07:30.000000 petljadoc-1.3.1/petljadoc/nb-templates/classic2/base/display_priority.j2
--rw-rw-rw-   0        0        0      993 2022-11-06 13:07:30.000000 petljadoc-1.3.1/petljadoc/nb-templates/classic2/base/jupyter_widgets.html.j2
--rw-rw-rw-   0        0        0     1386 2022-11-06 13:07:30.000000 petljadoc-1.3.1/petljadoc/nb-templates/classic2/base/mathjax.html.j2
--rw-rw-rw-   0        0        0     6340 2022-11-06 13:07:30.000000 petljadoc-1.3.1/petljadoc/nb-templates/classic2/base/null.j2
--rw-rw-rw-   0        0        0      401 2022-11-06 13:07:30.000000 petljadoc-1.3.1/petljadoc/nb-templates/classic2/index.html.j2
--rw-rw-rw-   0        0        0    40964 2023-03-06 12:31:02.000000 petljadoc-1.3.1/petljadoc/package.py
--rw-rw-rw-   0        0        0     2282 2022-12-02 13:00:34.000000 petljadoc-1.3.1/petljadoc/petlja_builder.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.548086 petljadoc-1.3.1/petljadoc/project-templates/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.921611 petljadoc-1.3.1/petljadoc/project-templates/course/
--rw-rw-rw-   0        0        0      142 2022-12-02 13:00:34.000000 petljadoc-1.3.1/petljadoc/project-templates/course/.t.gitignore
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.922609 petljadoc-1.3.1/petljadoc/project-templates/course/_images/
--rw-rw-rw-   0        0        0        1 2020-11-30 16:13:38.000000 petljadoc-1.3.1/petljadoc/project-templates/course/_images/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.923612 petljadoc-1.3.1/petljadoc/project-templates/course/_includes/
--rw-rw-rw-   0        0        0        1 2020-11-30 16:13:38.000000 petljadoc-1.3.1/petljadoc/project-templates/course/_includes/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.943872 petljadoc-1.3.1/petljadoc/project-templates/course/_sources/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.971207 petljadoc-1.3.1/petljadoc/project-templates/course/_sources/1_Lesson/
--rw-rw-rw-   0        0        0     2096 2020-11-30 16:13:38.000000 petljadoc-1.3.1/petljadoc/project-templates/course/_sources/1_Lesson/intro.rst
--rw-rw-rw-   0        0        0     1564 2022-11-06 13:07:30.000000 petljadoc-1.3.1/petljadoc/project-templates/course/_sources/1_Lesson/quiz.rst
--rw-rw-rw-   0        0        0     1368 2022-11-06 13:07:30.000000 petljadoc-1.3.1/petljadoc/project-templates/course/_sources/index.t.yaml
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.972208 petljadoc-1.3.1/petljadoc/project-templates/course/_static/
--rw-rw-rw-   0        0        0        1 2020-11-30 16:13:38.000000 petljadoc-1.3.1/petljadoc/project-templates/course/_static/.gitkeep
--rw-rw-rw-   0        0        0       75 2023-04-10 05:07:00.000000 petljadoc-1.3.1/petljadoc/project-templates/course/conf-petljadoc.t.json
--rw-rw-rw-   0        0        0     6291 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/project-templates/course/conf.t.py
--rw-rw-rw-   0        0        0       33 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/project-templates/course/package-conf.json
--rw-rw-rw-   0        0        0      777 2020-12-09 14:48:07.000000 petljadoc-1.3.1/petljadoc/project-templates/course/pavement.t.py
--rw-rw-rw-   0        0        0      110 2022-11-06 13:07:30.000000 petljadoc-1.3.1/petljadoc/project-templates/course/template_settings.t.json
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.004165 petljadoc-1.3.1/petljadoc/project-templates/runestone/
--rw-rw-rw-   0        0        0       56 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/.t.gitignore
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.005163 petljadoc-1.3.1/petljadoc/project-templates/runestone/_images/
--rw-rw-rw-   0        0        0        1 2020-11-30 16:13:38.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/_images/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.005163 petljadoc-1.3.1/petljadoc/project-templates/runestone/_includes/
--rw-rw-rw-   0        0        0        1 2020-11-30 16:13:38.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/_includes/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.033181 petljadoc-1.3.1/petljadoc/project-templates/runestone/_sources/
--rw-rw-rw-   0        0        0       90 2022-11-06 13:07:30.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/_sources/index-item.t.md
--rw-rw-rw-   0        0        0     3337 2020-11-30 16:13:38.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/_sources/index.rst
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.128639 petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/
--rw-rw-rw-   0        0        0        0 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/.gitignore
--rw-rw-rw-   0        0        0    92708 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/activecodethumb.png
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.237152 petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/audio/
--rw-rw-rw-   0        0        0    87168 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line01.mp3
--rw-rw-rw-   0        0        0   273068 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line01.wav
--rw-rw-rw-   0        0        0   115328 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line02.mp3
--rw-rw-rw-   0        0        0   361772 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line02.wav
--rw-rw-rw-   0        0        0   310985 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line03.mp3
--rw-rw-rw-   0        0        0   978092 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line03.wav
--rw-rw-rw-   0        0        0    23942 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/clock.png
--rw-rw-rw-   0        0        0     4497 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/close.png
--rw-rw-rw-   0        0        0    16165 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/first.png
--rw-rw-rw-   0        0        0    15899 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/last.png
--rw-rw-rw-   0        0        0    15743 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/next.png
--rw-rw-rw-   0        0        0    15344 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/pause.png
--rw-rw-rw-   0        0        0    15719 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/prev.png
--rw-rw-rw-   0        0        0       75 2023-04-10 05:07:00.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/conf-petljadoc.t.json
--rw-rw-rw-   0        0        0    10633 2022-11-06 13:07:30.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/conf.t.py
--rw-rw-rw-   0        0        0      770 2020-12-09 14:48:07.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/pavement.t.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.251002 petljadoc-1.3.1/petljadoc/runestone_ext/
--rw-rw-rw-   0        0        0     1782 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/runestone_ext/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.273348 petljadoc-1.3.1/petljadoc/runestone_ext/associations/
--rw-rw-rw-   0        0        0       29 2022-11-06 13:07:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/associations/__init__.py
--rw-rw-rw-   0        0        0     4629 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/runestone_ext/associations/associations.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.274361 petljadoc-1.3.1/petljadoc/runestone_ext/associations/css/
--rw-rw-rw-   0        0        0     3204 2022-11-06 13:07:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/associations/css/associations.css
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.278361 petljadoc-1.3.1/petljadoc/runestone_ext/associations/js/
--rw-rw-rw-   0        0        0      147 2022-11-06 13:07:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/associations/js/associations-i18n.en.js
--rw-rw-rw-   0        0        0      164 2022-11-06 13:07:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/associations/js/associations-i18n.sr-Cyrl.js
--rw-rw-rw-   0        0        0      144 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/associations/js/associations-i18n.sr-Latn.js
--rw-rw-rw-   0        0        0      159 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/associations/js/associations-i18n.sr.js
--rw-rw-rw-   0        0        0     5682 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/associations/js/associations.js
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.308389 petljadoc-1.3.1/petljadoc/runestone_ext/audio/
--rw-rw-rw-   0        0        0       20 2019-12-21 09:53:52.000000 petljadoc-1.3.1/petljadoc/runestone_ext/audio/__init__.py
--rw-rw-rw-   0        0        0     1297 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/audio/audio.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.309392 petljadoc-1.3.1/petljadoc/runestone_ext/audio/test/
--rw-rw-rw-   0        0        0        0 2019-12-21 09:53:52.000000 petljadoc-1.3.1/petljadoc/runestone_ext/audio/test/sphinx-enki-info.txt
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.326387 petljadoc-1.3.1/petljadoc/runestone_ext/blockly/
--rw-rw-rw-   0        0        0       27 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockly/__init__.py
--rw-rw-rw-   0        0        0     6966 2023-04-07 12:08:56.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockly/blocklykarel.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.326387 petljadoc-1.3.1/petljadoc/runestone_ext/blockly/css/
--rw-rw-rw-   0        0        0     2065 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockly/css/karelBlockly.css
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.332868 petljadoc-1.3.1/petljadoc/runestone_ext/blockly/js/
--rw-rw-rw-   0        0        0    80180 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockly/js/acorn_interpreter.js
--rw-rw-rw-   0        0        0   929342 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockly/js/blockly_compressed.js
--rw-rw-rw-   0        0        0    90975 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockly/js/blocks_compressed.js
--rw-rw-rw-   0        0        0    46593 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockly/js/javascript_compressed.js
--rw-rw-rw-   0        0        0    18815 2023-04-07 22:59:40.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockly/js/karelBlockly.js
--rw-rw-rw-   0        0        0    11952 2023-04-06 17:23:38.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockly/js/karelBlocks.js
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.334878 petljadoc-1.3.1/petljadoc/runestone_ext/blockly/js/msg/
--rw-rw-rw-   0        0        0    32475 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockly/js/msg/en.js
--rw-rw-rw-   0        0        0    40621 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockly/js/msg/sr.js
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.363149 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/
--rw-rw-rw-   0        0        0       25 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/__init__.py
--rw-rw-rw-   0        0        0     1299 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/blockpylib.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.382745 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.610664 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockly/
--rw-rw-rw-   0        0        0   683169 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockly/blockly_compressed.js
--rw-rw-rw-   0        0        0    92505 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockly/blocks_compressed.js
--rw-rw-rw-   0        0        0    61781 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockly/msg-sr.js
--rw-rw-rw-   0        0        0    40010 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockly/python_compressed.js
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.809358 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/
--rw-rw-rw-   0        0        0    35053 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/abstract_interpreter.js
--rw-rw-rw-   0        0        0     6384 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/abstract_interpreter_definitions.js
--rw-rw-rw-   0        0        0     3736 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/ast_node_visitor.js
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.068357 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/
--rw-rw-rw-   0        0        0     1888 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/class.js
--rw-rw-rw-   0        0        0     2178 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/comment.js
--rw-rw-rw-   0        0        0     1116 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/comprehensions.js
--rw-rw-rw-   0        0        0      522 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/decorator.js
--rw-rw-rw-   0        0        0     3777 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/dict.js
--rw-rw-rw-   0        0        0     7891 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/if.js
--rw-rw-rw-   0        0        0     1922 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/io.js
--rw-rw-rw-   0        0        0    12589 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/lists.js
--rw-rw-rw-   0        0        0     1799 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/loops.js
--rw-rw-rw-   0        0        0     8787 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/parking.js
--rw-rw-rw-   0        0        0      609 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/plots.js
--rw-rw-rw-   0        0        0     1718 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/sets.js
--rw-rw-rw-   0        0        0     1263 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/text.js
--rw-rw-rw-   0        0        0     1831 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/tuple.js
--rw-rw-rw-   0        0        0     6969 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/turtles.js
--rw-rw-rw-   0        0        0     4701 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/imported.js
--rw-rw-rw-   0        0        0     7255 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/python_errors.js
--rw-rw-rw-   0        0        0    51813 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/python_to_blockly.js
--rw-rw-rw-   0        0        0    59429 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/pytifa.js
--rw-rw-rw-   0        0        0     8165 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/utilities.js
--rw-rw-rw-   0        0        0     9503 2022-12-02 13:00:34.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy-modal.js
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.558088 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/test/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.558088 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/test/_templates/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.559088 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.559088 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.089359 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.560088 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.103361 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/
--rw-rw-rw-   0        0        0    97346 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.133360 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/
--rw-rw-rw-   0        0        0    27731 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/bootstrap.min.js
--rw-rw-rw-   0        0        0     3776 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-sphinx.js
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.152363 petljadoc-1.3.1/petljadoc/runestone_ext/dbDirective/
--rw-rw-rw-   0        0        0       28 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/dbDirective/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.154359 petljadoc-1.3.1/petljadoc/runestone_ext/dbDirective/css/
--rw-rw-rw-   0        0        0     2423 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/dbDirective/css/dbDirective.css
--rw-rw-rw-   0        0        0     4636 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/runestone_ext/dbDirective/dbDirective.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.168357 petljadoc-1.3.1/petljadoc/runestone_ext/dbDirective/js/
--rw-rw-rw-   0        0        0    16828 2022-12-02 13:00:34.000000 petljadoc-1.3.1/petljadoc/runestone_ext/dbDirective/js/dbDirective.js
--rw-rw-rw-   0        0        0    48501 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/dbDirective/js/sql.js
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.189361 petljadoc-1.3.1/petljadoc/runestone_ext/editor/
--rw-rw-rw-   0        0        0       21 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/editor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.190360 petljadoc-1.3.1/petljadoc/runestone_ext/editor/css/
--rw-rw-rw-   0        0        0     1771 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/editor/css/editor.css
--rw-rw-rw-   0        0        0     5287 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/runestone_ext/editor/editor.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.196359 petljadoc-1.3.1/petljadoc/runestone_ext/editor/js/
--rw-rw-rw-   0        0        0       72 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/editor/js/editor-i18n.en.js
--rw-rw-rw-   0        0        0      102 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/editor/js/editor-i18n.sr-Cyrl.js
--rw-rw-rw-   0        0        0       88 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/editor/js/editor-i18n.sr-Latn.js
--rw-rw-rw-   0        0        0       97 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/editor/js/editor-i18n.sr.js
--rw-rw-rw-   0        0        0    10712 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/editor/js/editor.js
--rw-rw-rw-   0        0        0   385745 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/editor/js/jszip.js
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.231359 petljadoc-1.3.1/petljadoc/runestone_ext/gallery/
--rw-rw-rw-   0        0        0       24 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/gallery/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.232359 petljadoc-1.3.1/petljadoc/runestone_ext/gallery/css/
--rw-rw-rw-   0        0        0      589 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/gallery/css/gallery.css
--rw-rw-rw-   0        0        0     4012 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/runestone_ext/gallery/gallery.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.233360 petljadoc-1.3.1/petljadoc/runestone_ext/gallery/js/
--rw-rw-rw-   0        0        0     2096 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/gallery/js/gallery.js
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.245359 petljadoc-1.3.1/petljadoc/runestone_ext/karel/
--rw-rw-rw-   0        0        0       20 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/karel/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.246373 petljadoc-1.3.1/petljadoc/runestone_ext/karel/css/
--rw-rw-rw-   0        0        0     1080 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/karel/css/karel.css
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.255090 petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/
--rw-rw-rw-   0        0        0      438 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/karel-i18n.en.js
--rw-rw-rw-   0        0        0      557 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/karel-i18n.sr-Cyrl.js
--rw-rw-rw-   0        0        0      560 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/karel-i18n.sr.js
--rw-rw-rw-   0        0        0     3676 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/karel.js
--rw-rw-rw-   0        0        0     1689 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/karelChat.js
--rw-rw-rw-   0        0        0     1455 2023-04-07 12:31:14.000000 petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/karelCorner.js
--rw-rw-rw-   0        0        0     6683 2022-12-02 13:00:34.000000 petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/karelRobot.js
--rw-rw-rw-   0        0        0    14648 2023-04-07 11:34:03.000000 petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/karelRobotDrawer.js
--rw-rw-rw-   0        0        0     9995 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/karelUI.js
--rw-rw-rw-   0        0        0     5047 2023-04-07 12:30:39.000000 petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/karelWorld.js
--rw-rw-rw-   0        0        0     5241 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/runestone_ext/karel/karel.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.256102 petljadoc-1.3.1/petljadoc/runestone_ext/karel/test/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.566085 petljadoc-1.3.1/petljadoc/runestone_ext/karel/test/_templates/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.566085 petljadoc-1.3.1/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.567086 petljadoc-1.3.1/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.266226 petljadoc-1.3.1/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.570087 petljadoc-1.3.1/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.286959 petljadoc-1.3.1/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/
--rw-rw-rw-   0        0        0    97346 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.316960 petljadoc-1.3.1/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/
--rw-rw-rw-   0        0        0    27731 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/bootstrap.min.js
--rw-rw-rw-   0        0        0     3776 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-sphinx.js
--rw-rw-rw-   0        0        0        0 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/karel/test/sphinx-enki-info.txt
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.344080 petljadoc-1.3.1/petljadoc/runestone_ext/nimgame/
--rw-rw-rw-   0        0        0       24 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/nimgame/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.345079 petljadoc-1.3.1/petljadoc/runestone_ext/nimgame/css/
--rw-rw-rw-   0        0        0     3729 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/nimgame/css/nimgame.css
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.352079 petljadoc-1.3.1/petljadoc/runestone_ext/nimgame/js/
--rw-rw-rw-   0        0        0      406 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/nimgame/js/nimgame-i18n.en.js
--rw-rw-rw-   0        0        0      565 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/nimgame/js/nimgame-i18n.sr-Cyrl.js
--rw-rw-rw-   0        0        0      455 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/nimgame/js/nimgame-i18n.sr-Latn.js
--rw-rw-rw-   0        0        0      560 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/nimgame/js/nimgame-i18n.sr.js
--rw-rw-rw-   0        0        0    13205 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/nimgame/js/nimgame.js
--rw-rw-rw-   0        0        0     4655 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/runestone_ext/nimgame/nimgame.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.369833 petljadoc-1.3.1/petljadoc/runestone_ext/notes/
--rw-rw-rw-   0        0        0       20 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.370845 petljadoc-1.3.1/petljadoc/runestone_ext/notes/css/
--rw-rw-rw-   0        0        0     3334 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/css/notes.css
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.371844 petljadoc-1.3.1/petljadoc/runestone_ext/notes/js/
--rw-rw-rw-   0        0        0     1101 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/js/notes.js
--rw-rw-rw-   0        0        0     5293 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/notes.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.371844 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.573087 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/_templates/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.574087 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.574087 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.381845 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.575086 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.397940 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/
--rw-rw-rw-   0        0        0    97346 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.416940 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/
--rw-rw-rw-   0        0        0    27731 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/bootstrap.min.js
--rw-rw-rw-   0        0        0     3776 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-sphinx.js
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.576087 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.423941 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.428939 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_sources/
--rw-rw-rw-   0        0        0      265 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_sources/index.rst.txt
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:02.080782 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/
--rw-rw-rw-   0        0        0     6355 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/Blob.js
--rw-rw-rw-   0        0        0     5120 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/FileSaver.min.js
--rw-rw-rw-   0        0        0     1511 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/LICENSE.txt
--rw-rw-rw-   0        0        0     3439 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/accessibility.css
--rw-rw-rw-   0        0        0     3445 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/accessibilitydarkest.css
--rw-rw-rw-   0        0        0     2669 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/accessibilitylight.css
--rw-rw-rw-   0        0        0     9490 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/activecode-i18n.en.js
--rw-rw-rw-   0        0        0    14677 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/activecode-i18n.sr-Cyrl.js
--rw-rw-rw-   0        0        0     2096 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/activecode.css
--rw-rw-rw-   0        0        0   103165 2020-02-25 19:14:39.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/activecode.js
--rw-rw-rw-   0        0        0     3903 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/animationbase.js
--rw-rw-rw-   0        0        0    10912 2020-03-17 13:54:33.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/basic.css
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:02.261777 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly/
--rw-rw-rw-   0        0        0   683169 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly/blockly_compressed.js
--rw-rw-rw-   0        0        0    92505 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly/blocks_compressed.js
--rw-rw-rw-   0        0        0    61781 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly/msg-sr.js
--rw-rw-rw-   0        0        0    40010 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly/python_compressed.js
--rw-rw-rw-   0        0        0   471577 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly_compressed.js
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:02.397022 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/
--rw-rw-rw-   0        0        0    35053 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/abstract_interpreter.js
--rw-rw-rw-   0        0        0     6384 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/abstract_interpreter_definitions.js
--rw-rw-rw-   0        0        0     3736 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/ast_node_visitor.js
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:02.570529 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/
--rw-rw-rw-   0        0        0     1888 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/class.js
--rw-rw-rw-   0        0        0     2178 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/comment.js
--rw-rw-rw-   0        0        0     1116 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/comprehensions.js
--rw-rw-rw-   0        0        0      522 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/decorator.js
--rw-rw-rw-   0        0        0     3777 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/dict.js
--rw-rw-rw-   0        0        0     7891 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/if.js
--rw-rw-rw-   0        0        0     1922 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/io.js
--rw-rw-rw-   0        0        0    12589 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/lists.js
--rw-rw-rw-   0        0        0     1799 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/loops.js
--rw-rw-rw-   0        0        0     8787 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/parking.js
--rw-rw-rw-   0        0        0      609 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/plots.js
--rw-rw-rw-   0        0        0     1718 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/sets.js
--rw-rw-rw-   0        0        0     1263 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/text.js
--rw-rw-rw-   0        0        0     1831 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/tuple.js
--rw-rw-rw-   0        0        0     6969 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/turtles.js
--rw-rw-rw-   0        0        0     4701 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/imported.js
--rw-rw-rw-   0        0        0     7255 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/python_errors.js
--rw-rw-rw-   0        0        0    51813 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/python_to_blockly.js
--rw-rw-rw-   0        0        0    59429 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/pytifa.js
--rw-rw-rw-   0        0        0     8165 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/utilities.js
--rw-rw-rw-   0        0        0     9298 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy-modal.js
--rw-rw-rw-   0        0        0    55934 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blocks_compressed.js
--rw-rw-rw-   0        0        0    10606 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bookfuncs.js
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.579086 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-4.0.0-dist/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:02.588321 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-4.0.0-dist/css/
--rw-rw-rw-   0        0        0   144838 2022-02-03 12:41:00.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-4.0.0-dist/css/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:02.662959 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-4.0.0-dist/js/
--rw-rw-rw-   0        0        0    67698 2022-02-03 12:41:15.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-4.0.0-dist/js/bootstrap.bundle.min.js
--rw-rw-rw-   0        0        0    48907 2022-02-03 12:41:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-4.0.0-dist/js/bootstrap.min.js
--rw-rw-rw-   0        0        0      425 2020-03-17 13:54:33.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-sphinx.css
--rw-rw-rw-   0        0        0     3776 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-sphinx.js
--rw-rw-rw-   0        0        0    97348 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap.min.css
--rw-rw-rw-   0        0        0     1123 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/clickable.css
--rw-rw-rw-   0        0        0    16404 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/clickable.js
--rw-rw-rw-   0        0        0    18265 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/clike.js
--rw-rw-rw-   0        0        0     2037 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/codelens.js
--rw-rw-rw-   0        0        0     7507 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/codemirror.css
--rw-rw-rw-   0        0        0   320980 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/codemirror.js
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:02.688962 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/css/
--rw-rw-rw-   0        0        0    31004 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/css/font-awesome.min.css
--rw-rw-rw-   0        0        0    32373 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/css.js
--rw-rw-rw-   0        0        0   111549 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/d3.v2.min.js
--rw-rw-rw-   0        0        0       95 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/datafile.css
--rw-rw-rw-   0        0        0     3000 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/datafile.js
--rw-rw-rw-   0        0        0    19241 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/diff_match_patch.js
--rw-rw-rw-   0        0        0     6868 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/doctools.js
--rw-rw-rw-   0        0        0      306 2020-03-17 13:54:33.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/documentation_options.js
--rw-rw-rw-   0        0        0      310 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/dragndrop-i18n.en.js
--rw-rw-rw-   0        0        0      394 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/dragndrop-i18n.sr-Cyrl.js
--rw-rw-rw-   0        0        0     1480 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/dragndrop.css
--rw-rw-rw-   0        0        0    18311 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/dragndrop.js
--rw-rw-rw-   0        0        0     1756 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/external.css
--rw-rw-rw-   0        0        0      130 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/fitb-i18n.en.js
--rw-rw-rw-   0        0        0      147 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/fitb-i18n.sr-Cyrl.js
--rw-rw-rw-   0        0        0      182 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/fitb.css
--rw-rw-rw-   0        0        0    13759 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/fitb.js
--rw-rw-rw-   0        0        0   127331 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/flatly.min.css
--rw-rw-rw-   0        0        0    21378 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/guiders-1.3.0.css
--rw-rw-rw-   0        0        0    20664 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/guiders-1.3.0.js
--rw-rw-rw-   0        0        0     5108 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/htmlmixed.js
--rw-rw-rw-   0        0        0    24396 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/javascript.js
--rw-rw-rw-   0        0        0    41074 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/javascript_compressed.js
--rw-rw-rw-   0        0        0   268039 2019-03-09 15:07:37.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery-3.2.1.js
--rw-rw-rw-   0        0        0      204 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery-fix.js
--rw-rw-rw-   0        0        0     7200 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery-migrate-1.2.1.min.js
--rw-rw-rw-   0        0        0    26010 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery-ui-1.10.3.custom.min.css
--rw-rw-rw-   0        0        0   217071 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery-ui-1.10.3.custom.min.js
--rw-rw-rw-   0        0        0     4255 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.ba-bbq.min.js
--rw-rw-rw-   0        0        0     1418 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.highlight.js
--rw-rw-rw-   0        0        0     1996 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.hotkey.js
--rw-rw-rw-   0        0        0     8182 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.idle-timer.js
--rw-rw-rw-   0        0        0    93069 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.js
--rw-rw-rw-   0        0        0   120545 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.jsPlumb-1.3.10-all-min.js
--rw-rw-rw-   0        0        0    40914 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.tablesorter.js
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:02.815307 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/
--rw-rw-rw-   0        0        0    13334 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/CLDRPluralRuleParser.js
--rw-rw-rw-   0        0        0    13513 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.emitter.bidi.js
--rw-rw-rw-   0        0        0     5561 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.emitter.js
--rw-rw-rw-   0        0        0     4261 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.fallbacks.js
--rw-rw-rw-   0        0        0     9027 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.js
--rw-rw-rw-   0        0        0    12427 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.language.js
--rw-rw-rw-   0        0        0     3749 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.messagestore.js
--rw-rw-rw-   0        0        0     8483 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.parser.js
--rw-rw-rw-   0        0        0      380 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karel-i18n.en.js
--rw-rw-rw-   0        0        0      484 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karel-i18n.sr-Cyrl.js
--rw-rw-rw-   0        0        0      984 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karel.css
--rw-rw-rw-   0        0        0     3676 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karel.js
--rw-rw-rw-   0        0        0     1105 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelCorner.js
--rw-rw-rw-   0        0        0     6290 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelRobot.js
--rw-rw-rw-   0        0        0    12016 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelRobotDrawer.js
--rw-rw-rw-   0        0        0     9995 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelUI.js
--rw-rw-rw-   0        0        0     4647 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelWorld.js
--rw-rw-rw-   0        0        0    10847 2020-03-17 13:54:33.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/language_data.js
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:02.868354 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/lib/
--rw-rw-rw-   0        0        0    20731 2022-02-03 12:41:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/lib/hammer.min.js
--rw-rw-rw-   0        0        0      469 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/lib/prettify.css
--rw-rw-rw-   0        0        0    17033 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/lib/prettify.js
--rw-rw-rw-   0        0        0     2541 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/matrixeq.css
--rw-rw-rw-   0        0        0    27123 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/matrixeq.js
--rw-rw-rw-   0        0        0      264 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/mchoice-i18n.en.js
--rw-rw-rw-   0        0        0      207 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/mchoice-i18n.sr-Cyrl.js
--rw-rw-rw-   0        0        0    20787 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/mchoice.js
--rw-rw-rw-   0        0        0     3014 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/merge.css
--rw-rw-rw-   0        0        0    20969 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/merge.js
--rw-rw-rw-   0        0        0     1335 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/modal-basic.css
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.581087 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/msg/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:02.892800 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/msg/js/
--rw-rw-rw-   0        0        0    28326 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/msg/js/en.js
--rw-rw-rw-   0        0        0     7117 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/navhelp.js
--rw-rw-rw-   0        0        0      252 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/notes.css
--rw-rw-rw-   0        0        0      216 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/notes.js
--rw-rw-rw-   0        0        0      319 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/parsons-i18n.en.js
--rw-rw-rw-   0        0        0      370 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/parsons-i18n.sr-Cyrl.js
--rw-rw-rw-   0        0        0     8848 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/parsons.css
--rw-rw-rw-   0        0        0    97344 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/parsons.js
--rw-rw-rw-   0        0        0     2666 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/petlja.css
--rw-rw-rw-   0        0        0      417 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/poll.css
--rw-rw-rw-   0        0        0     6877 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/poll.js
--rw-rw-rw-   0        0        0     3664 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/presenter_mode.css
--rw-rw-rw-   0        0        0     6290 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/presenter_mode.js
--rw-rw-rw-   0        0        0   231869 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/processing-1.4.1.min.js
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.067723 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/
--rw-rw-rw-   0        0        0    84233 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/__init__.js
--rw-rw-rw-   0        0        0     1888 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/display.js
--rw-rw-rw-   0        0        0     8368 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/draw.js
--rw-rw-rw-   0        0        0     3473 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/event.js
--rw-rw-rw-   0        0        0    11479 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/font.js
--rw-rw-rw-   0        0        0     4240 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/image.js
--rw-rw-rw-   0        0        0     6069 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/key.js
--rw-rw-rw-   0        0        0     1632 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/mouse.js
--rw-rw-rw-   0        0        0       47 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/pygame.js
--rw-rw-rw-   0        0        0     6205 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/time.js
--rw-rw-rw-   0        0        0     5597 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/transform.js
--rw-rw-rw-   0        0        0      254 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/version.js
--rw-rw-rw-   0        0        0     1315 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib-init.js
--rw-rw-rw-   0        0        0     4463 2020-03-17 13:54:33.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygments.css
--rw-rw-rw-   0        0        0    12629 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/python.js
--rw-rw-rw-   0        0        0    30613 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/python_compressed.js
--rw-rw-rw-   0        0        0    18580 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pytutor.css
--rw-rw-rw-   0        0        0   159859 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pytutor.js
--rw-rw-rw-   0        0        0    44234 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/rangy-core.js
--rw-rw-rw-   0        0        0    26515 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/rangy-cssclassapplier.js
--rw-rw-rw-   0        0        0    14204 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/rangy-textrange.js
--rw-rw-rw-   0        0        0     7907 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/reveal.js
--rw-rw-rw-   0        0        0    13625 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/runestone-custom-sphinx-bootstrap.css
--rw-rw-rw-   0        0        0     4326 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/runestonebase.js
--rw-rw-rw-   0        0        0     2181 2019-12-21 09:54:12.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/runestonevideo.js
--rw-rw-rw-   0        0        0    15059 2019-03-10 08:47:02.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/searchtools.js
--rw-rw-rw-   0        0        0   106155 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/sharedb.js
--rw-rw-rw-   0        0        0        0 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/shortanswer.css
--rw-rw-rw-   0        0        0     8135 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/shortanswer.js
--rw-rw-rw-   0        0        0      631 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/showEval.css
--rw-rw-rw-   0        0        0     5939 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/showEval.js
--rw-rw-rw-   0        0        0   472567 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/skulpt-stdlib.js
--rw-rw-rw-   0        0        0   483003 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/skulpt.min.js
--rw-rw-rw-   0        0        0    14765 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/sortmodels.js
--rw-rw-rw-   0        0        0     1314 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/sortviewers.js
--rw-rw-rw-   0        0        0     6509 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/style.css
--rw-rw-rw-   0        0        0      526 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/tabbedstuff.css
--rw-rw-rw-   0        0        0     6176 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/tabbedstuff.js
--rw-rw-rw-   0        0        0    34671 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timed.js
--rw-rw-rw-   0        0        0     2781 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timed_activecode.js
--rw-rw-rw-   0        0        0     1380 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timed_shortanswer.js
--rw-rw-rw-   0        0        0     1913 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timedclickable.js
--rw-rw-rw-   0        0        0     1885 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timeddnd.js
--rw-rw-rw-   0        0        0     1806 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timedfitb.js
--rw-rw-rw-   0        0        0     5551 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timedmc.js
--rw-rw-rw-   0        0        0      578 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timedparsons.js
--rw-rw-rw-   0        0        0    35168 2019-03-03 11:08:43.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/underscore-1.3.1.js
--rw-rw-rw-   0        0        0    12140 2019-03-03 11:08:43.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/underscore.js
--rw-rw-rw-   0        0        0     1839 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/user-highlights.css
--rw-rw-rw-   0        0        0     9337 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/user-highlights.js
--rw-rw-rw-   0        0        0      489 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/video.css
--rw-rw-rw-   0        0        0     8051 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/waypoints.min.js
--rw-rw-rw-   0        0        0      275 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/webgldemo.css
--rw-rw-rw-   0        0        0     4541 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/webglinteractive.css
--rw-rw-rw-   0        0        0    18025 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/webglinteractive.js
--rw-rw-rw-   0        0        0    25355 2019-03-10 08:47:02.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/websupport.js
--rw-rw-rw-   0        0        0    12741 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/xml.js
--rw-rw-rw-   0        0        0      445 2020-03-17 13:54:34.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/searchindex.js
--rw-rw-rw-   0        0        0        0 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/sphinx-enki-info.txt
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.091723 petljadoc-1.3.1/petljadoc/runestone_ext/p5js/
--rw-rw-rw-   0        0        0       21 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/p5js/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.096723 petljadoc-1.3.1/petljadoc/runestone_ext/p5js/css/
--rw-rw-rw-   0        0        0      164 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/p5js/css/p5js.css
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.110724 petljadoc-1.3.1/petljadoc/runestone_ext/p5js/js/
--rw-rw-rw-   0        0        0     1646 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/p5js/js/p5js.js
--rw-rw-rw-   0        0        0     5321 2022-12-02 13:00:34.000000 petljadoc-1.3.1/petljadoc/runestone_ext/p5js/p5js.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.130723 petljadoc-1.3.1/petljadoc/runestone_ext/pycode/
--rw-rw-rw-   0        0        0       23 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pycode/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.143723 petljadoc-1.3.1/petljadoc/runestone_ext/pycode/css/
--rw-rw-rw-   0        0        0     2816 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pycode/css/pycode.css
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.160723 petljadoc-1.3.1/petljadoc/runestone_ext/pycode/js/
--rw-rw-rw-   0        0        0    27491 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pycode/js/pycode.js
--rw-rw-rw-   0        0        0     4032 2022-12-02 13:00:34.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pycode/pycode.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.171723 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/
--rw-rw-rw-   0        0        0       24 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.172724 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.183724 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/
--rw-rw-rw-   0        0        0    84233 2019-09-27 19:15:50.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/__init__.js
--rw-rw-rw-   0        0        0     1888 2021-11-01 13:09:37.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/display.js
--rw-rw-rw-   0        0        0     8368 2021-11-01 13:09:37.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/draw.js
--rw-rw-rw-   0        0        0     3473 2021-11-01 13:09:37.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/event.js
--rw-rw-rw-   0        0        0    11479 2021-11-01 13:09:37.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/font.js
--rw-rw-rw-   0        0        0     4240 2021-11-01 13:09:37.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/image.js
--rw-rw-rw-   0        0        0     6069 2019-09-27 19:15:50.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/key.js
--rw-rw-rw-   0        0        0     1632 2021-11-01 13:09:37.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/mouse.js
--rw-rw-rw-   0        0        0       47 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/pygame.js
--rw-rw-rw-   0        0        0     6205 2021-11-01 13:09:37.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/time.js
--rw-rw-rw-   0        0        0     5597 2021-11-01 13:09:37.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/transform.js
--rw-rw-rw-   0        0        0      254 2021-11-01 13:09:37.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/version.js
--rw-rw-rw-   0        0        0     1315 2021-02-02 16:03:37.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib-init.js
--rw-rw-rw-   0        0        0       57 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/pygamelib.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.217724 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/test/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.588088 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/test/_templates/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.589086 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.589086 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.230724 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.590087 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.247960 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/
--rw-rw-rw-   0        0        0    97346 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.271960 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/
--rw-rw-rw-   0        0        0    27731 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/bootstrap.min.js
--rw-rw-rw-   0        0        0     3776 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-sphinx.js
--rw-rw-rw-   0        0        0     8444 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/test/conf.py
--rw-rw-rw-   0        0        0     1822 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/test/pavement.py
--rw-rw-rw-   0        0        0        0 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/test/sphinx-enki-info.txt
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.293811 petljadoc-1.3.1/petljadoc/runestone_ext/quizq/
--rw-rw-rw-   0        0        0       22 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/quizq/__init__.py
--rw-rw-rw-   0        0        0     1396 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/quizq/quizq.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.312750 petljadoc-1.3.1/petljadoc/runestone_ext/regexcheck/
--rw-rw-rw-   0        0        0       27 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/regexcheck/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.325895 petljadoc-1.3.1/petljadoc/runestone_ext/regexcheck/css/
--rw-rw-rw-   0        0        0     2809 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/regexcheck/css/regex-check.css
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.369363 petljadoc-1.3.1/petljadoc/runestone_ext/regexcheck/js/
--rw-rw-rw-   0        0        0      297 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/regexcheck/js/regex-check-i18n.en.js
--rw-rw-rw-   0        0        0      379 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/regexcheck/js/regex-check-i18n.sr-Cyrl.js
--rw-rw-rw-   0        0        0      316 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/regexcheck/js/regex-check-i18n.sr-Latn.js
--rw-rw-rw-   0        0        0      374 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/regexcheck/js/regex-check-i18n.sr.js
--rw-rw-rw-   0        0        0     5874 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/regexcheck/js/regex-check.js
--rw-rw-rw-   0        0        0     3703 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/runestone_ext/regexcheck/regexcheck.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.386142 petljadoc-1.3.1/petljadoc/runestone_ext/simanim/
--rw-rw-rw-   0        0        0       24 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/simanim/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.387149 petljadoc-1.3.1/petljadoc/runestone_ext/simanim/css/
--rw-rw-rw-   0        0        0     2332 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/simanim/css/simanim.css
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.387149 petljadoc-1.3.1/petljadoc/runestone_ext/simanim/js/
--rw-rw-rw-   0        0        0    21064 2023-03-06 12:31:02.000000 petljadoc-1.3.1/petljadoc/runestone_ext/simanim/js/simanim.js
--rw-rw-rw-   0        0        0     4137 2022-12-02 13:00:34.000000 petljadoc-1.3.1/petljadoc/runestone_ext/simanim/simanim.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.594087 petljadoc-1.3.1/petljadoc/runestone_ext/video/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.594087 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.595087 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.394142 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.399141 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_sources/
--rw-rw-rw-   0        0        0      254 2019-10-06 19:56:26.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_sources/index.rst.txt
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:05.603366 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/
--rw-rw-rw-   0        0        0     6355 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/Blob.js
--rw-rw-rw-   0        0        0     5120 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/FileSaver.min.js
--rw-rw-rw-   0        0        0     1511 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/LICENSE.txt
--rw-rw-rw-   0        0        0     3439 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/accessibility.css
--rw-rw-rw-   0        0        0     3445 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/accessibilitydarkest.css
--rw-rw-rw-   0        0        0     2669 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/accessibilitylight.css
--rw-rw-rw-   0        0        0     9490 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/activecode-i18n.en.js
--rw-rw-rw-   0        0        0    14672 2020-12-09 10:35:50.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/activecode-i18n.sr-Cyrl.js
--rw-rw-rw-   0        0        0     2096 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/activecode.css
--rw-rw-rw-   0        0        0   102910 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/activecode.js
--rw-rw-rw-   0        0        0     3903 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/animationbase.js
--rw-rw-rw-   0        0        0    10912 2019-10-06 20:19:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/basic.css
--rw-rw-rw-   0        0        0   471577 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/blockly_compressed.js
--rw-rw-rw-   0        0        0    55934 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/blocks_compressed.js
--rw-rw-rw-   0        0        0    10606 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bookfuncs.js
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.597088 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-3.0.0/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:05.618383 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-3.0.0/css/
--rw-rw-rw-   0        0        0    97346 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-3.0.0/css/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:05.636383 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-3.0.0/js/
--rw-rw-rw-   0        0        0    27731 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-3.0.0/js/bootstrap.min.js
--rw-rw-rw-   0        0        0      425 2019-10-06 20:19:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-sphinx.css
--rw-rw-rw-   0        0        0     3776 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-sphinx.js
--rw-rw-rw-   0        0        0    97348 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap.min.css
--rw-rw-rw-   0        0        0     1123 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/clickable.css
--rw-rw-rw-   0        0        0    16404 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/clickable.js
--rw-rw-rw-   0        0        0    18265 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/clike.js
--rw-rw-rw-   0        0        0     2037 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/codelens.js
--rw-rw-rw-   0        0        0     7507 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/codemirror.css
--rw-rw-rw-   0        0        0   320980 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/codemirror.js
--rw-rw-rw-   0        0        0    32373 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/css.js
--rw-rw-rw-   0        0        0   111549 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/d3.v2.min.js
--rw-rw-rw-   0        0        0       95 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/datafile.css
--rw-rw-rw-   0        0        0     3000 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/datafile.js
--rw-rw-rw-   0        0        0    19241 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/diff_match_patch.js
--rw-rw-rw-   0        0        0     6868 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/doctools.js
--rw-rw-rw-   0        0        0      307 2019-10-06 20:19:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/documentation_options.js
--rw-rw-rw-   0        0        0      310 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/dragndrop-i18n.en.js
--rw-rw-rw-   0        0        0      389 2020-12-09 10:35:50.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/dragndrop-i18n.sr-Cyrl.js
--rw-rw-rw-   0        0        0     1480 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/dragndrop.css
--rw-rw-rw-   0        0        0    18311 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/dragndrop.js
--rw-rw-rw-   0        0        0     1756 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/external.css
--rw-rw-rw-   0        0        0      130 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/fitb-i18n.en.js
--rw-rw-rw-   0        0        0      142 2020-12-09 10:35:50.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/fitb-i18n.sr-Cyrl.js
--rw-rw-rw-   0        0        0      182 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/fitb.css
--rw-rw-rw-   0        0        0    13759 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/fitb.js
--rw-rw-rw-   0        0        0    21378 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/guiders-1.3.0.css
--rw-rw-rw-   0        0        0    20664 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/guiders-1.3.0.js
--rw-rw-rw-   0        0        0     5108 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/htmlmixed.js
--rw-rw-rw-   0        0        0    24396 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/javascript.js
--rw-rw-rw-   0        0        0    41074 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/javascript_compressed.js
--rw-rw-rw-   0        0        0   268039 2019-03-09 15:07:37.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery-3.2.1.js
--rw-rw-rw-   0        0        0      204 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery-fix.js
--rw-rw-rw-   0        0        0     7200 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery-migrate-1.2.1.min.js
--rw-rw-rw-   0        0        0    26010 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery-ui-1.10.3.custom.min.css
--rw-rw-rw-   0        0        0   217071 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery-ui-1.10.3.custom.min.js
--rw-rw-rw-   0        0        0     4255 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.ba-bbq.min.js
--rw-rw-rw-   0        0        0     1418 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.highlight.js
--rw-rw-rw-   0        0        0     1996 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.hotkey.js
--rw-rw-rw-   0        0        0     8182 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.idle-timer.js
--rw-rw-rw-   0        0        0    93069 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.js
--rw-rw-rw-   0        0        0   120545 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.jsPlumb-1.3.10-all-min.js
--rw-rw-rw-   0        0        0    40914 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.tablesorter.js
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:05.831444 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/
--rw-rw-rw-   0        0        0    13334 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/CLDRPluralRuleParser.js
--rw-rw-rw-   0        0        0    13513 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.emitter.bidi.js
--rw-rw-rw-   0        0        0     5561 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.emitter.js
--rw-rw-rw-   0        0        0     4261 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.fallbacks.js
--rw-rw-rw-   0        0        0     9027 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.js
--rw-rw-rw-   0        0        0    12427 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.language.js
--rw-rw-rw-   0        0        0     3749 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.messagestore.js
--rw-rw-rw-   0        0        0     8483 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.parser.js
--rw-rw-rw-   0        0        0    10847 2019-10-06 20:19:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/language_data.js
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:05.887540 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/lib/
--rw-rw-rw-   0        0        0    20731 2022-02-03 12:41:37.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/lib/hammer.min.js
--rw-rw-rw-   0        0        0      469 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/lib/prettify.css
--rw-rw-rw-   0        0        0    17033 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/lib/prettify.js
--rw-rw-rw-   0        0        0     2541 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/matrixeq.css
--rw-rw-rw-   0        0        0    27123 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/matrixeq.js
--rw-rw-rw-   0        0        0      264 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/mchoice-i18n.en.js
--rw-rw-rw-   0        0        0      202 2020-12-09 10:35:50.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/mchoice-i18n.sr-Cyrl.js
--rw-rw-rw-   0        0        0    20787 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/mchoice.js
--rw-rw-rw-   0        0        0     3014 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/merge.css
--rw-rw-rw-   0        0        0    20969 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/merge.js
--rw-rw-rw-   0        0        0     1335 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/modal-basic.css
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.598087 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/msg/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:05.908193 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/msg/js/
--rw-rw-rw-   0        0        0    28326 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/msg/js/en.js
--rw-rw-rw-   0        0        0     7117 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/navhelp.js
--rw-rw-rw-   0        0        0      314 2020-12-09 10:35:50.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/parsons-i18n.en.js
--rw-rw-rw-   0        0        0      365 2020-12-09 10:35:50.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/parsons-i18n.sr-Cyrl.js
--rw-rw-rw-   0        0        0     8848 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/parsons.css
--rw-rw-rw-   0        0        0    97344 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/parsons.js
--rw-rw-rw-   0        0        0      417 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/poll.css
--rw-rw-rw-   0        0        0     6877 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/poll.js
--rw-rw-rw-   0        0        0     3664 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/presenter_mode.css
--rw-rw-rw-   0        0        0     6290 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/presenter_mode.js
--rw-rw-rw-   0        0        0   231869 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/processing-1.4.1.min.js
--rw-rw-rw-   0        0        0     4463 2019-10-06 20:19:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/pygments.css
--rw-rw-rw-   0        0        0    12629 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/python.js
--rw-rw-rw-   0        0        0    30613 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/python_compressed.js
--rw-rw-rw-   0        0        0    18580 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/pytutor.css
--rw-rw-rw-   0        0        0   159859 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/pytutor.js
--rw-rw-rw-   0        0        0    44234 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/rangy-core.js
--rw-rw-rw-   0        0        0    26515 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/rangy-cssclassapplier.js
--rw-rw-rw-   0        0        0    14204 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/rangy-textrange.js
--rw-rw-rw-   0        0        0     7907 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/reveal.js
--rw-rw-rw-   0        0        0    13625 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/runestone-custom-sphinx-bootstrap.css
--rw-rw-rw-   0        0        0     4326 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/runestonebase.js
--rw-rw-rw-   0        0        0     2181 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/runestonevideo.js
--rw-rw-rw-   0        0        0    15059 2019-03-10 08:47:02.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/searchtools.js
--rw-rw-rw-   0        0        0   106155 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/sharedb.js
--rw-rw-rw-   0        0        0        0 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/shortanswer.css
--rw-rw-rw-   0        0        0     8135 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/shortanswer.js
--rw-rw-rw-   0        0        0      631 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/showEval.css
--rw-rw-rw-   0        0        0     5939 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/showEval.js
--rw-rw-rw-   0        0        0   472567 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/skulpt-stdlib.js
--rw-rw-rw-   0        0        0   483003 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/skulpt.min.js
--rw-rw-rw-   0        0        0    14765 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/sortmodels.js
--rw-rw-rw-   0        0        0     1314 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/sortviewers.js
--rw-rw-rw-   0        0        0     6509 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/style.css
--rw-rw-rw-   0        0        0      526 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/tabbedstuff.css
--rw-rw-rw-   0        0        0     6176 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/tabbedstuff.js
--rw-rw-rw-   0        0        0    34671 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timed.js
--rw-rw-rw-   0        0        0     2781 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timed_activecode.js
--rw-rw-rw-   0        0        0     1380 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timed_shortanswer.js
--rw-rw-rw-   0        0        0     1913 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timedclickable.js
--rw-rw-rw-   0        0        0     1885 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timeddnd.js
--rw-rw-rw-   0        0        0     1806 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timedfitb.js
--rw-rw-rw-   0        0        0     5551 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timedmc.js
--rw-rw-rw-   0        0        0      578 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timedparsons.js
--rw-rw-rw-   0        0        0    35168 2019-03-03 11:08:43.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/underscore-1.3.1.js
--rw-rw-rw-   0        0        0    12140 2019-03-03 11:08:43.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/underscore.js
--rw-rw-rw-   0        0        0     1839 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/user-highlights.css
--rw-rw-rw-   0        0        0     9337 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/user-highlights.js
--rw-rw-rw-   0        0        0      489 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/video.css
--rw-rw-rw-   0        0        0     8051 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/waypoints.min.js
--rw-rw-rw-   0        0        0      275 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/webgldemo.css
--rw-rw-rw-   0        0        0     4541 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/webglinteractive.css
--rw-rw-rw-   0        0        0    18025 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/webglinteractive.js
--rw-rw-rw-   0        0        0    25355 2019-03-10 08:47:02.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/websupport.js
--rw-rw-rw-   0        0        0    12741 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/xml.js
--rw-rw-rw-   0        0        0      398 2019-10-06 20:19:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/searchindex.js
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:06.010388 petljadoc-1.3.1/petljadoc/scorm-proxy-templates/
--rw-rw-rw-   0        0        0     4508 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/scorm-proxy-templates/adlcp_rootv1p2.xsd
--rw-rw-rw-   0        0        0   100404 2022-12-02 13:00:34.000000 petljadoc-1.3.1/petljadoc/scorm-proxy-templates/bundle.js
--rw-rw-rw-   0        0        0    10462 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/scorm-proxy-templates/favicon.ico
--rw-rw-rw-   0        0        0     1236 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/scorm-proxy-templates/ims_xml.xsd
--rw-rw-rw-   0        0        0    14820 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/scorm-proxy-templates/imscp_rootv1p1p2.xsd
--rw-rw-rw-   0        0        0     1184 2023-03-06 12:31:02.000000 petljadoc-1.3.1/petljadoc/scorm-proxy-templates/imsmanifest.t.xml
--rw-rw-rw-   0        0        0    19397 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/scorm-proxy-templates/imsmd_rootv1p2p1.xsd
--rw-rw-rw-   0        0        0     1525 2022-12-02 13:00:34.000000 petljadoc-1.3.1/petljadoc/scorm-proxy-templates/index.t.html
--rw-rw-rw-   0        0        0    18985 2023-01-10 11:56:30.000000 petljadoc-1.3.1/petljadoc/scorm-proxy-templates/style-player.css
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:06.066388 petljadoc-1.3.1/petljadoc/scorm-templates/
--rw-rw-rw-   0        0        0     4508 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/scorm-templates/adlcp_rootv1p2.xsd
--rw-rw-rw-   0        0        0     1236 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/scorm-templates/ims_xml.xsd
--rw-rw-rw-   0        0        0    14820 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/scorm-templates/imscp_rootv1p1p2.xsd
--rw-rw-rw-   0        0        0    19397 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/scorm-templates/imsmd_rootv1p2p1.xsd
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:06.071388 petljadoc-1.3.1/petljadoc/themes/
--rw-rw-rw-   0        0        0       83 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:06.120388 petljadoc-1.3.1/petljadoc/themes/bc_theme/
--rw-rw-rw-   0        0        0      386 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/__init__.py
--rw-rw-rw-   0        0        0     5931 2023-03-15 11:59:27.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/layout.html
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.604086 petljadoc-1.3.1/petljadoc/themes/bc_theme/locale/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.602087 petljadoc-1.3.1/petljadoc/themes/bc_theme/locale/en/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:06.139219 petljadoc-1.3.1/petljadoc/themes/bc_theme/locale/en/LC_MESSAGES/
--rw-rw-rw-   0        0        0      968 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/locale/en/LC_MESSAGES/shpinx.mo
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.604086 petljadoc-1.3.1/petljadoc/themes/bc_theme/locale/sr/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:06.159734 petljadoc-1.3.1/petljadoc/themes/bc_theme/locale/sr/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1260 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/locale/sr/LC_MESSAGES/sphinx.mo
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.603086 petljadoc-1.3.1/petljadoc/themes/bc_theme/locale/sr@latn/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:06.148725 petljadoc-1.3.1/petljadoc/themes/bc_theme/locale/sr@latn/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1007 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/locale/sr@latn/LC_MESSAGES/sphinx.mo
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.605086 petljadoc-1.3.1/petljadoc/themes/bc_theme/locale/sr_RS/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:06.170158 petljadoc-1.3.1/petljadoc/themes/bc_theme/locale/sr_RS/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1260 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/locale/sr_RS/LC_MESSAGES/sphinx.mo
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:06.190761 petljadoc-1.3.1/petljadoc/themes/bc_theme/platform/
--rw-rw-rw-   0        0        0     8733 2022-12-02 13:00:34.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/platform/petljaRTBundle.js
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:06.479169 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.606086 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/bootstrap-4.0.0-dist/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:06.495169 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/bootstrap-4.0.0-dist/css/
--rw-rw-rw-   0        0        0   144836 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/bootstrap-4.0.0-dist/css/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:06.555166 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/bootstrap-4.0.0-dist/js/
--rw-rw-rw-   0        0        0    67698 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/bootstrap-4.0.0-dist/js/bootstrap.bundle.min.js
--rw-rw-rw-   0        0        0    48907 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/bootstrap-4.0.0-dist/js/bootstrap.min.js
--rw-rw-rw-   0        0        0      906 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/bootstrap-sphinx.css_t
--rw-rw-rw-   0        0        0     3776 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/bootstrap-sphinx.js
--rw-rw-rw-   0        0        0   100404 2022-12-02 13:00:34.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/bundle.js
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:06.571167 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/css/
--rw-rw-rw-   0        0        0    31004 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/css/font-awesome.min.css
--rw-rw-rw-   0        0        0    10462 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/favicon.ico
--rw-rw-rw-   0        0        0   127331 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/flatly.min.css
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:06.668167 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/fonts/
--rw-rw-rw-   0        0        0   134808 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/fonts/FontAwesome.otf
--rw-rw-rw-   0        0        0   165742 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.eot
--rw-rw-rw-   0        0        0   447050 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.svg
--rw-rw-rw-   0        0        0   165548 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.ttf
--rw-rw-rw-   0        0        0    98024 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.woff
--rw-rw-rw-   0        0        0    77160 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.woff2
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:06.862203 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/images/
--rw-rw-rw-   0        0        0    69642 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/images/choice-background.svg
--rw-rw-rw-   0        0        0    69619 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/images/dragndrop-background.svg
--rw-rw-rw-   0        0        0    69642 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/images/fitb-background.svg
--rw-rw-rw-   0        0        0      715 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/images/logo.svg
--rw-rw-rw-   0        0        0     1224 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/images/netkabinet-logo-strelica-wt.svg
--rw-rw-rw-   0        0        0    69646 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/images/parsons-background.svg
--rw-rw-rw-   0        0        0      782 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/images/petlja-logo-wt.svg
--rw-rw-rw-   0        0        0     1618 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/images/play_button.svg
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:07.890469 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/
--rw-rw-rw-   0        0        0     3152 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/Facebook.png
--rw-rw-rw-   0        0        0     3079 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/Facebook_icon.png
--rw-rw-rw-   0        0        0     3728 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/Twitter.png
--rw-rw-rw-   0        0        0     3177 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/Twitter_icon.png
--rw-rw-rw-   0        0        0      231 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/active.png
--rw-rw-rw-   0        0        0      332 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/completed.png
--rw-rw-rw-   0        0        0     3482 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/dragndrop-img.svg
--rw-rw-rw-   0        0        0    18186 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/favicon.ico
--rw-rw-rw-   0        0        0      640 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/fitb-img.svg
--rw-rw-rw-   0        0        0     5334 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/green-coin.png
--rw-rw-rw-   0        0        0      447 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/infonote-img.svg
--rw-rw-rw-   0        0        0      828 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-ball.png
--rw-rw-rw-   0        0        0     7370 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-east-balls.png
--rw-rw-rw-   0        0        0     5362 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-east.png
--rw-rw-rw-   0        0        0     8203 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-head.png
--rw-rw-rw-   0        0        0     6942 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-hole.png
--rw-rw-rw-   0        0        0     5910 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-north-balls.png
--rw-rw-rw-   0        0        0     7338 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-north.png
--rw-rw-rw-   0        0        0     6842 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-south-balls.png
--rw-rw-rw-   0        0        0    12370 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-south.png
--rw-rw-rw-   0        0        0    65211 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-west-balls.png
--rw-rw-rw-   0        0        0     7920 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-west.png
--rw-rw-rw-   0        0        0     2857 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/learnmorenote-img.svg
--rw-rw-rw-   0        0        0    37014 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/logo.png
--rw-rw-rw-   0        0        0   102151 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/logo_small.png
--rw-rw-rw-   0        0        0     1224 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/netkabinet-logo-strelica-wt.svg
--rw-rw-rw-   0        0        0     1434 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/parsons-img.svg
--rw-rw-rw-   0        0        0      782 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/petlja-logo-wt.svg
--rw-rw-rw-   0        0        0     5841 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/play_overlay_icon.png
--rw-rw-rw-   0        0        0      640 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/qchoice-img.svg
--rw-rw-rw-   0        0        0     4750 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/question-mark-old.png
--rw-rw-rw-   0        0        0     1327 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/question-mark.png
--rw-rw-rw-   0        0        0     1327 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/questionnote-img.svg
--rw-rw-rw-   0        0        0     3186 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/suggestionnote-img.svg
--rw-rw-rw-   0        0        0     3662 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/technicalnote-img.svg
--rw-rw-rw-   0        0        0    24003 2022-12-02 13:00:34.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/petlja-course.css
--rw-rw-rw-   0        0        0     4607 2023-03-06 12:31:02.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/petlja.js
--rw-rw-rw-   0        0        0    88628 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/require.js
--rw-rw-rw-   0        0        0    47740 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/simanim-0.0.4-py3-none-any.whl
--rw-rw-rw-   0        0        0   472567 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/skulpt-stdlib.js
--rw-rw-rw-   0        0        0   483003 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/skulpt.min.js
--rw-rw-rw-   0        0        0    18985 2022-12-02 13:00:34.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/style-player.css
--rw-rw-rw-   0        0        0     1295 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/theme.conf
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:07.958964 petljadoc-1.3.1/petljadoc/themes/course_theme/
--rw-rw-rw-   0        0        0      390 2022-11-06 09:12:12.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/__init__.py
--rw-rw-rw-   0        0        0     5667 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/basic_layout.html
--rw-rw-rw-   0        0        0     1935 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/course_homepage.html
--rw-rw-rw-   0        0        0     1653 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/globaltoc.html
--rw-rw-rw-   0        0        0     7299 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/layout.html
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.611087 petljadoc-1.3.1/petljadoc/themes/course_theme/locale/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.610088 petljadoc-1.3.1/petljadoc/themes/course_theme/locale/en/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.063336 petljadoc-1.3.1/petljadoc/themes/course_theme/locale/en/LC_MESSAGES/
--rw-rw-rw-   0        0        0      968 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/locale/en/LC_MESSAGES/shpinx.mo
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.611087 petljadoc-1.3.1/petljadoc/themes/course_theme/locale/sr/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.068346 petljadoc-1.3.1/petljadoc/themes/course_theme/locale/sr/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1260 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/locale/sr/LC_MESSAGES/sphinx.mo
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.610088 petljadoc-1.3.1/petljadoc/themes/course_theme/locale/sr@latn/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.068346 petljadoc-1.3.1/petljadoc/themes/course_theme/locale/sr@latn/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1007 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/locale/sr@latn/LC_MESSAGES/sphinx.mo
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.612087 petljadoc-1.3.1/petljadoc/themes/course_theme/locale/sr_RS/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.074334 petljadoc-1.3.1/petljadoc/themes/course_theme/locale/sr_RS/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1260 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/locale/sr_RS/LC_MESSAGES/sphinx.mo
--rw-rw-rw-   0        0        0      205 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/localtoc.html
--rw-rw-rw-   0        0        0      810 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/relations.html
--rw-rw-rw-   0        0        0      170 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/sourcelink.html
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.229806 petljadoc-1.3.1/petljadoc/themes/course_theme/static/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.613086 petljadoc-1.3.1/petljadoc/themes/course_theme/static/bootstrap-4.0.0-dist/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.230805 petljadoc-1.3.1/petljadoc/themes/course_theme/static/bootstrap-4.0.0-dist/css/
--rw-rw-rw-   0        0        0   144836 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/bootstrap-4.0.0-dist/css/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.233807 petljadoc-1.3.1/petljadoc/themes/course_theme/static/bootstrap-4.0.0-dist/js/
--rw-rw-rw-   0        0        0    67698 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/bootstrap-4.0.0-dist/js/bootstrap.bundle.min.js
--rw-rw-rw-   0        0        0    48907 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/bootstrap-4.0.0-dist/js/bootstrap.min.js
--rw-rw-rw-   0        0        0      906 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/bootstrap-sphinx.css_t
--rw-rw-rw-   0        0        0     3776 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/bootstrap-sphinx.js
--rw-rw-rw-   0        0        0      401 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/course-errors.js
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.234809 petljadoc-1.3.1/petljadoc/themes/course_theme/static/css/
--rw-rw-rw-   0        0        0    31004 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/css/font-awesome.min.css
--rw-rw-rw-   0        0        0        0 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/error_log.txt
--rw-rw-rw-   0        0        0    10462 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/favicon.ico
--rw-rw-rw-   0        0        0   127323 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/flatly.min.css
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.240806 petljadoc-1.3.1/petljadoc/themes/course_theme/static/fonts/
--rw-rw-rw-   0        0        0   134808 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/fonts/FontAwesome.otf
--rw-rw-rw-   0        0        0   165742 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.eot
--rw-rw-rw-   0        0        0   447050 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.svg
--rw-rw-rw-   0        0        0   165548 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.ttf
--rw-rw-rw-   0        0        0    98024 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.woff
--rw-rw-rw-   0        0        0    77160 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.woff2
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.247806 petljadoc-1.3.1/petljadoc/themes/course_theme/static/images/
--rw-rw-rw-   0        0        0    69642 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/images/choice-background.svg
--rw-rw-rw-   0        0        0    69619 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/images/dragndrop-background.svg
--rw-rw-rw-   0        0        0    69642 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/images/fitb-background.svg
--rw-rw-rw-   0        0        0      715 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/images/logo.svg
--rw-rw-rw-   0        0        0     1224 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/images/netkabinet-logo-strelica-wt.svg
--rw-rw-rw-   0        0        0    69646 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/images/parsons-background.svg
--rw-rw-rw-   0        0        0      782 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/images/petlja-logo-wt.svg
--rw-rw-rw-   0        0        0     1618 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/images/play_button.svg
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.282246 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/
--rw-rw-rw-   0        0        0     3152 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/Facebook.png
--rw-rw-rw-   0        0        0     3079 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/Facebook_icon.png
--rw-rw-rw-   0        0        0     3728 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/Twitter.png
--rw-rw-rw-   0        0        0     3177 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/Twitter_icon.png
--rw-rw-rw-   0        0        0      231 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/active.png
--rw-rw-rw-   0        0        0      332 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/completed.png
--rw-rw-rw-   0        0        0     3482 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/dragndrop-img.svg
--rw-rw-rw-   0        0        0    18186 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/favicon.ico
--rw-rw-rw-   0        0        0      640 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/fitb-img.svg
--rw-rw-rw-   0        0        0     5334 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/green-coin.png
--rw-rw-rw-   0        0        0      447 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/infonote-img.svg
--rw-rw-rw-   0        0        0      828 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-ball.png
--rw-rw-rw-   0        0        0     7370 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-east-balls.png
--rw-rw-rw-   0        0        0     5362 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-east.png
--rw-rw-rw-   0        0        0     8203 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-head.png
--rw-rw-rw-   0        0        0     6942 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-hole.png
--rw-rw-rw-   0        0        0     5910 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-north-balls.png
--rw-rw-rw-   0        0        0     7338 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-north.png
--rw-rw-rw-   0        0        0     6842 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-south-balls.png
--rw-rw-rw-   0        0        0    12370 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-south.png
--rw-rw-rw-   0        0        0    65211 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-west-balls.png
--rw-rw-rw-   0        0        0     7920 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-west.png
--rw-rw-rw-   0        0        0     2857 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/learnmorenote-img.svg
--rw-rw-rw-   0        0        0    37014 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/logo.png
--rw-rw-rw-   0        0        0   102151 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/logo_small.png
--rw-rw-rw-   0        0        0     1224 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/netkabinet-logo-strelica-wt.svg
--rw-rw-rw-   0        0        0     1434 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/parsons-img.svg
--rw-rw-rw-   0        0        0      782 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/petlja-logo-wt.svg
--rw-rw-rw-   0        0        0     5841 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/play_overlay_icon.png
--rw-rw-rw-   0        0        0      640 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/qchoice-img.svg
--rw-rw-rw-   0        0        0     4750 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/question-mark-old.png
--rw-rw-rw-   0        0        0     1327 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/question-mark.png
--rw-rw-rw-   0        0        0     1327 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/questionnote-img.svg
--rw-rw-rw-   0        0        0     3186 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/suggestionnote-img.svg
--rw-rw-rw-   0        0        0     3662 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/technicalnote-img.svg
--rw-rw-rw-   0        0        0   264982 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/nbstyle.css
--rw-rw-rw-   0        0        0    23457 2022-12-02 13:00:34.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/petlja-course.css
--rw-rw-rw-   0        0        0     7082 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/petlja.js
--rw-rw-rw-   0        0        0    88628 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/require.js
--rw-rw-rw-   0        0        0    47740 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/simanim-0.0.4-py3-none-any.whl
--rw-rw-rw-   0        0        0   472567 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/skulpt-stdlib.js
--rw-rw-rw-   0        0        0   483003 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/skulpt.min.js
--rw-rw-rw-   0        0        0      859 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/subchapter.html
--rw-rw-rw-   0        0        0     1297 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/theme.conf
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.383962 petljadoc-1.3.1/petljadoc/themes/runestone_theme/
--rw-rw-rw-   0        0        0      537 2020-12-09 14:48:07.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/__init__.py
--rw-rw-rw-   0        0        0     8162 2020-12-29 14:15:02.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/basic_layout.html
--rw-rw-rw-   0        0        0      372 2020-12-04 12:05:37.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/globaltoc.html
--rw-rw-rw-   0        0        0     5342 2023-03-06 12:31:02.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/layout.html
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.619087 petljadoc-1.3.1/petljadoc/themes/runestone_theme/locale/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.618087 petljadoc-1.3.1/petljadoc/themes/runestone_theme/locale/en/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.389963 petljadoc-1.3.1/petljadoc/themes/runestone_theme/locale/en/LC_MESSAGES/
--rw-rw-rw-   0        0        0      566 2020-12-09 14:48:07.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/locale/en/LC_MESSAGES/sphinx.mo
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.619087 petljadoc-1.3.1/petljadoc/themes/runestone_theme/locale/sr/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.400717 petljadoc-1.3.1/petljadoc/themes/runestone_theme/locale/sr/LC_MESSAGES/
--rw-rw-rw-   0        0        0      689 2020-12-09 14:48:07.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/locale/sr/LC_MESSAGES/sphinx.mo
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.618087 petljadoc-1.3.1/petljadoc/themes/runestone_theme/locale/sr@latn/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.394961 petljadoc-1.3.1/petljadoc/themes/runestone_theme/locale/sr@latn/LC_MESSAGES/
--rw-rw-rw-   0        0        0      655 2020-12-29 14:15:02.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/locale/sr@latn/LC_MESSAGES/sphinx.mo
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.620086 petljadoc-1.3.1/petljadoc/themes/runestone_theme/locale/sr_RS/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.401732 petljadoc-1.3.1/petljadoc/themes/runestone_theme/locale/sr_RS/LC_MESSAGES/
--rw-rw-rw-   0        0        0      689 2020-12-29 14:15:02.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/locale/sr_RS/LC_MESSAGES/sphinx.mo
--rw-rw-rw-   0        0        0      187 2020-12-08 00:51:34.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/localtoc.html
--rw-rw-rw-   0        0        0     1262 2020-12-09 14:48:07.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/relations.html
--rw-rw-rw-   0        0        0      170 2020-12-04 12:05:37.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/sourcelink.html
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.651963 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.621086 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/bootstrap-4.0.0-dist/
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.679961 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/bootstrap-4.0.0-dist/css/
--rw-rw-rw-   0        0        0   144838 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/bootstrap-4.0.0-dist/css/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.738043 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/bootstrap-4.0.0-dist/js/
--rw-rw-rw-   0        0        0    67698 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/bootstrap-4.0.0-dist/js/bootstrap.bundle.min.js
--rw-rw-rw-   0        0        0    48907 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/bootstrap-4.0.0-dist/js/bootstrap.min.js
--rw-rw-rw-   0        0        0      906 2020-12-04 12:05:37.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/bootstrap-sphinx.css_t
--rw-rw-rw-   0        0        0     3776 2020-12-04 12:05:37.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/bootstrap-sphinx.js
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.749061 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/css/
--rw-rw-rw-   0        0        0    31004 2020-12-04 12:05:37.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/css/font-awesome.min.css
--rw-rw-rw-   0        0        0        0 2020-12-29 14:15:02.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/error_log.txt
--rw-rw-rw-   0        0        0    10462 2020-12-04 12:05:37.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/favicon.ico
--rw-rw-rw-   0        0        0   127331 2020-12-04 12:05:37.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/flatly.min.css
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.847176 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/fonts/
--rw-rw-rw-   0        0        0   134808 2020-12-04 12:05:37.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/fonts/FontAwesome.otf
--rw-rw-rw-   0        0        0   165742 2020-12-04 12:05:37.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.eot
--rw-rw-rw-   0        0        0   447050 2020-12-04 12:05:37.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.svg
--rw-rw-rw-   0        0        0   165548 2020-12-04 12:05:37.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.ttf
--rw-rw-rw-   0        0        0    98024 2020-12-04 12:05:37.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.woff
--rw-rw-rw-   0        0        0    77160 2020-12-04 12:05:37.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.woff2
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.946294 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/images/
--rw-rw-rw-   0        0        0    69642 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/images/choice-background.svg
--rw-rw-rw-   0        0        0    69619 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/images/dragndrop-background.svg
--rw-rw-rw-   0        0        0    69642 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/images/fitb-background.svg
--rw-rw-rw-   0        0        0      715 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/images/logo.svg
--rw-rw-rw-   0        0        0     1224 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/images/netkabinet-logo-strelica-wt.svg
--rw-rw-rw-   0        0        0    69646 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/images/parsons-background.svg
--rw-rw-rw-   0        0        0      782 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/images/petlja-logo-wt.svg
--rw-rw-rw-   0        0        0     1618 2022-01-26 16:39:18.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/images/play_button.svg
-drwxrwxrwx   0        0        0        0 2023-04-10 05:44:09.214965 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/
--rw-rw-rw-   0        0        0     3152 2022-01-26 16:39:18.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/Facebook.png
--rw-rw-rw-   0        0        0     3079 2022-01-26 16:39:18.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/Facebook_icon.png
--rw-rw-rw-   0        0        0     3728 2022-01-26 16:39:18.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/Twitter.png
--rw-rw-rw-   0        0        0     3177 2022-01-26 16:39:18.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/Twitter_icon.png
--rw-rw-rw-   0        0        0      231 2022-01-26 16:39:18.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/active.png
--rw-rw-rw-   0        0        0      332 2022-01-26 16:39:18.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/completed.png
--rw-rw-rw-   0        0        0     3482 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/dragndrop-img.svg
--rw-rw-rw-   0        0        0    18186 2022-01-26 16:39:18.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/favicon.ico
--rw-rw-rw-   0        0        0      640 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/fitb-img.svg
--rw-rw-rw-   0        0        0     5334 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/green-coin.png
--rw-rw-rw-   0        0        0      447 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/infonote-img.svg
--rw-rw-rw-   0        0        0    10414 2022-01-26 16:39:18.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/karel-ball.png
--rw-rw-rw-   0        0        0    19798 2022-01-26 16:39:18.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/karel-east.png
--rw-rw-rw-   0        0        0     8203 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/karel-head.png
--rw-rw-rw-   0        0        0     6942 2022-01-26 16:39:18.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/karel-hole.png
--rw-rw-rw-   0        0        0    13690 2022-01-26 16:39:18.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/karel-north.png
--rw-rw-rw-   0        0        0    14972 2022-01-26 16:39:18.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/karel-south.png
--rw-rw-rw-   0        0        0    19805 2022-01-26 16:39:18.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/karel-west.png
--rw-rw-rw-   0        0        0     2857 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/learnmorenote-img.svg
--rw-rw-rw-   0        0        0    37014 2022-01-26 16:39:18.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/logo.png
--rw-rw-rw-   0        0        0   102151 2022-01-26 16:39:18.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/logo_small.png
--rw-rw-rw-   0        0        0     1224 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/netkabinet-logo-strelica-wt.svg
--rw-rw-rw-   0        0        0     1434 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/parsons-img.svg
--rw-rw-rw-   0        0        0      782 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/petlja-logo-wt.svg
--rw-rw-rw-   0        0        0     5841 2022-01-26 16:39:18.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/play_overlay_icon.png
--rw-rw-rw-   0        0        0      640 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/qchoice-img.svg
--rw-rw-rw-   0        0        0     4750 2022-01-26 16:39:18.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/question-mark-old.png
--rw-rw-rw-   0        0        0     1327 2022-01-26 16:39:18.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/question-mark.png
--rw-rw-rw-   0        0        0     1327 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/questionnote-img.svg
--rw-rw-rw-   0        0        0     3186 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/suggestionnote-img.svg
--rw-rw-rw-   0        0        0     3662 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/technicalnote-img.svg
--rw-rw-rw-   0        0        0   277929 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/nbstyle.css
--rw-rw-rw-   0        0        0     2821 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/petlja-runestone.css
--rw-rw-rw-   0        0        0        0 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/petlja_ruenstone.js
--rw-rw-rw-   0        0        0    88628 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/require.js
--rw-rw-rw-   0        0        0    47740 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/simanim-0.0.4-py3-none-any.whl
--rw-rw-rw-   0        0        0   472567 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/skulpt-stdlib.js
--rw-rw-rw-   0        0        0   483003 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/skulpt.min.js
--rw-rw-rw-   0        0        0     1264 2020-12-09 14:48:07.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/subchapter.html
--rw-rw-rw-   0        0        0     1297 2020-12-04 12:05:37.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/theme.conf
--rw-rw-rw-   0        0        0     4478 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/util.py
-drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.757089 petljadoc-1.3.1/petljadoc.egg-info/
--rw-rw-rw-   0        0        0     2389 2023-04-10 05:43:56.000000 petljadoc-1.3.1/petljadoc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    51038 2023-04-10 05:43:57.000000 petljadoc-1.3.1/petljadoc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 05:43:56.000000 petljadoc-1.3.1/petljadoc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      293 2023-04-10 05:43:56.000000 petljadoc-1.3.1/petljadoc.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2019-09-30 21:36:41.000000 petljadoc-1.3.1/petljadoc.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      195 2023-04-10 05:43:56.000000 petljadoc-1.3.1/petljadoc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-10 05:43:56.000000 petljadoc-1.3.1/petljadoc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      210 2023-03-06 12:48:22.000000 petljadoc-1.3.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 05:44:09.215963 petljadoc-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1707 2022-11-20 11:14:54.000000 petljadoc-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:57.230608 petljadoc-1.3.3/
+-rw-rw-rw-   0        0        0     1084 2019-09-29 18:46:11.000000 petljadoc-1.3.3/LICENSE
+-rw-rw-rw-   0        0        0      475 2022-11-20 11:14:54.000000 petljadoc-1.3.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3407 2023-06-05 12:58:57.229607 petljadoc-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2821 2023-04-12 14:24:18.000000 petljadoc-1.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.949499 petljadoc-1.3.3/petljadoc/
+-rw-rw-rw-   0        0        0       67 2023-06-05 12:58:35.000000 petljadoc-1.3.3/petljadoc/__init__.py
+-rw-rw-rw-   0        0        0       39 2020-12-07 14:32:36.000000 petljadoc-1.3.3/petljadoc/__main__.py
+-rw-rw-rw-   0        0        0    43045 2023-03-06 12:31:02.000000 petljadoc-1.3.3/petljadoc/cli.py
+-rw-rw-rw-   0        0        0    15820 2023-03-06 12:31:02.000000 petljadoc-1.3.3/petljadoc/course.py
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.859497 petljadoc-1.3.3/petljadoc/nb-templates/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.979498 petljadoc-1.3.3/petljadoc/nb-templates/classic2/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.983497 petljadoc-1.3.3/petljadoc/nb-templates/classic2/base/
+-rw-rw-rw-   0        0        0     7752 2022-11-06 13:07:30.000000 petljadoc-1.3.3/petljadoc/nb-templates/classic2/base/base.html.j2
+-rw-rw-rw-   0        0        0      220 2022-11-06 13:07:30.000000 petljadoc-1.3.3/petljadoc/nb-templates/classic2/base/celltags.j2
+-rw-rw-rw-   0        0        0     1634 2022-11-06 13:07:30.000000 petljadoc-1.3.3/petljadoc/nb-templates/classic2/base/display_priority.j2
+-rw-rw-rw-   0        0        0      993 2022-11-06 13:07:30.000000 petljadoc-1.3.3/petljadoc/nb-templates/classic2/base/jupyter_widgets.html.j2
+-rw-rw-rw-   0        0        0     1386 2022-11-06 13:07:30.000000 petljadoc-1.3.3/petljadoc/nb-templates/classic2/base/mathjax.html.j2
+-rw-rw-rw-   0        0        0     6340 2022-11-06 13:07:30.000000 petljadoc-1.3.3/petljadoc/nb-templates/classic2/base/null.j2
+-rw-rw-rw-   0        0        0      401 2022-11-06 13:07:30.000000 petljadoc-1.3.3/petljadoc/nb-templates/classic2/index.html.j2
+-rw-rw-rw-   0        0        0    40964 2023-03-06 12:31:02.000000 petljadoc-1.3.3/petljadoc/package.py
+-rw-rw-rw-   0        0        0     2282 2022-12-02 13:00:34.000000 petljadoc-1.3.3/petljadoc/petlja_builder.py
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.861497 petljadoc-1.3.3/petljadoc/project-templates/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.990497 petljadoc-1.3.3/petljadoc/project-templates/course/
+-rw-rw-rw-   0        0        0      142 2022-12-02 13:00:34.000000 petljadoc-1.3.3/petljadoc/project-templates/course/.t.gitignore
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.991498 petljadoc-1.3.3/petljadoc/project-templates/course/_images/
+-rw-rw-rw-   0        0        0        1 2020-11-30 16:13:38.000000 petljadoc-1.3.3/petljadoc/project-templates/course/_images/.gitkeep
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.992500 petljadoc-1.3.3/petljadoc/project-templates/course/_includes/
+-rw-rw-rw-   0        0        0        1 2020-11-30 16:13:38.000000 petljadoc-1.3.3/petljadoc/project-templates/course/_includes/.gitkeep
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.993498 petljadoc-1.3.3/petljadoc/project-templates/course/_sources/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.994498 petljadoc-1.3.3/petljadoc/project-templates/course/_sources/1_Lesson/
+-rw-rw-rw-   0        0        0     2096 2020-11-30 16:13:38.000000 petljadoc-1.3.3/petljadoc/project-templates/course/_sources/1_Lesson/intro.rst
+-rw-rw-rw-   0        0        0     1564 2022-11-06 13:07:30.000000 petljadoc-1.3.3/petljadoc/project-templates/course/_sources/1_Lesson/quiz.rst
+-rw-rw-rw-   0        0        0     1368 2022-11-06 13:07:30.000000 petljadoc-1.3.3/petljadoc/project-templates/course/_sources/index.t.yaml
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.995497 petljadoc-1.3.3/petljadoc/project-templates/course/_static/
+-rw-rw-rw-   0        0        0        1 2020-11-30 16:13:38.000000 petljadoc-1.3.3/petljadoc/project-templates/course/_static/.gitkeep
+-rw-rw-rw-   0        0        0       75 2023-06-05 12:58:35.000000 petljadoc-1.3.3/petljadoc/project-templates/course/conf-petljadoc.t.json
+-rw-rw-rw-   0        0        0     6291 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/project-templates/course/conf.t.py
+-rw-rw-rw-   0        0        0       33 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/project-templates/course/package-conf.json
+-rw-rw-rw-   0        0        0      777 2020-12-09 14:48:07.000000 petljadoc-1.3.3/petljadoc/project-templates/course/pavement.t.py
+-rw-rw-rw-   0        0        0      110 2022-11-06 13:07:30.000000 petljadoc-1.3.3/petljadoc/project-templates/course/template_settings.t.json
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.998498 petljadoc-1.3.3/petljadoc/project-templates/runestone/
+-rw-rw-rw-   0        0        0       56 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/project-templates/runestone/.t.gitignore
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.999498 petljadoc-1.3.3/petljadoc/project-templates/runestone/_images/
+-rw-rw-rw-   0        0        0        1 2020-11-30 16:13:38.000000 petljadoc-1.3.3/petljadoc/project-templates/runestone/_images/.gitkeep
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.000497 petljadoc-1.3.3/petljadoc/project-templates/runestone/_includes/
+-rw-rw-rw-   0        0        0        1 2020-11-30 16:13:38.000000 petljadoc-1.3.3/petljadoc/project-templates/runestone/_includes/.gitkeep
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.001498 petljadoc-1.3.3/petljadoc/project-templates/runestone/_sources/
+-rw-rw-rw-   0        0        0       90 2022-11-06 13:07:30.000000 petljadoc-1.3.3/petljadoc/project-templates/runestone/_sources/index-item.t.md
+-rw-rw-rw-   0        0        0     3337 2020-11-30 16:13:38.000000 petljadoc-1.3.3/petljadoc/project-templates/runestone/_sources/index.rst
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.010498 petljadoc-1.3.3/petljadoc/project-templates/runestone/_static/
+-rw-rw-rw-   0        0        0        0 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/project-templates/runestone/_static/.gitignore
+-rw-rw-rw-   0        0        0    92708 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/project-templates/runestone/_static/activecodethumb.png
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.032498 petljadoc-1.3.3/petljadoc/project-templates/runestone/_static/audio/
+-rw-rw-rw-   0        0        0    87168 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line01.mp3
+-rw-rw-rw-   0        0        0   273068 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line01.wav
+-rw-rw-rw-   0        0        0   115328 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line02.mp3
+-rw-rw-rw-   0        0        0   361772 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line02.wav
+-rw-rw-rw-   0        0        0   310985 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line03.mp3
+-rw-rw-rw-   0        0        0   978092 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line03.wav
+-rw-rw-rw-   0        0        0    23942 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/project-templates/runestone/_static/clock.png
+-rw-rw-rw-   0        0        0     4497 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/project-templates/runestone/_static/close.png
+-rw-rw-rw-   0        0        0    16165 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/project-templates/runestone/_static/first.png
+-rw-rw-rw-   0        0        0    15899 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/project-templates/runestone/_static/last.png
+-rw-rw-rw-   0        0        0    15743 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/project-templates/runestone/_static/next.png
+-rw-rw-rw-   0        0        0    15344 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/project-templates/runestone/_static/pause.png
+-rw-rw-rw-   0        0        0    15719 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/project-templates/runestone/_static/prev.png
+-rw-rw-rw-   0        0        0       75 2023-06-05 12:58:35.000000 petljadoc-1.3.3/petljadoc/project-templates/runestone/conf-petljadoc.t.json
+-rw-rw-rw-   0        0        0    10633 2022-11-06 13:07:30.000000 petljadoc-1.3.3/petljadoc/project-templates/runestone/conf.t.py
+-rw-rw-rw-   0        0        0      770 2020-12-09 14:48:07.000000 petljadoc-1.3.3/petljadoc/project-templates/runestone/pavement.t.py
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.035497 petljadoc-1.3.3/petljadoc/runestone_ext/
+-rw-rw-rw-   0        0        0     1782 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/runestone_ext/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.036498 petljadoc-1.3.3/petljadoc/runestone_ext/associations/
+-rw-rw-rw-   0        0        0       29 2022-11-06 13:07:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/associations/__init__.py
+-rw-rw-rw-   0        0        0     4629 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/runestone_ext/associations/associations.py
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.037500 petljadoc-1.3.3/petljadoc/runestone_ext/associations/css/
+-rw-rw-rw-   0        0        0     3204 2022-11-06 13:07:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/associations/css/associations.css
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.041498 petljadoc-1.3.3/petljadoc/runestone_ext/associations/js/
+-rw-rw-rw-   0        0        0      147 2022-11-06 13:07:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/associations/js/associations-i18n.en.js
+-rw-rw-rw-   0        0        0      164 2022-11-06 13:07:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/associations/js/associations-i18n.sr-Cyrl.js
+-rw-rw-rw-   0        0        0      144 2022-11-06 13:07:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/associations/js/associations-i18n.sr-Latn.js
+-rw-rw-rw-   0        0        0      159 2022-11-06 13:07:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/associations/js/associations-i18n.sr.js
+-rw-rw-rw-   0        0        0     5682 2022-11-06 13:07:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/associations/js/associations.js
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.043503 petljadoc-1.3.3/petljadoc/runestone_ext/audio/
+-rw-rw-rw-   0        0        0       20 2019-12-21 09:53:52.000000 petljadoc-1.3.3/petljadoc/runestone_ext/audio/__init__.py
+-rw-rw-rw-   0        0        0     1297 2022-11-06 13:07:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/audio/audio.py
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.044503 petljadoc-1.3.3/petljadoc/runestone_ext/audio/test/
+-rw-rw-rw-   0        0        0        0 2019-12-21 09:53:52.000000 petljadoc-1.3.3/petljadoc/runestone_ext/audio/test/sphinx-enki-info.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.045498 petljadoc-1.3.3/petljadoc/runestone_ext/blockly/
+-rw-rw-rw-   0        0        0       27 2022-11-06 13:07:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockly/__init__.py
+-rw-rw-rw-   0        0        0     7055 2023-06-05 12:58:35.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockly/blocklykarel.py
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.046498 petljadoc-1.3.3/petljadoc/runestone_ext/blockly/css/
+-rw-rw-rw-   0        0        0     2065 2022-11-06 13:07:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockly/css/karelBlockly.css
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.058498 petljadoc-1.3.3/petljadoc/runestone_ext/blockly/js/
+-rw-rw-rw-   0        0        0    80180 2022-11-06 13:07:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockly/js/acorn_interpreter.js
+-rw-rw-rw-   0        0        0   929342 2022-11-06 13:07:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockly/js/blockly_compressed.js
+-rw-rw-rw-   0        0        0    90975 2022-11-06 13:07:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockly/js/blocks_compressed.js
+-rw-rw-rw-   0        0        0    46593 2022-11-06 13:07:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockly/js/javascript_compressed.js
+-rw-rw-rw-   0        0        0    19442 2023-06-05 12:58:35.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockly/js/karelBlockly.js
+-rw-rw-rw-   0        0        0    12478 2023-06-05 12:58:35.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockly/js/karelBlocks.js
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.060498 petljadoc-1.3.3/petljadoc/runestone_ext/blockly/js/msg/
+-rw-rw-rw-   0        0        0    32475 2022-11-06 13:07:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockly/js/msg/en.js
+-rw-rw-rw-   0        0        0    40621 2022-11-06 13:07:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockly/js/msg/sr.js
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.061498 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/
+-rw-rw-rw-   0        0        0       25 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/__init__.py
+-rw-rw-rw-   0        0        0     1299 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/blockpylib.py
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.062498 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.070499 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockly/
+-rw-rw-rw-   0        0        0   683169 2019-11-01 17:26:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockly/blockly_compressed.js
+-rw-rw-rw-   0        0        0    92505 2019-11-01 17:26:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockly/blocks_compressed.js
+-rw-rw-rw-   0        0        0    61781 2019-11-01 17:26:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockly/msg-sr.js
+-rw-rw-rw-   0        0        0    40010 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockly/python_compressed.js
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.077500 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/
+-rw-rw-rw-   0        0        0    35053 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/abstract_interpreter.js
+-rw-rw-rw-   0        0        0     6384 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/abstract_interpreter_definitions.js
+-rw-rw-rw-   0        0        0     3736 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/ast_node_visitor.js
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.091498 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/
+-rw-rw-rw-   0        0        0     1888 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/class.js
+-rw-rw-rw-   0        0        0     2178 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/comment.js
+-rw-rw-rw-   0        0        0     1116 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/comprehensions.js
+-rw-rw-rw-   0        0        0      522 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/decorator.js
+-rw-rw-rw-   0        0        0     3777 2019-11-01 17:26:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/dict.js
+-rw-rw-rw-   0        0        0     7891 2019-11-01 17:26:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/if.js
+-rw-rw-rw-   0        0        0     1922 2019-11-01 17:26:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/io.js
+-rw-rw-rw-   0        0        0    12589 2019-11-01 17:26:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/lists.js
+-rw-rw-rw-   0        0        0     1799 2019-11-01 17:26:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/loops.js
+-rw-rw-rw-   0        0        0     8787 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/parking.js
+-rw-rw-rw-   0        0        0      609 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/plots.js
+-rw-rw-rw-   0        0        0     1718 2019-11-01 17:26:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/sets.js
+-rw-rw-rw-   0        0        0     1263 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/text.js
+-rw-rw-rw-   0        0        0     1831 2019-11-01 17:26:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/tuple.js
+-rw-rw-rw-   0        0        0     6969 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/turtles.js
+-rw-rw-rw-   0        0        0     4701 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/imported.js
+-rw-rw-rw-   0        0        0     7255 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/python_errors.js
+-rw-rw-rw-   0        0        0    51813 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/python_to_blockly.js
+-rw-rw-rw-   0        0        0    59429 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/pytifa.js
+-rw-rw-rw-   0        0        0     8165 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/utilities.js
+-rw-rw-rw-   0        0        0     9503 2022-12-02 13:00:34.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy-modal.js
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.870498 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/test/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.870498 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/test/_templates/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.871497 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.871497 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.091498 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.873499 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.092498 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/
+-rw-rw-rw-   0        0        0    97346 2019-11-01 17:26:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.093498 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/
+-rw-rw-rw-   0        0        0    27731 2019-11-01 17:26:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0     3776 2019-11-01 17:26:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-sphinx.js
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.094498 petljadoc-1.3.3/petljadoc/runestone_ext/dbDirective/
+-rw-rw-rw-   0        0        0       28 2022-11-06 13:07:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/dbDirective/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.095498 petljadoc-1.3.3/petljadoc/runestone_ext/dbDirective/css/
+-rw-rw-rw-   0        0        0     2423 2022-11-06 13:07:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/dbDirective/css/dbDirective.css
+-rw-rw-rw-   0        0        0     4636 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/runestone_ext/dbDirective/dbDirective.py
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.096500 petljadoc-1.3.3/petljadoc/runestone_ext/dbDirective/js/
+-rw-rw-rw-   0        0        0    16828 2022-12-02 13:00:34.000000 petljadoc-1.3.3/petljadoc/runestone_ext/dbDirective/js/dbDirective.js
+-rw-rw-rw-   0        0        0    48501 2022-11-06 13:07:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/dbDirective/js/sql.js
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.098498 petljadoc-1.3.3/petljadoc/runestone_ext/editor/
+-rw-rw-rw-   0        0        0       21 2022-11-06 13:07:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/editor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.101497 petljadoc-1.3.3/petljadoc/runestone_ext/editor/css/
+-rw-rw-rw-   0        0        0     1771 2022-11-06 13:07:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/editor/css/editor.css
+-rw-rw-rw-   0        0        0     5287 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/runestone_ext/editor/editor.py
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.105499 petljadoc-1.3.3/petljadoc/runestone_ext/editor/js/
+-rw-rw-rw-   0        0        0       72 2022-11-06 13:07:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/editor/js/editor-i18n.en.js
+-rw-rw-rw-   0        0        0      102 2022-11-06 13:07:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/editor/js/editor-i18n.sr-Cyrl.js
+-rw-rw-rw-   0        0        0       88 2022-11-06 13:07:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/editor/js/editor-i18n.sr-Latn.js
+-rw-rw-rw-   0        0        0       97 2022-11-06 13:07:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/editor/js/editor-i18n.sr.js
+-rw-rw-rw-   0        0        0    10712 2022-11-06 13:07:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/editor/js/editor.js
+-rw-rw-rw-   0        0        0   385745 2022-11-06 13:07:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/editor/js/jszip.js
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.107498 petljadoc-1.3.3/petljadoc/runestone_ext/gallery/
+-rw-rw-rw-   0        0        0       24 2022-11-06 13:07:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/gallery/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.108499 petljadoc-1.3.3/petljadoc/runestone_ext/gallery/css/
+-rw-rw-rw-   0        0        0      589 2022-11-06 13:07:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/gallery/css/gallery.css
+-rw-rw-rw-   0        0        0     4012 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/runestone_ext/gallery/gallery.py
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.109501 petljadoc-1.3.3/petljadoc/runestone_ext/gallery/js/
+-rw-rw-rw-   0        0        0     2096 2022-11-06 13:07:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/gallery/js/gallery.js
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.111500 petljadoc-1.3.3/petljadoc/runestone_ext/karel/
+-rw-rw-rw-   0        0        0       20 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/karel/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.111500 petljadoc-1.3.3/petljadoc/runestone_ext/karel/css/
+-rw-rw-rw-   0        0        0     1080 2022-11-06 13:07:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/karel/css/karel.css
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.120499 petljadoc-1.3.3/petljadoc/runestone_ext/karel/js/
+-rw-rw-rw-   0        0        0      438 2022-11-06 13:07:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/karel/js/karel-i18n.en.js
+-rw-rw-rw-   0        0        0      557 2022-11-06 13:07:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/karel/js/karel-i18n.sr-Cyrl.js
+-rw-rw-rw-   0        0        0      560 2022-11-06 13:07:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/karel/js/karel-i18n.sr.js
+-rw-rw-rw-   0        0        0     3676 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/karel/js/karel.js
+-rw-rw-rw-   0        0        0     1689 2022-11-06 13:07:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/karel/js/karelChat.js
+-rw-rw-rw-   0        0        0     1455 2023-04-10 05:48:22.000000 petljadoc-1.3.3/petljadoc/runestone_ext/karel/js/karelCorner.js
+-rw-rw-rw-   0        0        0     8406 2023-06-05 12:58:35.000000 petljadoc-1.3.3/petljadoc/runestone_ext/karel/js/karelRobot.js
+-rw-rw-rw-   0        0        0    14648 2023-04-10 05:48:22.000000 petljadoc-1.3.3/petljadoc/runestone_ext/karel/js/karelRobotDrawer.js
+-rw-rw-rw-   0        0        0     9995 2019-11-01 17:26:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/karel/js/karelUI.js
+-rw-rw-rw-   0        0        0     5047 2023-04-10 05:48:22.000000 petljadoc-1.3.3/petljadoc/runestone_ext/karel/js/karelWorld.js
+-rw-rw-rw-   0        0        0     5241 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/runestone_ext/karel/karel.py
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.121498 petljadoc-1.3.3/petljadoc/runestone_ext/karel/test/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.880497 petljadoc-1.3.3/petljadoc/runestone_ext/karel/test/_templates/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.880497 petljadoc-1.3.3/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.881497 petljadoc-1.3.3/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.122505 petljadoc-1.3.3/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.882500 petljadoc-1.3.3/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.123501 petljadoc-1.3.3/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/
+-rw-rw-rw-   0        0        0    97346 2019-11-01 17:26:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.124498 petljadoc-1.3.3/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/
+-rw-rw-rw-   0        0        0    27731 2019-11-01 17:26:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0     3776 2019-11-01 17:26:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-sphinx.js
+-rw-rw-rw-   0        0        0        0 2019-11-01 17:26:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/karel/test/sphinx-enki-info.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.125499 petljadoc-1.3.3/petljadoc/runestone_ext/nimgame/
+-rw-rw-rw-   0        0        0       24 2022-11-06 13:07:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/nimgame/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.126498 petljadoc-1.3.3/petljadoc/runestone_ext/nimgame/css/
+-rw-rw-rw-   0        0        0     3729 2022-11-06 13:07:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/nimgame/css/nimgame.css
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.130497 petljadoc-1.3.3/petljadoc/runestone_ext/nimgame/js/
+-rw-rw-rw-   0        0        0      406 2022-11-06 13:07:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/nimgame/js/nimgame-i18n.en.js
+-rw-rw-rw-   0        0        0      565 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/runestone_ext/nimgame/js/nimgame-i18n.sr-Cyrl.js
+-rw-rw-rw-   0        0        0      455 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/runestone_ext/nimgame/js/nimgame-i18n.sr-Latn.js
+-rw-rw-rw-   0        0        0      560 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/runestone_ext/nimgame/js/nimgame-i18n.sr.js
+-rw-rw-rw-   0        0        0    13205 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/runestone_ext/nimgame/js/nimgame.js
+-rw-rw-rw-   0        0        0     4655 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/runestone_ext/nimgame/nimgame.py
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.132499 petljadoc-1.3.3/petljadoc/runestone_ext/notes/
+-rw-rw-rw-   0        0        0       20 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.133497 petljadoc-1.3.3/petljadoc/runestone_ext/notes/css/
+-rw-rw-rw-   0        0        0     3334 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/css/notes.css
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.134498 petljadoc-1.3.3/petljadoc/runestone_ext/notes/js/
+-rw-rw-rw-   0        0        0     1101 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/js/notes.js
+-rw-rw-rw-   0        0        0     5293 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/notes.py
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.135498 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.885499 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/_templates/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.886499 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.886499 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.136498 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.887498 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.137499 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/
+-rw-rw-rw-   0        0        0    97346 2019-11-01 17:26:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.138499 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/
+-rw-rw-rw-   0        0        0    27731 2019-11-01 17:26:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0     3776 2019-11-01 17:26:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-sphinx.js
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.888497 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.144497 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:50.149500 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_sources/
+-rw-rw-rw-   0        0        0      265 2019-11-01 17:26:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_sources/index.rst.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:53.014889 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/
+-rw-rw-rw-   0        0        0     6355 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/Blob.js
+-rw-rw-rw-   0        0        0     5120 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/FileSaver.min.js
+-rw-rw-rw-   0        0        0     1511 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/LICENSE.txt
+-rw-rw-rw-   0        0        0     3439 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/accessibility.css
+-rw-rw-rw-   0        0        0     3445 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/accessibilitydarkest.css
+-rw-rw-rw-   0        0        0     2669 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/accessibilitylight.css
+-rw-rw-rw-   0        0        0     9490 2019-12-21 09:54:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/activecode-i18n.en.js
+-rw-rw-rw-   0        0        0    14677 2019-12-21 09:54:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/activecode-i18n.sr-Cyrl.js
+-rw-rw-rw-   0        0        0     2096 2019-12-21 09:54:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/activecode.css
+-rw-rw-rw-   0        0        0   103165 2020-02-25 19:14:39.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/activecode.js
+-rw-rw-rw-   0        0        0     3903 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/animationbase.js
+-rw-rw-rw-   0        0        0    10912 2020-03-17 13:54:33.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/basic.css
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:53.213884 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly/
+-rw-rw-rw-   0        0        0   683169 2019-11-01 17:26:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly/blockly_compressed.js
+-rw-rw-rw-   0        0        0    92505 2019-11-01 17:26:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly/blocks_compressed.js
+-rw-rw-rw-   0        0        0    61781 2019-11-01 17:26:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly/msg-sr.js
+-rw-rw-rw-   0        0        0    40010 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly/python_compressed.js
+-rw-rw-rw-   0        0        0   471577 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly_compressed.js
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:53.375808 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/
+-rw-rw-rw-   0        0        0    35053 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/abstract_interpreter.js
+-rw-rw-rw-   0        0        0     6384 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/abstract_interpreter_definitions.js
+-rw-rw-rw-   0        0        0     3736 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/ast_node_visitor.js
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:53.680808 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/
+-rw-rw-rw-   0        0        0     1888 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/class.js
+-rw-rw-rw-   0        0        0     2178 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/comment.js
+-rw-rw-rw-   0        0        0     1116 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/comprehensions.js
+-rw-rw-rw-   0        0        0      522 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/decorator.js
+-rw-rw-rw-   0        0        0     3777 2019-11-01 17:26:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/dict.js
+-rw-rw-rw-   0        0        0     7891 2019-11-01 17:26:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/if.js
+-rw-rw-rw-   0        0        0     1922 2019-11-01 17:26:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/io.js
+-rw-rw-rw-   0        0        0    12589 2019-11-01 17:26:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/lists.js
+-rw-rw-rw-   0        0        0     1799 2019-11-01 17:26:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/loops.js
+-rw-rw-rw-   0        0        0     8787 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/parking.js
+-rw-rw-rw-   0        0        0      609 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/plots.js
+-rw-rw-rw-   0        0        0     1718 2019-11-01 17:26:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/sets.js
+-rw-rw-rw-   0        0        0     1263 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/text.js
+-rw-rw-rw-   0        0        0     1831 2019-11-01 17:26:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/tuple.js
+-rw-rw-rw-   0        0        0     6969 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/turtles.js
+-rw-rw-rw-   0        0        0     4701 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/imported.js
+-rw-rw-rw-   0        0        0     7255 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/python_errors.js
+-rw-rw-rw-   0        0        0    51813 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/python_to_blockly.js
+-rw-rw-rw-   0        0        0    59429 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/pytifa.js
+-rw-rw-rw-   0        0        0     8165 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/utilities.js
+-rw-rw-rw-   0        0        0     9298 2019-11-01 17:26:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy-modal.js
+-rw-rw-rw-   0        0        0    55934 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blocks_compressed.js
+-rw-rw-rw-   0        0        0    10606 2019-12-21 09:54:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bookfuncs.js
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.893497 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-4.0.0-dist/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:53.696515 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-4.0.0-dist/css/
+-rw-rw-rw-   0        0        0   144838 2022-02-03 12:41:00.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-4.0.0-dist/css/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:53.773491 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-4.0.0-dist/js/
+-rw-rw-rw-   0        0        0    67698 2022-02-03 12:41:15.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-4.0.0-dist/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0    48907 2022-02-03 12:41:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-4.0.0-dist/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0      425 2020-03-17 13:54:33.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-sphinx.css
+-rw-rw-rw-   0        0        0     3776 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-sphinx.js
+-rw-rw-rw-   0        0        0    97348 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap.min.css
+-rw-rw-rw-   0        0        0     1123 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/clickable.css
+-rw-rw-rw-   0        0        0    16404 2019-12-21 09:54:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/clickable.js
+-rw-rw-rw-   0        0        0    18265 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/clike.js
+-rw-rw-rw-   0        0        0     2037 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/codelens.js
+-rw-rw-rw-   0        0        0     7507 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/codemirror.css
+-rw-rw-rw-   0        0        0   320980 2019-12-21 09:54:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/codemirror.js
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:53.805490 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/css/
+-rw-rw-rw-   0        0        0    31004 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/css/font-awesome.min.css
+-rw-rw-rw-   0        0        0    32373 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/css.js
+-rw-rw-rw-   0        0        0   111549 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/d3.v2.min.js
+-rw-rw-rw-   0        0        0       95 2019-12-21 09:54:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/datafile.css
+-rw-rw-rw-   0        0        0     3000 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/datafile.js
+-rw-rw-rw-   0        0        0    19241 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/diff_match_patch.js
+-rw-rw-rw-   0        0        0     6868 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/doctools.js
+-rw-rw-rw-   0        0        0      306 2020-03-17 13:54:33.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/documentation_options.js
+-rw-rw-rw-   0        0        0      310 2019-12-21 09:54:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/dragndrop-i18n.en.js
+-rw-rw-rw-   0        0        0      394 2019-12-21 09:54:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/dragndrop-i18n.sr-Cyrl.js
+-rw-rw-rw-   0        0        0     1480 2019-12-21 09:54:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/dragndrop.css
+-rw-rw-rw-   0        0        0    18311 2019-12-21 09:54:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/dragndrop.js
+-rw-rw-rw-   0        0        0     1756 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/external.css
+-rw-rw-rw-   0        0        0      130 2019-12-21 09:54:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/fitb-i18n.en.js
+-rw-rw-rw-   0        0        0      147 2019-12-21 09:54:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/fitb-i18n.sr-Cyrl.js
+-rw-rw-rw-   0        0        0      182 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/fitb.css
+-rw-rw-rw-   0        0        0    13759 2019-12-21 09:54:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/fitb.js
+-rw-rw-rw-   0        0        0   127331 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/flatly.min.css
+-rw-rw-rw-   0        0        0    21378 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/guiders-1.3.0.css
+-rw-rw-rw-   0        0        0    20664 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/guiders-1.3.0.js
+-rw-rw-rw-   0        0        0     5108 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/htmlmixed.js
+-rw-rw-rw-   0        0        0    24396 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/javascript.js
+-rw-rw-rw-   0        0        0    41074 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/javascript_compressed.js
+-rw-rw-rw-   0        0        0   268039 2019-03-09 15:07:37.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery-3.2.1.js
+-rw-rw-rw-   0        0        0      204 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery-fix.js
+-rw-rw-rw-   0        0        0     7200 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery-migrate-1.2.1.min.js
+-rw-rw-rw-   0        0        0    26010 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery-ui-1.10.3.custom.min.css
+-rw-rw-rw-   0        0        0   217071 2019-12-21 09:54:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery-ui-1.10.3.custom.min.js
+-rw-rw-rw-   0        0        0     4255 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.ba-bbq.min.js
+-rw-rw-rw-   0        0        0     1418 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.highlight.js
+-rw-rw-rw-   0        0        0     1996 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.hotkey.js
+-rw-rw-rw-   0        0        0     8182 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.idle-timer.js
+-rw-rw-rw-   0        0        0    93069 2019-12-21 09:54:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.js
+-rw-rw-rw-   0        0        0   120545 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.jsPlumb-1.3.10-all-min.js
+-rw-rw-rw-   0        0        0    40914 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.tablesorter.js
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:54.002407 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/
+-rw-rw-rw-   0        0        0    13334 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/CLDRPluralRuleParser.js
+-rw-rw-rw-   0        0        0    13513 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.emitter.bidi.js
+-rw-rw-rw-   0        0        0     5561 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.emitter.js
+-rw-rw-rw-   0        0        0     4261 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.fallbacks.js
+-rw-rw-rw-   0        0        0     9027 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.js
+-rw-rw-rw-   0        0        0    12427 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.language.js
+-rw-rw-rw-   0        0        0     3749 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.messagestore.js
+-rw-rw-rw-   0        0        0     8483 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.parser.js
+-rw-rw-rw-   0        0        0      380 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karel-i18n.en.js
+-rw-rw-rw-   0        0        0      484 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karel-i18n.sr-Cyrl.js
+-rw-rw-rw-   0        0        0      984 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karel.css
+-rw-rw-rw-   0        0        0     3676 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karel.js
+-rw-rw-rw-   0        0        0     1105 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelCorner.js
+-rw-rw-rw-   0        0        0     6290 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelRobot.js
+-rw-rw-rw-   0        0        0    12016 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelRobotDrawer.js
+-rw-rw-rw-   0        0        0     9995 2019-11-01 17:26:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelUI.js
+-rw-rw-rw-   0        0        0     4647 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelWorld.js
+-rw-rw-rw-   0        0        0    10847 2020-03-17 13:54:33.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/language_data.js
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:54.086346 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/lib/
+-rw-rw-rw-   0        0        0    20731 2022-02-03 12:41:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/lib/hammer.min.js
+-rw-rw-rw-   0        0        0      469 2019-12-21 09:54:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/lib/prettify.css
+-rw-rw-rw-   0        0        0    17033 2019-12-21 09:54:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/lib/prettify.js
+-rw-rw-rw-   0        0        0     2541 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/matrixeq.css
+-rw-rw-rw-   0        0        0    27123 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/matrixeq.js
+-rw-rw-rw-   0        0        0      264 2019-12-21 09:54:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/mchoice-i18n.en.js
+-rw-rw-rw-   0        0        0      207 2019-12-21 09:54:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/mchoice-i18n.sr-Cyrl.js
+-rw-rw-rw-   0        0        0    20787 2019-12-21 09:54:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/mchoice.js
+-rw-rw-rw-   0        0        0     3014 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/merge.css
+-rw-rw-rw-   0        0        0    20969 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/merge.js
+-rw-rw-rw-   0        0        0     1335 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/modal-basic.css
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.895499 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/msg/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:54.110358 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/msg/js/
+-rw-rw-rw-   0        0        0    28326 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/msg/js/en.js
+-rw-rw-rw-   0        0        0     7117 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/navhelp.js
+-rw-rw-rw-   0        0        0      252 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/notes.css
+-rw-rw-rw-   0        0        0      216 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/notes.js
+-rw-rw-rw-   0        0        0      319 2019-12-21 09:54:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/parsons-i18n.en.js
+-rw-rw-rw-   0        0        0      370 2019-12-21 09:54:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/parsons-i18n.sr-Cyrl.js
+-rw-rw-rw-   0        0        0     8848 2019-12-21 09:54:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/parsons.css
+-rw-rw-rw-   0        0        0    97344 2019-12-21 09:54:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/parsons.js
+-rw-rw-rw-   0        0        0     2666 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/petlja.css
+-rw-rw-rw-   0        0        0      417 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/poll.css
+-rw-rw-rw-   0        0        0     6877 2019-12-21 09:54:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/poll.js
+-rw-rw-rw-   0        0        0     3664 2019-12-21 09:54:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/presenter_mode.css
+-rw-rw-rw-   0        0        0     6290 2019-12-21 09:54:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/presenter_mode.js
+-rw-rw-rw-   0        0        0   231869 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/processing-1.4.1.min.js
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:54.311807 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/
+-rw-rw-rw-   0        0        0    84233 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/__init__.js
+-rw-rw-rw-   0        0        0     1888 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/display.js
+-rw-rw-rw-   0        0        0     8368 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/draw.js
+-rw-rw-rw-   0        0        0     3473 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/event.js
+-rw-rw-rw-   0        0        0    11479 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/font.js
+-rw-rw-rw-   0        0        0     4240 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/image.js
+-rw-rw-rw-   0        0        0     6069 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/key.js
+-rw-rw-rw-   0        0        0     1632 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/mouse.js
+-rw-rw-rw-   0        0        0       47 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/pygame.js
+-rw-rw-rw-   0        0        0     6205 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/time.js
+-rw-rw-rw-   0        0        0     5597 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/transform.js
+-rw-rw-rw-   0        0        0      254 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/version.js
+-rw-rw-rw-   0        0        0     1315 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib-init.js
+-rw-rw-rw-   0        0        0     4463 2020-03-17 13:54:33.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygments.css
+-rw-rw-rw-   0        0        0    12629 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/python.js
+-rw-rw-rw-   0        0        0    30613 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/python_compressed.js
+-rw-rw-rw-   0        0        0    18580 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pytutor.css
+-rw-rw-rw-   0        0        0   159859 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pytutor.js
+-rw-rw-rw-   0        0        0    44234 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/rangy-core.js
+-rw-rw-rw-   0        0        0    26515 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/rangy-cssclassapplier.js
+-rw-rw-rw-   0        0        0    14204 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/rangy-textrange.js
+-rw-rw-rw-   0        0        0     7907 2019-12-21 09:54:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/reveal.js
+-rw-rw-rw-   0        0        0    13625 2019-12-21 09:54:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/runestone-custom-sphinx-bootstrap.css
+-rw-rw-rw-   0        0        0     4326 2019-12-21 09:54:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/runestonebase.js
+-rw-rw-rw-   0        0        0     2181 2019-12-21 09:54:12.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/runestonevideo.js
+-rw-rw-rw-   0        0        0    15059 2019-03-10 08:47:02.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/searchtools.js
+-rw-rw-rw-   0        0        0   106155 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/sharedb.js
+-rw-rw-rw-   0        0        0        0 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/shortanswer.css
+-rw-rw-rw-   0        0        0     8135 2019-12-21 09:54:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/shortanswer.js
+-rw-rw-rw-   0        0        0      631 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/showEval.css
+-rw-rw-rw-   0        0        0     5939 2019-12-21 09:54:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/showEval.js
+-rw-rw-rw-   0        0        0   472567 2019-12-21 09:54:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/skulpt-stdlib.js
+-rw-rw-rw-   0        0        0   483003 2019-12-21 09:54:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/skulpt.min.js
+-rw-rw-rw-   0        0        0    14765 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/sortmodels.js
+-rw-rw-rw-   0        0        0     1314 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/sortviewers.js
+-rw-rw-rw-   0        0        0     6509 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/style.css
+-rw-rw-rw-   0        0        0      526 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/tabbedstuff.css
+-rw-rw-rw-   0        0        0     6176 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/tabbedstuff.js
+-rw-rw-rw-   0        0        0    34671 2019-12-21 09:54:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timed.js
+-rw-rw-rw-   0        0        0     2781 2019-12-21 09:54:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timed_activecode.js
+-rw-rw-rw-   0        0        0     1380 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timed_shortanswer.js
+-rw-rw-rw-   0        0        0     1913 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timedclickable.js
+-rw-rw-rw-   0        0        0     1885 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timeddnd.js
+-rw-rw-rw-   0        0        0     1806 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timedfitb.js
+-rw-rw-rw-   0        0        0     5551 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timedmc.js
+-rw-rw-rw-   0        0        0      578 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timedparsons.js
+-rw-rw-rw-   0        0        0    35168 2019-03-03 11:08:43.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/underscore-1.3.1.js
+-rw-rw-rw-   0        0        0    12140 2019-03-03 11:08:43.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/underscore.js
+-rw-rw-rw-   0        0        0     1839 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/user-highlights.css
+-rw-rw-rw-   0        0        0     9337 2019-12-21 09:54:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/user-highlights.js
+-rw-rw-rw-   0        0        0      489 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/video.css
+-rw-rw-rw-   0        0        0     8051 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/waypoints.min.js
+-rw-rw-rw-   0        0        0      275 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/webgldemo.css
+-rw-rw-rw-   0        0        0     4541 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/webglinteractive.css
+-rw-rw-rw-   0        0        0    18025 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/webglinteractive.js
+-rw-rw-rw-   0        0        0    25355 2019-03-10 08:47:02.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/websupport.js
+-rw-rw-rw-   0        0        0    12741 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/xml.js
+-rw-rw-rw-   0        0        0      445 2020-03-17 13:54:34.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/searchindex.js
+-rw-rw-rw-   0        0        0        0 2019-11-01 17:26:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/sphinx-enki-info.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:54.313807 petljadoc-1.3.3/petljadoc/runestone_ext/p5js/
+-rw-rw-rw-   0        0        0       21 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/runestone_ext/p5js/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:54.314808 petljadoc-1.3.3/petljadoc/runestone_ext/p5js/css/
+-rw-rw-rw-   0        0        0      164 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/runestone_ext/p5js/css/p5js.css
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:54.314808 petljadoc-1.3.3/petljadoc/runestone_ext/p5js/js/
+-rw-rw-rw-   0        0        0     1646 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/runestone_ext/p5js/js/p5js.js
+-rw-rw-rw-   0        0        0     5321 2022-12-02 13:00:34.000000 petljadoc-1.3.3/petljadoc/runestone_ext/p5js/p5js.py
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:54.316806 petljadoc-1.3.3/petljadoc/runestone_ext/pycode/
+-rw-rw-rw-   0        0        0       23 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/runestone_ext/pycode/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:54.318806 petljadoc-1.3.3/petljadoc/runestone_ext/pycode/css/
+-rw-rw-rw-   0        0        0     2816 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/runestone_ext/pycode/css/pycode.css
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:54.318806 petljadoc-1.3.3/petljadoc/runestone_ext/pycode/js/
+-rw-rw-rw-   0        0        0    27491 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/runestone_ext/pycode/js/pycode.js
+-rw-rw-rw-   0        0        0     4032 2022-12-02 13:00:34.000000 petljadoc-1.3.3/petljadoc/runestone_ext/pycode/pycode.py
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:54.320807 petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/
+-rw-rw-rw-   0        0        0       24 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:54.321807 petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/js/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:54.335808 petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/js/pygamelib/
+-rw-rw-rw-   0        0        0    84233 2019-09-27 19:15:50.000000 petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/js/pygamelib/__init__.js
+-rw-rw-rw-   0        0        0     1888 2021-11-01 13:09:37.000000 petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/js/pygamelib/display.js
+-rw-rw-rw-   0        0        0     8368 2021-11-01 13:09:37.000000 petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/js/pygamelib/draw.js
+-rw-rw-rw-   0        0        0     3473 2021-11-01 13:09:37.000000 petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/js/pygamelib/event.js
+-rw-rw-rw-   0        0        0    11479 2021-11-01 13:09:37.000000 petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/js/pygamelib/font.js
+-rw-rw-rw-   0        0        0     4240 2021-11-01 13:09:37.000000 petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/js/pygamelib/image.js
+-rw-rw-rw-   0        0        0     6069 2019-09-27 19:15:50.000000 petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/js/pygamelib/key.js
+-rw-rw-rw-   0        0        0     1632 2021-11-01 13:09:37.000000 petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/js/pygamelib/mouse.js
+-rw-rw-rw-   0        0        0       47 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/js/pygamelib/pygame.js
+-rw-rw-rw-   0        0        0     6205 2021-11-01 13:09:37.000000 petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/js/pygamelib/time.js
+-rw-rw-rw-   0        0        0     5597 2021-11-01 13:09:37.000000 petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/js/pygamelib/transform.js
+-rw-rw-rw-   0        0        0      254 2021-11-01 13:09:37.000000 petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/js/pygamelib/version.js
+-rw-rw-rw-   0        0        0     1315 2021-02-02 16:03:37.000000 petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/js/pygamelib-init.js
+-rw-rw-rw-   0        0        0       57 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/pygamelib.py
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:54.338809 petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/test/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.900498 petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/test/_templates/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.900498 petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.900498 petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:54.339806 petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.902497 petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:54.340807 petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/
+-rw-rw-rw-   0        0        0    97346 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:54.341807 petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/
+-rw-rw-rw-   0        0        0    27731 2019-09-29 18:46:11.000000 petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0     3776 2019-11-01 17:26:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-sphinx.js
+-rw-rw-rw-   0        0        0     8444 2019-11-01 17:26:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/test/conf.py
+-rw-rw-rw-   0        0        0     1822 2019-11-01 17:26:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/test/pavement.py
+-rw-rw-rw-   0        0        0        0 2019-11-01 17:26:30.000000 petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/test/sphinx-enki-info.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:54.344807 petljadoc-1.3.3/petljadoc/runestone_ext/quizq/
+-rw-rw-rw-   0        0        0       22 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/runestone_ext/quizq/__init__.py
+-rw-rw-rw-   0        0        0     1396 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/runestone_ext/quizq/quizq.py
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:54.346807 petljadoc-1.3.3/petljadoc/runestone_ext/regexcheck/
+-rw-rw-rw-   0        0        0       27 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/runestone_ext/regexcheck/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:54.346807 petljadoc-1.3.3/petljadoc/runestone_ext/regexcheck/css/
+-rw-rw-rw-   0        0        0     2809 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/runestone_ext/regexcheck/css/regex-check.css
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:54.351807 petljadoc-1.3.3/petljadoc/runestone_ext/regexcheck/js/
+-rw-rw-rw-   0        0        0      297 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/runestone_ext/regexcheck/js/regex-check-i18n.en.js
+-rw-rw-rw-   0        0        0      379 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/runestone_ext/regexcheck/js/regex-check-i18n.sr-Cyrl.js
+-rw-rw-rw-   0        0        0      316 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/runestone_ext/regexcheck/js/regex-check-i18n.sr-Latn.js
+-rw-rw-rw-   0        0        0      374 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/runestone_ext/regexcheck/js/regex-check-i18n.sr.js
+-rw-rw-rw-   0        0        0     5874 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/runestone_ext/regexcheck/js/regex-check.js
+-rw-rw-rw-   0        0        0     3703 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/runestone_ext/regexcheck/regexcheck.py
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:54.353807 petljadoc-1.3.3/petljadoc/runestone_ext/simanim/
+-rw-rw-rw-   0        0        0       24 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/runestone_ext/simanim/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:54.353807 petljadoc-1.3.3/petljadoc/runestone_ext/simanim/css/
+-rw-rw-rw-   0        0        0     2332 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/runestone_ext/simanim/css/simanim.css
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:54.354807 petljadoc-1.3.3/petljadoc/runestone_ext/simanim/js/
+-rw-rw-rw-   0        0        0    21251 2023-04-11 09:01:42.000000 petljadoc-1.3.3/petljadoc/runestone_ext/simanim/js/simanim.js
+-rw-rw-rw-   0        0        0     4137 2022-12-02 13:00:34.000000 petljadoc-1.3.3/petljadoc/runestone_ext/simanim/simanim.py
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.905498 petljadoc-1.3.3/petljadoc/runestone_ext/video/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.905498 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.906497 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:54.360807 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:54.366807 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_sources/
+-rw-rw-rw-   0        0        0      254 2019-10-06 19:56:26.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_sources/index.rst.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:56.622162 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/
+-rw-rw-rw-   0        0        0     6355 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/Blob.js
+-rw-rw-rw-   0        0        0     5120 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/FileSaver.min.js
+-rw-rw-rw-   0        0        0     1511 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/LICENSE.txt
+-rw-rw-rw-   0        0        0     3439 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/accessibility.css
+-rw-rw-rw-   0        0        0     3445 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/accessibilitydarkest.css
+-rw-rw-rw-   0        0        0     2669 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/accessibilitylight.css
+-rw-rw-rw-   0        0        0     9490 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/activecode-i18n.en.js
+-rw-rw-rw-   0        0        0    14672 2020-12-09 10:35:50.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/activecode-i18n.sr-Cyrl.js
+-rw-rw-rw-   0        0        0     2096 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/activecode.css
+-rw-rw-rw-   0        0        0   102910 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/activecode.js
+-rw-rw-rw-   0        0        0     3903 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/animationbase.js
+-rw-rw-rw-   0        0        0    10912 2019-10-06 20:19:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/basic.css
+-rw-rw-rw-   0        0        0   471577 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/blockly_compressed.js
+-rw-rw-rw-   0        0        0    55934 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/blocks_compressed.js
+-rw-rw-rw-   0        0        0    10606 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bookfuncs.js
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.912499 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-3.0.0/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:56.635172 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-3.0.0/css/
+-rw-rw-rw-   0        0        0    97346 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-3.0.0/css/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:56.655172 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-3.0.0/js/
+-rw-rw-rw-   0        0        0    27731 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-3.0.0/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0      425 2019-10-06 20:19:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-sphinx.css
+-rw-rw-rw-   0        0        0     3776 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-sphinx.js
+-rw-rw-rw-   0        0        0    97348 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap.min.css
+-rw-rw-rw-   0        0        0     1123 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/clickable.css
+-rw-rw-rw-   0        0        0    16404 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/clickable.js
+-rw-rw-rw-   0        0        0    18265 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/clike.js
+-rw-rw-rw-   0        0        0     2037 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/codelens.js
+-rw-rw-rw-   0        0        0     7507 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/codemirror.css
+-rw-rw-rw-   0        0        0   320980 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/codemirror.js
+-rw-rw-rw-   0        0        0    32373 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/css.js
+-rw-rw-rw-   0        0        0   111549 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/d3.v2.min.js
+-rw-rw-rw-   0        0        0       95 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/datafile.css
+-rw-rw-rw-   0        0        0     3000 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/datafile.js
+-rw-rw-rw-   0        0        0    19241 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/diff_match_patch.js
+-rw-rw-rw-   0        0        0     6868 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/doctools.js
+-rw-rw-rw-   0        0        0      307 2019-10-06 20:19:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/documentation_options.js
+-rw-rw-rw-   0        0        0      310 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/dragndrop-i18n.en.js
+-rw-rw-rw-   0        0        0      389 2020-12-09 10:35:50.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/dragndrop-i18n.sr-Cyrl.js
+-rw-rw-rw-   0        0        0     1480 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/dragndrop.css
+-rw-rw-rw-   0        0        0    18311 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/dragndrop.js
+-rw-rw-rw-   0        0        0     1756 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/external.css
+-rw-rw-rw-   0        0        0      130 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/fitb-i18n.en.js
+-rw-rw-rw-   0        0        0      142 2020-12-09 10:35:50.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/fitb-i18n.sr-Cyrl.js
+-rw-rw-rw-   0        0        0      182 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/fitb.css
+-rw-rw-rw-   0        0        0    13759 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/fitb.js
+-rw-rw-rw-   0        0        0    21378 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/guiders-1.3.0.css
+-rw-rw-rw-   0        0        0    20664 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/guiders-1.3.0.js
+-rw-rw-rw-   0        0        0     5108 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/htmlmixed.js
+-rw-rw-rw-   0        0        0    24396 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/javascript.js
+-rw-rw-rw-   0        0        0    41074 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/javascript_compressed.js
+-rw-rw-rw-   0        0        0   268039 2019-03-09 15:07:37.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery-3.2.1.js
+-rw-rw-rw-   0        0        0      204 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery-fix.js
+-rw-rw-rw-   0        0        0     7200 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery-migrate-1.2.1.min.js
+-rw-rw-rw-   0        0        0    26010 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery-ui-1.10.3.custom.min.css
+-rw-rw-rw-   0        0        0   217071 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery-ui-1.10.3.custom.min.js
+-rw-rw-rw-   0        0        0     4255 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.ba-bbq.min.js
+-rw-rw-rw-   0        0        0     1418 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.highlight.js
+-rw-rw-rw-   0        0        0     1996 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.hotkey.js
+-rw-rw-rw-   0        0        0     8182 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.idle-timer.js
+-rw-rw-rw-   0        0        0    93069 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.js
+-rw-rw-rw-   0        0        0   120545 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.jsPlumb-1.3.10-all-min.js
+-rw-rw-rw-   0        0        0    40914 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.tablesorter.js
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:56.807607 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/
+-rw-rw-rw-   0        0        0    13334 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/CLDRPluralRuleParser.js
+-rw-rw-rw-   0        0        0    13513 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.emitter.bidi.js
+-rw-rw-rw-   0        0        0     5561 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.emitter.js
+-rw-rw-rw-   0        0        0     4261 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.fallbacks.js
+-rw-rw-rw-   0        0        0     9027 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.js
+-rw-rw-rw-   0        0        0    12427 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.language.js
+-rw-rw-rw-   0        0        0     3749 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.messagestore.js
+-rw-rw-rw-   0        0        0     8483 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.parser.js
+-rw-rw-rw-   0        0        0    10847 2019-10-06 20:19:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/language_data.js
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:56.880607 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/lib/
+-rw-rw-rw-   0        0        0    20731 2022-02-03 12:41:37.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/lib/hammer.min.js
+-rw-rw-rw-   0        0        0      469 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/lib/prettify.css
+-rw-rw-rw-   0        0        0    17033 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/lib/prettify.js
+-rw-rw-rw-   0        0        0     2541 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/matrixeq.css
+-rw-rw-rw-   0        0        0    27123 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/matrixeq.js
+-rw-rw-rw-   0        0        0      264 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/mchoice-i18n.en.js
+-rw-rw-rw-   0        0        0      202 2020-12-09 10:35:50.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/mchoice-i18n.sr-Cyrl.js
+-rw-rw-rw-   0        0        0    20787 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/mchoice.js
+-rw-rw-rw-   0        0        0     3014 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/merge.css
+-rw-rw-rw-   0        0        0    20969 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/merge.js
+-rw-rw-rw-   0        0        0     1335 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/modal-basic.css
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.913498 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/msg/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:56.901608 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/msg/js/
+-rw-rw-rw-   0        0        0    28326 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/msg/js/en.js
+-rw-rw-rw-   0        0        0     7117 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/navhelp.js
+-rw-rw-rw-   0        0        0      314 2020-12-09 10:35:50.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/parsons-i18n.en.js
+-rw-rw-rw-   0        0        0      365 2020-12-09 10:35:50.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/parsons-i18n.sr-Cyrl.js
+-rw-rw-rw-   0        0        0     8848 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/parsons.css
+-rw-rw-rw-   0        0        0    97344 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/parsons.js
+-rw-rw-rw-   0        0        0      417 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/poll.css
+-rw-rw-rw-   0        0        0     6877 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/poll.js
+-rw-rw-rw-   0        0        0     3664 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/presenter_mode.css
+-rw-rw-rw-   0        0        0     6290 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/presenter_mode.js
+-rw-rw-rw-   0        0        0   231869 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/processing-1.4.1.min.js
+-rw-rw-rw-   0        0        0     4463 2019-10-06 20:19:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/pygments.css
+-rw-rw-rw-   0        0        0    12629 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/python.js
+-rw-rw-rw-   0        0        0    30613 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/python_compressed.js
+-rw-rw-rw-   0        0        0    18580 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/pytutor.css
+-rw-rw-rw-   0        0        0   159859 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/pytutor.js
+-rw-rw-rw-   0        0        0    44234 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/rangy-core.js
+-rw-rw-rw-   0        0        0    26515 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/rangy-cssclassapplier.js
+-rw-rw-rw-   0        0        0    14204 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/rangy-textrange.js
+-rw-rw-rw-   0        0        0     7907 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/reveal.js
+-rw-rw-rw-   0        0        0    13625 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/runestone-custom-sphinx-bootstrap.css
+-rw-rw-rw-   0        0        0     4326 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/runestonebase.js
+-rw-rw-rw-   0        0        0     2181 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/runestonevideo.js
+-rw-rw-rw-   0        0        0    15059 2019-03-10 08:47:02.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/searchtools.js
+-rw-rw-rw-   0        0        0   106155 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/sharedb.js
+-rw-rw-rw-   0        0        0        0 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/shortanswer.css
+-rw-rw-rw-   0        0        0     8135 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/shortanswer.js
+-rw-rw-rw-   0        0        0      631 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/showEval.css
+-rw-rw-rw-   0        0        0     5939 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/showEval.js
+-rw-rw-rw-   0        0        0   472567 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/skulpt-stdlib.js
+-rw-rw-rw-   0        0        0   483003 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/skulpt.min.js
+-rw-rw-rw-   0        0        0    14765 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/sortmodels.js
+-rw-rw-rw-   0        0        0     1314 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/sortviewers.js
+-rw-rw-rw-   0        0        0     6509 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/style.css
+-rw-rw-rw-   0        0        0      526 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/tabbedstuff.css
+-rw-rw-rw-   0        0        0     6176 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/tabbedstuff.js
+-rw-rw-rw-   0        0        0    34671 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timed.js
+-rw-rw-rw-   0        0        0     2781 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timed_activecode.js
+-rw-rw-rw-   0        0        0     1380 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timed_shortanswer.js
+-rw-rw-rw-   0        0        0     1913 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timedclickable.js
+-rw-rw-rw-   0        0        0     1885 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timeddnd.js
+-rw-rw-rw-   0        0        0     1806 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timedfitb.js
+-rw-rw-rw-   0        0        0     5551 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timedmc.js
+-rw-rw-rw-   0        0        0      578 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timedparsons.js
+-rw-rw-rw-   0        0        0    35168 2019-03-03 11:08:43.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/underscore-1.3.1.js
+-rw-rw-rw-   0        0        0    12140 2019-03-03 11:08:43.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/underscore.js
+-rw-rw-rw-   0        0        0     1839 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/user-highlights.css
+-rw-rw-rw-   0        0        0     9337 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/user-highlights.js
+-rw-rw-rw-   0        0        0      489 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/video.css
+-rw-rw-rw-   0        0        0     8051 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/waypoints.min.js
+-rw-rw-rw-   0        0        0      275 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/webgldemo.css
+-rw-rw-rw-   0        0        0     4541 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/webglinteractive.css
+-rw-rw-rw-   0        0        0    18025 2019-09-29 18:45:24.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/webglinteractive.js
+-rw-rw-rw-   0        0        0    25355 2019-03-10 08:47:02.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/websupport.js
+-rw-rw-rw-   0        0        0    12741 2019-09-29 18:45:23.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/xml.js
+-rw-rw-rw-   0        0        0      398 2019-10-06 20:19:31.000000 petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/searchindex.js
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:56.921608 petljadoc-1.3.3/petljadoc/scorm-proxy-templates/
+-rw-rw-rw-   0        0        0     4508 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/scorm-proxy-templates/adlcp_rootv1p2.xsd
+-rw-rw-rw-   0        0        0   100404 2022-12-02 13:00:34.000000 petljadoc-1.3.3/petljadoc/scorm-proxy-templates/bundle.js
+-rw-rw-rw-   0        0        0    10462 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/scorm-proxy-templates/favicon.ico
+-rw-rw-rw-   0        0        0     1236 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/scorm-proxy-templates/ims_xml.xsd
+-rw-rw-rw-   0        0        0    14820 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/scorm-proxy-templates/imscp_rootv1p1p2.xsd
+-rw-rw-rw-   0        0        0     1184 2023-03-06 12:31:02.000000 petljadoc-1.3.3/petljadoc/scorm-proxy-templates/imsmanifest.t.xml
+-rw-rw-rw-   0        0        0    19397 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/scorm-proxy-templates/imsmd_rootv1p2p1.xsd
+-rw-rw-rw-   0        0        0     1525 2022-12-02 13:00:34.000000 petljadoc-1.3.3/petljadoc/scorm-proxy-templates/index.t.html
+-rw-rw-rw-   0        0        0    18985 2023-01-10 11:56:30.000000 petljadoc-1.3.3/petljadoc/scorm-proxy-templates/style-player.css
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:56.925608 petljadoc-1.3.3/petljadoc/scorm-templates/
+-rw-rw-rw-   0        0        0     4508 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/scorm-templates/adlcp_rootv1p2.xsd
+-rw-rw-rw-   0        0        0     1236 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/scorm-templates/ims_xml.xsd
+-rw-rw-rw-   0        0        0    14820 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/scorm-templates/imscp_rootv1p1p2.xsd
+-rw-rw-rw-   0        0        0    19397 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/scorm-templates/imsmd_rootv1p2p1.xsd
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:56.927606 petljadoc-1.3.3/petljadoc/themes/
+-rw-rw-rw-   0        0        0       83 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:56.931608 petljadoc-1.3.3/petljadoc/themes/bc_theme/
+-rw-rw-rw-   0        0        0      386 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/__init__.py
+-rw-rw-rw-   0        0        0     5931 2023-03-15 11:59:27.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/layout.html
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.918498 petljadoc-1.3.3/petljadoc/themes/bc_theme/locale/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.916497 petljadoc-1.3.3/petljadoc/themes/bc_theme/locale/en/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:56.933606 petljadoc-1.3.3/petljadoc/themes/bc_theme/locale/en/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      968 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/locale/en/LC_MESSAGES/shpinx.mo
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.917498 petljadoc-1.3.3/petljadoc/themes/bc_theme/locale/sr/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:56.935606 petljadoc-1.3.3/petljadoc/themes/bc_theme/locale/sr/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1260 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/locale/sr/LC_MESSAGES/sphinx.mo
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.917498 petljadoc-1.3.3/petljadoc/themes/bc_theme/locale/sr@latn/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:56.934607 petljadoc-1.3.3/petljadoc/themes/bc_theme/locale/sr@latn/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1007 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/locale/sr@latn/LC_MESSAGES/sphinx.mo
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.918498 petljadoc-1.3.3/petljadoc/themes/bc_theme/locale/sr_RS/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:56.936606 petljadoc-1.3.3/petljadoc/themes/bc_theme/locale/sr_RS/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1260 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/locale/sr_RS/LC_MESSAGES/sphinx.mo
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:56.937605 petljadoc-1.3.3/petljadoc/themes/bc_theme/platform/
+-rw-rw-rw-   0        0        0     8733 2022-12-02 13:00:34.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/platform/petljaRTBundle.js
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:56.960606 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.920498 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/bootstrap-4.0.0-dist/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:56.962607 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/bootstrap-4.0.0-dist/css/
+-rw-rw-rw-   0        0        0   144836 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/bootstrap-4.0.0-dist/css/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:56.965610 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/bootstrap-4.0.0-dist/js/
+-rw-rw-rw-   0        0        0    67698 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/bootstrap-4.0.0-dist/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0    48907 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/bootstrap-4.0.0-dist/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0      906 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/bootstrap-sphinx.css_t
+-rw-rw-rw-   0        0        0     3776 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/bootstrap-sphinx.js
+-rw-rw-rw-   0        0        0   100404 2022-12-02 13:00:34.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/bundle.js
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:56.967606 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/css/
+-rw-rw-rw-   0        0        0    31004 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/css/font-awesome.min.css
+-rw-rw-rw-   0        0        0    10462 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/favicon.ico
+-rw-rw-rw-   0        0        0   127331 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/flatly.min.css
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:56.986606 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/fonts/
+-rw-rw-rw-   0        0        0   134808 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/fonts/FontAwesome.otf
+-rw-rw-rw-   0        0        0   165742 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.eot
+-rw-rw-rw-   0        0        0   447050 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.svg
+-rw-rw-rw-   0        0        0   165548 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.ttf
+-rw-rw-rw-   0        0        0    98024 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.woff
+-rw-rw-rw-   0        0        0    77160 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.woff2
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:56.998607 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/images/
+-rw-rw-rw-   0        0        0    69642 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/images/choice-background.svg
+-rw-rw-rw-   0        0        0    69619 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/images/dragndrop-background.svg
+-rw-rw-rw-   0        0        0    69642 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/images/fitb-background.svg
+-rw-rw-rw-   0        0        0      715 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/images/logo.svg
+-rw-rw-rw-   0        0        0     1224 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/images/netkabinet-logo-strelica-wt.svg
+-rw-rw-rw-   0        0        0    69646 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/images/parsons-background.svg
+-rw-rw-rw-   0        0        0      782 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/images/petlja-logo-wt.svg
+-rw-rw-rw-   0        0        0     1618 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/images/play_button.svg
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:57.047607 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/
+-rw-rw-rw-   0        0        0     3152 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/Facebook.png
+-rw-rw-rw-   0        0        0     3079 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/Facebook_icon.png
+-rw-rw-rw-   0        0        0     3728 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/Twitter.png
+-rw-rw-rw-   0        0        0     3177 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/Twitter_icon.png
+-rw-rw-rw-   0        0        0      231 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/active.png
+-rw-rw-rw-   0        0        0      332 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/completed.png
+-rw-rw-rw-   0        0        0     3482 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/dragndrop-img.svg
+-rw-rw-rw-   0        0        0    18186 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/favicon.ico
+-rw-rw-rw-   0        0        0      640 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/fitb-img.svg
+-rw-rw-rw-   0        0        0     5334 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/green-coin.png
+-rw-rw-rw-   0        0        0      447 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/infonote-img.svg
+-rw-rw-rw-   0        0        0      828 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/karel-ball.png
+-rw-rw-rw-   0        0        0     7370 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/karel-east-balls.png
+-rw-rw-rw-   0        0        0     5362 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/karel-east.png
+-rw-rw-rw-   0        0        0     8203 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/karel-head.png
+-rw-rw-rw-   0        0        0     6942 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/karel-hole.png
+-rw-rw-rw-   0        0        0     5910 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/karel-north-balls.png
+-rw-rw-rw-   0        0        0     7338 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/karel-north.png
+-rw-rw-rw-   0        0        0     6842 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/karel-south-balls.png
+-rw-rw-rw-   0        0        0    12370 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/karel-south.png
+-rw-rw-rw-   0        0        0    65211 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/karel-west-balls.png
+-rw-rw-rw-   0        0        0     7920 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/karel-west.png
+-rw-rw-rw-   0        0        0     2857 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/learnmorenote-img.svg
+-rw-rw-rw-   0        0        0    37014 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/logo.png
+-rw-rw-rw-   0        0        0   102151 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/logo_small.png
+-rw-rw-rw-   0        0        0     1224 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/netkabinet-logo-strelica-wt.svg
+-rw-rw-rw-   0        0        0     1434 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/parsons-img.svg
+-rw-rw-rw-   0        0        0      782 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/petlja-logo-wt.svg
+-rw-rw-rw-   0        0        0     5841 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/play_overlay_icon.png
+-rw-rw-rw-   0        0        0      640 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/qchoice-img.svg
+-rw-rw-rw-   0        0        0     4750 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/question-mark-old.png
+-rw-rw-rw-   0        0        0     1327 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/question-mark.png
+-rw-rw-rw-   0        0        0     1327 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/questionnote-img.svg
+-rw-rw-rw-   0        0        0     3186 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/suggestionnote-img.svg
+-rw-rw-rw-   0        0        0     3662 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/technicalnote-img.svg
+-rw-rw-rw-   0        0        0    24003 2022-12-02 13:00:34.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/petlja-course.css
+-rw-rw-rw-   0        0        0     4607 2023-03-06 12:31:02.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/petlja.js
+-rw-rw-rw-   0        0        0    88628 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/require.js
+-rw-rw-rw-   0        0        0    47740 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/simanim-0.0.4-py3-none-any.whl
+-rw-rw-rw-   0        0        0   472567 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/skulpt-stdlib.js
+-rw-rw-rw-   0        0        0   483003 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/skulpt.min.js
+-rw-rw-rw-   0        0        0    18985 2022-12-02 13:00:34.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/static/style-player.css
+-rw-rw-rw-   0        0        0     1295 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/bc_theme/theme.conf
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:57.056607 petljadoc-1.3.3/petljadoc/themes/course_theme/
+-rw-rw-rw-   0        0        0      390 2022-11-06 09:12:12.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/__init__.py
+-rw-rw-rw-   0        0        0     5667 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/basic_layout.html
+-rw-rw-rw-   0        0        0     1935 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/course_homepage.html
+-rw-rw-rw-   0        0        0     1675 2023-06-05 12:58:35.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/globaltoc.html
+-rw-rw-rw-   0        0        0     7299 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/layout.html
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.927498 petljadoc-1.3.3/petljadoc/themes/course_theme/locale/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.926498 petljadoc-1.3.3/petljadoc/themes/course_theme/locale/en/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:57.057606 petljadoc-1.3.3/petljadoc/themes/course_theme/locale/en/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      968 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/locale/en/LC_MESSAGES/shpinx.mo
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.927498 petljadoc-1.3.3/petljadoc/themes/course_theme/locale/sr/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:57.061607 petljadoc-1.3.3/petljadoc/themes/course_theme/locale/sr/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1260 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/locale/sr/LC_MESSAGES/sphinx.mo
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.926498 petljadoc-1.3.3/petljadoc/themes/course_theme/locale/sr@latn/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:57.060606 petljadoc-1.3.3/petljadoc/themes/course_theme/locale/sr@latn/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1007 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/locale/sr@latn/LC_MESSAGES/sphinx.mo
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.928498 petljadoc-1.3.3/petljadoc/themes/course_theme/locale/sr_RS/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:57.062607 petljadoc-1.3.3/petljadoc/themes/course_theme/locale/sr_RS/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1260 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/locale/sr_RS/LC_MESSAGES/sphinx.mo
+-rw-rw-rw-   0        0        0      205 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/localtoc.html
+-rw-rw-rw-   0        0        0      810 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/relations.html
+-rw-rw-rw-   0        0        0      170 2022-11-03 09:45:51.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/sourcelink.html
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:57.077606 petljadoc-1.3.3/petljadoc/themes/course_theme/static/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.929498 petljadoc-1.3.3/petljadoc/themes/course_theme/static/bootstrap-4.0.0-dist/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:57.079610 petljadoc-1.3.3/petljadoc/themes/course_theme/static/bootstrap-4.0.0-dist/css/
+-rw-rw-rw-   0        0        0   144836 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/bootstrap-4.0.0-dist/css/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:57.082605 petljadoc-1.3.3/petljadoc/themes/course_theme/static/bootstrap-4.0.0-dist/js/
+-rw-rw-rw-   0        0        0    67698 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/bootstrap-4.0.0-dist/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0    48907 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/bootstrap-4.0.0-dist/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0      906 2022-11-03 09:45:51.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/bootstrap-sphinx.css_t
+-rw-rw-rw-   0        0        0     3776 2022-11-03 09:45:51.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/bootstrap-sphinx.js
+-rw-rw-rw-   0        0        0      401 2022-11-03 09:45:51.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/course-errors.js
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:57.083607 petljadoc-1.3.3/petljadoc/themes/course_theme/static/css/
+-rw-rw-rw-   0        0        0    31004 2022-11-03 09:45:51.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/css/font-awesome.min.css
+-rw-rw-rw-   0        0        0        0 2022-11-03 09:45:51.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/error_log.txt
+-rw-rw-rw-   0        0        0    10462 2022-11-03 09:45:51.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/favicon.ico
+-rw-rw-rw-   0        0        0   127323 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/flatly.min.css
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:57.090606 petljadoc-1.3.3/petljadoc/themes/course_theme/static/fonts/
+-rw-rw-rw-   0        0        0   134808 2022-11-03 09:45:51.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/fonts/FontAwesome.otf
+-rw-rw-rw-   0        0        0   165742 2022-11-03 09:45:51.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.eot
+-rw-rw-rw-   0        0        0   447050 2022-11-03 09:45:51.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.svg
+-rw-rw-rw-   0        0        0   165548 2022-11-03 09:45:51.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.ttf
+-rw-rw-rw-   0        0        0    98024 2022-11-03 09:45:51.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.woff
+-rw-rw-rw-   0        0        0    77160 2022-11-03 09:45:51.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.woff2
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:57.099607 petljadoc-1.3.3/petljadoc/themes/course_theme/static/images/
+-rw-rw-rw-   0        0        0    69642 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/images/choice-background.svg
+-rw-rw-rw-   0        0        0    69619 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/images/dragndrop-background.svg
+-rw-rw-rw-   0        0        0    69642 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/images/fitb-background.svg
+-rw-rw-rw-   0        0        0      715 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/images/logo.svg
+-rw-rw-rw-   0        0        0     1224 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/images/netkabinet-logo-strelica-wt.svg
+-rw-rw-rw-   0        0        0    69646 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/images/parsons-background.svg
+-rw-rw-rw-   0        0        0      782 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/images/petlja-logo-wt.svg
+-rw-rw-rw-   0        0        0     1618 2022-11-03 09:45:51.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/images/play_button.svg
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:57.140609 petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/
+-rw-rw-rw-   0        0        0     3152 2022-11-03 09:45:51.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/Facebook.png
+-rw-rw-rw-   0        0        0     3079 2022-11-03 09:45:51.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/Facebook_icon.png
+-rw-rw-rw-   0        0        0     3728 2022-11-03 09:45:51.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/Twitter.png
+-rw-rw-rw-   0        0        0     3177 2022-11-03 09:45:51.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/Twitter_icon.png
+-rw-rw-rw-   0        0        0      231 2022-11-03 09:45:51.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/active.png
+-rw-rw-rw-   0        0        0      332 2022-11-03 09:45:51.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/completed.png
+-rw-rw-rw-   0        0        0     3482 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/dragndrop-img.svg
+-rw-rw-rw-   0        0        0    18186 2022-11-03 09:45:51.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/favicon.ico
+-rw-rw-rw-   0        0        0      640 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/fitb-img.svg
+-rw-rw-rw-   0        0        0     5334 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/green-coin.png
+-rw-rw-rw-   0        0        0      447 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/infonote-img.svg
+-rw-rw-rw-   0        0        0      828 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/karel-ball.png
+-rw-rw-rw-   0        0        0     7370 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/karel-east-balls.png
+-rw-rw-rw-   0        0        0     5362 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/karel-east.png
+-rw-rw-rw-   0        0        0     8203 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/karel-head.png
+-rw-rw-rw-   0        0        0     6942 2022-11-03 09:45:51.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/karel-hole.png
+-rw-rw-rw-   0        0        0     5910 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/karel-north-balls.png
+-rw-rw-rw-   0        0        0     7338 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/karel-north.png
+-rw-rw-rw-   0        0        0     6842 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/karel-south-balls.png
+-rw-rw-rw-   0        0        0    12370 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/karel-south.png
+-rw-rw-rw-   0        0        0    65211 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/karel-west-balls.png
+-rw-rw-rw-   0        0        0     7920 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/karel-west.png
+-rw-rw-rw-   0        0        0     2857 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/learnmorenote-img.svg
+-rw-rw-rw-   0        0        0    37014 2022-11-03 09:45:51.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/logo.png
+-rw-rw-rw-   0        0        0   102151 2022-11-03 09:45:51.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/logo_small.png
+-rw-rw-rw-   0        0        0     1224 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/netkabinet-logo-strelica-wt.svg
+-rw-rw-rw-   0        0        0     1434 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/parsons-img.svg
+-rw-rw-rw-   0        0        0      782 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/petlja-logo-wt.svg
+-rw-rw-rw-   0        0        0     5841 2022-11-03 09:45:51.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/play_overlay_icon.png
+-rw-rw-rw-   0        0        0      640 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/qchoice-img.svg
+-rw-rw-rw-   0        0        0     4750 2022-11-03 09:45:51.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/question-mark-old.png
+-rw-rw-rw-   0        0        0     1327 2022-11-03 09:45:51.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/question-mark.png
+-rw-rw-rw-   0        0        0     1327 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/questionnote-img.svg
+-rw-rw-rw-   0        0        0     3186 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/suggestionnote-img.svg
+-rw-rw-rw-   0        0        0     3662 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/technicalnote-img.svg
+-rw-rw-rw-   0        0        0   264982 2022-11-20 11:14:54.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/nbstyle.css
+-rw-rw-rw-   0        0        0    23457 2022-12-02 13:00:34.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/petlja-course.css
+-rw-rw-rw-   0        0        0     7226 2023-06-05 12:58:35.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/petlja.js
+-rw-rw-rw-   0        0        0    88628 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/require.js
+-rw-rw-rw-   0        0        0    47740 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/simanim-0.0.4-py3-none-any.whl
+-rw-rw-rw-   0        0        0   472567 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/skulpt-stdlib.js
+-rw-rw-rw-   0        0        0   483003 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/static/skulpt.min.js
+-rw-rw-rw-   0        0        0      859 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/subchapter.html
+-rw-rw-rw-   0        0        0     1297 2022-11-03 09:45:51.000000 petljadoc-1.3.3/petljadoc/themes/course_theme/theme.conf
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:57.147607 petljadoc-1.3.3/petljadoc/themes/runestone_theme/
+-rw-rw-rw-   0        0        0      537 2020-12-09 14:48:07.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/__init__.py
+-rw-rw-rw-   0        0        0     8162 2020-12-29 14:15:02.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/basic_layout.html
+-rw-rw-rw-   0        0        0      372 2020-12-04 12:05:37.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/globaltoc.html
+-rw-rw-rw-   0        0        0     5342 2023-03-06 12:31:02.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/layout.html
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.934498 petljadoc-1.3.3/petljadoc/themes/runestone_theme/locale/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.932498 petljadoc-1.3.3/petljadoc/themes/runestone_theme/locale/en/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:57.148606 petljadoc-1.3.3/petljadoc/themes/runestone_theme/locale/en/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      566 2020-12-09 14:48:07.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/locale/en/LC_MESSAGES/sphinx.mo
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.933498 petljadoc-1.3.3/petljadoc/themes/runestone_theme/locale/sr/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:57.149607 petljadoc-1.3.3/petljadoc/themes/runestone_theme/locale/sr/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      689 2020-12-09 14:48:07.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/locale/sr/LC_MESSAGES/sphinx.mo
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.933498 petljadoc-1.3.3/petljadoc/themes/runestone_theme/locale/sr@latn/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:57.148606 petljadoc-1.3.3/petljadoc/themes/runestone_theme/locale/sr@latn/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      655 2020-12-29 14:15:02.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/locale/sr@latn/LC_MESSAGES/sphinx.mo
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.934498 petljadoc-1.3.3/petljadoc/themes/runestone_theme/locale/sr_RS/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:57.150606 petljadoc-1.3.3/petljadoc/themes/runestone_theme/locale/sr_RS/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      689 2020-12-29 14:15:02.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/locale/sr_RS/LC_MESSAGES/sphinx.mo
+-rw-rw-rw-   0        0        0      187 2020-12-08 00:51:34.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/localtoc.html
+-rw-rw-rw-   0        0        0     1262 2020-12-09 14:48:07.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/relations.html
+-rw-rw-rw-   0        0        0      170 2020-12-04 12:05:37.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/sourcelink.html
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:57.171607 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.936500 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/bootstrap-4.0.0-dist/
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:57.172607 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/bootstrap-4.0.0-dist/css/
+-rw-rw-rw-   0        0        0   144838 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/bootstrap-4.0.0-dist/css/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:57.174607 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/bootstrap-4.0.0-dist/js/
+-rw-rw-rw-   0        0        0    67698 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/bootstrap-4.0.0-dist/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0    48907 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/bootstrap-4.0.0-dist/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0      906 2020-12-04 12:05:37.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/bootstrap-sphinx.css_t
+-rw-rw-rw-   0        0        0     3776 2020-12-04 12:05:37.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/bootstrap-sphinx.js
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:57.175607 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/css/
+-rw-rw-rw-   0        0        0    31004 2020-12-04 12:05:37.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/css/font-awesome.min.css
+-rw-rw-rw-   0        0        0        0 2020-12-29 14:15:02.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/error_log.txt
+-rw-rw-rw-   0        0        0    10462 2020-12-04 12:05:37.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/favicon.ico
+-rw-rw-rw-   0        0        0   127331 2020-12-04 12:05:37.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/flatly.min.css
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:57.194606 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/fonts/
+-rw-rw-rw-   0        0        0   134808 2020-12-04 12:05:37.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/fonts/FontAwesome.otf
+-rw-rw-rw-   0        0        0   165742 2020-12-04 12:05:37.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.eot
+-rw-rw-rw-   0        0        0   447050 2020-12-04 12:05:37.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.svg
+-rw-rw-rw-   0        0        0   165548 2020-12-04 12:05:37.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.ttf
+-rw-rw-rw-   0        0        0    98024 2020-12-04 12:05:37.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.woff
+-rw-rw-rw-   0        0        0    77160 2020-12-04 12:05:37.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.woff2
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:57.202607 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/images/
+-rw-rw-rw-   0        0        0    69642 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/images/choice-background.svg
+-rw-rw-rw-   0        0        0    69619 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/images/dragndrop-background.svg
+-rw-rw-rw-   0        0        0    69642 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/images/fitb-background.svg
+-rw-rw-rw-   0        0        0      715 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/images/logo.svg
+-rw-rw-rw-   0        0        0     1224 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/images/netkabinet-logo-strelica-wt.svg
+-rw-rw-rw-   0        0        0    69646 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/images/parsons-background.svg
+-rw-rw-rw-   0        0        0      782 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/images/petlja-logo-wt.svg
+-rw-rw-rw-   0        0        0     1618 2022-01-26 16:39:18.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/images/play_button.svg
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:57.228607 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/
+-rw-rw-rw-   0        0        0     3152 2022-01-26 16:39:18.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/Facebook.png
+-rw-rw-rw-   0        0        0     3079 2022-01-26 16:39:18.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/Facebook_icon.png
+-rw-rw-rw-   0        0        0     3728 2022-01-26 16:39:18.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/Twitter.png
+-rw-rw-rw-   0        0        0     3177 2022-01-26 16:39:18.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/Twitter_icon.png
+-rw-rw-rw-   0        0        0      231 2022-01-26 16:39:18.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/active.png
+-rw-rw-rw-   0        0        0      332 2022-01-26 16:39:18.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/completed.png
+-rw-rw-rw-   0        0        0     3482 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/dragndrop-img.svg
+-rw-rw-rw-   0        0        0    18186 2022-01-26 16:39:18.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/favicon.ico
+-rw-rw-rw-   0        0        0      640 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/fitb-img.svg
+-rw-rw-rw-   0        0        0     5334 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/green-coin.png
+-rw-rw-rw-   0        0        0      447 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/infonote-img.svg
+-rw-rw-rw-   0        0        0    10414 2022-01-26 16:39:18.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/karel-ball.png
+-rw-rw-rw-   0        0        0    19798 2022-01-26 16:39:18.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/karel-east.png
+-rw-rw-rw-   0        0        0     8203 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/karel-head.png
+-rw-rw-rw-   0        0        0     6942 2022-01-26 16:39:18.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/karel-hole.png
+-rw-rw-rw-   0        0        0    13690 2022-01-26 16:39:18.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/karel-north.png
+-rw-rw-rw-   0        0        0    14972 2022-01-26 16:39:18.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/karel-south.png
+-rw-rw-rw-   0        0        0    19805 2022-01-26 16:39:18.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/karel-west.png
+-rw-rw-rw-   0        0        0     2857 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/learnmorenote-img.svg
+-rw-rw-rw-   0        0        0    37014 2022-01-26 16:39:18.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/logo.png
+-rw-rw-rw-   0        0        0   102151 2022-01-26 16:39:18.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/logo_small.png
+-rw-rw-rw-   0        0        0     1224 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/netkabinet-logo-strelica-wt.svg
+-rw-rw-rw-   0        0        0     1434 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/parsons-img.svg
+-rw-rw-rw-   0        0        0      782 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/petlja-logo-wt.svg
+-rw-rw-rw-   0        0        0     5841 2022-01-26 16:39:18.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/play_overlay_icon.png
+-rw-rw-rw-   0        0        0      640 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/qchoice-img.svg
+-rw-rw-rw-   0        0        0     4750 2022-01-26 16:39:18.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/question-mark-old.png
+-rw-rw-rw-   0        0        0     1327 2022-01-26 16:39:18.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/question-mark.png
+-rw-rw-rw-   0        0        0     1327 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/questionnote-img.svg
+-rw-rw-rw-   0        0        0     3186 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/suggestionnote-img.svg
+-rw-rw-rw-   0        0        0     3662 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/technicalnote-img.svg
+-rw-rw-rw-   0        0        0   277929 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/nbstyle.css
+-rw-rw-rw-   0        0        0     2821 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/petlja-runestone.css
+-rw-rw-rw-   0        0        0        0 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/petlja_ruenstone.js
+-rw-rw-rw-   0        0        0    88628 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/require.js
+-rw-rw-rw-   0        0        0    47740 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/simanim-0.0.4-py3-none-any.whl
+-rw-rw-rw-   0        0        0   472567 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/skulpt-stdlib.js
+-rw-rw-rw-   0        0        0   483003 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/skulpt.min.js
+-rw-rw-rw-   0        0        0     1264 2020-12-09 14:48:07.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/subchapter.html
+-rw-rw-rw-   0        0        0     1297 2020-12-04 12:05:37.000000 petljadoc-1.3.3/petljadoc/themes/runestone_theme/theme.conf
+-rw-rw-rw-   0        0        0     4478 2022-11-06 13:07:32.000000 petljadoc-1.3.3/petljadoc/util.py
+drwxrwxrwx   0        0        0        0 2023-06-05 12:58:49.978497 petljadoc-1.3.3/petljadoc.egg-info/
+-rw-rw-rw-   0        0        0     3407 2023-06-05 12:58:49.000000 petljadoc-1.3.3/petljadoc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    51038 2023-06-05 12:58:49.000000 petljadoc-1.3.3/petljadoc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 12:58:49.000000 petljadoc-1.3.3/petljadoc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      293 2023-06-05 12:58:49.000000 petljadoc-1.3.3/petljadoc.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2019-09-30 21:36:41.000000 petljadoc-1.3.3/petljadoc.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      195 2023-06-05 12:58:49.000000 petljadoc-1.3.3/petljadoc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-05 12:58:49.000000 petljadoc-1.3.3/petljadoc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      210 2023-03-06 12:48:22.000000 petljadoc-1.3.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 12:58:57.230608 petljadoc-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1707 2022-11-20 11:14:54.000000 petljadoc-1.3.3/setup.py
```

### Comparing `petljadoc-1.3.1/LICENSE` & `petljadoc-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/PKG-INFO` & `petljadoc-1.3.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,16 @@
-Metadata-Version: 2.1
-Name: petljadoc
-Version: 1.3.1
-Summary: Petlja's command-line interface for learning content
-Home-page: https://github.com/Petlja/PetljaDoc
-Author: Fondacija Petlja
-Author-email: team@petlja.org
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Education
-Classifier: Topic :: Text Processing :: Markup
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PetljaDoc - Petlja's tool for eLearning content
 
 The tool is based on https://github.com/RunestoneInteractive/RunestoneComponents and https://github.com/sphinx-doc/sphinx and includes:
 
-- additional Sphinx extensions 
+- additional Sphinx extensions
 - partial Pygame implementation for Sculpt (https://github.com/Petlja/pygame4skulpt)
 - additional ActiveCode features
-- customized Sphinx theme 
-- customized project template 
+- customized Sphinx theme
+- customized project template
 - exteded online course format
 - ``petljadoc`` command line interface (CLI)
 
 PetljaDoc currently depends on forked RunestoneComonents, but we are gradually closing the gap with the upstream repository through pull requests.
 
 ## Installation
 
@@ -41,23 +23,24 @@
 `py -3 -m pip install petljadoc`
 
 ## CLI usage
 
 `petljadoc [OPTIONS] COMMAND [ARGS]...`
 
 Options:
-  - `--help`&nbsp;&nbsp;&nbsp;&nbsp;Show help message 
+
+- `--help`&nbsp;&nbsp;&nbsp;&nbsp;Show help message
 
 Commands:
-  - `init-course`&nbsp;&nbsp;&nbsp;&nbsp;Create a new online course project in your current directory
-  - `init-runestone`&nbsp;&nbsp;&nbsp;&nbsp;Create a new Runestone project in your current directory
-  - `preview`&nbsp;&nbsp;&nbsp;&nbsp;Build the project, open it in a web browser, watch for changes, rebuild changed files and refresh browser after rebuild (using [sphinx-autobuild](https://github.com/GaretJax/sphinx-autobuild))
-  - `publish`&nbsp;&nbsp;&nbsp;&nbsp;Build the project and copy produced content in `docs` subfolder (ready to be published using GitHub Pages)
+
+- `init-course`&nbsp;&nbsp;&nbsp;&nbsp;Create a new online course project in your current directory
+- `init-runestone`&nbsp;&nbsp;&nbsp;&nbsp;Create a new Runestone project in your current directory
+- `preview`&nbsp;&nbsp;&nbsp;&nbsp;Build the project, open it in a web browser, watch for changes, rebuild changed files and refresh browser after rebuild (using [sphinx-autobuild](https://github.com/GaretJax/sphinx-autobuild))
+- `publish`&nbsp;&nbsp;&nbsp;&nbsp;Build the project and copy produced content in `docs` subfolder (ready to be published using GitHub Pages)
+- `export`&nbsp;&nbsp;&nbsp; &nbsp;Builds the project and exports its content as a SCORM package. You can select one of the 3 options with will deliver you diffrent type of packages:
+  - `single`: A single SCO (Shareable Content Object) SCORM package, which contains all course content in a single file
+  - `multi`: A multi SCO SCORM package, which breaks the course content into multiple modules or units
+  - `proxy`: A proxy SCORM package, that can be used with a Learning Management System (LMS) and an additional Moodle backup file. This option requires you to upload your course files to a web server and provide a link to the packager via `package-conf.json`. We recommend to upload your course files to a web server like GitHub Pages, which allows you to host static web content for free. You can create a new repository for your course files and enable GitHub Pages to generate a website URL for your repository. Then, you can update `package-conf.json` to include the GitHub Pages URL as the `data_content_url` property.
 
 By using `petljadoc preview`, an author may keep opened a browser window for preview. Any saved changes will be updated in browser in about 5-10 seconds.
 
 `petljadoc publish` command helps an author to share a public preview of his work via GitHub Pages.
-
-
-
-
-
```

### Comparing `petljadoc-1.3.1/petljadoc/cli.py` & `petljadoc-1.3.3/petljadoc/cli.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/course.py` & `petljadoc-1.3.3/petljadoc/course.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/nb-templates/classic2/base/base.html.j2` & `petljadoc-1.3.3/petljadoc/nb-templates/classic2/base/base.html.j2`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/nb-templates/classic2/base/display_priority.j2` & `petljadoc-1.3.3/petljadoc/nb-templates/classic2/base/display_priority.j2`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/nb-templates/classic2/base/jupyter_widgets.html.j2` & `petljadoc-1.3.3/petljadoc/nb-templates/classic2/base/jupyter_widgets.html.j2`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/nb-templates/classic2/base/mathjax.html.j2` & `petljadoc-1.3.3/petljadoc/nb-templates/classic2/base/mathjax.html.j2`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/nb-templates/classic2/base/null.j2` & `petljadoc-1.3.3/petljadoc/nb-templates/classic2/base/null.j2`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/package.py` & `petljadoc-1.3.3/petljadoc/package.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/petlja_builder.py` & `petljadoc-1.3.3/petljadoc/petlja_builder.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/project-templates/course/_sources/1_Lesson/intro.rst` & `petljadoc-1.3.3/petljadoc/project-templates/course/_sources/1_Lesson/intro.rst`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/project-templates/course/_sources/1_Lesson/quiz.rst` & `petljadoc-1.3.3/petljadoc/project-templates/course/_sources/1_Lesson/quiz.rst`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/project-templates/course/_sources/index.t.yaml` & `petljadoc-1.3.3/petljadoc/project-templates/course/_sources/index.t.yaml`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/project-templates/course/conf.t.py` & `petljadoc-1.3.3/petljadoc/project-templates/course/conf.t.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/project-templates/course/pavement.t.py` & `petljadoc-1.3.3/petljadoc/project-templates/course/pavement.t.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/project-templates/runestone/_sources/index.rst` & `petljadoc-1.3.3/petljadoc/project-templates/runestone/_sources/index.rst`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/activecodethumb.png` & `petljadoc-1.3.3/petljadoc/project-templates/runestone/_static/activecodethumb.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line01.mp3` & `petljadoc-1.3.3/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line01.mp3`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line01.wav` & `petljadoc-1.3.3/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line01.wav`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line02.mp3` & `petljadoc-1.3.3/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line02.mp3`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line02.wav` & `petljadoc-1.3.3/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line02.wav`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line03.mp3` & `petljadoc-1.3.3/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line03.mp3`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line03.wav` & `petljadoc-1.3.3/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line03.wav`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/clock.png` & `petljadoc-1.3.3/petljadoc/project-templates/runestone/_static/clock.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/close.png` & `petljadoc-1.3.3/petljadoc/project-templates/runestone/_static/close.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/first.png` & `petljadoc-1.3.3/petljadoc/project-templates/runestone/_static/first.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/last.png` & `petljadoc-1.3.3/petljadoc/project-templates/runestone/_static/last.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/next.png` & `petljadoc-1.3.3/petljadoc/project-templates/runestone/_static/next.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/pause.png` & `petljadoc-1.3.3/petljadoc/project-templates/runestone/_static/pause.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/prev.png` & `petljadoc-1.3.3/petljadoc/project-templates/runestone/_static/prev.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/project-templates/runestone/conf.t.py` & `petljadoc-1.3.3/petljadoc/project-templates/runestone/conf.t.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/project-templates/runestone/pavement.t.py` & `petljadoc-1.3.3/petljadoc/project-templates/runestone/pavement.t.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/__init__.py` & `petljadoc-1.3.3/petljadoc/runestone_ext/__init__.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/associations/associations.py` & `petljadoc-1.3.3/petljadoc/runestone_ext/associations/associations.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/associations/css/associations.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/associations/css/associations.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/associations/js/associations.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/associations/js/associations.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/audio/audio.py` & `petljadoc-1.3.3/petljadoc/runestone_ext/audio/audio.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockly/blocklykarel.py` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockly/blocklykarel.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,15 @@
         """
         generate html to include Karel box.
         :param self:
         :return:
         """
 
         env = self.state.document.settings.env
-        categories = ["KarelCommands", "BeginnerKarelCommands","KarelBrain","Values", "Branching", "KarelBranching", "Loops", "KarelLoops", "Arithmetic", "Logic", "KarelSays", "AskUser", "Vars"]
+        categories = ["KarelCommands", "BeginnerKarelCommands", "KarelStreightLineCommands","KarelBrain","Values", "Branching", "KarelBranching", "Loops", "KarelLoops", "Arithmetic", "Logic", "KarelSays", "AskUser", "Vars"]
         self.options['name'] = self.arguments[0].strip()
         self.options['divid'] = self.arguments[0]
 
         if not self.options['divid']:
             raise Exception("No divid")
 
 
@@ -153,14 +153,15 @@
             source = '\n'
 
         if 'categories' in self.options:
             author_categories = [categoty.strip() for categoty in self.options['categories'].split(',') if categoty.strip() in categories]
             self.options['data_categories'] = json.dumps(author_categories)
         else:
             categories.remove('BeginnerKarelCommands')
+            categories.remove('KarelStreightLineCommands')
             self.options['data_categories'] = json.dumps(categories)
         if 'exportmode' in self.options:
             self.options['export_button'] = '<button class="btn btn-default export-button">Сачувај стање</button>'
         else:
             self.options['export_button'] = ''
 
         if 'flyouttoolbox' in self.options:
```

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockly/css/karelBlockly.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockly/css/karelBlockly.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockly/js/acorn_interpreter.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockly/js/acorn_interpreter.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockly/js/blockly_compressed.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockly/js/blockly_compressed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockly/js/blocks_compressed.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockly/js/blocks_compressed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockly/js/javascript_compressed.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockly/js/javascript_compressed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockly/js/karelBlockly.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockly/js/karelBlockly.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -86,14 +86,29 @@
                     "kind": "block",
                     "type": "turn_right"
                 }, {
                     "kind": "block",
                     "type": "pick_up"
                 }, ]
             },
+            'KarelStreightLineCommands': {
+                "kind": "category",
+                "name": "Наредбе роботу",
+                "colour": 295,
+                "contents": [{
+                    "kind": "block",
+                    "type": "move",
+                }, {
+                    "kind": "block",
+                    "type": "move_back",
+                }, {
+                    "kind": "block",
+                    "type": "pick_up"
+                }, ]
+            },
             'KarelBrain': {
                 "kind": "category",
                 "name": "Питај робота",
                 "colour": 275,
                 "contents": [{
                     "kind": "block",
                     "type": "balls_present",
@@ -297,14 +312,19 @@
                 interpreter.setProperty(globalObject, 'prompt', interpreter.createNativeFunction(wrapper));
                 wrapper = function() {
                     robot.move();
                     drawer.drawFrame(robot.clone());
                 };
                 interpreter.setProperty(globalObject, 'move_forward', interpreter.createNativeFunction(wrapper));
                 wrapper = function() {
+                    robot.moveBack();
+                    drawer.drawFrame(robot.clone());
+                };
+                interpreter.setProperty(globalObject, 'move_backward', interpreter.createNativeFunction(wrapper));
+                wrapper = function() {
                     robot.turnLeft();
                     drawer.drawFrame(robot.clone());
                 };
                 interpreter.setProperty(globalObject, 'turn_left', interpreter.createNativeFunction(wrapper));
                 wrapper = function() {
                     robot.turnRight();
                     drawer.drawFrame(robot.clone());
```

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockly/js/karelBlocks.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockly/js/karelBlocks.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -15,14 +15,34 @@
 };
 
 Blockly.JavaScript['move'] = function(block) {
     // Generate JavaScript for moving forward.
     return 'move_forward()\n';
 };
 
+Blockly.Blocks['move_back'] = {
+    /**
+     * Block for moving karel forward.
+     * @this {Blockly.Block}
+     */
+    init: function() {
+        this.jsonInit({
+            "message0": 'корак назад',
+            "previousStatement": null,
+            "nextStatement": null,
+            "colour": 250,
+            "tooltip": 'Робот се помера једно поље у назад.'
+        });
+    }
+};
+
+Blockly.JavaScript['move_back'] = function(block) {
+    // Generate JavaScript for moving forward.
+    return 'move_backward()\n';
+};
 Blockly.Blocks['turn_left'] = {
     /**
      * Block for moving forward.
      * @this {Blockly.Block}
      */
     init: function() {
         this.jsonInit({
```

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockly/js/msg/en.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockly/js/msg/en.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockly/js/msg/sr.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockly/js/msg/sr.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/blockpylib.py` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/blockpylib.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockly/blockly_compressed.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockly/blockly_compressed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockly/blocks_compressed.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockly/blocks_compressed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockly/msg-sr.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockly/msg-sr.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockly/python_compressed.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockly/python_compressed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/abstract_interpreter.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/abstract_interpreter.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/abstract_interpreter_definitions.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/abstract_interpreter_definitions.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/ast_node_visitor.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/ast_node_visitor.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/class.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/class.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/comment.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/comment.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/comprehensions.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/comprehensions.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/decorator.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/decorator.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/dict.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/dict.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/if.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/if.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/io.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/io.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/lists.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/lists.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/loops.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/loops.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/parking.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/parking.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/plots.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/plots.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/sets.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/sets.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/text.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/text.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/tuple.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/tuple.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/turtles.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/turtles.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/imported.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/imported.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/python_errors.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/python_errors.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/python_to_blockly.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/python_to_blockly.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/pytifa.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/pytifa.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/utilities.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy/utilities.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy-modal.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/js/blockpy-modal.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/bootstrap.min.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/bootstrap.min.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-sphinx.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-sphinx.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/dbDirective/css/dbDirective.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/dbDirective/css/dbDirective.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/dbDirective/dbDirective.py` & `petljadoc-1.3.3/petljadoc/runestone_ext/dbDirective/dbDirective.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/dbDirective/js/dbDirective.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/dbDirective/js/dbDirective.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/dbDirective/js/sql.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/dbDirective/js/sql.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/editor/css/editor.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/editor/css/editor.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/editor/editor.py` & `petljadoc-1.3.3/petljadoc/runestone_ext/editor/editor.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/editor/js/editor.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/editor/js/editor.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/editor/js/jszip.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/editor/js/jszip.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/gallery/css/gallery.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/gallery/css/gallery.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/gallery/gallery.py` & `petljadoc-1.3.3/petljadoc/runestone_ext/gallery/gallery.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/gallery/js/gallery.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/gallery/js/gallery.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/karel/css/karel.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/karel/css/karel.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/karel-i18n.sr-Cyrl.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/karel/js/karel-i18n.sr-Cyrl.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/karel-i18n.sr.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/karel/js/karel-i18n.sr.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/karel.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/karel/js/karel.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/karelChat.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/karel/js/karelChat.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/karelCorner.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/karel/js/karelCorner.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/karelRobot.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelRobot.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -17,23 +17,17 @@
         r.location.y = this.location.y;
         r.direction = this.direction;
         r.numBalls = this.numBalls;
         r.infiniteBalls = this.infiniteBalls;
         r.lastMessage = this.lastMessage;
         r.messagesOn = this.messagesOn;
         r.world = this.world.clone();
-        if (this.chat)
-            r.chat = this.chat.clone();
         return r;
     }
 
-    Robot.prototype.setChat = function(c) {
-        this.chat = c;
-    }
-
     Robot.prototype.setWorld = function(w) {
         this.world = w;
         this.location.x = w.getRobotStartAvenue();
         this.location.y = w.getRobotStartStreet();
         this.direction = w.getRobotStartDirection();
     };
 
@@ -207,25 +201,15 @@
 
     Robot.prototype.turnMessagesOn = function() {
         this.messagesOn = true;
     };
 
     Robot.prototype.turnMessagesOff = function() {
         this.messagesOn = false;
-    };
+    }
 
     Robot.prototype.getLastMessage = function() {
         return this.lastMessage;
     };
 
-
-    Robot.prototype.clearMessages = function() {
-        this.chat.clearMessages();
-    }
-    Robot.prototype.showMessage = function(message) {
-        this.chat.showMessage(message);
-        this.lastMessage = message;
-    }
-
-
     return Robot;
 })();
```

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/karelRobotDrawer.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/karel/js/karelRobotDrawer.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/karelUI.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/karel/js/karelUI.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/karelWorld.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/karel/js/karelWorld.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/karel/karel.py` & `petljadoc-1.3.3/petljadoc/runestone_ext/karel/karel.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/bootstrap.min.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/bootstrap.min.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-sphinx.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-sphinx.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/nimgame/css/nimgame.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/nimgame/css/nimgame.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/nimgame/js/nimgame-i18n.sr-Cyrl.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/nimgame/js/nimgame-i18n.sr-Cyrl.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/nimgame/js/nimgame-i18n.sr.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/nimgame/js/nimgame-i18n.sr.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/nimgame/js/nimgame.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/nimgame/js/nimgame.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/nimgame/nimgame.py` & `petljadoc-1.3.3/petljadoc/runestone_ext/nimgame/nimgame.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/css/notes.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/css/notes.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/js/notes.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/js/notes.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/notes.py` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/notes.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/bootstrap.min.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/bootstrap.min.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-sphinx.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-sphinx.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/Blob.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/Blob.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/FileSaver.min.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/FileSaver.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/LICENSE.txt` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/accessibility.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/accessibility.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/accessibilitydarkest.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/accessibilitydarkest.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/accessibilitylight.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/accessibilitylight.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/activecode-i18n.en.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/activecode-i18n.en.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/activecode-i18n.sr-Cyrl.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/activecode-i18n.sr-Cyrl.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/activecode.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/activecode.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/activecode.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/activecode.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/animationbase.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/animationbase.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/basic.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/basic.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly/blockly_compressed.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly/blockly_compressed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly/blocks_compressed.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly/blocks_compressed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly/msg-sr.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly/msg-sr.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly/python_compressed.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly/python_compressed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly_compressed.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly_compressed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/abstract_interpreter.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/abstract_interpreter.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/abstract_interpreter_definitions.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/abstract_interpreter_definitions.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/ast_node_visitor.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/ast_node_visitor.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/class.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/class.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/comment.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/comment.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/comprehensions.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/comprehensions.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/decorator.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/decorator.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/dict.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/dict.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/if.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/if.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/io.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/io.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/lists.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/lists.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/loops.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/loops.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/parking.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/parking.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/plots.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/plots.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/sets.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/sets.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/text.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/text.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/tuple.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/tuple.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/turtles.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/turtles.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/imported.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/imported.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/python_errors.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/python_errors.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/python_to_blockly.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/python_to_blockly.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/pytifa.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/pytifa.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/utilities.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/utilities.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy-modal.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy-modal.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blocks_compressed.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blocks_compressed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bookfuncs.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bookfuncs.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-4.0.0-dist/css/bootstrap.min.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-4.0.0-dist/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-4.0.0-dist/js/bootstrap.bundle.min.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-4.0.0-dist/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-4.0.0-dist/js/bootstrap.min.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-4.0.0-dist/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-sphinx.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-sphinx.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap.min.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/clickable.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/clickable.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/clickable.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/clickable.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/clike.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/clike.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/codelens.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/codelens.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/codemirror.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/codemirror.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/codemirror.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/codemirror.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/css/font-awesome.min.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/css.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/css.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/d3.v2.min.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/d3.v2.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/datafile.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/datafile.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/diff_match_patch.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/diff_match_patch.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/doctools.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/dragndrop.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/dragndrop.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/dragndrop.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/dragndrop.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/external.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/external.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/fitb.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/fitb.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/flatly.min.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/flatly.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/guiders-1.3.0.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/guiders-1.3.0.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/guiders-1.3.0.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/guiders-1.3.0.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/htmlmixed.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/htmlmixed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/javascript.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/javascript.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/javascript_compressed.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/javascript_compressed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery-3.2.1.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery-3.2.1.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery-migrate-1.2.1.min.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery-migrate-1.2.1.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery-ui-1.10.3.custom.min.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery-ui-1.10.3.custom.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery-ui-1.10.3.custom.min.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery-ui-1.10.3.custom.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.ba-bbq.min.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.ba-bbq.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.highlight.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.highlight.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.hotkey.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.hotkey.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.idle-timer.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.idle-timer.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.jsPlumb-1.3.10-all-min.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.jsPlumb-1.3.10-all-min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.tablesorter.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.tablesorter.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/CLDRPluralRuleParser.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/CLDRPluralRuleParser.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.emitter.bidi.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.emitter.bidi.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.emitter.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.emitter.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.fallbacks.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.fallbacks.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.language.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.language.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.messagestore.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.messagestore.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.parser.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.parser.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karel.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karel.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karel.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karel.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelCorner.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelCorner.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelRobot.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/karel/js/karelRobot.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -17,17 +17,23 @@
         r.location.y = this.location.y;
         r.direction = this.direction;
         r.numBalls = this.numBalls;
         r.infiniteBalls = this.infiniteBalls;
         r.lastMessage = this.lastMessage;
         r.messagesOn = this.messagesOn;
         r.world = this.world.clone();
+        if (this.chat)
+            r.chat = this.chat.clone();
         return r;
     }
 
+    Robot.prototype.setChat = function(c) {
+        this.chat = c;
+    }
+
     Robot.prototype.setWorld = function(w) {
         this.world = w;
         this.location.x = w.getRobotStartAvenue();
         this.location.y = w.getRobotStartStreet();
         this.direction = w.getRobotStartDirection();
     };
 
@@ -150,14 +156,55 @@
                 } else {
                     this.setAvenue(this.getAvenue() - 1);
                 }
                 break;
         }
     };
 
+    Robot.prototype.moveBack = function() {
+        switch (this.getDirection()) {
+            case "N":
+                if (!(this.world.isInBounds(this.getAvenue(), this.getStreet() - 1))) {
+                    throw "out_of_bounds"
+                } else if (this.world.checkEWWall(this.getAvenue(), this.getStreet() - 1)) {
+                    throw "crashed";
+                } else {
+                    this.setStreet(this.getStreet() - 1);
+                }
+                break;
+            case "S":
+                if (!(this.world.isInBounds(this.getAvenue(), this.getStreet() + 1))) {
+                    throw "out_of_bounds"
+                } else if (this.world.checkEWWall(this.getAvenue(), this.getStreet())) {
+                    throw "crashed";
+                } else {
+                    this.setStreet(this.getStreet() + 1);
+                }
+                break;
+            case "E":
+                if (!(this.world.isInBounds(this.getAvenue() - 1, this.getStreet()))) {
+                    throw "out_of_bounds"
+                } else if (this.world.checkNSWall(this.getAvenue() - 1, this.getStreet())) {
+                    throw "crashed";
+                } else {
+                    this.setAvenue(this.getAvenue() - 1);
+                }
+                break;
+            case "W":
+                if (!(this.world.isInBounds(this.getAvenue() + 1, this.getStreet()))) {
+                    throw "out_of_bounds"
+                } else if (this.world.checkNSWall(this.getAvenue(), this.getStreet())) {
+                    throw "crashed";
+                } else {
+                    this.setAvenue(this.getAvenue() + 1);
+                }
+                break;
+        }
+    };
+
     Robot.prototype.frontIsClear = function() {
         var isDirBlocked = false;
         switch (this.getDirection()) {
             case "N":
                 isDirBlocked = this.world.checkEWWall(this.getAvenue(), this.getStreet());
                 break;
             case "E":
@@ -201,15 +248,25 @@
 
     Robot.prototype.turnMessagesOn = function() {
         this.messagesOn = true;
     };
 
     Robot.prototype.turnMessagesOff = function() {
         this.messagesOn = false;
-    }
+    };
 
     Robot.prototype.getLastMessage = function() {
         return this.lastMessage;
     };
 
+
+    Robot.prototype.clearMessages = function() {
+        this.chat.clearMessages();
+    }
+    Robot.prototype.showMessage = function(message) {
+        this.chat.showMessage(message);
+        this.lastMessage = message;
+    }
+
+
     return Robot;
 })();
```

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelRobotDrawer.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelRobotDrawer.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelUI.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelUI.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelWorld.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelWorld.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/language_data.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/lib/hammer.min.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/lib/hammer.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/lib/prettify.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/lib/prettify.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/matrixeq.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/matrixeq.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/matrixeq.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/matrixeq.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/mchoice.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/mchoice.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/merge.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/merge.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/merge.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/merge.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/modal-basic.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/modal-basic.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/msg/js/en.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/msg/js/en.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/navhelp.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/navhelp.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/parsons.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/parsons.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/parsons.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/parsons.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/petlja.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/petlja.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/poll.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/poll.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/presenter_mode.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/presenter_mode.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/presenter_mode.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/presenter_mode.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/processing-1.4.1.min.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/processing-1.4.1.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/__init__.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/__init__.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/display.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/display.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/draw.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/draw.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/event.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/event.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/font.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/font.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/image.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/image.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/key.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/key.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/mouse.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/mouse.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/time.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/time.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/transform.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/transform.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib-init.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib-init.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygments.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/python.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/python.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/python_compressed.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/python_compressed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pytutor.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pytutor.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pytutor.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pytutor.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/rangy-core.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/rangy-core.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/rangy-cssclassapplier.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/rangy-cssclassapplier.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/rangy-textrange.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/rangy-textrange.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/reveal.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/reveal.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/runestone-custom-sphinx-bootstrap.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/runestone-custom-sphinx-bootstrap.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/runestonebase.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/runestonebase.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/runestonevideo.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/runestonevideo.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/searchtools.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/sharedb.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/sharedb.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/shortanswer.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/shortanswer.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/showEval.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/showEval.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/showEval.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/showEval.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/skulpt-stdlib.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/skulpt-stdlib.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/skulpt.min.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/skulpt.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/sortmodels.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/sortmodels.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/sortviewers.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/sortviewers.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/style.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/style.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/tabbedstuff.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/tabbedstuff.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/tabbedstuff.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/tabbedstuff.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timed.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timed_activecode.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timed_activecode.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timed_shortanswer.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timed_shortanswer.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timedclickable.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timedclickable.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timeddnd.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timeddnd.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timedfitb.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timedfitb.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timedmc.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timedmc.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timedparsons.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timedparsons.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/underscore-1.3.1.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/underscore.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/user-highlights.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/user-highlights.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/user-highlights.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/user-highlights.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/waypoints.min.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/waypoints.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/webglinteractive.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/webglinteractive.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/webglinteractive.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/webglinteractive.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/websupport.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/websupport.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/xml.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/notes/test/build/noteTests/_static/xml.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/p5js/js/p5js.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/p5js/js/p5js.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/p5js/p5js.py` & `petljadoc-1.3.3/petljadoc/runestone_ext/p5js/p5js.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/pycode/css/pycode.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/pycode/css/pycode.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/pycode/js/pycode.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/pycode/js/pycode.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/pycode/pycode.py` & `petljadoc-1.3.3/petljadoc/runestone_ext/pycode/pycode.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/__init__.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/js/pygamelib/__init__.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/display.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/js/pygamelib/display.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/draw.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/js/pygamelib/draw.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/event.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/js/pygamelib/event.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/font.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/js/pygamelib/font.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/image.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/js/pygamelib/image.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/key.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/js/pygamelib/key.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/mouse.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/js/pygamelib/mouse.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/time.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/js/pygamelib/time.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/transform.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/js/pygamelib/transform.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib-init.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/js/pygamelib-init.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/bootstrap.min.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/bootstrap.min.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-sphinx.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-sphinx.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/test/conf.py` & `petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/test/conf.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/test/pavement.py` & `petljadoc-1.3.3/petljadoc/runestone_ext/pygamelib/test/pavement.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/quizq/quizq.py` & `petljadoc-1.3.3/petljadoc/runestone_ext/quizq/quizq.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/regexcheck/css/regex-check.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/regexcheck/css/regex-check.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/regexcheck/js/regex-check.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/regexcheck/js/regex-check.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/regexcheck/regexcheck.py` & `petljadoc-1.3.3/petljadoc/runestone_ext/regexcheck/regexcheck.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/simanim/css/simanim.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/simanim/css/simanim.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/simanim/js/simanim.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/simanim/js/simanim.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -524,16 +524,19 @@
     this.bufferCanvsContext.translate(-scaledPoint[0], -scaledPoint[1]);
 }
 
 window.addEventListener('load', function() {
     var simanimWhlUrl = ''
     if (location.hostname === "localhost" || location.hostname === "127.0.0.1")
         simanimWhlUrl = document.location.origin + '/_static/simanim-0.0.4-py3-none-any.whl'
-    else
+    else if (location.hostname.endsWith('github.io')) {
+        simanimWhlUrl = document.location.origin + '/' + location.pathname.split('/')[1] + '/_static/simanim-0.0.4-py3-none-any.whl'
+    } else {
         simanimWhlUrl = 'https://petljastorage.blob.core.windows.net/kursevi/common_assets/simanim-0.0.4-py3-none-any.whl'
+    }
     // init pyodide
     languagePluginLoader.then(() =>
         pyodide.runPythonAsync(`
 	import sys
 	import traceback
 	import io
 	import js
```

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/simanim/simanim.py` & `petljadoc-1.3.3/petljadoc/runestone_ext/simanim/simanim.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/Blob.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/Blob.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/FileSaver.min.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/FileSaver.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/LICENSE.txt` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/accessibility.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/accessibility.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/accessibilitydarkest.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/accessibilitydarkest.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/accessibilitylight.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/accessibilitylight.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/activecode-i18n.en.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/activecode-i18n.en.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/activecode-i18n.sr-Cyrl.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/activecode-i18n.sr-Cyrl.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/activecode.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/activecode.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/activecode.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/activecode.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/animationbase.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/animationbase.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/basic.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/basic.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/blockly_compressed.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/blockly_compressed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/blocks_compressed.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/blocks_compressed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bookfuncs.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bookfuncs.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-3.0.0/css/bootstrap.min.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-3.0.0/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-3.0.0/js/bootstrap.min.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-3.0.0/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-sphinx.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-sphinx.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap.min.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/clickable.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/clickable.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/clickable.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/clickable.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/clike.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/clike.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/codelens.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/codelens.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/codemirror.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/codemirror.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/codemirror.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/codemirror.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/css.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/css.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/d3.v2.min.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/d3.v2.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/datafile.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/datafile.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/diff_match_patch.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/diff_match_patch.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/doctools.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/dragndrop.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/dragndrop.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/dragndrop.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/dragndrop.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/external.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/external.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/fitb.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/fitb.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/guiders-1.3.0.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/guiders-1.3.0.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/guiders-1.3.0.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/guiders-1.3.0.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/htmlmixed.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/htmlmixed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/javascript.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/javascript.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/javascript_compressed.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/javascript_compressed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery-3.2.1.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery-3.2.1.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery-migrate-1.2.1.min.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery-migrate-1.2.1.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery-ui-1.10.3.custom.min.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery-ui-1.10.3.custom.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery-ui-1.10.3.custom.min.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery-ui-1.10.3.custom.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.ba-bbq.min.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.ba-bbq.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.highlight.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.highlight.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.hotkey.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.hotkey.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.idle-timer.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.idle-timer.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.jsPlumb-1.3.10-all-min.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.jsPlumb-1.3.10-all-min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.tablesorter.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.tablesorter.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/CLDRPluralRuleParser.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/CLDRPluralRuleParser.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.emitter.bidi.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.emitter.bidi.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.emitter.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.emitter.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.fallbacks.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.fallbacks.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.language.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.language.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.messagestore.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.messagestore.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.parser.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.parser.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/language_data.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/lib/hammer.min.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/lib/hammer.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/lib/prettify.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/lib/prettify.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/matrixeq.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/matrixeq.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/matrixeq.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/matrixeq.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/mchoice.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/mchoice.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/merge.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/merge.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/merge.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/merge.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/modal-basic.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/modal-basic.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/msg/js/en.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/msg/js/en.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/navhelp.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/navhelp.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/parsons.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/parsons.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/parsons.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/parsons.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/poll.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/poll.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/presenter_mode.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/presenter_mode.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/presenter_mode.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/presenter_mode.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/processing-1.4.1.min.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/processing-1.4.1.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/pygments.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/python.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/python.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/python_compressed.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/python_compressed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/pytutor.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/pytutor.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/pytutor.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/pytutor.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/rangy-core.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/rangy-core.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/rangy-cssclassapplier.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/rangy-cssclassapplier.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/rangy-textrange.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/rangy-textrange.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/reveal.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/reveal.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/runestone-custom-sphinx-bootstrap.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/runestone-custom-sphinx-bootstrap.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/runestonebase.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/runestonebase.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/runestonevideo.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/runestonevideo.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/searchtools.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/sharedb.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/sharedb.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/shortanswer.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/shortanswer.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/showEval.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/showEval.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/showEval.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/showEval.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/skulpt-stdlib.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/skulpt-stdlib.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/skulpt.min.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/skulpt.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/sortmodels.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/sortmodels.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/sortviewers.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/sortviewers.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/style.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/style.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/tabbedstuff.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/tabbedstuff.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/tabbedstuff.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/tabbedstuff.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timed.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timed_activecode.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timed_activecode.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timed_shortanswer.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timed_shortanswer.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timedclickable.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timedclickable.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timeddnd.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timeddnd.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timedfitb.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timedfitb.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timedmc.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timedmc.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timedparsons.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timedparsons.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/underscore-1.3.1.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/underscore.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/user-highlights.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/user-highlights.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/user-highlights.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/user-highlights.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/waypoints.min.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/waypoints.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/webglinteractive.css` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/webglinteractive.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/webglinteractive.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/webglinteractive.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/websupport.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/websupport.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/xml.js` & `petljadoc-1.3.3/petljadoc/runestone_ext/video/test/build/VideoTests/_static/xml.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/scorm-proxy-templates/adlcp_rootv1p2.xsd` & `petljadoc-1.3.3/petljadoc/scorm-proxy-templates/adlcp_rootv1p2.xsd`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/scorm-proxy-templates/bundle.js` & `petljadoc-1.3.3/petljadoc/scorm-proxy-templates/bundle.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/scorm-proxy-templates/favicon.ico` & `petljadoc-1.3.3/petljadoc/scorm-proxy-templates/favicon.ico`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/scorm-proxy-templates/ims_xml.xsd` & `petljadoc-1.3.3/petljadoc/scorm-proxy-templates/ims_xml.xsd`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/scorm-proxy-templates/imscp_rootv1p1p2.xsd` & `petljadoc-1.3.3/petljadoc/scorm-proxy-templates/imscp_rootv1p1p2.xsd`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/scorm-proxy-templates/imsmanifest.t.xml` & `petljadoc-1.3.3/petljadoc/scorm-proxy-templates/imsmanifest.t.xml`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/scorm-proxy-templates/imsmd_rootv1p2p1.xsd` & `petljadoc-1.3.3/petljadoc/scorm-proxy-templates/imsmd_rootv1p2p1.xsd`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/scorm-proxy-templates/index.t.html` & `petljadoc-1.3.3/petljadoc/scorm-proxy-templates/index.t.html`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/scorm-proxy-templates/style-player.css` & `petljadoc-1.3.3/petljadoc/scorm-proxy-templates/style-player.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/scorm-templates/adlcp_rootv1p2.xsd` & `petljadoc-1.3.3/petljadoc/scorm-templates/adlcp_rootv1p2.xsd`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/scorm-templates/ims_xml.xsd` & `petljadoc-1.3.3/petljadoc/scorm-templates/ims_xml.xsd`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/scorm-templates/imscp_rootv1p1p2.xsd` & `petljadoc-1.3.3/petljadoc/scorm-templates/imscp_rootv1p1p2.xsd`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/scorm-templates/imsmd_rootv1p2p1.xsd` & `petljadoc-1.3.3/petljadoc/scorm-templates/imsmd_rootv1p2p1.xsd`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/layout.html` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/layout.html`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/locale/en/LC_MESSAGES/shpinx.mo` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/locale/en/LC_MESSAGES/shpinx.mo`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/locale/sr/LC_MESSAGES/sphinx.mo` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/locale/sr/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/locale/sr@latn/LC_MESSAGES/sphinx.mo` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/locale/sr@latn/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/locale/sr_RS/LC_MESSAGES/sphinx.mo` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/locale/sr_RS/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/platform/petljaRTBundle.js` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/platform/petljaRTBundle.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/bootstrap-4.0.0-dist/css/bootstrap.min.css` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/bootstrap-4.0.0-dist/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/bootstrap-4.0.0-dist/js/bootstrap.bundle.min.js` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/bootstrap-4.0.0-dist/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/bootstrap-4.0.0-dist/js/bootstrap.min.js` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/bootstrap-4.0.0-dist/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/bootstrap-sphinx.css_t` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/bootstrap-sphinx.css_t`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/bootstrap-sphinx.js` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/bootstrap-sphinx.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/bundle.js` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/bundle.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/css/font-awesome.min.css` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/favicon.ico` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/flatly.min.css` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/flatly.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/fonts/FontAwesome.otf` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.eot` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.svg` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.ttf` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.woff` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.woff2` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/images/choice-background.svg` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/images/choice-background.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/images/dragndrop-background.svg` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/images/dragndrop-background.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/images/fitb-background.svg` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/images/fitb-background.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/images/logo.svg` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/images/netkabinet-logo-strelica-wt.svg` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/images/netkabinet-logo-strelica-wt.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/images/parsons-background.svg` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/images/parsons-background.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/images/petlja-logo-wt.svg` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/images/petlja-logo-wt.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/images/play_button.svg` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/images/play_button.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/Facebook.png` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/Facebook.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/Facebook_icon.png` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/Facebook_icon.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/Twitter.png` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/Twitter.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/Twitter_icon.png` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/Twitter_icon.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/dragndrop-img.svg` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/dragndrop-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/favicon.ico` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/fitb-img.svg` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/fitb-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/green-coin.png` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/green-coin.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-ball.png` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/karel-ball.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-east-balls.png` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/karel-east-balls.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-east.png` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/karel-east.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-head.png` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/karel-head.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-hole.png` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/karel-hole.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-north-balls.png` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/karel-north-balls.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-north.png` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/karel-north.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-south-balls.png` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/karel-south-balls.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-south.png` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/karel-south.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-west-balls.png` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/karel-west-balls.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-west.png` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/karel-west.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/learnmorenote-img.svg` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/learnmorenote-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/logo.png` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/logo.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/logo_small.png` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/logo_small.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/netkabinet-logo-strelica-wt.svg` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/netkabinet-logo-strelica-wt.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/parsons-img.svg` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/parsons-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/petlja-logo-wt.svg` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/petlja-logo-wt.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/play_overlay_icon.png` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/play_overlay_icon.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/qchoice-img.svg` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/qchoice-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/question-mark-old.png` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/question-mark-old.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/question-mark.png` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/question-mark.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/questionnote-img.svg` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/questionnote-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/suggestionnote-img.svg` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/suggestionnote-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/technicalnote-img.svg` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/img/technicalnote-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/petlja-course.css` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/petlja-course.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/petlja.js` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/petlja.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/require.js` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/require.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/simanim-0.0.4-py3-none-any.whl` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/simanim-0.0.4-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/skulpt-stdlib.js` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/skulpt-stdlib.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/skulpt.min.js` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/skulpt.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/style-player.css` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/static/style-player.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/bc_theme/theme.conf` & `petljadoc-1.3.3/petljadoc/themes/bc_theme/theme.conf`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/basic_layout.html` & `petljadoc-1.3.3/petljadoc/themes/course_theme/basic_layout.html`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/course_homepage.html` & `petljadoc-1.3.3/petljadoc/themes/course_theme/course_homepage.html`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/globaltoc.html` & `petljadoc-1.3.3/petljadoc/themes/course_theme/globaltoc.html`

 * *Files 13% similar despite different names*

```diff
@@ -12,15 +12,15 @@
                 <div class="courseContentsSubSection d-none">
                     {%- for activity in lesson.active_activities -%}
                     {%- if pagename == 'index' -%}
                         <a href=./{{lesson.folder_url}}/{{activity.toc_url}}.html>
                     {%- else -%}
                         <a href=../{{lesson.folder_url}}/{{activity.toc_url}}.html>
                     {%- endif -%}
-                    <div class="studioLecture" id=activity-{{activity.toc_url}}>
+                    <div class="studioLecture" id=activity-{{lesson.folder_url}}-{{activity.toc_url}}>
                         {%- if "reading" == activity.type -%}
                         <i class="fas fa-file-alt activity-icon"></i>
                         {%- elif "video" == activity.type -%}
                         <i class="fas fa-film activity-icon"></i>
                         {%- else -%}
                         <i class="far fa-question-circle activity-icon"></i>
                         {%- endif -%}
```

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/layout.html` & `petljadoc-1.3.3/petljadoc/themes/course_theme/layout.html`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/locale/en/LC_MESSAGES/shpinx.mo` & `petljadoc-1.3.3/petljadoc/themes/course_theme/locale/en/LC_MESSAGES/shpinx.mo`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/locale/sr/LC_MESSAGES/sphinx.mo` & `petljadoc-1.3.3/petljadoc/themes/course_theme/locale/sr/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/locale/sr@latn/LC_MESSAGES/sphinx.mo` & `petljadoc-1.3.3/petljadoc/themes/course_theme/locale/sr@latn/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/locale/sr_RS/LC_MESSAGES/sphinx.mo` & `petljadoc-1.3.3/petljadoc/themes/course_theme/locale/sr_RS/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/relations.html` & `petljadoc-1.3.3/petljadoc/themes/course_theme/relations.html`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/bootstrap-4.0.0-dist/css/bootstrap.min.css` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/bootstrap-4.0.0-dist/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/bootstrap-4.0.0-dist/js/bootstrap.bundle.min.js` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/bootstrap-4.0.0-dist/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/bootstrap-4.0.0-dist/js/bootstrap.min.js` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/bootstrap-4.0.0-dist/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/bootstrap-sphinx.css_t` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/bootstrap-sphinx.css_t`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/bootstrap-sphinx.js` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/bootstrap-sphinx.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/css/font-awesome.min.css` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/favicon.ico` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/flatly.min.css` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/flatly.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/fonts/FontAwesome.otf` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.eot` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.svg` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.ttf` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.woff` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.woff2` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/images/choice-background.svg` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/images/choice-background.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/images/dragndrop-background.svg` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/images/dragndrop-background.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/images/fitb-background.svg` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/images/fitb-background.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/images/logo.svg` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/images/netkabinet-logo-strelica-wt.svg` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/images/netkabinet-logo-strelica-wt.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/images/parsons-background.svg` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/images/parsons-background.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/images/petlja-logo-wt.svg` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/images/petlja-logo-wt.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/images/play_button.svg` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/images/play_button.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/Facebook.png` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/Facebook.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/Facebook_icon.png` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/Facebook_icon.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/Twitter.png` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/Twitter.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/Twitter_icon.png` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/Twitter_icon.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/dragndrop-img.svg` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/dragndrop-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/favicon.ico` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/fitb-img.svg` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/fitb-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/green-coin.png` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/green-coin.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-ball.png` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/karel-ball.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-east-balls.png` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/karel-east-balls.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-east.png` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/karel-east.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-head.png` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/karel-head.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-hole.png` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/karel-hole.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-north-balls.png` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/karel-north-balls.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-north.png` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/karel-north.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-south-balls.png` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/karel-south-balls.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-south.png` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/karel-south.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-west-balls.png` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/karel-west-balls.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-west.png` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/karel-west.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/learnmorenote-img.svg` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/learnmorenote-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/logo.png` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/logo.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/logo_small.png` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/logo_small.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/netkabinet-logo-strelica-wt.svg` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/netkabinet-logo-strelica-wt.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/parsons-img.svg` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/parsons-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/petlja-logo-wt.svg` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/petlja-logo-wt.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/play_overlay_icon.png` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/play_overlay_icon.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/qchoice-img.svg` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/qchoice-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/question-mark-old.png` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/question-mark-old.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/question-mark.png` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/question-mark.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/questionnote-img.svg` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/questionnote-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/suggestionnote-img.svg` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/suggestionnote-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/technicalnote-img.svg` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/img/technicalnote-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/nbstyle.css` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/nbstyle.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/petlja-course.css` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/petlja-course.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/petlja.js` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/petlja.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -22,50 +22,50 @@
     var activity = path.substring(path.indexOf('/') + 1).replace('.html', '');
 
     if (document.getElementById("lecture-" + lecture)) {
         document.getElementById("lecture-" + lecture).click();
         activeLecture = lecture;
     }
 
-    if (document.getElementById("activity-" + activity)) {
-        document.getElementById("activity-" + activity).classList.add('active');
+    if (document.getElementById("activity-" + lecture + "-" + activity)) {
+        document.getElementById("activity-" + lecture + "-" + activity).classList.add('active');
         activeActivity = activity;
     }
 
     if (document.getElementById('prevLectureLink'))
         document.getElementById('prevLectureLink').addEventListener('click', function(e) {
             localStorage.setItem('scrollpos', 0);
             e.preventDefault();
             var lectureDiv = document.getElementById(activeLecture);
-            if (document.getElementById("activity-" + activity).parentElement.previousElementSibling != null) {
-                document.getElementById("activity-" + activity).parentElement.previousElementSibling.click();
+            if (document.getElementById("activity-" + lecture + "-" + activity).parentElement.previousElementSibling != null) {
+                document.getElementById("activity-" + lecture + "-" + activity).parentElement.previousElementSibling.click();
             } else {
-                document.getElementById("activity-" + activity).parentElement.parentElement.parentElement.previousElementSibling.children[1].lastElementChild.click()
+                document.getElementById("activity-" + lecture + "-" + activity).parentElement.parentElement.parentElement.previousElementSibling.children[1].lastElementChild.click()
             }
         });
 
     if (document.getElementById('nextLectureLink'))
         document.getElementById('nextLectureLink').addEventListener('click', function(e) {
             localStorage.setItem('scrollpos', 0);
             e.preventDefault();
             if (activeLecture == '') {
                 var lectureDiv = document.getElementsByClassName('lecture-div')[0];
                 lectureDiv.nextElementSibling.firstElementChild.click();
             } else {
                 var lectureDiv = document.getElementById(activeLecture);
-                if (document.getElementById("activity-" + activity).parentElement.nextElementSibling != null) {
-                    document.getElementById("activity-" + activity).parentElement.nextElementSibling.click();
+                if (document.getElementById("activity-" + lecture + "-" + activity).parentElement.nextElementSibling != null) {
+                    document.getElementById("activity-" + lecture + "-" + activity).parentElement.nextElementSibling.click();
                 } else {
                     document.getElementById("lecture-" + lecture).parentElement.nextElementSibling.children[1].firstChild.click()
                 }
             }
         });
 
     if (activeLecture != '') {
-        if (document.getElementById("activity-" + activity).parentElement.parentElement.parentElement.previousElementSibling == null && document.getElementById("activity-" + activity).parentElement.previousElementSibling == null)
+        if (document.getElementById("activity-" + lecture + "-" + activity).parentElement.parentElement.parentElement.previousElementSibling == null && document.getElementById("activity-" + lecture + "-" + activity).parentElement.previousElementSibling == null)
             document.getElementById('prevLectureLink').classList.add('invisible');
     }
 
     if (document.getElementsByClassName('course-requirements').length > 0) {
         var learningDiv = document.getElementsByClassName("course-requirements")[0].firstElementChild;
         var learningDivList = learningDiv.querySelector('ul');
         var numberOfLiElements = learningDivList.querySelectorAll('li').length;
```

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/require.js` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/require.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/simanim-0.0.4-py3-none-any.whl` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/simanim-0.0.4-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/skulpt-stdlib.js` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/skulpt-stdlib.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/static/skulpt.min.js` & `petljadoc-1.3.3/petljadoc/themes/course_theme/static/skulpt.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/subchapter.html` & `petljadoc-1.3.3/petljadoc/themes/course_theme/subchapter.html`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/course_theme/theme.conf` & `petljadoc-1.3.3/petljadoc/themes/course_theme/theme.conf`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/__init__.py` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/basic_layout.html` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/basic_layout.html`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/layout.html` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/layout.html`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/locale/en/LC_MESSAGES/sphinx.mo` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/locale/en/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/locale/sr/LC_MESSAGES/sphinx.mo` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/locale/sr/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/locale/sr@latn/LC_MESSAGES/sphinx.mo` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/locale/sr@latn/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/locale/sr_RS/LC_MESSAGES/sphinx.mo` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/locale/sr_RS/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/relations.html` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/relations.html`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/bootstrap-4.0.0-dist/css/bootstrap.min.css` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/bootstrap-4.0.0-dist/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/bootstrap-4.0.0-dist/js/bootstrap.bundle.min.js` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/bootstrap-4.0.0-dist/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/bootstrap-4.0.0-dist/js/bootstrap.min.js` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/bootstrap-4.0.0-dist/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/bootstrap-sphinx.css_t` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/bootstrap-sphinx.css_t`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/bootstrap-sphinx.js` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/bootstrap-sphinx.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/css/font-awesome.min.css` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/favicon.ico` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/flatly.min.css` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/flatly.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/fonts/FontAwesome.otf` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.eot` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.svg` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.ttf` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.woff` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.woff2` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/images/choice-background.svg` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/images/choice-background.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/images/dragndrop-background.svg` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/images/dragndrop-background.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/images/fitb-background.svg` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/images/fitb-background.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/images/logo.svg` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/images/netkabinet-logo-strelica-wt.svg` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/images/netkabinet-logo-strelica-wt.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/images/parsons-background.svg` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/images/parsons-background.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/images/petlja-logo-wt.svg` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/images/petlja-logo-wt.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/images/play_button.svg` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/images/play_button.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/Facebook.png` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/Facebook.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/Facebook_icon.png` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/Facebook_icon.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/Twitter.png` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/Twitter.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/Twitter_icon.png` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/Twitter_icon.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/dragndrop-img.svg` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/dragndrop-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/favicon.ico` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/fitb-img.svg` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/fitb-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/green-coin.png` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/green-coin.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/karel-ball.png` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/karel-ball.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/karel-east.png` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/karel-east.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/karel-head.png` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/karel-head.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/karel-hole.png` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/karel-hole.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/karel-north.png` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/karel-north.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/karel-south.png` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/karel-south.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/karel-west.png` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/karel-west.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/learnmorenote-img.svg` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/learnmorenote-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/logo.png` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/logo.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/logo_small.png` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/logo_small.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/netkabinet-logo-strelica-wt.svg` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/netkabinet-logo-strelica-wt.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/parsons-img.svg` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/parsons-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/petlja-logo-wt.svg` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/petlja-logo-wt.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/play_overlay_icon.png` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/play_overlay_icon.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/qchoice-img.svg` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/qchoice-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/question-mark-old.png` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/question-mark-old.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/question-mark.png` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/question-mark.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/questionnote-img.svg` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/questionnote-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/suggestionnote-img.svg` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/suggestionnote-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/technicalnote-img.svg` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/img/technicalnote-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/nbstyle.css` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/nbstyle.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/petlja-runestone.css` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/petlja-runestone.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/require.js` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/require.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/simanim-0.0.4-py3-none-any.whl` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/simanim-0.0.4-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/skulpt-stdlib.js` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/skulpt-stdlib.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/skulpt.min.js` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/static/skulpt.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/subchapter.html` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/subchapter.html`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/themes/runestone_theme/theme.conf` & `petljadoc-1.3.3/petljadoc/themes/runestone_theme/theme.conf`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc/util.py` & `petljadoc-1.3.3/petljadoc/util.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/petljadoc.egg-info/SOURCES.txt` & `petljadoc-1.3.3/petljadoc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.1/setup.py` & `petljadoc-1.3.3/setup.py`

 * *Files identical despite different names*

