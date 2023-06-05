# Comparing `tmp/pyflp-2.2.0.tar.gz` & `tmp/pyflp-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyflp-2.2.0.tar", last modified: Sun May 28 11:44:37 2023, max compression
+gzip compressed data, was "pyflp-2.2.1.tar", last modified: Mon Jun  5 13:15:15 2023, max compression
```

## Comparing `pyflp-2.2.0.tar` & `pyflp-2.2.1.tar`

### file list

```diff
@@ -1,317 +1,317 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.257686 pyflp-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-28 11:44:21.000000 pyflp-2.2.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.229686 pyflp-2.2.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-28 11:44:21.000000 pyflp-2.2.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-28 11:44:21.000000 pyflp-2.2.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-28 11:44:21.000000 pyflp-2.2.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    26412 2023-05-28 11:44:21.000000 pyflp-2.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-05-28 11:44:21.000000 pyflp-2.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-28 11:44:21.000000 pyflp-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-28 11:44:21.000000 pyflp-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    21556 2023-05-28 11:44:37.257686 pyflp-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20297 2023-05-28 11:44:21.000000 pyflp-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.229686 pyflp-2.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.229686 pyflp-2.2.0/docs/architecture/
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/architecture/flp-format.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/architecture/how-it-works.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/architecture/reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/architecture.rst
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8222 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/features.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.229686 pyflp-2.2.0/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/guides/plugin.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/guides/reversing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/guides.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/handbook.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/helping.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.225686 pyflp-2.2.0/docs/img/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.229686 pyflp-2.2.0/docs/img/arrangement/
--rw-r--r--   0 runner    (1001) docker     (123)    61669 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/arrangement/preview.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/arrangement/time-signature.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.229686 pyflp-2.2.0/docs/img/arrangement/timemarker/
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/arrangement/timemarker/action.png
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/arrangement/timemarker/preview.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.229686 pyflp-2.2.0/docs/img/arrangement/track/
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/arrangement/track/color.gif
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/arrangement/track/enabled.gif
--rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/arrangement/track/grouped.gif
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/arrangement/track/icon.gif
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/arrangement/track/locked.gif
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/arrangement/track/motion.png
--rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/arrangement/track/performance-settings.png
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/arrangement/track/press.png
--rw-r--r--   0 runner    (1001) docker     (123)    22957 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/arrangement/track/preview.png
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/arrangement/track/sync.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.233686 pyflp-2.2.0/docs/img/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/arp.png
--rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/automation.png
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/color.gif
--rw-r--r--   0 runner    (1001) docker     (123)     9518 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/content.png
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/delay.png
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/enabled.gif
--rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/envelope.png
--rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/filter.png
--rw-r--r--   0 runner    (1001) docker     (123)    12931 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/fx1.png
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/fx2.png
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/icon.gif
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/keyboard.png
--rw-r--r--   0 runner    (1001) docker     (123)    13046 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/layer.png
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/level-adjusts.png
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/lfo.png
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/locked.gif
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/playback.png
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/polyphony.png
--rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/rack.png
--rw-r--r--   0 runner    (1001) docker     (123)    47255 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/sampler.png
--rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/stretch-mode.png
--rw-r--r--   0 runner    (1001) docker     (123)    14945 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/stretching.png
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/time.png
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/toolbar.png
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/tracking.png
--rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/channel/zipped.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.233686 pyflp-2.2.0/docs/img/contributing/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/contributing/pytest.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/contributing/readthedocs.svg
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/contributing/vscode.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.233686 pyflp-2.2.0/docs/img/controller/
--rw-r--r--   0 runner    (1001) docker     (123)    17142 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/controller/remote.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.237686 pyflp-2.2.0/docs/img/features/
--rw-r--r--   0 runner    (1001) docker     (123)    25693 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/features/images-dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    25798 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/features/images-light.png
--rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/features/tables-dark.png
--rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/features/tables-light.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.225686 pyflp-2.2.0/docs/img/guides/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.237686 pyflp-2.2.0/docs/img/guides/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)    13283 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/guides/plugin/1-parameters.png
--rw-r--r--   0 runner    (1001) docker     (123)    30725 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/guides/plugin/2-load-plugin.png
--rw-r--r--   0 runner    (1001) docker     (123)    29072 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/guides/plugin/3-observe-knob-positions.png
--rw-r--r--   0 runner    (1001) docker     (123)     8241 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/guides/plugin/4-hint-panel.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.237686 pyflp-2.2.0/docs/img/guides/reversing/
--rw-r--r--   0 runner    (1001) docker     (123)    41307 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/guides/reversing/flpedit.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.237686 pyflp-2.2.0/docs/img/helping/
--rw-r--r--   0 runner    (1001) docker     (123)    23109 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/helping/open-issue-dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    23706 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/helping/open-issue-light.png
--rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/helping/star-repo-dark.gif
--rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/helping/star-repo-light.gif
--rw-r--r--   0 runner    (1001) docker     (123)    42665 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/helping/watch-repo-dark.gif
--rw-r--r--   0 runner    (1001) docker     (123)    42617 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/helping/watch-repo-light.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.237686 pyflp-2.2.0/docs/img/mixer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.237686 pyflp-2.2.0/docs/img/mixer/insert/
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/mixer/insert/dock.png
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/mixer/insert/enabled.gif
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/mixer/insert/eq.png
--rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/mixer/insert/input.png
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/mixer/insert/locked.gif
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/mixer/insert/output.png
--rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/mixer/insert/pan.gif
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/mixer/insert/preview.png
--rw-r--r--   0 runner    (1001) docker     (123)   111613 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/mixer/preview.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.237686 pyflp-2.2.0/docs/img/mixer/slot/
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/mixer/slot/color.gif
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/mixer/slot/enabled.gif
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/mixer/slot/icon.gif
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/mixer/slot/locked.gif
--rw-r--r--   0 runner    (1001) docker     (123)     9679 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/mixer/slots.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.237686 pyflp-2.2.0/docs/img/pattern/
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/pattern/color.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.237686 pyflp-2.2.0/docs/img/pattern/note/
--rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/pattern/note/group.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.237686 pyflp-2.2.0/docs/img/plugin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.241686 pyflp-2.2.0/docs/img/plugin/effects/
--rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/effects/fruity-balance.png
--rw-r--r--   0 runner    (1001) docker     (123)    42770 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/effects/fruity-blood-overdrive.png
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/effects/fruity-center.png
--rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/effects/fruity-fast-dist.png
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/effects/fruity-notebook2.png
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/effects/fruity-send.png
--rw-r--r--   0 runner    (1001) docker     (123)    13567 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/effects/fruity-soft-clipper.png
--rw-r--r--   0 runner    (1001) docker     (123)    18730 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/effects/fruity-stereo-enhancer.png
--rw-r--r--   0 runner    (1001) docker     (123)    35054 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/effects/soundgoodizer.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.241686 pyflp-2.2.0/docs/img/plugin/generators/
--rw-r--r--   0 runner    (1001) docker     (123)     7655 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/generators/boobass.png
--rw-r--r--   0 runner    (1001) docker     (123)    22178 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/generators/fruit-kick.png
--rw-r--r--   0 runner    (1001) docker     (123)    47669 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/generators/plucked.png
--rw-r--r--   0 runner    (1001) docker     (123)    52803 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/maximize.gif
--rw-r--r--   0 runner    (1001) docker     (123)    24100 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/toolbar_collapse.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.241686 pyflp-2.2.0/docs/img/plugin/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/wrapper/page.gif
--rw-r--r--   0 runner    (1001) docker     (123)    37229 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/wrapper/processing.png
--rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/wrapper/settings-gui.png
--rw-r--r--   0 runner    (1001) docker     (123)    14866 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/wrapper/settings-midi.png
--rw-r--r--   0 runner    (1001) docker     (123)    48421 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/wrapper/settings.png
--rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/plugin/wrapper/troubleshooting.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.241686 pyflp-2.2.0/docs/img/project/
--rw-r--r--   0 runner    (1001) docker     (123)    36725 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/project/info.png
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/project/ppq.png
--rw-r--r--   0 runner    (1001) docker     (123)    27649 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/project/settings.png
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/project/tempo.png
--rw-r--r--   0 runner    (1001) docker     (123)     9859 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/project/time-spent.png
--rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/img/project/version.png
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/limitations.rst
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.241686 pyflp-2.2.0/docs/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.245686 pyflp-2.2.0/docs/reference/arrangement/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/arrangement/arrangement.rst
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/arrangement/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/arrangement/playlist.rst
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/arrangement/track.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.245686 pyflp-2.2.0/docs/reference/channel/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/channel/automation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/channel/channel.rst
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/channel/display-group.rst
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/channel/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/channel/instrument.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/channel/layer.rst
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/channel/sampler.rst
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/channel/shared.rst
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/controllers.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/events.rst
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/exceptions.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.245686 pyflp-2.2.0/docs/reference/mixer/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/mixer/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/mixer/insert.rst
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/mixer/slot.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.245686 pyflp-2.2.0/docs/reference/patterns/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/patterns/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/patterns/pattern.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.245686 pyflp-2.2.0/docs/reference/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/plugins/effects.rst
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/plugins/generators.rst
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/plugins/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/plugins/vst.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/project.rst
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference/timemarkers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-28 11:44:21.000000 pyflp-2.2.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.245686 pyflp-2.2.0/pyflp/
--rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-05-28 11:44:21.000000 pyflp-2.2.0/pyflp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-28 11:44:21.000000 pyflp-2.2.0/pyflp/_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-05-28 11:44:21.000000 pyflp-2.2.0/pyflp/_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)    19152 2023-05-28 11:44:21.000000 pyflp-2.2.0/pyflp/_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-05-28 11:44:21.000000 pyflp-2.2.0/pyflp/_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-28 11:44:37.000000 pyflp-2.2.0/pyflp/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    17705 2023-05-28 11:44:21.000000 pyflp-2.2.0/pyflp/arrangement.py
--rw-r--r--   0 runner    (1001) docker     (123)    50356 2023-05-28 11:44:21.000000 pyflp-2.2.0/pyflp/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-28 11:44:21.000000 pyflp-2.2.0/pyflp/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-28 11:44:21.000000 pyflp-2.2.0/pyflp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-05-28 11:44:21.000000 pyflp-2.2.0/pyflp/mixer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12461 2023-05-28 11:44:21.000000 pyflp-2.2.0/pyflp/pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)    34899 2023-05-28 11:44:21.000000 pyflp-2.2.0/pyflp/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    18882 2023-05-28 11:44:21.000000 pyflp-2.2.0/pyflp/project.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:21.000000 pyflp-2.2.0/pyflp/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-05-28 11:44:21.000000 pyflp-2.2.0/pyflp/timemarker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-05-28 11:44:21.000000 pyflp-2.2.0/pyflp/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.249686 pyflp-2.2.0/pyflp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21556 2023-05-28 11:44:37.000000 pyflp-2.2.0/pyflp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8752 2023-05-28 11:44:37.000000 pyflp-2.2.0/pyflp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 11:44:37.000000 pyflp-2.2.0/pyflp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-28 11:44:37.000000 pyflp-2.2.0/pyflp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-28 11:44:37.000000 pyflp-2.2.0/pyflp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-05-28 11:44:21.000000 pyflp-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-28 11:44:21.000000 pyflp-2.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 11:44:37.257686 pyflp-2.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.249686 pyflp-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.249686 pyflp-2.2.0/tests/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   190128 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/FL 20.8.4.flp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.253686 pyflp-2.2.0/tests/assets/channels/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/+4800-cents.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/-4800-cents.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/100%-left.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/100%-right.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/arp.fst
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/automation-lfo.fst
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/automation-points.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/colored.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/cut-groups.fst
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/delay.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/disabled.fst
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/envelope.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/full-volume.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/iconified.fst
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/keyboard.fst
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/layer-crossfade.fst
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/layer-random.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/level-adjusts.fst
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/lfo.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/locked.fst
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/polyphony.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/routed.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/sampler-content.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/sampler-filter.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/sampler-fx.fst
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/sampler-path.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/sampler-playback.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/sampler-stretching.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/time.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/tracking.fst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/channels/zero-volume.fst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.253686 pyflp-2.2.0/tests/assets/corrupted/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/corrupted/invalid-data-magic.flp
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/corrupted/invalid-event-size.flp
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/corrupted/invalid-format.flp
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/corrupted/invalid-header-magic.flp
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/corrupted/invalid-header-size.flp
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/corrupted/invalid-ppq.flp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.257686 pyflp-2.2.0/tests/assets/inserts/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/inserts/100%-left.fst
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/inserts/100%-merged.fst
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/inserts/100%-right.fst
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/inserts/100%-separated.fst
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/inserts/50ms-input-latency.fst
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/inserts/50ms-track-latency.fst
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/inserts/armed.fst
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/inserts/channels-swapped.fst
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/inserts/colored.fst
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/inserts/disabled.fst
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/inserts/effects-bypassed.fst
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/inserts/iconified.fst
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/inserts/locked.fst
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/inserts/polarity-reversed.fst
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/inserts/post-eq.fst
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/inserts/separator.fst
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/inserts/zero-volume.fst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.257686 pyflp-2.2.0/tests/assets/patterns/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/patterns/c-major-scale.fsc
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/patterns/c5-1bar.fsc
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/patterns/color-9.fsc
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/patterns/common-group.fsc
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/patterns/empty.fsc
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/patterns/fine-pitch-min-max.fsc
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/patterns/modx-min-max.fsc
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/patterns/mody-min-max.fsc
--rw-r--r--   0 runner    (1001) docker     (123)   115522 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/patterns/multi-channel.flp
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/patterns/pan-min-max.fsc
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/patterns/release-min-max.fsc
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/patterns/slide-note.fsc
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/patterns/velocity-min-max.fsc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:44:37.257686 pyflp-2.2.0/tests/assets/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/plugins/boobass.fst
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/plugins/fruit-kick.fst
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/plugins/fruity-balance.fst
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/plugins/fruity-blood-overdrive.fst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/plugins/fruity-center.fst
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/plugins/fruity-fast-dist.fst
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/plugins/fruity-send.fst
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/plugins/fruity-soft-clipper.fst
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/plugins/fruity-stereo-enhancer.fst
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/plugins/fruity-wrapper.fst
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/plugins/plucked.fst
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/plugins/soundgoodizer.fst
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/assets/plugins/xfer-djmfilter.fst
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/test_arrangement.py
--rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/test_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/test_corrupted.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/test_mixer.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/test_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-28 11:44:21.000000 pyflp-2.2.0/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-28 11:44:21.000000 pyflp-2.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.472836 pyflp-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-05 13:15:00.000000 pyflp-2.2.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.444836 pyflp-2.2.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-05 13:15:00.000000 pyflp-2.2.1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-05 13:15:00.000000 pyflp-2.2.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-05 13:15:00.000000 pyflp-2.2.1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26611 2023-06-05 13:15:00.000000 pyflp-2.2.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-06-05 13:15:00.000000 pyflp-2.2.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-05 13:15:00.000000 pyflp-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-05 13:15:00.000000 pyflp-2.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    21556 2023-06-05 13:15:15.472836 pyflp-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20297 2023-06-05 13:15:00.000000 pyflp-2.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.444836 pyflp-2.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.444836 pyflp-2.2.1/docs/architecture/
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/architecture/flp-format.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/architecture/how-it-works.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/architecture/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/architecture.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8222 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/features.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.444836 pyflp-2.2.1/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/guides/plugin.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/guides/reversing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/guides.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/handbook.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/helping.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.440836 pyflp-2.2.1/docs/img/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.444836 pyflp-2.2.1/docs/img/arrangement/
+-rw-r--r--   0 runner    (1001) docker     (123)    61669 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/arrangement/preview.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/arrangement/time-signature.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.444836 pyflp-2.2.1/docs/img/arrangement/timemarker/
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/arrangement/timemarker/action.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/arrangement/timemarker/preview.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.448836 pyflp-2.2.1/docs/img/arrangement/track/
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/arrangement/track/color.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/arrangement/track/enabled.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/arrangement/track/grouped.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/arrangement/track/icon.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/arrangement/track/locked.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/arrangement/track/motion.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/arrangement/track/performance-settings.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/arrangement/track/press.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22957 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/arrangement/track/preview.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/arrangement/track/sync.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.452836 pyflp-2.2.1/docs/img/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/channel/arp.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/channel/automation.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/channel/color.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     9518 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/channel/content.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/channel/delay.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/channel/enabled.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/channel/envelope.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/channel/filter.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12931 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/channel/fx1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/channel/fx2.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/channel/icon.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/channel/keyboard.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13046 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/channel/layer.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/channel/level-adjusts.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/channel/lfo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/channel/locked.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/channel/playback.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/channel/polyphony.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/channel/rack.png
+-rw-r--r--   0 runner    (1001) docker     (123)    47255 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/channel/sampler.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/channel/stretch-mode.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14945 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/channel/stretching.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/channel/time.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/channel/toolbar.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/channel/tracking.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/channel/zipped.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.452836 pyflp-2.2.1/docs/img/contributing/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/contributing/pytest.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/contributing/readthedocs.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/contributing/vscode.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.452836 pyflp-2.2.1/docs/img/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)    17142 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/controller/remote.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.452836 pyflp-2.2.1/docs/img/features/
+-rw-r--r--   0 runner    (1001) docker     (123)    25693 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/features/images-dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    25798 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/features/images-light.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/features/tables-dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/features/tables-light.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.440836 pyflp-2.2.1/docs/img/guides/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.452836 pyflp-2.2.1/docs/img/guides/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)    13283 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/guides/plugin/1-parameters.png
+-rw-r--r--   0 runner    (1001) docker     (123)    30725 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/guides/plugin/2-load-plugin.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29072 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/guides/plugin/3-observe-knob-positions.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8241 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/guides/plugin/4-hint-panel.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.452836 pyflp-2.2.1/docs/img/guides/reversing/
+-rw-r--r--   0 runner    (1001) docker     (123)    41307 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/guides/reversing/flpedit.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.452836 pyflp-2.2.1/docs/img/helping/
+-rw-r--r--   0 runner    (1001) docker     (123)    23109 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/helping/open-issue-dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23706 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/helping/open-issue-light.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/helping/star-repo-dark.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/helping/star-repo-light.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    42665 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/helping/watch-repo-dark.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    42617 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/helping/watch-repo-light.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.456836 pyflp-2.2.1/docs/img/mixer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.456836 pyflp-2.2.1/docs/img/mixer/insert/
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/mixer/insert/dock.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/mixer/insert/enabled.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/mixer/insert/eq.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/mixer/insert/input.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/mixer/insert/locked.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/mixer/insert/output.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/mixer/insert/pan.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/mixer/insert/preview.png
+-rw-r--r--   0 runner    (1001) docker     (123)   111613 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/mixer/preview.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.456836 pyflp-2.2.1/docs/img/mixer/slot/
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/mixer/slot/color.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/mixer/slot/enabled.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/mixer/slot/icon.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/mixer/slot/locked.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     9679 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/mixer/slots.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.456836 pyflp-2.2.1/docs/img/pattern/
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/pattern/color.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.456836 pyflp-2.2.1/docs/img/pattern/note/
+-rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/pattern/note/group.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.456836 pyflp-2.2.1/docs/img/plugin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.456836 pyflp-2.2.1/docs/img/plugin/effects/
+-rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/plugin/effects/fruity-balance.png
+-rw-r--r--   0 runner    (1001) docker     (123)    42770 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/plugin/effects/fruity-blood-overdrive.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/plugin/effects/fruity-center.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/plugin/effects/fruity-fast-dist.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/plugin/effects/fruity-notebook2.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/plugin/effects/fruity-send.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13567 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/plugin/effects/fruity-soft-clipper.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18730 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/plugin/effects/fruity-stereo-enhancer.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35054 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/plugin/effects/soundgoodizer.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.456836 pyflp-2.2.1/docs/img/plugin/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)     7655 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/plugin/generators/boobass.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22178 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/plugin/generators/fruit-kick.png
+-rw-r--r--   0 runner    (1001) docker     (123)    47669 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/plugin/generators/plucked.png
+-rw-r--r--   0 runner    (1001) docker     (123)    52803 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/plugin/maximize.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    24100 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/plugin/toolbar_collapse.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.460836 pyflp-2.2.1/docs/img/plugin/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/plugin/wrapper/page.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    37229 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/plugin/wrapper/processing.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/plugin/wrapper/settings-gui.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14866 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/plugin/wrapper/settings-midi.png
+-rw-r--r--   0 runner    (1001) docker     (123)    48421 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/plugin/wrapper/settings.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/plugin/wrapper/troubleshooting.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.460836 pyflp-2.2.1/docs/img/project/
+-rw-r--r--   0 runner    (1001) docker     (123)    36725 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/project/info.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/project/ppq.png
+-rw-r--r--   0 runner    (1001) docker     (123)    27649 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/project/settings.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/project/tempo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9859 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/project/time-spent.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/img/project/version.png
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/limitations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.460836 pyflp-2.2.1/docs/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.460836 pyflp-2.2.1/docs/reference/arrangement/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/reference/arrangement/arrangement.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/reference/arrangement/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/reference/arrangement/playlist.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/reference/arrangement/track.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.460836 pyflp-2.2.1/docs/reference/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/reference/channel/automation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/reference/channel/channel.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/reference/channel/display-group.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/reference/channel/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/reference/channel/instrument.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/reference/channel/layer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/reference/channel/sampler.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/reference/channel/shared.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/reference/controllers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/reference/events.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/reference/exceptions.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.460836 pyflp-2.2.1/docs/reference/mixer/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/reference/mixer/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/reference/mixer/insert.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/reference/mixer/slot.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.460836 pyflp-2.2.1/docs/reference/patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/reference/patterns/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/reference/patterns/pattern.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.460836 pyflp-2.2.1/docs/reference/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/reference/plugins/effects.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/reference/plugins/generators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/reference/plugins/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/reference/plugins/vst.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/reference/project.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/reference/timemarkers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-05 13:15:00.000000 pyflp-2.2.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.464836 pyflp-2.2.1/pyflp/
+-rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-06-05 13:15:00.000000 pyflp-2.2.1/pyflp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-06-05 13:15:00.000000 pyflp-2.2.1/pyflp/_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-06-05 13:15:00.000000 pyflp-2.2.1/pyflp/_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19137 2023-06-05 13:15:00.000000 pyflp-2.2.1/pyflp/_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-06-05 13:15:00.000000 pyflp-2.2.1/pyflp/_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-05 13:15:15.000000 pyflp-2.2.1/pyflp/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17705 2023-06-05 13:15:00.000000 pyflp-2.2.1/pyflp/arrangement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50356 2023-06-05 13:15:00.000000 pyflp-2.2.1/pyflp/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-06-05 13:15:00.000000 pyflp-2.2.1/pyflp/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-06-05 13:15:00.000000 pyflp-2.2.1/pyflp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-06-05 13:15:00.000000 pyflp-2.2.1/pyflp/mixer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12461 2023-06-05 13:15:00.000000 pyflp-2.2.1/pyflp/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34899 2023-06-05 13:15:00.000000 pyflp-2.2.1/pyflp/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18882 2023-06-05 13:15:00.000000 pyflp-2.2.1/pyflp/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:00.000000 pyflp-2.2.1/pyflp/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-06-05 13:15:00.000000 pyflp-2.2.1/pyflp/timemarker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-05 13:15:00.000000 pyflp-2.2.1/pyflp/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.464836 pyflp-2.2.1/pyflp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21556 2023-06-05 13:15:15.000000 pyflp-2.2.1/pyflp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8752 2023-06-05 13:15:15.000000 pyflp-2.2.1/pyflp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:15:15.000000 pyflp-2.2.1/pyflp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-05 13:15:15.000000 pyflp-2.2.1/pyflp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 13:15:15.000000 pyflp-2.2.1/pyflp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-05 13:15:00.000000 pyflp-2.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-05 13:15:00.000000 pyflp-2.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 13:15:15.472836 pyflp-2.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.464836 pyflp-2.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.464836 pyflp-2.2.1/tests/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   190128 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/FL 20.8.4.flp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.468836 pyflp-2.2.1/tests/assets/channels/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/channels/+4800-cents.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/channels/-4800-cents.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/channels/100%-left.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/channels/100%-right.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/channels/arp.fst
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/channels/automation-lfo.fst
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/channels/automation-points.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/channels/colored.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/channels/cut-groups.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/channels/delay.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/channels/disabled.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/channels/envelope.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/channels/full-volume.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/channels/iconified.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/channels/keyboard.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/channels/layer-crossfade.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/channels/layer-random.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/channels/level-adjusts.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/channels/lfo.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/channels/locked.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/channels/polyphony.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/channels/routed.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/channels/sampler-content.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/channels/sampler-filter.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/channels/sampler-fx.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/channels/sampler-path.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/channels/sampler-playback.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/channels/sampler-stretching.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/channels/time.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/channels/tracking.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/channels/zero-volume.fst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.468836 pyflp-2.2.1/tests/assets/corrupted/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/corrupted/invalid-data-magic.flp
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/corrupted/invalid-event-size.flp
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/corrupted/invalid-format.flp
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/corrupted/invalid-header-magic.flp
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/corrupted/invalid-header-size.flp
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/corrupted/invalid-ppq.flp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.472836 pyflp-2.2.1/tests/assets/inserts/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/inserts/100%-left.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/inserts/100%-merged.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/inserts/100%-right.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/inserts/100%-separated.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/inserts/50ms-input-latency.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/inserts/50ms-track-latency.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/inserts/armed.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/inserts/channels-swapped.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/inserts/colored.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/inserts/disabled.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/inserts/effects-bypassed.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/inserts/iconified.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/inserts/locked.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/inserts/polarity-reversed.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/inserts/post-eq.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/inserts/separator.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/inserts/zero-volume.fst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.472836 pyflp-2.2.1/tests/assets/patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/patterns/c-major-scale.fsc
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/patterns/c5-1bar.fsc
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/patterns/color-9.fsc
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/patterns/common-group.fsc
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/patterns/empty.fsc
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/patterns/fine-pitch-min-max.fsc
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/patterns/modx-min-max.fsc
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/patterns/mody-min-max.fsc
+-rw-r--r--   0 runner    (1001) docker     (123)   115522 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/patterns/multi-channel.flp
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/patterns/pan-min-max.fsc
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/patterns/release-min-max.fsc
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/patterns/slide-note.fsc
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/patterns/velocity-min-max.fsc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:15:15.472836 pyflp-2.2.1/tests/assets/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/plugins/boobass.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/plugins/fruit-kick.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/plugins/fruity-balance.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/plugins/fruity-blood-overdrive.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/plugins/fruity-center.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/plugins/fruity-fast-dist.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/plugins/fruity-send.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/plugins/fruity-soft-clipper.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/plugins/fruity-stereo-enhancer.fst
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/plugins/fruity-wrapper.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/plugins/plucked.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/plugins/soundgoodizer.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/assets/plugins/xfer-djmfilter.fst
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/test_arrangement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/test_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/test_corrupted.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/test_mixer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/test_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-05 13:15:00.000000 pyflp-2.2.1/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-05 13:15:00.000000 pyflp-2.2.1/tox.ini
```

### Comparing `pyflp-2.2.0/.vscode/extensions.json` & `pyflp-2.2.1/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/.vscode/settings.json` & `pyflp-2.2.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/.vscode/tasks.json` & `pyflp-2.2.1/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/CHANGELOG.md` & `pyflp-2.2.1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [2.2.1] - 2023-06-05
+
+### Fixed
+
+- Python 3.8 compatibility.
+
 ## [2.2.0] - 2023-05-28
 
 ### Changed
 
 - All event parsing happens during `pyflp.parse` itself.
 - `colour.Color` replaced with `pyflp.types.RGBA`.
 - Increase *line-length* of 100.
