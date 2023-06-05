# Comparing `tmp/dallinger-9.7.0.tar.gz` & `tmp/dallinger-9.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dallinger-9.7.0.tar", last modified: Thu Apr 27 20:42:48 2023, max compression
+gzip compressed data, was "dallinger-9.8.0.tar", last modified: Mon Jun  5 06:09:37 2023, max compression
```

## Comparing `dallinger-9.7.0.tar` & `dallinger-9.8.0.tar`

### file list

```diff
@@ -1,274 +1,274 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.637323 dallinger-9.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-27 20:41:50.000000 dallinger-9.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-27 20:41:50.000000 dallinger-9.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-27 20:42:48.637323 dallinger-9.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-27 20:41:50.000000 dallinger-9.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-27 20:42:41.000000 dallinger-9.7.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12319 2023-04-27 20:41:50.000000 dallinger-9.7.0/constraints.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.553322 dallinger-9.7.0/dallinger/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/bots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.561322 dallinger-9.7.0/dallinger/command_line/
--rwxr-xr-x   0 runner    (1001) docker     (123)    30603 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/command_line/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24511 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/command_line/appdirs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/command_line/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/command_line/develop.py
--rw-r--r--   0 runner    (1001) docker     (123)    18044 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/command_line/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)    26720 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/command_line/docker_ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/command_line/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    14107 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14038 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.561322 dallinger-9.7.0/dallinger/default_configs/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/default_configs/.dallingerconfig
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/default_configs/global_config_defaults.txt
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/default_configs/local_config_defaults.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20250 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/deployment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.561322 dallinger-9.7.0/dallinger/dev_server/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/dev_server/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/dev_server/run.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.565322 dallinger-9.7.0/dallinger/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/docker/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/docker/docker-compose.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/docker/heroku.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      417 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/docker/prepare_docker_image.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.565322 dallinger-9.7.0/dallinger/docker/ssh_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/docker/ssh_templates/docker-compose-experiment.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/docker/ssh_templates/docker-compose-server.yml
--rw-r--r--   0 runner    (1001) docker     (123)    13935 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/docker/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/docker/wheel_filename.py
--rw-r--r--   0 runner    (1001) docker     (123)    60122 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.569322 dallinger-9.7.0/dallinger/experiment_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/experiment_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28025 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/experiment_server/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    58202 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/experiment_server/experiment_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/experiment_server/gunicorn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/experiment_server/replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/experiment_server/sockets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/experiment_server/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/experiment_server/worker_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.569322 dallinger-9.7.0/dallinger/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/experiments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.533321 dallinger-9.7.0/dallinger/frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.569322 dallinger-9.7.0/dallinger/frontend/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.569322 dallinger-9.7.0/dallinger/frontend/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)   160403 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/css/dallinger.css
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/css/dashboard.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.569322 dallinger-9.7.0/dallinger/frontend/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.577322 dallinger-9.7.0/dallinger/frontend/static/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    60174 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/scripts/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/scripts/clipboard.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    24886 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/scripts/dallinger2.js
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/scripts/dallinger2.test.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.533321 dallinger-9.7.0/dallinger/frontend/static/scripts/fingerprintjs2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.577322 dallinger-9.7.0/dallinger/frontend/static/scripts/fingerprintjs2/1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34376 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/scripts/fingerprintjs2/1.5.1/fingerprint2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/scripts/jquery-3.6.0.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    21814 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/scripts/network-monitor.js
--rw-r--r--   0 runner    (1001) docker     (123)    21257 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/scripts/popper.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/scripts/reconnecting-websocket.js
--rw-r--r--   0 runner    (1001) docker     (123)    17738 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/scripts/require.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     9342 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/scripts/reqwest.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/scripts/spin.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/scripts/store+json2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    36956 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/scripts/tracker.js
--rw-r--r--   0 runner    (1001) docker     (123)    44433 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/scripts/tracker.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.577322 dallinger-9.7.0/dallinger/frontend/static/scripts/tracking/
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/scripts/tracking/load-tracker.js
--rw-r--r--   0 runner    (1001) docker     (123)    29161 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/scripts/tracking/scribe-analytics.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/scripts/tracking/scribe-console.js
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/scripts/tracking/scribe-dallinger.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.533321 dallinger-9.7.0/dallinger/frontend/static/vis@4.17.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.577322 dallinger-9.7.0/dallinger/frontend/static/vis@4.17.0/dist/
--rw-r--r--   0 runner    (1001) docker     (123)    15046 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/vis@4.17.0/dist/vis-network.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   635830 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/vis@4.17.0/dist/vis.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.585322 dallinger-9.7.0/dallinger/frontend/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.589322 dallinger-9.7.0/dallinger/frontend/templates/base/
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/base/ad.html
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/base/consent.html
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/base/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/base/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/base/questionnaire.html
--rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/dashboard_database.html
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/dashboard_develop.html
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/dashboard_heroku.html
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/dashboard_home.html
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/dashboard_lifecycle.html
--rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/dashboard_monitor.html
--rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/dashboard_mturk.html
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/error-complete.html
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/exit_recruiter.html
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/exit_recruiter_mturk.html
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/exit_recruiter_prolific.html
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/launch.html
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/questionnaire.html
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/waiting.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.589322 dallinger-9.7.0/dallinger/heroku/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/heroku/Procfile
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/heroku/Procfile_no_clock
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/heroku/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/heroku/clock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/heroku/rq_gevent_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    20061 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/heroku/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/heroku/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/information.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/logging.ini
--rw-r--r--   0 runner    (1001) docker     (123)    68520 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    28478 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/mturk.py
--rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/networks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/processes.py
--rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/prolific.py
--rw-r--r--   0 runner    (1001) docker     (123)    20456 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/pytest_dallinger.py
--rw-r--r--   0 runner    (1001) docker     (123)    64023 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/recruiters.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/redis_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)    32799 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.557322 dallinger-9.7.0/dallinger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-27 20:42:48.000000 dallinger-9.7.0/dallinger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-04-27 20:42:48.000000 dallinger-9.7.0/dallinger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 20:42:48.000000 dallinger-9.7.0/dallinger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-27 20:42:48.000000 dallinger-9.7.0/dallinger.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 20:42:48.000000 dallinger-9.7.0/dallinger.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-27 20:42:48.000000 dallinger-9.7.0/dallinger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-27 20:42:48.000000 dallinger-9.7.0/dallinger.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.593322 dallinger-9.7.0/dallinger_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger_scripts/clock.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger_scripts/web.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger_scripts/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    12324 2023-04-27 20:41:50.000000 dallinger-9.7.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.593322 dallinger-9.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.609323 dallinger-9.7.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.621323 dallinger-9.7.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    20033 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/AvenirLTStd-Book_gdi.eot
--rw-r--r--   0 runner    (1001) docker     (123)    62093 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/AvenirLTStd-Book_gdi.svg
--rw-r--r--   0 runner    (1001) docker     (123)    46176 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/AvenirLTStd-Book_gdi.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    23000 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/AvenirLTStd-Book_gdi.woff
--rw-r--r--   0 runner    (1001) docker     (123)   335782 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/Dallinger AWS Group.png
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/barplot.png
--rw-r--r--   0 runner    (1001) docker     (123)    21280 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/burst.png
--rw-r--r--   0 runner    (1001) docker     (123)    11068 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/chain.png
--rw-r--r--   0 runner    (1001) docker     (123)   317968 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/class_chart.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    32421 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/corner.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)    44987 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/delayed.png
--rw-r--r--   0 runner    (1001) docker     (123)   419192 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/directories.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    19688 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/empty.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   235602 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/front_back_layout.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    55137 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/full.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     9193 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/grid.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     6231 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/grid_mini.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     8152 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/grid_small.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    91384 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/heroku.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    21947 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/star.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.621323 dallinger-9.7.0/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/acknowledgments.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/aws_etc_keys.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/build_demo_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/building_documentation.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15176 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/command_line_utility.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/communicating_with_the_server.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12384 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    19287 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/contributing_to_dallinger.rst
--rw-r--r--   0 runner    (1001) docker     (123)    61118 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/creating_an_experiment.rst
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/dallinger_the_scientist.rst
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/demo_index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/demoing_dallinger.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/demos_on_heroku.rst
--rw-r--r--   0 runner    (1001) docker     (123)    21478 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/developing_dallinger_setup_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/docker_only.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/docker_support.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/docker_tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/email_setup.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/experiment_data.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/extra_configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17494 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/installing_dallinger_for_users.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/javascript_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/learning_to_use_dallinger.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/monitoring_a_live_experiment.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14663 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/networks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/postico_and_postgres.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/private_repo.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/python_module.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/recruitment.rst
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/registration_on_OSF.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/required_experiment_files.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/rewarding_participants.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/running_bots.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/running_the_tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/scheduled_tasks.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.621323 dallinger-9.7.0/docs/source/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/schemas/info.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/schemas/network.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/schemas/node.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/schemas/notification.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/schemas/participant.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/schemas/transformation.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/schemas/transmission.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/schemas/vector.csvs
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/the_experiment_class.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/troubleshooting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/vagrant_setup.rst
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/waiting_rooms.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/web_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/writing_bots.rst
--rw-r--r--   0 runner    (1001) docker     (123)    85530 2023-04-27 20:41:50.000000 dallinger-9.7.0/incubator.png
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-04-27 20:41:50.000000 dallinger-9.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-27 20:42:48.637323 dallinger-9.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-27 20:41:50.000000 dallinger-9.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.637323 dallinger-9.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_bots.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_cli_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    40472 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_command_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    38988 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    13889 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_demos.py
--rw-r--r--   0 runner    (1001) docker     (123)    42400 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_environments.py
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    77379 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_experiment_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_griduniverse.py
--rw-r--r--   0 runner    (1001) docker     (123)    24865 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_heroku.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_local_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    28921 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    50155 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_mturk.py
--rw-r--r--   0 runner    (1001) docker     (123)    23282 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_networks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_prolific.py
--rw-r--r--   0 runner    (1001) docker     (123)    57519 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_recruiters.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_replay_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_sockets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.797674 dallinger-9.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-05 06:08:49.000000 dallinger-9.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-05 06:08:49.000000 dallinger-9.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-05 06:09:37.797674 dallinger-9.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-05 06:08:49.000000 dallinger-9.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-05 06:09:31.000000 dallinger-9.8.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12304 2023-06-05 06:08:49.000000 dallinger-9.8.0/constraints.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.773674 dallinger-9.8.0/dallinger/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12262 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/bots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.773674 dallinger-9.8.0/dallinger/command_line/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30603 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/command_line/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24511 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/command_line/appdirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/command_line/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/command_line/develop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18044 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/command_line/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26878 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/command_line/docker_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/command_line/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14108 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14038 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.773674 dallinger-9.8.0/dallinger/default_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/default_configs/.dallingerconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/default_configs/global_config_defaults.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/default_configs/local_config_defaults.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20250 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/deployment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.773674 dallinger-9.8.0/dallinger/dev_server/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/dev_server/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/dev_server/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.777674 dallinger-9.8.0/dallinger/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/docker/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/docker/docker-compose.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/docker/heroku.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      417 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/docker/prepare_docker_image.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.777674 dallinger-9.8.0/dallinger/docker/ssh_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/docker/ssh_templates/docker-compose-experiment.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/docker/ssh_templates/docker-compose-server.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    14085 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/docker/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/docker/wheel_filename.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60122 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.777674 dallinger-9.8.0/dallinger/experiment_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/experiment_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28025 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/experiment_server/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58487 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/experiment_server/experiment_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/experiment_server/gunicorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/experiment_server/replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/experiment_server/sockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/experiment_server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/experiment_server/worker_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.777674 dallinger-9.8.0/dallinger/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/experiments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.769674 dallinger-9.8.0/dallinger/frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.777674 dallinger-9.8.0/dallinger/frontend/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.777674 dallinger-9.8.0/dallinger/frontend/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   160403 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/css/dallinger.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/css/dashboard.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.777674 dallinger-9.8.0/dallinger/frontend/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.777674 dallinger-9.8.0/dallinger/frontend/static/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    60174 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/scripts/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/scripts/clipboard.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    25872 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/scripts/dallinger2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/scripts/dallinger2.test.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.765674 dallinger-9.8.0/dallinger/frontend/static/scripts/fingerprintjs2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.781674 dallinger-9.8.0/dallinger/frontend/static/scripts/fingerprintjs2/1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34376 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/scripts/fingerprintjs2/1.5.1/fingerprint2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/scripts/jquery-3.6.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21814 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/scripts/network-monitor.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21257 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/scripts/popper.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/scripts/reconnecting-websocket.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17738 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/scripts/require.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9342 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/scripts/reqwest.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/scripts/spin.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/scripts/store+json2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    36956 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/scripts/tracker.js
+-rw-r--r--   0 runner    (1001) docker     (123)    44433 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/scripts/tracker.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.781674 dallinger-9.8.0/dallinger/frontend/static/scripts/tracking/
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/scripts/tracking/load-tracker.js
+-rw-r--r--   0 runner    (1001) docker     (123)    29161 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/scripts/tracking/scribe-analytics.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/scripts/tracking/scribe-console.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/scripts/tracking/scribe-dallinger.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.765674 dallinger-9.8.0/dallinger/frontend/static/vis@4.17.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.781674 dallinger-9.8.0/dallinger/frontend/static/vis@4.17.0/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)    15046 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/vis@4.17.0/dist/vis-network.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   635830 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/vis@4.17.0/dist/vis.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.781674 dallinger-9.8.0/dallinger/frontend/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.781674 dallinger-9.8.0/dallinger/frontend/templates/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/base/ad.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/base/consent.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/base/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/base/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/base/questionnaire.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/dashboard_database.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/dashboard_develop.html
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/dashboard_heroku.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/dashboard_home.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/dashboard_lifecycle.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/dashboard_monitor.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/dashboard_mturk.html
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/error-complete.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/exit_recruiter.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/exit_recruiter_mturk.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/exit_recruiter_prolific.html
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/launch.html
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/questionnaire.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/waiting.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.785674 dallinger-9.8.0/dallinger/heroku/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/heroku/Procfile
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/heroku/Procfile_no_clock
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/heroku/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/heroku/clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/heroku/rq_gevent_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20061 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/heroku/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/heroku/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/logging.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    68521 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28478 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/mturk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/prolific.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20449 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/pytest_dallinger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64023 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/recruiters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/redis_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32914 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.773674 dallinger-9.8.0/dallinger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-05 06:09:37.000000 dallinger-9.8.0/dallinger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-06-05 06:09:37.000000 dallinger-9.8.0/dallinger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 06:09:37.000000 dallinger-9.8.0/dallinger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-05 06:09:37.000000 dallinger-9.8.0/dallinger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 06:09:37.000000 dallinger-9.8.0/dallinger.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-05 06:09:37.000000 dallinger-9.8.0/dallinger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-05 06:09:37.000000 dallinger-9.8.0/dallinger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.785674 dallinger-9.8.0/dallinger_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger_scripts/clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger_scripts/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger_scripts/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-06-05 06:08:49.000000 dallinger-9.8.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.785674 dallinger-9.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.789674 dallinger-9.8.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.793674 dallinger-9.8.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    20033 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/AvenirLTStd-Book_gdi.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    62093 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/AvenirLTStd-Book_gdi.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    46176 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/AvenirLTStd-Book_gdi.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    23000 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/AvenirLTStd-Book_gdi.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   335782 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/Dallinger AWS Group.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/barplot.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21280 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/burst.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11068 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/chain.png
+-rw-r--r--   0 runner    (1001) docker     (123)   317968 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/class_chart.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    32421 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/corner.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)    44987 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/delayed.png
+-rw-r--r--   0 runner    (1001) docker     (123)   419192 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/directories.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    19688 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/empty.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   235602 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/front_back_layout.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    55137 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/full.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9193 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/grid.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6231 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/grid_mini.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8152 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/grid_small.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    91384 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/heroku.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    21947 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/star.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.793674 dallinger-9.8.0/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/acknowledgments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/aws_etc_keys.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/build_demo_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/building_documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15176 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/command_line_utility.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/communicating_with_the_server.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12384 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19287 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/contributing_to_dallinger.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    61118 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/creating_an_experiment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/dallinger_the_scientist.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/demo_index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/demoing_dallinger.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/demos_on_heroku.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    21478 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/developing_dallinger_setup_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/docker_only.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/docker_support.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/docker_tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/email_setup.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/experiment_data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/extra_configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17494 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/installing_dallinger_for_users.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/javascript_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/learning_to_use_dallinger.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/monitoring_a_live_experiment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14663 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/networks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/postico_and_postgres.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/private_repo.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/python_module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/recruitment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/registration_on_OSF.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/required_experiment_files.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/rewarding_participants.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/running_bots.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/running_the_tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/scheduled_tasks.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.793674 dallinger-9.8.0/docs/source/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/schemas/info.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/schemas/network.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/schemas/node.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/schemas/notification.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/schemas/participant.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/schemas/transformation.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/schemas/transmission.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/schemas/vector.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/the_experiment_class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/troubleshooting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/vagrant_setup.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/waiting_rooms.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/web_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/writing_bots.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    85530 2023-06-05 06:08:49.000000 dallinger-9.8.0/incubator.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-06-05 06:08:49.000000 dallinger-9.8.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-05 06:09:37.797674 dallinger-9.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-06-05 06:08:49.000000 dallinger-9.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.797674 dallinger-9.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_bots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_cli_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40486 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38988 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13898 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42171 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77386 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_experiment_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_griduniverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24865 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_heroku.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_local_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28921 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50155 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_mturk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23282 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_prolific.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57519 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_recruiters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_replay_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_sockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_utils.py
```

### Comparing `dallinger-9.7.0/LICENSE` & `dallinger-9.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/PKG-INFO` & `dallinger-9.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: dallinger
-Version: 9.7.0
+Version: 9.8.0
 Summary: Laboratory automation for the behavioral and social sciences
 Home-page: http://github.com/Dallinger/Dallinger
 Maintainer: Jordan Suchow
 Maintainer-email: suchow@berkeley.edu
 License: MIT
 Keywords: science,cultural evolution,experiments,psychology
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Pytest
 Description-Content-Type: text/markdown
 Provides-Extra: jupyter
 Provides-Extra: data
 Provides-Extra: dev
 Provides-Extra: docker
 License-File: LICENSE
