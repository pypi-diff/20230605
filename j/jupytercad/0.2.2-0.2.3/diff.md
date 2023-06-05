# Comparing `tmp/jupytercad-0.2.2.tar.gz` & `tmp/jupytercad-0.2.3.tar.gz`

## Comparing `jupytercad-0.2.2.tar` & `jupytercad-0.2.3.tar`

### file list

```diff
@@ -1,725 +1,725 @@
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupytercad-0.2.2/.eslintignore
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 jupytercad-0.2.2/.eslintrc.js
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 jupytercad-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 jupytercad-0.2.2/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupytercad-0.2.2/.prettierrc
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupytercad-0.2.2/.yarnrc.yml
--rw-r--r--   0        0        0    21322 2020-02-02 00:00:00.000000 jupytercad-0.2.2/CHANGELOG.md
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 jupytercad-0.2.2/CONTRIBUTING.md
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 jupytercad-0.2.2/RELEASE.md
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 jupytercad-0.2.2/install.json
--rw-r--r--   0        0        0   196437 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad-screenshot.png
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 jupytercad-0.2.2/lerna.json
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 jupytercad-0.2.2/package.json
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupytercad-0.2.2/setup.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupytercad-0.2.2/tsconfig.eslint.json
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 jupytercad-0.2.2/tsconfigbase.json
--rw-r--r--   0        0        0   435349 2020-02-02 00:00:00.000000 jupytercad-0.2.2/yarn.lock
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 jupytercad-0.2.2/etc/jupyter/jupyter_server_config.d/jupytercad.json
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/_version.py
--rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/fcstd_ydoc.py
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/jcad_ydoc.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/__init__.py
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/cadapp.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/utils.py
--rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/application-extension/commands.json
--rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/application-extension/context-menu.json
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/application-extension/package.json.orig
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/application-extension/property-inspector.json
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/application-extension/shell.json
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/application-extension/top-bar.json
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/apputils-extension/notification.json
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/apputils-extension/package.json.orig
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/apputils-extension/palette.json
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/apputils-extension/print.json
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/apputils-extension/sanitizer.json
--rw-r--r--   0        0        0     3717 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/apputils-extension/themes.json
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/apputils-extension/utilityCommands.json
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/apputils-extension/workspaces.json
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/codemirror-extension/package.json.orig
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/codemirror-extension/plugin.json
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/docmanager-extension/download.json
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/docmanager-extension/package.json.orig
--rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/docmanager-extension/plugin.json
--rw-r--r--   0        0        0     6134 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/filebrowser-extension/browser.json
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/filebrowser-extension/download.json
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/filebrowser-extension/open-browser-tab.json
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/filebrowser-extension/open-with.json
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/filebrowser-extension/package.json.orig
--rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/filebrowser-extension/widget.json
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/launcher-extension/package.json.orig
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/launcher-extension/plugin.json
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/mainmenu-extension/package.json.orig
--rw-r--r--   0        0        0     9894 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/mainmenu-extension/plugin.json
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/translation-extension/package.json.orig
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/translation-extension/plugin.json
--rw-r--r--   0        0        0    10149 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/103.app.js
--rw-r--r--   0        0        0     7215 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/1053.app.js
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/1058.app.js
--rw-r--r--   0        0        0   302401 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/1072.app.js
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/1072.app.js.LICENSE.txt
--rw-r--r--   0        0        0   128612 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/1123.app.js
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/1123.app.js.LICENSE.txt
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/1152.app.js
--rw-r--r--   0        0        0    33344 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/1186.app.js
--rw-r--r--   0        0        0    14228 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/1208.app.js
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/1210.app.js
--rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/1222.app.js
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/1227.app.js
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/1278.app.js
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/1286.app.js
--rw-r--r--   0        0        0     6784 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/13.app.js
--rw-r--r--   0        0        0    20577 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/1320.app.js
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/1322.app.js
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/1377.app.js
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/1403.app.js
--rw-r--r--   0        0        0     9838 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/15.app.js
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/151.app.js
--rw-r--r--   0        0        0   214831 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/1520.app.js
--rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/1567.app.js
--rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/1580.app.js
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/1581.app.js
--rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/1623.app.js
--rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/1729.app.js
--rw-r--r--   0        0        0    12512 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/1746.app.js
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/1770.app.js
--rw-r--r--   0        0        0    60948 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/1880.app.js
--rw-r--r--   0        0        0     9036 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/1882.app.js
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/1935.app.js
--rw-r--r--   0        0        0   199427 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/1959.app.js
--rw-r--r--   0        0        0     8068 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/2033.app.js
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/2042.app.js
--rw-r--r--   0        0        0    24578 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/2075.app.js
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/2100.app.js
--rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/2106.app.js
--rw-r--r--   0        0        0    11835 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/2185.app.js
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/2194.app.js
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/2266.app.js
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/2284.app.js
--rw-r--r--   0        0        0    14227 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/23.app.js
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/231.app.js
--rw-r--r--   0        0        0    77242 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/2318.app.js
--rw-r--r--   0        0        0     9467 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/2488.app.js
--rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/2502.app.js
--rw-r--r--   0        0        0    39462 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/2553.app.js
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/2563.app.js
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/2628.app.js
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/2667.app.js
--rw-r--r--   0        0        0    13343 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/2687.app.js
--rw-r--r--   0        0        0    25924 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/274.app.js
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/275.app.js
--rw-r--r--   0        0        0     6617 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/2784.app.js
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/2784.app.js.LICENSE.txt
--rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/2805.app.js
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/288.app.js
--rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/2970.app.js
--rw-r--r--   0        0        0     4978 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/3007.app.js
--rw-r--r--   0        0        0     9009 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/3093.app.js
--rw-r--r--   0        0        0     5911 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/3159.app.js
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/3191.app.js
--rw-r--r--   0        0        0     9662 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/3192.app.js
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/3206.app.js
--rw-r--r--   0        0        0    16702 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/3211.app.js
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/3265.app.js
--rw-r--r--   0        0        0   432933 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/330.app.js
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/3312.app.js
--rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/3316.app.js
--rw-r--r--   0        0        0    14228 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/3324.app.js
--rw-r--r--   0        0        0   171985 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/3326.app.js
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/3330.app.js
--rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/3397.app.js
--rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/3466.app.js
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/3499.app.js
--rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/3500.app.js
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/351.app.js
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/3540.app.js
--rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/3542.app.js
--rw-r--r--   0        0        0   169327 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/358.app.js
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/360.app.js
--rw-r--r--   0        0        0  1020115 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/3656.app.js
--rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/3656.app.js.LICENSE.txt
--rw-r--r--   0        0        0     6711 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/370.app.js
--rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/3726.app.js
--rw-r--r--   0        0        0   203030 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/373c04fd2418f5c77eea.eot
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/3811.app.js
--rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/3851.app.js
--rw-r--r--   0        0        0    61590 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/3855.app.js
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/386.app.js
--rw-r--r--   0        0        0    46084 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/3872.app.js
--rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/3880.app.js
--rw-r--r--   0        0        0   101648 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/3f6d3488cf65374f6f67.woff
--rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/4024.app.js
--rw-r--r--   0        0        0     5267 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/4040.app.js
--rw-r--r--   0        0        0     9009 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/4059.app.js
--rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/4065.app.js
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/4073.app.js
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/4123.app.js
--rw-r--r--   0        0        0    52558 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/4171.app.js
--rw-r--r--   0        0        0     6636 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/4282.app.js
--rw-r--r--   0        0        0    10948 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/4283.app.js
--rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/4299.app.js
--rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/4351.app.js
--rw-r--r--   0        0        0    16452 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/4359.app.js
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/4391.app.js
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/4403.app.js
--rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/4462.app.js
--rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/4476.app.js
--rw-r--r--   0        0        0   143645 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/450.app.js
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/4608.app.js
--rw-r--r--   0        0        0    18653 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/4651.app.js
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/4651.app.js.LICENSE.txt
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/4654.app.js
--rw-r--r--   0        0        0    23079 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/4679.app.js
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/4702.app.js
--rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/4718.app.js
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/4808.app.js
--rw-r--r--   0        0        0    15011 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/484.app.js
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/4874.app.js
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/4878.app.js
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/4935.app.js
--rw-r--r--   0        0        0    27298 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/4965.app.js
--rw-r--r--   0        0        0    69298 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/4973.app.js
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/4973.app.js.LICENSE.txt
--rw-r--r--   0        0        0    22107 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/4982.app.js
--rw-r--r--   0        0        0    62789 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/5002.app.js
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/5024.app.js
--rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/504.app.js
--rw-r--r--   0        0        0     6711 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/5064.app.js
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/5101.app.js
--rw-r--r--   0        0        0    94906 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/5148.app.js
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/5172.app.js
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/5176.app.js
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/5223.app.js
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/5225.app.js
--rw-r--r--   0        0        0    86931 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/5231.app.js
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/5263.app.js
--rw-r--r--   0        0        0   101929 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/5340.app.js
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/5393.app.js
--rw-r--r--   0        0        0   180936 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/5430.app.js
--rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/5433.app.js
--rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/5445.app.js
--rw-r--r--   0        0        0    24464 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/550.app.js
--rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/5513.app.js
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/5514.app.js
--rw-r--r--   0        0        0    18861 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/5544.app.js
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/5556.app.js
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/558.app.js
--rw-r--r--   0        0        0    10154 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/5587.app.js
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/5681.app.js
--rw-r--r--   0        0        0    68549 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/5708.app.js
--rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/5764.app.js
--rw-r--r--   0        0        0     6452 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/5811.app.js
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/5817.app.js
--rw-r--r--   0        0        0     5242 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/5876.app.js
--rw-r--r--   0        0        0     7078 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/5882.app.js
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/5882.app.js.LICENSE.txt
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/6146.app.js
--rw-r--r--   0        0        0     4683 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/6151.app.js
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/6186.app.js
--rw-r--r--   0        0        0    10302 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/6196.app.js
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/6410.app.js
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/6483.app.js
--rw-r--r--   0        0        0    30696 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/6510.app.js
--rw-r--r--   0        0        0    37190 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/6645.app.js
--rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/6686.app.js
--rw-r--r--   0        0        0     9416 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/6770.app.js
--rw-r--r--   0        0        0    49485 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/6778.app.js
--rw-r--r--   0        0        0    12106 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/6782.app.js
--rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/6808.app.js
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/6833.app.js
--rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/6835.app.js
--rw-r--r--   0        0        0    99172 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/6914.app.js
--rw-r--r--   0        0        0     7871 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/6970.app.js
--rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/7058.app.js
--rw-r--r--   0        0        0    65804 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/7102.app.js
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/7111.app.js
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/7127.app.js
--rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/7149.app.js
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/7174.app.js
--rw-r--r--   0        0        0    27083 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/7233.app.js
--rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/7236.app.js
--rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/7294.app.js
--rw-r--r--   0        0        0    11619 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/730.app.js
--rw-r--r--   0        0        0     4177 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/7377.app.js
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/7379.app.js
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/7424.app.js
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/7469.app.js
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/7498.app.js
--rw-r--r--   0        0        0    33625 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/7526.app.js
--rw-r--r--   0        0        0    40106 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/7529.app.js
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/7600.app.js
--rw-r--r--   0        0        0     6490 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/765.app.js
--rw-r--r--   0        0        0    22254 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/7664.app.js
--rw-r--r--   0        0        0    65777 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/769.app.js
--rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/7710.app.js
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/7806.app.js
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/7860.app.js
--rw-r--r--   0        0        0     7432 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/7882.app.js
--rw-r--r--   0        0        0    17079 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/7884.app.js
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/7955.app.js
--rw-r--r--   0        0        0   103425 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/7991.app.js
--rw-r--r--   0        0        0    34034 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/79d088064beb3826054f.eot
--rw-r--r--   0        0        0   199428 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/8078.app.js
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/8090.app.js
--rw-r--r--   0        0        0   113878 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/8100.app.js
--rw-r--r--   0        0        0    47563 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/8124.app.js
--rw-r--r--   0        0        0    54614 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/8138.app.js
--rw-r--r--   0        0        0     8337 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/819.app.js
--rw-r--r--   0        0        0     6571 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/8307.app.js
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/8342.app.js
--rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/8409.app.js
--rw-r--r--   0        0        0    25262 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/8423.app.js
--rw-r--r--   0        0        0    25112 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/8441.app.js
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/8442.app.js
--rw-r--r--   0        0        0     6447 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/846.app.js
--rw-r--r--   0        0        0    66111 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/8466.app.js
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/8496.app.js
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/8518.app.js
--rw-r--r--   0        0        0    17922 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/8561.app.js
--rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/8576.app.js
--rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/8615.app.js
--rw-r--r--   0        0        0    40918 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/8640.app.js
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/8658.app.js
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/8662.app.js
--rw-r--r--   0        0        0    10154 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/8728.app.js
--rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/8763.app.js
--rw-r--r--   0        0        0    39773 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/8769.app.js
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/8782.app.js
--rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/8803.app.js
--rw-r--r--   0        0        0   292717 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/882.app.js
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/8866.app.js
--rw-r--r--   0        0        0     4537 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/8877.app.js
--rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/8914.app.js
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/8953.app.js
--rw-r--r--   0        0        0    76736 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/8ea8791754915a898a31.woff2
--rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/9036.app.js
--rw-r--r--   0        0        0     7780 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/9060.app.js
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/9117.app.js
--rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/9172.app.js
--rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/9304.app.js
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/9308.app.js
--rw-r--r--   0        0        0     6452 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/9318.app.js
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/9319.app.js
--rw-r--r--   0        0        0     8950 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/9339.app.js
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/9369.app.js
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/9397.app.js
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/9406.app.js
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/9411.app.js
--rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/9472.app.js
--rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/9473.app.js
--rw-r--r--   0        0        0   253965 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/9491.app.js
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/9491.app.js.LICENSE.txt
--rw-r--r--   0        0        0     6712 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/9513.app.js
--rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/9583.app.js
--rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/9631.app.js
--rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/9636.app.js
--rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/9672.app.js
--rw-r--r--   0        0        0   918991 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/9674eb1bd55047179038.svg
--rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/9715.app.js
--rw-r--r--   0        0        0    16181 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/9787.app.js
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/9787.app.js.LICENSE.txt
--rw-r--r--   0        0        0    10153 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/9811.app.js
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/9822.app.js
--rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/9827.app.js
--rw-r--r--   0        0        0    78268 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/9834b82ad26e2a37583d.woff2
--rw-r--r--   0        0        0     9146 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/9866.app.js
--rw-r--r--   0        0        0    59178 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/9877.app.js
--rw-r--r--   0        0        0   138733 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/9908.app.js
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/9908.app.js.LICENSE.txt
--rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/9932.app.js
--rw-r--r--   0        0        0    22523 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/9961.app.js
--rw-r--r--   0        0        0   569513 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/9976.app.js
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/9976.app.js.LICENSE.txt
--rw-r--r--   0        0        0   747927 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/a3b9817780214caf01e8.svg
--rw-r--r--   0        0        0   202744 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/af6397503fcefbd61397.ttf
--rw-r--r--   0        0        0    33575 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/app.js
--rw-r--r--   0        0        0   144714 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/be0a084962d8066884f7.svg
--rw-r--r--   0        0        0    16276 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/cb9e9e693192413cde2b.woff
--rw-r--r--   0        0        0   133988 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/cda59d6efffa685830fd.ttf
--rw-r--r--   0        0        0   134294 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/e4299464e7b012968eed.eot
--rw-r--r--   0        0        0    13224 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/e42a88444448ac3d6054.woff2
--rw-r--r--   0        0        0    33736 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/e8711bbb871afd8e9dea.ttf
--rw-r--r--   0        0        0    89988 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/static/f9217f66874b0c01cd8c.woff
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/templates/index.html
--rw-r--r--   0        0        0    17760 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/themes/@jupyterlab/theme-dark-extension/index.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/themes/@jupyterlab/theme-dark-extension/index.js
--rw-r--r--   0        0        0    16493 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/themes/@jupyterlab/theme-light-extension/index.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/cadapp/themes/@jupyterlab/theme-light-extension/index.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/freecad/__init__.py
--rw-r--r--   0        0        0     6406 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/freecad/loader.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/freecad/props/__init__.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/freecad/props/base_prop.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/freecad/props/property_angle.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/freecad/props/property_bool.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/freecad/props/property_distance.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/freecad/props/property_geometrylist.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/freecad/props/property_length.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/freecad/props/property_link.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/freecad/props/property_link_list.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/freecad/props/property_map.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/freecad/props/property_partshape.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/freecad/props/property_placement.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/freecad/props/geometry/__init__.py
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/freecad/props/geometry/geom_circle.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/freecad/props/geometry/geom_linesegment.py
--rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/labextension/package.json
--rw-r--r--   0        0        0    52115 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/labextension/static/184.6f76dd957e411be19baa.js
--rw-r--r--   0        0        0    86711 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/labextension/static/213.778b3209dbe7ec5470b6.js
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/labextension/static/268.16c8a4126908b03651f0.js
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/labextension/static/288.11fba3e29cc454c9c071.js
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/labextension/static/358.45fb46ea24bb44ba7fa9.js
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/labextension/static/379.5df518c877987fc7ca0c.js
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/labextension/static/406.5ed89c99d9b3043c85c0.js
--rw-r--r--   0        0        0    59793 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/labextension/static/422.39a95e19d3a414516796.js
--rw-r--r--   0        0        0    10419 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/labextension/static/52.477d969cb88d8007c4f0.js
--rw-r--r--   0        0        0   124222 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/labextension/static/544.40107d96caa6825dcd16.js
--rw-r--r--   0        0        0     8094 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/labextension/static/643.850e055919134443b4fa.js
--rw-r--r--   0        0        0    18686 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/labextension/static/651.3736a4bd9cf2725cc067.js
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/labextension/static/651.3736a4bd9cf2725cc067.js.LICENSE.txt
--rw-r--r--   0        0        0    12432 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/labextension/static/711.9ae86a9a4b0e0a748ae7.js
--rw-r--r--   0        0        0     8086 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/labextension/static/712.3d4b32523dbb4dff584d.js
--rw-r--r--   0        0        0   183517 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/labextension/static/730.5a8c1aad713514a0a596.js
--rw-r--r--   0        0        0   116747 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/labextension/static/733.89a6a4e0561966230286.js
--rw-r--r--   0        0        0    31683 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/labextension/static/761.1bd8bdc8d51f62af816d.js
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/labextension/static/761.1bd8bdc8d51f62af816d.js.LICENSE.txt
--rw-r--r--   0        0        0     8567 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/labextension/static/78.8e87e13a67c31f2732c7.js
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/labextension/static/811.d1c8b6a87faba2d069bd.js
--rw-r--r--   0        0        0     6111 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/labextension/static/816.00326e9e5f2436d0d67f.js
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/labextension/static/833.253bc84b61cd4e2beb80.js
--rw-r--r--   0        0        0   254953 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/labextension/static/842.116bb3340768f53ea709.js
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/labextension/static/842.116bb3340768f53ea709.js.LICENSE.txt
--rw-r--r--   0        0        0    13339 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/labextension/static/847.6efcc69e25d704ee7090.js
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/labextension/static/860.9dcab30c320fd0b9cfe1.js
--rw-r--r--   0        0        0   623572 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/labextension/static/955.a084e75defa008fca238.js
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/labextension/static/955.a084e75defa008fca238.js.LICENSE.txt
--rw-r--r--   0        0        0   114029 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/labextension/static/963.ba192cdc34bc5ccdfe40.js
--rw-r--r--   0        0        0  5065593 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/labextension/static/jupytercad.opencascade.wasm
--rw-r--r--   0        0        0    13025 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/labextension/static/remoteEntry.ed192893ffeb37154379.js
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/labextension/static/style.js
--rw-r--r--   0        0        0    67986 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/notebook/__init__.py
--rw-r--r--   0        0        0    22888 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/notebook/cad_document.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/notebook/utils.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/notebook/y_connector.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/notebook/objects/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/notebook/objects/_schema/__init__.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/notebook/objects/_schema/box.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/notebook/objects/_schema/cone.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/notebook/objects/_schema/cut.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/notebook/objects/_schema/cylinder.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/notebook/objects/_schema/extrusion.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/notebook/objects/_schema/fuse.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/notebook/objects/_schema/geomCircle.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/notebook/objects/_schema/geomLineSegment.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/notebook/objects/_schema/intersection.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/notebook/objects/_schema/jcad.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/notebook/objects/_schema/placement.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/notebook/objects/_schema/sketch.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/notebook/objects/_schema/sphere.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 jupytercad-0.2.2/jupytercad/notebook/objects/_schema/torus.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 jupytercad-0.2.2/scripts/bump-version.py
--rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/package.json
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/tsconfig.json
--rw-r--r--   0        0        0   132758 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/tsconfig.tsbuildinfo
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/webpack.config.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/build/bootstrap.d.ts
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/build/bootstrap.js
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/build/main.d.ts
--rw-r--r--   0        0        0     6407 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/build/main.js
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/build/sharedscope.d.ts
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/build/sharedscope.js
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/build/style.js
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/build/app/app.d.ts
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/build/app/app.js
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/build/app/shell.d.ts
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/build/app/shell.js
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/build/app/plugins/browser/index.d.ts
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/build/app/plugins/browser/index.js
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/build/app/plugins/launcher/index.d.ts
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/build/app/plugins/launcher/index.js
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/build/app/plugins/mainmenu/index.d.ts
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/build/app/plugins/mainmenu/index.js
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/build/app/plugins/mainmenu/menuWidget.d.ts
--rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/build/app/plugins/mainmenu/menuWidget.js
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/build/app/plugins/mainmenu/titleWidget.d.ts
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/build/app/plugins/mainmenu/titleWidget.js
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/build/app/plugins/mainmenu/userWidget.d.ts
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/build/app/plugins/mainmenu/userWidget.js
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/build/app/plugins/paths/index.d.ts
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/build/app/plugins/paths/index.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/lib/bootstrap.d.ts
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/lib/bootstrap.js
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/lib/main.d.ts
--rw-r--r--   0        0        0     6407 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/lib/main.js
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/lib/sharedscope.d.ts
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/lib/sharedscope.js
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/lib/app/app.d.ts
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/lib/app/app.js
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/lib/app/shell.d.ts
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/lib/app/shell.js
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/lib/app/plugins/browser/index.d.ts
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/lib/app/plugins/browser/index.js
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/lib/app/plugins/launcher/index.d.ts
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/lib/app/plugins/launcher/index.js
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/lib/app/plugins/mainmenu/index.d.ts
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/lib/app/plugins/mainmenu/index.js
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/lib/app/plugins/mainmenu/menuWidget.d.ts
--rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/lib/app/plugins/mainmenu/menuWidget.js
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/lib/app/plugins/mainmenu/titleWidget.d.ts
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/lib/app/plugins/mainmenu/titleWidget.js
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/lib/app/plugins/mainmenu/userWidget.d.ts
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/lib/app/plugins/mainmenu/userWidget.js
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/lib/app/plugins/paths/index.d.ts
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/lib/app/plugins/paths/index.js
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/src/bootstrap.ts
--rw-r--r--   0        0        0     6198 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/src/main.ts
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/src/sharedscope.ts
--rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/src/app/app.ts
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/src/app/shell.ts
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/src/app/plugins/browser/index.ts
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/src/app/plugins/launcher/index.ts
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/src/app/plugins/mainmenu/index.ts
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/src/app/plugins/mainmenu/menuWidget.ts
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/src/app/plugins/mainmenu/titleWidget.tsx
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/src/app/plugins/mainmenu/userWidget.tsx
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/src/app/plugins/paths/index.ts
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-app/style/index.js
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/extension.webpack.config.js
--rw-r--r--   0        0        0     4637 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/package.json
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/schema.js
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/tsconfig.json
--rw-r--r--   0        0        0   189578 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/tsconfig.tsbuildinfo
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/tsconfig.worker.json
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/worker.webpack.config.js
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/commands.d.ts
--rw-r--r--   0        0        0    23175 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/commands.js
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/factory.d.ts
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/factory.js
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/formdialog.d.ts
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/formdialog.js
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/index.d.ts
--rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/index.js
--rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/mainview.d.ts
--rw-r--r--   0        0        0    37791 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/mainview.js
--rw-r--r--   0        0        0     4466 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/model.d.ts
--rw-r--r--   0        0        0    10228 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/model.js
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/token.d.ts
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/token.js
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/tools.d.ts
--rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/tools.js
--rw-r--r--   0        0        0     6742 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/types.d.ts
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/types.js
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/widget.d.ts
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/widget.js
--rw-r--r--   0        0        0    86564 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/worker.js
--rw-r--r--   0        0        0    26960 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/_interface/forms.json
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/annotation/message.d.ts
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/annotation/message.js
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/annotation/model.d.ts
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/annotation/model.js
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/annotation/view.d.ts
--rw-r--r--   0        0        0     4537 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/annotation/view.js
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/fcplugin/modelfactory.d.ts
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/fcplugin/modelfactory.js
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/fcplugin/plugins.d.ts
--rw-r--r--   0        0        0     4817 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/fcplugin/plugins.js
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/jcadplugin/modelfactory.d.ts
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/jcadplugin/modelfactory.js
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/jcadplugin/plugins.d.ts
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/jcadplugin/plugins.js
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/notebookrenderer/index.d.ts
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/notebookrenderer/index.js
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/notebookrenderer/model.d.ts
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/notebookrenderer/model.js
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/notebookrenderer/token.d.ts
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/notebookrenderer/token.js
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/notebookrenderer/view.d.ts
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/notebookrenderer/view.js
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/notebookrenderer/widgetManager.d.ts
--rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/notebookrenderer/widgetManager.js
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/notebookrenderer/yCommProvider.d.ts
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/notebookrenderer/yCommProvider.js
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/panelview/annotations.d.ts
--rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/panelview/annotations.js
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/panelview/formbuilder.d.ts
--rw-r--r--   0        0        0     6348 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/panelview/formbuilder.js
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/panelview/header.d.ts
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/panelview/header.js
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/panelview/leftpanel.d.ts
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/panelview/leftpanel.js
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/panelview/model.d.ts
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/panelview/model.js
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/panelview/objectproperties.d.ts
--rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/panelview/objectproperties.js
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/panelview/objecttree.d.ts
--rw-r--r--   0        0        0    12942 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/panelview/objecttree.js
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/panelview/rightpanel.d.ts
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/panelview/rightpanel.js
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/schema/box.json
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/schema/cone.json
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/schema/cut.json
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/schema/cylinder.json
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/schema/extrusion.json
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/schema/fuse.json
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/schema/geomCircle.json
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/schema/geomLineSegment.json
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/schema/intersection.json
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/schema/jcad.json
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/schema/placement.json
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/schema/sketch.json
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/schema/sphere.json
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/schema/torus.json
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/sketcher/helper.d.ts
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/sketcher/helper.js
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/sketcher/panzoom.d.ts
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/sketcher/panzoom.js
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/sketcher/sketcherdialog.d.ts
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/sketcher/sketcherdialog.js
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/sketcher/sketchermodel.d.ts
--rw-r--r--   0        0        0     6417 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/sketcher/sketchermodel.js
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/sketcher/sketcherwidget.d.ts
--rw-r--r--   0        0        0    19357 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/sketcher/sketcherwidget.js
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/sketcher/types.d.ts
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/sketcher/types.js
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/sketcher/elements/circle.d.ts
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/sketcher/elements/circle.js
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/sketcher/elements/line.d.ts
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/sketcher/elements/line.js
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/sketcher/elements/point.d.ts
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/sketcher/elements/point.js
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/toolbar/usertoolbaritem.d.ts
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/toolbar/usertoolbaritem.js
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/toolbar/widget.d.ts
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/toolbar/widget.js
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/worker/actions.d.ts
--rw-r--r--   0        0        0     6797 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/worker/actions.js
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/worker/occapi.d.ts
--rw-r--r--   0        0        0     8828 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/worker/occapi.js
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/worker/occparser.d.ts
--rw-r--r--   0        0        0     8462 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/worker/occparser.js
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/worker/operatorcache.d.ts
--rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/worker/operatorcache.js
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/worker/types.d.ts
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/worker/types.js
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/worker/utils.d.ts
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/worker/utils.js
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/worker/worker.d.ts
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/worker/worker.js
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/worker/geometry/geomCircle.d.ts
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/worker/geometry/geomCircle.js
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/worker/geometry/geomLineSegment.d.ts
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/lib/worker/geometry/geomLineSegment.js
--rw-r--r--   0        0        0    19412 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/commands.ts
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/factory.ts
--rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/formdialog.tsx
--rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/index.ts
--rw-r--r--   0        0        0    34821 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/mainview.tsx
--rw-r--r--   0        0        0    11815 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/model.ts
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/svg.d.ts
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/token.ts
--rw-r--r--   0        0        0     6187 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/tools.ts
--rw-r--r--   0        0        0     6416 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/types.ts
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/widget.tsx
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/_interface/box.d.ts
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/_interface/cone.d.ts
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/_interface/cut.d.ts
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/_interface/cylinder.d.ts
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/_interface/extrusion.d.ts
--rw-r--r--   0        0        0    19613 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/_interface/forms.json
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/_interface/fuse.d.ts
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/_interface/geomCircle.d.ts
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/_interface/geomLineSegment.d.ts
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/_interface/intersection.d.ts
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/_interface/jcad.d.ts
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/_interface/placement.d.ts
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/_interface/sketch.d.ts
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/_interface/sphere.d.ts
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/_interface/torus.d.ts
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/annotation/message.tsx
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/annotation/model.ts
--rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/annotation/view.tsx
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/fcplugin/modelfactory.ts
--rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/fcplugin/plugins.ts
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/jcadplugin/modelfactory.ts
--rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/jcadplugin/plugins.ts
--rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/notebookrenderer/index.ts
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/notebookrenderer/model.ts
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/notebookrenderer/token.ts
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/notebookrenderer/view.ts
--rw-r--r--   0        0        0     3587 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/notebookrenderer/widgetManager.ts
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/notebookrenderer/yCommProvider.ts
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/panelview/annotations.tsx
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/panelview/formbuilder.tsx
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/panelview/header.tsx
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/panelview/leftpanel.tsx
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/panelview/model.ts
--rw-r--r--   0        0        0     7437 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/panelview/objectproperties.tsx
--rw-r--r--   0        0        0    12066 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/panelview/objecttree.tsx
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/panelview/rightpanel.tsx
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/schema/box.json
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/schema/cone.json
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/schema/cut.json
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/schema/cylinder.json
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/schema/extrusion.json
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/schema/fuse.json
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/schema/geomCircle.json
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/schema/geomLineSegment.json
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/schema/intersection.json
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/schema/jcad.json
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/schema/placement.json
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/schema/sketch.json
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/schema/sphere.json
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/schema/torus.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/sketcher/helper.tsx
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/sketcher/panzoom.ts
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/sketcher/sketcherdialog.tsx
--rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/sketcher/sketchermodel.ts
--rw-r--r--   0        0        0    16285 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/sketcher/sketcherwidget.tsx
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/sketcher/types.ts
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/sketcher/elements/circle.ts
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/sketcher/elements/line.ts
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/sketcher/elements/point.ts
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/toolbar/usertoolbaritem.tsx
--rw-r--r--   0        0        0     4157 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/toolbar/widget.tsx
--rw-r--r--   0        0        0     6891 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/worker/actions.ts
--rw-r--r--   0        0        0    10134 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/worker/occapi.ts
--rw-r--r--   0        0        0     8609 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/worker/occparser.ts
--rw-r--r--   0        0        0     3587 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/worker/operatorcache.ts
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/worker/types.ts
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/worker/utils.ts
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/worker/worker.ts
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/worker/geometry/geomCircle.ts
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/src/worker/geometry/geomLineSegment.ts
--rw-r--r--   0        0        0     7174 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/style/index.js
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/style/icon/axes.svg
--rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/style/icon/box.svg
--rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/style/icon/cone.svg
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/style/icon/cut.svg
--rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/style/icon/cylinder.svg
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/style/icon/extrusion.svg
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/style/icon/intersection.svg
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/style/icon/jvcontrol.svg
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/style/icon/minimize.svg
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/style/icon/sphere.svg
--rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/style/icon/torus.svg
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/style/icon/union.svg
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/style/icon/visibility.svg
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-extension/style/icon/visibilityOff.svg
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-opencascade/build.yml
--rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-opencascade/build_opencascade.js
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-opencascade/package.json
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-opencascade/lib/build.yml
--rw-r--r--   0        0        0   129654 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-opencascade/lib/jupytercad.opencascade.d.ts
--rw-r--r--   0        0        0   123823 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-opencascade/lib/jupytercad.opencascade.js
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-opencascade/lib/jupytercad.opencascade.version
--rwxr-xr-x   0        0        0  5065593 2020-02-02 00:00:00.000000 jupytercad-0.2.2/packages/jupytercad-opencascade/lib/jupytercad.opencascade.wasm
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 jupytercad-0.2.2/.gitignore
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 jupytercad-0.2.2/LICENSE
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 jupytercad-0.2.2/README.md
--rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 jupytercad-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 jupytercad-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupytercad-0.2.3/.eslintignore
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 jupytercad-0.2.3/.eslintrc.js
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 jupytercad-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 jupytercad-0.2.3/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupytercad-0.2.3/.prettierrc
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupytercad-0.2.3/.yarnrc.yml
+-rw-r--r--   0        0        0    21949 2020-02-02 00:00:00.000000 jupytercad-0.2.3/CHANGELOG.md
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 jupytercad-0.2.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 jupytercad-0.2.3/RELEASE.md
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 jupytercad-0.2.3/install.json
+-rw-r--r--   0        0        0   196437 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad-screenshot.png
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 jupytercad-0.2.3/lerna.json
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 jupytercad-0.2.3/package.json
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupytercad-0.2.3/setup.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupytercad-0.2.3/tsconfig.eslint.json
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 jupytercad-0.2.3/tsconfigbase.json
+-rw-r--r--   0        0        0   435349 2020-02-02 00:00:00.000000 jupytercad-0.2.3/yarn.lock
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 jupytercad-0.2.3/etc/jupyter/jupyter_server_config.d/jupytercad.json
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/_version.py
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/fcstd_ydoc.py
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/jcad_ydoc.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/__init__.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/cadapp.py
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/utils.py
+-rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/application-extension/commands.json
+-rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/application-extension/context-menu.json
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/application-extension/package.json.orig
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/application-extension/property-inspector.json
+-rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/application-extension/shell.json
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/application-extension/top-bar.json
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/apputils-extension/notification.json
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/apputils-extension/package.json.orig
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/apputils-extension/palette.json
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/apputils-extension/print.json
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/apputils-extension/sanitizer.json
+-rw-r--r--   0        0        0     3717 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/apputils-extension/themes.json
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/apputils-extension/utilityCommands.json
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/apputils-extension/workspaces.json
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/codemirror-extension/package.json.orig
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/codemirror-extension/plugin.json
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/docmanager-extension/download.json
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/docmanager-extension/package.json.orig
+-rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/docmanager-extension/plugin.json
+-rw-r--r--   0        0        0     6134 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/filebrowser-extension/browser.json
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/filebrowser-extension/download.json
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/filebrowser-extension/open-browser-tab.json
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/filebrowser-extension/open-with.json
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/filebrowser-extension/package.json.orig
+-rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/filebrowser-extension/widget.json
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/launcher-extension/package.json.orig
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/launcher-extension/plugin.json
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/mainmenu-extension/package.json.orig
+-rw-r--r--   0        0        0     9894 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/mainmenu-extension/plugin.json
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/translation-extension/package.json.orig
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/translation-extension/plugin.json
+-rw-r--r--   0        0        0    10149 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/103.app.js
+-rw-r--r--   0        0        0     7215 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/1053.app.js
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/1058.app.js
+-rw-r--r--   0        0        0   302401 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/1072.app.js
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/1072.app.js.LICENSE.txt
+-rw-r--r--   0        0        0   128612 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/1123.app.js
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/1123.app.js.LICENSE.txt
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/1152.app.js
+-rw-r--r--   0        0        0    33344 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/1186.app.js
+-rw-r--r--   0        0        0    14228 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/1208.app.js
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/1210.app.js
+-rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/1222.app.js
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/1227.app.js
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/1278.app.js
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/1286.app.js
+-rw-r--r--   0        0        0     6784 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/13.app.js
+-rw-r--r--   0        0        0    20577 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/1320.app.js
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/1322.app.js
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/1377.app.js
+-rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/1403.app.js
+-rw-r--r--   0        0        0     9838 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/15.app.js
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/151.app.js
+-rw-r--r--   0        0        0   214831 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/1520.app.js
+-rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/1567.app.js
+-rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/1580.app.js
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/1581.app.js
+-rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/1623.app.js
+-rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/1729.app.js
+-rw-r--r--   0        0        0    12512 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/1746.app.js
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/1770.app.js
+-rw-r--r--   0        0        0    60948 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/1880.app.js
+-rw-r--r--   0        0        0     9036 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/1882.app.js
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/1935.app.js
+-rw-r--r--   0        0        0   199427 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/1959.app.js
+-rw-r--r--   0        0        0     8068 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/2033.app.js
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/2042.app.js
+-rw-r--r--   0        0        0    24578 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/2075.app.js
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/2100.app.js
+-rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/2106.app.js
+-rw-r--r--   0        0        0    11835 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/2185.app.js
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/2194.app.js
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/2266.app.js
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/2284.app.js
+-rw-r--r--   0        0        0    14227 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/23.app.js
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/231.app.js
+-rw-r--r--   0        0        0    77242 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/2318.app.js
+-rw-r--r--   0        0        0     9467 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/2488.app.js
+-rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/2502.app.js
+-rw-r--r--   0        0        0    39462 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/2553.app.js
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/2563.app.js
+-rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/2628.app.js
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/2667.app.js
+-rw-r--r--   0        0        0    13343 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/2687.app.js
+-rw-r--r--   0        0        0    25924 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/274.app.js
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/275.app.js
+-rw-r--r--   0        0        0     6617 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/2784.app.js
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/2784.app.js.LICENSE.txt
+-rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/2805.app.js
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/288.app.js
+-rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/2970.app.js
+-rw-r--r--   0        0        0     4978 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/3007.app.js
+-rw-r--r--   0        0        0     9009 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/3093.app.js
+-rw-r--r--   0        0        0     5911 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/3159.app.js
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/3191.app.js
+-rw-r--r--   0        0        0     9662 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/3192.app.js
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/3206.app.js
+-rw-r--r--   0        0        0    16702 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/3211.app.js
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/3265.app.js
+-rw-r--r--   0        0        0   432933 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/330.app.js
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/3312.app.js
+-rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/3316.app.js
+-rw-r--r--   0        0        0    14228 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/3324.app.js
+-rw-r--r--   0        0        0   171985 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/3326.app.js
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/3330.app.js
+-rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/3397.app.js
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/3466.app.js
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/3499.app.js
+-rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/3500.app.js
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/351.app.js
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/3540.app.js
+-rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/3542.app.js
+-rw-r--r--   0        0        0   169327 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/358.app.js
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/360.app.js
+-rw-r--r--   0        0        0  1020115 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/3656.app.js
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/3656.app.js.LICENSE.txt
+-rw-r--r--   0        0        0     6711 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/370.app.js
+-rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/3726.app.js
+-rw-r--r--   0        0        0   203030 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/373c04fd2418f5c77eea.eot
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/3811.app.js
+-rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/3851.app.js
+-rw-r--r--   0        0        0    61590 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/3855.app.js
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/386.app.js
+-rw-r--r--   0        0        0    46084 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/3872.app.js
+-rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/3880.app.js
+-rw-r--r--   0        0        0   101648 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/3f6d3488cf65374f6f67.woff
+-rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/4024.app.js
+-rw-r--r--   0        0        0     5267 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/4040.app.js
+-rw-r--r--   0        0        0     9009 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/4059.app.js
+-rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/4065.app.js
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/4073.app.js
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/4123.app.js
+-rw-r--r--   0        0        0    52558 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/4171.app.js
+-rw-r--r--   0        0        0     6636 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/4282.app.js
+-rw-r--r--   0        0        0    10948 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/4283.app.js
+-rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/4299.app.js
+-rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/4351.app.js
+-rw-r--r--   0        0        0    16452 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/4359.app.js
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/4391.app.js
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/4403.app.js
+-rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/4462.app.js
+-rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/4476.app.js
+-rw-r--r--   0        0        0   143645 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/450.app.js
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/4608.app.js
+-rw-r--r--   0        0        0    18653 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/4651.app.js
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/4651.app.js.LICENSE.txt
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/4654.app.js
+-rw-r--r--   0        0        0    23079 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/4679.app.js
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/4702.app.js
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/4718.app.js
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/4808.app.js
+-rw-r--r--   0        0        0    15011 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/484.app.js
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/4874.app.js
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/4878.app.js
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/4935.app.js
+-rw-r--r--   0        0        0    27298 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/4965.app.js
+-rw-r--r--   0        0        0    69298 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/4973.app.js
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/4973.app.js.LICENSE.txt
+-rw-r--r--   0        0        0    22107 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/4982.app.js
+-rw-r--r--   0        0        0    62789 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/5002.app.js
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/5024.app.js
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/504.app.js
+-rw-r--r--   0        0        0     6711 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/5064.app.js
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/5101.app.js
+-rw-r--r--   0        0        0    94906 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/5148.app.js
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/5172.app.js
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/5176.app.js
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/5223.app.js
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/5225.app.js
+-rw-r--r--   0        0        0    86931 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/5231.app.js
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/5263.app.js
+-rw-r--r--   0        0        0   101929 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/5340.app.js
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/5393.app.js
+-rw-r--r--   0        0        0   180936 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/5430.app.js
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/5433.app.js
+-rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/5445.app.js
+-rw-r--r--   0        0        0    24464 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/550.app.js
+-rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/5513.app.js
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/5514.app.js
+-rw-r--r--   0        0        0    18861 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/5544.app.js
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/5556.app.js
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/558.app.js
+-rw-r--r--   0        0        0    10154 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/5587.app.js
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/5681.app.js
+-rw-r--r--   0        0        0    68549 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/5708.app.js
+-rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/5764.app.js
+-rw-r--r--   0        0        0     6452 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/5811.app.js
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/5817.app.js
+-rw-r--r--   0        0        0     5242 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/5876.app.js
+-rw-r--r--   0        0        0     7078 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/5882.app.js
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/5882.app.js.LICENSE.txt
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/6146.app.js
+-rw-r--r--   0        0        0     4683 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/6151.app.js
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/6186.app.js
+-rw-r--r--   0        0        0    10302 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/6196.app.js
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/6410.app.js
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/6483.app.js
+-rw-r--r--   0        0        0    30696 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/6510.app.js
+-rw-r--r--   0        0        0    37190 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/6645.app.js
+-rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/6686.app.js
+-rw-r--r--   0        0        0     9416 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/6770.app.js
+-rw-r--r--   0        0        0    49485 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/6778.app.js
+-rw-r--r--   0        0        0    12106 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/6782.app.js
+-rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/6808.app.js
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/6833.app.js
+-rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/6835.app.js
+-rw-r--r--   0        0        0    99172 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/6914.app.js
+-rw-r--r--   0        0        0     7871 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/6970.app.js
+-rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/7058.app.js
+-rw-r--r--   0        0        0    65804 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/7102.app.js
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/7111.app.js
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/7127.app.js
+-rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/7149.app.js
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/7174.app.js
+-rw-r--r--   0        0        0    27083 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/7233.app.js
+-rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/7236.app.js
+-rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/7294.app.js
+-rw-r--r--   0        0        0    11619 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/730.app.js
+-rw-r--r--   0        0        0     4177 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/7377.app.js
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/7379.app.js
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/7424.app.js
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/7469.app.js
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/7498.app.js
+-rw-r--r--   0        0        0    33625 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/7526.app.js
+-rw-r--r--   0        0        0    40106 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/7529.app.js
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/7600.app.js
+-rw-r--r--   0        0        0     6490 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/765.app.js
+-rw-r--r--   0        0        0    22254 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/7664.app.js
+-rw-r--r--   0        0        0    65777 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/769.app.js
+-rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/7710.app.js
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/7806.app.js
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/7860.app.js
+-rw-r--r--   0        0        0     7432 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/7882.app.js
+-rw-r--r--   0        0        0    17079 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/7884.app.js
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/7955.app.js
+-rw-r--r--   0        0        0   103425 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/7991.app.js
+-rw-r--r--   0        0        0    34034 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/79d088064beb3826054f.eot
+-rw-r--r--   0        0        0   199428 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/8078.app.js
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/8090.app.js
+-rw-r--r--   0        0        0   113878 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/8100.app.js
+-rw-r--r--   0        0        0    47563 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/8124.app.js
+-rw-r--r--   0        0        0    54614 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/8138.app.js
+-rw-r--r--   0        0        0     8337 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/819.app.js
+-rw-r--r--   0        0        0     6571 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/8307.app.js
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/8342.app.js
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/8409.app.js
+-rw-r--r--   0        0        0    25262 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/8423.app.js
+-rw-r--r--   0        0        0    25112 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/8441.app.js
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/8442.app.js
+-rw-r--r--   0        0        0     6447 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/846.app.js
+-rw-r--r--   0        0        0    66111 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/8466.app.js
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/8496.app.js
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/8518.app.js
+-rw-r--r--   0        0        0    17922 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/8561.app.js
+-rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/8576.app.js
+-rw-r--r--   0        0        0    14229 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/8615.app.js
+-rw-r--r--   0        0        0    40918 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/8640.app.js
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/8658.app.js
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/8662.app.js
+-rw-r--r--   0        0        0    10154 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/8728.app.js
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/8763.app.js
+-rw-r--r--   0        0        0    39773 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/8769.app.js
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/8782.app.js
+-rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/8803.app.js
+-rw-r--r--   0        0        0   292717 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/882.app.js
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/8866.app.js
+-rw-r--r--   0        0        0     4537 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/8877.app.js
+-rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/8914.app.js
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/8953.app.js
+-rw-r--r--   0        0        0    76736 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/8ea8791754915a898a31.woff2
+-rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/9036.app.js
+-rw-r--r--   0        0        0     7780 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/9060.app.js
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/9117.app.js
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/9172.app.js
+-rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/9304.app.js
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/9308.app.js
+-rw-r--r--   0        0        0     6452 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/9318.app.js
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/9319.app.js
+-rw-r--r--   0        0        0     8950 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/9339.app.js
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/9369.app.js
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/9397.app.js
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/9406.app.js
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/9411.app.js
+-rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/9472.app.js
+-rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/9473.app.js
+-rw-r--r--   0        0        0   253965 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/9491.app.js
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/9491.app.js.LICENSE.txt
+-rw-r--r--   0        0        0     6712 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/9513.app.js
+-rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/9583.app.js
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/9631.app.js
+-rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/9636.app.js
+-rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/9672.app.js
+-rw-r--r--   0        0        0   918991 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/9674eb1bd55047179038.svg
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/9715.app.js
+-rw-r--r--   0        0        0    16181 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/9787.app.js
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/9787.app.js.LICENSE.txt
+-rw-r--r--   0        0        0    10153 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/9811.app.js
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/9822.app.js
+-rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/9827.app.js
+-rw-r--r--   0        0        0    78268 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/9834b82ad26e2a37583d.woff2
+-rw-r--r--   0        0        0     9146 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/9866.app.js
+-rw-r--r--   0        0        0    59178 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/9877.app.js
+-rw-r--r--   0        0        0   138733 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/9908.app.js
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/9908.app.js.LICENSE.txt
+-rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/9932.app.js
+-rw-r--r--   0        0        0    22523 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/9961.app.js
+-rw-r--r--   0        0        0   569513 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/9976.app.js
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/9976.app.js.LICENSE.txt
+-rw-r--r--   0        0        0   747927 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/a3b9817780214caf01e8.svg
+-rw-r--r--   0        0        0   202744 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/af6397503fcefbd61397.ttf
+-rw-r--r--   0        0        0    33575 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/app.js
+-rw-r--r--   0        0        0   144714 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/be0a084962d8066884f7.svg
+-rw-r--r--   0        0        0    16276 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/cb9e9e693192413cde2b.woff
+-rw-r--r--   0        0        0   133988 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/cda59d6efffa685830fd.ttf
+-rw-r--r--   0        0        0   134294 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/e4299464e7b012968eed.eot
+-rw-r--r--   0        0        0    13224 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/e42a88444448ac3d6054.woff2
+-rw-r--r--   0        0        0    33736 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/e8711bbb871afd8e9dea.ttf
+-rw-r--r--   0        0        0    89988 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/static/f9217f66874b0c01cd8c.woff
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/templates/index.html
+-rw-r--r--   0        0        0    17760 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/themes/@jupyterlab/theme-dark-extension/index.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/themes/@jupyterlab/theme-dark-extension/index.js
+-rw-r--r--   0        0        0    16493 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/themes/@jupyterlab/theme-light-extension/index.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/cadapp/themes/@jupyterlab/theme-light-extension/index.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/freecad/__init__.py
+-rw-r--r--   0        0        0     6406 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/freecad/loader.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/freecad/props/__init__.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/freecad/props/base_prop.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/freecad/props/property_angle.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/freecad/props/property_bool.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/freecad/props/property_distance.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/freecad/props/property_geometrylist.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/freecad/props/property_length.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/freecad/props/property_link.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/freecad/props/property_link_list.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/freecad/props/property_map.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/freecad/props/property_partshape.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/freecad/props/property_placement.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/freecad/props/geometry/__init__.py
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/freecad/props/geometry/geom_circle.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/freecad/props/geometry/geom_linesegment.py
+-rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/labextension/package.json
+-rw-r--r--   0        0        0    52115 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/labextension/static/184.6f76dd957e411be19baa.js
+-rw-r--r--   0        0        0    86711 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/labextension/static/213.778b3209dbe7ec5470b6.js
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/labextension/static/268.16c8a4126908b03651f0.js
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/labextension/static/288.11fba3e29cc454c9c071.js
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/labextension/static/358.45fb46ea24bb44ba7fa9.js
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/labextension/static/379.5df518c877987fc7ca0c.js
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/labextension/static/406.5ed89c99d9b3043c85c0.js
+-rw-r--r--   0        0        0    59793 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/labextension/static/422.39a95e19d3a414516796.js
+-rw-r--r--   0        0        0    10419 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/labextension/static/52.477d969cb88d8007c4f0.js
+-rw-r--r--   0        0        0   124222 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/labextension/static/544.04fb377af8d9c7574a58.js
+-rw-r--r--   0        0        0     8094 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/labextension/static/643.850e055919134443b4fa.js
+-rw-r--r--   0        0        0    18686 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/labextension/static/651.3736a4bd9cf2725cc067.js
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/labextension/static/651.3736a4bd9cf2725cc067.js.LICENSE.txt
+-rw-r--r--   0        0        0    12432 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/labextension/static/711.9ae86a9a4b0e0a748ae7.js
+-rw-r--r--   0        0        0     8086 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/labextension/static/712.3d4b32523dbb4dff584d.js
+-rw-r--r--   0        0        0   183517 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/labextension/static/730.5a8c1aad713514a0a596.js
+-rw-r--r--   0        0        0   116747 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/labextension/static/733.89a6a4e0561966230286.js
+-rw-r--r--   0        0        0    31683 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/labextension/static/761.1bd8bdc8d51f62af816d.js
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/labextension/static/761.1bd8bdc8d51f62af816d.js.LICENSE.txt
+-rw-r--r--   0        0        0     8567 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/labextension/static/78.8e87e13a67c31f2732c7.js
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/labextension/static/811.d1c8b6a87faba2d069bd.js
+-rw-r--r--   0        0        0     6111 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/labextension/static/816.00326e9e5f2436d0d67f.js
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/labextension/static/833.253bc84b61cd4e2beb80.js
+-rw-r--r--   0        0        0   254953 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/labextension/static/842.116bb3340768f53ea709.js
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/labextension/static/842.116bb3340768f53ea709.js.LICENSE.txt
+-rw-r--r--   0        0        0    13339 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/labextension/static/847.6efcc69e25d704ee7090.js
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/labextension/static/860.9dcab30c320fd0b9cfe1.js
+-rw-r--r--   0        0        0   623572 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/labextension/static/955.a084e75defa008fca238.js
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/labextension/static/955.a084e75defa008fca238.js.LICENSE.txt
+-rw-r--r--   0        0        0   114029 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/labextension/static/963.ba192cdc34bc5ccdfe40.js
+-rw-r--r--   0        0        0  5065593 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/labextension/static/jupytercad.opencascade.wasm
+-rw-r--r--   0        0        0    13025 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/labextension/static/remoteEntry.190fffa25e51baa1896b.js
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/labextension/static/style.js
+-rw-r--r--   0        0        0    67986 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/notebook/__init__.py
+-rw-r--r--   0        0        0    22888 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/notebook/cad_document.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/notebook/utils.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/notebook/y_connector.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/notebook/objects/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/notebook/objects/_schema/__init__.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/notebook/objects/_schema/box.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/notebook/objects/_schema/cone.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/notebook/objects/_schema/cut.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/notebook/objects/_schema/cylinder.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/notebook/objects/_schema/extrusion.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/notebook/objects/_schema/fuse.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/notebook/objects/_schema/geomCircle.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/notebook/objects/_schema/geomLineSegment.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/notebook/objects/_schema/intersection.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/notebook/objects/_schema/jcad.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/notebook/objects/_schema/placement.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/notebook/objects/_schema/sketch.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/notebook/objects/_schema/sphere.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 jupytercad-0.2.3/jupytercad/notebook/objects/_schema/torus.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 jupytercad-0.2.3/scripts/bump-version.py
+-rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/package.json
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/tsconfig.json
+-rw-r--r--   0        0        0   132758 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/tsconfig.tsbuildinfo
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/webpack.config.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/build/bootstrap.d.ts
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/build/bootstrap.js
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/build/main.d.ts
+-rw-r--r--   0        0        0     6407 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/build/main.js
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/build/sharedscope.d.ts
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/build/sharedscope.js
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/build/style.js
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/build/app/app.d.ts
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/build/app/app.js
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/build/app/shell.d.ts
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/build/app/shell.js
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/build/app/plugins/browser/index.d.ts
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/build/app/plugins/browser/index.js
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/build/app/plugins/launcher/index.d.ts
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/build/app/plugins/launcher/index.js
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/build/app/plugins/mainmenu/index.d.ts
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/build/app/plugins/mainmenu/index.js
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/build/app/plugins/mainmenu/menuWidget.d.ts
+-rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/build/app/plugins/mainmenu/menuWidget.js
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/build/app/plugins/mainmenu/titleWidget.d.ts
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/build/app/plugins/mainmenu/titleWidget.js
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/build/app/plugins/mainmenu/userWidget.d.ts
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/build/app/plugins/mainmenu/userWidget.js
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/build/app/plugins/paths/index.d.ts
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/build/app/plugins/paths/index.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/lib/bootstrap.d.ts
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/lib/bootstrap.js
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/lib/main.d.ts
+-rw-r--r--   0        0        0     6407 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/lib/main.js
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/lib/sharedscope.d.ts
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/lib/sharedscope.js
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/lib/app/app.d.ts
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/lib/app/app.js
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/lib/app/shell.d.ts
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/lib/app/shell.js
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/lib/app/plugins/browser/index.d.ts
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/lib/app/plugins/browser/index.js
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/lib/app/plugins/launcher/index.d.ts
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/lib/app/plugins/launcher/index.js
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/lib/app/plugins/mainmenu/index.d.ts
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/lib/app/plugins/mainmenu/index.js
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/lib/app/plugins/mainmenu/menuWidget.d.ts
+-rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/lib/app/plugins/mainmenu/menuWidget.js
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/lib/app/plugins/mainmenu/titleWidget.d.ts
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/lib/app/plugins/mainmenu/titleWidget.js
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/lib/app/plugins/mainmenu/userWidget.d.ts
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/lib/app/plugins/mainmenu/userWidget.js
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/lib/app/plugins/paths/index.d.ts
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/lib/app/plugins/paths/index.js
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/src/bootstrap.ts
+-rw-r--r--   0        0        0     6198 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/src/main.ts
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/src/sharedscope.ts
+-rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/src/app/app.ts
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/src/app/shell.ts
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/src/app/plugins/browser/index.ts
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/src/app/plugins/launcher/index.ts
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/src/app/plugins/mainmenu/index.ts
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/src/app/plugins/mainmenu/menuWidget.ts
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/src/app/plugins/mainmenu/titleWidget.tsx
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/src/app/plugins/mainmenu/userWidget.tsx
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/src/app/plugins/paths/index.ts
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-app/style/index.js
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/extension.webpack.config.js
+-rw-r--r--   0        0        0     4637 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/package.json
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/schema.js
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/tsconfig.json
+-rw-r--r--   0        0        0   189578 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/tsconfig.tsbuildinfo
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/tsconfig.worker.json
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/worker.webpack.config.js
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/commands.d.ts
+-rw-r--r--   0        0        0    23175 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/commands.js
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/factory.d.ts
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/factory.js
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/formdialog.d.ts
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/formdialog.js
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/index.d.ts
+-rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/index.js
+-rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/mainview.d.ts
+-rw-r--r--   0        0        0    37791 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/mainview.js
+-rw-r--r--   0        0        0     4466 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/model.d.ts
+-rw-r--r--   0        0        0    10228 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/model.js
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/token.d.ts
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/token.js
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/tools.d.ts
+-rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/tools.js
+-rw-r--r--   0        0        0     6742 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/types.d.ts
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/types.js
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/widget.d.ts
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/widget.js
+-rw-r--r--   0        0        0    86564 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/worker.js
+-rw-r--r--   0        0        0    26960 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/_interface/forms.json
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/annotation/message.d.ts
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/annotation/message.js
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/annotation/model.d.ts
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/annotation/model.js
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/annotation/view.d.ts
+-rw-r--r--   0        0        0     4537 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/annotation/view.js
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/fcplugin/modelfactory.d.ts
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/fcplugin/modelfactory.js
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/fcplugin/plugins.d.ts
+-rw-r--r--   0        0        0     4817 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/fcplugin/plugins.js
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/jcadplugin/modelfactory.d.ts
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/jcadplugin/modelfactory.js
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/jcadplugin/plugins.d.ts
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/jcadplugin/plugins.js
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/notebookrenderer/index.d.ts
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/notebookrenderer/index.js
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/notebookrenderer/model.d.ts
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/notebookrenderer/model.js
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/notebookrenderer/token.d.ts
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/notebookrenderer/token.js
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/notebookrenderer/view.d.ts
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/notebookrenderer/view.js
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/notebookrenderer/widgetManager.d.ts
+-rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/notebookrenderer/widgetManager.js
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/notebookrenderer/yCommProvider.d.ts
+-rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/notebookrenderer/yCommProvider.js
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/panelview/annotations.d.ts
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/panelview/annotations.js
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/panelview/formbuilder.d.ts
+-rw-r--r--   0        0        0     6348 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/panelview/formbuilder.js
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/panelview/header.d.ts
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/panelview/header.js
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/panelview/leftpanel.d.ts
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/panelview/leftpanel.js
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/panelview/model.d.ts
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/panelview/model.js
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/panelview/objectproperties.d.ts
+-rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/panelview/objectproperties.js
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/panelview/objecttree.d.ts
+-rw-r--r--   0        0        0    12942 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/panelview/objecttree.js
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/panelview/rightpanel.d.ts
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/panelview/rightpanel.js
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/schema/box.json
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/schema/cone.json
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/schema/cut.json
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/schema/cylinder.json
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/schema/extrusion.json
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/schema/fuse.json
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/schema/geomCircle.json
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/schema/geomLineSegment.json
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/schema/intersection.json
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/schema/jcad.json
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/schema/placement.json
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/schema/sketch.json
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/schema/sphere.json
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/schema/torus.json
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/sketcher/helper.d.ts
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/sketcher/helper.js
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/sketcher/panzoom.d.ts
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/sketcher/panzoom.js
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/sketcher/sketcherdialog.d.ts
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/sketcher/sketcherdialog.js
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/sketcher/sketchermodel.d.ts
+-rw-r--r--   0        0        0     6417 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/sketcher/sketchermodel.js
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/sketcher/sketcherwidget.d.ts
+-rw-r--r--   0        0        0    19357 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/sketcher/sketcherwidget.js
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/sketcher/types.d.ts
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/sketcher/types.js
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/sketcher/elements/circle.d.ts
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/sketcher/elements/circle.js
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/sketcher/elements/line.d.ts
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/sketcher/elements/line.js
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/sketcher/elements/point.d.ts
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/sketcher/elements/point.js
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/toolbar/usertoolbaritem.d.ts
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/toolbar/usertoolbaritem.js
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/toolbar/widget.d.ts
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/toolbar/widget.js
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/worker/actions.d.ts
+-rw-r--r--   0        0        0     6797 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/worker/actions.js
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/worker/occapi.d.ts
+-rw-r--r--   0        0        0     8828 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/worker/occapi.js
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/worker/occparser.d.ts
+-rw-r--r--   0        0        0     8462 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/worker/occparser.js
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/worker/operatorcache.d.ts
+-rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/worker/operatorcache.js
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/worker/types.d.ts
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/worker/types.js
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/worker/utils.d.ts
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/worker/utils.js
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/worker/worker.d.ts
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/worker/worker.js
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/worker/geometry/geomCircle.d.ts
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/worker/geometry/geomCircle.js
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/worker/geometry/geomLineSegment.d.ts
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/lib/worker/geometry/geomLineSegment.js
+-rw-r--r--   0        0        0    19412 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/commands.ts
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/factory.ts
+-rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/formdialog.tsx
+-rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/index.ts
+-rw-r--r--   0        0        0    34821 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/mainview.tsx
+-rw-r--r--   0        0        0    11815 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/model.ts
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/svg.d.ts
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/token.ts
+-rw-r--r--   0        0        0     6187 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/tools.ts
+-rw-r--r--   0        0        0     6416 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/types.ts
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/widget.tsx
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/_interface/box.d.ts
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/_interface/cone.d.ts
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/_interface/cut.d.ts
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/_interface/cylinder.d.ts
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/_interface/extrusion.d.ts
+-rw-r--r--   0        0        0    19613 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/_interface/forms.json
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/_interface/fuse.d.ts
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/_interface/geomCircle.d.ts
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/_interface/geomLineSegment.d.ts
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/_interface/intersection.d.ts
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/_interface/jcad.d.ts
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/_interface/placement.d.ts
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/_interface/sketch.d.ts
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/_interface/sphere.d.ts
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/_interface/torus.d.ts
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/annotation/message.tsx
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/annotation/model.ts
+-rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/annotation/view.tsx
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/fcplugin/modelfactory.ts
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/fcplugin/plugins.ts
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/jcadplugin/modelfactory.ts
+-rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/jcadplugin/plugins.ts
+-rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/notebookrenderer/index.ts
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/notebookrenderer/model.ts
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/notebookrenderer/token.ts
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/notebookrenderer/view.ts
+-rw-r--r--   0        0        0     3587 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/notebookrenderer/widgetManager.ts
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/notebookrenderer/yCommProvider.ts
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/panelview/annotations.tsx
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/panelview/formbuilder.tsx
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/panelview/header.tsx
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/panelview/leftpanel.tsx
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/panelview/model.ts
+-rw-r--r--   0        0        0     7437 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/panelview/objectproperties.tsx
+-rw-r--r--   0        0        0    12066 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/panelview/objecttree.tsx
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/panelview/rightpanel.tsx
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/schema/box.json
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/schema/cone.json
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/schema/cut.json
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/schema/cylinder.json
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/schema/extrusion.json
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/schema/fuse.json
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/schema/geomCircle.json
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/schema/geomLineSegment.json
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/schema/intersection.json
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/schema/jcad.json
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/schema/placement.json
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/schema/sketch.json
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/schema/sphere.json
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/schema/torus.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/sketcher/helper.tsx
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/sketcher/panzoom.ts
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/sketcher/sketcherdialog.tsx
+-rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/sketcher/sketchermodel.ts
+-rw-r--r--   0        0        0    16285 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/sketcher/sketcherwidget.tsx
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/sketcher/types.ts
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/sketcher/elements/circle.ts
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/sketcher/elements/line.ts
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/sketcher/elements/point.ts
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/toolbar/usertoolbaritem.tsx
+-rw-r--r--   0        0        0     4157 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/toolbar/widget.tsx
+-rw-r--r--   0        0        0     6891 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/worker/actions.ts
+-rw-r--r--   0        0        0    10134 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/worker/occapi.ts
+-rw-r--r--   0        0        0     8609 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/worker/occparser.ts
+-rw-r--r--   0        0        0     3587 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/worker/operatorcache.ts
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/worker/types.ts
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/worker/utils.ts
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/worker/worker.ts
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/worker/geometry/geomCircle.ts
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/src/worker/geometry/geomLineSegment.ts
+-rw-r--r--   0        0        0     7174 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/style/index.js
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/style/icon/axes.svg
+-rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/style/icon/box.svg
+-rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/style/icon/cone.svg
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/style/icon/cut.svg
+-rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/style/icon/cylinder.svg
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/style/icon/extrusion.svg
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/style/icon/intersection.svg
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/style/icon/jvcontrol.svg
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/style/icon/minimize.svg
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/style/icon/sphere.svg
+-rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/style/icon/torus.svg
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/style/icon/union.svg
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/style/icon/visibility.svg
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-extension/style/icon/visibilityOff.svg
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-opencascade/build.yml
+-rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-opencascade/build_opencascade.js
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-opencascade/package.json
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-opencascade/lib/build.yml
+-rw-r--r--   0        0        0   129654 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-opencascade/lib/jupytercad.opencascade.d.ts
+-rw-r--r--   0        0        0   123823 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-opencascade/lib/jupytercad.opencascade.js
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-opencascade/lib/jupytercad.opencascade.version
+-rwxr-xr-x   0        0        0  5065593 2020-02-02 00:00:00.000000 jupytercad-0.2.3/packages/jupytercad-opencascade/lib/jupytercad.opencascade.wasm
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 jupytercad-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 jupytercad-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 jupytercad-0.2.3/README.md
+-rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 jupytercad-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 jupytercad-0.2.3/PKG-INFO
```

