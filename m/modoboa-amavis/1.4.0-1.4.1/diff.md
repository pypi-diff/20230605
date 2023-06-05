# Comparing `tmp/modoboa-amavis-1.4.0.tar.gz` & `tmp/modoboa-amavis-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modoboa-amavis-1.4.0.tar", last modified: Thu May  5 14:39:09 2022, max compression
+gzip compressed data, was "modoboa-amavis-1.4.1.tar", last modified: Mon Jun  5 13:41:35 2023, max compression
```

## Comparing `modoboa-amavis-1.4.0.tar` & `modoboa-amavis-1.4.1.tar`

### file list

```diff
@@ -1,189 +1,189 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.879952 modoboa-amavis-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (121)      343 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.867952 modoboa-amavis-1.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.867952 modoboa-amavis-1.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     5404 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/.github/workflows/plugin.yml
--rw-r--r--   0 runner    (1001) docker     (121)      675 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.867952 modoboa-amavis-1.4.0/.tx/
--rw-r--r--   0 runner    (1001) docker     (121)      422 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/.tx/config
--rw-r--r--   0 runner    (1001) docker     (121)     1099 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2429 2022-05-05 14:39:09.879952 modoboa-amavis-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1580 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.867952 modoboa-amavis-1.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     6794 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     8347 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1440 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      975 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10421 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/docs/setup.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.867952 modoboa-amavis-1.4.0/modoboa_amavis/
--rw-r--r--   0 runner    (1001) docker     (121)      355 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      440 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.871952 modoboa-amavis-1.4.0/modoboa_amavis/checks/
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1809 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/checks/settings_checks.py
--rw-r--r--   0 runner    (1001) docker     (121)      697 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     1383 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/dbrouter.py
--rw-r--r--   0 runner    (1001) docker     (121)     4829 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/factories.py
--rw-r--r--   0 runner    (1001) docker     (121)     9239 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/forms.py
--rw-r--r--   0 runner    (1001) docker     (121)     6674 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/handlers.py
--rw-r--r--   0 runner    (1001) docker     (121)    14991 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.863952 modoboa-amavis-1.4.0/modoboa_amavis/locale/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.863952 modoboa-amavis-1.4.0/modoboa_amavis/locale/cs_CZ/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.871952 modoboa-amavis-1.4.0/modoboa_amavis/locale/cs_CZ/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     8998 2022-05-05 14:39:03.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/cs_CZ/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    14950 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/cs_CZ/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)     1257 2022-05-05 14:39:03.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/cs_CZ/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)     2077 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/cs_CZ/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.863952 modoboa-amavis-1.4.0/modoboa_amavis/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.871952 modoboa-amavis-1.4.0/modoboa_amavis/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     8560 2022-05-05 14:39:03.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    14299 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)     1189 2022-05-05 14:39:03.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/de/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)     2049 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/de/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.863952 modoboa-amavis-1.4.0/modoboa_amavis/locale/el_GR/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.871952 modoboa-amavis-1.4.0/modoboa_amavis/locale/el_GR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    12161 2022-05-05 14:39:03.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/el_GR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    17050 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/el_GR/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)     1543 2022-05-05 14:39:03.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/el_GR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)     2431 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/el_GR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.863952 modoboa-amavis-1.4.0/modoboa_amavis/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.871952 modoboa-amavis-1.4.0/modoboa_amavis/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      337 2022-05-05 14:39:03.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    10314 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)      337 2022-05-05 14:39:03.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/en/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1619 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/en/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.863952 modoboa-amavis-1.4.0/modoboa_amavis/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.871952 modoboa-amavis-1.4.0/modoboa_amavis/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     9351 2022-05-05 14:39:03.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    14192 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)     1193 2022-05-05 14:39:03.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/es/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)     2115 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/es/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.863952 modoboa-amavis-1.4.0/modoboa_amavis/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.871952 modoboa-amavis-1.4.0/modoboa_amavis/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    10330 2022-05-05 14:39:03.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    14440 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)     1225 2022-05-05 14:39:03.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/fr/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)     2004 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/fr/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.863952 modoboa-amavis-1.4.0/modoboa_amavis/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.871952 modoboa-amavis-1.4.0/modoboa_amavis/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     8549 2022-05-05 14:39:03.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    14353 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)     1217 2022-05-05 14:39:03.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/it/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)     2031 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/it/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.863952 modoboa-amavis-1.4.0/modoboa_amavis/locale/nl_NL/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.875952 modoboa-amavis-1.4.0/modoboa_amavis/locale/nl_NL/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     8598 2022-05-05 14:39:03.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/nl_NL/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    14430 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/nl_NL/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)     1234 2022-05-05 14:39:03.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/nl_NL/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)     2096 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/nl_NL/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.863952 modoboa-amavis-1.4.0/modoboa_amavis/locale/pl_PL/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.875952 modoboa-amavis-1.4.0/modoboa_amavis/locale/pl_PL/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     9620 2022-05-05 14:39:03.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/pl_PL/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    14541 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/pl_PL/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)     1298 2022-05-05 14:39:03.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/pl_PL/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)     2108 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/pl_PL/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.863952 modoboa-amavis-1.4.0/modoboa_amavis/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.875952 modoboa-amavis-1.4.0/modoboa_amavis/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     8636 2022-05-05 14:39:03.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    14454 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/pt_BR/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)     1225 2022-05-05 14:39:03.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/pt_BR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)     2059 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/pt_BR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.863952 modoboa-amavis-1.4.0/modoboa_amavis/locale/pt_PT/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.875952 modoboa-amavis-1.4.0/modoboa_amavis/locale/pt_PT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     8744 2022-05-05 14:39:03.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/pt_PT/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    14768 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/pt_PT/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)     1258 2022-05-05 14:39:03.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/pt_PT/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)     2278 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/pt_PT/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.863952 modoboa-amavis-1.4.0/modoboa_amavis/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.875952 modoboa-amavis-1.4.0/modoboa_amavis/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     7622 2022-05-05 14:39:03.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    15647 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)     1008 2022-05-05 14:39:03.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/ru/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)     2122 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/ru/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.863952 modoboa-amavis-1.4.0/modoboa_amavis/locale/sv/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.875952 modoboa-amavis-1.4.0/modoboa_amavis/locale/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     8331 2022-05-05 14:39:03.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/sv/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    14221 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/sv/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-05-05 14:39:03.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/sv/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)     2054 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/locale/sv/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.875952 modoboa-amavis-1.4.0/modoboa_amavis/management/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.875952 modoboa-amavis-1.4.0/modoboa_amavis/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3792 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/management/commands/amnotify.py
--rw-r--r--   0 runner    (1001) docker     (121)     2559 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/management/commands/qcleanup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.875952 modoboa-amavis-1.4.0/modoboa_amavis/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)    10503 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9236 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1395 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/modo_extension.py
--rw-r--r--   0 runner    (1001) docker     (121)      585 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     8337 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/sql_connector.py
--rw-r--r--   0 runner    (1001) docker     (121)     2235 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/sql_email.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.863952 modoboa-amavis-1.4.0/modoboa_amavis/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.863952 modoboa-amavis-1.4.0/modoboa_amavis/static/modoboa_amavis/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.875952 modoboa-amavis-1.4.0/modoboa_amavis/static/modoboa_amavis/css/
--rw-r--r--   0 runner    (1001) docker     (121)     1230 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/static/modoboa_amavis/css/quarantine.css
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/static/modoboa_amavis/css/selfservice.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.875952 modoboa-amavis-1.4.0/modoboa_amavis/static/modoboa_amavis/js/
--rw-r--r--   0 runner    (1001) docker     (121)    15464 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/static/modoboa_amavis/js/quarantine.js
--rw-r--r--   0 runner    (1001) docker     (121)      680 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/static/modoboa_amavis/js/selfservice.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.863952 modoboa-amavis-1.4.0/modoboa_amavis/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.879952 modoboa-amavis-1.4.0/modoboa_amavis/templates/modoboa_amavis/
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/templates/modoboa_amavis/_email_display.html
--rw-r--r--   0 runner    (1001) docker     (121)      751 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/templates/modoboa_amavis/domain_content_filter.html
--rw-r--r--   0 runner    (1001) docker     (121)     1184 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/templates/modoboa_amavis/email_list.html
--rw-r--r--   0 runner    (1001) docker     (121)     1320 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/templates/modoboa_amavis/emails_page.html
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/templates/modoboa_amavis/empty_quarantine.html
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/templates/modoboa_amavis/getmailcontent.html
--rw-r--r--   0 runner    (1001) docker     (121)     1527 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/templates/modoboa_amavis/index.html
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/templates/modoboa_amavis/mailheaders.html
--rw-r--r--   0 runner    (1001) docker     (121)     1795 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/templates/modoboa_amavis/main_action_bar.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.879952 modoboa-amavis-1.4.0/modoboa_amavis/templates/modoboa_amavis/notifications/
--rw-r--r--   0 runner    (1001) docker     (121)      707 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/templates/modoboa_amavis/notifications/pending_requests.html
--rw-r--r--   0 runner    (1001) docker     (121)      846 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/templates/modoboa_amavis/quarantine.html
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/templates/modoboa_amavis/viewheader.html
--rw-r--r--   0 runner    (1001) docker     (121)     1512 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/templates/modoboa_amavis/viewmail_selfservice.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.879952 modoboa-amavis-1.4.0/modoboa_amavis/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4439 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/templatetags/amavis_tags.py
--rw-r--r--   0 runner    (1001) docker     (121)     1216 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/test_runners.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.879952 modoboa-amavis-1.4.0/modoboa_amavis/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)       18 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/tests/sa-learn
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.879952 modoboa-amavis-1.4.0/modoboa_amavis/tests/sample_messages/
--rw-r--r--   0 runner    (1001) docker     (121)     4442 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/tests/sample_messages/quarantined-input.txt
--rw-r--r--   0 runner    (1001) docker     (121)      459 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/tests/sample_messages/quarantined-output-plain_nolinks.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)       18 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/tests/spamc
--rw-r--r--   0 runner    (1001) docker     (121)      917 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (121)     8472 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/tests/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3677 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/tests/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (121)     1605 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/tests/test_management_commands.py
--rw-r--r--   0 runner    (1001) docker     (121)     2372 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/tests/test_sql_email.py
--rw-r--r--   0 runner    (1001) docker     (121)      703 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    13006 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (121)     1043 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     3644 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    14964 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/modoboa_amavis/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.871952 modoboa-amavis-1.4.0/modoboa_amavis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2429 2022-05-05 14:39:09.000000 modoboa-amavis-1.4.0/modoboa_amavis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5598 2022-05-05 14:39:09.000000 modoboa-amavis-1.4.0/modoboa_amavis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-05 14:39:09.000000 modoboa-amavis-1.4.0/modoboa_amavis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-05 14:39:09.000000 modoboa-amavis-1.4.0/modoboa_amavis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-05 14:39:09.000000 modoboa-amavis-1.4.0/modoboa_amavis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-05-05 14:39:09.000000 modoboa-amavis-1.4.0/modoboa_amavis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10074 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      587 2022-05-05 14:39:09.879952 modoboa-amavis-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2655 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.879952 modoboa-amavis-1.4.0/test_project/
--rwxr-xr-x   0 runner    (1001) docker     (121)      860 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/test_project/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 14:39:09.879952 modoboa-amavis-1.4.0/test_project/test_project/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/test_project/test_project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8200 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/test_project/test_project/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/test_project/test_project/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)      443 2022-05-05 14:37:47.000000 modoboa-amavis-1.4.0/test_project/test_project/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.569687 modoboa-amavis-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.557686 modoboa-amavis-1.4.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.557686 modoboa-amavis-1.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/.github/workflows/plugin.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.557686 modoboa-amavis-1.4.1/.tx/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-05 13:41:35.569687 modoboa-amavis-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.557686 modoboa-amavis-1.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10421 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/docs/setup.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.557686 modoboa-amavis-1.4.1/modoboa_amavis/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.557686 modoboa-amavis-1.4.1/modoboa_amavis/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/checks/settings_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/dbrouter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9239 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14990 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.553686 modoboa-amavis-1.4.1/modoboa_amavis/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.553686 modoboa-amavis-1.4.1/modoboa_amavis/locale/cs_CZ/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.561686 modoboa-amavis-1.4.1/modoboa_amavis/locale/cs_CZ/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-06-05 13:41:32.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/cs_CZ/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    14950 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/cs_CZ/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-05 13:41:32.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/cs_CZ/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/cs_CZ/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.553686 modoboa-amavis-1.4.1/modoboa_amavis/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.561686 modoboa-amavis-1.4.1/modoboa_amavis/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-06-05 13:41:32.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    14299 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-05 13:41:32.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/de/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/de/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.553686 modoboa-amavis-1.4.1/modoboa_amavis/locale/el_GR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.561686 modoboa-amavis-1.4.1/modoboa_amavis/locale/el_GR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-06-05 13:41:32.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/el_GR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    17050 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/el_GR/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-05 13:41:32.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/el_GR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/el_GR/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.553686 modoboa-amavis-1.4.1/modoboa_amavis/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.561686 modoboa-amavis-1.4.1/modoboa_amavis/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-05 13:41:32.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-05 13:41:32.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/en/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/en/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.553686 modoboa-amavis-1.4.1/modoboa_amavis/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.561686 modoboa-amavis-1.4.1/modoboa_amavis/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-06-05 13:41:32.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    14192 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-05 13:41:32.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/es/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/es/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.553686 modoboa-amavis-1.4.1/modoboa_amavis/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.561686 modoboa-amavis-1.4.1/modoboa_amavis/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-06-05 13:41:32.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    14440 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-05 13:41:32.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/fr/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/fr/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.553686 modoboa-amavis-1.4.1/modoboa_amavis/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.561686 modoboa-amavis-1.4.1/modoboa_amavis/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-06-05 13:41:32.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    14353 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-05 13:41:32.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/it/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/it/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.553686 modoboa-amavis-1.4.1/modoboa_amavis/locale/nl_NL/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.561686 modoboa-amavis-1.4.1/modoboa_amavis/locale/nl_NL/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8598 2023-06-05 13:41:32.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/nl_NL/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    14430 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/nl_NL/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-05 13:41:32.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/nl_NL/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/nl_NL/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.553686 modoboa-amavis-1.4.1/modoboa_amavis/locale/pl_PL/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.561686 modoboa-amavis-1.4.1/modoboa_amavis/locale/pl_PL/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     9620 2023-06-05 13:41:32.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/pl_PL/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    14541 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/pl_PL/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-05 13:41:32.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/pl_PL/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/pl_PL/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.553686 modoboa-amavis-1.4.1/modoboa_amavis/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.565687 modoboa-amavis-1.4.1/modoboa_amavis/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-06-05 13:41:32.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    14454 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-05 13:41:32.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/pt_BR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/pt_BR/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.553686 modoboa-amavis-1.4.1/modoboa_amavis/locale/pt_PT/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.565687 modoboa-amavis-1.4.1/modoboa_amavis/locale/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8744 2023-06-05 13:41:32.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/pt_PT/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    14768 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/pt_PT/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-05 13:41:32.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/pt_PT/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/pt_PT/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.553686 modoboa-amavis-1.4.1/modoboa_amavis/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.565687 modoboa-amavis-1.4.1/modoboa_amavis/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-06-05 13:41:32.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    15647 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-05 13:41:32.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/ru/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/ru/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.553686 modoboa-amavis-1.4.1/modoboa_amavis/locale/sv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.565687 modoboa-amavis-1.4.1/modoboa_amavis/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-06-05 13:41:32.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/sv/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    14221 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/sv/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-05 13:41:32.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/sv/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/locale/sv/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.565687 modoboa-amavis-1.4.1/modoboa_amavis/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.565687 modoboa-amavis-1.4.1/modoboa_amavis/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/management/commands/amnotify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/management/commands/qcleanup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.565687 modoboa-amavis-1.4.1/modoboa_amavis/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/modo_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8337 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/sql_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/sql_email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.553686 modoboa-amavis-1.4.1/modoboa_amavis/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.553686 modoboa-amavis-1.4.1/modoboa_amavis/static/modoboa_amavis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.565687 modoboa-amavis-1.4.1/modoboa_amavis/static/modoboa_amavis/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/static/modoboa_amavis/css/quarantine.css
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/static/modoboa_amavis/css/selfservice.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.565687 modoboa-amavis-1.4.1/modoboa_amavis/static/modoboa_amavis/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    15464 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/static/modoboa_amavis/js/quarantine.js
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/static/modoboa_amavis/js/selfservice.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.553686 modoboa-amavis-1.4.1/modoboa_amavis/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.569687 modoboa-amavis-1.4.1/modoboa_amavis/templates/modoboa_amavis/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/templates/modoboa_amavis/_email_display.html
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/templates/modoboa_amavis/domain_content_filter.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/templates/modoboa_amavis/email_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/templates/modoboa_amavis/emails_page.html
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/templates/modoboa_amavis/empty_quarantine.html
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/templates/modoboa_amavis/getmailcontent.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/templates/modoboa_amavis/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/templates/modoboa_amavis/mailheaders.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/templates/modoboa_amavis/main_action_bar.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.569687 modoboa-amavis-1.4.1/modoboa_amavis/templates/modoboa_amavis/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/templates/modoboa_amavis/notifications/pending_requests.html
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/templates/modoboa_amavis/quarantine.html
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/templates/modoboa_amavis/viewheader.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/templates/modoboa_amavis/viewmail_selfservice.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.569687 modoboa-amavis-1.4.1/modoboa_amavis/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/templatetags/amavis_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/test_runners.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.569687 modoboa-amavis-1.4.1/modoboa_amavis/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       18 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/tests/sa-learn
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.569687 modoboa-amavis-1.4.1/modoboa_amavis/tests/sample_messages/
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/tests/sample_messages/quarantined-input.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/tests/sample_messages/quarantined-output-plain_nolinks.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       18 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/tests/spamc
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/tests/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/tests/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/tests/test_management_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/tests/test_sql_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13006 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14964 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/modoboa_amavis/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.557686 modoboa-amavis-1.4.1/modoboa_amavis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-05 13:41:35.000000 modoboa-amavis-1.4.1/modoboa_amavis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-06-05 13:41:35.000000 modoboa-amavis-1.4.1/modoboa_amavis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:41:35.000000 modoboa-amavis-1.4.1/modoboa_amavis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:41:35.000000 modoboa-amavis-1.4.1/modoboa_amavis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 13:41:35.000000 modoboa-amavis-1.4.1/modoboa_amavis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-05 13:41:35.000000 modoboa-amavis-1.4.1/modoboa_amavis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10074 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-05 13:41:35.569687 modoboa-amavis-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.569687 modoboa-amavis-1.4.1/test_project/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      860 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/test_project/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:41:35.569687 modoboa-amavis-1.4.1/test_project/test_project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/test_project/test_project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8281 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/test_project/test_project/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/test_project/test_project/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-05 13:40:57.000000 modoboa-amavis-1.4.1/test_project/test_project/wsgi.py
```

### Comparing `modoboa-amavis-1.4.0/.github/workflows/plugin.yml` & `modoboa-amavis-1.4.1/.github/workflows/plugin.yml`

 * *Files 1% similar despite different names*

```diff
@@ -40,24 +40,24 @@
     strategy:
       matrix:
         database: ['postgres', 'mysql']
         python-version: [3.7, 3.8, 3.9]
       fail-fast: false
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           sudo apt-get update -y && sudo apt-get install -y librrd-dev rrdtool
           python -m pip install --upgrade pip