```

### Comparing `dallinger-9.7.0/README.md` & `dallinger-9.8.0/README.md`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/README.rst` & `dallinger-9.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/constraints.txt` & `dallinger-9.8.0/constraints.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 
     # via -r constraints.in
 alabaster==0.7.13
     # via
     #   dallinger
     #   sphinx
-anyio==3.6.2
+anyio==3.7.0
     # via jupyter-server
 apscheduler==3.10.1
     # via dallinger
 argon2-cffi==21.3.0
     # via
     #   jupyter-server
     #   nbclassic
@@ -44,33 +44,33 @@
     # via nbconvert
 black==23.3.0
     # via dallinger
 bleach==6.0.0
     # via nbconvert
 blinker==1.6.2
     # via flask
-boto3==1.26.121
+boto3==1.26.146
     # via dallinger
-botocore==1.29.121
+botocore==1.29.146
     # via
     #   boto3
     #   s3transfer
 build==0.10.0
     # via
     #   dallinger
     #   pip-tools
 bump2version==1.0.1
     # via bumpversion
 bumpversion==0.6.0
     # via dallinger
 cached-property==1.5.2
     # via dallinger
-cachetools==5.3.0
+cachetools==5.3.1
     # via tox
-certifi==2022.12.7
+certifi==2023.5.7
     # via
     #   requests
     #   selenium
 cffi==1.15.1
     # via
     #   argon2-cffi-bindings
     #   cryptography
@@ -88,61 +88,62 @@
     #   flask
     #   pip-tools
     #   rq
 colorama==0.4.6
     # via tox
 comm==0.1.3
     # via ipykernel
-coverage==7.2.3
+coverage==7.2.7
     # via
     #   coverage-pth
     #   dallinger
 coverage-pth==0.0.2
     # via dallinger
-cryptography==40.0.2
+cryptography==41.0.1
     # via
     #   paramiko
     #   pyopenssl
 debugpy==1.6.7
     # via ipykernel
 decorator==5.1.1
     # via ipython
 defusedxml==0.7.1
     # via
     #   nbconvert
     #   odfpy
 distlib==0.3.6
     # via virtualenv
-docker==6.0.1
+docker==6.1.3
     # via dallinger
 docutils==0.18.1
     # via
     #   myst-parser
     #   sphinx
     #   sphinx-rtd-theme
 et-xmlfile==1.1.0
     # via openpyxl
 exceptiongroup==1.1.1
     # via
+    #   anyio
     #   pytest
     #   trio
     #   trio-websocket
 executing==1.2.0
     # via stack-data
-faker==18.5.1
+faker==18.10.1
     # via dallinger
-fastjsonschema==2.16.3
+fastjsonschema==2.17.1
     # via nbformat
 filelock==3.12.0
     # via
     #   tox
     #   virtualenv
 flake8==6.0.0
     # via dallinger
-flask==2.3.1
+flask==2.3.2
     # via
     #   dallinger
     #   flask-crossdomain
     #   flask-login
     #   flask-sockets
     #   flask-wtf
 flask-crossdomain==0.1
@@ -171,36 +172,37 @@
     #   sqlalchemy
 gunicorn==20.1.0
     # via dallinger
 h11==0.14.0
     # via wsproto
 heroku3==5.2.1
     # via dallinger
-identify==2.5.23
+identify==2.5.24
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   jsonschema
     #   requests
     #   trio
 imagesize==1.4.1
     # via sphinx
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.22.0
+ipykernel==6.23.1
     # via
     #   ipywidgets
     #   jupyter
     #   jupyter-console
     #   nbclassic
     #   notebook
     #   qtconsole
-ipython==8.12.0
+ipython==8.12.2
     # via
+    #   dallinger
     #   ipykernel
     #   ipywidgets
     #   jupyter-console
 ipython-genutils==0.2.0
     # via
     #   nbclassic
     #   notebook
@@ -261,15 +263,15 @@
     #   nbclient
     #   nbconvert
     #   nbformat
     #   notebook
     #   qtconsole
 jupyter-events==0.6.3
     # via jupyter-server
-jupyter-server==2.5.0
+jupyter-server==2.6.0
     # via
     #   dallinger
     #   nbclassic
     #   notebook-shim
 jupyter-server-terminals==0.4.4
     # via jupyter-server
 jupyterlab-pygments==0.2.2
@@ -280,15 +282,15 @@
     # via dallinger
 markdown-it-py==2.2.0
     # via
     #   mdit-py-plugins
     #   myst-parser
 markuppy==1.14
     # via tablib
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via
     #   jinja2
     #   nbconvert
     #   werkzeug
     #   wtforms
 matplotlib-inline==0.1.6
     # via
@@ -298,56 +300,58 @@
     # via flake8
 mdit-py-plugins==0.3.5
     # via myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mistune==2.0.5
     # via nbconvert
-mock==5.0.0
+mock==5.0.2
     # via dallinger
 mypy-extensions==1.0.0
     # via black
 myst-parser==1.0.0
     # via dallinger
-nbclassic==0.5.5
+nbclassic==1.0.0
     # via notebook
-nbclient==0.7.4
+nbclient==0.8.0
     # via nbconvert
-nbconvert==7.3.1
+nbconvert==7.4.0
     # via
     #   jupyter
     #   jupyter-server
     #   nbclassic
     #   notebook
-nbformat==5.8.0
+nbformat==5.9.0
     # via
     #   jupyter-server
     #   nbclassic
     #   nbclient
     #   nbconvert
     #   notebook
 nest-asyncio==1.5.6
     # via
     #   ipykernel
     #   nbclassic
     #   notebook
-nodeenv==1.7.0
+nodeenv==1.8.0
     # via pre-commit
 notebook==6.5.4
     # via jupyter
 notebook-shim==0.2.3
     # via nbclassic
 numpy==1.24.3
     # via pandas
 odfpy==1.4.1
     # via tablib
 openpyxl==3.1.2
     # via tablib
 outcome==1.2.0
     # via trio
+overrides==7.3.1
+    # via jupyter-server
 packaging==23.1
     # via
     #   black
     #   build
     #   docker
     #   ipykernel
     #   jupyter-server
@@ -355,21 +359,21 @@
     #   pyproject-api
     #   pytest
     #   pytest-rerunfailures
     #   qtconsole
     #   qtpy
     #   sphinx
     #   tox
-pandas==2.0.1
+pandas==2.0.2
     # via
     #   dallinger
     #   tablib
 pandocfilters==1.5.0
     # via nbconvert
-paramiko==3.1.0
+paramiko==3.2.0
     # via
     #   dallinger
     #   sshtunnel
 parso==0.8.3
     # via jedi
 pathspec==0.11.1
     # via black
@@ -377,27 +381,27 @@
     # via
     #   dallinger
     #   ipython
 pickleshare==0.7.5
     # via ipython
 pip-tools==6.13.0
     # via dallinger
-platformdirs==3.4.0
+platformdirs==3.5.1
     # via
     #   black
     #   jupyter-core
     #   tox
     #   virtualenv
 pluggy==1.0.0
     # via
     #   pytest
     #   tox
-pre-commit==3.2.2
+pre-commit==3.3.2
     # via dallinger
-prometheus-client==0.16.0
+prometheus-client==0.17.0
     # via
     #   jupyter-server
     #   nbclassic
     #   notebook
 prompt-toolkit==3.0.38
     # via
     #   ipython
@@ -431,15 +435,15 @@
     #   ipython
     #   jupyter-console
     #   nbconvert
     #   qtconsole
     #   sphinx
 pynacl==1.5.0
     # via paramiko
-pyopenssl==23.1.1
+pyopenssl==23.2.0
     # via dallinger
 pypandoc==1.11
     # via dallinger
 pyproject-api==1.5.1
     # via tox
 pyproject-hooks==1.0.0
     # via build
@@ -463,60 +467,58 @@
     #   pandas
 python-json-logger==2.0.7
     # via jupyter-events
 pytz==2023.3
     # via
     #   apscheduler
     #   pandas
-pytz-deprecation-shim==0.1.0.post0
-    # via tzlocal
 pyyaml==6.0
     # via
     #   jupyter-events
     #   myst-parser
     #   pre-commit
     #   tablib
-pyzmq==25.0.2
+pyzmq==25.1.0
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-console
     #   jupyter-server
     #   nbclassic
     #   notebook
     #   qtconsole
-qtconsole==5.4.2
+qtconsole==5.4.3
     # via jupyter
 qtpy==2.3.1
     # via qtconsole
-redis==4.5.4
+redis==4.5.5
     # via
     #   dallinger
     #   rq
-requests==2.29.0
+requests==2.31.0
     # via
     #   dallinger
     #   docker
     #   heroku3
     #   sphinx
 rfc3339-validator==0.1.4
     # via
     #   jsonschema
     #   jupyter-events
 rfc3986-validator==0.1.1
     # via
     #   jsonschema
     #   jupyter-events
-rq==1.13.0
+rq==1.15.0
     # via dallinger
-s3transfer==0.6.0
+s3transfer==0.6.1
     # via boto3
-selenium==4.9.0
+selenium==4.9.1
     # via dallinger
-send2trash==1.8.0
+send2trash==1.8.2
     # via
     #   jupyter-server
     #   nbclassic
     #   notebook
 six==1.16.0
     # via
     #   apscheduler
@@ -539,15 +541,15 @@
 sphinx==6.2.1
     # via
     #   dallinger
     #   myst-parser
     #   sphinx-rtd-theme
     #   sphinxcontrib-jquery
     #   sphinxcontrib-spelling
-sphinx-rtd-theme==1.2.0
+sphinx-rtd-theme==1.2.1
     # via dallinger
 sphinxcontrib-applehelp==1.0.4
     # via sphinx
 sphinxcontrib-devhelp==1.0.2
     # via sphinx
 sphinxcontrib-htmlhelp==2.0.1
     # via sphinx
@@ -557,15 +559,15 @@
     # via sphinx
 sphinxcontrib-qthelp==1.0.3
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
 sphinxcontrib-spelling==8.0.0
     # via dallinger
-sqlalchemy==1.4.47
+sqlalchemy==1.4.48
     # via
     #   dallinger
     #   sqlalchemy-postgres-copy
 sqlalchemy-postgres-copy==0.5.0
     # via dallinger
 sshtunnel==0.4.0
     # via dallinger
@@ -593,23 +595,23 @@
     # via
     #   black
     #   build
     #   pyproject-api
     #   pyproject-hooks
     #   pytest
     #   tox
-tornado==6.3.1
+tornado==6.3.2
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
     #   nbclassic
     #   notebook
     #   terminado
-tox==4.5.1
+tox==4.5.2
     # via dallinger
 traitlets==5.9.0
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
@@ -628,52 +630,50 @@
 trio==0.22.0
     # via
     #   selenium
     #   trio-websocket
 trio-websocket==0.10.2
     # via selenium
 tzdata==2023.3
-    # via
-    #   pandas
-    #   pytz-deprecation-shim
-tzlocal==4.3
+    # via pandas
+tzlocal==5.0.1
     # via
     #   apscheduler
     #   dallinger
 ua-parser==0.16.1
     # via
     #   dallinger
     #   user-agents
 uri-template==1.2.0
     # via jsonschema
-urllib3==1.26.15
+urllib3==1.26.16
     # via
     #   botocore
     #   docker
     #   requests
     #   selenium
 user-agents==2.2.0
     # via dallinger
-virtualenv==20.22.0
+virtualenv==20.23.0
     # via
     #   pre-commit
     #   tox
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
 webencodings==0.5.1
     # via
     #   bleach
     #   tinycss2
-websocket-client==1.5.1
+websocket-client==1.5.2
     # via
     #   docker
     #   jupyter-server
-werkzeug==2.3.0
+werkzeug==2.3.4
     # via
     #   flask
     #   flask-login
 wheel==0.40.0
     # via pip-tools
 widgetsnbextension==4.0.7
     # via ipywidgets
```