### Comparing `jupytercad-0.2.2/.eslintrc.js` & `jupytercad-0.2.3/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/.pre-commit-config.yaml` & `jupytercad-0.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/CHANGELOG.md` & `jupytercad-0.2.3/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,41 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.2.3
+
+([Full Changelog](https://github.com/QuantStack/jupytercad/compare/@jupytercad/jupytercad-app@0.2.2...a85d44387dbfefd8cd0a068d1d749a676cf5a82b))
+
+### Bugs fixed
+
+- Missing dependencies [#184](https://github.com/QuantStack/jupytercad/pull/184) ([@martinRenou](https://github.com/martinRenou))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/QuantStack/jupytercad/graphs/contributors?from=2023-06-03&to=2023-06-05&type=c))
+
+[@martinRenou](https://github.com/search?q=repo%3AQuantStack%2Fjupytercad+involves%3AmartinRenou+updated%3A2023-06-03..2023-06-05&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 0.2.2
 
 ([Full Changelog](https://github.com/QuantStack/jupytercad/compare/v0.2.1...d2d79078ab974673b6fcadd4e5ef8f16abf5022a))
 
 ### Bugs fixed
 
 - Update shared scope [#182](https://github.com/QuantStack/jupytercad/pull/182) ([@trungleduc](https://github.com/trungleduc))
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/QuantStack/jupytercad/graphs/contributors?from=2023-06-03&to=2023-06-03&type=c))
 
 [@trungleduc](https://github.com/search?q=repo%3AQuantStack%2Fjupytercad+involves%3Atrungleduc+updated%3A2023-06-03..2023-06-03&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.2.1
 
 ([Full Changelog](https://github.com/QuantStack/jupytercad/compare/v0.2.0...ec0b05cb38d16a1a8fc0a853a53328c4a05542dd))
 
 ### Bugs fixed
 
 - Fix missing static files in cad app [#181](https://github.com/QuantStack/jupytercad/pull/181) ([@trungleduc](https://github.com/trungleduc))
```

### Comparing `jupytercad-0.2.2/CONTRIBUTING.md` & `jupytercad-0.2.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/RELEASE.md` & `jupytercad-0.2.3/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad-screenshot.png` & `jupytercad-0.2.3/jupytercad-screenshot.png`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/package.json` & `jupytercad-0.2.3/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9642857142857143%*

 * *Differences: {"'version'": "'0.2.3'"}*

```diff
@@ -50,12 +50,12 @@
         "eslint:check": "eslint . --ext .ts,.tsx",
         "lint": "jlpm run prettier && jlpm run eslint",
         "lint:check": "jlpm run prettier:check && jlpm run eslint:check",
         "prettier": "prettier --write \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "prettier:check": "prettier --list-different \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "test": "lerna run test"
     },
-    "version": "0.2.2",
+    "version": "0.2.3",
     "workspaces": [
         "packages/*"
     ]
 }
```

### Comparing `jupytercad-0.2.2/tsconfigbase.json` & `jupytercad-0.2.3/tsconfigbase.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/yarn.lock` & `jupytercad-0.2.3/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -818,15 +818,15 @@
   resolution: "@jupytercad/jupytercad-app@workspace:packages/jupytercad-app"
   dependencies:
     "@codemirror/state": ^6.2.0
     "@codemirror/view": ^6.9.3
     "@jupyter/collaboration": ^1.0.0
     "@jupyter/docprovider": ^1.0.0
     "@jupyter/ydoc": ^0.3.4 || ^1.0.2
-    "@jupytercad/jupytercad-extension": ^0.2.2
+    "@jupytercad/jupytercad-extension": ^0.2.3
     "@jupyterlab/application": ^4.0.0
     "@jupyterlab/application-extension": ^4.0.0
     "@jupyterlab/apputils": ^4.0.0
     "@jupyterlab/apputils-extension": ^4.0.0
     "@jupyterlab/builder": ^4.0.0
     "@jupyterlab/codemirror": ^4.0.0
     "@jupyterlab/codemirror-extension": ^4.0.0
@@ -868,24 +868,24 @@
     tsc-watch: ^6.0.0
     typescript: ^5
     webpack: ^5.76.3
     yjs: ^13.5.40
   languageName: unknown
   linkType: soft
 
-"@jupytercad/jupytercad-extension@^0.2.2, @jupytercad/jupytercad-extension@workspace:packages/jupytercad-extension":
+"@jupytercad/jupytercad-extension@^0.2.3, @jupytercad/jupytercad-extension@workspace:packages/jupytercad-extension":
   version: 0.0.0-use.local
   resolution: "@jupytercad/jupytercad-extension@workspace:packages/jupytercad-extension"
   dependencies:
     "@apidevtools/json-schema-ref-parser": ^9.0.9
     "@deathbeds/jupyterlab-rjsf": ^1.1.0
     "@jupyter/collaboration": ^1.0.0
     "@jupyter/docprovider": ^1.0.0
     "@jupyter/ydoc": ^0.3.4 || ^1.0.2
-    "@jupytercad/jupytercad-opencascade": ^0.2.2
+    "@jupytercad/jupytercad-opencascade": ^0.2.3
     "@jupyterlab/application": ^4.0.0
     "@jupyterlab/apputils": ^4.0.0
     "@jupyterlab/builder": ^4.0.0
     "@jupyterlab/coreutils": ^6.0.0
     "@jupyterlab/docregistry": ^4.0.0
     "@jupyterlab/filebrowser": ^4.0.0
     "@jupyterlab/launcher": ^4.0.0
@@ -918,15 +918,15 @@
     ts-loader: ^9.2.6
     typescript: ^5
     uuid: ^8.3.2
     webpack: ^5.76.3
   languageName: unknown
   linkType: soft
 
-"@jupytercad/jupytercad-opencascade@^0.2.2, @jupytercad/jupytercad-opencascade@workspace:packages/jupytercad-opencascade":
+"@jupytercad/jupytercad-opencascade@^0.2.3, @jupytercad/jupytercad-opencascade@workspace:packages/jupytercad-opencascade":
   version: 0.0.0-use.local
   resolution: "@jupytercad/jupytercad-opencascade@workspace:packages/jupytercad-opencascade"
   dependencies:
     js-yaml: ^4.1.0
     rimraf: ^3.0.2
   languageName: unknown
   linkType: soft
```

### Comparing `jupytercad-0.2.2/jupytercad/fcstd_ydoc.py` & `jupytercad-0.2.3/jupytercad/fcstd_ydoc.py`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/jcad_ydoc.py` & `jupytercad-0.2.3/jupytercad/jcad_ydoc.py`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/cadapp.py` & `jupytercad-0.2.3/jupytercad/cadapp/cadapp.py`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/utils.py` & `jupytercad-0.2.3/jupytercad/cadapp/utils.py`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/application-extension/commands.json` & `jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/application-extension/commands.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/application-extension/context-menu.json` & `jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/application-extension/context-menu.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/application-extension/package.json.orig` & `jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/application-extension/package.json.orig`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/application-extension/property-inspector.json` & `jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/application-extension/property-inspector.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/application-extension/shell.json` & `jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/application-extension/shell.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/application-extension/top-bar.json` & `jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/application-extension/top-bar.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/apputils-extension/notification.json` & `jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/apputils-extension/notification.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/apputils-extension/package.json.orig` & `jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/apputils-extension/package.json.orig`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/apputils-extension/palette.json` & `jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/apputils-extension/palette.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/apputils-extension/print.json` & `jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/apputils-extension/print.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/apputils-extension/sanitizer.json` & `jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/apputils-extension/sanitizer.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/apputils-extension/themes.json` & `jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/apputils-extension/themes.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/apputils-extension/utilityCommands.json` & `jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/apputils-extension/utilityCommands.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/codemirror-extension/package.json.orig` & `jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/codemirror-extension/package.json.orig`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/docmanager-extension/package.json.orig` & `jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/docmanager-extension/package.json.orig`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/docmanager-extension/plugin.json` & `jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/docmanager-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/filebrowser-extension/browser.json` & `jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/filebrowser-extension/browser.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/filebrowser-extension/download.json` & `jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/filebrowser-extension/download.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/filebrowser-extension/package.json.orig` & `jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/filebrowser-extension/package.json.orig`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/filebrowser-extension/widget.json` & `jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/filebrowser-extension/widget.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/launcher-extension/package.json.orig` & `jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/launcher-extension/package.json.orig`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/launcher-extension/plugin.json` & `jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/launcher-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/mainmenu-extension/package.json.orig` & `jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/mainmenu-extension/package.json.orig`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/mainmenu-extension/plugin.json` & `jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/mainmenu-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/translation-extension/package.json.orig` & `jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/translation-extension/package.json.orig`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/schemas/@jupyterlab/translation-extension/plugin.json` & `jupytercad-0.2.3/jupytercad/cadapp/schemas/@jupyterlab/translation-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/103.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/103.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/1053.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/1053.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/1058.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/1058.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/1072.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/1072.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/1123.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/1123.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/1123.app.js.LICENSE.txt` & `jupytercad-0.2.3/jupytercad/cadapp/static/1123.app.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/1152.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/1152.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/1186.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/1186.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/1208.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/1208.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/1210.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/1210.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/1222.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/1222.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/1227.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/1227.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/1278.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/1278.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/1286.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/1286.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/13.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/13.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/1320.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/1320.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/1322.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/1322.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/1377.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/1377.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/1403.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/1403.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/15.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/15.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/151.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/151.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/1520.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/1520.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/1567.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/1567.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/1580.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/1580.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/1581.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/1581.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/1623.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/1623.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/1729.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/1729.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/1746.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/1746.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/1770.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/1770.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/1880.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/1880.app.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -373,15 +373,15 @@
                     })), super({
                         title: e.title,
                         body: o,
                         buttons: [s.Dialog.cancelButton()]
                     }), this.addClass("jpcad-property-FormDialog")
                 }
             }
-            const b = JSON.parse('{"Part::GeomCircle":{"type":"object","required":["TypeId","CenterX","CenterY","CenterZ","NormalX","NormalY","NormalZ","AngleXU","Radius"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomCircle","description":"Geometry type"},"CenterX":{"type":"number","description":"CenterX"},"CenterY":{"type":"number","description":"CenterY"},"CenterZ":{"type":"number","description":"CenterZ"},"NormalX":{"type":"number","description":"NormalX"},"NormalY":{"type":"number","description":"NormalY"},"NormalZ":{"type":"number","description":"NormalZ"},"AngleXU":{"type":"number","description":"AngleXU"},"Radius":{"type":"number","description":"Radius"}}},"Part::GeomLineSegment":{"type":"object","required":["TypeId","StartX","StartY","StartZ","EndX","EndY","EndZ"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomLineSegment","description":"Geometry type"},"StartX":{"type":"number","description":"StartX"},"StartY":{"type":"number","description":"StartY"},"StartZ":{"type":"number","description":"StartZ"},"EndX":{"type":"number","description":"EndX"},"EndY":{"type":"number","description":"EndY"},"EndZ":{"type":"number","description":"EndZ"}}},"Placement of the box":{"type":"object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}},"Part::Box":{"type":"object","required":["Length","Width","Height","Placement"],"additionalProperties":false,"properties":{"Length":{"type":"number","description":"The length of the box"},"Width":{"type":"number","description":"The width of the box"},"Height":{"type":"number","description":"The height of the box"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Cone":{"type":"object","required":["Radius1","Radius2","Height","Angle","Placement"],"additionalProperties":false,"properties":{"Radius1":{"type":"number","description":"The bottom radius of the cone"},"Radius2":{"type":"number","description":"The top radius of the cone"},"Height":{"type":"number","description":"The height of the cone"},"Angle":{"type":"number","description":"The angle of the cone"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Cut":{"type":"object","required":["Base","Tool","Refine","Placement"],"additionalProperties":false,"properties":{"Base":{"type":"string","description":"The base of the cut operator","fcType":"App::PropertyLink"},"Tool":{"type":"string","description":"The tool of the cut operator","fcType":"App::PropertyLink"},"Refine":{"type":"boolean","description":"Refine shape"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Cylinder":{"type":"object","required":["Radius","Angle","Height","Placement"],"additionalProperties":false,"properties":{"Radius":{"type":"number","description":"Radius of the cylinder"},"Height":{"type":"number","description":"Height of the cylinder"},"Angle":{"type":"number","description":"Angle of the cylinder"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::MultiFuse":{"type":"object","required":["Shapes","Refine","Placement"],"additionalProperties":false,"properties":{"Shapes":{"type":"array","description":"The shapes of the individual elements","fcType":"App::PropertyLinkList","items":{"type":"string"}},"Refine":{"type":"boolean","description":"Refine shape"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Extrusion":{"type":"object","required":["Base","Dir","LengthFwd","LengthRev","Solid","Placement"],"additionalProperties":false,"properties":{"Base":{"type":"string","description":"Shape to extrude","fcType":"App::PropertyLink"},"Dir":{"type":"array","description":"Direction of extrusion","items":{"type":"number"}},"LengthFwd":{"type":"number","description":"Length of extrusion along the direction"},"LengthRev":{"type":"number","description":"Length of extrusion against the direction"},"Solid":{"type":"boolean","description":"If true, creating a solid"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::MultiCommon":{"type":"object","required":["Shapes","Refine","Placement"],"additionalProperties":false,"properties":{"Shapes":{"type":"array","description":"The objects to intersect","fcType":"App::PropertyLinkList","items":{"type":"string"}},"Refine":{"type":"boolean","description":"Refine shape"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Sketcher::SketchObject":{"type":"object","required":["AttachmentOffset","Geometry"],"additionalProperties":false,"properties":{"AttachmentOffset":{"description":"The attachment offset","type":"object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}},"Geometry":{"type":"array","description":"The geometry list","items":{"anyOf":[{"type":"object","description":"Part::GeomCircle","title":"IGeomCircle","required":["TypeId","CenterX","CenterY","CenterZ","NormalX","NormalY","NormalZ","AngleXU","Radius"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomCircle","description":"Geometry type"},"CenterX":{"type":"number","description":"CenterX"},"CenterY":{"type":"number","description":"CenterY"},"CenterZ":{"type":"number","description":"CenterZ"},"NormalX":{"type":"number","description":"NormalX"},"NormalY":{"type":"number","description":"NormalY"},"NormalZ":{"type":"number","description":"NormalZ"},"AngleXU":{"type":"number","description":"AngleXU"},"Radius":{"type":"number","description":"Radius"}}},{"type":"object","description":"Part::GeomLineSegment","title":"IGeomLineSegment","required":["TypeId","StartX","StartY","StartZ","EndX","EndY","EndZ"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomLineSegment","description":"Geometry type"},"StartX":{"type":"number","description":"StartX"},"StartY":{"type":"number","description":"StartY"},"StartZ":{"type":"number","description":"StartZ"},"EndX":{"type":"number","description":"EndX"},"EndY":{"type":"number","description":"EndY"},"EndZ":{"type":"number","description":"EndZ"}}}]}},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Sphere":{"type":"object","required":["Radius","Angle1","Angle2","Angle3","Placement"],"additionalProperties":false,"properties":{"Radius":{"type":"number","description":"The radius of the sphere"},"Angle1":{"type":"number","description":"The angle of the sphere"},"Angle2":{"type":"number","description":"The angle of the sphere"},"Angle3":{"type":"number","description":"The angle of the sphere"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Torus":{"type":"object","required":["Radius1","Radius2","Angle1","Angle2","Angle3","Placement"],"additionalProperties":false,"properties":{"Radius1":{"type":"number","description":"The radius of the torus"},"Radius2":{"type":"number","description":"The radius of the torus"},"Angle1":{"type":"number","description":"The angle of the torus"},"Angle2":{"type":"number","description":"The angle of the torus"},"Angle3":{"type":"number","description":"The angle of the torus"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}}}');
+            const b = JSON.parse('{"Part::GeomCircle":{"type":"object","required":["TypeId","CenterX","CenterY","CenterZ","NormalX","NormalY","NormalZ","AngleXU","Radius"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomCircle","description":"Geometry type"},"CenterX":{"type":"number","description":"CenterX"},"CenterY":{"type":"number","description":"CenterY"},"CenterZ":{"type":"number","description":"CenterZ"},"NormalX":{"type":"number","description":"NormalX"},"NormalY":{"type":"number","description":"NormalY"},"NormalZ":{"type":"number","description":"NormalZ"},"AngleXU":{"type":"number","description":"AngleXU"},"Radius":{"type":"number","description":"Radius"}}},"Part::GeomLineSegment":{"type":"object","required":["TypeId","StartX","StartY","StartZ","EndX","EndY","EndZ"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomLineSegment","description":"Geometry type"},"StartX":{"type":"number","description":"StartX"},"StartY":{"type":"number","description":"StartY"},"StartZ":{"type":"number","description":"StartZ"},"EndX":{"type":"number","description":"EndX"},"EndY":{"type":"number","description":"EndY"},"EndZ":{"type":"number","description":"EndZ"}}},"Placement of the box":{"type":"object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}},"Part::Box":{"type":"object","required":["Length","Width","Height","Placement"],"additionalProperties":false,"properties":{"Length":{"type":"number","description":"The length of the box"},"Width":{"type":"number","description":"The width of the box"},"Height":{"type":"number","description":"The height of the box"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Cone":{"type":"object","required":["Radius1","Radius2","Height","Angle","Placement"],"additionalProperties":false,"properties":{"Radius1":{"type":"number","description":"The bottom radius of the cone"},"Radius2":{"type":"number","description":"The top radius of the cone"},"Height":{"type":"number","description":"The height of the cone"},"Angle":{"type":"number","description":"The angle of the cone"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Cut":{"type":"object","required":["Base","Tool","Refine","Placement"],"additionalProperties":false,"properties":{"Base":{"type":"string","description":"The base of the cut operator","fcType":"App::PropertyLink"},"Tool":{"type":"string","description":"The tool of the cut operator","fcType":"App::PropertyLink"},"Refine":{"type":"boolean","description":"Refine shape"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::MultiFuse":{"type":"object","required":["Shapes","Refine","Placement"],"additionalProperties":false,"properties":{"Shapes":{"type":"array","description":"The shapes of the individual elements","fcType":"App::PropertyLinkList","items":{"type":"string"}},"Refine":{"type":"boolean","description":"Refine shape"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Extrusion":{"type":"object","required":["Base","Dir","LengthFwd","LengthRev","Solid","Placement"],"additionalProperties":false,"properties":{"Base":{"type":"string","description":"Shape to extrude","fcType":"App::PropertyLink"},"Dir":{"type":"array","description":"Direction of extrusion","items":{"type":"number"}},"LengthFwd":{"type":"number","description":"Length of extrusion along the direction"},"LengthRev":{"type":"number","description":"Length of extrusion against the direction"},"Solid":{"type":"boolean","description":"If true, creating a solid"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Cylinder":{"type":"object","required":["Radius","Angle","Height","Placement"],"additionalProperties":false,"properties":{"Radius":{"type":"number","description":"Radius of the cylinder"},"Height":{"type":"number","description":"Height of the cylinder"},"Angle":{"type":"number","description":"Angle of the cylinder"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::MultiCommon":{"type":"object","required":["Shapes","Refine","Placement"],"additionalProperties":false,"properties":{"Shapes":{"type":"array","description":"The objects to intersect","fcType":"App::PropertyLinkList","items":{"type":"string"}},"Refine":{"type":"boolean","description":"Refine shape"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Sketcher::SketchObject":{"type":"object","required":["AttachmentOffset","Geometry"],"additionalProperties":false,"properties":{"AttachmentOffset":{"description":"The attachment offset","type":"object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}},"Geometry":{"type":"array","description":"The geometry list","items":{"anyOf":[{"type":"object","description":"Part::GeomCircle","title":"IGeomCircle","required":["TypeId","CenterX","CenterY","CenterZ","NormalX","NormalY","NormalZ","AngleXU","Radius"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomCircle","description":"Geometry type"},"CenterX":{"type":"number","description":"CenterX"},"CenterY":{"type":"number","description":"CenterY"},"CenterZ":{"type":"number","description":"CenterZ"},"NormalX":{"type":"number","description":"NormalX"},"NormalY":{"type":"number","description":"NormalY"},"NormalZ":{"type":"number","description":"NormalZ"},"AngleXU":{"type":"number","description":"AngleXU"},"Radius":{"type":"number","description":"Radius"}}},{"type":"object","description":"Part::GeomLineSegment","title":"IGeomLineSegment","required":["TypeId","StartX","StartY","StartZ","EndX","EndY","EndZ"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomLineSegment","description":"Geometry type"},"StartX":{"type":"number","description":"StartX"},"StartY":{"type":"number","description":"StartY"},"StartZ":{"type":"number","description":"StartZ"},"EndX":{"type":"number","description":"EndX"},"EndY":{"type":"number","description":"EndY"},"EndZ":{"type":"number","description":"EndZ"}}}]}},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Sphere":{"type":"object","required":["Radius","Angle1","Angle2","Angle3","Placement"],"additionalProperties":false,"properties":{"Radius":{"type":"number","description":"The radius of the sphere"},"Angle1":{"type":"number","description":"The angle of the sphere"},"Angle2":{"type":"number","description":"The angle of the sphere"},"Angle3":{"type":"number","description":"The angle of the sphere"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Torus":{"type":"object","required":["Radius1","Radius2","Angle1","Angle2","Angle3","Placement"],"additionalProperties":false,"properties":{"Radius1":{"type":"number","description":"The radius of the torus"},"Radius2":{"type":"number","description":"The radius of the torus"},"Angle1":{"type":"number","description":"The angle of the torus"},"Angle2":{"type":"number","description":"The angle of the torus"},"Angle3":{"type":"number","description":"The angle of the torus"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}}}');
             var f = function(e, t) {
                 var n = {};
                 for (var a in e) Object.prototype.hasOwnProperty.call(e, a) && t.indexOf(a) < 0 && (n[a] = e[a]);
                 if (null != e && "function" == typeof Object.getOwnPropertySymbols) {
                     var o = 0;
                     for (a = Object.getOwnPropertySymbols(e); o < a.length; o++) t.indexOf(a[o]) < 0 && Object.prototype.propertyIsEnumerable.call(e, a[o]) && (n[a[o]] = e[a[o]])
                 }
```

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/1882.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/1882.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/1935.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/1935.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/1959.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/1959.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/2033.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/2033.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/2042.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/2042.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/2075.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/2075.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/2100.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/2100.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/2106.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/2106.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/2185.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/2185.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/2194.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/2194.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/2284.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/2284.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/23.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/23.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/231.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/231.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/2318.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/2318.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/2488.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/2488.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/2502.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/2502.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/2553.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/2553.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/2628.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/2628.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/2667.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/2667.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/2687.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/2687.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/274.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/274.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/275.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/275.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/2784.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/2784.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/2805.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/2805.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/288.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/288.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/2970.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/2970.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/3007.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/3007.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/3093.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/3093.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/3159.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/3159.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/3191.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/3191.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/3192.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/3192.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/3206.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/3206.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/3211.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/3211.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/330.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/330.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/3312.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/3312.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/3316.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/3316.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/3324.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/3324.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/3326.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/3326.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/3330.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/3330.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/3397.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/3397.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/3466.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/3466.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/3499.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/3499.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/3500.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/3500.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/351.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/351.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/3540.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/3540.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/3542.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/3542.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/358.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/358.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/360.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/360.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/3656.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/3656.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/3656.app.js.LICENSE.txt` & `jupytercad-0.2.3/jupytercad/cadapp/static/3656.app.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/370.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/370.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/3726.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/3726.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/373c04fd2418f5c77eea.eot` & `jupytercad-0.2.3/jupytercad/cadapp/static/373c04fd2418f5c77eea.eot`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/3811.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/3811.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/3851.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/3851.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/3855.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/3855.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/386.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/386.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/3872.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/3872.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/3880.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/3880.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/3f6d3488cf65374f6f67.woff` & `jupytercad-0.2.3/jupytercad/cadapp/static/3f6d3488cf65374f6f67.woff`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/4024.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/4024.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/4040.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/4040.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/4059.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/4059.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/4065.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/4065.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/4073.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/4073.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/4123.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/4123.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/4171.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/4171.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/4282.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/4282.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/4283.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/4283.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/4299.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/4299.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/4351.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/4351.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/4359.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/4359.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/4391.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/4391.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/4403.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/4403.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/4462.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/4462.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/4476.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/4476.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/450.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/450.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/4608.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/4608.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/4651.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/4651.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/4654.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/4654.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/4679.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/4679.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/4702.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/4702.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/4718.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/4718.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/4808.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/4808.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/484.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/484.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/4874.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/4874.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/4878.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/4878.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/4935.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/4935.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/4965.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/4965.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/4973.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/4973.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/4982.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/4982.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/5002.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/5002.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/5024.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/5024.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/504.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/504.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/5064.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/5064.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/5101.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/5101.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/5148.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/5148.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/5172.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/5172.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/5176.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/5176.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/5223.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/5223.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/5225.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/5225.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/5231.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/5231.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/5263.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/5263.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/5340.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/5340.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/5393.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/5393.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/5430.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/5430.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/5433.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/5433.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/5445.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/5445.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/550.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/550.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/5513.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/5513.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/5514.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/5514.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/5544.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/5544.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/5556.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/5556.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/558.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/558.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/5587.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/5587.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/5681.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/5681.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/5708.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/5708.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/5764.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/5764.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/5811.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/5811.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/5817.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/5817.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/5876.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/5876.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/5882.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/5882.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/6146.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/6146.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/6151.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/6151.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/6186.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/6186.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/6196.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/6196.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/6410.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/6410.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/6483.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/6483.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/6510.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/6510.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/6645.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/6645.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/6686.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/6686.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/6770.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/6770.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/6778.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/6778.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/6782.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/6782.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/6808.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/6808.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/6833.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/6833.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/6835.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/6835.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/6914.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/6914.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/6970.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/6970.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/7058.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/7058.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/7102.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/7102.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/7111.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/7111.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/7127.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/7127.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/7149.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/7149.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/7174.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/7174.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/7233.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/7233.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/7236.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/7236.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/7294.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/7294.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/730.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/730.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/7377.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/7377.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/7379.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/7379.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/7424.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/7424.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/7469.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/7469.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/7498.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/7498.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/7526.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/7526.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/7529.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/7529.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/7600.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/7600.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/765.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/765.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/7664.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/7664.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/769.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/769.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/7710.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/7710.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/7806.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/7806.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/7860.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/7860.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/7882.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/7882.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/7884.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/7884.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/7955.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/7955.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/7991.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/7991.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/79d088064beb3826054f.eot` & `jupytercad-0.2.3/jupytercad/cadapp/static/79d088064beb3826054f.eot`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/8078.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/8078.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/8090.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/8090.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/8100.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/8100.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/8124.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/8124.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/8138.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/8138.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/819.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/819.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/8307.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/8307.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/8342.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/8342.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/8409.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/8409.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/8423.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/8423.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/8441.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/8441.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/8442.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/8442.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/846.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/846.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/8466.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/8466.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/8496.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/8496.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/8518.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/8518.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/8561.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/8561.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/8576.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/8576.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/8615.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/8615.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/8640.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/8640.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/8658.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/8658.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/8662.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/8662.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/8728.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/8728.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/8763.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/8763.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/8769.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/8769.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/8782.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/8782.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/8803.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/8803.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/882.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/882.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/8866.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/8866.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/8877.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/8877.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/8914.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/8914.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/8953.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/8953.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/8ea8791754915a898a31.woff2` & `jupytercad-0.2.3/jupytercad/cadapp/static/8ea8791754915a898a31.woff2`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/9036.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/9036.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/9060.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/9060.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/9117.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/9117.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/9172.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/9172.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/9304.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/9304.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/9308.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/9308.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/9318.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/9318.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/9319.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/9319.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/9339.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/9339.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/9369.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/9369.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/9397.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/9397.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/9406.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/9406.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/9411.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/9411.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/9472.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/9472.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/9473.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/9473.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/9491.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/9491.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/9513.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/9513.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/9583.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/9583.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/9631.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/9631.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/9636.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/9636.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/9672.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/9672.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/9674eb1bd55047179038.svg` & `jupytercad-0.2.3/jupytercad/cadapp/static/9674eb1bd55047179038.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/9715.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/9715.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/9787.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/9787.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/9787.app.js.LICENSE.txt` & `jupytercad-0.2.3/jupytercad/cadapp/static/9787.app.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/9811.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/9811.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/9822.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/9822.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/9827.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/9827.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/9834b82ad26e2a37583d.woff2` & `jupytercad-0.2.3/jupytercad/cadapp/static/9834b82ad26e2a37583d.woff2`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/9866.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/9866.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/9877.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/9877.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/9908.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/9908.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/9932.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/9932.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/9961.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/9961.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/9976.app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/9976.app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/a3b9817780214caf01e8.svg` & `jupytercad-0.2.3/jupytercad/cadapp/static/a3b9817780214caf01e8.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/af6397503fcefbd61397.ttf` & `jupytercad-0.2.3/jupytercad/cadapp/static/af6397503fcefbd61397.ttf`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/app.js` & `jupytercad-0.2.3/jupytercad/cadapp/static/app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/be0a084962d8066884f7.svg` & `jupytercad-0.2.3/jupytercad/cadapp/static/be0a084962d8066884f7.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/cb9e9e693192413cde2b.woff` & `jupytercad-0.2.3/jupytercad/cadapp/static/cb9e9e693192413cde2b.woff`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/cda59d6efffa685830fd.ttf` & `jupytercad-0.2.3/jupytercad/cadapp/static/cda59d6efffa685830fd.ttf`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/e4299464e7b012968eed.eot` & `jupytercad-0.2.3/jupytercad/cadapp/static/e4299464e7b012968eed.eot`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/e42a88444448ac3d6054.woff2` & `jupytercad-0.2.3/jupytercad/cadapp/static/e42a88444448ac3d6054.woff2`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/e8711bbb871afd8e9dea.ttf` & `jupytercad-0.2.3/jupytercad/cadapp/static/e8711bbb871afd8e9dea.ttf`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/static/f9217f66874b0c01cd8c.woff` & `jupytercad-0.2.3/jupytercad/cadapp/static/f9217f66874b0c01cd8c.woff`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/templates/index.html` & `jupytercad-0.2.3/jupytercad/cadapp/templates/index.html`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/themes/@jupyterlab/theme-dark-extension/index.css` & `jupytercad-0.2.3/jupytercad/cadapp/themes/@jupyterlab/theme-dark-extension/index.css`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/cadapp/themes/@jupyterlab/theme-light-extension/index.css` & `jupytercad-0.2.3/jupytercad/cadapp/themes/@jupyterlab/theme-light-extension/index.css`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/freecad/loader.py` & `jupytercad-0.2.3/jupytercad/freecad/loader.py`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/freecad/props/base_prop.py` & `jupytercad-0.2.3/jupytercad/freecad/props/base_prop.py`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/freecad/props/property_geometrylist.py` & `jupytercad-0.2.3/jupytercad/freecad/props/property_geometrylist.py`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/freecad/props/property_partshape.py` & `jupytercad-0.2.3/jupytercad/freecad/props/property_partshape.py`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/freecad/props/property_placement.py` & `jupytercad-0.2.3/jupytercad/freecad/props/property_placement.py`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/freecad/props/geometry/geom_circle.py` & `jupytercad-0.2.3/jupytercad/freecad/props/geometry/geom_circle.py`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/freecad/props/geometry/geom_linesegment.py` & `jupytercad-0.2.3/jupytercad/freecad/props/geometry/geom_linesegment.py`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/labextension/package.json` & `jupytercad-0.2.3/jupytercad/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9741927083333334%*

 * *Differences: {"'dependencies'": "{'@jupytercad/jupytercad-opencascade': '^0.2.3'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.190fffa25e51baa1896b.js'}}",*

 * * "'version'": "'0.2.3'"}*

```diff
@@ -6,15 +6,15 @@
         "url": "https://github.com/QuantStack/jupytercad/issues"
     },
     "dependencies": {
         "@deathbeds/jupyterlab-rjsf": "^1.1.0",
         "@jupyter/collaboration": "^1.0.0",
         "@jupyter/docprovider": "^1.0.0",
         "@jupyter/ydoc": "^0.3.4 || ^1.0.2",
-        "@jupytercad/jupytercad-opencascade": "^0.2.2",
+        "@jupytercad/jupytercad-opencascade": "^0.2.3",
         "@jupyterlab/application": "^4.0.0",
         "@jupyterlab/apputils": "^4.0.0",
         "@jupyterlab/coreutils": "^6.0.0",
         "@jupyterlab/docregistry": "^4.0.0",
         "@jupyterlab/filebrowser": "^4.0.0",
         "@jupyterlab/launcher": "^4.0.0",
         "@jupyterlab/mainmenu": "^4.0.0",
@@ -57,15 +57,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/QuantStack/jupytercad",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.ed192893ffeb37154379.js",
+            "load": "static/remoteEntry.190fffa25e51baa1896b.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../../jupytercad/labextension",
         "sharedPackages": {
             "yjs": {
                 "bundled": false,
@@ -113,9 +113,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.2.2"
+    "version": "0.2.3"
 }
```

### Comparing `jupytercad-0.2.2/jupytercad/labextension/static/184.6f76dd957e411be19baa.js` & `jupytercad-0.2.3/jupytercad/labextension/static/184.6f76dd957e411be19baa.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/labextension/static/213.778b3209dbe7ec5470b6.js` & `jupytercad-0.2.3/jupytercad/labextension/static/213.778b3209dbe7ec5470b6.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/labextension/static/268.16c8a4126908b03651f0.js` & `jupytercad-0.2.3/jupytercad/labextension/static/268.16c8a4126908b03651f0.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/labextension/static/288.11fba3e29cc454c9c071.js` & `jupytercad-0.2.3/jupytercad/labextension/static/288.11fba3e29cc454c9c071.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/labextension/static/358.45fb46ea24bb44ba7fa9.js` & `jupytercad-0.2.3/jupytercad/labextension/static/358.45fb46ea24bb44ba7fa9.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/labextension/static/379.5df518c877987fc7ca0c.js` & `jupytercad-0.2.3/jupytercad/labextension/static/379.5df518c877987fc7ca0c.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/labextension/static/406.5ed89c99d9b3043c85c0.js` & `jupytercad-0.2.3/jupytercad/labextension/static/406.5ed89c99d9b3043c85c0.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/labextension/static/422.39a95e19d3a414516796.js` & `jupytercad-0.2.3/jupytercad/labextension/static/422.39a95e19d3a414516796.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/labextension/static/52.477d969cb88d8007c4f0.js` & `jupytercad-0.2.3/jupytercad/labextension/static/52.477d969cb88d8007c4f0.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/labextension/static/544.40107d96caa6825dcd16.js` & `jupytercad-0.2.3/jupytercad/labextension/static/544.04fb377af8d9c7574a58.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -892,15 +892,15 @@
                     })), super({
                         title: e.title,
                         body: i,
                         buttons: [o.Dialog.cancelButton()]
                     }), this.addClass("jpcad-property-FormDialog")
                 }
             }