-          pip install -e git+https://github.com/modoboa/modoboa.git#egg=modoboa
+          #pip install -e git+https://github.com/modoboa/modoboa.git#egg=modoboa
           pip install -r requirements.txt
           pip install -r test-requirements.txt
           python setup.py develop
       - name: Install postgres requirements
         if: ${{ matrix.database == 'postgres' }}
         run: |
           pip install 'psycopg2-binary>=2.8,<2.9'
@@ -100,15 +100,15 @@
           name: coverage-results
           path: test_project/.coverage
 
   coverage:
     needs: test
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Set up Python 3.9
         uses: actions/setup-python@v2
         with:
           python-version: '3.9'
       - name: Install dependencies
         run: |
           pip install codecov
@@ -121,19 +121,19 @@
           coverage report
           codecov
 
   release:
     needs: coverage
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - name: Set up Python 3.9
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: '3.9'
       - name: Build packages
         run: |
           sudo apt-get install librrd-dev rrdtool libssl-dev gettext
           python -m pip install --upgrade pip setuptools wheel
           pip install -r requirements.txt
```

### Comparing `modoboa-amavis-1.4.0/.gitignore` & `modoboa-amavis-1.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/LICENSE` & `modoboa-amavis-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/PKG-INFO` & `modoboa-amavis-1.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: modoboa-amavis
-Version: 1.4.0
+Version: 1.4.1
 Summary: The amavis frontend of Modoboa
 Home-page: http://modoboa.org/
 Author: Antoine Nguyen
 Author-email: tonio@ngyn.org
 License: MIT
 Keywords: email amavis spamassassin
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django :: 2.2
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -74,9 +73,7 @@
 won't work. Check `docs/setup` for more information.
 
 .. |gha| image:: https://github.com/modoboa/modoboa-amavis/actions/workflows/plugin.yml/badge.svg
    :target: https://github.com/modoboa/modoboa-amavis/actions/workflows/plugin.yml
 
 .. |codecov| image:: https://codecov.io/gh/modoboa/modoboa-amavis/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/modoboa/modoboa-amavis