@@ -687,14 +693,16 @@
 - A lot of potential bugs in `FLObject` subclasses.
 
 ### Known issues
 
 - `flpinfo` doesn't output correctly sometimes due to long strings.
 - Extraneous data dumped sometimes by `InsertSlotEvent.Plugin`, why this is caused is not known.
 
+[2.2.1]: https://github.com/demberto/PyFLP/compare/v2.2.0...v2.2.1
+[2.2.0]: https://github.com/demberto/PyFLP/compare/v2.1.1...v2.2.0
 [2.1.1]: https://github.com/demberto/PyFLP/compare/v2.1.0...v2.1.1
 [2.1.0]: https://github.com/demberto/PyFLP/compare/v2.0.0...v2.1.0
 [2.0.0]: https://github.com/demberto/PyFLP/compare/v2.0.0a7.post0...v2.0.0
 [2.0.0a7]: https://github.com/demberto/PyFLP/compare/v2.0.0a6...v2.0.0a7
 [2.0.0a6]: https://github.com/demberto/PyFLP/compare/v2.0.0a5.post...v2.0.0a6
 [2.0.0a5.post]: https://github.com/demberto/PyFLP/compare/v2.0.0a5...v2.0.0a5.post
 [2.0.0a5]: https://github.com/demberto/PyFLP/compare/v2.0.0a4...v2.0.0a5