-            const ee = JSON.parse('{"Part::GeomCircle":{"type":"object","required":["TypeId","CenterX","CenterY","CenterZ","NormalX","NormalY","NormalZ","AngleXU","Radius"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomCircle","description":"Geometry type"},"CenterX":{"type":"number","description":"CenterX"},"CenterY":{"type":"number","description":"CenterY"},"CenterZ":{"type":"number","description":"CenterZ"},"NormalX":{"type":"number","description":"NormalX"},"NormalY":{"type":"number","description":"NormalY"},"NormalZ":{"type":"number","description":"NormalZ"},"AngleXU":{"type":"number","description":"AngleXU"},"Radius":{"type":"number","description":"Radius"}}},"Part::GeomLineSegment":{"type":"object","required":["TypeId","StartX","StartY","StartZ","EndX","EndY","EndZ"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomLineSegment","description":"Geometry type"},"StartX":{"type":"number","description":"StartX"},"StartY":{"type":"number","description":"StartY"},"StartZ":{"type":"number","description":"StartZ"},"EndX":{"type":"number","description":"EndX"},"EndY":{"type":"number","description":"EndY"},"EndZ":{"type":"number","description":"EndZ"}}},"Placement of the box":{"type":"object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}},"Part::Box":{"type":"object","required":["Length","Width","Height","Placement"],"additionalProperties":false,"properties":{"Length":{"type":"number","description":"The length of the box"},"Width":{"type":"number","description":"The width of the box"},"Height":{"type":"number","description":"The height of the box"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Cone":{"type":"object","required":["Radius1","Radius2","Height","Angle","Placement"],"additionalProperties":false,"properties":{"Radius1":{"type":"number","description":"The bottom radius of the cone"},"Radius2":{"type":"number","description":"The top radius of the cone"},"Height":{"type":"number","description":"The height of the cone"},"Angle":{"type":"number","description":"The angle of the cone"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Cut":{"type":"object","required":["Base","Tool","Refine","Placement"],"additionalProperties":false,"properties":{"Base":{"type":"string","description":"The base of the cut operator","fcType":"App::PropertyLink"},"Tool":{"type":"string","description":"The tool of the cut operator","fcType":"App::PropertyLink"},"Refine":{"type":"boolean","description":"Refine shape"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Cylinder":{"type":"object","required":["Radius","Angle","Height","Placement"],"additionalProperties":false,"properties":{"Radius":{"type":"number","description":"Radius of the cylinder"},"Height":{"type":"number","description":"Height of the cylinder"},"Angle":{"type":"number","description":"Angle of the cylinder"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::MultiFuse":{"type":"object","required":["Shapes","Refine","Placement"],"additionalProperties":false,"properties":{"Shapes":{"type":"array","description":"The shapes of the individual elements","fcType":"App::PropertyLinkList","items":{"type":"string"}},"Refine":{"type":"boolean","description":"Refine shape"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Extrusion":{"type":"object","required":["Base","Dir","LengthFwd","LengthRev","Solid","Placement"],"additionalProperties":false,"properties":{"Base":{"type":"string","description":"Shape to extrude","fcType":"App::PropertyLink"},"Dir":{"type":"array","description":"Direction of extrusion","items":{"type":"number"}},"LengthFwd":{"type":"number","description":"Length of extrusion along the direction"},"LengthRev":{"type":"number","description":"Length of extrusion against the direction"},"Solid":{"type":"boolean","description":"If true, creating a solid"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::MultiCommon":{"type":"object","required":["Shapes","Refine","Placement"],"additionalProperties":false,"properties":{"Shapes":{"type":"array","description":"The objects to intersect","fcType":"App::PropertyLinkList","items":{"type":"string"}},"Refine":{"type":"boolean","description":"Refine shape"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Sketcher::SketchObject":{"type":"object","required":["AttachmentOffset","Geometry"],"additionalProperties":false,"properties":{"AttachmentOffset":{"description":"The attachment offset","type":"object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}},"Geometry":{"type":"array","description":"The geometry list","items":{"anyOf":[{"type":"object","description":"Part::GeomCircle","title":"IGeomCircle","required":["TypeId","CenterX","CenterY","CenterZ","NormalX","NormalY","NormalZ","AngleXU","Radius"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomCircle","description":"Geometry type"},"CenterX":{"type":"number","description":"CenterX"},"CenterY":{"type":"number","description":"CenterY"},"CenterZ":{"type":"number","description":"CenterZ"},"NormalX":{"type":"number","description":"NormalX"},"NormalY":{"type":"number","description":"NormalY"},"NormalZ":{"type":"number","description":"NormalZ"},"AngleXU":{"type":"number","description":"AngleXU"},"Radius":{"type":"number","description":"Radius"}}},{"type":"object","description":"Part::GeomLineSegment","title":"IGeomLineSegment","required":["TypeId","StartX","StartY","StartZ","EndX","EndY","EndZ"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomLineSegment","description":"Geometry type"},"StartX":{"type":"number","description":"StartX"},"StartY":{"type":"number","description":"StartY"},"StartZ":{"type":"number","description":"StartZ"},"EndX":{"type":"number","description":"EndX"},"EndY":{"type":"number","description":"EndY"},"EndZ":{"type":"number","description":"EndZ"}}}]}},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Sphere":{"type":"object","required":["Radius","Angle1","Angle2","Angle3","Placement"],"additionalProperties":false,"properties":{"Radius":{"type":"number","description":"The radius of the sphere"},"Angle1":{"type":"number","description":"The angle of the sphere"},"Angle2":{"type":"number","description":"The angle of the sphere"},"Angle3":{"type":"number","description":"The angle of the sphere"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Torus":{"type":"object","required":["Radius1","Radius2","Angle1","Angle2","Angle3","Placement"],"additionalProperties":false,"properties":{"Radius1":{"type":"number","description":"The radius of the torus"},"Radius2":{"type":"number","description":"The radius of the torus"},"Angle1":{"type":"number","description":"The angle of the torus"},"Angle2":{"type":"number","description":"The angle of the torus"},"Angle3":{"type":"number","description":"The angle of the torus"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}}}');
+            const ee = JSON.parse('{"Part::GeomCircle":{"type":"object","required":["TypeId","CenterX","CenterY","CenterZ","NormalX","NormalY","NormalZ","AngleXU","Radius"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomCircle","description":"Geometry type"},"CenterX":{"type":"number","description":"CenterX"},"CenterY":{"type":"number","description":"CenterY"},"CenterZ":{"type":"number","description":"CenterZ"},"NormalX":{"type":"number","description":"NormalX"},"NormalY":{"type":"number","description":"NormalY"},"NormalZ":{"type":"number","description":"NormalZ"},"AngleXU":{"type":"number","description":"AngleXU"},"Radius":{"type":"number","description":"Radius"}}},"Part::GeomLineSegment":{"type":"object","required":["TypeId","StartX","StartY","StartZ","EndX","EndY","EndZ"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomLineSegment","description":"Geometry type"},"StartX":{"type":"number","description":"StartX"},"StartY":{"type":"number","description":"StartY"},"StartZ":{"type":"number","description":"StartZ"},"EndX":{"type":"number","description":"EndX"},"EndY":{"type":"number","description":"EndY"},"EndZ":{"type":"number","description":"EndZ"}}},"Placement of the box":{"type":"object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}},"Part::Box":{"type":"object","required":["Length","Width","Height","Placement"],"additionalProperties":false,"properties":{"Length":{"type":"number","description":"The length of the box"},"Width":{"type":"number","description":"The width of the box"},"Height":{"type":"number","description":"The height of the box"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Cone":{"type":"object","required":["Radius1","Radius2","Height","Angle","Placement"],"additionalProperties":false,"properties":{"Radius1":{"type":"number","description":"The bottom radius of the cone"},"Radius2":{"type":"number","description":"The top radius of the cone"},"Height":{"type":"number","description":"The height of the cone"},"Angle":{"type":"number","description":"The angle of the cone"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Cut":{"type":"object","required":["Base","Tool","Refine","Placement"],"additionalProperties":false,"properties":{"Base":{"type":"string","description":"The base of the cut operator","fcType":"App::PropertyLink"},"Tool":{"type":"string","description":"The tool of the cut operator","fcType":"App::PropertyLink"},"Refine":{"type":"boolean","description":"Refine shape"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::MultiFuse":{"type":"object","required":["Shapes","Refine","Placement"],"additionalProperties":false,"properties":{"Shapes":{"type":"array","description":"The shapes of the individual elements","fcType":"App::PropertyLinkList","items":{"type":"string"}},"Refine":{"type":"boolean","description":"Refine shape"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Extrusion":{"type":"object","required":["Base","Dir","LengthFwd","LengthRev","Solid","Placement"],"additionalProperties":false,"properties":{"Base":{"type":"string","description":"Shape to extrude","fcType":"App::PropertyLink"},"Dir":{"type":"array","description":"Direction of extrusion","items":{"type":"number"}},"LengthFwd":{"type":"number","description":"Length of extrusion along the direction"},"LengthRev":{"type":"number","description":"Length of extrusion against the direction"},"Solid":{"type":"boolean","description":"If true, creating a solid"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Cylinder":{"type":"object","required":["Radius","Angle","Height","Placement"],"additionalProperties":false,"properties":{"Radius":{"type":"number","description":"Radius of the cylinder"},"Height":{"type":"number","description":"Height of the cylinder"},"Angle":{"type":"number","description":"Angle of the cylinder"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::MultiCommon":{"type":"object","required":["Shapes","Refine","Placement"],"additionalProperties":false,"properties":{"Shapes":{"type":"array","description":"The objects to intersect","fcType":"App::PropertyLinkList","items":{"type":"string"}},"Refine":{"type":"boolean","description":"Refine shape"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Sketcher::SketchObject":{"type":"object","required":["AttachmentOffset","Geometry"],"additionalProperties":false,"properties":{"AttachmentOffset":{"description":"The attachment offset","type":"object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}},"Geometry":{"type":"array","description":"The geometry list","items":{"anyOf":[{"type":"object","description":"Part::GeomCircle","title":"IGeomCircle","required":["TypeId","CenterX","CenterY","CenterZ","NormalX","NormalY","NormalZ","AngleXU","Radius"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomCircle","description":"Geometry type"},"CenterX":{"type":"number","description":"CenterX"},"CenterY":{"type":"number","description":"CenterY"},"CenterZ":{"type":"number","description":"CenterZ"},"NormalX":{"type":"number","description":"NormalX"},"NormalY":{"type":"number","description":"NormalY"},"NormalZ":{"type":"number","description":"NormalZ"},"AngleXU":{"type":"number","description":"AngleXU"},"Radius":{"type":"number","description":"Radius"}}},{"type":"object","description":"Part::GeomLineSegment","title":"IGeomLineSegment","required":["TypeId","StartX","StartY","StartZ","EndX","EndY","EndZ"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomLineSegment","description":"Geometry type"},"StartX":{"type":"number","description":"StartX"},"StartY":{"type":"number","description":"StartY"},"StartZ":{"type":"number","description":"StartZ"},"EndX":{"type":"number","description":"EndX"},"EndY":{"type":"number","description":"EndY"},"EndZ":{"type":"number","description":"EndZ"}}}]}},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Sphere":{"type":"object","required":["Radius","Angle1","Angle2","Angle3","Placement"],"additionalProperties":false,"properties":{"Radius":{"type":"number","description":"The radius of the sphere"},"Angle1":{"type":"number","description":"The angle of the sphere"},"Angle2":{"type":"number","description":"The angle of the sphere"},"Angle3":{"type":"number","description":"The angle of the sphere"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Torus":{"type":"object","required":["Radius1","Radius2","Angle1","Angle2","Angle3","Placement"],"additionalProperties":false,"properties":{"Radius1":{"type":"number","description":"The radius of the torus"},"Radius2":{"type":"number","description":"The radius of the torus"},"Angle1":{"type":"number","description":"The angle of the torus"},"Angle2":{"type":"number","description":"The angle of the torus"},"Angle3":{"type":"number","description":"The angle of the torus"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}}}');
             var te = function(e, t) {
                 var n = {};
                 for (var s in e) Object.prototype.hasOwnProperty.call(e, s) && t.indexOf(s) < 0 && (n[s] = e[s]);
                 if (null != e && "function" == typeof Object.getOwnPropertySymbols) {
                     var o = 0;
                     for (s = Object.getOwnPropertySymbols(e); o < s.length; o++) t.indexOf(s[o]) < 0 && Object.prototype.propertyIsEnumerable.call(e, s[o]) && (n[s[o]] = e[s[o]])
                 }
```

### Comparing `jupytercad-0.2.2/jupytercad/labextension/static/643.850e055919134443b4fa.js` & `jupytercad-0.2.3/jupytercad/labextension/static/643.850e055919134443b4fa.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/labextension/static/651.3736a4bd9cf2725cc067.js` & `jupytercad-0.2.3/jupytercad/labextension/static/651.3736a4bd9cf2725cc067.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/labextension/static/711.9ae86a9a4b0e0a748ae7.js` & `jupytercad-0.2.3/jupytercad/labextension/static/711.9ae86a9a4b0e0a748ae7.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/labextension/static/712.3d4b32523dbb4dff584d.js` & `jupytercad-0.2.3/jupytercad/labextension/static/712.3d4b32523dbb4dff584d.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/labextension/static/730.5a8c1aad713514a0a596.js` & `jupytercad-0.2.3/jupytercad/labextension/static/730.5a8c1aad713514a0a596.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/labextension/static/733.89a6a4e0561966230286.js` & `jupytercad-0.2.3/jupytercad/labextension/static/733.89a6a4e0561966230286.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/labextension/static/761.1bd8bdc8d51f62af816d.js` & `jupytercad-0.2.3/jupytercad/labextension/static/761.1bd8bdc8d51f62af816d.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/labextension/static/78.8e87e13a67c31f2732c7.js` & `jupytercad-0.2.3/jupytercad/labextension/static/78.8e87e13a67c31f2732c7.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/labextension/static/811.d1c8b6a87faba2d069bd.js` & `jupytercad-0.2.3/jupytercad/labextension/static/811.d1c8b6a87faba2d069bd.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/labextension/static/816.00326e9e5f2436d0d67f.js` & `jupytercad-0.2.3/jupytercad/labextension/static/816.00326e9e5f2436d0d67f.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/labextension/static/833.253bc84b61cd4e2beb80.js` & `jupytercad-0.2.3/jupytercad/labextension/static/833.253bc84b61cd4e2beb80.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/labextension/static/842.116bb3340768f53ea709.js` & `jupytercad-0.2.3/jupytercad/labextension/static/842.116bb3340768f53ea709.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/labextension/static/847.6efcc69e25d704ee7090.js` & `jupytercad-0.2.3/jupytercad/labextension/static/847.6efcc69e25d704ee7090.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/labextension/static/860.9dcab30c320fd0b9cfe1.js` & `jupytercad-0.2.3/jupytercad/labextension/static/860.9dcab30c320fd0b9cfe1.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/labextension/static/955.a084e75defa008fca238.js` & `jupytercad-0.2.3/jupytercad/labextension/static/955.a084e75defa008fca238.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/labextension/static/963.ba192cdc34bc5ccdfe40.js` & `jupytercad-0.2.3/jupytercad/labextension/static/963.ba192cdc34bc5ccdfe40.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/labextension/static/jupytercad.opencascade.wasm` & `jupytercad-0.2.3/jupytercad/labextension/static/jupytercad.opencascade.wasm`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/labextension/static/remoteEntry.ed192893ffeb37154379.js` & `jupytercad-0.2.3/jupytercad/labextension/static/remoteEntry.190fffa25e51baa1896b.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, d, n, o, f, c, l, u, i, b, s, p, h, m, v, y, j, g, P, w, _, x, O, S = {
+    var e, r, t, a, d, n, o, f, l, c, u, i, b, s, p, h, m, v, y, j, g, P, w, _, x, O, S = {
             21306: (e, r, t) => {
                 var a = {
                         "./index": () => Promise.all([t.e(651), t.e(78), t.e(963), t.e(29), t.e(662), t.e(930), t.e(647), t.e(387), t.e(544)]).then((() => () => t(38790))),
                         "./extension": () => Promise.all([t.e(651), t.e(78), t.e(963), t.e(29), t.e(662), t.e(930), t.e(647), t.e(387), t.e(544)]).then((() => () => t(38790))),
                         "./style": () => Promise.all([t.e(847), t.e(643)]).then((() => () => t(76643)))
                     },
                     d = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
@@ -70,15 +70,15 @@
         294: "454be2b126053f634b3b",
         358: "45fb46ea24bb44ba7fa9",
         379: "5df518c877987fc7ca0c",
         387: "4b2774fa163561009f77",
         391: "b0cccbdfb86a0129bdc4",
         406: "5ed89c99d9b3043c85c0",
         422: "39a95e19d3a414516796",
-        544: "40107d96caa6825dcd16",
+        544: "04fb377af8d9c7574a58",
         643: "850e055919134443b4fa",
         647: "de9d2ebc968580177a57",
         651: "3736a4bd9cf2725cc067",
         662: "5542c04bd2cba2e92de1",
         711: "9ae86a9a4b0e0a748ae7",
         712: "3d4b32523dbb4dff584d",
         730: "5a8c1aad713514a0a596",
@@ -104,15 +104,15 @@
         294: "454be2b126053f634b3b",
         358: "45fb46ea24bb44ba7fa9",
         379: "5df518c877987fc7ca0c",
         387: "4b2774fa163561009f77",
         391: "b0cccbdfb86a0129bdc4",
         406: "5ed89c99d9b3043c85c0",
         422: "39a95e19d3a414516796",
-        544: "40107d96caa6825dcd16",
+        544: "04fb377af8d9c7574a58",
         643: "850e055919134443b4fa",
         647: "de9d2ebc968580177a57",
         651: "3736a4bd9cf2725cc067",
         662: "5542c04bd2cba2e92de1",
         711: "9ae86a9a4b0e0a748ae7",
         712: "3d4b32523dbb4dff584d",
         730: "5a8c1aad713514a0a596",
@@ -136,16 +136,16 @@
             if ("object" == typeof window) return window
         }
     }(), k.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), t = {}, a = "@jupytercad/jupytercad-extension:", k.l = (e, r, d, n) => {
         if (t[e]) t[e].push(r);
         else {
             var o, f;
             if (void 0 !== d)
-                for (var c = document.getElementsByTagName("script"), l = 0; l < c.length; l++) {
-                    var u = c[l];
+                for (var l = document.getElementsByTagName("script"), c = 0; c < l.length; c++) {
+                    var u = l[c];
                     if (u.getAttribute("src") == e || u.getAttribute("data-webpack") == a + d) {
                         o = u;
                         break
                     }
                 }
             o || (f = !0, (o = document.createElement("script")).charset = "utf-8", o.timeout = 120, k.nc && o.setAttribute("nonce", k.nc), o.setAttribute("data-webpack", a + d), o.src = e), t[e] = [r];
             var i = (r, a) => {
@@ -182,16 +182,16 @@
                             f = d[r];
                         (!f || !f.loaded && (!a != !f.eager ? a : o > f.from)) && (d[r] = {
                             get: t,
                             from: o,
                             eager: !!a
                         })
                     },
-                    c = [];
-                return "default" === t && (f("@deathbeds/jupyterlab-rjsf", "1.1.0", (() => Promise.all([k.e(184), k.e(29), k.e(662), k.e(294), k.e(387)]).then((() => () => k(46184))))), f("@jupyter/docprovider", "1.0.0", (() => Promise.all([k.e(78), k.e(711), k.e(662), k.e(930), k.e(647)]).then((() => () => k(44711))))), f("@jupytercad/jupytercad-extension", "0.2.2", (() => Promise.all([k.e(651), k.e(78), k.e(963), k.e(29), k.e(662), k.e(930), k.e(647), k.e(387), k.e(544)]).then((() => () => k(38790))))), f("@naisutech/react-tree", "3.1.0", (() => Promise.all([k.e(733), k.e(29), k.e(778), k.e(406)]).then((() => () => k(74733))))), f("@rjsf/core", "3.2.1", (() => Promise.all([k.e(651), k.e(842), k.e(29)]).then((() => () => k(28842))))), f("d3-color", "3.1.0", (() => k.e(52).then((() => () => k(37052))))), f("styled-components", "5.3.10", (() => Promise.all([k.e(761), k.e(29), k.e(816)]).then((() => () => k(69761))))), f("three-mesh-bvh", "0.5.24", (() => Promise.all([k.e(422), k.e(391)]).then((() => () => k(31422))))), f("three", "0.135.0", (() => k.e(955).then((() => () => k(12955))))), f("uuid", "8.3.2", (() => k.e(712).then((() => () => k(67712)))))), e[t] = c.length ? Promise.all(c).then((() => e[t] = 1)) : 1
+                    l = [];
+                return "default" === t && (f("@deathbeds/jupyterlab-rjsf", "1.1.0", (() => Promise.all([k.e(184), k.e(29), k.e(662), k.e(294), k.e(387)]).then((() => () => k(46184))))), f("@jupyter/docprovider", "1.0.0", (() => Promise.all([k.e(78), k.e(711), k.e(662), k.e(930), k.e(647)]).then((() => () => k(44711))))), f("@jupytercad/jupytercad-extension", "0.2.3", (() => Promise.all([k.e(651), k.e(78), k.e(963), k.e(29), k.e(662), k.e(930), k.e(647), k.e(387), k.e(544)]).then((() => () => k(38790))))), f("@naisutech/react-tree", "3.1.0", (() => Promise.all([k.e(733), k.e(29), k.e(778), k.e(406)]).then((() => () => k(74733))))), f("@rjsf/core", "3.2.1", (() => Promise.all([k.e(651), k.e(842), k.e(29)]).then((() => () => k(28842))))), f("d3-color", "3.1.0", (() => k.e(52).then((() => () => k(37052))))), f("styled-components", "5.3.10", (() => Promise.all([k.e(761), k.e(29), k.e(816)]).then((() => () => k(69761))))), f("three-mesh-bvh", "0.5.24", (() => Promise.all([k.e(422), k.e(391)]).then((() => () => k(31422))))), f("three", "0.135.0", (() => k.e(955).then((() => () => k(12955))))), f("uuid", "8.3.2", (() => k.e(712).then((() => () => k(67712)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         k.g.importScripts && (e = k.g.location + "");
         var r = k.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -227,61 +227,61 @@
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
             for (var a = 1, d = 1; d < e.length; d++) a--, t += "u" == (typeof(f = e[d]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, f);
             return t
         }
         var n = [];
         for (d = 1; d < e.length; d++) {
             var f = e[d];
-            n.push(0 === f ? "not(" + c() + ")" : 1 === f ? "(" + c() + " || " + c() + ")" : 2 === f ? n.pop() + " " + n.pop() : o(f))
+            n.push(0 === f ? "not(" + l() + ")" : 1 === f ? "(" + l() + " || " + l() + ")" : 2 === f ? n.pop() + " " + n.pop() : o(f))
         }
-        return c();
+        return l();
 
-        function c() {
+        function l() {
             return n.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, f = (e, r) => {
         if (0 in e) {
             r = d(r);
             var t = e[0],
                 a = t < 0;
             a && (t = -t - 1);
-            for (var n = 0, o = 1, c = !0;; o++, n++) {
-                var l, u, i = o < e.length ? (typeof e[o])[0] : "";
-                if (n >= r.length || "o" == (u = (typeof(l = r[n]))[0])) return !c || ("u" == i ? o > t && !a : "" == i != a);
+            for (var n = 0, o = 1, l = !0;; o++, n++) {
+                var c, u, i = o < e.length ? (typeof e[o])[0] : "";
+                if (n >= r.length || "o" == (u = (typeof(c = r[n]))[0])) return !l || ("u" == i ? o > t && !a : "" == i != a);
                 if ("u" == u) {
-                    if (!c || "u" != i) return !1
-                } else if (c)
+                    if (!l || "u" != i) return !1
+                } else if (l)
                     if (i == u)
                         if (o <= t) {
-                            if (l != e[o]) return !1
+                            if (c != e[o]) return !1
                         } else {
-                            if (a ? l > e[o] : l < e[o]) return !1;
-                            l != e[o] && (c = !1)
+                            if (a ? c > e[o] : c < e[o]) return !1;
+                            c != e[o] && (l = !1)
                         }
                 else if ("s" != i && "n" != i) {
                     if (a || o <= t) return !1;
-                    c = !1, o--
+                    l = !1, o--
                 } else {
                     if (o <= t || u < i != a) return !1;
-                    c = !1
-                } else "s" != i && "n" != i && (c = !1, o--)
+                    l = !1
+                } else "s" != i && "n" != i && (l = !1, o--)
             }
         }
         var b = [],
             s = b.pop.bind(b);
         for (n = 1; n < e.length; n++) {
             var p = e[n];
             b.push(1 == p ? s() | s() : 2 == p ? s() & s() : p ? f(p, r) : !s())
         }
         return !!s()
-    }, c = (e, r) => {
+    }, l = (e, r) => {
         var t = k.S[e];
         if (!t || !k.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
-    }, l = (e, r) => {
+    }, c = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || n(e, r) ? r : e), 0)) && t[r]
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, i = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(a) + ")", b = (e, r, t, a) => {
         var d = u(e, t);
@@ -295,15 +295,15 @@
     }, h = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, m = (e, r, t, a) => {
         h(p(e, r, t, a))
     }, v = e => (e.loaded = 1, e.get()), j = (y = e => function(r, t, a, d) {
         var n = k.I(r);
         return n && n.then ? n.then(e.bind(e, r, k.S[r], t, a, d)) : e(r, k.S[r], t, a, d)
-    })(((e, r, t, a) => r && k.o(r, t) ? v(l(r, t)) : a())), g = y(((e, r, t, a) => (c(e, t), v(s(r, t, a) || m(r, e, t, a) || l(r, t))))), P = y(((e, r, t, a) => (c(e, t), b(r, 0, t, a)))), w = y(((e, r, t, a, d) => {
+    })(((e, r, t, a) => r && k.o(r, t) ? v(c(r, t)) : a())), g = y(((e, r, t, a) => (l(e, t), v(s(r, t, a) || m(r, e, t, a) || c(r, t))))), P = y(((e, r, t, a) => (l(e, t), b(r, 0, t, a)))), w = y(((e, r, t, a, d) => {
         var n = r && k.o(r, t) && s(r, t, a);
         return n ? v(n) : d()
     })), _ = {}, x = {
         66029: () => P("default", "react", [1, 18, 2, 0]),
         9324: () => P("default", "@jupyterlab/apputils", [1, 4, 1, 1]),
         59474: () => P("default", "@jupyterlab/coreutils", [1, 6, 0, 1]),
         74901: () => P("default", "@lumino/signaling", [1, 2, 0, 0]),
@@ -389,20 +389,20 @@
                         o.message = "Loading chunk " + r + " failed.\n(" + d + ": " + n + ")", o.name = "ChunkLoadError", o.type = d, o.request = n, a[1](o)
                     }
                 }), "chunk-" + r, r)
             }
         };
         var r = (r, t) => {
                 var a, d, [n, o, f] = t,
-                    c = 0;
+                    l = 0;
                 if (n.some((r => 0 !== e[r]))) {
                     for (a in o) k.o(o, a) && (k.m[a] = o[a]);
                     f && f(k)
                 }
-                for (r && r(t); c < n.length; c++) d = n[c], k.o(e, d) && e[d] && e[d][0](), e[d] = 0
+                for (r && r(t); l < n.length; l++) d = n[l], k.o(e, d) && e[d] && e[d][0](), e[d] = 0
             },
             t = self.webpackChunk_jupytercad_jupytercad_extension = self.webpackChunk_jupytercad_jupytercad_extension || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), k.nc = void 0;
     var T = k(21306);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@jupytercad/jupytercad-extension"] = T
 })();
```

### Comparing `jupytercad-0.2.2/jupytercad/labextension/static/third-party-licenses.json` & `jupytercad-0.2.3/jupytercad/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/notebook/cad_document.py` & `jupytercad-0.2.3/jupytercad/notebook/cad_document.py`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/notebook/y_connector.py` & `jupytercad-0.2.3/jupytercad/notebook/y_connector.py`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/jupytercad/notebook/objects/_schema/box.py` & `jupytercad-0.2.3/jupytercad/notebook/objects/_schema/cone.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # generated by datamodel-codegen:
-#   filename:  box.json
-#   timestamp: 2023-06-03T11:37:49+00:00
+#   filename:  cone.json
+#   timestamp: 2023-06-05T08:00:30+00:00
 
 from __future__ import annotations
 
 from pydantic import BaseModel, Extra, Field
 
 from . import placement
 
 
-class IBox(BaseModel):
+class ICone(BaseModel):
     class Config:
         extra = Extra.forbid
 
-    Length: float = Field(..., description='The length of the box')
-    Width: float = Field(..., description='The width of the box')
-    Height: float = Field(..., description='The height of the box')
+    Radius1: float = Field(..., description='The bottom radius of the cone')
+    Radius2: float = Field(..., description='The top radius of the cone')
+    Height: float = Field(..., description='The height of the cone')
+    Angle: float = Field(..., description='The angle of the cone')
     Placement: placement.Model
```

### Comparing `jupytercad-0.2.2/jupytercad/notebook/objects/_schema/cone.py` & `jupytercad-0.2.3/jupytercad/notebook/objects/_schema/sphere.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # generated by datamodel-codegen:
-#   filename:  cone.json
-#   timestamp: 2023-06-03T11:37:49+00:00
+#   filename:  sphere.json
+#   timestamp: 2023-06-05T08:00:30+00:00
 
 from __future__ import annotations
 
 from pydantic import BaseModel, Extra, Field
 
 from . import placement
 
 
-class ICone(BaseModel):
+class ISphere(BaseModel):
     class Config:
         extra = Extra.forbid
 
-    Radius1: float = Field(..., description='The bottom radius of the cone')
-    Radius2: float = Field(..., description='The top radius of the cone')
-    Height: float = Field(..., description='The height of the cone')
-    Angle: float = Field(..., description='The angle of the cone')
+    Radius: float = Field(..., description='The radius of the sphere')
+    Angle1: float = Field(..., description='The angle of the sphere')
+    Angle2: float = Field(..., description='The angle of the sphere')
+    Angle3: float = Field(..., description='The angle of the sphere')
     Placement: placement.Model
```

### Comparing `jupytercad-0.2.2/jupytercad/notebook/objects/_schema/cylinder.py` & `jupytercad-0.2.3/jupytercad/notebook/objects/_schema/cylinder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  cylinder.json
-#   timestamp: 2023-06-03T11:37:49+00:00
+#   timestamp: 2023-06-05T08:00:30+00:00
 
 from __future__ import annotations
 
 from pydantic import BaseModel, Extra, Field
 
 from . import placement
```

### Comparing `jupytercad-0.2.2/jupytercad/notebook/objects/_schema/extrusion.py` & `jupytercad-0.2.3/jupytercad/notebook/objects/_schema/extrusion.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  extrusion.json
-#   timestamp: 2023-06-03T11:37:49+00:00
+#   timestamp: 2023-06-05T08:00:30+00:00
 
 from __future__ import annotations
 
 from typing import List
 
 from pydantic import BaseModel, Extra, Field
```

### Comparing `jupytercad-0.2.2/jupytercad/notebook/objects/_schema/geomCircle.py` & `jupytercad-0.2.3/jupytercad/notebook/objects/_schema/geomCircle.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  geomCircle.json
-#   timestamp: 2023-06-03T11:37:49+00:00
+#   timestamp: 2023-06-05T08:00:30+00:00
 
 from __future__ import annotations
 
 from pydantic import BaseModel, Extra, Field
 
 
 class IGeomCircle(BaseModel):
```

### Comparing `jupytercad-0.2.2/jupytercad/notebook/objects/_schema/geomLineSegment.py` & `jupytercad-0.2.3/jupytercad/notebook/objects/_schema/geomLineSegment.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  geomLineSegment.json
-#   timestamp: 2023-06-03T11:37:49+00:00
+#   timestamp: 2023-06-05T08:00:30+00:00
 
 from __future__ import annotations
 
 from pydantic import BaseModel, Extra, Field
 
 
 class IGeomLineSegment(BaseModel):
```

### Comparing `jupytercad-0.2.2/jupytercad/notebook/objects/_schema/jcad.py` & `jupytercad-0.2.3/jupytercad/notebook/objects/_schema/jcad.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  jcad.json
-#   timestamp: 2023-06-03T11:37:49+00:00
+#   timestamp: 2023-06-05T08:00:30+00:00
 
 from __future__ import annotations
 
 from enum import Enum
 from typing import Any, Dict, List, Optional
 
 from pydantic import BaseModel, Extra, Field, constr
```

### Comparing `jupytercad-0.2.2/jupytercad/notebook/objects/_schema/sketch.py` & `jupytercad-0.2.3/jupytercad/notebook/objects/_schema/sketch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  sketch.json
-#   timestamp: 2023-06-03T11:37:49+00:00
+#   timestamp: 2023-06-05T08:00:30+00:00
 
 from __future__ import annotations
 
 from typing import List, Optional, Union
 
 from pydantic import BaseModel, Extra, Field
```

### Comparing `jupytercad-0.2.2/jupytercad/notebook/objects/_schema/sphere.py` & `jupytercad-0.2.3/jupytercad/notebook/objects/_schema/torus.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # generated by datamodel-codegen:
-#   filename:  sphere.json
-#   timestamp: 2023-06-03T11:37:49+00:00
+#   filename:  torus.json
+#   timestamp: 2023-06-05T08:00:30+00:00
 
 from __future__ import annotations
 
 from pydantic import BaseModel, Extra, Field
 
 from . import placement
 
 
-class ISphere(BaseModel):
+class ITorus(BaseModel):
     class Config:
         extra = Extra.forbid
 
-    Radius: float = Field(..., description='The radius of the sphere')
-    Angle1: float = Field(..., description='The angle of the sphere')
-    Angle2: float = Field(..., description='The angle of the sphere')
-    Angle3: float = Field(..., description='The angle of the sphere')
+    Radius1: float = Field(..., description='The radius of the torus')
+    Radius2: float = Field(..., description='The radius of the torus')
+    Angle1: float = Field(..., description='The angle of the torus')
+    Angle2: float = Field(..., description='The angle of the torus')
+    Angle3: float = Field(..., description='The angle of the torus')
     Placement: placement.Model
```

### Comparing `jupytercad-0.2.2/scripts/bump-version.py` & `jupytercad-0.2.3/scripts/bump-version.py`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-app/package.json` & `jupytercad-0.2.3/packages/jupytercad-app/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9639057750759878%*

 * *Differences: {"'dependencies'": "{'@jupytercad/jupytercad-extension': '^0.2.3'}", "'version'": "'0.2.3'"}*

```diff
@@ -4,15 +4,15 @@
     },
     "dependencies": {
         "@codemirror/state": "^6.2.0",
         "@codemirror/view": "^6.9.3",
         "@jupyter/collaboration": "^1.0.0",
         "@jupyter/docprovider": "^1.0.0",
         "@jupyter/ydoc": "^0.3.4 || ^1.0.2",
-        "@jupytercad/jupytercad-extension": "^0.2.2",
+        "@jupytercad/jupytercad-extension": "^0.2.3",
         "@jupyterlab/application": "^4.0.0",
         "@jupyterlab/application-extension": "^4.0.0",
         "@jupyterlab/apputils": "^4.0.0",
         "@jupyterlab/apputils-extension": "^4.0.0",
         "@jupyterlab/codemirror": "^4.0.0",
         "@jupyterlab/codemirror-extension": "^4.0.0",
         "@jupyterlab/coreutils": "^6.0.0",
@@ -84,9 +84,9 @@
         "watch:webpack": "webpack --watch"
     },
     "sideEffects": [
         "style/**/*.css"
     ],
     "style": "style/index.css",
     "types": "lib/index.d.ts",
