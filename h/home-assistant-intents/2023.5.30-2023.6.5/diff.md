# Comparing `tmp/home-assistant-intents-2023.5.30.tar.gz` & `tmp/home-assistant-intents-2023.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "home-assistant-intents-2023.5.30.tar", last modified: Tue May 30 16:41:22 2023, max compression
+gzip compressed data, was "home-assistant-intents-2023.6.5.tar", last modified: Mon Jun  5 15:46:39 2023, max compression
```

## Comparing `home-assistant-intents-2023.5.30.tar` & `home-assistant-intents-2023.6.5.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-30 16:41:22.618410 home-assistant-intents-2023.5.30/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    18657 2023-02-15 17:17:10.000000 home-assistant-intents-2023.5.30/LICENSE.md
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       72 2023-01-11 16:06:16.000000 home-assistant-intents-2023.5.30/MANIFEST.in
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1290 2023-05-30 16:41:22.618410 home-assistant-intents-2023.5.30/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      577 2023-05-30 16:40:56.000000 home-assistant-intents-2023.5.30/README.md
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-30 16:41:22.610411 home-assistant-intents-2023.5.30/home_assistant_intents/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      935 2023-04-17 16:30:47.000000 home-assistant-intents-2023.5.30/home_assistant_intents/__init__.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-30 16:41:22.610411 home-assistant-intents-2023.5.30/home_assistant_intents/data/
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-30 16:41:22.614410 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    15762 2023-05-30 16:41:15.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/ar.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    54166 2023-05-30 16:41:15.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/bg.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1903 2023-05-30 16:41:15.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/bn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    12544 2023-05-30 16:41:15.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/ca.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    21247 2023-05-30 16:41:15.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/cs.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    19985 2023-05-30 16:41:15.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/da.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    19712 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/de-CH.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    35266 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/de.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    61958 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/el.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    56864 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/en.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14986 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/es.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2885 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/fa.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    40173 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/fi.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     6747 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/fr-CA.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    78566 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/fr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5245 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/gl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1373 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/gu.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16181 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/he.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1525 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/hi.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    18547 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/hr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7330 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/hu.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3603 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/id.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3834 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/is.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14790 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/it.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3331 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/ka.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1197 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/kn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3160 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/ko.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11801 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/lb.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11322 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/lt.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     8002 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/lv.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11714 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/ml.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1367 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/mn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4824 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/ms.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16333 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/nb.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    74600 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/nl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    28368 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/pl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7860 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/pt-br.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    13050 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/pt.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    51451 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/ro.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14961 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/ru.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11029 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/sk.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3079 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/sl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4312 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/sr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11472 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/sv.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1197 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/sw.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1296 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/te.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5477 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/tr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14445 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/uk.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14341 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/ur.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    12024 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/vi.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16782 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/zh-cn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    13464 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/zh-hk.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    38206 2023-05-30 16:41:17.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/zh-tw.json
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-30 16:41:22.614410 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3727 2023-05-30 16:41:15.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/ar.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4257 2023-05-30 16:41:15.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/bg.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-05-30 16:41:15.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/bn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      725 2023-05-30 16:41:15.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/ca.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3620 2023-05-30 16:41:15.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/cs.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1479 2023-05-30 16:41:15.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/da.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1696 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/de-CH.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1656 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/de.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1209 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/el.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3236 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/en.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1608 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/es.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/fa.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5421 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/fi.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1876 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/fr-CA.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3063 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/fr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1350 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/gl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/gu.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1223 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/he.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/hi.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2274 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/hr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1723 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/hu.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1258 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/id.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      422 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/is.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1774 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/it.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      598 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/ka.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/kn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      180 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/ko.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2574 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/lb.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2145 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/lt.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2062 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/lv.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2720 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/ml.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/mn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1368 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/ms.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2174 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/nb.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2594 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/nl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1163 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/pl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      419 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/pt-br.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1950 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/pt.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3315 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/ro.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1857 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/ru.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1548 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/sk.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/sl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1554 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/sr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2563 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/sv.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/sw.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/te.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/tr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1681 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/uk.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1405 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/ur.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1510 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/vi.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2172 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/zh-cn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2008 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/zh-hk.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2322 2023-05-30 16:41:17.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/zh-tw.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1600 2023-05-30 16:41:17.000000 home-assistant-intents-2023.5.30/home_assistant_intents/domains.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-30 16:41:22.610411 home-assistant-intents-2023.5.30/home_assistant_intents.egg-info/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1290 2023-05-30 16:41:22.000000 home-assistant-intents-2023.5.30/home_assistant_intents.egg-info/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5253 2023-05-30 16:41:22.000000 home-assistant-intents-2023.5.30/home_assistant_intents.egg-info/SOURCES.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-05-30 16:41:22.000000 home-assistant-intents-2023.5.30/home_assistant_intents.egg-info/dependency_links.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       23 2023-05-30 16:41:22.000000 home-assistant-intents-2023.5.30/home_assistant_intents.egg-info/top_level.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-05-30 16:35:50.000000 home-assistant-intents-2023.5.30/home_assistant_intents.egg-info/zip-safe
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      990 2023-05-30 16:41:12.000000 home-assistant-intents-2023.5.30/pyproject.toml
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2023-05-30 16:41:22.618410 home-assistant-intents-2023.5.30/setup.cfg
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-05 15:46:39.333424 home-assistant-intents-2023.6.5/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    18657 2023-02-15 17:17:10.000000 home-assistant-intents-2023.6.5/LICENSE.md
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       72 2023-01-11 16:06:16.000000 home-assistant-intents-2023.6.5/MANIFEST.in
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1286 2023-06-05 15:46:39.333424 home-assistant-intents-2023.6.5/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      523 2023-05-30 16:59:24.000000 home-assistant-intents-2023.6.5/README.md
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-05 15:46:39.325424 home-assistant-intents-2023.6.5/home_assistant_intents/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      935 2023-04-17 16:30:47.000000 home-assistant-intents-2023.6.5/home_assistant_intents/__init__.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-05 15:46:39.325424 home-assistant-intents-2023.6.5/home_assistant_intents/data/
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-05 15:46:39.329424 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    15762 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/ar.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    54166 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/bg.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1903 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/bn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    12544 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/ca.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    21247 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/cs.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    19985 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/da.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    19712 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/de-CH.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    35995 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/de.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    61958 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/el.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    56864 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/en.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14986 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/es.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2885 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/fa.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    40173 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/fi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     6747 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/fr-CA.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    78566 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/fr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5245 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/gl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1373 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/gu.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16181 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/he.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1525 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/hi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    18547 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/hr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7330 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/hu.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3603 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/id.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3834 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/is.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14790 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/it.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3331 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/ka.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1197 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/kn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3160 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/ko.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11801 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/lb.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11322 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/lt.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     8002 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/lv.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11714 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/ml.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1367 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/mn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4824 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/ms.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16333 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/nb.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    74600 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/nl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    28368 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/pl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7860 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/pt-br.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    13050 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/pt.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    51451 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/ro.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14961 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/ru.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11029 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/sk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3079 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/sl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4312 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/sr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11472 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/sv.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1197 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/sw.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1296 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/te.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5477 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/tr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14445 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/uk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14341 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/ur.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    12024 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/vi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16782 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/zh-cn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    13464 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/zh-hk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    38206 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/zh-tw.json
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-05 15:46:39.333424 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3727 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/ar.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4257 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/bg.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/bn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      725 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/ca.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3620 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/cs.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1479 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/da.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1696 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/de-CH.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2248 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/de.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1209 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/el.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3236 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/en.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1608 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/es.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-06-05 15:46:32.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/fa.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5421 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/fi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1876 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/fr-CA.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3063 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/fr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1350 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/gl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/gu.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1223 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/he.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/hi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2274 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/hr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1723 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/hu.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1258 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/id.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      422 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/is.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1774 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/it.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      598 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/ka.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/kn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      180 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/ko.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2574 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/lb.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2145 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/lt.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2062 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/lv.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2720 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/ml.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/mn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1368 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/ms.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2174 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/nb.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2594 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/nl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1163 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/pl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      419 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/pt-br.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1950 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/pt.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3315 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/ro.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1857 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/ru.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1548 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/sk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/sl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1554 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/sr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2563 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/sv.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/sw.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/te.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/tr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1681 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/uk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1405 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/ur.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1510 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/vi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2172 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/zh-cn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2008 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/zh-hk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2322 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/data/light/zh-tw.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1600 2023-06-05 15:46:33.000000 home-assistant-intents-2023.6.5/home_assistant_intents/domains.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-06-05 15:46:39.325424 home-assistant-intents-2023.6.5/home_assistant_intents.egg-info/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1286 2023-06-05 15:46:38.000000 home-assistant-intents-2023.6.5/home_assistant_intents.egg-info/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5253 2023-06-05 15:46:39.000000 home-assistant-intents-2023.6.5/home_assistant_intents.egg-info/SOURCES.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-06-05 15:46:38.000000 home-assistant-intents-2023.6.5/home_assistant_intents.egg-info/dependency_links.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       23 2023-06-05 15:46:39.000000 home-assistant-intents-2023.6.5/home_assistant_intents.egg-info/top_level.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-05-30 16:35:50.000000 home-assistant-intents-2023.6.5/home_assistant_intents.egg-info/zip-safe
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1035 2023-06-05 15:45:56.000000 home-assistant-intents-2023.6.5/pyproject.toml
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2023-06-05 15:46:39.333424 home-assistant-intents-2023.6.5/setup.cfg
```

### Comparing `home-assistant-intents-2023.5.30/LICENSE.md` & `home-assistant-intents-2023.6.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/PKG-INFO` & `home-assistant-intents-2023.6.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: home-assistant-intents
-Version: 2023.5.30
+Version: 2023.6.5
 Summary: Intents for Home Assistant
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/home-assistant/intents
 Keywords: home,assistant,intent,recognition
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Home Assistant Intents Package
 
 Packaging for [intents](https://github.com/home-assistant/intents/)
@@ -25,30 +26,28 @@
 ## Install
 
 Clone the repo and create a virtual environment:
 
 ``` sh
 git clone --recursive https://github.com/home-assistant/intents-package
 cd intents-package
-python3 -m venv venv
-venv/bin/pip3 install --upgrade pip
-venv/bin/pip3 install -r requirements.txt
+script/setup
 ```
 
 
 ## Package
 
-Update the submodule
+Update the submodule:
 
 ``` sh
 git submodule update --remote
 ```
 
-Bump the version in `pyproject.toml` to `YYYY.M.D`
+Bump the version in `pyproject.toml` to `YYYY.M.D` and commit changes.
 
 Generate dist:
 
 ``` sh
 script/package
 ```
 
-Upload `.tar.gz` and `.whl` to PyPI.
+Upload `.tar.gz` and `.whl` in `dist/` to PyPI.
```

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/__init__.py` & `home-assistant-intents-2023.6.5/home_assistant_intents/__init__.py`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/ar.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/ar.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/bg.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/bg.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/bn.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/bn.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/ca.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/ca.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/cs.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/cs.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/da.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/da.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/de-CH.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/de-CH.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/de.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/de.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9904395517676768%*

 * *Differences: {"'expansion_rules'": "{'alle': '((alle|sämtliche)[r]|jede[r|s|n]|[die|der] "*

 * *                      "(ganze|komplette|sämtliche)[n]) [der]', 'luefter': '([den] Ventilator|[die] "*

 * *                      "Ventilatoren|[den|die] Lüfter)', 'alle_luefter': '<alle> "*

 * *                      "(Ventilatoren|Lüfter)', 'alle_lichter': '(<alle> "*

 * *                      '(<lichter>|Beleuchtung)|von allen '*

 * *                      "[Lichtern|Lampen|Leuchten|Beleuchtungen])'}",*

 * * "'intents'": "{'HassTurnOff': {'data': {0: {'sen […]*

```diff
@@ -1,17 +1,17 @@
 {
     "expansion_rules": {
         "abdeckung": "(das Rollo|die Rollos|die (Abdeckung|Abdeckungen)|(den|die) Rolll(a|\u00e4)den|die (Jalousie|Jalousien)|(den|die) Raffstore[s]|die (Markise|Markisen))",
         "absperren": "(zu|ab)<sperren>|verrieg(el|le)[n]",
         "aktivieren": "aktivier[e|en]",
-        "alle": "(alle|s\u00e4mtliche|jede[r|s|n]|[die] (ganze|komplette)[n]) [der]",
+        "alle": "((alle|s\u00e4mtliche)[r]|jede[r|s|n]|[die|der] (ganze|komplette|s\u00e4mtliche)[n]) [der]",
         "alle_abdeckungen": "<alle> (Rollos|Abdeckungen|Rolll(a|\u00e4)den|Jalousien|Raffstores|Markisen)",
         "alle_garagen": "<alle> (Garagen|Garagentore)",
-        "alle_lichter": "(<alle>[r] <lichter>|von allen [Lichtern|Lampen|Leuchten|Beleuchtungen]|[die] ganze Beleuchtung)",
-        "alle_luefter": "alle (Ventilatoren|L\u00fcfter)",
+        "alle_lichter": "(<alle> (<lichter>|Beleuchtung)|von allen [Lichtern|Lampen|Leuchten|Beleuchtungen])",
+        "alle_luefter": "<alle> (Ventilatoren|L\u00fcfter)",
         "alle_tore": "<alle> (Tore|Garagentore)",
         "an": "(an|ein|auf)",
         "area": "((in|an|auf) (der|dem)|im|am) {area}",
         "auf": "(auf|hoch|rauf|nach oben)",
         "aus": "(aus|ab|zu)",
         "ausfuehren": "(start[e|en]|ausf\u00fchren)",
         "batterie": "[die|der|des] (Batterie[n]|Akku[s])",
@@ -23,15 +23,15 @@
         "entsperren": "((ent|auf)<sperren>|\u00f6ffne|entrieg(el|le))[n]",
         "etwas": "[irgend][et]was",
         "garage": "(die Garage|die Garagen|das Garagentor|die Garagentore)",
         "irgend": "(irgend(ein[e][s|r]|welche[s])|einige[s]) [der]",
         "ladestand": "[der] [Lade][zu]Stand",
         "licht": "([das] Licht|[die] Lampe|[die] Beleuchtung)",
         "lichter": "[die|der|von den] (Lichter|Lichtern|Lampen|Leuchten|Beleuchtungen)",
-        "luefter": "(den Ventilator|die Ventilatoren|(den|die) L\u00fcfter)",
+        "luefter": "([den] Ventilator|[die] Ventilatoren|[den|die] L\u00fcfter)",
         "machen": "(mach[e|en])",
         "name": "[(der|den|dem|die|das)] {name}",
         "schalten": "(schalt[e|en])",
         "schliessen": "(schlie(\u00df|ss)[e|en]|zumachen|zu machen)",
         "schloss": "[das|die] (Schloss|Schl\u00f6sser)",
         "setzen": "(setz[e|en]|stell[e|en]|einstellen|\u00e4nder[e|n]|ver\u00e4nder[e|n])",
         "skript": "[das] Skript",
@@ -474,26 +474,30 @@
             ]
         },
         "HassTurnOff": {
             "data": [
                 {
                     "response": "fan_all",
                     "sentences": [
-                        "schalte <luefter> <area> <aus>",
-                        "schalte <area> <luefter> <aus>",
+                        "<schalten> <luefter> <area> <aus>",
+                        "<schalten> <area> <luefter> <aus>",
                         "stoppe <luefter> <area> [<aus>]",
                         "stoppe <area> <luefter> [<aus>]",
-                        "(mach|mache) <luefter> <area> <aus>",
-                        "(mach|mache) <area> <luefter> <aus>",
-                        "schalte <alle_luefter> [<area>] <aus>",
-                        "schalte [<area>] <alle_luefter> <aus>",
+                        "<machen> <luefter> <area> <aus>",
+                        "<machen> <area> <luefter> <aus>",
+                        "<luefter> <area> <aus>[<schalten>|<machen>]",
+                        "<area> <luefter> <aus>[<schalten>|<machen>]",
+                        "<schalten> <alle_luefter> [<area>] <aus>",
+                        "<schalten> <area> <alle_luefter> <aus>",
                         "stoppe <alle_luefter> [<area>] [<aus>]",
                         "stoppe [<area>] <alle_luefter> [<aus>]",
-                        "(mach|mache) <alle_luefter> [<area>] <aus>",
-                        "(mach|mache) [<area>] <alle_luefter> <aus>"
+                        "<machen> <alle_luefter> [<area>] <aus>",
+                        "<machen> <area> <alle_luefter> <aus>",
+                        "<alle_luefter> [<area>] <aus>[<schalten>|<machen>]",
+                        "<area> <alle_luefter> <aus>[<schalten>|<machen>]"
                     ],
                     "slots": {
                         "domain": "fan",
                         "name": "all"
                     }
                 },
                 {
@@ -694,26 +698,30 @@
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "fan_all",
                     "sentences": [
-                        "schalte <luefter> <area> <an>",
-                        "schalte <area> <luefter> <an>",
+                        "<schalten> <luefter> <area> <an>",
+                        "<schalten> <area> <luefter> <an>",
                         "starte <luefter> <area> [<an>]",
                         "starte <area> <luefter> [<an>]",
-                        "(mach|mache) <luefter> <area> <an>",
-                        "(mach|mache) <area> <luefter> <an>",
+                        "<machen> <luefter> <area> <an>",
+                        "<machen> <area> <luefter> <an>",
+                        "<luefter> <area> <an>[<schalten>|<machen>]",
+                        "<area> <luefter> <an>[<schalten>|<machen>]",
                         "starte <alle_luefter> [<area>] [<an>]",
                         "starte [<area>] <alle_luefter> [<an>]",
-                        "schalte <alle_luefter> [<area>] <an>",
-                        "schalte [<area>] <alle_luefter> <an>",
-                        "(mach|mache) <alle_luefter> [<area>] <an>",
-                        "(mach|mache) [<area>] <alle_luefter> <an>"
+                        "<schalten> <alle_luefter> [<area>] <an>",
+                        "<schalten> <area> <alle_luefter> <an>",
+                        "<machen> <alle_luefter> [<area>] <an>",
+                        "<machen> <area> <alle_luefter> <an>",
+                        "<alle_luefter> [<area>] <an>[<schalten>|<machen>]",
+                        "<area> <alle_luefter> <an>[<schalten>|<machen>]"
                     ],
                     "slots": {
                         "domain": "fan",
                         "name": "all"
                     }
                 },
                 {
@@ -789,14 +797,26 @@
         "brightness": {
             "range": {
                 "from": 0,
                 "to": 100,
                 "type": "percentage"
             }
         },
+        "brightness_level": {
+            "values": [
+                {
+                    "in": "(max[imale|imum]|h\u00f6chste|volle)",
+                    "out": 100
+                },
+                {
+                    "in": "(min[imale|imum]|niedrigste)",
+                    "out": 1
+                }
+            ]
+        },
         "bs_battery_charging_states": {
             "values": [
                 {
                     "in": "(l\u00e4dt|[auf][ge]laden) [auf]",
                     "out": "on"
                 },
                 {
```

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/el.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/el.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/en.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/en.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/es.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/es.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/fa.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/fa.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/fi.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/fi.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/fr-CA.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/fr-CA.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/fr.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/fr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/gl.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/gl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/gu.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/gu.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/he.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/he.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/hi.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/hi.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/hr.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/hr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/hu.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/hu.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/id.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/id.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/is.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/is.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/it.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/it.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/ka.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/ka.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/kn.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/kn.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/ko.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/ko.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/lb.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/lb.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/lt.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/lt.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/lv.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/lv.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/ml.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/ml.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/mn.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/mn.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/ms.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/ms.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/nb.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/nb.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/nl.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/nl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/pl.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/pl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/pt-br.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/pt-br.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/pt.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/pt.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/ro.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/ro.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/ru.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/ru.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/sk.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/sk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/sl.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/sl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/sr.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/sr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/sv.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/sv.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/sw.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/sw.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/te.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/te.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/tr.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/tr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/uk.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/uk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/ur.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/ur.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/vi.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/vi.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/zh-cn.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/zh-cn.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/zh-hk.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/zh-hk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/zh-tw.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/homeassistant/zh-tw.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/ar.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/ar.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/bg.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/bg.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/ca.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/ca.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/cs.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/cs.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/da.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/da.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/de-CH.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/de-CH.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/de.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/de.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9916666666666667%*

 * *Differences: {"'intents'": "{'HassLightSet': {'data': {insert: [(4, OrderedDict([('sentences', ['<setzen> "*

 * *              "<name> auf [die|das] {brightness_level:brightness} [Helligkeit|Stufe] [ein]', "*

 * *              "'<setzen> [die] Helligkeit [<von_dem>] <name> auf [die|das] "*

 * *              "{brightness_level:brightness} [Stufe] [ein]', '[die] Helligkeit [<von_dem>] <name> "*

 * *              "auf [die|das] {brightness_level:brightness} [Stufe] <setzen>', '<name> auf "*

 * *              "[die|das] {brightness_level:brightness […]*

```diff
@@ -31,14 +31,26 @@
                 },
                 {
                     "response": "color",
                     "sentences": [
                         "<setzen> die Farbe [<lichter>|<alle_lichter>] [<area>] auf {color}",
                         "die Farbe [<lichter>|<alle_lichter>] [<area>] auf {color} <setzen>"
                     ]
+                },
+                {
+                    "requires_context": {
+                        "domain": "light"
+                    },
+                    "response": "brightness",
+                    "sentences": [
+                        "<setzen> <name> auf [die|das] {brightness_level:brightness} [Helligkeit|Stufe] [ein]",
+                        "<setzen> [die] Helligkeit [<von_dem>] <name> auf [die|das] {brightness_level:brightness} [Stufe] [ein]",
+                        "[die] Helligkeit [<von_dem>] <name> auf [die|das] {brightness_level:brightness} [Stufe] <setzen>",
+                        "<name> auf [die|das] {brightness_level:brightness} [Helligkeit|Stufe] <setzen>"
+                    ]
                 }
             ]
         }
     },
     "language": "de",
     "responses": {
         "intents": {
```

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/el.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/el.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/en.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/en.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/es.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/es.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/fi.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/fi.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/fr-CA.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/fr-CA.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/fr.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/fr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/gl.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/gl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/he.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/he.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/hr.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/hr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/hu.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/hu.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/id.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/id.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/it.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/it.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/ka.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/ka.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/lb.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/lb.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/lt.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/lt.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/lv.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/lv.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/ml.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/ml.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/ms.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/ms.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/nb.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/nb.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/nl.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/nl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/pl.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/pl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/pt.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/pt.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/ro.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/ro.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/ru.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/ru.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/sk.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/sk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/sr.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/sr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/sv.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/sv.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/uk.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/uk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/ur.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/ur.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/vi.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/vi.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/zh-cn.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/zh-cn.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/zh-hk.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/zh-hk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/zh-tw.json` & `home-assistant-intents-2023.6.5/home_assistant_intents/data/light/zh-tw.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents/domains.py` & `home-assistant-intents-2023.6.5/home_assistant_intents/domains.py`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents.egg-info/PKG-INFO` & `home-assistant-intents-2023.6.5/home_assistant_intents.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: home-assistant-intents
-Version: 2023.5.30
+Version: 2023.6.5
 Summary: Intents for Home Assistant
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/home-assistant/intents
 Keywords: home,assistant,intent,recognition
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Home Assistant Intents Package
 
 Packaging for [intents](https://github.com/home-assistant/intents/)
@@ -25,30 +26,28 @@
 ## Install
 
 Clone the repo and create a virtual environment:
 
 ``` sh
 git clone --recursive https://github.com/home-assistant/intents-package
 cd intents-package
-python3 -m venv venv
-venv/bin/pip3 install --upgrade pip
-venv/bin/pip3 install -r requirements.txt
+script/setup
 ```
 
 
 ## Package
 
-Update the submodule
+Update the submodule:
 
 ``` sh
 git submodule update --remote
 ```
 
-Bump the version in `pyproject.toml` to `YYYY.M.D`
+Bump the version in `pyproject.toml` to `YYYY.M.D` and commit changes.
 
 Generate dist:
 
 ``` sh
 script/package
 ```
 
-Upload `.tar.gz` and `.whl` to PyPI.
+Upload `.tar.gz` and `.whl` in `dist/` to PyPI.
```

### Comparing `home-assistant-intents-2023.5.30/home_assistant_intents.egg-info/SOURCES.txt` & `home-assistant-intents-2023.6.5/home_assistant_intents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.5.30/pyproject.toml` & `home-assistant-intents-2023.6.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "home-assistant-intents"
-version     = "2023.5.30"
+version     = "2023.6.5"
 license     = {text = "Apache-2.0"}
 description = "Intents for Home Assistant"
 readme      = "README.md"
 authors     = [
     {name = "The Home Assistant Authors", email = "hello@home-assistant.io"}
 ]
 keywords    = ["home", "assistant", "intent", "recognition"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Topic :: Text Processing :: Linguistic",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 requires-python = ">=3.9.0"
 
 [project.urls]
 "Source Code" = "https://github.com/home-assistant/intents"
 
 [tool.setuptools]
```

