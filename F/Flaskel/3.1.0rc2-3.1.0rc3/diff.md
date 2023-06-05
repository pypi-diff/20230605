# Comparing `tmp/Flaskel-3.1.0rc2.tar.gz` & `tmp/Flaskel-3.1.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flaskel-3.1.0rc2.tar", last modified: Thu May 25 21:39:53 2023, max compression
+gzip compressed data, was "Flaskel-3.1.0rc3.tar", last modified: Mon Jun  5 00:39:53 2023, max compression
```

## Comparing `Flaskel-3.1.0rc2.tar` & `Flaskel-3.1.0rc3.tar`

### file list

```diff
@@ -1,171 +1,225 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.264777 Flaskel-3.1.0rc2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.243777 Flaskel-3.1.0rc2/Flaskel.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15616 2023-05-25 21:39:53.000000 Flaskel-3.1.0rc2/Flaskel.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4585 2023-05-25 21:39:53.000000 Flaskel-3.1.0rc2/Flaskel.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 21:39:53.000000 Flaskel-3.1.0rc2/Flaskel.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-05-25 21:39:53.000000 Flaskel-3.1.0rc2/Flaskel.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 21:39:53.000000 Flaskel-3.1.0rc2/Flaskel.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      893 2023-05-25 21:39:53.000000 Flaskel-3.1.0rc2/Flaskel.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-25 21:39:53.000000 Flaskel-3.1.0rc2/Flaskel.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    15616 2023-05-25 21:39:53.264777 Flaskel-3.1.0rc2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    14795 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.244777 Flaskel-3.1.0rc2/flaskel/
--rw-rw-rw-   0 root         (0) root         (0)      712 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12156 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/builder.py
--rw-rw-rw-   0 root         (0) root         (0)     9054 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1188 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/converters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.247777 Flaskel-3.1.0rc2/flaskel/ext/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7321 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     4245 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/caching.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.247777 Flaskel-3.1.0rc2/flaskel/ext/crypto/
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/crypto/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1777 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/crypto/argon.py
--rw-rw-rw-   0 root         (0) root         (0)      885 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/datetime.py
--rw-rw-rw-   0 root         (0) root         (0)     1278 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/default.py
--rw-rw-rw-   0 root         (0) root         (0)      646 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.247777 Flaskel-3.1.0rc2/flaskel/ext/healthcheck/
--rw-rw-rw-   0 root         (0) root         (0)      203 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/healthcheck/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6601 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/healthcheck/checkers.py
--rw-rw-rw-   0 root         (0) root         (0)     4957 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/healthcheck/health.py
--rw-rw-rw-   0 root         (0) root         (0)     7842 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/ipban.py
--rw-rw-rw-   0 root         (0) root         (0)     5419 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/jobs.py
--rw-rw-rw-   0 root         (0) root         (0)     1309 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/limit.py
--rw-rw-rw-   0 root         (0) root         (0)     6072 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/mongo.py
--rw-rw-rw-   0 root         (0) root         (0)     1045 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/redis.py
--rw-rw-rw-   0 root         (0) root         (0)     1605 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/sendmail.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.248777 Flaskel-3.1.0rc2/flaskel/ext/sqlalchemy/
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/sqlalchemy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2402 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/sqlalchemy/model.py
--rw-rw-rw-   0 root         (0) root         (0)     1020 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/useragent.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.248777 Flaskel-3.1.0rc2/flaskel/ext/websocket/
--rw-rw-rw-   0 root         (0) root         (0)      526 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/ext/websocket/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.249777 Flaskel-3.1.0rc2/flaskel/extra/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/extra/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8963 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/extra/account.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.249777 Flaskel-3.1.0rc2/flaskel/extra/apidoc/
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/extra/apidoc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2515 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/extra/apidoc/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.250777 Flaskel-3.1.0rc2/flaskel/extra/media/
--rw-rw-rw-   0 root         (0) root         (0)      111 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/extra/media/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       82 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/extra/media/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2127 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/extra/media/repo.py
--rw-rw-rw-   0 root         (0) root         (0)     2214 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/extra/media/service.py
--rw-rw-rw-   0 root         (0) root         (0)     1144 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/extra/media/view.py
--rw-rw-rw-   0 root         (0) root         (0)    11414 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/extra/mobile_support.py
--rw-rw-rw-   0 root         (0) root         (0)     5218 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/extra/notification.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.250777 Flaskel-3.1.0rc2/flaskel/extra/payments/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/extra/payments/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.251777 Flaskel-3.1.0rc2/flaskel/extra/payments/stripe/
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/extra/payments/stripe/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3529 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/extra/payments/stripe/handler.py
--rw-rw-rw-   0 root         (0) root         (0)     2831 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/extra/payments/stripe/repo.py
--rw-rw-rw-   0 root         (0) root         (0)     1374 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/extra/payments/stripe/view.py
--rw-rw-rw-   0 root         (0) root         (0)     4678 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/flaskel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.251777 Flaskel-3.1.0rc2/flaskel/http/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/http/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2223 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/http/client.py
--rw-rw-rw-   0 root         (0) root         (0)     9019 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/http/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     7168 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/middlewares.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.252777 Flaskel-3.1.0rc2/flaskel/scripts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      253 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1425 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/init_app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.241777 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.253777 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/resources/
--rw-rw-rw-   0 root         (0) root         (0)      305 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/resources/Caddyfile.example
--rw-rw-rw-   0 root         (0) root         (0)      532 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/resources/conf.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2271 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/resources/log.yaml
--rw-rw-rw-   0 root         (0) root         (0)      757 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/resources/manage.sh
--rw-rw-rw-   0 root         (0) root         (0)      414 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/resources/nginx.example
--rw-rw-rw-   0 root         (0) root         (0)     1561 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/resources/nuisances.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1325 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/resources/schemas.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1775 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/resources/settings.ini.sample
--rw-rw-rw-   0 root         (0) root         (0)      492 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/resources/supervisor.example
--rw-rw-rw-   0 root         (0) root         (0)    14323 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/resources/swagger.yaml
--rw-rw-rw-   0 root         (0) root         (0)      139 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/resources/uwsgi.yaml.example
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.254777 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.254777 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/ext/
--rw-rw-rw-   0 root         (0) root         (0)     1768 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/ext/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      434 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/ext/auth.py
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/ext/database.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.254777 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/forms/
--rw-rw-rw-   0 root         (0) root         (0)      330 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/forms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.255777 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/models/
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      189 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/models/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.255777 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/scripts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      685 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/scripts/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      504 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/scripts/config.py
--rw-rw-rw-   0 root         (0) root         (0)      915 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/scripts/ws.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.255777 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/tasks/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      252 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.256777 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/
--rw-rw-rw-   0 root         (0) root         (0)      856 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1010 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/blueprints.py
--rw-rw-rw-   0 root         (0) root         (0)     1672 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.240777 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.256777 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/static/css/
--rw-rw-rw-   0 root         (0) root         (0)      190 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/static/css/main.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.256777 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/static/img/
--rw-rw-rw-   0 root         (0) root         (0)      318 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/static/img/favicon.ico
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.256777 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/static/js/
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/static/js/main.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.257777 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.257777 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/templates/core/
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/templates/core/error.html
--rw-rw-rw-   0 root         (0) root         (0)     1103 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/templates/core/head.html
--rw-rw-rw-   0 root         (0) root         (0)      655 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/templates/core/scripts.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.257777 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/templates/emails/
--rw-rw-rw-   0 root         (0) root         (0)      220 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/templates/emails/forgot.html
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/templates/emails/registration.html
--rw-rw-rw-   0 root         (0) root         (0)    13479 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/templates/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.258777 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/templates/layout/
--rw-rw-rw-   0 root         (0) root         (0)      458 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/templates/layout/base.html
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/templates/layout/container.html
--rw-rw-rw-   0 root         (0) root         (0)       20 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/templates/layout/footer.html
--rw-rw-rw-   0 root         (0) root         (0)       20 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/templates/layout/header.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.259777 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2433 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)      190 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/tests/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     2167 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/scripts/skeleton/tests/test_smoke.py
--rw-rw-rw-   0 root         (0) root         (0)     5319 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/standalone.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.259777 Flaskel-3.1.0rc2/flaskel/tester/
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/tester/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1432 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/tester/client.py
--rw-rw-rw-   0 root         (0) root         (0)     7354 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/tester/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.260777 Flaskel-3.1.0rc2/flaskel/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2551 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/utils/datastruct.py
--rw-rw-rw-   0 root         (0) root         (0)     3433 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/utils/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.261777 Flaskel-3.1.0rc2/flaskel/utils/schemas/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/utils/schemas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5018 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/utils/schemas/default.py
--rw-rw-rw-   0 root         (0) root         (0)    34444 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/utils/schemas/openapi3.py
--rw-rw-rw-   0 root         (0) root         (0)     1263 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/utils/validator.py
--rw-rw-rw-   0 root         (0) root         (0)     2765 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/utils/webargs.py
--rw-rw-rw-   0 root         (0) root         (0)      256 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.262777 Flaskel-3.1.0rc2/flaskel/views/
--rw-rw-rw-   0 root         (0) root         (0)      105 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7046 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/views/base.py
--rw-rw-rw-   0 root         (0) root         (0)     9130 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/views/proxy.py
--rw-rw-rw-   0 root         (0) root         (0)     7866 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/views/resource.py
--rw-rw-rw-   0 root         (0) root         (0)     5689 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/views/rpc.py
--rw-rw-rw-   0 root         (0) root         (0)     1210 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/views/static.py
--rw-rw-rw-   0 root         (0) root         (0)     1185 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/views/template.py
--rw-rw-rw-   0 root         (0) root         (0)     2820 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/views/token.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 21:39:53.263777 Flaskel-3.1.0rc2/flaskel/wsgi/
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/wsgi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      861 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/wsgi/base.py
--rw-rw-rw-   0 root         (0) root         (0)      790 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/wsgi/factory.py
--rw-rw-rw-   0 root         (0) root         (0)      584 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/wsgi/wsgi_gevent.py
--rw-rw-rw-   0 root         (0) root         (0)     4389 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/wsgi/wsgi_gunicorn.py
--rw-rw-rw-   0 root         (0) root         (0)      656 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/wsgi/wsgi_tornado.py
--rw-rw-rw-   0 root         (0) root         (0)      856 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/wsgi/wsgi_twisted.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/flaskel/wsgi/wsgi_waitress.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 21:39:53.264777 Flaskel-3.1.0rc2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     4611 2023-05-25 21:39:41.000000 Flaskel-3.1.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.035697 Flaskel-3.1.0rc3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.011697 Flaskel-3.1.0rc3/Flaskel.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15616 2023-06-05 00:39:52.000000 Flaskel-3.1.0rc3/Flaskel.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6189 2023-06-05 00:39:52.000000 Flaskel-3.1.0rc3/Flaskel.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 00:39:52.000000 Flaskel-3.1.0rc3/Flaskel.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-06-05 00:39:52.000000 Flaskel-3.1.0rc3/Flaskel.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 00:39:52.000000 Flaskel-3.1.0rc3/Flaskel.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      352 2023-06-05 00:39:52.000000 Flaskel-3.1.0rc3/Flaskel.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-05 00:39:52.000000 Flaskel-3.1.0rc3/Flaskel.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      146 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    15616 2023-06-05 00:39:53.035697 Flaskel-3.1.0rc3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    14795 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.013697 Flaskel-3.1.0rc3/flaskel/
+-rw-rw-rw-   0 root         (0) root         (0)      709 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12101 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/builder.py
+-rw-rw-rw-   0 root         (0) root         (0)     9072 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1188 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/converters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.014697 Flaskel-3.1.0rc3/flaskel/ext/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7359 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     4245 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/caching.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.014697 Flaskel-3.1.0rc3/flaskel/ext/cloudflare/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/cloudflare/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4239 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/cloudflare/remote.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.015697 Flaskel-3.1.0rc3/flaskel/ext/crypto/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/crypto/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1710 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/crypto/argon.py
+-rw-rw-rw-   0 root         (0) root         (0)      818 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/datetime.py
+-rw-rw-rw-   0 root         (0) root         (0)     1200 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.015697 Flaskel-3.1.0rc3/flaskel/ext/errors/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/errors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1954 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/errors/dispatchers.py
+-rw-rw-rw-   0 root         (0) root         (0)     4349 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/errors/exception.py
+-rw-rw-rw-   0 root         (0) root         (0)     7822 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/errors/handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     4499 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/errors/normalize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.016697 Flaskel-3.1.0rc3/flaskel/ext/healthcheck/
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/healthcheck/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6601 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/healthcheck/checkers.py
+-rw-rw-rw-   0 root         (0) root         (0)     4889 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/healthcheck/health.py
+-rw-rw-rw-   0 root         (0) root         (0)     7775 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/ipban.py
+-rw-rw-rw-   0 root         (0) root         (0)     5351 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/jobs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1309 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/limit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.016697 Flaskel-3.1.0rc3/flaskel/ext/logging/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/logging/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.017697 Flaskel-3.1.0rc3/flaskel/ext/logging/builders/
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/logging/builders/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1744 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/logging/builders/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2993 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/logging/builders/json.py
+-rw-rw-rw-   0 root         (0) root         (0)     2864 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/logging/builders/text.py
+-rw-rw-rw-   0 root         (0) root         (0)      951 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/logging/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1357 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/logging/formatters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1795 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/logging/handlers.py
+-rw-rw-rw-   0 root         (0) root         (0)     4279 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/logging/logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     6005 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/mongo.py
+-rw-rw-rw-   0 root         (0) root         (0)      978 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/redis.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.018697 Flaskel-3.1.0rc3/flaskel/ext/response/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/response/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7380 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/response/builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.019697 Flaskel-3.1.0rc3/flaskel/ext/response/builders/
+-rw-rw-rw-   0 root         (0) root         (0)      180 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/response/builders/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      768 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/response/builders/base64.py
+-rw-rw-rw-   0 root         (0) root         (0)     1845 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/response/builders/builder.py
+-rw-rw-rw-   0 root         (0) root         (0)     1973 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/response/builders/csv.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/response/builders/html.py
+-rw-rw-rw-   0 root         (0) root         (0)     1750 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/response/builders/json.py
+-rw-rw-rw-   0 root         (0) root         (0)      740 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/response/builders/xml.py
+-rw-rw-rw-   0 root         (0) root         (0)      906 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/response/builders/yaml.py
+-rw-rw-rw-   0 root         (0) root         (0)     1648 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/response/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1490 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/response/dictutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1538 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/sendmail.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.019697 Flaskel-3.1.0rc3/flaskel/ext/sqlalchemy/
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/sqlalchemy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2414 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/sqlalchemy/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.019697 Flaskel-3.1.0rc3/flaskel/ext/templating/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/templating/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      367 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/templating/default.py
+-rw-rw-rw-   0 root         (0) root         (0)     1646 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/templating/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/templating/functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2067 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/templating/support.py
+-rw-rw-rw-   0 root         (0) root         (0)      953 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/useragent.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.020697 Flaskel-3.1.0rc3/flaskel/ext/websocket/
+-rw-rw-rw-   0 root         (0) root         (0)      526 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/ext/websocket/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.020697 Flaskel-3.1.0rc3/flaskel/extra/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/extra/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8975 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/extra/account.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.020697 Flaskel-3.1.0rc3/flaskel/extra/apidoc/
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/extra/apidoc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2521 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/extra/apidoc/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.021697 Flaskel-3.1.0rc3/flaskel/extra/media/
+-rw-rw-rw-   0 root         (0) root         (0)      111 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/extra/media/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       82 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/extra/media/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2127 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/extra/media/repo.py
+-rw-rw-rw-   0 root         (0) root         (0)     2214 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/extra/media/service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1144 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/extra/media/view.py
+-rw-rw-rw-   0 root         (0) root         (0)    11461 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/extra/mobile_support.py
+-rw-rw-rw-   0 root         (0) root         (0)     5218 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/extra/notification.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.021697 Flaskel-3.1.0rc3/flaskel/extra/payments/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/extra/payments/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.022697 Flaskel-3.1.0rc3/flaskel/extra/payments/stripe/
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/extra/payments/stripe/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3498 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/extra/payments/stripe/handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     2831 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/extra/payments/stripe/repo.py
+-rw-rw-rw-   0 root         (0) root         (0)     1374 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/extra/payments/stripe/view.py
+-rw-rw-rw-   0 root         (0) root         (0)     4943 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/flaskel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.022697 Flaskel-3.1.0rc3/flaskel/http/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/http/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2223 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/http/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     9008 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/http/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7220 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/middlewares.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.023697 Flaskel-3.1.0rc3/flaskel/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1425 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/init_app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.010697 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.024697 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/resources/
+-rw-rw-rw-   0 root         (0) root         (0)      305 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/resources/Caddyfile.example
+-rw-rw-rw-   0 root         (0) root         (0)      532 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/resources/conf.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2271 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/resources/log.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      757 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/resources/manage.sh
+-rw-rw-rw-   0 root         (0) root         (0)      414 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/resources/nginx.example
+-rw-rw-rw-   0 root         (0) root         (0)     1561 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/resources/nuisances.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1325 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/resources/schemas.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1775 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/resources/settings.ini.sample
+-rw-rw-rw-   0 root         (0) root         (0)      492 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/resources/supervisor.example
+-rw-rw-rw-   0 root         (0) root         (0)    14323 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/resources/swagger.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      139 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/resources/uwsgi.yaml.example
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.024697 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.025697 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/ext/
+-rw-rw-rw-   0 root         (0) root         (0)     1768 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/ext/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      434 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/ext/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/ext/database.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.025697 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/forms/
+-rw-rw-rw-   0 root         (0) root         (0)      330 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/forms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.025697 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/models/
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      189 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/models/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.026697 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      685 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/scripts/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      504 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/scripts/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      915 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/scripts/ws.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.026697 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.026697 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/
+-rw-rw-rw-   0 root         (0) root         (0)      856 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1010 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/blueprints.py
+-rw-rw-rw-   0 root         (0) root         (0)     1672 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.009697 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.026697 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/static/css/
+-rw-rw-rw-   0 root         (0) root         (0)      190 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/static/css/main.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.027697 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/static/img/
+-rw-rw-rw-   0 root         (0) root         (0)      318 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/static/img/favicon.ico
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.027697 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/static/js/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/static/js/main.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.027697 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.027697 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/templates/core/
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/templates/core/error.html
+-rw-rw-rw-   0 root         (0) root         (0)     1103 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/templates/core/head.html
+-rw-rw-rw-   0 root         (0) root         (0)      655 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/templates/core/scripts.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.028697 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/templates/emails/
+-rw-rw-rw-   0 root         (0) root         (0)      220 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/templates/emails/forgot.html
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/templates/emails/registration.html
+-rw-rw-rw-   0 root         (0) root         (0)    13479 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/templates/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.028697 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/templates/layout/
+-rw-rw-rw-   0 root         (0) root         (0)      458 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/templates/layout/base.html
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/templates/layout/container.html
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/templates/layout/footer.html
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/templates/layout/header.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.029697 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2434 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)      190 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/tests/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2180 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/scripts/skeleton/tests/test_smoke.py
+-rw-rw-rw-   0 root         (0) root         (0)     5361 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/standalone.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.029697 Flaskel-3.1.0rc3/flaskel/tester/
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/tester/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1432 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/tester/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     7428 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/tester/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.030697 Flaskel-3.1.0rc3/flaskel/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2551 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/utils/datastruct.py
+-rw-rw-rw-   0 root         (0) root         (0)     3513 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/utils/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.030697 Flaskel-3.1.0rc3/flaskel/utils/schemas/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/utils/schemas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5018 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/utils/schemas/default.py
+-rw-rw-rw-   0 root         (0) root         (0)    34444 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/utils/schemas/openapi3.py
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/utils/validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     2812 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/utils/webargs.py
+-rw-rw-rw-   0 root         (0) root         (0)      256 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.031697 Flaskel-3.1.0rc3/flaskel/views/
+-rw-rw-rw-   0 root         (0) root         (0)      105 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7046 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/views/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     9148 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/views/proxy.py
+-rw-rw-rw-   0 root         (0) root         (0)     7866 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/views/resource.py
+-rw-rw-rw-   0 root         (0) root         (0)     5689 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/views/rpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1210 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/views/static.py
+-rw-rw-rw-   0 root         (0) root         (0)     1185 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/views/template.py
+-rw-rw-rw-   0 root         (0) root         (0)     2826 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/views/token.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.032697 Flaskel-3.1.0rc3/flaskel/wsgi/
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/wsgi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      861 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/wsgi/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      790 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/wsgi/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)      584 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/wsgi/wsgi_gevent.py
+-rw-rw-rw-   0 root         (0) root         (0)     4389 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/wsgi/wsgi_gunicorn.py
+-rw-rw-rw-   0 root         (0) root         (0)      656 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/wsgi/wsgi_tornado.py
+-rw-rw-rw-   0 root         (0) root         (0)      856 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/wsgi/wsgi_twisted.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/flaskel/wsgi/wsgi_waitress.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:39:53.034697 Flaskel-3.1.0rc3/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)       93 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/requirements/requirements-all.in
+-rw-rw-rw-   0 root         (0) root         (0)    10050 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/requirements/requirements-all.txt
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/requirements/requirements-build.in
+-rw-rw-rw-   0 root         (0) root         (0)     3256 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/requirements/requirements-build.txt
+-rw-rw-rw-   0 root         (0) root         (0)      413 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/requirements/requirements-dev.in
+-rw-rw-rw-   0 root         (0) root         (0)     6727 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/requirements/requirements-dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)      139 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/requirements/requirements-extra.in
+-rw-rw-rw-   0 root         (0) root         (0)     3155 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/requirements/requirements-extra.txt
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/requirements/requirements-test.in
+-rw-rw-rw-   0 root         (0) root         (0)     1417 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/requirements/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/requirements/requirements-wsgi.in
+-rw-rw-rw-   0 root         (0) root         (0)     1141 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/requirements/requirements-wsgi.txt
+-rw-rw-rw-   0 root         (0) root         (0)      182 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/requirements/requirements.in
+-rw-rw-rw-   0 root         (0) root         (0)     4329 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/requirements/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 00:39:53.035697 Flaskel-3.1.0rc3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4682 2023-06-05 00:39:41.000000 Flaskel-3.1.0rc3/setup.py
```

### Comparing `Flaskel-3.1.0rc2/Flaskel.egg-info/PKG-INFO` & `Flaskel-3.1.0rc3/Flaskel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flaskel
-Version: 3.1.0rc2
+Version: 3.1.0rc3
 Summary: Skeleton for flask applications
 Home-page: https://github.com/cs91chris/flaskel
 Author: cs91chris
 Author-email: cs91chris@voidbrain.me
 License: MIT
 Platform: any
 Classifier: Environment :: Web Environment