-    "version": "0.2.2"
+    "version": "0.2.3"
 }
```

### Comparing `jupytercad-0.2.2/packages/jupytercad-app/tsconfig.tsbuildinfo` & `jupytercad-0.2.3/packages/jupytercad-app/tsconfig.tsbuildinfo`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-app/webpack.config.js` & `jupytercad-0.2.3/packages/jupytercad-app/webpack.config.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-app/build/main.js` & `jupytercad-0.2.3/packages/jupytercad-app/build/main.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-app/build/style.js` & `jupytercad-0.2.3/packages/jupytercad-app/build/style.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-app/build/app/app.d.ts` & `jupytercad-0.2.3/packages/jupytercad-app/build/app/app.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-app/build/app/app.js` & `jupytercad-0.2.3/packages/jupytercad-app/build/app/app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-app/build/app/plugins/browser/index.js` & `jupytercad-0.2.3/packages/jupytercad-app/build/app/plugins/browser/index.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-app/build/app/plugins/launcher/index.js` & `jupytercad-0.2.3/packages/jupytercad-app/build/app/plugins/launcher/index.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-app/build/app/plugins/mainmenu/index.js` & `jupytercad-0.2.3/packages/jupytercad-app/build/app/plugins/mainmenu/index.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-app/build/app/plugins/mainmenu/menuWidget.js` & `jupytercad-0.2.3/packages/jupytercad-app/build/app/plugins/mainmenu/menuWidget.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-app/build/app/plugins/mainmenu/userWidget.js` & `jupytercad-0.2.3/packages/jupytercad-app/build/app/plugins/mainmenu/userWidget.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-app/lib/main.js` & `jupytercad-0.2.3/packages/jupytercad-app/lib/main.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-app/lib/app/app.d.ts` & `jupytercad-0.2.3/packages/jupytercad-app/lib/app/app.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-app/lib/app/app.js` & `jupytercad-0.2.3/packages/jupytercad-app/lib/app/app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-app/lib/app/plugins/browser/index.js` & `jupytercad-0.2.3/packages/jupytercad-app/lib/app/plugins/browser/index.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-app/lib/app/plugins/launcher/index.js` & `jupytercad-0.2.3/packages/jupytercad-app/lib/app/plugins/launcher/index.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-app/lib/app/plugins/mainmenu/index.js` & `jupytercad-0.2.3/packages/jupytercad-app/lib/app/plugins/mainmenu/index.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-app/lib/app/plugins/mainmenu/menuWidget.js` & `jupytercad-0.2.3/packages/jupytercad-app/lib/app/plugins/mainmenu/menuWidget.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-app/lib/app/plugins/mainmenu/userWidget.js` & `jupytercad-0.2.3/packages/jupytercad-app/lib/app/plugins/mainmenu/userWidget.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-app/src/main.ts` & `jupytercad-0.2.3/packages/jupytercad-app/src/main.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-app/src/app/app.ts` & `jupytercad-0.2.3/packages/jupytercad-app/src/app/app.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-app/src/app/plugins/browser/index.ts` & `jupytercad-0.2.3/packages/jupytercad-app/src/app/plugins/browser/index.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-app/src/app/plugins/launcher/index.ts` & `jupytercad-0.2.3/packages/jupytercad-app/src/app/plugins/launcher/index.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-app/src/app/plugins/mainmenu/index.ts` & `jupytercad-0.2.3/packages/jupytercad-app/src/app/plugins/mainmenu/index.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-app/src/app/plugins/mainmenu/menuWidget.ts` & `jupytercad-0.2.3/packages/jupytercad-app/src/app/plugins/mainmenu/menuWidget.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-app/src/app/plugins/mainmenu/userWidget.tsx` & `jupytercad-0.2.3/packages/jupytercad-app/src/app/plugins/mainmenu/userWidget.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-app/style/base.css` & `jupytercad-0.2.3/packages/jupytercad-app/style/base.css`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/extension.webpack.config.js` & `jupytercad-0.2.3/packages/jupytercad-extension/extension.webpack.config.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/package.json` & `jupytercad-0.2.3/packages/jupytercad-extension/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.974609375%*

 * *Differences: {"'dependencies'": "{'@jupytercad/jupytercad-opencascade': '^0.2.3'}", "'version'": "'0.2.3'"}*