-
-
```

### Comparing `modoboa-amavis-1.4.0/README.rst` & `modoboa-amavis-1.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/docs/Makefile` & `modoboa-amavis-1.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/docs/conf.py` & `modoboa-amavis-1.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/docs/index.rst` & `modoboa-amavis-1.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/docs/install.rst` & `modoboa-amavis-1.4.1/docs/install.rst`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/docs/setup.rst` & `modoboa-amavis-1.4.1/docs/setup.rst`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/checks/settings_checks.py` & `modoboa-amavis-1.4.1/modoboa_amavis/checks/settings_checks.py`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/constants.py` & `modoboa-amavis-1.4.1/modoboa_amavis/constants.py`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/dbrouter.py` & `modoboa-amavis-1.4.1/modoboa_amavis/dbrouter.py`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/factories.py` & `modoboa-amavis-1.4.1/modoboa_amavis/factories.py`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/forms.py` & `modoboa-amavis-1.4.1/modoboa_amavis/forms.py`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/handlers.py` & `modoboa-amavis-1.4.1/modoboa_amavis/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,22 +178,22 @@
         "counter": nbrequests, "level": "danger"
     }]
 
 
 @receiver(admin_signals.extra_domain_forms)
 def extra_domain_form(sender, user, domain, **kwargs):
     """Return domain config form."""
-    if not user.has_perm("admin.view_domains"):
+    if not user.has_perm("admin.view_domain"):
         return []
     return [{
         "id": "amavis", "title": _("Content filter"),
         "cls": forms.DomainPolicyForm,
         "formtpl": "modoboa_amavis/domain_content_filter.html"
     }]
 
 
 @receiver(admin_signals.get_domain_form_instances)
 def fill_domain_instances(sender, user, domain, **kwargs):
     """Return domain instance."""
-    if not user.has_perm("admin.view_domains"):
+    if not user.has_perm("admin.view_domain"):
         return {}
     return {"amavis": domain}
```

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/lib.py` & `modoboa-amavis-1.4.1/modoboa_amavis/lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -351,15 +351,15 @@
 
     :return: True if learning is enabled, False otherwise.
     """
     conf = dict(param_tools.get_global_parameters("modoboa_amavis"))
     if not conf["manual_learning"]:
         return False
     if user.role != "SuperAdmins":
-        if user.has_perm("admin.view_domains"):
+        if user.has_perm("admin.view_domain"):
             manual_learning = (
                 conf["domain_level_learning"] or conf["user_level_learning"])
         else:
             manual_learning = conf["user_level_learning"]
         return manual_learning
     return True
```

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/cs_CZ/LC_MESSAGES/django.mo` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/cs_CZ/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/cs_CZ/LC_MESSAGES/django.po` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/cs_CZ/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/cs_CZ/LC_MESSAGES/djangojs.mo` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/cs_CZ/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/cs_CZ/LC_MESSAGES/djangojs.po` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/cs_CZ/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/de/LC_MESSAGES/django.mo` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/de/LC_MESSAGES/django.po` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/de/LC_MESSAGES/djangojs.mo` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/de/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/de/LC_MESSAGES/djangojs.po` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/de/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/el_GR/LC_MESSAGES/django.mo` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/el_GR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/el_GR/LC_MESSAGES/django.po` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/el_GR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/el_GR/LC_MESSAGES/djangojs.mo` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/el_GR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/el_GR/LC_MESSAGES/djangojs.po` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/el_GR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/en/LC_MESSAGES/django.po` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/en/LC_MESSAGES/djangojs.po` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/en/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/es/LC_MESSAGES/django.mo` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/es/LC_MESSAGES/django.po` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/es/LC_MESSAGES/djangojs.mo` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/es/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/es/LC_MESSAGES/djangojs.po` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/es/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/fr/LC_MESSAGES/django.mo` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/fr/LC_MESSAGES/django.po` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/fr/LC_MESSAGES/djangojs.mo` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/fr/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/fr/LC_MESSAGES/djangojs.po` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/fr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/it/LC_MESSAGES/django.mo` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/it/LC_MESSAGES/django.po` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/it/LC_MESSAGES/djangojs.mo` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/it/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/it/LC_MESSAGES/djangojs.po` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/it/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/nl_NL/LC_MESSAGES/django.mo` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/nl_NL/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/nl_NL/LC_MESSAGES/django.po` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/nl_NL/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/nl_NL/LC_MESSAGES/djangojs.mo` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/nl_NL/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/nl_NL/LC_MESSAGES/djangojs.po` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/nl_NL/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/pl_PL/LC_MESSAGES/django.mo` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/pl_PL/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/pl_PL/LC_MESSAGES/django.po` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/pl_PL/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/pl_PL/LC_MESSAGES/djangojs.mo` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/pl_PL/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/pl_PL/LC_MESSAGES/djangojs.po` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/pl_PL/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/pt_BR/LC_MESSAGES/django.mo` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/pt_BR/LC_MESSAGES/django.po` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/pt_BR/LC_MESSAGES/djangojs.mo` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/pt_BR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/pt_BR/LC_MESSAGES/djangojs.po` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/pt_BR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/pt_PT/LC_MESSAGES/django.mo` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/pt_PT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/pt_PT/LC_MESSAGES/django.po` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/pt_PT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/pt_PT/LC_MESSAGES/djangojs.mo` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/pt_PT/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/pt_PT/LC_MESSAGES/djangojs.po` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/pt_PT/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/ru/LC_MESSAGES/django.mo` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/ru/LC_MESSAGES/django.po` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/ru/LC_MESSAGES/djangojs.mo` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/ru/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/ru/LC_MESSAGES/djangojs.po` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/ru/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/sv/LC_MESSAGES/django.mo` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/sv/LC_MESSAGES/django.po` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/sv/LC_MESSAGES/djangojs.mo` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/sv/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/locale/sv/LC_MESSAGES/djangojs.po` & `modoboa-amavis-1.4.1/modoboa_amavis/locale/sv/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/management/commands/amnotify.py` & `modoboa-amavis-1.4.1/modoboa_amavis/management/commands/amnotify.py`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/management/commands/qcleanup.py` & `modoboa-amavis-1.4.1/modoboa_amavis/management/commands/qcleanup.py`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/migrations/0001_initial.py` & `modoboa-amavis-1.4.1/modoboa_amavis/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/models.py` & `modoboa-amavis-1.4.1/modoboa_amavis/models.py`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/modo_extension.py` & `modoboa-amavis-1.4.1/modoboa_amavis/modo_extension.py`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/settings.py` & `modoboa-amavis-1.4.1/modoboa_amavis/settings.py`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/sql_connector.py` & `modoboa-amavis-1.4.1/modoboa_amavis/sql_connector.py`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/sql_email.py` & `modoboa-amavis-1.4.1/modoboa_amavis/sql_email.py`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/static/modoboa_amavis/css/quarantine.css` & `modoboa-amavis-1.4.1/modoboa_amavis/static/modoboa_amavis/css/quarantine.css`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/static/modoboa_amavis/js/quarantine.js` & `modoboa-amavis-1.4.1/modoboa_amavis/static/modoboa_amavis/js/quarantine.js`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/static/modoboa_amavis/js/selfservice.js` & `modoboa-amavis-1.4.1/modoboa_amavis/static/modoboa_amavis/js/selfservice.js`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/templates/modoboa_amavis/domain_content_filter.html` & `modoboa-amavis-1.4.1/modoboa_amavis/templates/modoboa_amavis/domain_content_filter.html`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/templates/modoboa_amavis/email_list.html` & `modoboa-amavis-1.4.1/modoboa_amavis/templates/modoboa_amavis/email_list.html`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/templates/modoboa_amavis/emails_page.html` & `modoboa-amavis-1.4.1/modoboa_amavis/templates/modoboa_amavis/emails_page.html`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/templates/modoboa_amavis/index.html` & `modoboa-amavis-1.4.1/modoboa_amavis/templates/modoboa_amavis/index.html`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/templates/modoboa_amavis/main_action_bar.html` & `modoboa-amavis-1.4.1/modoboa_amavis/templates/modoboa_amavis/main_action_bar.html`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/templates/modoboa_amavis/notifications/pending_requests.html` & `modoboa-amavis-1.4.1/modoboa_amavis/templates/modoboa_amavis/notifications/pending_requests.html`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/templates/modoboa_amavis/quarantine.html` & `modoboa-amavis-1.4.1/modoboa_amavis/templates/modoboa_amavis/quarantine.html`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/templates/modoboa_amavis/viewmail_selfservice.html` & `modoboa-amavis-1.4.1/modoboa_amavis/templates/modoboa_amavis/viewmail_selfservice.html`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/templatetags/amavis_tags.py` & `modoboa-amavis-1.4.1/modoboa_amavis/templatetags/amavis_tags.py`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/test_runners.py` & `modoboa-amavis-1.4.1/modoboa_amavis/test_runners.py`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/tests/sample_messages/quarantined-input.txt` & `modoboa-amavis-1.4.1/modoboa_amavis/tests/sample_messages/quarantined-input.txt`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/tests/test_checks.py` & `modoboa-amavis-1.4.1/modoboa_amavis/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/tests/test_handlers.py` & `modoboa-amavis-1.4.1/modoboa_amavis/tests/test_handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,11 +223,11 @@
             "address": "@test.com",
             "recipients": "admin@test.com",
             "enabled": True
         }
         self.ajax_post(reverse("admin:alias_add"), values)
 
         alias = admin_models.Alias.objects.get(address="@test.com")
-        self.ajax_post(
+        self.ajax_delete(
             reverse("admin:alias_delete") + "?selection={}".format(alias.id)
         )
         self.assertTrue(models.Users.objects.get(email="@test.com"))
```

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/tests/test_lib.py` & `modoboa-amavis-1.4.1/modoboa_amavis/tests/test_lib.py`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/tests/test_management_commands.py` & `modoboa-amavis-1.4.1/modoboa_amavis/tests/test_management_commands.py`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/tests/test_sql_email.py` & `modoboa-amavis-1.4.1/modoboa_amavis/tests/test_sql_email.py`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/tests/test_utils.py` & `modoboa-amavis-1.4.1/modoboa_amavis/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/tests/test_views.py` & `modoboa-amavis-1.4.1/modoboa_amavis/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/urls.py` & `modoboa-amavis-1.4.1/modoboa_amavis/urls.py`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/utils.py` & `modoboa-amavis-1.4.1/modoboa_amavis/utils.py`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis/views.py` & `modoboa-amavis-1.4.1/modoboa_amavis/views.py`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis.egg-info/PKG-INFO` & `modoboa-amavis-1.4.1/modoboa_amavis.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: modoboa-amavis
-Version: 1.4.0
+Version: 1.4.1
 Summary: The amavis frontend of Modoboa
 Home-page: http://modoboa.org/
 Author: Antoine Nguyen
 Author-email: tonio@ngyn.org
 License: MIT
 Keywords: email amavis spamassassin
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django :: 2.2
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -74,9 +73,7 @@
 won't work. Check `docs/setup` for more information.
 
 .. |gha| image:: https://github.com/modoboa/modoboa-amavis/actions/workflows/plugin.yml/badge.svg
    :target: https://github.com/modoboa/modoboa-amavis/actions/workflows/plugin.yml
 
 .. |codecov| image:: https://codecov.io/gh/modoboa/modoboa-amavis/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/modoboa/modoboa-amavis
-
-
```

### Comparing `modoboa-amavis-1.4.0/modoboa_amavis.egg-info/SOURCES.txt` & `modoboa-amavis-1.4.1/modoboa_amavis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/pylintrc` & `modoboa-amavis-1.4.1/pylintrc`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/setup.cfg` & `modoboa-amavis-1.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/setup.py` & `modoboa-amavis-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/test_project/manage.py` & `modoboa-amavis-1.4.1/test_project/manage.py`

 * *Files identical despite different names*

### Comparing `modoboa-amavis-1.4.0/test_project/test_project/settings.py` & `modoboa-amavis-1.4.1/test_project/test_project/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,17 @@
     "modoboa.admin",
     "modoboa.transport",
     "modoboa.relaydomains",
     "modoboa.limits",
     "modoboa.parameters",
     "modoboa.dnstools",
     "modoboa.maillog",
+    "modoboa.pdfcredentials",
+    "modoboa.dmarc",
+    "modoboa.imap_migration",
     # Modoboa extensions here.
     "modoboa_amavis",
 )
 
 INSTALLED_APPS += MODOBOA_APPS
 
 AUTH_USER_MODEL = "core.User"
```