```

### Comparing `Flaskel-3.1.0rc2/PKG-INFO` & `Flaskel-3.1.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flaskel
-Version: 3.1.0rc2
+Version: 3.1.0rc3
 Summary: Skeleton for flask applications
 Home-page: https://github.com/cs91chris/flaskel
 Author: cs91chris
 Author-email: cs91chris@voidbrain.me
 License: MIT
 Platform: any
 Classifier: Environment :: Web Environment
```

### Comparing `Flaskel-3.1.0rc2/README.md` & `Flaskel-3.1.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/__init__.py` & `Flaskel-3.1.0rc3/flaskel/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 from .version import *  # noqa: F403
 from .wsgi import BaseApplication, WSGIFactory
 
 client_redis = ExtProxy("redis")
 client_mail = ExtProxy("client_mail")
 job_scheduler = ExtProxy("scheduler")
 client_mongo = ExtProxy("mongo.default.db")
-db_session = ExtProxy("sqlalchemy.db.session")
+db_session = ExtProxy("sqlalchemy.session")
```

### Comparing `Flaskel-3.1.0rc2/flaskel/builder.py` & `Flaskel-3.1.0rc3/flaskel/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 import typing as t
 
 from flask import Blueprint
 from flask.typing import AfterRequestCallable, BeforeRequestCallable
 from jinja2 import ChoiceLoader, FileSystemLoader
 from vbcore.db.support import SQLASupport