### Comparing `dallinger-9.7.0/dallinger/__init__.py` & `dallinger-9.8.0/dallinger/__init__.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/bots.py` & `dallinger-9.8.0/dallinger/bots.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
             if driver_class is not None:
                 kwargs = {}
                 if driver_type.lower() == "chrome_headless":
                     from selenium.webdriver.chrome.options import Options
 
                     chrome_options = Options()
                     chrome_options.add_argument("--headless")
-                    kwargs = {"chrome_options": chrome_options}
+                    kwargs = {"options": chrome_options}
                 driver = driver_class(**kwargs)
 
         if driver is None:
             raise ValueError("Unsupported webdriver_type: {}".format(driver_type))
 
         driver.set_window_size(1024, 768)
         logger.info("Created {} webdriver.".format(driver_type))
```

### Comparing `dallinger-9.7.0/dallinger/command_line/__init__.py` & `dallinger-9.8.0/dallinger/command_line/__init__.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/command_line/appdirs.py` & `dallinger-9.8.0/dallinger/command_line/appdirs.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/command_line/config.py` & `dallinger-9.8.0/dallinger/command_line/config.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/command_line/develop.py` & `dallinger-9.8.0/dallinger/command_line/develop.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/command_line/docker.py` & `dallinger-9.8.0/dallinger/command_line/docker.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/command_line/docker_ssh.py` & `dallinger-9.8.0/dallinger/command_line/docker_ssh.py`

 * *Files 1% similar despite different names*

```diff
@@ -299,15 +299,16 @@
         BytesIO(CADDYFILE.format(host=dns_host, tls=tls).encode()),
         "dallinger/Caddyfile",
     )
 
     print("Removing any pre-existing app with the same name.")
     app_yml = f"~/dallinger/{app_name}/docker-compose.yml"
     executor.run(
-        f"if [ -f {app_yml} ]; then docker compose -f {app_yml} down --remove-orphans; fi"
+        f"if [ -f {app_yml} ]; then docker compose -f {app_yml} down --remove-orphans; fi",
+        raise_=False,
     )
 
     print("Removing any pre-existing Redis volumes.")
     remove_redis_volumes(app_name, executor)
 
     print("Launching http and postgresql servers.")
     executor.run("docker compose -f ~/dallinger/docker-compose.yml up -d")
@@ -583,32 +584,36 @@
 def get_docker_compose_yml(
     config: Dict[str, str],
     experiment_id: str,
     experiment_image: str,
     postgresql_password: str,
 ) -> str:
     """Generate a docker-compose.yml file based on the given"""
-    docker_volumes = config.get("docker_volumes", "[]")
+    docker_volumes = config.get("docker_volumes", "")
     config_str = {key: re.sub("\\$", "$$", str(value)) for key, value in config.items()}
 
     return DOCKER_COMPOSE_EXP_TPL.render(
         experiment_id=experiment_id,
         experiment_image=experiment_image,
         config=config_str,
         docker_volumes=docker_volumes,
         postgresql_password=postgresql_password,
     )
 
 
 def get_retrying_http_client():
+    parameter_name = "method_whitelist"
+    if hasattr(Retry.DEFAULT, "allowed_methods"):
+        parameter_name = "allowed_methods"
+
     retry_strategy = Retry(
         total=30,
         backoff_factor=0.2,
         status_forcelist=[429, 500, 502, 503, 504],
-        method_whitelist=["POST"],
+        **{parameter_name: ["POST"]},
     )
     adapter = HTTPAdapter(max_retries=retry_strategy)
     http = requests.Session()
     http.mount("https://", adapter)
     http.mount("http://", adapter)
     return http
```

### Comparing `dallinger-9.7.0/dallinger/command_line/utils.py` & `dallinger-9.8.0/dallinger/command_line/utils.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/config.py` & `dallinger-9.8.0/dallinger/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import unicode_literals
 
-import distutils.util
 import io
 import json
 import logging
 import os
 import sys
 from collections import deque
 from contextlib import contextmanager
 from pathlib import Path
 
 import six
+from setuptools.dist import strtobool
 from six.moves import configparser
 
 logger = logging.getLogger(__file__)
 
 marker = object()
 
 LOCAL_CONFIG = "config.txt"
@@ -150,15 +150,15 @@
                 if isinstance(value, six.text_type) and value.startswith("file:"):
                     # Load this value from a file
                     _, filename = value.split(":", 1)
                     with io.open(filename, "rt", encoding="utf-8") as source_file:
                         value = source_file.read()
                 try:
                     if expected_type == bool:
-                        value = distutils.util.strtobool(value)
+                        value = strtobool(value)
                     value = expected_type(value)
                 except ValueError:
                     pass
             if not isinstance(value, expected_type):
                 raise TypeError(
                     "Got {value} for {key}, expected {expected_type}".format(
                         value=repr(value), key=key, expected_type=expected_type
```

### Comparing `dallinger-9.7.0/dallinger/data.py` & `dallinger-9.8.0/dallinger/data.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/db.py` & `dallinger-9.8.0/dallinger/db.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/default_configs/global_config_defaults.txt` & `dallinger-9.8.0/dallinger/default_configs/global_config_defaults.txt`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/deployment.py` & `dallinger-9.8.0/dallinger/deployment.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/dev_server/app.py` & `dallinger-9.8.0/dallinger/dev_server/app.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/docker/deployment.py` & `dallinger-9.8.0/dallinger/docker/deployment.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/docker/docker-compose.yml.j2` & `dallinger-9.8.0/dallinger/docker/docker-compose.yml.j2`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/docker/ssh_templates/docker-compose-experiment.yml.j2` & `dallinger-9.8.0/dallinger/docker/ssh_templates/docker-compose-experiment.yml.j2`

 * *Files 11% similar despite different names*

```diff
@@ -25,17 +25,19 @@
     {%- for key, value in config.items() %}
       {{ key }}: {{ value | string() | tojson }}
     {%- endfor %}
     networks:
       - dallinger
     volumes:
       - ${HOME}/dallinger-data/{{ experiment_id }}:/var/lib/dallinger
-    {%- for volume in docker_volumes.split(",") %}
-      - {{ volume | string() | tojson }}
-    {%- endfor %}
+    {%- if docker_volumes | length > 0 %}
+      {%- for volume in docker_volumes.split(",") %}
+        - {{ volume | string() | tojson }}
+      {%- endfor %}
+    {%- endif %}
 
   web:
     image: {{ experiment_image }}
     user: "${UID}:${GID}"
     command: dallinger_heroku_web
     depends_on:
       <<: *commondepends
@@ -44,17 +46,19 @@
       PORT: 5000
     networks:
       dallinger:
         aliases:
           - {{ experiment_id }}_web
     volumes:
       - ${HOME}/dallinger-data/{{ experiment_id }}:/var/lib/dallinger
-    {%- for volume in docker_volumes.split(",") %}
-      - {{ volume | string() | tojson }}
-    {%- endfor %}
+    {%- if docker_volumes | length > 0 %}
+      {%- for volume in docker_volumes.split(",") %}
+        - {{ volume | string() | tojson }}
+      {%- endfor %}
+    {%- endif %}
 
 {%- if config["clock_on"] %}
   clock:
     image: {{ experiment_image }}
     user: "${UID}:${GID}"
     command: dallinger_heroku_clock
     depends_on:
```

### Comparing `dallinger-9.7.0/dallinger/docker/ssh_templates/docker-compose-server.yml` & `dallinger-9.8.0/dallinger/docker/ssh_templates/docker-compose-server.yml`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/docker/tools.py` & `dallinger-9.8.0/dallinger/docker/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,29 +53,32 @@
         self.env = env if env is not None else os.environ.copy()
         self.tmp_dir = tmp_dir
         self.original_dir = original_dir
         self.experiment_name = Path(self.original_dir).name
         self._record = []
         self.needs_chrome = needs_chrome
 
-    def copy_docker_compse_files(self):
+    def copy_docker_compose_files(self):
         """Prepare a docker-compose.yml file and place it in the experiment tmp dir"""
         volumes = [
             f"{self.original_dir}:{self.original_dir}",
             f"{self.tmp_dir}:/experiment",
         ]
         editable_dallinger_path = get_editable_dallinger_path()
         if editable_dallinger_path:
             volumes.append(f"{editable_dallinger_path}/dallinger:/dallinger/dallinger")
             volumes.append(
-                f"{editable_dallinger_path}/dallinger:/usr/local/lib/python3.8/dist-packages/dallinger/"
+                f"{editable_dallinger_path}/dallinger:/usr/local/lib/python3.10/dist-packages/dallinger/"
             )
             volumes.append(
                 f"{editable_dallinger_path}/dallinger:/usr/local/lib/python3.9/dist-packages/dallinger/"
             )
+            volumes.append(
+                f"{editable_dallinger_path}/dallinger:/usr/local/lib/python3.8/dist-packages/dallinger/"
+            )
         tag = get_experiment_image_tag(self.tmp_dir)
         with open(os.path.join(self.tmp_dir, "docker-compose.yml"), "w") as fh:
             fh.write(
                 docker_compose_template.render(
                     volumes=volumes,
                     experiment_name=self.experiment_name,
                     experiment_image=f"{self.experiment_name}:{tag}",
@@ -111,15 +114,15 @@
         needle = b"ready to accept connections"
         while needle not in self.run_compose(["logs", "postgresql"]):
             self.out.blather("Waiting for postgresql\n")
             time.sleep(1)
         self.out.blather("Postgresql ready\n")
 
     def start(self):
-        self.copy_docker_compse_files()
+        self.copy_docker_compose_files()
         build_image(self.tmp_dir, self.experiment_name, self.out, self.needs_chrome)
         check_output("docker compose up -d".split())
         # Wait for postgres to complete initialization
         self.wait_postgres_ready()
         try:
             self.run_compose(["exec", "worker", "dallinger-housekeeper", "initdb"])
         except CalledProcessError:
```

### Comparing `dallinger-9.7.0/dallinger/docker/wheel_filename.py` & `dallinger-9.8.0/dallinger/docker/wheel_filename.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/experiment.py` & `dallinger-9.8.0/dallinger/experiment.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/experiment_server/dashboard.py` & `dallinger-9.8.0/dallinger/experiment_server/dashboard.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/experiment_server/experiment_server.py` & `dallinger-9.8.0/dallinger/experiment_server/experiment_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,14 +50,19 @@
 q = Queue(connection=redis_conn)
 WAITING_ROOM_CHANNEL = "quorum"
 
 app = Flask("Experiment_Server")
 
 
 @app.before_request
+def _load_config():
+    _config()
+
+
+@app.before_request
 def check_for_protected_routes():
     if current_user.is_authenticated:
         return
 
     try:
         active_rule = request.url_rule.rule
     except AttributeError:
@@ -874,15 +879,22 @@
         return error_response(error_type=msg, status=400)
 
     session.flush()
     overrecruited = exp.is_overrecruited(nonfailed_count)
     if overrecruited:
         participant.status = "overrecruited"
 
-    result = {"participant": participant.__json__()}
+    result = {
+        "participant": {
+            **participant.__json__(),
+            # Add some extra information that is useful for initializing dallinger.identity
+            "unique_id": participant.unique_id,
+            "worker_id": participant.worker_id,
+        }
+    }
 
     # Queue notification to others in waiting room
     if exp.quorum:
         quorum = {
             "q": exp.quorum,
             "n": nonfailed_count,
             "overrecruited": participant.status == "overrecruited",
```

### Comparing `dallinger-9.7.0/dallinger/experiment_server/gunicorn.py` & `dallinger-9.8.0/dallinger/experiment_server/gunicorn.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/experiment_server/replay.py` & `dallinger-9.8.0/dallinger/experiment_server/replay.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/experiment_server/sockets.py` & `dallinger-9.8.0/dallinger/experiment_server/sockets.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/experiment_server/utils.py` & `dallinger-9.8.0/dallinger/experiment_server/utils.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/experiment_server/worker_events.py` & `dallinger-9.8.0/dallinger/experiment_server/worker_events.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/frontend/static/css/bootstrap.min.css` & `dallinger-9.8.0/dallinger/frontend/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/frontend/static/css/dashboard.css` & `dallinger-9.8.0/dallinger/frontend/static/css/dashboard.css`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/frontend/static/scripts/bootstrap.min.js` & `dallinger-9.8.0/dallinger/frontend/static/scripts/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/frontend/static/scripts/clipboard.min.js` & `dallinger-9.8.0/dallinger/frontend/static/scripts/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/frontend/static/scripts/dallinger2.js` & `dallinger-9.8.0/dallinger/frontend/static/scripts/dallinger2.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -76,14 +76,16 @@
      *
      * ``hitId``         - MTurk HIT Id
      *
      * ``workerId``      - MTurk Worker Id
      *
      * ``assignmentId``  - MTurk Assignment Id
      *
+     * ``uniqueId``      - MTurk Worker Id and Assignment Id
+     *
      * ``mode``          - Dallinger experiment mode
      *
      * ``participantId`` - Dallinger participant Id
      *
      * @namespace
      */
     dlgr.identity = {
@@ -107,14 +109,20 @@
         },
         get assignmentId() {
             return dlgr.storage.get('assignment_id');
         },
         set assignmentId(value) {
             dlgr.storage.set('assignment_id', value);
         },
+        get uniqueId() {
+            return dlgr.storage.get('unique_id');
+        },
+        set uniqueId(value) {
+            dlgr.storage.set('unique_id', value);
+        },
         get mode() {
             return dlgr.storage.get('mode');
         },
         set mode(value) {
             dlgr.storage.set('mode', value);
         },
         get participantId() {
@@ -137,14 +145,15 @@
         },
 
         initialize: function() {
             this.recruiter = dlgr.getUrlParameter('recruiter');
             this.hitId = dlgr.getUrlParameter('hitId');
             this.workerId = dlgr.getUrlParameter('workerId');
             this.assignmentId = dlgr.getUrlParameter('assignmentId');
+            this.uniqueId = dlgr.getUrlParameter('workerId') + ":" + dlgr.getUrlParameter('assignmentId');
             this.mode = dlgr.getUrlParameter('mode');
             // Store all url parameters as entry information.
             // This won't work in IE, but should work in Edge.
             var entry_info = {};
             var query_params = new URLSearchParams(location.search);
             for (const [k, v] of query_params) {
                 entry_info[k] = v;
@@ -420,15 +429,26 @@
             exitRoute = "/recruiter-exit?participant_id=" + participantId;
 
         dlgr.post('/worker_complete', {
             'participant_id': participantId
         }).done(function() {
             deferred.resolve();
             dlgr.allowExit();
-            if (window.opener && !window.opener.location.pathname.startsWith("/dashboard")) {
+
+            let openedFromDashboard;
+            try {
+                openedFromDashboard = window.opener && !window.opener.location.pathname.startsWith("/dashboard")
+            } catch (error) {
+                // If the parent window was from a different origin (e.g. Prolific) then we see an error like this:
+                // Uncaught DOMException: Blocked a frame with origin XXX from accessing a cross-origin frame.
+                // We catch and ignore this error.
+                openedFromDashboard = false;
+            }
+
+            if (window.opener && !openedFromDashboard) {
                 // If the parent window is still around, redirect it to the exit route
                 // and close the secondary window (this one) that held the main experiment:
                 window.opener.location = exitRoute;
                 window.close();
             } else {
                 // We're the only window, so show the exit route here:
                 window.location = exitRoute;
@@ -477,14 +497,18 @@
         } else {
             $(function() {
                 $('.btn-success').prop('disabled', true);
                 dlgr.post(url, data).done(function(resp) {
                     console.log(resp);
                     $('.btn-success').prop('disabled', false);
                     dlgr.identity.participantId = resp.participant.id;
+                    dlgr.identity.assignmentId = resp.participant.assignment_id;
+                    dlgr.identity.uniqueId = resp.participant.unique_id;
+                    dlgr.identity.workerId = resp.participant.worker_id;
+                    dlgr.identity.hitId = resp.participant.hit_id;
                     if (!resp.quorum) { // We're not using a waiting room.
                         deferred.resolve();
                         return;
                     }
 
                     // We've got a waiting room, so run waiting room checks...
                     if (resp.quorum.overrecruited) {
```

### Comparing `dallinger-9.7.0/dallinger/frontend/static/scripts/dallinger2.test.js` & `dallinger-9.8.0/dallinger/frontend/static/scripts/dallinger2.test.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -110,14 +110,15 @@
     });
 
     test('identity object is initialized from query string', () => {
         expect(dlgr.identity.recruiter).toBe('hotair');
         expect(dlgr.identity.assignmentId).toBe('AAA');
         expect(dlgr.identity.hitId).toBe('HHH');
         expect(dlgr.identity.workerId).toBe('WWW');
+        expect(dlgr.identity.uniqueId).toBe('WWW:AAA');
         expect(dlgr.identity.mode).toBe('debug');
     });
 
     test('participantId is initially undefined', () => {
         expect(dlgr.identity.participantId).toBe(undefined);
     });
```

### Comparing `dallinger-9.7.0/dallinger/frontend/static/scripts/fingerprintjs2/1.5.1/fingerprint2.min.js` & `dallinger-9.8.0/dallinger/frontend/static/scripts/fingerprintjs2/1.5.1/fingerprint2.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/frontend/static/scripts/jquery-3.6.0.min.js` & `dallinger-9.8.0/dallinger/frontend/static/scripts/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/frontend/static/scripts/network-monitor.js` & `dallinger-9.8.0/dallinger/frontend/static/scripts/network-monitor.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/frontend/static/scripts/popper.min.js` & `dallinger-9.8.0/dallinger/frontend/static/scripts/popper.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/frontend/static/scripts/reconnecting-websocket.js` & `dallinger-9.8.0/dallinger/frontend/static/scripts/reconnecting-websocket.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/frontend/static/scripts/require.js` & `dallinger-9.8.0/dallinger/frontend/static/scripts/require.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/frontend/static/scripts/reqwest.min.js` & `dallinger-9.8.0/dallinger/frontend/static/scripts/reqwest.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/frontend/static/scripts/spin.min.js` & `dallinger-9.8.0/dallinger/frontend/static/scripts/spin.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/frontend/static/scripts/store+json2.min.js` & `dallinger-9.8.0/dallinger/frontend/static/scripts/store+json2.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/frontend/static/scripts/tracker.js` & `dallinger-9.8.0/dallinger/frontend/static/scripts/tracker.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/frontend/static/scripts/tracker.js.map` & `dallinger-9.8.0/dallinger/frontend/static/scripts/tracker.js.map`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/frontend/static/scripts/tracking/load-tracker.js` & `dallinger-9.8.0/dallinger/frontend/static/scripts/tracking/load-tracker.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/frontend/static/scripts/tracking/scribe-analytics.min.js` & `dallinger-9.8.0/dallinger/frontend/static/scripts/tracking/scribe-analytics.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/frontend/static/scripts/tracking/scribe-dallinger.js` & `dallinger-9.8.0/dallinger/frontend/static/scripts/tracking/scribe-dallinger.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/frontend/static/vis@4.17.0/dist/vis-network.min.css` & `dallinger-9.8.0/dallinger/frontend/static/vis@4.17.0/dist/vis-network.min.css`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/frontend/static/vis@4.17.0/dist/vis.min.js` & `dallinger-9.8.0/dallinger/frontend/static/vis@4.17.0/dist/vis.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/frontend/templates/base/ad.html` & `dallinger-9.8.0/dallinger/frontend/templates/base/ad.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/frontend/templates/base/consent.html` & `dallinger-9.8.0/dallinger/frontend/templates/base/consent.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/frontend/templates/base/dashboard.html` & `dallinger-9.8.0/dallinger/frontend/templates/base/dashboard.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/frontend/templates/base/layout.html` & `dallinger-9.8.0/dallinger/frontend/templates/base/layout.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/frontend/templates/base/questionnaire.html` & `dallinger-9.8.0/dallinger/frontend/templates/base/questionnaire.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/frontend/templates/dashboard_database.html` & `dallinger-9.8.0/dallinger/frontend/templates/dashboard_database.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/frontend/templates/dashboard_develop.html` & `dallinger-9.8.0/dallinger/frontend/templates/dashboard_develop.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/frontend/templates/dashboard_home.html` & `dallinger-9.8.0/dallinger/frontend/templates/dashboard_home.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/frontend/templates/dashboard_lifecycle.html` & `dallinger-9.8.0/dallinger/frontend/templates/dashboard_lifecycle.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/frontend/templates/dashboard_monitor.html` & `dallinger-9.8.0/dallinger/frontend/templates/dashboard_monitor.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/frontend/templates/dashboard_mturk.html` & `dallinger-9.8.0/dallinger/frontend/templates/dashboard_mturk.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/frontend/templates/error-complete.html` & `dallinger-9.8.0/dallinger/frontend/templates/error-complete.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/frontend/templates/error.html` & `dallinger-9.8.0/dallinger/frontend/templates/error.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/frontend/templates/exit_recruiter.html` & `dallinger-9.8.0/dallinger/frontend/templates/exit_recruiter.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/frontend/templates/exit_recruiter_mturk.html` & `dallinger-9.8.0/dallinger/frontend/templates/exit_recruiter_mturk.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/frontend/templates/exit_recruiter_prolific.html` & `dallinger-9.8.0/dallinger/frontend/templates/exit_recruiter_prolific.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/frontend/templates/login.html` & `dallinger-9.8.0/dallinger/frontend/templates/login.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/frontend/templates/waiting.html` & `dallinger-9.8.0/dallinger/frontend/templates/waiting.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/heroku/clock.py` & `dallinger-9.8.0/dallinger/heroku/clock.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/heroku/rq_gevent_worker.py` & `dallinger-9.8.0/dallinger/heroku/rq_gevent_worker.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/heroku/tools.py` & `dallinger-9.8.0/dallinger/heroku/tools.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/jupyter.py` & `dallinger-9.8.0/dallinger/jupyter.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/models.py` & `dallinger-9.8.0/dallinger/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,15 +209,15 @@
     worker_id = Column(String(50), nullable=False)
 
     #: A String, the assignment id of the participant.
     assignment_id = Column(String(50), nullable=False, index=True)
 
     #: A String, a concatenation of :attr:`~dallinger.models.Participant.worker_id`
     #: and :attr:`~dallinger.models.Participant.assignment_id`
-    unique_id = Column(String(75), nullable=False, index=True)
+    unique_id = Column(String(150), nullable=False, index=True)
 
     #: A String, the id of the hit the participant is working on
     hit_id = Column(String(50), nullable=False)
 
     #: A String, the mode in which Dallinger is running: live,
     #: sandbox or debug.
     mode = Column(String(50), nullable=False)
```

### Comparing `dallinger-9.7.0/dallinger/mturk.py` & `dallinger-9.8.0/dallinger/mturk.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/networks.py` & `dallinger-9.8.0/dallinger/networks.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/nodes.py` & `dallinger-9.8.0/dallinger/nodes.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/notifications.py` & `dallinger-9.8.0/dallinger/notifications.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/processes.py` & `dallinger-9.8.0/dallinger/processes.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/prolific.py` & `dallinger-9.8.0/dallinger/prolific.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/pytest_dallinger.py` & `dallinger-9.8.0/dallinger/pytest_dallinger.py`

 * *Files 0% similar despite different names*

```diff
@@ -551,15 +551,15 @@
             kwargs = {}
             driver_class = DRIVER_MAP.get(request.param, webdriver.Chrome)
             if request.param == "chrome_headless":
                 from selenium.webdriver.chrome.options import Options
 
                 chrome_options = Options()
                 chrome_options.add_argument("--headless")
-                kwargs = {"chrome_options": chrome_options}
+                kwargs = {"options": chrome_options}
             driver = driver_class(**kwargs)
             driver.get(url)
             try:
                 yield driver
             finally:
                 try:
                     driver.quit()
```

### Comparing `dallinger-9.7.0/dallinger/recruiters.py` & `dallinger-9.8.0/dallinger/recruiters.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/redis_utils.py` & `dallinger-9.8.0/dallinger/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/registration.py` & `dallinger-9.8.0/dallinger/registration.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/transformations.py` & `dallinger-9.8.0/dallinger/transformations.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger/utils.py` & `dallinger-9.8.0/dallinger/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,28 +9,23 @@
 import shutil
 import string
 import subprocess
 import sys
 import tempfile
 import webbrowser
 from hashlib import md5
+from importlib.metadata import files as files_metadata
+from importlib.util import find_spec
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from unicodedata import normalize
 
-import pkg_resources
 import requests
 from faker import Faker
 from flask import request
-from pkg_resources import get_distribution
-
-try:
-    from importlib.metadata import files as files_metadata
-except ImportError:
-    from importlib_metadata import files as files_metadata
 
 from dallinger import db
 from dallinger.compat import is_command
 from dallinger.config import get_config
 from dallinger.version import __version__
 
 fake = Faker()
@@ -70,18 +65,15 @@
 def dallinger_package_path():
     """Return the absolute path of the root directory of the installed
     Dallinger package:
 
     >>> utils.dallinger_package_location()
     '/Users/janedoe/projects/Dallinger3/dallinger'
     """
-    dist = get_distribution("dallinger")
-    src_base = os.path.join(dist.location, dist.project_name)
-
-    return src_base
+    return os.path.dirname(find_spec("dallinger").origin)
 
 
 def generate_random_id(size=6, chars=string.ascii_uppercase + string.digits):
     """Generate random id numbers."""
     return "".join(random.choice(chars) for x in range(size))
 
 
@@ -383,28 +375,37 @@
         log("Checking your local Postgres database connection...")
         db.check_connection()
     except Exception:
         log("There was a problem connecting!")
         raise
 
 
-def check_experiment_dependencies(requirement_file):
+def check_experiment_dependencies(requirements_file):
     """Verify that the dependencies defined in a requirements file are
     in fact installed.
     If the environment variable SKIP_DEPENDENCY_CHECK is set, no check
     will be performed.
     """
     if os.environ.get("SKIP_DEPENDENCY_CHECK"):
         return
     try:
-        with open(requirement_file, "r") as f:
-            dependencies = [r for r in f.readlines() if r[:3] != "-e "]
+        with open(requirements_file, "r") as f:
+            dependencies = [
+                re.split("@|\\ |>|<|=|\\[", line)[0].strip()
+                for line in f.readlines()
+                if line[:3] != "-e " and line[0].strip() not in ["#", ""]
+            ]
     except (OSError, IOError):
         dependencies = []
-    pkg_resources.require(dependencies)
+
+    for dep in dependencies:
+        if find_spec(dep) is None:
+            raise ValueError(
+                f"Please install the '{dep}' package to run this experiment."
+            )
 
 
 def develop_target_path(config):
     """Extract the target `dallinger develop` working directory from
     configuration, and return it as a Path.
     """
     develop_path_string = config.get("dallinger_develop_directory", None)
```

### Comparing `dallinger-9.7.0/dallinger.egg-info/PKG-INFO` & `dallinger-9.8.0/dallinger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: dallinger
-Version: 9.7.0
+Version: 9.8.0
 Summary: Laboratory automation for the behavioral and social sciences
 Home-page: http://github.com/Dallinger/Dallinger
 Maintainer: Jordan Suchow
 Maintainer-email: suchow@berkeley.edu
 License: MIT
 Keywords: science,cultural evolution,experiments,psychology
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Pytest
 Description-Content-Type: text/markdown
 Provides-Extra: jupyter
 Provides-Extra: data
 Provides-Extra: dev
 Provides-Extra: docker
 License-File: LICENSE
```

### Comparing `dallinger-9.7.0/dallinger.egg-info/SOURCES.txt` & `dallinger-9.8.0/dallinger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dallinger.egg-info/requires.txt` & `dallinger-9.8.0/dallinger.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 flask-login
 Flask-WTF
 future
 gevent
 greenlet
 gunicorn
 heroku3
+ipython<8.13
 localconfig
 pexpect
 pip>=20
 pip-tools
 psycopg2
 psutil
 pyopenssl
@@ -31,30 +32,27 @@
 tabulate
 tenacity
 timeago
 tzlocal
 ua-parser
 user-agents
 
-[:python_version <= "3.7"]
-importlib_metadata
-
 [data]
 pandas
 tablib[all]
 
 [dev]
 alabaster
 black
 bumpversion
 coverage
 coverage_pth
 flake8
 isort
-mock==5.0.0
+mock
 myst-parser
 pre-commit
 pycodestyle
 pypandoc
 pytest
 pytest-rerunfailures
 sphinx
```

### Comparing `dallinger-9.7.0/dallinger_scripts/worker.py` & `dallinger-9.8.0/dallinger_scripts/worker.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/dev-requirements.txt` & `dallinger-9.8.0/dev-requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 
     # via -r dev-requirements.in
 alabaster==0.7.13
     # via
     #   dallinger
     #   sphinx
-anyio==3.6.2
+anyio==3.7.0
     # via jupyter-server
 apscheduler==3.10.1
     # via dallinger
 argon2-cffi==21.3.0
     # via
     #   jupyter-server
     #   nbclassic
@@ -44,33 +44,33 @@
     # via nbconvert
 black==23.3.0
     # via dallinger
 bleach==6.0.0
     # via nbconvert
 blinker==1.6.2
     # via flask
-boto3==1.26.121
+boto3==1.26.146
     # via dallinger
-botocore==1.29.121
+botocore==1.29.146
     # via
     #   boto3
     #   s3transfer
 build==0.10.0
     # via
     #   dallinger
     #   pip-tools
 bump2version==1.0.1
     # via bumpversion
 bumpversion==0.6.0
     # via dallinger
 cached-property==1.5.2
     # via dallinger
-cachetools==5.3.0
+cachetools==5.3.1
     # via tox
-certifi==2022.12.7
+certifi==2023.5.7
     # via
     #   requests
     #   selenium
 cffi==1.15.1
     # via
     #   argon2-cffi-bindings
     #   cryptography
@@ -88,61 +88,62 @@
     #   flask
     #   pip-tools
     #   rq
 colorama==0.4.6
     # via tox
 comm==0.1.3
     # via ipykernel
-coverage==7.2.3
+coverage==7.2.7
     # via
     #   coverage-pth
     #   dallinger
 coverage-pth==0.0.2
     # via dallinger
-cryptography==40.0.2
+cryptography==41.0.1
     # via
     #   paramiko
     #   pyopenssl
 debugpy==1.6.7
     # via ipykernel
 decorator==5.1.1
     # via ipython
 defusedxml==0.7.1
     # via
     #   nbconvert
     #   odfpy
 distlib==0.3.6
     # via virtualenv
-docker==6.0.1
+docker==6.1.3
     # via dallinger
 docutils==0.18.1
     # via
     #   myst-parser
     #   sphinx
     #   sphinx-rtd-theme
 et-xmlfile==1.1.0
     # via openpyxl
 exceptiongroup==1.1.1
     # via
+    #   anyio
     #   pytest
     #   trio
     #   trio-websocket
 executing==1.2.0
     # via stack-data
-faker==18.5.1
+faker==18.10.1
     # via dallinger
-fastjsonschema==2.16.3
+fastjsonschema==2.17.1
     # via nbformat
 filelock==3.12.0
     # via
     #   tox
     #   virtualenv
 flake8==6.0.0
     # via dallinger
-flask==2.3.1
+flask==2.3.2
     # via
     #   dallinger
     #   flask-crossdomain
     #   flask-login
     #   flask-sockets
     #   flask-wtf
 flask-crossdomain==0.1
@@ -171,36 +172,37 @@
     #   sqlalchemy
 gunicorn==20.1.0
     # via dallinger
 h11==0.14.0
     # via wsproto
 heroku3==5.2.1
     # via dallinger
-identify==2.5.23
+identify==2.5.24
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   jsonschema
     #   requests
     #   trio
 imagesize==1.4.1
     # via sphinx
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.22.0
+ipykernel==6.23.1
     # via
     #   ipywidgets
     #   jupyter
     #   jupyter-console
     #   nbclassic
     #   notebook
     #   qtconsole
-ipython==8.12.0
+ipython==8.12.2
     # via
+    #   dallinger
     #   ipykernel
     #   ipywidgets
     #   jupyter-console
 ipython-genutils==0.2.0
     # via
     #   nbclassic
     #   notebook
@@ -261,15 +263,15 @@
     #   nbclient
     #   nbconvert
     #   nbformat
     #   notebook
     #   qtconsole
 jupyter-events==0.6.3
     # via jupyter-server
-jupyter-server==2.5.0
+jupyter-server==2.6.0
     # via
     #   dallinger
     #   nbclassic
     #   notebook-shim
 jupyter-server-terminals==0.4.4
     # via jupyter-server
 jupyterlab-pygments==0.2.2
@@ -280,15 +282,15 @@
     # via dallinger
 markdown-it-py==2.2.0
     # via
     #   mdit-py-plugins
     #   myst-parser
 markuppy==1.14
     # via tablib
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via
     #   jinja2
     #   nbconvert
     #   werkzeug
     #   wtforms
 matplotlib-inline==0.1.6
     # via
@@ -298,56 +300,58 @@
     # via flake8
 mdit-py-plugins==0.3.5
     # via myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mistune==2.0.5
     # via nbconvert
-mock==5.0.0
+mock==5.0.2
     # via dallinger
 mypy-extensions==1.0.0
     # via black
 myst-parser==1.0.0
     # via dallinger
-nbclassic==0.5.5
+nbclassic==1.0.0
     # via notebook
-nbclient==0.7.4
+nbclient==0.8.0
     # via nbconvert
-nbconvert==7.3.1
+nbconvert==7.4.0
     # via
     #   jupyter
     #   jupyter-server
     #   nbclassic
     #   notebook
-nbformat==5.8.0
+nbformat==5.9.0
     # via
     #   jupyter-server
     #   nbclassic
     #   nbclient
     #   nbconvert
     #   notebook
 nest-asyncio==1.5.6
     # via
     #   ipykernel
     #   nbclassic
     #   notebook
-nodeenv==1.7.0
+nodeenv==1.8.0
     # via pre-commit
 notebook==6.5.4
     # via jupyter
 notebook-shim==0.2.3
     # via nbclassic
 numpy==1.24.3
     # via pandas
 odfpy==1.4.1
     # via tablib
 openpyxl==3.1.2
     # via tablib
 outcome==1.2.0
     # via trio
+overrides==7.3.1
+    # via jupyter-server
 packaging==23.1
     # via
     #   black
     #   build
     #   docker
     #   ipykernel
     #   jupyter-server
@@ -355,21 +359,21 @@
     #   pyproject-api
     #   pytest
     #   pytest-rerunfailures
     #   qtconsole
     #   qtpy
     #   sphinx
     #   tox
-pandas==2.0.1
+pandas==2.0.2
     # via
     #   dallinger
     #   tablib
 pandocfilters==1.5.0
     # via nbconvert
-paramiko==3.1.0
+paramiko==3.2.0
     # via
     #   dallinger
     #   sshtunnel
 parso==0.8.3
     # via jedi
 pathspec==0.11.1
     # via black
@@ -377,27 +381,27 @@
     # via
     #   dallinger
     #   ipython
 pickleshare==0.7.5
     # via ipython
 pip-tools==6.13.0
     # via dallinger
-platformdirs==3.4.0
+platformdirs==3.5.1
     # via
     #   black
     #   jupyter-core
     #   tox
     #   virtualenv
 pluggy==1.0.0
     # via
     #   pytest
     #   tox
-pre-commit==3.2.2
+pre-commit==3.3.2
     # via dallinger
-prometheus-client==0.16.0
+prometheus-client==0.17.0
     # via
     #   jupyter-server
     #   nbclassic
     #   notebook
 prompt-toolkit==3.0.38
     # via
     #   ipython
@@ -431,15 +435,15 @@
     #   ipython
     #   jupyter-console
     #   nbconvert
     #   qtconsole
     #   sphinx
 pynacl==1.5.0
     # via paramiko
-pyopenssl==23.1.1
+pyopenssl==23.2.0
     # via dallinger
 pypandoc==1.11
     # via dallinger
 pyproject-api==1.5.1
     # via tox
 pyproject-hooks==1.0.0
     # via build
@@ -463,60 +467,58 @@
     #   pandas
 python-json-logger==2.0.7
     # via jupyter-events
 pytz==2023.3
     # via
     #   apscheduler
     #   pandas
-pytz-deprecation-shim==0.1.0.post0
-    # via tzlocal
 pyyaml==6.0
     # via
     #   jupyter-events
     #   myst-parser
     #   pre-commit
     #   tablib
-pyzmq==25.0.2
+pyzmq==25.1.0
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-console
     #   jupyter-server
     #   nbclassic
     #   notebook
     #   qtconsole
-qtconsole==5.4.2
+qtconsole==5.4.3
     # via jupyter
 qtpy==2.3.1
     # via qtconsole
-redis==4.5.4
+redis==4.5.5
     # via
     #   dallinger
     #   rq
-requests==2.29.0
+requests==2.31.0
     # via
     #   dallinger
     #   docker
     #   heroku3
     #   sphinx
 rfc3339-validator==0.1.4
     # via
     #   jsonschema
     #   jupyter-events
 rfc3986-validator==0.1.1
     # via
     #   jsonschema
     #   jupyter-events
-rq==1.13.0
+rq==1.15.0
     # via dallinger
-s3transfer==0.6.0
+s3transfer==0.6.1
     # via boto3
-selenium==4.9.0
+selenium==4.9.1
     # via dallinger
-send2trash==1.8.0
+send2trash==1.8.2
     # via
     #   jupyter-server
     #   nbclassic
     #   notebook
 six==1.16.0
     # via
     #   apscheduler
@@ -539,15 +541,15 @@
 sphinx==6.2.1
     # via
     #   dallinger
     #   myst-parser
     #   sphinx-rtd-theme
     #   sphinxcontrib-jquery
     #   sphinxcontrib-spelling
-sphinx-rtd-theme==1.2.0
+sphinx-rtd-theme==1.2.1
     # via dallinger
 sphinxcontrib-applehelp==1.0.4
     # via sphinx
 sphinxcontrib-devhelp==1.0.2
     # via sphinx
 sphinxcontrib-htmlhelp==2.0.1
     # via sphinx
@@ -557,15 +559,15 @@
     # via sphinx
 sphinxcontrib-qthelp==1.0.3
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
 sphinxcontrib-spelling==8.0.0
     # via dallinger
-sqlalchemy==1.4.47
+sqlalchemy==1.4.48
     # via
     #   dallinger
     #   sqlalchemy-postgres-copy
 sqlalchemy-postgres-copy==0.5.0
     # via dallinger
 sshtunnel==0.4.0
     # via dallinger
@@ -593,23 +595,23 @@
     # via
     #   black
     #   build
     #   pyproject-api
     #   pyproject-hooks
     #   pytest
     #   tox
-tornado==6.3.1
+tornado==6.3.2
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
     #   nbclassic
     #   notebook
     #   terminado
-tox==4.5.1
+tox==4.5.2
     # via dallinger
 traitlets==5.9.0
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
@@ -628,52 +630,50 @@
 trio==0.22.0
     # via
     #   selenium
     #   trio-websocket
 trio-websocket==0.10.2
     # via selenium
 tzdata==2023.3
-    # via
-    #   pandas
-    #   pytz-deprecation-shim
-tzlocal==4.3
+    # via pandas
+tzlocal==5.0.1
     # via
     #   apscheduler
     #   dallinger
 ua-parser==0.16.1
     # via
     #   dallinger
     #   user-agents
 uri-template==1.2.0
     # via jsonschema
-urllib3==1.26.15
+urllib3==1.26.16
     # via
     #   botocore
     #   docker
     #   requests
     #   selenium
 user-agents==2.2.0
     # via dallinger
-virtualenv==20.22.0
+virtualenv==20.23.0
     # via
     #   pre-commit
     #   tox
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
 webencodings==0.5.1
     # via
     #   bleach
     #   tinycss2
-websocket-client==1.5.1
+websocket-client==1.5.2
     # via
     #   docker
     #   jupyter-server
-werkzeug==2.3.0
+werkzeug==2.3.4
     # via
     #   flask
     #   flask-login
 wheel==0.40.0
     # via pip-tools
 widgetsnbextension==4.0.7
     # via ipywidgets
```

### Comparing `dallinger-9.7.0/docs/Makefile` & `dallinger-9.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/make.bat` & `dallinger-9.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/_static/AvenirLTStd-Book_gdi.eot` & `dallinger-9.8.0/docs/source/_static/AvenirLTStd-Book_gdi.eot`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/_static/AvenirLTStd-Book_gdi.svg` & `dallinger-9.8.0/docs/source/_static/AvenirLTStd-Book_gdi.svg`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/_static/AvenirLTStd-Book_gdi.ttf` & `dallinger-9.8.0/docs/source/_static/AvenirLTStd-Book_gdi.ttf`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/_static/AvenirLTStd-Book_gdi.woff` & `dallinger-9.8.0/docs/source/_static/AvenirLTStd-Book_gdi.woff`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/_static/Dallinger AWS Group.png` & `dallinger-9.8.0/docs/source/_static/Dallinger AWS Group.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/_static/barplot.png` & `dallinger-9.8.0/docs/source/_static/barplot.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/_static/burst.png` & `dallinger-9.8.0/docs/source/_static/burst.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/_static/chain.png` & `dallinger-9.8.0/docs/source/_static/chain.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/_static/class_chart.jpg` & `dallinger-9.8.0/docs/source/_static/class_chart.jpg`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/_static/corner.jpg` & `dallinger-9.8.0/docs/source/_static/corner.jpg`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/_static/custom.css` & `dallinger-9.8.0/docs/source/_static/custom.css`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/_static/delayed.png` & `dallinger-9.8.0/docs/source/_static/delayed.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/_static/directories.jpg` & `dallinger-9.8.0/docs/source/_static/directories.jpg`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/_static/empty.jpg` & `dallinger-9.8.0/docs/source/_static/empty.jpg`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/_static/front_back_layout.jpg` & `dallinger-9.8.0/docs/source/_static/front_back_layout.jpg`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/_static/full.png` & `dallinger-9.8.0/docs/source/_static/full.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/_static/grid.png` & `dallinger-9.8.0/docs/source/_static/grid.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/_static/grid_mini.png` & `dallinger-9.8.0/docs/source/_static/grid_mini.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/_static/grid_small.png` & `dallinger-9.8.0/docs/source/_static/grid_small.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/_static/heroku.jpg` & `dallinger-9.8.0/docs/source/_static/heroku.jpg`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/_static/star.png` & `dallinger-9.8.0/docs/source/_static/star.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/aws_etc_keys.rst` & `dallinger-9.8.0/docs/source/aws_etc_keys.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/build_demo_docs.py` & `dallinger-9.8.0/docs/source/build_demo_docs.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/building_documentation.rst` & `dallinger-9.8.0/docs/source/building_documentation.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/classes.rst` & `dallinger-9.8.0/docs/source/classes.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/command_line_utility.rst` & `dallinger-9.8.0/docs/source/command_line_utility.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/communicating_with_the_server.rst` & `dallinger-9.8.0/docs/source/communicating_with_the_server.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/conf.py` & `dallinger-9.8.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/configuration.rst` & `dallinger-9.8.0/docs/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/contributing_to_dallinger.rst` & `dallinger-9.8.0/docs/source/contributing_to_dallinger.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/creating_an_experiment.rst` & `dallinger-9.8.0/docs/source/creating_an_experiment.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/demo_index.rst` & `dallinger-9.8.0/docs/source/demo_index.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/demoing_dallinger.rst` & `dallinger-9.8.0/docs/source/demoing_dallinger.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/demos_on_heroku.rst` & `dallinger-9.8.0/docs/source/demos_on_heroku.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/developing_dallinger_setup_guide.rst` & `dallinger-9.8.0/docs/source/developing_dallinger_setup_guide.rst`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 Mac OS X
 --------
 
 Install Python
 ~~~~~~~~~~~~~~
 
 Dallinger is written in the language Python. For it to work, you will need
-to have Python 3.7 or higher. You can check what version of Python you
+to have Python 3.8 or higher. You can check what version of Python you
 have by running:
 ::
 
     python --version
 
 
 .. note::
@@ -350,15 +350,15 @@
 Ubuntu
 ------
 
 Install Python
 ~~~~~~~~~~~~~~
 
 Dallinger is written in the language Python. For it to work, you will need
-to have Python 3.7 or higher. Python 3 is the preferred option.
+to have Python 3.8 or higher. Python 3 is the preferred option.
 You can check what version of Python you have by running:
 ::
 
     python --version
 
 
 Ubuntu 18.04 LTS ships with Python 3.6.
```

### Comparing `dallinger-9.7.0/docs/source/docker_only.rst` & `dallinger-9.8.0/docs/source/docker_only.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/docker_support.rst` & `dallinger-9.8.0/docs/source/docker_support.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/docker_tutorial.rst` & `dallinger-9.8.0/docs/source/docker_tutorial.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/email_setup.rst` & `dallinger-9.8.0/docs/source/email_setup.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/experiment_data.rst` & `dallinger-9.8.0/docs/source/experiment_data.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/extra_configuration.rst` & `dallinger-9.8.0/docs/source/extra_configuration.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/index.rst` & `dallinger-9.8.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/installing_dallinger_for_users.rst` & `dallinger-9.8.0/docs/source/installing_dallinger_for_users.rst`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 Mac OS X
 --------
 
 Install Python
 ~~~~~~~~~~~~~~
 
 Dallinger is written in the language Python. For it to work, you will need
-to have Python 3.7 or higher. You can check what version of Python you have
+to have Python 3.8 or higher. You can check what version of Python you have
 by running:
 ::
 
     python --version
 
 
 .. note::
@@ -303,15 +303,15 @@
 Ubuntu
 ------
 
 Install Python
 ~~~~~~~~~~~~~~
 
 Dallinger is written in the language Python. For it to work, you will need
-to have Python 3.7 or higher. You can check what version of Python you have
+to have Python 3.8 or higher. You can check what version of Python you have
 by running:
 ::
 
     python --version
 
 
 Ubuntu 18.04 LTS ships with Python 3.6.
```

### Comparing `dallinger-9.7.0/docs/source/javascript_api.rst` & `dallinger-9.8.0/docs/source/javascript_api.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/learning_to_use_dallinger.rst` & `dallinger-9.8.0/docs/source/learning_to_use_dallinger.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/monitoring_a_live_experiment.rst` & `dallinger-9.8.0/docs/source/monitoring_a_live_experiment.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/networks.rst` & `dallinger-9.8.0/docs/source/networks.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/postico_and_postgres.rst` & `dallinger-9.8.0/docs/source/postico_and_postgres.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/private_repo.rst` & `dallinger-9.8.0/docs/source/private_repo.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/python_module.rst` & `dallinger-9.8.0/docs/source/python_module.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/recruitment.rst` & `dallinger-9.8.0/docs/source/recruitment.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/required_experiment_files.rst` & `dallinger-9.8.0/docs/source/required_experiment_files.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/rewarding_participants.rst` & `dallinger-9.8.0/docs/source/rewarding_participants.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/running_bots.rst` & `dallinger-9.8.0/docs/source/running_bots.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/running_the_tests.rst` & `dallinger-9.8.0/docs/source/running_the_tests.rst`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 The tests include:
 
 * Making sure that a source distribution of the Python package can be created.
 * Running `flake8 <https://flake8.readthedocs.io>`_ to make sure Python code
   conforms to the `PEP 8 <https://www.python.org/dev/peps/pep-0008/>`_ style guide.
 * Running the tests for the Python code using `pytest <http://doc.pytest.org/>`_
-  and making sure they pass on Python 3.7, 3.8, and 3.9.
+  and making sure they pass on Python 3.8, 3.9, and 3.10.
 * Making sure that `code coverage <https://coverage.readthedocs.io/>`_
   for the Python code is above the desired threshold.
 * Making sure the docs build without error.
 
 If you see ImportErrors related to demo packages, this most likely means you
 have not installed the ``dlgr.demos`` sub-package. See the
 :doc:`Dallinger development installation instructions
```

### Comparing `dallinger-9.7.0/docs/source/scheduled_tasks.rst` & `dallinger-9.8.0/docs/source/scheduled_tasks.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/spelling_wordlist.txt` & `dallinger-9.8.0/docs/source/spelling_wordlist.txt`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/the_experiment_class.rst` & `dallinger-9.8.0/docs/source/the_experiment_class.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/troubleshooting.rst` & `dallinger-9.8.0/docs/source/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/vagrant_setup.rst` & `dallinger-9.8.0/docs/source/vagrant_setup.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/waiting_rooms.rst` & `dallinger-9.8.0/docs/source/waiting_rooms.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/web_api.rst` & `dallinger-9.8.0/docs/source/web_api.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/docs/source/writing_bots.rst` & `dallinger-9.8.0/docs/source/writing_bots.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/incubator.png` & `dallinger-9.8.0/incubator.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/requirements.txt` & `dallinger-9.8.0/requirements.txt`

 * *Files 12% similar despite different names*

```diff
@@ -4,59 +4,67 @@
 #
 #    ./scripts/update_dependencies.sh
 #
 
     # via -r requirements.in
 apscheduler==3.10.1
     # via dallinger
+asttokens==2.2.1
+    # via stack-data
 async-generator==1.10
     # via trio
 async-timeout==4.0.2
     # via redis
 attrs==23.1.0
     # via
     #   outcome
     #   trio
+backcall==0.2.0
+    # via ipython
 blinker==1.6.2
     # via flask
-boto3==1.26.121
+boto3==1.26.146
     # via dallinger
-botocore==1.29.121
+botocore==1.29.146
     # via
     #   boto3
     #   s3transfer
 build==0.10.0
     # via
     #   dallinger
     #   pip-tools
 cached-property==1.5.2
     # via dallinger
-certifi==2022.12.7
+certifi==2023.5.7
     # via
     #   requests
     #   selenium
 cffi==1.15.1
     # via cryptography
 charset-normalizer==3.1.0
     # via requests
 click==8.1.3
     # via
     #   dallinger
     #   flask
     #   pip-tools
     #   rq
-cryptography==40.0.2
+cryptography==41.0.1
     # via pyopenssl
+decorator==5.1.1
+    # via ipython
 exceptiongroup==1.1.1
     # via
     #   trio
     #   trio-websocket
-faker==18.5.1
+executing==1.2.0
+    # via stack-data
+faker==18.10.1
     # via dallinger
-flask==2.3.1
+flask==2.3.2
     # via
     #   dallinger
     #   flask-crossdomain
     #   flask-login
     #   flask-sockets
     #   flask-wtf
 flask-crossdomain==0.1
@@ -87,128 +95,151 @@
     # via wsproto
 heroku3==5.2.1
     # via dallinger
 idna==3.4
     # via
     #   requests
     #   trio
+ipython==8.12.2
+    # via dallinger
 itsdangerous==2.1.2
     # via
     #   flask
     #   flask-wtf
+jedi==0.18.2
+    # via ipython
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
 localconfig==1.1.3
     # via dallinger
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
     #   wtforms
+matplotlib-inline==0.1.6
+    # via ipython
 outcome==1.2.0
     # via trio
 packaging==23.1
     # via build
+parso==0.8.3
+    # via jedi
 pexpect==4.8.0
-    # via dallinger
+    # via
+    #   dallinger
+    #   ipython
+pickleshare==0.7.5
+    # via ipython
 pip-tools==6.13.0
     # via dallinger
+prompt-toolkit==3.0.38
+    # via ipython
 psutil==5.9.5
     # via dallinger
 psycopg2==2.9.6
     # via
     #   dallinger
     #   sqlalchemy-postgres-copy
 ptyprocess==0.7.0
     # via pexpect
+pure-eval==0.2.2
+    # via stack-data
 pycparser==2.21
     # via cffi
-pyopenssl==23.1.1
+pygments==2.15.1
+    # via ipython
+pyopenssl==23.2.0
     # via dallinger
 pyproject-hooks==1.0.0
     # via build
 pysocks==1.7.1
     # via urllib3
 python-dateutil==2.8.2
     # via
     #   botocore
     #   faker
     #   heroku3
 pytz==2023.3
     # via apscheduler
-pytz-deprecation-shim==0.1.0.post0
-    # via tzlocal
-redis==4.5.4
+redis==4.5.5
     # via
     #   dallinger
     #   rq
-requests==2.29.0
+requests==2.31.0
     # via
     #   dallinger
     #   heroku3
-rq==1.13.0
+rq==1.15.0
     # via dallinger
-s3transfer==0.6.0
+s3transfer==0.6.1
     # via boto3
-selenium==4.9.0
+selenium==4.9.1
     # via dallinger
 six==1.16.0
     # via
     #   apscheduler
+    #   asttokens
     #   dallinger
     #   python-dateutil
     #   sqlalchemy-postgres-copy
 sniffio==1.3.0
     # via trio
 sortedcontainers==2.4.0
     # via trio
-sqlalchemy==1.4.47
+sqlalchemy==1.4.48
     # via
     #   dallinger
     #   sqlalchemy-postgres-copy
 sqlalchemy-postgres-copy==0.5.0
     # via dallinger
+stack-data==0.6.2
+    # via ipython
 tabulate==0.9.0
     # via dallinger
 tenacity==8.2.2
     # via dallinger
 timeago==1.0.16
     # via dallinger
 tomli==2.0.1
     # via
     #   build
     #   pyproject-hooks
+traitlets==5.9.0
+    # via
+    #   ipython
+    #   matplotlib-inline
 trio==0.22.0
     # via
     #   selenium
     #   trio-websocket
 trio-websocket==0.10.2
     # via selenium
-tzdata==2023.3
-    # via pytz-deprecation-shim
-tzlocal==4.3
+tzlocal==5.0.1
     # via
     #   apscheduler
     #   dallinger
 ua-parser==0.16.1
     # via
     #   dallinger
     #   user-agents
-urllib3==1.26.15
+urllib3==1.26.16
     # via
     #   botocore
     #   requests
     #   selenium
 user-agents==2.2.0
     # via dallinger
-werkzeug==2.3.0
+wcwidth==0.2.6
+    # via prompt-toolkit
+werkzeug==2.3.4
     # via
     #   flask
     #   flask-login
 wheel==0.40.0
     # via pip-tools
 wsproto==1.2.0
     # via trio-websocket
```

### Comparing `dallinger-9.7.0/setup.py` & `dallinger-9.8.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,32 +8,32 @@
 
 README = (HERE / "README.md").read_text(encoding="utf-8")
 
 
 setup_args = dict(
     name="dallinger",
     packages=["dallinger", "dallinger_scripts"],
-    version="9.7.0",
+    version="9.8.0",
     description="Laboratory automation for the behavioral and social sciences",
     long_description=README,
     long_description_content_type="text/markdown",
     url="http://github.com/Dallinger/Dallinger",
     maintainer="Jordan Suchow",
     maintainer_email="suchow@berkeley.edu",
     license="MIT",
     keywords=["science", "cultural evolution", "experiments", "psychology"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Framework :: Pytest",
     ],
     include_package_data=True,
     zip_safe=False,
     entry_points={
         "console_scripts": [
             "dallinger = dallinger.command_line:dallinger",
@@ -58,14 +58,15 @@
         "flask-login",
         "Flask-WTF",
         "future",
         "gevent",
         "greenlet",
         "gunicorn",
         "heroku3",
+        "ipython < 8.13",
         "localconfig",
         "pexpect",
         "pip>=20",
         "pip-tools",
         "psycopg2",
         "psutil",
         "pyopenssl",
@@ -97,25 +98,24 @@
             "alabaster",
             "black",
             "bumpversion",
             "coverage",
             "coverage_pth",
             "flake8",
             "isort",
-            "mock==5.0.0",
+            "mock",
             "myst-parser",
             "pre-commit",
             "pycodestyle",
             "pypandoc",
             "pytest",
             "pytest-rerunfailures",
             "sphinx",
             "sphinx_rtd_theme",
             "sphinxcontrib-spelling",
             "tox",
         ],
         "docker": ["docker", "paramiko", "sshtunnel"],
-        ':python_version <= "3.7"': ["importlib_metadata"],
     },
 )
 
 setup(**setup_args)
```

### Comparing `dallinger-9.7.0/tests/test_agents.py` & `dallinger-9.8.0/tests/test_agents.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/tests/test_api.py` & `dallinger-9.8.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/tests/test_bots.py` & `dallinger-9.8.0/tests/test_bots.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
     def req_get(self):
         with mock.patch("requests.get") as patch_get:
             yield patch_get
 
     @pytest.fixture
     def fake_uuid(self):
         with mock.patch("uuid.uuid4") as patch_uuid4:
-            patch_uuid4.hex.return_value = "fakehash"
+            patch_uuid4.return_value.hex = "fakehash"
             yield patch_uuid4
 
     def test_create_bot(self, bot):
         """Create a bot."""
         from dallinger.bots import HighPerformanceBotBase
 
         assert isinstance(bot, HighPerformanceBotBase)
@@ -145,37 +145,37 @@
 
     def test_sign_up(self, bot, req_post, fake_uuid):
         mock_return = mock.Mock()
         mock_return.json.return_value = {"status": "OK", "participant": {"id": 4}}
         req_post.return_value = mock_return
 
         bot.sign_up()
-        assert bot.subscribe_to_quorum_channel.called_once_with()
-        assert req_post.called_once_with(
+        bot.subscribe_to_quorum_channel.assert_called_once_with()
+        req_post.assert_called_once_with(
             "https://dallinger.io/participant/worker1/hit1/assignment1/debug?"
             "fingerprint_hash=fakehash&recruiter=bots:HighPerformanceBotBase"
         )
         assert bot.participant_id == 4
 
     def test_sign_off(self, bot, req_post):
         value = bot.sign_off()
-        assert req_post.called_once_with(
-            "https://dallinger.io/question/participant1",
+        req_post.assert_called_once_with(
+            "https://dallinger.io/question/1",
             data={
                 "question": "questionnaire",
                 "number": 1,
                 "response": json.dumps({"engagement": 4, "difficulty": 3}),
             },
         )
         assert value is True
 
     def test_complete_experiment(self, bot, req_get):
         mock_return = mock.Mock()
         mock_return.dummy = 1
         req_get.return_value = mock_return
 
         response = bot.complete_experiment("worker_complete")
-        assert req_get.called_once_with(
+        req_get.assert_called_once_with(
             "https://dallinger.io/worker_complete?participant_id=1"
         )
         # returns the response object
         assert response.dummy == 1
```

### Comparing `dallinger-9.7.0/tests/test_cli_config.py` & `dallinger-9.8.0/tests/test_cli_config.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/tests/test_command_line.py` & `dallinger-9.8.0/tests/test_command_line.py`

 * *Files 0% similar despite different names*

```diff
@@ -981,16 +981,16 @@
 
     def test_destroy_no_expire_hits(self, destroy, heroku, mturk):
         CliRunner().invoke(
             destroy, ["--app", "some-app-uid", "--yes", "--no-expire-hit"]
         )
         heroku.destroy.assert_called_once()
         mturk_instance = mturk.return_value
-        mturk_instance.get_hits.not_called()
-        mturk_instance.expire_hit.not_called()
+        mturk_instance.get_hits.assert_not_called()
+        mturk_instance.expire_hit.assert_not_called()
 
     def test_requires_confirmation(self, destroy, heroku):
         CliRunner().invoke(destroy, ["--app", "some-app-uid"])
         heroku.destroy.assert_not_called()
 
     def test_destroy_expire_uses_sandbox(self, destroy, heroku, mturk):
         CliRunner().invoke(
```

### Comparing `dallinger-9.7.0/tests/test_config.py` & `dallinger-9.8.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/tests/test_dashboard.py` & `dallinger-9.8.0/tests/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/tests/test_data.py` & `dallinger-9.8.0/tests/test_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
             # The registration creates a new file in the dallinger-registrations bucket
             assert url.startswith("https://my-fake-registrations.")
             assert new_uuid in url
 
             # We should be able to check that the UUID is registered
             assert dallinger.data.is_registered(new_uuid) is False
-            assert s3_filter.called_once_with(Prefix=new_uuid)
+            s3_filter.assert_called_once_with(Prefix=new_uuid + ".reg")
 
 
 class TestDataLocally(object):
     """Tests that interact with local data only, and are relatively fast to
     execute.
     """
```

### Comparing `dallinger-9.7.0/tests/test_db.py` & `dallinger-9.8.0/tests/test_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import mock
+import pytest
 
 
 def test_redis():
     from dallinger.db import redis_conn
 
     assert redis_conn.ping()
 
@@ -60,22 +61,23 @@
     serialized_write()
 
     # Which we can check by making sure that `add_participant`
     # calculated the count at least 3 times
     assert counts == [0, 0, 1]
 
 
+@pytest.mark.skip(reason="This test needs to be re-investigated.")
 def test_after_commit_hook(db_session):
     with mock.patch("dallinger.db.redis_conn") as redis:
         from dallinger.db import queue_message
 
         queue_message("test", "test")
         db_session.commit()
 
-        assert redis.called_once_with("test", "test")
+        redis.assert_called_once_with("test", "test")
 
 
 def test_create_db_engine_updates_postgresql_scheme():
     old_scheme_uri = "postgres://foo:bar@somehost:5432/blah"
     from dallinger.db import create_db_engine
 
     engine = create_db_engine(old_scheme_uri)
```

### Comparing `dallinger-9.7.0/tests/test_demos.py` & `dallinger-9.8.0/tests/test_demos.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     def test_verify_all_demos(self, iter_demos):
         for demo in iter_demos:
             if not verify_package(verbose=False):
                 pytest.fail("{} did not verify!".format(demo))
 
     def test_instantiation_via_entry_points(self):
         failures = []
-        for entry in experiments.iter_entry_points(group="dallinger.experiments"):
+        for entry in experiments.entry_points().get("dallinger.experiments"):
             try:
                 entry.load()()
             except Exception as ex:
                 failures.append("{}: {}".format(entry.name, ex))
 
         if failures:
             pytest.fail(
```

### Comparing `dallinger-9.7.0/tests/test_deployment.py` & `dallinger-9.8.0/tests/test_deployment.py`

 * *Files 4% similar despite different names*

```diff
@@ -922,28 +922,23 @@
             except IOError:
                 pass
 
     def test_failure(self, debugger):
         from requests.exceptions import HTTPError
 
         with mock.patch("dallinger.deployment.HerokuLocalDeployment.WRAPPER_CLASS"):
-            # For some reason this test alone triggers a failure in the line in
-            # deployment.py that invokes `pkg_resources.require`.
-            # Monkey patching it here makes it work.
-            # It would be interesting to get to the root cause.
-            with mock.patch("dallinger.utils.pkg_resources"):
-                with mock.patch("dallinger.deployment.requests.post") as mock_post:
-                    mock_post.return_value = mock.Mock(
-                        ok=False,
-                        json=mock.Mock(return_value={"message": "msg!"}),
-                        raise_for_status=mock.Mock(side_effect=HTTPError),
-                        status_code=500,
-                        text="Failure",
-                    )
-                    debugger.run()
+            with mock.patch("dallinger.deployment.requests.post") as mock_post:
+                mock_post.return_value = mock.Mock(
+                    ok=False,
+                    json=mock.Mock(return_value={"message": "msg!"}),
+                    raise_for_status=mock.Mock(side_effect=HTTPError),
+                    status_code=500,
+                    text="Failure",
+                )
+                debugger.run()
 
         # Only one launch attempt should be made in debug mode
         debugger.out.error.assert_has_calls(
             [
                 mock.call(
                     "Error accessing http://localhost:5000/launch (500):\nFailure"
                 ),
@@ -1132,15 +1127,18 @@
         extant_github_tag = "b98f719c1ce851353f7cfcc78362cfaace51bb8d"
         (Path(tmp_path) / "requirements.txt").write_text("black")
         with mock.patch("dallinger.utils.__version__", extant_github_tag):
             ensure_constraints_file_presence(tmp_path)
             constraints_file = Path(tmp_path) / "constraints.txt"
             # If not present a `constraints.txt` file will be generated
             assert constraints_file.exists()
-            assert "toml" in constraints_file.read_text()
+            if sys.version_info >= (3, 11):
+                assert "toml" not in constraints_file.read_text()
+            else:
+                assert "toml" in constraints_file.read_text()
 
             # An existing file will be left untouched
             constraints_file.write_text("foobar")
             with pytest.raises(ValueError):
                 ensure_constraints_file_presence(tmp_path)
             assert constraints_file.read_text() == "foobar"
```

### Comparing `dallinger-9.7.0/tests/test_docker.py` & `dallinger-9.8.0/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/tests/test_environments.py` & `dallinger-9.8.0/tests/test_environments.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/tests/test_experiment.py` & `dallinger-9.8.0/tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/tests/test_experiment_server.py` & `dallinger-9.8.0/tests/test_experiment_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         from dallinger.experiment_server.gunicorn import StandaloneServer
 
         with mock.patch("sys.argv", ["gunicorn"]):
             with mock.patch(
                 "dallinger.experiment_server.gunicorn.ProxyFix"
             ) as ProxyFix:
                 StandaloneServer().load()
-                ProxyFix.called_once_with(webapp.application)
+                ProxyFix.assert_called_once_with(webapp.application)
 
     def test_load_sets_flask_secret_from_env(self, webapp, active_config, env):
         webapp.application.debug = False
         from dallinger.experiment_server.gunicorn import StandaloneServer
 
         env["FLASK_SECRET_KEY"] = "A BAD SECRET KEY"
         with mock.patch("sys.argv", ["gunicorn"]):
```

### Comparing `dallinger-9.7.0/tests/test_griduniverse.py` & `dallinger-9.8.0/tests/test_griduniverse.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/tests/test_heroku.py` & `dallinger-9.8.0/tests/test_heroku.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         assert (
             jobs[0].func_ref
             == "dallinger.heroku.clock:check_db_for_missing_notifications"
         )
 
     def test_launch_loads_config(self, patched_scheduler):
         self.clock.launch()
-        assert patched_scheduler.start.called_once()
+        patched_scheduler.start.assert_called_once()
         assert get_config().ready
 
     def test_launch_registers_additional_tasks(
         self, patched_scheduler, tasks_with_cleanup
     ):
         jobs = patched_scheduler.get_jobs()
         assert len(jobs) == 1
```

### Comparing `dallinger-9.7.0/tests/test_information.py` & `dallinger-9.8.0/tests/test_information.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/tests/test_jupyter.py` & `dallinger-9.8.0/tests/test_jupyter.py`

 * *Files 21% similar despite different names*

```diff
@@ -22,14 +22,14 @@
         exp.update_status("Testing")
         assert exp.widget.status == "Testing"
         assert "Testing" in exp.widget.children[0].value
 
     def test_experiment_displays_widget(self, exp):
         with mock.patch("IPython.display.display") as display:
             exp._ipython_display_()
-            assert display.called_once_with(exp.widget)
+            display.assert_called_once_with(exp.widget)
 
     def test_widget_children_no_config(self, exp):
         assert exp.widget.children[1].children[0].value == "Not loaded."
 
     def test_widget_children_with_config(self, active_config, exp):
         assert exp.widget.children[1].children[0].value != "Not loaded."
```

### Comparing `dallinger-9.7.0/tests/test_models.py` & `dallinger-9.8.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/tests/test_mturk.py` & `dallinger-9.8.0/tests/test_mturk.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/tests/test_networks.py` & `dallinger-9.8.0/tests/test_networks.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/tests/test_notifications.py` & `dallinger-9.8.0/tests/test_notifications.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/tests/test_processes.py` & `dallinger-9.8.0/tests/test_processes.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/tests/test_prolific.py` & `dallinger-9.8.0/tests/test_prolific.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/tests/test_recruiters.py` & `dallinger-9.8.0/tests/test_recruiters.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/tests/test_replay.py` & `dallinger-9.8.0/tests/test_replay.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/tests/test_replay_state.py` & `dallinger-9.8.0/tests/test_replay_state.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/tests/test_sockets.py` & `dallinger-9.8.0/tests/test_sockets.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/tests/test_sources.py` & `dallinger-9.8.0/tests/test_sources.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/tests/test_transformations.py` & `dallinger-9.8.0/tests/test_transformations.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.7.0/tests/test_utils.py` & `dallinger-9.8.0/tests/test_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # -*- coding: utf-8 -*-
 import io
 import locale
 from datetime import datetime, timedelta
+from tempfile import NamedTemporaryFile
 
 import mock
 import pytest
 
 from dallinger import config, utils
+from dallinger.utils import check_experiment_dependencies
 
 
 class TestSubprocessWrapper(object):
     @pytest.fixture
     def sys(self):
         with mock.patch("dallinger.utils.sys") as sys:
             yield sys
@@ -284,7 +286,43 @@
         with mock.patch.multiple(
             "dallinger.utils", is_command=mock.DEFAULT, sys=mock.DEFAULT
         ) as patches:
             patches["is_command"].return_value = False
             patches["sys"].platform = 'anything but "darwin"'
             isolated = utils._new_webbrowser_profile()
         assert isolated == webbrowser
+
+
+def test_check_experiment_dependencies_successful():
+    with NamedTemporaryFile() as requirements_file:
+        requirements = [
+            "dallinger",
+            "dallinger==9.7.0",
+            "dallinger<=9.7.0",
+            "dallinger>=9.7.0",
+            "dallinger == 9.7.0",
+            "dallinger@git+https://github.com/Dallinger/Dallinger",
+            "dallinger @ git+https://github.com/Dallinger/Dallinger",
+            "dallinger[demos]",
+            "dallinger [demos]",
+            "# dallinger",
+            "",
+            " # dallinger",
+        ]
+        lines = [f"{r}\n".encode("utf-8") for r in requirements]
+        requirements_file.writelines(lines)
+        requirements_file.flush()
+
+        check_experiment_dependencies(requirements_file.name)
+
+
+def test_check_experiment_dependencies_unsuccessful():
+    with NamedTemporaryFile() as requirements_file:
+        requirements_file.writelines(["NOTINSTALLED\n".encode("utf-8")])
+        requirements_file.flush()
+
+        with pytest.raises(ValueError) as e:
+            check_experiment_dependencies(requirements_file.name)
+        assert (
+            str(e.value)
+            == "Please install the 'NOTINSTALLED' package to run this experiment."
+        )
```