```diff
@@ -6,15 +6,15 @@
         "url": "https://github.com/QuantStack/jupytercad/issues"
     },
     "dependencies": {
         "@deathbeds/jupyterlab-rjsf": "^1.1.0",
         "@jupyter/collaboration": "^1.0.0",
         "@jupyter/docprovider": "^1.0.0",
         "@jupyter/ydoc": "^0.3.4 || ^1.0.2",
-        "@jupytercad/jupytercad-opencascade": "^0.2.2",
+        "@jupytercad/jupytercad-opencascade": "^0.2.3",
         "@jupyterlab/application": "^4.0.0",
         "@jupyterlab/apputils": "^4.0.0",
         "@jupyterlab/coreutils": "^6.0.0",
         "@jupyterlab/docregistry": "^4.0.0",
         "@jupyterlab/filebrowser": "^4.0.0",
         "@jupyterlab/launcher": "^4.0.0",
         "@jupyterlab/mainmenu": "^4.0.0",
@@ -108,9 +108,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.2.2"
+    "version": "0.2.3"
 }
```

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/schema.js` & `jupytercad-0.2.3/packages/jupytercad-extension/schema.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/tsconfig.tsbuildinfo` & `jupytercad-0.2.3/packages/jupytercad-extension/tsconfig.tsbuildinfo`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999729788153913%*

 * *Differences: {"'program'": "{'fileInfos': {insert: [(656, "*

 * *              "'c6a686ed29b723628b47829dfde402f7a550fbe14e8b6b8e0ace806dc6110576')], delete: "*

 * *              '[656]}}'}*

```diff
@@ -11813,15 +11813,15 @@
                 "signature": "b0b2e26f6c0af31421caacaa42d50526b8472ab99c53a2e084623ba38f018cf1",
                 "version": "7d699ee11551656103fc9d2aa490dbba77007338910bfb0d1efa6e2cd95719a8"
             },
             {
                 "signature": "7b2d5be885bc8529df052b09cd46b2d783d292837815f61bbce6ea1c257c99bf",
                 "version": "2b3def2e55b1a604998b3d2b204ff5e64790974fcf9821564ec67222093337d4"
             },