-from vbcore.misc import random_string
+from vbcore.stringutils.misc import random_string
 from werkzeug.middleware.lint import LintMiddleware
 from werkzeug.middleware.profiler import ProfilerMiddleware
 from werkzeug.routing import BaseConverter
 
 from flaskel import config, flaskel
 
 from .converters import CONVERTERS
@@ -136,15 +136,15 @@
             else:
                 secret_key = self.load_secret_key(self.secret_file)
                 secret_key = secret_key or self.generate_secret_key(
                     self.secret_file, key_length
                 )
         elif not self._app.config.SECRET_KEY:
             self._app.logger.debug("set secret key in development mode")
-            secret_key = "fake_very_complex_string"
+            secret_key = "fake_very_complex_string"  # nosec
 
         self._app.config.SECRET_KEY = secret_key or self._app.config.SECRET_KEY
         if len(secret_key) < key_length:
             self._app.logger.warning("secret key length is less than: %s", key_length)
 
         if not self._app.config.JWT_SECRET_KEY:
             self._app.config.JWT_SECRET_KEY = self._app.config.SECRET_KEY
@@ -162,30 +162,29 @@
     @staticmethod
     def normalize_tuple(tokens: t.Union[t.Any, tuple]) -> t.Tuple[t.Any, t.Dict]:
         if not isinstance(tokens, tuple):
             return tokens, {}
         return tokens[0], tokens[1] if len(tokens) > 1 else {}
 
     def register_extensions(self):