```

### Comparing `pyflp-2.2.0/CODE_OF_CONDUCT.md` & `pyflp-2.2.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/LICENSE` & `pyflp-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/PKG-INFO` & `pyflp-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyflp
-Version: 2.2.0
+Version: 2.2.1
 Summary: FL Studio project file parser
 Author-email: demberto <demberto@protonmail.com>
 License: GPL-3.0
 Project-URL: Source, https://github.com/demberto/PyFLP
 Project-URL: Changelog, https://github.com/demberto/PyFLP/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://pyflp.rtfd.io
 Project-URL: Bug Tracker, https://github.com/demberto/PyFLP/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyflp Version: 2.2.0 Summary: FL Studio project
+Metadata-Version: 2.1 Name: pyflp Version: 2.2.1 Summary: FL Studio project
 file parser Author-email: demberto
 protonmail.com> License: GPL-3.0 Project-URL: Source, https://github.com/
 demberto/PyFLP Project-URL: Changelog, https://github.com/demberto/PyFLP/blob/
 master/CHANGELOG.md Project-URL: Documentation, https://pyflp.rtfd.io Project-
 URL: Bug Tracker, https://github.com/demberto/PyFLP/issues Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `pyflp-2.2.0/README.md` & `pyflp-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/Makefile` & `pyflp-2.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/architecture/flp-format.rst` & `pyflp-2.2.1/docs/architecture/flp-format.rst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/architecture/how-it-works.rst` & `pyflp-2.2.1/docs/architecture/how-it-works.rst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/architecture/reference.rst` & `pyflp-2.2.1/docs/architecture/reference.rst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/conf.py` & `pyflp-2.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/contributing.rst` & `pyflp-2.2.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/faq.rst` & `pyflp-2.2.1/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/features.rst` & `pyflp-2.2.1/docs/features.rst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/guides/plugin.rst` & `pyflp-2.2.1/docs/guides/plugin.rst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/guides/reversing.rst` & `pyflp-2.2.1/docs/guides/reversing.rst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/handbook.rst` & `pyflp-2.2.1/docs/handbook.rst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/helping.rst` & `pyflp-2.2.1/docs/helping.rst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/arrangement/preview.jpg` & `pyflp-2.2.1/docs/img/arrangement/preview.jpg`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/arrangement/time-signature.png` & `pyflp-2.2.1/docs/img/arrangement/time-signature.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/arrangement/timemarker/action.png` & `pyflp-2.2.1/docs/img/arrangement/timemarker/action.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/arrangement/timemarker/preview.png` & `pyflp-2.2.1/docs/img/arrangement/timemarker/preview.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/arrangement/track/color.gif` & `pyflp-2.2.1/docs/img/arrangement/track/color.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/arrangement/track/enabled.gif` & `pyflp-2.2.1/docs/img/arrangement/track/enabled.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/arrangement/track/grouped.gif` & `pyflp-2.2.1/docs/img/arrangement/track/grouped.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/arrangement/track/icon.gif` & `pyflp-2.2.1/docs/img/arrangement/track/icon.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/arrangement/track/locked.gif` & `pyflp-2.2.1/docs/img/arrangement/track/locked.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/arrangement/track/motion.png` & `pyflp-2.2.1/docs/img/arrangement/track/motion.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/arrangement/track/performance-settings.png` & `pyflp-2.2.1/docs/img/arrangement/track/performance-settings.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/arrangement/track/press.png` & `pyflp-2.2.1/docs/img/arrangement/track/press.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/arrangement/track/preview.png` & `pyflp-2.2.1/docs/img/arrangement/track/preview.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/arrangement/track/sync.png` & `pyflp-2.2.1/docs/img/arrangement/track/sync.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/channel/arp.png` & `pyflp-2.2.1/docs/img/channel/arp.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/channel/automation.png` & `pyflp-2.2.1/docs/img/channel/automation.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/channel/color.gif` & `pyflp-2.2.1/docs/img/channel/color.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/channel/content.png` & `pyflp-2.2.1/docs/img/channel/content.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/channel/delay.png` & `pyflp-2.2.1/docs/img/channel/delay.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/channel/enabled.gif` & `pyflp-2.2.1/docs/img/channel/enabled.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/channel/envelope.png` & `pyflp-2.2.1/docs/img/channel/envelope.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/channel/filter.png` & `pyflp-2.2.1/docs/img/channel/filter.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/channel/fx1.png` & `pyflp-2.2.1/docs/img/channel/fx1.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/channel/fx2.png` & `pyflp-2.2.1/docs/img/channel/fx2.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/channel/icon.gif` & `pyflp-2.2.1/docs/img/channel/icon.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/channel/keyboard.png` & `pyflp-2.2.1/docs/img/channel/keyboard.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/channel/layer.png` & `pyflp-2.2.1/docs/img/channel/layer.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/channel/level-adjusts.png` & `pyflp-2.2.1/docs/img/channel/level-adjusts.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/channel/lfo.png` & `pyflp-2.2.1/docs/img/channel/lfo.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/channel/locked.gif` & `pyflp-2.2.1/docs/img/channel/locked.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/channel/playback.png` & `pyflp-2.2.1/docs/img/channel/playback.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/channel/polyphony.png` & `pyflp-2.2.1/docs/img/channel/polyphony.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/channel/rack.png` & `pyflp-2.2.1/docs/img/channel/rack.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/channel/sampler.png` & `pyflp-2.2.1/docs/img/channel/sampler.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/channel/stretch-mode.png` & `pyflp-2.2.1/docs/img/channel/stretch-mode.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/channel/stretching.png` & `pyflp-2.2.1/docs/img/channel/stretching.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/channel/time.png` & `pyflp-2.2.1/docs/img/channel/time.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/channel/toolbar.png` & `pyflp-2.2.1/docs/img/channel/toolbar.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/channel/tracking.png` & `pyflp-2.2.1/docs/img/channel/tracking.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/channel/zipped.png` & `pyflp-2.2.1/docs/img/channel/zipped.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/contributing/pytest.svg` & `pyflp-2.2.1/docs/img/contributing/pytest.svg`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/contributing/readthedocs.svg` & `pyflp-2.2.1/docs/img/contributing/readthedocs.svg`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/contributing/vscode.svg` & `pyflp-2.2.1/docs/img/contributing/vscode.svg`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/controller/remote.png` & `pyflp-2.2.1/docs/img/controller/remote.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/features/images-dark.png` & `pyflp-2.2.1/docs/img/features/images-dark.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/features/images-light.png` & `pyflp-2.2.1/docs/img/features/images-light.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/features/tables-dark.png` & `pyflp-2.2.1/docs/img/features/tables-dark.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/features/tables-light.png` & `pyflp-2.2.1/docs/img/features/tables-light.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/guides/plugin/1-parameters.png` & `pyflp-2.2.1/docs/img/guides/plugin/1-parameters.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/guides/plugin/2-load-plugin.png` & `pyflp-2.2.1/docs/img/guides/plugin/2-load-plugin.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/guides/plugin/3-observe-knob-positions.png` & `pyflp-2.2.1/docs/img/guides/plugin/3-observe-knob-positions.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/guides/plugin/4-hint-panel.png` & `pyflp-2.2.1/docs/img/guides/plugin/4-hint-panel.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/guides/reversing/flpedit.png` & `pyflp-2.2.1/docs/img/guides/reversing/flpedit.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/helping/open-issue-dark.png` & `pyflp-2.2.1/docs/img/helping/open-issue-dark.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/helping/open-issue-light.png` & `pyflp-2.2.1/docs/img/helping/open-issue-light.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/helping/star-repo-dark.gif` & `pyflp-2.2.1/docs/img/helping/star-repo-dark.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/helping/star-repo-light.gif` & `pyflp-2.2.1/docs/img/helping/star-repo-light.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/helping/watch-repo-dark.gif` & `pyflp-2.2.1/docs/img/helping/watch-repo-dark.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/helping/watch-repo-light.gif` & `pyflp-2.2.1/docs/img/helping/watch-repo-light.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/mixer/insert/dock.png` & `pyflp-2.2.1/docs/img/mixer/insert/dock.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/mixer/insert/enabled.gif` & `pyflp-2.2.1/docs/img/mixer/insert/enabled.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/mixer/insert/eq.png` & `pyflp-2.2.1/docs/img/mixer/insert/eq.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/mixer/insert/input.png` & `pyflp-2.2.1/docs/img/mixer/insert/input.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/mixer/insert/locked.gif` & `pyflp-2.2.1/docs/img/mixer/insert/locked.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/mixer/insert/output.png` & `pyflp-2.2.1/docs/img/mixer/insert/output.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/mixer/insert/pan.gif` & `pyflp-2.2.1/docs/img/mixer/insert/pan.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/mixer/insert/preview.png` & `pyflp-2.2.1/docs/img/mixer/insert/preview.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/mixer/preview.png` & `pyflp-2.2.1/docs/img/mixer/preview.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/mixer/slot/color.gif` & `pyflp-2.2.1/docs/img/mixer/slot/color.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/mixer/slot/enabled.gif` & `pyflp-2.2.1/docs/img/mixer/slot/enabled.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/mixer/slot/icon.gif` & `pyflp-2.2.1/docs/img/mixer/slot/icon.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/mixer/slot/locked.gif` & `pyflp-2.2.1/docs/img/mixer/slot/locked.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/mixer/slots.png` & `pyflp-2.2.1/docs/img/mixer/slots.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/pattern/color.gif` & `pyflp-2.2.1/docs/img/pattern/color.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/pattern/note/group.gif` & `pyflp-2.2.1/docs/img/pattern/note/group.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/plugin/effects/fruity-balance.png` & `pyflp-2.2.1/docs/img/plugin/effects/fruity-balance.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/plugin/effects/fruity-blood-overdrive.png` & `pyflp-2.2.1/docs/img/plugin/effects/fruity-blood-overdrive.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/plugin/effects/fruity-center.png` & `pyflp-2.2.1/docs/img/plugin/effects/fruity-center.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/plugin/effects/fruity-fast-dist.png` & `pyflp-2.2.1/docs/img/plugin/effects/fruity-fast-dist.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/plugin/effects/fruity-notebook2.png` & `pyflp-2.2.1/docs/img/plugin/effects/fruity-notebook2.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/plugin/effects/fruity-send.png` & `pyflp-2.2.1/docs/img/plugin/effects/fruity-send.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/plugin/effects/fruity-soft-clipper.png` & `pyflp-2.2.1/docs/img/plugin/effects/fruity-soft-clipper.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/plugin/effects/fruity-stereo-enhancer.png` & `pyflp-2.2.1/docs/img/plugin/effects/fruity-stereo-enhancer.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/plugin/effects/soundgoodizer.png` & `pyflp-2.2.1/docs/img/plugin/effects/soundgoodizer.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/plugin/generators/boobass.png` & `pyflp-2.2.1/docs/img/plugin/generators/boobass.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/plugin/generators/fruit-kick.png` & `pyflp-2.2.1/docs/img/plugin/generators/fruit-kick.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/plugin/generators/plucked.png` & `pyflp-2.2.1/docs/img/plugin/generators/plucked.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/plugin/maximize.gif` & `pyflp-2.2.1/docs/img/plugin/maximize.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/plugin/toolbar_collapse.gif` & `pyflp-2.2.1/docs/img/plugin/toolbar_collapse.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/plugin/wrapper/page.gif` & `pyflp-2.2.1/docs/img/plugin/wrapper/page.gif`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/plugin/wrapper/processing.png` & `pyflp-2.2.1/docs/img/plugin/wrapper/processing.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/plugin/wrapper/settings-gui.png` & `pyflp-2.2.1/docs/img/plugin/wrapper/settings-gui.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/plugin/wrapper/settings-midi.png` & `pyflp-2.2.1/docs/img/plugin/wrapper/settings-midi.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/plugin/wrapper/settings.png` & `pyflp-2.2.1/docs/img/plugin/wrapper/settings.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/plugin/wrapper/troubleshooting.png` & `pyflp-2.2.1/docs/img/plugin/wrapper/troubleshooting.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/project/info.png` & `pyflp-2.2.1/docs/img/project/info.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/project/ppq.png` & `pyflp-2.2.1/docs/img/project/ppq.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/project/settings.png` & `pyflp-2.2.1/docs/img/project/settings.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/project/tempo.png` & `pyflp-2.2.1/docs/img/project/tempo.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/project/time-spent.png` & `pyflp-2.2.1/docs/img/project/time-spent.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/img/project/version.png` & `pyflp-2.2.1/docs/img/project/version.png`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/limitations.rst` & `pyflp-2.2.1/docs/limitations.rst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/make.bat` & `pyflp-2.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/reference/arrangement/track.rst` & `pyflp-2.2.1/docs/reference/arrangement/track.rst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/reference/channel/sampler.rst` & `pyflp-2.2.1/docs/reference/channel/sampler.rst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/reference/events.rst` & `pyflp-2.2.1/docs/reference/events.rst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/reference/plugins/vst.rst` & `pyflp-2.2.1/docs/reference/plugins/vst.rst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/docs/reference/project.rst` & `pyflp-2.2.1/docs/reference/project.rst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/pyflp/__init__.py` & `pyflp-2.2.1/pyflp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/pyflp/_adapters.py` & `pyflp-2.2.1/pyflp/_adapters.py`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/pyflp/_descriptors.py` & `pyflp-2.2.1/pyflp/_descriptors.py`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/pyflp/_events.py` & `pyflp-2.2.1/pyflp/_events.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,30 +18,29 @@
 """
 
 from __future__ import annotations
 
 import abc
 import enum
 import warnings
-from collections import UserDict, UserList
 from collections.abc import Callable, Iterable, Iterator, Sequence
 from dataclasses import dataclass, field
 from itertools import zip_longest
 from typing import TYPE_CHECKING, Any, ClassVar, Final, Generic, Tuple, cast
 
 import construct as c
 from sortedcontainers import SortedList
 from typing_extensions import Concatenate, TypeAlias
 
 from pyflp.exceptions import (
     EventIDOutOfRange,
     InvalidEventChunkSize,
     PropertyCannotBeSet,
 )
-from pyflp.types import RGBA, P, T
+from pyflp.types import RGBA, P, T, AnyContainer, AnyListContainer, AnyList, AnyDict
 
 BYTE: Final = 0
 WORD: Final = 64
 DWORD: Final = 128
 TEXT: Final = 192
 DATA: Final = 208
 NEW_TEXT_IDS: Final = (
@@ -322,15 +321,15 @@
         STRUCT = c.ExprAdapter(
             c.GreedyString("utf-16-le"),
             lambda obj, *_: obj.rstrip("\0"),
             lambda obj, *_: obj + "\0",
         )
 
 
-class StructEventBase(EventBase[c.Container[Any]], UserDict[str, Any]):
+class StructEventBase(EventBase[AnyContainer], AnyDict):
     """Base class for events used for storing fixed size structured data.
 
     Consists of a collection of POD types like int, bool, float, but not strings.
     Its size is determined by the event as well as FL version.
     """
 
     def __init__(self, id: EventEnum, data: bytes) -> None:
@@ -343,15 +342,15 @@
 
         if self[key] is None:
             raise PropertyCannotBeSet
 
         self.data[key] = value
 
 
-class ListEventBase(EventBase[c.ListContainer[Any]], UserList[c.Container[Any]]):
+class ListEventBase(EventBase[AnyListContainer], AnyList):
     """Base class for events storing an array of structured data.
 
     Attributes:
         kwds: Keyword args passed to :meth:`STRUCT.parse` & :meth:`STRUCT.build`.
     """
 
     STRUCT: c.Subconstruct[Any, Any, Any, Any]
@@ -419,15 +418,15 @@
     def __init__(
         self,
         parent: EventTree | None = None,
         init: Iterable[IndexedEvent] | None = None,
     ) -> None:
         """Create a new dictionary with an optional :attr:`parent`."""
         self.children: list[EventTree] = []
-        self.lst: list[IndexedEvent] = SortedList(init or [])
+        self.lst: list[IndexedEvent] = SortedList(init or [])  # type: ignore
 
         self.parent = parent
         if parent is not None:
             parent.children.append(self)
 
         while parent is not None and parent.parent is not None:
             parent = parent.parent
```

### Comparing `pyflp-2.2.0/pyflp/_models.py` & `pyflp-2.2.1/pyflp/_models.py`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/pyflp/arrangement.py` & `pyflp-2.2.1/pyflp/arrangement.py`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/pyflp/channel.py` & `pyflp-2.2.1/pyflp/channel.py`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/pyflp/controller.py` & `pyflp-2.2.1/pyflp/controller.py`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/pyflp/exceptions.py` & `pyflp-2.2.1/pyflp/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/pyflp/mixer.py` & `pyflp-2.2.1/pyflp/mixer.py`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/pyflp/pattern.py` & `pyflp-2.2.1/pyflp/pattern.py`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/pyflp/plugin.py` & `pyflp-2.2.1/pyflp/plugin.py`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/pyflp/project.py` & `pyflp-2.2.1/pyflp/project.py`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/pyflp/timemarker.py` & `pyflp-2.2.1/pyflp/timemarker.py`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/pyflp/types.py` & `pyflp-2.2.1/pyflp/types.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,19 +10,21 @@
 # Public License for more details. You should have received a copy of the
 # GNU General Public License along with this program. If not, see
 # <https://www.gnu.org/licenses/>.
 
 from __future__ import annotations
 
 import enum
+from collections import UserDict, UserList
 from dataclasses import dataclass
-from typing import NamedTuple, TypeVar, Union
+from typing import Any, NamedTuple, TypeVar, Union, TYPE_CHECKING
 
+import construct
 import construct_typed as ct
-from typing_extensions import ParamSpec
+from typing_extensions import ParamSpec, TypeAlias
 
 P = ParamSpec("P")
 T = TypeVar("T")
 U = TypeVar("U")
 ET = TypeVar("ET", bound=Union[ct.EnumBase, enum.IntFlag])
 T_co = TypeVar("T_co", covariant=True)
 
@@ -60,7 +62,19 @@
 
     @staticmethod
     def from_bytes(buf: bytes) -> RGBA:
         return RGBA(*(c / 255 for c in buf))
 
     def __bytes__(self) -> bytes:
         return bytes(round(c * 255) for c in self)
+
+
+if TYPE_CHECKING:
+    AnyContainer: TypeAlias = construct.Container[Any]
+    AnyListContainer: TypeAlias = construct.ListContainer[Any]
+    AnyDict: TypeAlias = UserDict[str, Any]
+    AnyList: TypeAlias = UserList[AnyContainer]
+else:
+    AnyContainer = construct.Container
+    AnyListContainer = construct.ListContainer
+    AnyDict = UserDict
+    AnyList = UserList
```

### Comparing `pyflp-2.2.0/pyflp.egg-info/PKG-INFO` & `pyflp-2.2.1/pyflp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyflp
-Version: 2.2.0
+Version: 2.2.1
 Summary: FL Studio project file parser
 Author-email: demberto <demberto@protonmail.com>
 License: GPL-3.0
 Project-URL: Source, https://github.com/demberto/PyFLP
 Project-URL: Changelog, https://github.com/demberto/PyFLP/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://pyflp.rtfd.io
 Project-URL: Bug Tracker, https://github.com/demberto/PyFLP/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyflp Version: 2.2.0 Summary: FL Studio project
+Metadata-Version: 2.1 Name: pyflp Version: 2.2.1 Summary: FL Studio project
 file parser Author-email: demberto
 protonmail.com> License: GPL-3.0 Project-URL: Source, https://github.com/
 demberto/PyFLP Project-URL: Changelog, https://github.com/demberto/PyFLP/blob/
 master/CHANGELOG.md Project-URL: Documentation, https://pyflp.rtfd.io Project-
 URL: Bug Tracker, https://github.com/demberto/PyFLP/issues Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `pyflp-2.2.0/pyflp.egg-info/SOURCES.txt` & `pyflp-2.2.1/pyflp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/pyproject.toml` & `pyflp-2.2.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -74,19 +74,16 @@
 python_version = "3.8"
 check_untyped_defs = true
 enable_incomplete_feature = ["Unpack"]
 ignore_missing_imports = true
 warn_no_return = false
 
 [tool.pyright]
-ignore = ["./venv"]
 reportPrivateUsage = false
 reportMissingTypeStubs = false
-venvPath = "."
-venv = "venv"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "-ra -q"
 testpaths = "tests"
 
 [tool.ruff]
```

### Comparing `pyflp-2.2.0/tests/assets/FL 20.8.4.flp` & `pyflp-2.2.1/tests/assets/FL 20.8.4.flp`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/assets/channels/+4800-cents.fst` & `pyflp-2.2.1/tests/assets/channels/+4800-cents.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/assets/channels/-4800-cents.fst` & `pyflp-2.2.1/tests/assets/channels/-4800-cents.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/assets/channels/100%-left.fst` & `pyflp-2.2.1/tests/assets/channels/100%-left.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/assets/channels/100%-right.fst` & `pyflp-2.2.1/tests/assets/channels/100%-right.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/assets/channels/arp.fst` & `pyflp-2.2.1/tests/assets/channels/arp.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/assets/channels/automation-lfo.fst` & `pyflp-2.2.1/tests/assets/channels/automation-lfo.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/assets/channels/automation-points.fst` & `pyflp-2.2.1/tests/assets/channels/automation-points.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/assets/channels/colored.fst` & `pyflp-2.2.1/tests/assets/channels/colored.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/assets/channels/cut-groups.fst` & `pyflp-2.2.1/tests/assets/channels/cut-groups.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/assets/channels/delay.fst` & `pyflp-2.2.1/tests/assets/channels/delay.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/assets/channels/disabled.fst` & `pyflp-2.2.1/tests/assets/channels/disabled.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/assets/channels/envelope.fst` & `pyflp-2.2.1/tests/assets/channels/envelope.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/assets/channels/full-volume.fst` & `pyflp-2.2.1/tests/assets/channels/full-volume.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/assets/channels/iconified.fst` & `pyflp-2.2.1/tests/assets/channels/iconified.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/assets/channels/keyboard.fst` & `pyflp-2.2.1/tests/assets/channels/keyboard.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/assets/channels/layer-crossfade.fst` & `pyflp-2.2.1/tests/assets/channels/layer-crossfade.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/assets/channels/layer-random.fst` & `pyflp-2.2.1/tests/assets/channels/layer-random.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/assets/channels/level-adjusts.fst` & `pyflp-2.2.1/tests/assets/channels/level-adjusts.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/assets/channels/lfo.fst` & `pyflp-2.2.1/tests/assets/channels/lfo.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/assets/channels/locked.fst` & `pyflp-2.2.1/tests/assets/channels/locked.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/assets/channels/polyphony.fst` & `pyflp-2.2.1/tests/assets/channels/polyphony.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/assets/channels/routed.fst` & `pyflp-2.2.1/tests/assets/channels/routed.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/assets/channels/sampler-content.fst` & `pyflp-2.2.1/tests/assets/channels/sampler-content.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/assets/channels/sampler-filter.fst` & `pyflp-2.2.1/tests/assets/channels/sampler-filter.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/assets/channels/sampler-fx.fst` & `pyflp-2.2.1/tests/assets/channels/sampler-fx.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/assets/channels/sampler-path.fst` & `pyflp-2.2.1/tests/assets/channels/sampler-path.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/assets/channels/sampler-playback.fst` & `pyflp-2.2.1/tests/assets/channels/sampler-playback.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/assets/channels/sampler-stretching.fst` & `pyflp-2.2.1/tests/assets/channels/sampler-stretching.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/assets/channels/time.fst` & `pyflp-2.2.1/tests/assets/channels/time.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/assets/channels/tracking.fst` & `pyflp-2.2.1/tests/assets/channels/tracking.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/assets/channels/zero-volume.fst` & `pyflp-2.2.1/tests/assets/channels/zero-volume.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/assets/inserts/50ms-input-latency.fst` & `pyflp-2.2.1/tests/assets/inserts/50ms-input-latency.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/assets/inserts/50ms-track-latency.fst` & `pyflp-2.2.1/tests/assets/inserts/50ms-track-latency.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/assets/inserts/effects-bypassed.fst` & `pyflp-2.2.1/tests/assets/inserts/effects-bypassed.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/assets/patterns/multi-channel.flp` & `pyflp-2.2.1/tests/assets/patterns/multi-channel.flp`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/assets/plugins/fruit-kick.fst` & `pyflp-2.2.1/tests/assets/plugins/fruit-kick.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/assets/plugins/fruity-wrapper.fst` & `pyflp-2.2.1/tests/assets/plugins/fruity-wrapper.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/assets/plugins/plucked.fst` & `pyflp-2.2.1/tests/assets/plugins/plucked.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/assets/plugins/xfer-djmfilter.fst` & `pyflp-2.2.1/tests/assets/plugins/xfer-djmfilter.fst`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/conftest.py` & `pyflp-2.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/test_arrangement.py` & `pyflp-2.2.1/tests/test_arrangement.py`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/test_channel.py` & `pyflp-2.2.1/tests/test_channel.py`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/test_corrupted.py` & `pyflp-2.2.1/tests/test_corrupted.py`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/test_events.py` & `pyflp-2.2.1/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/test_mixer.py` & `pyflp-2.2.1/tests/test_mixer.py`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/test_pattern.py` & `pyflp-2.2.1/tests/test_pattern.py`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/test_plugin.py` & `pyflp-2.2.1/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tests/test_project.py` & `pyflp-2.2.1/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `pyflp-2.2.0/tox.ini` & `pyflp-2.2.1/tox.ini`

 * *Files 15% similar despite different names*

```diff
@@ -10,14 +10,15 @@
   mypy
   pytest
 commands =
   coverage run -m pytest
   mypy pyflp
 
 [testenv:precommit]
+skip_install = True
 deps = pre-commit
 commands = pre-commit run --all-files
 
 [testenv:docs]
 # Exclude GH Actions Mac OS runners due to PyEnchant (needed by sphinxcontrib.spelling)
 # issue on Apple silicon, see https://github.com/pyenchant/pyenchant/issues/265
 platform = ^((?!darwin).)*$
```