-            "2a142c3e36d8ca6a7893bf1cdd61dc2c652ef3aefdab1a56f907ccf715d91d75",
+            "c6a686ed29b723628b47829dfde402f7a550fbe14e8b6b8e0ace806dc6110576",
             {
                 "signature": "5570335ff6452229406838ff2c0cf08a6736e1e1064d0c4c8dcef0dd0e490592",
                 "version": "4d72f3934a62e515ef8284df1522b9bccc3c2bbc0a8c81329ee5c11ba9300e1f"
             },
             "9f3c5498245c38c9016a369795ec5ef1768d09db63643c8dba9656e5ab294825",
             "2d225e7bda2871c066a7079c88174340950fb604f624f2586d3ea27bb9e5f4ff",
             "6a785f84e63234035e511817dd48ada756d984dd8f9344e56eb8b2bdcd8fd001",
```

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/worker.webpack.config.js` & `jupytercad-0.2.3/packages/jupytercad-extension/worker.webpack.config.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/commands.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/commands.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/commands.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/commands.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/factory.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/factory.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/factory.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/factory.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/formdialog.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/formdialog.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/formdialog.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/formdialog.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/index.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/index.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/mainview.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/mainview.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/mainview.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/mainview.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/model.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/model.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/model.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/model.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/tools.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/tools.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/tools.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/tools.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/types.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/types.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/widget.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/widget.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/widget.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/widget.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/worker.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/worker.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/_interface/forms.json` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/_interface/forms.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -289,35 +289,34 @@
                         "type": "number",
                         "description": "Angle of the Placement"
                     }
                 }
             }
         }
     },