-        with self._app.app_context():
-            for name, e in self._extensions.items():
-                try:
-                    ext, opt = self.normalize_tuple(e)
-                    if not ext:
-                        raise TypeError("extension could not be None or empty")
-                except (TypeError, IndexError) as exc:
-                    self._app.logger.warning(
-                        "Invalid extension '%s' configuration '%s': %s", name, e, exc
-                    )
-                    continue
-
-                ext.init_app(self._app, **opt)
-                self._app.logger.debug(
-                    "Registered extension '%s' with options: %s", name, opt
+        for name, e in self._extensions.items():
+            try:
+                ext, opt = self.normalize_tuple(e)
+                if not ext:
+                    raise TypeError("extension could not be None or empty")
+            except (TypeError, IndexError) as exc:
+                self._app.logger.warning(
+                    "Invalid extension '%s' configuration '%s': %s", name, e, exc
                 )
+                continue
+
+            ext.init_app(self._app, **opt)
+            self._app.logger.debug(
+                "Registered extension '%s' with options: %s", name, opt
+            )
 
         self._app.logger.debug("Dump flask extensions:")
         for k, v in self._app.extensions.items():
             self._app.logger.debug("Registered extension '%s': %s", k, v)
 
     def register_blueprints(self):
         for b in self._blueprints:
@@ -276,43 +275,43 @@
         if self._app is not None:
             self._app.logger.debug("Registered routes:\n%s", DumpUrls(self._app))
 
     def init_db(self):
         try:
             sqlalchemy = self._app.extensions.get("sqlalchemy")
             if sqlalchemy is not None:
-                SQLASupport.register_custom_handlers(sqlalchemy.db.engine)
-                sqlalchemy.db.create_all()
+                SQLASupport.register_custom_handlers(sqlalchemy.engine)
+                sqlalchemy.create_all()
         except Exception as exc:  # pylint: disable=broad-except
             self._app.logger.exception(exc)
 
     def after_create_hook(self):
         self.dump_urls()
 
         if self._app.debug:
             self.set_linter_and_profiler()
 
-        with self._app.app_context():
-            self.init_db()
-            if callable(self._after_create_callback):
-                self._after_create_callback()
+        self.init_db()
+        if callable(self._after_create_callback):
+            self._after_create_callback()
 
     def create(
         self, conf: t.Optional[t.Union[str, t.Dict[str, t.Any]]] = None
     ) -> Flaskel:
         self._app = self._app or self.flask_class(self.app_name, **self._options)
         self._app.version = self._version
 
         self.set_config(conf)
         self.set_secret_key()
 
-        self.register_extensions()
-        self.register_middlewares()
-        self.register_template_folders()
-        self.register_converters()
-        self.register_views()
-        self.register_blueprints()
-        self.register_after_request()
-        self.register_before_request()
+        with self._app.app_context():
+            self.register_extensions()
+            self.register_middlewares()
+            self.register_template_folders()
+            self.register_converters()
+            self.register_views()
+            self.register_blueprints()
+            self.register_after_request()
+            self.register_before_request()
+            self.after_create_hook()
 
-        self.after_create_hook()
         return self._app
```

### Comparing `Flaskel-3.1.0rc2/flaskel/config.py` & `Flaskel-3.1.0rc3/flaskel/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 TEMPLATES_AUTO_RELOAD = config("TEMPLATES_AUTO_RELOAD", default=DEBUG, cast=bool)
 EXPLAIN_TEMPLATE_LOADING = config("EXPLAIN_TEMPLATE_LOADING", default=False, cast=bool)
 APIDOCS_ENABLED = config("APIDOCS_ENABLED", default=True, cast=bool)
 CONF_PATH = config("CONF_PATH", default=os.path.join(config.search_path, "resources"))
 
 JWT_DEFAULT_SCOPE = None
 JWT_IDENTITY_CLAIM = "identity"
-JWT_DEFAULT_TOKEN_TYPE = "bearer"
+JWT_DEFAULT_TOKEN_TYPE = "bearer"  # nosec
 JWT_ERROR_MESSAGE_KEY = "message"
 JWT_QUERY_STRING_NAME = "token"
 JWT_TOKEN_LOCATION = ["headers", "query_string"]
 JWT_ALGORITHM = config("JWT_ALGORITHM", default="HS512")
 JWT_DECODE_ALGORITHMS = config(
     "JWT_ALGORITHM", default=JWT_ALGORITHM, cast=decouple.Csv()
 )
@@ -160,15 +160,15 @@
 RATELIMIT_HEADERS_ENABLED = config("RATELIMIT_HEADERS_ENABLED", default=True, cast=bool)
 RATELIMIT_IN_MEMORY_FALLBACK_ENABLED = config(
     "RATELIMIT_IN_MEMORY_FALLBACK_ENABLED", default=True, cast=bool
 )
 
 DATABASE_URL = SQLALCHEMY_DATABASE_URI
 ERROR_PAGE = "core/error.html"
-SECRET_KEY_FILE_NAME = ".secret.key"
+SECRET_KEY_FILE_NAME = ".secret.key"  # nosec
 SECRET_KEY_MIN_LENGTH = 256
 RB_DEFAULT_ACCEPTABLE_MIMETYPES = [
     ContentTypeEnum.JSON,
 ]
 
 PRETTY_DATE = "%d %B %Y %I:%M %p"
 DATE_ISO_FORMAT = "%Y-%m-%dT%H:%M:%S"
```

### Comparing `Flaskel-3.1.0rc2/flaskel/converters.py` & `Flaskel-3.1.0rc3/flaskel/converters.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/ext/auth.py` & `Flaskel-3.1.0rc3/flaskel/ext/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,21 +28,21 @@
 
 @basic_auth.verify_password
 def simple_basic_auth(username: str, password: str) -> t.Optional[dict]:
     if (
         username == cap.config.BASIC_AUTH_USERNAME
         and password == cap.config.BASIC_AUTH_PASSWORD
     ):
-        return dict(username=username, password=password)
+        return {"username": username, "password": password}
     return None
 
 
 @token_auth.invalid_token_loader
 def invalid_token_loader(mess) -> t.Tuple[dict, int]:
-    return dict(message=mess), httpcode.UNAUTHORIZED
+    return {"message": mess}, httpcode.UNAUTHORIZED
 
 
 class RevokedTokenMixin(StandardMixin):
     jti = sa.Column(sa.String(120), nullable=False, unique=True)
 
     def __repr__(self):
         return f"<RevokedToken: {self.id} - {self.jti}>"
@@ -70,15 +70,15 @@
     access_token: str
     expires_in: int
     issued_at: int
     token_type: str
     scope: t.Optional[str] = None
     refresh_token: t.Optional[str] = None
 
-    def to_dict(self, **kwargs) -> ObjectDict:
+    def to_dict(self, *_, **kwargs) -> ObjectDict:
         data = ObjectDict(
             access_token=self.access_token,
             expires_in=self.expires_in,
             issued_at=self.issued_at,
             token_type=self.token_type,
             scope=self.scope,
             **kwargs,
@@ -86,15 +86,16 @@
         if self.refresh_token:
             data.refresh_token = self.refresh_token
         return data
 
 
 class BaseTokenHandler:
     def __init__(self, blocklist_loader: t.Optional[t.Callable] = None):
-        token_auth.token_in_blocklist_loader(blocklist_loader)
+        if blocklist_loader:
+            token_auth.token_in_blocklist_loader(blocklist_loader)
 
     def check_token_block_listed(self, jwt_headers, jwt_data) -> bool:
         _ = jwt_headers, jwt_data
         return False
 
     def revoke(self, token: t.Optional[str] = None):
         """can be implemented by subclass"""
```

### Comparing `Flaskel-3.1.0rc2/flaskel/ext/caching.py` & `Flaskel-3.1.0rc3/flaskel/ext/caching.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/ext/crypto/argon.py` & `Flaskel-3.1.0rc3/flaskel/ext/crypto/argon.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,12 +35,11 @@
         app.config.setdefault(f"{cls.CONFIG_PREFIX}SALT_LEN", params.salt_len)
 
     def init_app(self, app, argon_class: t.Type[HasherArgon2] = HasherArgon2):
         self.set_default_config(app)
         self._argon = argon_class(
             Argon2Options(**app.config.get_namespace(self.CONFIG_PREFIX))
         )
-        setattr(app, "extensions", getattr(app, "extensions", {}))
         app.extensions["argon2"] = self
 
     def __getattr__(self, item):
         return getattr(self._argon, item)
```

### Comparing `Flaskel-3.1.0rc2/flaskel/ext/datetime.py` & `Flaskel-3.1.0rc3/flaskel/ext/datetime.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,12 +15,11 @@
         app.config.setdefault("DATE_HELPER_STATE", None)
         app.config.setdefault("DATE_PRETTY", DateTimeFmt.PRETTY)
         app.config.setdefault("DATE_ISO_FORMAT", DateTimeFmt.ISO)
 
         self._helper = helper
         self.iso_format = app.config.DATE_ISO_FORMAT
 
-        setattr(app, "extensions", getattr(app, "extensions", {}))
         app.extensions["date_helper"] = self
 
     def __getattr__(self, name):
         return getattr(self._helper, name)
```

### Comparing `Flaskel-3.1.0rc2/flaskel/ext/default.py` & `Flaskel-3.1.0rc3/flaskel/ext/default.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 import functools
 import typing as t
 
-from flask_cloudflare_remote import CloudflareRemote
 from flask_cors import CORS
-from flask_errors_handler import ErrorHandler
-from flask_logify import FlaskLogging
-from flask_response_builder import ResponseBuilder
 from flask_sqlalchemy import SQLAlchemy
-from flask_template_support import TemplateSupport
 
 from .caching import Caching
+from .cloudflare.remote import CloudflareRemote
 from .crypto.argon import Argon2
 from .datetime import FlaskDateHelper
-from .errors import ErrorNormalizer
+from .errors.handler import ErrorHandler
 from .healthcheck import HealthCheck
 from .jobs import APJobs
+from .logging.logging import FlaskLogging
+from .response.builder import ResponseBuilder
 from .sqlalchemy import SQLAModel
+from .templating.support import TemplateSupport
 from .useragent import UserAgent
 
 cors: CORS = CORS()
 logger: FlaskLogging = FlaskLogging()
 builder: ResponseBuilder = ResponseBuilder()
 template: TemplateSupport = TemplateSupport()
 cfremote: CloudflareRemote = CloudflareRemote()
-error_handler: ErrorHandler = ErrorHandler(normalizer=ErrorNormalizer())
+error_handler: ErrorHandler = ErrorHandler()
 
 argon2: Argon2 = Argon2()
 caching: Caching = Caching()
 useragent: UserAgent = UserAgent()
 health_checks: HealthCheck = HealthCheck()
 date_helper: FlaskDateHelper = FlaskDateHelper()
```

### Comparing `Flaskel-3.1.0rc2/flaskel/ext/healthcheck/checkers.py` & `Flaskel-3.1.0rc3/flaskel/ext/healthcheck/checkers.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/ext/healthcheck/health.py` & `Flaskel-3.1.0rc3/flaskel/ext/healthcheck/health.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,14 @@
         self.app = app
         self._executor = executor or self._executor
 
         self.set_default_config()
         self.register_checkers(checkers)
         self.register_route(blueprint or app, decorators)
 
-        setattr(app, "extensions", getattr(app, "extensions", {}))
         app.extensions["healthcheck"] = self
 
     def set_default_config(self):
         self.app.config.setdefault("HEALTHCHECK_ABOUT_LINK", None)
         self.app.config.setdefault("HEALTHCHECK_VIEW_NAME", "healthcheck")
         self.app.config.setdefault("HEALTHCHECK_PATH", "/healthcheck")
         self.app.config.setdefault("HEALTHCHECK_PARAM_KEY", "checks")
@@ -99,15 +98,15 @@
             all_checkers
             if not only_checkers
             else set(only_checkers).intersection(all_checkers)
         )
 
     def execute(self) -> t.Tuple[t.List[str], t.List[CheckerResponseType]]:
         checkers = self.get_checkers()
-        tasks = [(self._checkers.get(c), dict(app=self.app)) for c in checkers]
+        tasks = [(self._checkers.get(c), {"app": self.app}) for c in checkers]
         return checkers, self._executor(tasks=tasks).run()
 
     def perform(self) -> t.Tuple[dict, int, dict]:
         healthy = True
         response: t.Dict[str, t.Any] = {
             "status": CheckStatus.PASS,
             "checks": {},
```

### Comparing `Flaskel-3.1.0rc2/flaskel/ext/ipban.py` & `Flaskel-3.1.0rc3/flaskel/ext/ipban.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,15 +191,14 @@
             app.after_request(self.after_request_hook)
             app.before_request(self.before_request_hook)
             self.service = self.service_factory(service_class, app.config)
             self.service.load_whitelist(
                 ip=app.config.IPBAN_IP_WHITELIST, net=app.config.IPBAN_NET_WHITELIST
             )
 
-        setattr(app, "extensions", getattr(app, "extensions", {}))
         app.extensions["ipban"] = self
 
     def service_factory(self, service_class: t.Type[IpBanService], config):
         return service_class(
             self.backends[config.IPBAN_BACKEND],
             max_attempts=config.IPBAN_COUNT,
             default_ttl=config.IPBAN_SECONDS,
```

### Comparing `Flaskel-3.1.0rc2/flaskel/ext/jobs.py` & `Flaskel-3.1.0rc3/flaskel/ext/jobs.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,16 +32,14 @@
 
         if APScheduler is object:
             raise ImportError(
                 "you must install 'flask_apscheduler'"
             )  # pragma: no cover
 
         self.set_config(app)
-
-        setattr(app, "extensions", getattr(app, "extensions", {}))
         app.extensions["scheduler"] = self
 
         if app.config.SCHEDULER_PATCH_MULTITHREAD is True:
             if fcntl is None:  # pragma: no cover
                 app.logger.warning(
                     "fcntl not supported on this platform, no locking mechanism used"
                 )
```

### Comparing `Flaskel-3.1.0rc2/flaskel/ext/limit.py` & `Flaskel-3.1.0rc3/flaskel/ext/limit.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/ext/mongo.py` & `Flaskel-3.1.0rc3/flaskel/ext/mongo.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from flaskel.utils.datastruct import Pagination
 
 
 class FlaskMongoDB(PyMongo):
     def init_app(self, app, *args, ext_name: str = "default", **kwargs):
         self.set_default_config(app, **kwargs)
         super().init_app(app, *args, **app.config.MONGO_OPTS)
-        setattr(app, "extensions", getattr(app, "extensions", {}))
         app.extensions["mongo"] = ObjectDict()
         app.extensions["mongo"][ext_name] = self
 
     @classmethod
     def set_default_config(cls, app, **kwargs):
         app.config.setdefault("MONGO_URI", "mongodb://localhost")
         app.config.setdefault("MONGO_OPTS", {})
```

### Comparing `Flaskel-3.1.0rc2/flaskel/ext/redis.py` & `Flaskel-3.1.0rc3/flaskel/ext/redis.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,12 +21,11 @@
         app.config["REDIS_OPTS"].update(**kwargs)
 
         if not self._client:
             self._client = redis_class.from_url(
                 app.config["REDIS_URL"], **app.config["REDIS_OPTS"]
             )
 
-        setattr(app, "extensions", getattr(app, "extensions", {}))
         app.extensions["redis"] = self
 
     def __getattr__(self, name):
         return getattr(self.client, name)
```

### Comparing `Flaskel-3.1.0rc2/flaskel/ext/sendmail.py` & `Flaskel-3.1.0rc3/flaskel/ext/sendmail.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 AddressType = t.Union[str, t.Tuple[str, str]]
 
 
 class ClientMail(Mail):
     def init_app(self, app):
         self.app = app
         super().init_app(app)
-        setattr(app, "extensions", getattr(app, "extensions", {}))
         app.extensions["client_mail"] = self
 
     def sendmail(
         self,
         subject: str,
         html: t.Optional[str] = None,
         body: t.Optional[str] = None,
```

### Comparing `Flaskel-3.1.0rc2/flaskel/ext/sqlalchemy/model.py` & `Flaskel-3.1.0rc3/flaskel/ext/sqlalchemy/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import typing as t
 
-from flask_sqlalchemy import Model
+from flask_sqlalchemy.model import Model
 from vbcore.datastruct import ObjectDict
 
 
 class SQLAModel(Model):
     __table__ = None
 
     def columns(self) -> t.List[str]:
@@ -12,20 +12,20 @@
             return list(self.__table__.columns.keys())
         return []
 
     @classmethod
     def get_one(
         cls, *args, raise_not_found: bool = True, to_dict: bool = True, **kwargs
     ):
-        res = cls.query.filter(*args).filter_by(**kwargs)
+        query = cls.query.filter(*args).filter_by(**kwargs)
 
         if raise_not_found:
-            res = res.first_or_404()
+            res = query.first_or_404()
         else:
-            res = res.first()
+            res = query.first()
             if res is None:
                 return None
 
         if to_dict is True:
             return res.to_dict()
         return res
```

### Comparing `Flaskel-3.1.0rc2/flaskel/ext/useragent.py` & `Flaskel-3.1.0rc3/flaskel/ext/useragent.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,14 @@
         if app is not None:
             self.init_app(app, **kwargs)
 
     def init_app(self, app, parser_class=UserAgentParser):
         self._parser = parser_class
         app.config.setdefault("USER_AGENT_AUTO_PARSE", False)
 
-        setattr(app, "extensions", getattr(app, "extensions", {}))
         app.extensions["useragent"] = self
 
         app.before_request_funcs.setdefault(None, []).append(
             partial(self.before_request_hook, app)
         )
 
     def before_request_hook(self, app):
```

### Comparing `Flaskel-3.1.0rc2/flaskel/ext/websocket/__init__.py` & `Flaskel-3.1.0rc3/flaskel/ext/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/extra/account.py` & `Flaskel-3.1.0rc3/flaskel/extra/account.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from flask import render_template
 from sqlalchemy.exc import SQLAlchemyError
 from vbcore.datastruct import ObjectDict
 from vbcore.db.exceptions import DBDuplicateEntry
 from vbcore.db.mixins import StandardMixin, UserMixin
 from vbcore.http import httpcode, HttpMethod
 from vbcore.jsonschema.support import Fields
-from vbcore.misc import random_string
+from vbcore.stringutils.misc import random_string
 
 from flaskel import (
     abort,
     cap,
     client_mail,
     client_redis,
     db_session,
```

### Comparing `Flaskel-3.1.0rc2/flaskel/extra/apidoc/template.py` & `Flaskel-3.1.0rc3/flaskel/extra/apidoc/template.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 </html>"""
 
     def service(self, *_, **__) -> dict:
         if not cap.config.APIDOCS_ENABLED:
             return abort(httpcode.NOT_FOUND)
 
         proto = cap.config.PREFERRED_URL_SCHEME
-        return dict(
+        return ObjectDict(
             rapidoc_version=cap.config.RAPIDOC_VERSION or "9",
             rapidoc_theme=cap.config.RAPIDOC_THEME or "dark",
             page_title=f"{cap.config.APP_NAME} - API DOCS",
             spec_url=url_for(self.apispec_view, _external=True, _scheme=proto),
         )
```

### Comparing `Flaskel-3.1.0rc2/flaskel/extra/media/repo.py` & `Flaskel-3.1.0rc3/flaskel/extra/media/repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,16 @@
     filename = sa.Column(sa.String(255))
 
     def to_dict(self, *_, **__):
         return ObjectDict(id=self.id, link=self.link)
 
 
 class MediaRepo:
-    entity_model = None
-    media_model = None
+    entity_model: t.Any
+    media_model: t.Any
     session = db_session
 
     @classmethod
     def entity_name(cls) -> t.Optional[str]:
         if cls.entity_model:
             return cls.entity_model.__tablename__
         return None
```

### Comparing `Flaskel-3.1.0rc2/flaskel/extra/media/service.py` & `Flaskel-3.1.0rc3/flaskel/extra/media/service.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/extra/media/view.py` & `Flaskel-3.1.0rc3/flaskel/extra/media/view.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/extra/mobile_support.py` & `Flaskel-3.1.0rc3/flaskel/extra/mobile_support.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 import typing as t
 from datetime import datetime
 
 import flask
 from packaging import version
+from vbcore.datastruct import ObjectDict
 from vbcore.http import httpcode, HttpMethod
 from vbcore.http.headers import ContentTypeEnum, HeaderEnum
 
 from flaskel import abort, cap, ExtProxy, Flaskel, request, Response, webargs
 from flaskel.ext.default import builder
 from flaskel.ext.limit import RateLimit
 from flaskel.views import BaseView
@@ -215,15 +216,15 @@
     default_view_name = "mobile_release"
     default_urls = (
         "/mobile/release",
         "/mobile/release/<ver>",
     )
 
     @webargs.query(
-        dict(
+        ObjectDict(
             all=webargs.OptField.boolean(),
             critical=webargs.OptField.boolean(),
             agent=webargs.Field.string(required=True),
         )
     )
     def dispatch_request(self, params: dict, *_, ver=None, **__):
         agent = params["agent"]
```

### Comparing `Flaskel-3.1.0rc2/flaskel/extra/notification.py` & `Flaskel-3.1.0rc3/flaskel/extra/notification.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/extra/payments/stripe/handler.py` & `Flaskel-3.1.0rc3/flaskel/extra/payments/stripe/handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,30 +24,31 @@
 
     @staticmethod
     def _not_registered(callback_type: str, *_):
         cap.logger.warning("no callback registered for: %s", callback_type)
 
     @staticmethod
     def check_prerequisites(app):
-        assert app.config.STRIPE_SECRET_KEY is not None, "missing STRIPE_SECRET_KEY"
-        assert app.config.STRIPE_PUBLIC_KEY is not None, "missing STRIPE_PUBLIC_KEY"
+        if not app.config.STRIPE_SECRET_KEY:
+            raise ValueError("missing STRIPE_SECRET_KEY")
+        if not app.config.STRIPE_PUBLIC_KEY:
+            raise ValueError("missing STRIPE_PUBLIC_KEY")
 
     def init_app(self, app, name: t.Optional[str] = None, **kwargs):
         self.check_prerequisites(app)
         app.config.setdefault("STRIPE_DEBUG", False)
         app.config.setdefault("STRIPE_DEFAULT_CURRENCY", "eur")
         app.config.setdefault("STRIPE_API_VERSION", "2020-08-27")
 
         self.handler.enable_telemetry = False
         self.handler.api_key = app.config.STRIPE_SECRET_KEY
         self.handler.api_version = app.config.STRIPE_API_VERSION
         self.handler.log = "debug" if app.config.STRIPE_DEBUG else "info"
         self.handler.set_app_info(name or app.config.APP_NAME, **kwargs)
 
-        setattr(app, "extensions", getattr(app, "extensions", {}))
         app.extensions["stripe"] = self
 
     @staticmethod
     def prepare_amount(value):
         return int(value * 100)
 
     def create_payment_intent(
```

### Comparing `Flaskel-3.1.0rc2/flaskel/extra/payments/stripe/repo.py` & `Flaskel-3.1.0rc3/flaskel/extra/payments/stripe/repo.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/extra/payments/stripe/view.py` & `Flaskel-3.1.0rc3/flaskel/extra/payments/stripe/view.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/flaskel.py` & `Flaskel-3.1.0rc3/flaskel/flaskel.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import os.path
 import typing as t
 
 import flask
+from flask.json.provider import JSONProvider
+from vbcore import json as vbcore_json
 from vbcore.datastruct import ObjectDict
 from vbcore.datastruct.lazy import Dumper
 from vbcore.http import httpcode
 from vbcore.http.headers import HeaderEnum
-from vbcore.json import JsonDecoder, JsonEncoder
 from vbcore.types import OptStr
 from werkzeug.routing import Rule
 from werkzeug.utils import safe_join
 
 from flaskel.utils.datastruct import Pagination
 
 cap: "Flaskel" = t.cast("Flaskel", flask.current_app)
@@ -114,18 +115,25 @@
             HeaderEnum.X_PAGINATION_COUNT: total,
             HeaderEnum.X_PAGINATION_PAGE: pagination.page or 1,
             HeaderEnum.X_PAGINATION_NUM_PAGES: pagination.pages(total),
             HeaderEnum.X_PAGINATION_PAGE_SIZE: pagination.per_page(),
         }
 
 
+class VBJSONProvider(JSONProvider):
+    def dumps(self, obj: t.Any, **kwargs: t.Any) -> str:
+        return vbcore_json.dumps(obj, **kwargs)
+
+    def loads(self, s: str | bytes, **kwargs: t.Any) -> t.Any:
+        return vbcore_json.loads(s, **kwargs)
+
+
 class Flaskel(flask.Flask):
     config_class = Config
     request_class = Request
     response_class = Response
-    _json_encoder = JsonEncoder
-    _json_decoder = JsonDecoder
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.version: OptStr = None
         self.config: Config
+        self.json = VBJSONProvider(self)
```

### Comparing `Flaskel-3.1.0rc2/flaskel/http/client.py` & `Flaskel-3.1.0rc3/flaskel/http/client.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/http/exceptions.py` & `Flaskel-3.1.0rc3/flaskel/http/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,8 +297,8 @@
 
 # until a better way is found
 errors = inspect.getmembers(
     sys.modules[__name__],
     lambda c: inspect.isclass(c) and issubclass(c, exceptions.HTTPException),
 )
 abort = exceptions.Aborter(extra={e.code: e for _, e in errors})
-setattr(flask, "abort", abort)
+flask.abort = abort
```

### Comparing `Flaskel-3.1.0rc2/flaskel/middlewares.py` & `Flaskel-3.1.0rc3/flaskel/middlewares.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typing as t
+from urllib.parse import parse_qs
 
 from vbcore import uuid
 from vbcore.datastruct import ObjectDict
 from werkzeug.middleware.proxy_fix import ProxyFix
-from werkzeug.urls import url_decode
 
 if t.TYPE_CHECKING:
     # pylint: disable=unused-import
     from _typeshed.wsgi import StartResponse, WSGIApplication, WSGIEnvironment
 
     from flaskel import Flaskel
 
@@ -102,16 +102,17 @@
         self, environ: "WSGIEnvironment", start_response: "StartResponse"
     ) -> t.Iterable[bytes]:
         conf = self.get_config()
         methods = conf.OVERRIDE_METHODS or ("POST",)
         method = environ.get("HTTP_X_HTTP_METHOD_OVERRIDE")
 
         if "_method_override" in environ.get("QUERY_STRING", ""):
-            args = url_decode(environ["QUERY_STRING"])
-            method = args.get("_method_override")
+            args = parse_qs(environ["QUERY_STRING"])
+            _methods = args.get("_method_override")
+            method = _methods[0] if _methods else None
 
         if method and environ["REQUEST_METHOD"] in methods:
             environ["REQUEST_METHOD"] = method.upper()
 
         return self.app(environ, start_response)
```

### Comparing `Flaskel-3.1.0rc2/flaskel/scripts/init_app.py` & `Flaskel-3.1.0rc3/flaskel/scripts/init_app.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/scripts/skeleton/resources/conf.yaml` & `Flaskel-3.1.0rc3/flaskel/scripts/skeleton/resources/conf.yaml`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/scripts/skeleton/resources/log.yaml` & `Flaskel-3.1.0rc3/flaskel/scripts/skeleton/resources/log.yaml`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/scripts/skeleton/resources/manage.sh` & `Flaskel-3.1.0rc3/flaskel/scripts/skeleton/resources/manage.sh`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/scripts/skeleton/resources/nuisances.yaml` & `Flaskel-3.1.0rc3/flaskel/scripts/skeleton/resources/nuisances.yaml`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/scripts/skeleton/resources/schemas.yaml` & `Flaskel-3.1.0rc3/flaskel/scripts/skeleton/resources/schemas.yaml`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/scripts/skeleton/resources/settings.ini.sample` & `Flaskel-3.1.0rc3/flaskel/scripts/skeleton/resources/settings.ini.sample`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/scripts/skeleton/resources/swagger.yaml` & `Flaskel-3.1.0rc3/flaskel/scripts/skeleton/resources/swagger.yaml`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/ext/__init__.py` & `Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/scripts/cli.py` & `Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/scripts/ws.py` & `Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/scripts/ws.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/__init__.py` & `Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/__init__.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/blueprints.py` & `Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/blueprints.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/common.py` & `Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/common.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/templates/core/head.html` & `Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/templates/core/head.html`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/templates/core/scripts.html` & `Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/templates/core/scripts.html`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/scripts/skeleton/skel/views/templates/index.html` & `Flaskel-3.1.0rc3/flaskel/scripts/skeleton/skel/views/templates/index.html`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/scripts/skeleton/tests/conftest.py` & `Flaskel-3.1.0rc3/flaskel/scripts/skeleton/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 @pytest.fixture(scope="session")
 def views():
     return Views
 
 
 @pytest.fixture()
 def auth_token(test_client, views):
-    def get_access_token(token=None, email=None, password=None, in_query=True):
+    def get_access_token(token=None, email=None, password=None, in_query=False):
         if token is not None:
             if in_query is True:
                 return f"token={token}"
             return dict(Authorization=f"Bearer {token}")
 
         credentials = dict(
             email=email or h.config.ADMIN_EMAIL,
```

### Comparing `Flaskel-3.1.0rc2/flaskel/scripts/skeleton/tests/test_smoke.py` & `Flaskel-3.1.0rc3/flaskel/scripts/skeleton/tests/test_smoke.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     Asserter.assert_allin(
         res.headers[HeaderEnum.ACCESS_CONTROL_EXPOSE_HEADERS].split(", "),
         config.CORS_EXPOSE_HEADERS,
     )
 
 
 def test_apidoc(config, api_tester, views):
-    headers = basic_auth_header(config.ADMIN_EMAIL, config.ADMIN_PASSWORD)
+    headers = basic_auth_header(config.BASIC_AUTH_USERNAME, config.BASIC_AUTH_PASSWORD)
 
     api_tester.get(
         url=url_for(views.api_docs), headers=headers, mimetype=ContentTypeEnum.HTML
     )
     res = api_tester.get(
         url=url_for(views.api_spec), headers=headers, mimetype=ContentTypeEnum.JSON
     )
```

### Comparing `Flaskel-3.1.0rc2/flaskel/standalone.py` & `Flaskel-3.1.0rc3/flaskel/standalone.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,37 +17,37 @@
     for opt in value:
         k, v = opt.split("=", 2)
         ret.update({k: parse_value(v)})
     return ret
 
 
 class Server:
-    opt_config_attr = dict(default=None, help="app yaml/json configuration file")
-    opt_log_config_attr = dict(
+    opt_config_attr = ObjectDict(default=None, help="app yaml/json configuration file")
+    opt_log_config_attr = ObjectDict(
         default=None, help="alternative log yaml/json configuration file"
     )
-    opt_bing_attr = dict(
+    opt_bing_attr = ObjectDict(
         default="127.0.0.1:5000", help="address to bind", show_default=True
     )
-    opt_debug_attr = dict(
+    opt_debug_attr = ObjectDict(
         is_flag=True, flag_value=True, default=False, help="enable debug mode"
     )
-    opt_wsgi_server_attr = dict(
+    opt_wsgi_server_attr = ObjectDict(
         default=None,
         type=click.Choice(list(DEFAULT_WSGI_SERVERS.keys()), case_sensitive=False),
         help="name of wsgi server to use",
     )
-    option_wsgi_config_attr = dict(
+    option_wsgi_config_attr = ObjectDict(
         default={},
         multiple=True,
         callback=option_as_dict,
         metavar="KEY=VAL",
         help="wsgi configuration",
     )
-    option_app_config_attr = dict(
+    option_app_config_attr = ObjectDict(
         default={},
         multiple=True,
         callback=option_as_dict,
         metavar="KEY=VAL",
         help="app configuration",
     )
```

### Comparing `Flaskel-3.1.0rc2/flaskel/tester/client.py` & `Flaskel-3.1.0rc3/flaskel/tester/client.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/tester/helpers.py` & `Flaskel-3.1.0rc3/flaskel/tester/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import typing as t
 from functools import partial
 
 import flask
+from vbcore.datastruct import ObjectDict
 from vbcore.db.support import SQLASupport
 from vbcore.http import httpcode, HttpMethod
 from vbcore.tester.asserter import Asserter
 from vbcore.tester.helpers import build_url
 
 from flaskel import TestClient
 from flaskel.utils.datastruct import ConfigProxy
@@ -233,26 +234,26 @@
             )
 
 
 def get_access_token(
     client,
     is_query: bool = False,
     token: t.Optional[str] = None,
-    token_type: str = "Bearer",
+    token_type: str = "Bearer",  # nosec
     access_view: str = "auth.token_access",
     credentials: t.Optional[t.Union[t.Dict[str, str], t.Tuple[str, str]]] = None,
 ) -> t.Dict[str, str]:
     conf = client.application.config
 
     if token is not None:
-        return dict(Authorization=f"{token_type} {token}")
+        return ObjectDict(Authorization=f"{token_type} {token}")
 
     if not credentials:
-        credentials = dict(email=conf.ADMIN_EMAIL, password=conf.ADMIN_PASSWORD)
+        credentials = ObjectDict(email=conf.ADMIN_EMAIL, password=conf.ADMIN_PASSWORD)
     elif isinstance(credentials, tuple):
-        credentials = dict(email=credentials[0], password=credentials[1])
+        credentials = ObjectDict(email=credentials[0], password=credentials[1])
 
     tokens = client.post(url_for(access_view), json=credentials)
     if is_query is True:
         return {conf.JWT_QUERY_STRING_NAME: tokens.json.access_token}
 
-    return dict(Authorization=f"{token_type} {tokens.json.access_token}")
+    return ObjectDict(Authorization=f"{token_type} {tokens.json.access_token}")
```

### Comparing `Flaskel-3.1.0rc2/flaskel/utils/datastruct.py` & `Flaskel-3.1.0rc3/flaskel/utils/datastruct.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/utils/logger.py` & `Flaskel-3.1.0rc3/flaskel/utils/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,24 @@
-REQUEST_FORMATTER = "flask_logify.formatters.RequestFormatter"
+from vbcore.datastruct import ObjectDict
+
+REQUEST_FORMATTER = "flaskel.ext.logging.formatters.RequestFormatter"
+CUSTOM_HANDLER = "flaskel.ext.logging.handlers.FlaskSysLogHandler"
+QUEUE_HANDLER = "flaskel.ext.logging.handlers.QueueHandler"
 
 
 def handler(formatter, **kwargs):
     return {
         "class": "logging.StreamHandler",
         "stream": "ext://sys.stderr",
         "formatter": formatter,
         **kwargs,
     }
 
 
-LOGGING = dict(
+LOGGING = ObjectDict(
     version=1,
     disable_existing_loggers=False,
     objects={"queue": {"class": "queue.Queue", "maxsize": 10000}},
     formatters={
         "simple": {"format": "[%(asctime)s][%(levelname)s]: %(message)s"},
         "consoleDebug": {
             "class": REQUEST_FORMATTER,
@@ -44,34 +48,34 @@
         },
     },
     handlers={
         "simple": handler("simple"),
         "console": handler("console"),
         "consoleDebug": handler("consoleDebug"),
         "syslog": {
-            "class": "flask_logify.handlers.FlaskSysLogHandler",
+            "class": CUSTOM_HANDLER,
             "address": ["localhost", 514],
             "formatter": "syslog",
             "facility": "user",
         },
         "syslogNoRequest": {
-            "class": "flask_logify.handlers.FlaskSysLogHandler",
+            "class": CUSTOM_HANDLER,
             "address": ["localhost", 514],
             "formatter": "syslogNoRequest",
             "facility": "user",
         },
         "queueConsole": {
             "respect_handler_level": True,
-            "class": "flask_logify.handlers.QueueHandler",
+            "class": QUEUE_HANDLER,
             "queue": "cfg://objects.queue",
             "handlers": ["cfg://handlers.console"],
         },
         "queueSyslogNoRequest": {
             "respect_handler_level": True,
-            "class": "flask_logify.handlers.QueueHandler",
+            "class": QUEUE_HANDLER,
             "queue": "cfg://objects.queue",
             "handlers": ["cfg://handlers.syslogNoRequest"],
         },
     },
     loggers={
         "development": {
             "level": "DEBUG",
```

### Comparing `Flaskel-3.1.0rc2/flaskel/utils/schemas/default.py` & `Flaskel-3.1.0rc3/flaskel/utils/schemas/default.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/utils/schemas/openapi3.py` & `Flaskel-3.1.0rc3/flaskel/utils/schemas/openapi3.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/utils/validator.py` & `Flaskel-3.1.0rc3/flaskel/utils/validator.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,9 +26,17 @@
             cls.validator.validate(payload, schema, raise_exc=True)
             return payload
         except jsonschema.SchemaError as exc:
             cap.logger.exception(exc)
             return abort(httpcode.INTERNAL_SERVER_ERROR)
         except jsonschema.ValidationError as exc:
             cap.logger.error(cls.validator.error_report(exc, payload))
-            reason = dict(cause=exc.cause, message=exc.message, path=exc.path)
-            return abort(httpcode.UNPROCESSABLE_ENTITY, response=dict(reason=reason))
+            return abort(
+                httpcode.UNPROCESSABLE_ENTITY,
+                response={
+                    "reason": {
+                        "cause": exc.cause,
+                        "message": exc.message,
+                        "path": exc.path,
+                    },
+                },
+            )
```

### Comparing `Flaskel-3.1.0rc2/flaskel/utils/webargs.py` & `Flaskel-3.1.0rc3/flaskel/utils/webargs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from functools import partial
 
+from vbcore.datastruct import ObjectDict
 from vbcore.http import httpcode
 from webargs import fields, flaskparser
 
 from flaskel.http.exceptions import abort
 
 parser = flaskparser.FlaskParser()
 query = partial(parser.use_args, location="query")
@@ -55,15 +56,15 @@
 @parser.error_handler
 def handle_error(error, *_, **__):
     abort(httpcode.BAD_REQUEST, response=error.messages)
 
 
 query_paginate = partial(
     query,
-    dict(
+    ObjectDict(
         page=OptField.positive(),
         page_size=OptField.positive(),
         related=OptField.boolean(load_default=False),
     ),
 )
```

### Comparing `Flaskel-3.1.0rc2/flaskel/views/base.py` & `Flaskel-3.1.0rc3/flaskel/views/base.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/views/proxy.py` & `Flaskel-3.1.0rc3/flaskel/views/proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,16 @@
 
 class ConfProxyView(BaseView):
     sep = "."
     config_key = None
 
     def __init__(self, config_key: t.Optional[str] = None):
         self._config_key = config_key or self.config_key
-        assert self._config_key is not None, "missing 'config_key'"
+        if not self._config_key:
+            raise ValueError("missing 'config_key'")
 
     def dispatch_request(self, *args, **kwargs):
         return self.perform(*args, **kwargs)
 
     def perform(self, *_, item=None, **__) -> ObjectDict:
         conf = cap.config
         keys = self._config_key.split(self.sep)
```

### Comparing `Flaskel-3.1.0rc2/flaskel/views/resource.py` & `Flaskel-3.1.0rc3/flaskel/views/resource.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/views/rpc.py` & `Flaskel-3.1.0rc3/flaskel/views/rpc.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/views/static.py` & `Flaskel-3.1.0rc3/flaskel/views/static.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/views/template.py` & `Flaskel-3.1.0rc3/flaskel/views/template.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/views/token.py` & `Flaskel-3.1.0rc3/flaskel/views/token.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             and data.password == cap.config.ADMIN_PASSWORD
         ):
             return data
         return None
 
     @classmethod
     @webargs.query(
-        dict(
+        ObjectDict(
             expires_access=webargs.OptField.positive(),
             expires_refresh=webargs.OptField.positive(),
         )
     )
     def access_token(cls, args) -> ObjectDict:
         credentials = cls.check_credential()
         if credentials:
```

### Comparing `Flaskel-3.1.0rc2/flaskel/wsgi/base.py` & `Flaskel-3.1.0rc3/flaskel/wsgi/base.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/wsgi/factory.py` & `Flaskel-3.1.0rc3/flaskel/wsgi/factory.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/wsgi/wsgi_gevent.py` & `Flaskel-3.1.0rc3/flaskel/wsgi/wsgi_gevent.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/wsgi/wsgi_gunicorn.py` & `Flaskel-3.1.0rc3/flaskel/wsgi/wsgi_gunicorn.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/wsgi/wsgi_tornado.py` & `Flaskel-3.1.0rc3/flaskel/wsgi/wsgi_tornado.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/flaskel/wsgi/wsgi_twisted.py` & `Flaskel-3.1.0rc3/flaskel/wsgi/wsgi_twisted.py`

 * *Files identical despite different names*

### Comparing `Flaskel-3.1.0rc2/setup.py` & `Flaskel-3.1.0rc3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,63 +2,32 @@
 Flaskel
 -------
 """
 import os
 import re
 import sys
 
-from pkg_resources import parse_requirements
+from pkg_resources import Requirement, yield_lines
 from setuptools import find_packages as base_find_packages, setup
 from setuptools.command.test import test
 
 LICENSE = "MIT"
 PLATFORMS = "any"
 PYTHON_VERSION = ">3.6"
 URL = "https://github.com/cs91chris/flaskel"
 DESCRIPTION = "Skeleton for flask applications"
 
 PKG_NAME = "flaskel"
 PKG_TEST = "tests"
 PKG_SCRIPTS = f"{PKG_NAME}.scripts"
+REQ_PATH = "requirements"
 
 BASE_PATH = os.path.dirname(__file__)
 SKEL_DIR = os.path.join(*PKG_SCRIPTS.split("."), "skeleton")
 VERSION_FILE = os.path.join(BASE_PATH, PKG_NAME, "version.py")
-REQUIRES = [
-    "Flask",
-    "Flask-Caching",
-    "Flask-CloudflareRemote",
-    "Flask-Cors",
-    "Flask-ErrorsHandler",
-    "Flask-HTTPAuth",
-    "Flask-JWT-Extended",
-    "Flask-Limiter",
-    "Flask-Logify",
-    "Flask-ResponseBuilder",
-    "Flask-SQLAlchemy",
-    "Flask-TemplateSupport",
-    "webargs",
-    "aiohttp",
-    "nest-asyncio",
-    "vbcore[all]",
-]
-REQUIRES_EXT = REQUIRES + [
-    "pyfcm",
-    "stripe",
-    "redis",
-    "hiredis",
-    "Flask-Mail",
-    "Flask-APScheduler",
-    "flask_pymongo",
-]
-REQUIRES_TEST = REQUIRES_EXT + [
-    "coverage",
-    "pytest",
-    "pytest-cov",
-]
 
 ENTRY_POINTS = {
     "console_scripts": [
         f"{PKG_NAME}={PKG_SCRIPTS}.cli:cli",
     ]
 }
 
@@ -107,26 +76,40 @@
     try:
         return read(file)
     except OSError as exc:
         print(str(exc), file=sys.stderr)
     return None
 
 
-def read_requirements(filename):
-    return [str(req) for req in parse_requirements(read(filename))]
-
-
 def skeleton_files():
     paths = []
     for path, _, filenames in os.walk(SKEL_DIR):
         for f in filenames:
             paths.append(os.path.join(path, f))
     return paths
 
 
+def read_requirements(filename):
+    reqs = []
+    lines = iter(yield_lines(read(filename)))
+    for line in lines:
+        if line.startswith("-c"):
+            continue
+        if " #" in line:
+            line = line[: line.find(" #")]
+        if line.endswith("\\"):
+            line = line[:-2].strip()
+            try:
+                line += next(lines)
+            except StopIteration:
+                break
+        reqs.append(str(Requirement(line)))
+    return reqs
+
+
 class PyTest(test):
     def finalize_options(self):
         test.finalize_options(self)
 
     def run_tests(self):
         import pytest  # pylint: disable=C0415
 
@@ -142,14 +125,18 @@
 
 def find_packages():
     if base_cythonize is not None:
         return [PKG_SCRIPTS]
     return base_find_packages(exclude=(PKG_TEST, f"{PKG_TEST}.*"))
 
 
+install_requires = read_requirements(os.path.join(REQ_PATH, "requirements.in"))
+tests_requires = read_requirements(os.path.join(REQ_PATH, "requirements-test.in"))
+extra_requires = read_requirements(os.path.join(REQ_PATH, "requirements-extra.in"))
+
 setup(
     name="Flaskel",
     url=URL,
     license=LICENSE,
     description=DESCRIPTION,
     platforms=PLATFORMS,
     python_requires=PYTHON_VERSION,
@@ -161,18 +148,18 @@
     zip_safe=False,
     include_package_data=True,
     packages=find_packages(),
     ext_modules=cythonize(ext_paths(PKG_NAME, skeleton_files())),
     test_suite=PKG_TEST,
     entry_points=ENTRY_POINTS,
     cmdclass={"test": PyTest},
-    install_requires=REQUIRES,
+    install_requires=install_requires,
     extras_require={
-        "test": REQUIRES_TEST,
-        "all": REQUIRES_EXT,
+        "test": tests_requires,
+        "all": extra_requires,
     },
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Flask",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