-    "Part::Cylinder": {
+    "Part::MultiFuse": {
         "type": "object",
         "required": [
-            "Radius",
-            "Angle",
-            "Height",
+            "Shapes",
+            "Refine",
             "Placement"
         ],
         "additionalProperties": false,
         "properties": {
-            "Radius": {
-                "type": "number",
-                "description": "Radius of the cylinder"
-            },
-            "Height": {
-                "type": "number",
-                "description": "Height of the cylinder"
+            "Shapes": {
+                "type": "array",
+                "description": "The shapes of the individual elements",
+                "fcType": "App::PropertyLinkList",
+                "items": {
+                    "type": "string"
+                }
             },
-            "Angle": {
-                "type": "number",
-                "description": "Angle of the cylinder"
+            "Refine": {
+                "type": "boolean",
+                "description": "Refine shape"
             },
             "Placement": {
                 "type": "object",
                 "description": "Placement of the box",
                 "additionalProperties": false,
                 "required": [
                     "Position",
@@ -343,34 +342,49 @@
                         "type": "number",
                         "description": "Angle of the Placement"
                     }
                 }
             }
         }
     },
-    "Part::MultiFuse": {
+    "Part::Extrusion": {
         "type": "object",
         "required": [
-            "Shapes",
-            "Refine",
+            "Base",
+            "Dir",
+            "LengthFwd",
+            "LengthRev",
+            "Solid",
             "Placement"
         ],
         "additionalProperties": false,
         "properties": {
-            "Shapes": {
+            "Base": {
+                "type": "string",
+                "description": "Shape to extrude",
+                "fcType": "App::PropertyLink"
+            },
+            "Dir": {
                 "type": "array",
-                "description": "The shapes of the individual elements",
-                "fcType": "App::PropertyLinkList",
+                "description": "Direction of extrusion",
                 "items": {
-                    "type": "string"
+                    "type": "number"
                 }
             },
-            "Refine": {
+            "LengthFwd": {
+                "type": "number",
+                "description": "Length of extrusion along the direction"
+            },
+            "LengthRev": {
+                "type": "number",
+                "description": "Length of extrusion against the direction"
+            },
+            "Solid": {
                 "type": "boolean",
-                "description": "Refine shape"
+                "description": "If true, creating a solid"
             },
             "Placement": {
                 "type": "object",
                 "description": "Placement of the box",
                 "additionalProperties": false,
                 "required": [
                     "Position",
@@ -396,49 +410,35 @@
                         "type": "number",
                         "description": "Angle of the Placement"
                     }
                 }
             }
         }
     },
-    "Part::Extrusion": {
+    "Part::Cylinder": {
         "type": "object",
         "required": [
-            "Base",
-            "Dir",
-            "LengthFwd",
-            "LengthRev",
-            "Solid",
+            "Radius",
+            "Angle",
+            "Height",
             "Placement"
         ],
         "additionalProperties": false,
         "properties": {
-            "Base": {
-                "type": "string",
-                "description": "Shape to extrude",
-                "fcType": "App::PropertyLink"
-            },
-            "Dir": {
-                "type": "array",
-                "description": "Direction of extrusion",
-                "items": {
-                    "type": "number"
-                }
-            },
-            "LengthFwd": {
+            "Radius": {
                 "type": "number",
-                "description": "Length of extrusion along the direction"
+                "description": "Radius of the cylinder"
             },
-            "LengthRev": {
+            "Height": {
                 "type": "number",
-                "description": "Length of extrusion against the direction"
+                "description": "Height of the cylinder"
             },
-            "Solid": {
-                "type": "boolean",
-                "description": "If true, creating a solid"
+            "Angle": {
+                "type": "number",
+                "description": "Angle of the cylinder"
             },
             "Placement": {
                 "type": "object",
                 "description": "Placement of the box",
                 "additionalProperties": false,
                 "required": [
                     "Position",
```

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/annotation/message.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/annotation/message.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/annotation/model.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/annotation/model.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/annotation/model.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/annotation/model.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/annotation/view.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/annotation/view.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/fcplugin/modelfactory.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/fcplugin/modelfactory.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/fcplugin/modelfactory.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/fcplugin/modelfactory.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/fcplugin/plugins.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/fcplugin/plugins.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/jcadplugin/modelfactory.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/jcadplugin/modelfactory.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/jcadplugin/modelfactory.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/jcadplugin/modelfactory.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/jcadplugin/plugins.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/jcadplugin/plugins.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/notebookrenderer/index.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/notebookrenderer/index.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/notebookrenderer/model.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/notebookrenderer/model.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/notebookrenderer/model.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/notebookrenderer/model.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/notebookrenderer/token.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/notebookrenderer/token.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/notebookrenderer/view.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/notebookrenderer/view.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/notebookrenderer/view.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/notebookrenderer/view.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/notebookrenderer/widgetManager.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/notebookrenderer/widgetManager.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/notebookrenderer/widgetManager.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/notebookrenderer/widgetManager.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/notebookrenderer/yCommProvider.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/notebookrenderer/yCommProvider.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/notebookrenderer/yCommProvider.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/notebookrenderer/yCommProvider.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/panelview/annotations.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/panelview/annotations.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/panelview/annotations.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/panelview/annotations.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/panelview/formbuilder.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/panelview/formbuilder.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/panelview/formbuilder.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/panelview/formbuilder.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/panelview/leftpanel.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/panelview/leftpanel.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/panelview/leftpanel.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/panelview/leftpanel.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/panelview/model.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/panelview/model.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/panelview/model.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/panelview/model.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/panelview/objectproperties.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/panelview/objectproperties.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/panelview/objecttree.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/panelview/objecttree.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/panelview/rightpanel.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/panelview/rightpanel.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/schema/box.json` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/schema/box.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/schema/cone.json` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/schema/cone.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/schema/cut.json` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/schema/cut.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/schema/cylinder.json` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/schema/cylinder.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/schema/extrusion.json` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/schema/extrusion.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/schema/fuse.json` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/schema/fuse.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/schema/geomCircle.json` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/schema/geomCircle.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/schema/geomLineSegment.json` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/schema/geomLineSegment.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/schema/intersection.json` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/schema/intersection.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/schema/jcad.json` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/schema/jcad.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/schema/placement.json` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/schema/placement.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/schema/sketch.json` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/schema/sketch.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/schema/sphere.json` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/schema/sphere.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/schema/torus.json` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/schema/torus.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/sketcher/helper.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/sketcher/helper.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/sketcher/helper.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/sketcher/helper.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/sketcher/panzoom.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/sketcher/panzoom.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/sketcher/sketcherdialog.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/sketcher/sketcherdialog.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/sketcher/sketchermodel.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/sketcher/sketchermodel.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/sketcher/sketchermodel.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/sketcher/sketchermodel.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/sketcher/sketcherwidget.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/sketcher/sketcherwidget.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/sketcher/sketcherwidget.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/sketcher/sketcherwidget.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/sketcher/types.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/sketcher/types.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/toolbar/usertoolbaritem.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/toolbar/usertoolbaritem.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/toolbar/usertoolbaritem.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/toolbar/usertoolbaritem.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/toolbar/widget.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/toolbar/widget.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/toolbar/widget.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/toolbar/widget.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/worker/actions.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/worker/actions.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/worker/actions.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/worker/actions.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/worker/occapi.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/worker/occapi.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/worker/occapi.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/worker/occapi.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/worker/occparser.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/worker/occparser.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/worker/occparser.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/worker/occparser.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/worker/operatorcache.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/worker/operatorcache.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/worker/types.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/worker/types.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/worker/worker.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/worker/worker.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/lib/worker/geometry/geomCircle.js` & `jupytercad-0.2.3/packages/jupytercad-extension/lib/worker/geometry/geomCircle.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/commands.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/commands.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/factory.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/factory.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/formdialog.tsx` & `jupytercad-0.2.3/packages/jupytercad-extension/src/formdialog.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/index.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/mainview.tsx` & `jupytercad-0.2.3/packages/jupytercad-extension/src/mainview.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/model.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/model.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/tools.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/tools.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/types.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/types.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/widget.tsx` & `jupytercad-0.2.3/packages/jupytercad-extension/src/widget.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/_interface/box.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/_interface/box.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/_interface/cone.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/_interface/cone.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/_interface/cut.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/_interface/cut.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/_interface/cylinder.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/_interface/cylinder.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/_interface/extrusion.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/_interface/extrusion.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/_interface/forms.json` & `jupytercad-0.2.3/packages/jupytercad-extension/src/_interface/forms.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -289,35 +289,34 @@
                         "type": "number",
                         "description": "Angle of the Placement"
                     }
                 }
             }
         }
     },
-    "Part::Cylinder": {
+    "Part::MultiFuse": {
         "type": "object",
         "required": [
-            "Radius",
-            "Angle",
-            "Height",
+            "Shapes",
+            "Refine",
             "Placement"
         ],
         "additionalProperties": false,
         "properties": {
-            "Radius": {
-                "type": "number",
-                "description": "Radius of the cylinder"
-            },
-            "Height": {
-                "type": "number",
-                "description": "Height of the cylinder"
+            "Shapes": {
+                "type": "array",
+                "description": "The shapes of the individual elements",
+                "fcType": "App::PropertyLinkList",
+                "items": {
+                    "type": "string"
+                }
             },
-            "Angle": {
-                "type": "number",
-                "description": "Angle of the cylinder"
+            "Refine": {
+                "type": "boolean",
+                "description": "Refine shape"
             },
             "Placement": {
                 "type": "object",
                 "description": "Placement of the box",
                 "additionalProperties": false,
                 "required": [
                     "Position",
@@ -343,34 +342,49 @@
                         "type": "number",
                         "description": "Angle of the Placement"
                     }
                 }
             }
         }
     },
-    "Part::MultiFuse": {
+    "Part::Extrusion": {
         "type": "object",
         "required": [
-            "Shapes",
-            "Refine",
+            "Base",
+            "Dir",
+            "LengthFwd",
+            "LengthRev",
+            "Solid",
             "Placement"
         ],
         "additionalProperties": false,
         "properties": {
-            "Shapes": {
+            "Base": {
+                "type": "string",
+                "description": "Shape to extrude",
+                "fcType": "App::PropertyLink"
+            },
+            "Dir": {
                 "type": "array",
-                "description": "The shapes of the individual elements",
-                "fcType": "App::PropertyLinkList",
+                "description": "Direction of extrusion",
                 "items": {
-                    "type": "string"
+                    "type": "number"
                 }
             },
-            "Refine": {
+            "LengthFwd": {
+                "type": "number",
+                "description": "Length of extrusion along the direction"
+            },
+            "LengthRev": {
+                "type": "number",
+                "description": "Length of extrusion against the direction"
+            },
+            "Solid": {
                 "type": "boolean",
-                "description": "Refine shape"
+                "description": "If true, creating a solid"
             },
             "Placement": {
                 "type": "object",
                 "description": "Placement of the box",
                 "additionalProperties": false,
                 "required": [
                     "Position",
@@ -396,49 +410,35 @@
                         "type": "number",
                         "description": "Angle of the Placement"
                     }
                 }
             }
         }
     },
-    "Part::Extrusion": {
+    "Part::Cylinder": {
         "type": "object",
         "required": [
-            "Base",
-            "Dir",
-            "LengthFwd",
-            "LengthRev",
-            "Solid",
+            "Radius",
+            "Angle",
+            "Height",
             "Placement"
         ],
         "additionalProperties": false,
         "properties": {
-            "Base": {
-                "type": "string",
-                "description": "Shape to extrude",
-                "fcType": "App::PropertyLink"
-            },
-            "Dir": {
-                "type": "array",
-                "description": "Direction of extrusion",
-                "items": {
-                    "type": "number"
-                }
-            },
-            "LengthFwd": {
+            "Radius": {
                 "type": "number",
-                "description": "Length of extrusion along the direction"
+                "description": "Radius of the cylinder"
             },
-            "LengthRev": {
+            "Height": {
                 "type": "number",
-                "description": "Length of extrusion against the direction"
+                "description": "Height of the cylinder"
             },
-            "Solid": {
-                "type": "boolean",
-                "description": "If true, creating a solid"
+            "Angle": {
+                "type": "number",
+                "description": "Angle of the cylinder"
             },
             "Placement": {
                 "type": "object",
                 "description": "Placement of the box",
                 "additionalProperties": false,
                 "required": [
                     "Position",
```

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/_interface/fuse.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/_interface/fuse.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/_interface/geomCircle.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/_interface/geomCircle.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/_interface/geomLineSegment.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/_interface/geomLineSegment.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/_interface/intersection.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/_interface/intersection.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/_interface/jcad.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/_interface/jcad.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/_interface/sketch.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/_interface/sketch.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/_interface/sphere.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/_interface/sphere.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/_interface/torus.d.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/_interface/torus.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/annotation/message.tsx` & `jupytercad-0.2.3/packages/jupytercad-extension/src/annotation/message.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/annotation/model.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/annotation/model.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/annotation/view.tsx` & `jupytercad-0.2.3/packages/jupytercad-extension/src/annotation/view.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/fcplugin/modelfactory.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/fcplugin/modelfactory.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/fcplugin/plugins.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/fcplugin/plugins.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/jcadplugin/modelfactory.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/jcadplugin/modelfactory.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/jcadplugin/plugins.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/jcadplugin/plugins.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/notebookrenderer/index.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/notebookrenderer/index.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/notebookrenderer/model.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/notebookrenderer/model.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/notebookrenderer/token.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/notebookrenderer/token.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/notebookrenderer/view.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/notebookrenderer/view.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/notebookrenderer/widgetManager.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/notebookrenderer/widgetManager.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/notebookrenderer/yCommProvider.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/notebookrenderer/yCommProvider.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/panelview/annotations.tsx` & `jupytercad-0.2.3/packages/jupytercad-extension/src/panelview/annotations.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/panelview/formbuilder.tsx` & `jupytercad-0.2.3/packages/jupytercad-extension/src/panelview/formbuilder.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/panelview/leftpanel.tsx` & `jupytercad-0.2.3/packages/jupytercad-extension/src/panelview/leftpanel.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/panelview/model.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/panelview/model.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/panelview/objectproperties.tsx` & `jupytercad-0.2.3/packages/jupytercad-extension/src/panelview/objectproperties.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/panelview/objecttree.tsx` & `jupytercad-0.2.3/packages/jupytercad-extension/src/panelview/objecttree.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/panelview/rightpanel.tsx` & `jupytercad-0.2.3/packages/jupytercad-extension/src/panelview/rightpanel.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/schema/box.json` & `jupytercad-0.2.3/packages/jupytercad-extension/src/schema/box.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/schema/cone.json` & `jupytercad-0.2.3/packages/jupytercad-extension/src/schema/cone.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/schema/cut.json` & `jupytercad-0.2.3/packages/jupytercad-extension/src/schema/cut.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/schema/cylinder.json` & `jupytercad-0.2.3/packages/jupytercad-extension/src/schema/cylinder.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/schema/extrusion.json` & `jupytercad-0.2.3/packages/jupytercad-extension/src/schema/extrusion.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/schema/fuse.json` & `jupytercad-0.2.3/packages/jupytercad-extension/src/schema/fuse.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/schema/geomCircle.json` & `jupytercad-0.2.3/packages/jupytercad-extension/src/schema/geomCircle.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/schema/geomLineSegment.json` & `jupytercad-0.2.3/packages/jupytercad-extension/src/schema/geomLineSegment.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/schema/intersection.json` & `jupytercad-0.2.3/packages/jupytercad-extension/src/schema/intersection.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/schema/jcad.json` & `jupytercad-0.2.3/packages/jupytercad-extension/src/schema/jcad.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/schema/placement.json` & `jupytercad-0.2.3/packages/jupytercad-extension/src/schema/placement.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/schema/sketch.json` & `jupytercad-0.2.3/packages/jupytercad-extension/src/schema/sketch.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/schema/sphere.json` & `jupytercad-0.2.3/packages/jupytercad-extension/src/schema/sphere.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/schema/torus.json` & `jupytercad-0.2.3/packages/jupytercad-extension/src/schema/torus.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/sketcher/helper.tsx` & `jupytercad-0.2.3/packages/jupytercad-extension/src/sketcher/helper.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/sketcher/panzoom.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/sketcher/panzoom.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/sketcher/sketcherdialog.tsx` & `jupytercad-0.2.3/packages/jupytercad-extension/src/sketcher/sketcherdialog.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/sketcher/sketchermodel.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/sketcher/sketchermodel.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/sketcher/sketcherwidget.tsx` & `jupytercad-0.2.3/packages/jupytercad-extension/src/sketcher/sketcherwidget.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/sketcher/types.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/sketcher/types.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/sketcher/elements/line.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/sketcher/elements/line.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/toolbar/usertoolbaritem.tsx` & `jupytercad-0.2.3/packages/jupytercad-extension/src/toolbar/usertoolbaritem.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/toolbar/widget.tsx` & `jupytercad-0.2.3/packages/jupytercad-extension/src/toolbar/widget.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/worker/actions.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/worker/actions.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/worker/occapi.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/worker/occapi.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/worker/occparser.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/worker/occparser.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/worker/operatorcache.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/worker/operatorcache.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/worker/types.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/worker/types.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/worker/worker.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/worker/worker.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/src/worker/geometry/geomCircle.ts` & `jupytercad-0.2.3/packages/jupytercad-extension/src/worker/geometry/geomCircle.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/style/base.css` & `jupytercad-0.2.3/packages/jupytercad-extension/style/base.css`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/style/icon/axes.svg` & `jupytercad-0.2.3/packages/jupytercad-extension/style/icon/axes.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/style/icon/box.svg` & `jupytercad-0.2.3/packages/jupytercad-extension/style/icon/box.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/style/icon/cone.svg` & `jupytercad-0.2.3/packages/jupytercad-extension/style/icon/cone.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/style/icon/cut.svg` & `jupytercad-0.2.3/packages/jupytercad-extension/style/icon/cut.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/style/icon/cylinder.svg` & `jupytercad-0.2.3/packages/jupytercad-extension/style/icon/cylinder.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/style/icon/extrusion.svg` & `jupytercad-0.2.3/packages/jupytercad-extension/style/icon/extrusion.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/style/icon/intersection.svg` & `jupytercad-0.2.3/packages/jupytercad-extension/style/icon/intersection.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/style/icon/jvcontrol.svg` & `jupytercad-0.2.3/packages/jupytercad-extension/style/icon/jvcontrol.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/style/icon/sphere.svg` & `jupytercad-0.2.3/packages/jupytercad-extension/style/icon/sphere.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/style/icon/torus.svg` & `jupytercad-0.2.3/packages/jupytercad-extension/style/icon/torus.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/style/icon/union.svg` & `jupytercad-0.2.3/packages/jupytercad-extension/style/icon/union.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/style/icon/visibility.svg` & `jupytercad-0.2.3/packages/jupytercad-extension/style/icon/visibility.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-extension/style/icon/visibilityOff.svg` & `jupytercad-0.2.3/packages/jupytercad-extension/style/icon/visibilityOff.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-opencascade/build.yml` & `jupytercad-0.2.3/packages/jupytercad-opencascade/build.yml`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-opencascade/build_opencascade.js` & `jupytercad-0.2.3/packages/jupytercad-opencascade/build_opencascade.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-opencascade/package.json` & `jupytercad-0.2.3/packages/jupytercad-opencascade/package.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'version'": "'0.2.3'"}*

```diff
@@ -33,9 +33,9 @@
     "scripts": {
         "build": "node build_opencascade.js",
         "build:prod": "node build_opencascade.js",
         "clean": "rimraf ./lib",
         "clean:all": "rimraf ./lib"
     },
     "types": "lib/jupytercad.opencascade.d.ts",
-    "version": "0.2.2"
+    "version": "0.2.3"
 }
```

### Comparing `jupytercad-0.2.2/packages/jupytercad-opencascade/lib/build.yml` & `jupytercad-0.2.3/packages/jupytercad-opencascade/lib/build.yml`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-opencascade/lib/jupytercad.opencascade.d.ts` & `jupytercad-0.2.3/packages/jupytercad-opencascade/lib/jupytercad.opencascade.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-opencascade/lib/jupytercad.opencascade.js` & `jupytercad-0.2.3/packages/jupytercad-opencascade/lib/jupytercad.opencascade.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/packages/jupytercad-opencascade/lib/jupytercad.opencascade.wasm` & `jupytercad-0.2.3/packages/jupytercad-opencascade/lib/jupytercad.opencascade.wasm`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/.gitignore` & `jupytercad-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/LICENSE` & `jupytercad-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/README.md` & `jupytercad-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `jupytercad-0.2.2/pyproject.toml` & `jupytercad-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 [project]
 name = "jupytercad"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 dependencies = [
     "jupyter_server>=2.0.6",
+    "jupyterlab>=4,<5",
     "jupyter_collaboration>=1.0.0a9,<2",
     "ypywidgets>=0.1.2,<0.2.0",
     "comm>=0.1.2,<0.2.0",
     "pydantic",
 ]
 classifiers = [
     "License :: OSI Approved :: BSD License",
```

### Comparing `jupytercad-0.2.2/PKG-INFO` & `jupytercad-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupytercad
-Version: 0.2.2
+Version: 0.2.3
 Summary: A JupyterLab extension for 3D modelling.
 Project-URL: Homepage, https://github.com/QuantStack/jupytercad
 Project-URL: Bug Tracker, https://github.com/QuantStack/jupytercad/issues
 Project-URL: Repository, https://github.com/QuantStack/jupytercad.git
 Author: JupyterCad contributors
 License: BSD 3-Clause License
         
@@ -49,14 +49,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Requires-Dist: comm<0.2.0,>=0.1.2
 Requires-Dist: jupyter-collaboration<2,>=1.0.0a9
 Requires-Dist: jupyter-server>=2.0.6
+Requires-Dist: jupyterlab<5,>=4
 Requires-Dist: pydantic
 Requires-Dist: ypywidgets<0.2.0,>=0.1.2
 Description-Content-Type: text/markdown
 
 # JupyterCAD - A JupyterLab extension for 3D geometry modeling.
 
 JupyterCAD is a JupyterLab extension for 3D geometry modeling with collaborative editing support. It is designed to allow multiple people to work on the same file at the same time, and to facilitate discussion and collaboration around the 3D shapes being created.
```

