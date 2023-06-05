# Comparing `tmp/google-i18n-address-2.5.2.tar.gz` & `tmp/google_i18n_address-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-i18n-address-2.5.2.tar", last modified: Tue Jun 28 09:13:46 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `google-i18n-address-2.5.2.tar` & `google_i18n_address-3.0.0.tar`

### file list

```diff
@@ -1,272 +1,262 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 09:13:46.930881 google-i18n-address-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1467 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    14352 2022-06-28 09:13:46.926881 google-i18n-address-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13748 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 09:13:46.886881 google-i18n-address-2.5.2/google_i18n_address.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14352 2022-06-28 09:13:46.000000 google-i18n-address-2.5.2/google_i18n_address.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6696 2022-06-28 09:13:46.000000 google-i18n-address-2.5.2/google_i18n_address.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-28 09:13:46.000000 google-i18n-address-2.5.2/google_i18n_address.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-28 09:13:44.000000 google-i18n-address-2.5.2/google_i18n_address.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-06-28 09:13:46.000000 google-i18n-address-2.5.2/google_i18n_address.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-06-28 09:13:46.000000 google-i18n-address-2.5.2/google_i18n_address.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 09:13:46.886881 google-i18n-address-2.5.2/i18naddress/
--rw-r--r--   0 runner    (1001) docker     (121)    19131 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 09:13:46.926881 google-i18n-address-2.5.2/i18naddress/data/
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ac.json
--rw-r--r--   0 runner    (1001) docker     (121)     1848 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ad.json
--rw-r--r--   0 runner    (1001) docker     (121)     1792 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ae.json
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/af.json
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ag.json
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ai.json
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/al.json
--rw-r--r--   0 runner    (1001) docker     (121)  1973679 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/all.json
--rw-r--r--   0 runner    (1001) docker     (121)     2624 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/am.json
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ao.json
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/aq.json
--rw-r--r--   0 runner    (1001) docker     (121)     4301 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ar.json
--rw-r--r--   0 runner    (1001) docker     (121)      291 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/as.json
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/at.json
--rw-r--r--   0 runner    (1001) docker     (121)     2165 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/au.json
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/aw.json
--rw-r--r--   0 runner    (1001) docker     (121)      304 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ax.json
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/az.json
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ba.json
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/bb.json
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/bd.json
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/be.json
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/bf.json
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/bg.json
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/bh.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/bi.json
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/bj.json
--rw-r--r--   0 runner    (1001) docker     (121)      296 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/bl.json
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/bm.json
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/bn.json
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/bo.json
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/bq.json
--rw-r--r--   0 runner    (1001) docker     (121)   604459 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/br.json
--rw-r--r--   0 runner    (1001) docker     (121)     2814 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/bs.json
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/bt.json
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/bv.json
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/bw.json
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/by.json
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/bz.json
--rw-r--r--   0 runner    (1001) docker     (121)     4534 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ca.json
--rw-r--r--   0 runner    (1001) docker     (121)      151 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/cc.json
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/cd.json
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/cf.json
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/cg.json
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ch.json
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ci.json
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ck.json
--rw-r--r--   0 runner    (1001) docker     (121)    41904 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/cl.json
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/cm.json
--rw-r--r--   0 runner    (1001) docker     (121)   870659 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/cn.json
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/co.json
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/cr.json
--rw-r--r--   0 runner    (1001) docker     (121)     2034 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/cu.json
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/cv.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/cw.json
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/cx.json
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/cy.json
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/cz.json
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/de.json
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/dj.json
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/dk.json
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/dm.json
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/do.json
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/dz.json
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ec.json
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ee.json
--rw-r--r--   0 runner    (1001) docker     (121)     6332 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/eg.json
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/eh.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/er.json
--rw-r--r--   0 runner    (1001) docker     (121)    24420 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/es.json
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/et.json
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/fi.json
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/fj.json
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/fk.json
--rw-r--r--   0 runner    (1001) docker     (121)      318 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/fm.json
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/fo.json
--rw-r--r--   0 runner    (1001) docker     (121)      293 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/fr.json
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ga.json
--rw-r--r--   0 runner    (1001) docker     (121)      821 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/gb.json
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/gd.json
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ge.json
--rw-r--r--   0 runner    (1001) docker     (121)      290 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/gf.json
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/gg.json
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/gh.json
--rw-r--r--   0 runner    (1001) docker     (121)      151 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/gi.json
--rw-r--r--   0 runner    (1001) docker     (121)      151 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/gl.json
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/gm.json
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/gn.json
--rw-r--r--   0 runner    (1001) docker     (121)      290 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/gp.json
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/gq.json
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/gr.json
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/gs.json
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/gt.json
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/gu.json
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/gw.json
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/gy.json
--rw-r--r--   0 runner    (1001) docker     (121)    44334 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/hk.json
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/hm.json
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/hn.json
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/hr.json
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ht.json
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/hu.json
--rw-r--r--   0 runner    (1001) docker     (121)     5651 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/id.json
--rw-r--r--   0 runner    (1001) docker     (121)     3287 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ie.json
--rw-r--r--   0 runner    (1001) docker     (121)      203 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/il.json
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/im.json
--rw-r--r--   0 runner    (1001) docker     (121)    14606 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/in.json
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/io.json
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/iq.json
--rw-r--r--   0 runner    (1001) docker     (121)     7312 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ir.json
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/is.json
--rw-r--r--   0 runner    (1001) docker     (121)    14096 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/it.json
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/je.json
--rw-r--r--   0 runner    (1001) docker     (121)     1723 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/jm.json
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/jo.json
--rw-r--r--   0 runner    (1001) docker     (121)     7879 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/jp.json
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ke.json
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/kg.json
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/kh.json
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ki.json
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/km.json
--rw-r--r--   0 runner    (1001) docker     (121)      406 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/kn.json
--rw-r--r--   0 runner    (1001) docker     (121)     1923 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/kp.json
--rw-r--r--   0 runner    (1001) docker     (121)    56274 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/kr.json
--rw-r--r--   0 runner    (1001) docker     (121)      137 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/kw.json
--rw-r--r--   0 runner    (1001) docker     (121)      595 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ky.json
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/kz.json
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/la.json
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/lb.json
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/lc.json
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/li.json
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/lk.json
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/lr.json
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ls.json
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/lt.json
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/lu.json
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/lv.json
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ly.json
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ma.json
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/mc.json
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/md.json
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/me.json
--rw-r--r--   0 runner    (1001) docker     (121)      250 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/mf.json
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/mg.json
--rw-r--r--   0 runner    (1001) docker     (121)      304 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/mh.json
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/mk.json
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ml.json
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/mm.json
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/mn.json
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/mo.json
--rw-r--r--   0 runner    (1001) docker     (121)      317 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/mp.json
--rw-r--r--   0 runner    (1001) docker     (121)      287 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/mq.json
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/mr.json
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ms.json
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/mt.json
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/mu.json
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/mv.json
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/mw.json
--rw-r--r--   0 runner    (1001) docker     (121)     6245 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/mx.json
--rw-r--r--   0 runner    (1001) docker     (121)     3112 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/my.json
--rw-r--r--   0 runner    (1001) docker     (121)     1298 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/mz.json
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/na.json
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/nc.json
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ne.json
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/nf.json
--rw-r--r--   0 runner    (1001) docker     (121)     3845 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ng.json
--rw-r--r--   0 runner    (1001) docker     (121)     2693 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ni.json
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/nl.json
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/no.json
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/np.json
--rw-r--r--   0 runner    (1001) docker     (121)     2003 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/nr.json
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/nu.json
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/nz.json
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/om.json
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/pa.json
--rw-r--r--   0 runner    (1001) docker     (121)     3212 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/pe.json
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/pf.json
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/pg.json
--rw-r--r--   0 runner    (1001) docker     (121)    14403 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ph.json
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/pk.json
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/pl.json
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/pm.json
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/pn.json
--rw-r--r--   0 runner    (1001) docker     (121)      287 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/pr.json
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ps.json
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/pt.json
--rw-r--r--   0 runner    (1001) docker     (121)      289 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/pw.json
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/py.json
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/qa.json
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/re.json
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ro.json
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/rs.json
--rw-r--r--   0 runner    (1001) docker     (121)    33040 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ru.json
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/rw.json
--rw-r--r--   0 runner    (1001) docker     (121)      137 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/sa.json
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/sb.json
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/sc.json
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/sd.json
--rw-r--r--   0 runner    (1001) docker     (121)      307 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/se.json
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/sg.json
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/sh.json
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/si.json
--rw-r--r--   0 runner    (1001) docker     (121)      232 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/sj.json
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/sk.json
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/sl.json
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/sm.json
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/sn.json
--rw-r--r--   0 runner    (1001) docker     (121)     2217 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/so.json
--rw-r--r--   0 runner    (1001) docker     (121)     1209 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/sr.json
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ss.json
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/st.json
--rw-r--r--   0 runner    (1001) docker     (121)     2950 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/sv.json
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/sx.json
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/sy.json
--rw-r--r--   0 runner    (1001) docker     (121)      206 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/sz.json
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ta.json
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/tc.json
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/td.json
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/tf.json
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/tg.json
--rw-r--r--   0 runner    (1001) docker     (121)    16648 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/th.json
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/tj.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/tk.json
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/tl.json
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/tm.json
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/tn.json
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/to.json
--rw-r--r--   0 runner    (1001) docker     (121)     9626 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/tr.json
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/tt.json
--rw-r--r--   0 runner    (1001) docker     (121)     1116 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/tv.json
--rw-r--r--   0 runner    (1001) docker     (121)    71096 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/tw.json
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/tz.json
--rw-r--r--   0 runner    (1001) docker     (121)    10362 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ua.json
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ug.json
--rw-r--r--   0 runner    (1001) docker     (121)      291 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/um.json
--rw-r--r--   0 runner    (1001) docker     (121)    11125 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/us.json
--rw-r--r--   0 runner    (1001) docker     (121)     2722 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/uy.json
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/uz.json
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/va.json
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/vc.json
--rw-r--r--   0 runner    (1001) docker     (121)     2904 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ve.json
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/vg.json
--rw-r--r--   0 runner    (1001) docker     (121)      338 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/vi.json
--rw-r--r--   0 runner    (1001) docker     (121)    10638 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/vn.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/vu.json
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/wf.json
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ws.json
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/xk.json
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/ye.json
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/yt.json
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/za.json
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/zm.json
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/zw.json
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/data/zz.json
--rw-r--r--   0 runner    (1001) docker     (121)     3112 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/i18naddress/downloader.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-28 09:13:46.930881 google-i18n-address-2.5.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1989 2022-06-28 09:13:33.000000 google-i18n-address-2.5.2/setup.py
+-rw-r--r--   0        0        0    18796 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/__init__.py
+-rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/downloader.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/scripts.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ac.json
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ad.json
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ae.json
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/af.json
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ag.json
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ai.json
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/al.json
+-rw-r--r--   0        0        0  1978328 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/all.json
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/am.json
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ao.json
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/aq.json
+-rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ar.json
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/as.json
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/at.json
+-rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/au.json
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/aw.json
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ax.json
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/az.json
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ba.json
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/bb.json
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/bd.json
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/be.json
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/bf.json
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/bg.json
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/bh.json
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/bi.json
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/bj.json
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/bl.json
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/bm.json
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/bn.json
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/bo.json
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/bq.json
+-rw-r--r--   0        0        0   604459 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/br.json
+-rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/bs.json
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/bt.json
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/bv.json
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/bw.json
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/by.json
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/bz.json
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ca.json
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/cc.json
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/cd.json
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/cf.json
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/cg.json
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ch.json
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ci.json
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ck.json
+-rw-r--r--   0        0        0    42698 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/cl.json
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/cm.json
+-rw-r--r--   0        0        0   870883 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/cn.json
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/co.json
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/cr.json
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/cu.json
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/cv.json
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/cw.json
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/cx.json
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/cy.json
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/cz.json
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/de.json
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/dj.json
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/dk.json
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/dm.json
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/do.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/dz.json
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ec.json
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ee.json
+-rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/eg.json
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/eh.json
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/er.json
+-rw-r--r--   0        0        0    24348 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/es.json
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/et.json
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/fi.json
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/fj.json
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/fk.json
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/fm.json
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/fo.json
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/fr.json
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ga.json
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/gb.json
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/gd.json
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ge.json
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/gf.json
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/gg.json
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/gh.json
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/gi.json
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/gl.json
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/gm.json
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/gn.json
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/gp.json
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/gq.json
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/gr.json
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/gs.json
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/gt.json
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/gu.json
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/gw.json
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/gy.json
+-rw-r--r--   0        0        0    44334 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/hk.json
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/hm.json
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/hn.json
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/hr.json
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ht.json
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/hu.json
+-rw-r--r--   0        0        0     5651 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/id.json
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ie.json
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/il.json
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/im.json
+-rw-r--r--   0        0        0    14606 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/in.json
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/io.json
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/iq.json
+-rw-r--r--   0        0        0     7312 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ir.json
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/is.json
+-rw-r--r--   0        0        0    14096 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/it.json
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/je.json
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/jm.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/jo.json
+-rw-r--r--   0        0        0     7879 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/jp.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ke.json
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/kg.json
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/kh.json
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ki.json
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/km.json
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/kn.json
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/kp.json
+-rw-r--r--   0        0        0    56280 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/kr.json
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/kw.json
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ky.json
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/kz.json
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/la.json
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/lb.json
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/lc.json
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/li.json
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/lk.json
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/lr.json
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ls.json
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/lt.json
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/lu.json
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/lv.json
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ly.json
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ma.json
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/mc.json
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/md.json
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/me.json
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/mf.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/mg.json
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/mh.json
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/mk.json
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ml.json
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/mm.json
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/mn.json
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/mo.json
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/mp.json
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/mq.json
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/mr.json
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ms.json
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/mt.json
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/mu.json
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/mv.json
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/mw.json
+-rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/mx.json
+-rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/my.json
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/mz.json
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/na.json
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/nc.json
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ne.json
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/nf.json
+-rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ng.json
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ni.json
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/nl.json
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/no.json
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/np.json
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/nr.json
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/nu.json
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/nz.json
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/om.json
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/pa.json
+-rw-r--r--   0        0        0     3212 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/pe.json
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/pf.json
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/pg.json
+-rw-r--r--   0        0        0    14403 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ph.json
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/pk.json
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/pl.json
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/pm.json
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/pn.json
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/pr.json
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ps.json
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/pt.json
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/pw.json
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/py.json
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/qa.json
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/re.json
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ro.json
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/rs.json
+-rw-r--r--   0        0        0    33040 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ru.json
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/rw.json
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/sa.json
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/sb.json
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/sc.json
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/sd.json
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/se.json
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/sg.json
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/sh.json
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/si.json
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/sj.json
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/sk.json
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/sl.json
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/sm.json
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/sn.json
+-rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/so.json
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/sr.json
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ss.json
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/st.json
+-rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/sv.json
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/sx.json
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/sy.json
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/sz.json
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ta.json
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/tc.json
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/td.json
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/tf.json
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/tg.json
+-rw-r--r--   0        0        0    16648 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/th.json
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/tj.json
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/tk.json
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/tl.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/tm.json
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/tn.json
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/to.json
+-rw-r--r--   0        0        0     9626 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/tr.json
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/tt.json
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/tv.json
+-rw-r--r--   0        0        0    71130 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/tw.json
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/tz.json
+-rw-r--r--   0        0        0    10362 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ua.json
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ug.json
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/um.json
+-rw-r--r--   0        0        0    11125 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/us.json
+-rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/uy.json
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/uz.json
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/va.json
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/vc.json
+-rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ve.json
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/vg.json
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/vi.json
+-rw-r--r--   0        0        0    10638 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/vn.json
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/vu.json
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/wf.json
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ws.json
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/xk.json
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/ye.json
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/yt.json
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/za.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/zm.json
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/zw.json
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/i18naddress/data/zz.json
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/.gitignore
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/LICENSE
+-rw-r--r--   0        0        0    13625 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/README.rst
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0    14932 2020-02-02 00:00:00.000000 google_i18n_address-3.0.0/PKG-INFO
```

### Comparing `google-i18n-address-2.5.2/LICENSE` & `google_i18n_address-3.0.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2010-2016, Mirumee Software
+Copyright (c) 2010-2023, Mirumee Software
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright
    notice, this list of conditions and the following disclaimer.
```

### Comparing `google-i18n-address-2.5.2/PKG-INFO` & `google_i18n_address-3.0.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,11 @@
-Metadata-Version: 2.1
-Name: google-i18n-address
-Version: 2.5.2
-Summary: Address validation helpers for Google's i18n address database
-Home-page: https://github.com/mirumee/google-i18n-address
-Author: Mirumee Software
-Author-email: hello@mirumee.com
-License: BSD
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Environment :: Web Environment
-Classifier: Topic :: Software Development :: Internationalization
-License-File: LICENSE
-
 Google i18n address
 ===========================================================================================
 
-|codecov.io| |Circle CI| |PyPi downloads| |requires.io| |PyPi version| |PyPi pythons| |GitHub|
+|codecov.io| |GH Actions| |PyPi downloads| |PyPi version| |PyPi pythons|
 
 This package contains a copy of `Google's i18n
 address <https://chromium-i18n.appspot.com/ssl-address>`_ metadata repository
 that contains great data but comes with no uptime guarantees.
 
 Contents of this package will allow you to programatically build address
 forms that adhere to rules of a particular region or country, validate
@@ -31,15 +15,15 @@
 The package also contains a Python interface for address validation.
 
 Addresses validation
 --------------------
 
 The ``normalize_address`` function checks the address and either returns its
 canonical form (suitable for storage and use in addressing envelopes) or
-raises an ``InvalidAddress`` exception that contains a list of errors.
+raises an ``InvalidAddressError`` exception that contains a list of errors.
 
 
 Address fields
 ~~~~~~~~~~~~~~
 
 Here is the list of recognized fields:
 
@@ -61,18 +45,18 @@
 Errors
 ~~~~~~
 
 Address validation with only country code:
 
 .. code:: python
 
-    >>> from i18naddress import InvalidAddress, normalize_address
+    >>> from i18naddress import InvalidAddressError, normalize_address
     >>> try:
     ...     address = normalize_address({'country_code': 'US'})
-    ... except InvalidAddress as e:
+    ... except InvalidAddressError as e:
     ...     print(e.errors)
     ...
     {'city': 'required',
      'country_area': 'required',
      'postal_code': 'required',
      'street_address': 'required'}
 
@@ -96,23 +80,23 @@
      'sorting_code': '',
      'street_address': '1600 Amphitheatre Pkwy'}
 
 Postal code/zip code validation example:
 
 .. code:: python
 
-    >>> from i18naddress import InvalidAddress, normalize_address
+    >>> from i18naddress import InvalidAddressError, normalize_address
     >>> try:
     ...     address = normalize_address({
     ...         'country_code': 'US',
     ...         'country_area': 'California',
     ...         'city': 'Mountain View',
     ...         'postal_code': '74043',
     ...         'street_address': '1600 Amphitheatre Pkwy'})
-    ... except InvalidAddress as e:
+    ... except InvalidAddressError as e:
     ...     print(e.errors)
     ...
     {'postal_code': 'invalid'}
 
 
 Address latinization
 ~~~~~~~~~~~~~~~~~~~~
@@ -290,15 +274,15 @@
 
 Django forms will return only required address fields in ``form.cleaned_data`` dict. So addresses in the database will be normalized.
 
 .. code:: python
 
     from django import forms
 
-    from i18naddress import InvalidAddress, normalize_address, get_validation_rules
+    from i18naddress import InvalidAddressError, normalize_address, get_validation_rules
 
 
     class AddressForm(forms.Form):
 
         COUNTRY_CHOICES = [
             ('PL', 'Poland'),
             ('AE', 'United Arab Emirates'),
@@ -335,19 +319,17 @@
             return valid_address or clean_data
 
 
 .. image:: https://ga-beacon.appspot.com/UA-10159761-14/mirumee/google-i18n-address?pixel
 
 .. |codecov.io| image:: https://img.shields.io/codecov/c/github/mirumee/google-i18n-address.svg
    :target: https://codecov.io/github/mirumee/google-i18n-address?branch=master
-.. |Circle CI| image:: https://img.shields.io/circleci/project/mirumee/google-i18n-address.svg
-   :target: https://circleci.com/gh/mirumee/google-i18n-address/tree/master
+.. |GH Actions| image:: https://github.com/mirumee/google-i18n-address/actions/workflows/python-package.yml/badge.svg?branch=master
+   :target: https://github.com/mirumee/google-i18n-address/actions?query=branch%3Amaster+
 .. |PyPi downloads| image:: https://img.shields.io/pypi/dm/google-i18n-address.svg
    :target: https://pypi.python.org/pypi/google-i18n-address
 .. |PyPi pythons| image:: https://img.shields.io/pypi/pyversions/google-i18n-address.svg
    :target: https://pypi.python.org/pypi/google-i18n-address
 .. |PyPi version| image:: https://img.shields.io/pypi/v/google-i18n-address.svg
    :target: https://pypi.python.org/pypi/google-i18n-address
 .. |GitHub| image:: https://img.shields.io/github/stars/mirumee/google-i18n-address.svg?style=social
    :target: https://github.com/mirumee/google-i18n-address
-.. |requires.io| image:: https://img.shields.io/requires/github/mirumee/google-i18n-address.svg
-   :target: https://requires.io/github/mirumee/google-i18n-address/requirements/?branch=master
```

### Comparing `google-i18n-address-2.5.2/README.rst` & `google_i18n_address-3.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,41 @@
+Metadata-Version: 2.1
+Name: google-i18n-address
+Version: 3.0.0
+Summary: Address validation helpers for Google's i18n address database
+Project-URL: Homepage, https://github.com/mirumee/google-i18n-address
+Project-URL: Repository, https://github.com/mirumee/google-i18n-address
+Project-URL: Bug Tracker, https://github.com/mirumee/google-i18n-address/issues
+Author-email: Mirumee Software <hello@mirumee.com>
+License-Expression: BSD-3-Clause
+License-File: LICENSE
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Web Environment
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Internationalization
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: requests>=2.7.0
+Provides-Extra: dev
+Requires-Dist: black; extra == 'dev'
+Requires-Dist: ruff; extra == 'dev'
+Provides-Extra: test
+Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pytest-cov; extra == 'test'
+Description-Content-Type: text/x-rst
+
 Google i18n address
 ===========================================================================================
 
-|codecov.io| |Circle CI| |PyPi downloads| |requires.io| |PyPi version| |PyPi pythons|
+|codecov.io| |GH Actions| |PyPi downloads| |PyPi version| |PyPi pythons|
 
 This package contains a copy of `Google's i18n
 address <https://chromium-i18n.appspot.com/ssl-address>`_ metadata repository
 that contains great data but comes with no uptime guarantees.
 
 Contents of this package will allow you to programatically build address
 forms that adhere to rules of a particular region or country, validate
@@ -15,15 +45,15 @@
 The package also contains a Python interface for address validation.
 
 Addresses validation
 --------------------
 
 The ``normalize_address`` function checks the address and either returns its
 canonical form (suitable for storage and use in addressing envelopes) or
-raises an ``InvalidAddress`` exception that contains a list of errors.
+raises an ``InvalidAddressError`` exception that contains a list of errors.
 
 
 Address fields
 ~~~~~~~~~~~~~~
 
 Here is the list of recognized fields:
 
@@ -45,18 +75,18 @@
 Errors
 ~~~~~~
 
 Address validation with only country code:
 
 .. code:: python
 
-    >>> from i18naddress import InvalidAddress, normalize_address
+    >>> from i18naddress import InvalidAddressError, normalize_address
     >>> try:
     ...     address = normalize_address({'country_code': 'US'})
-    ... except InvalidAddress as e:
+    ... except InvalidAddressError as e:
     ...     print(e.errors)
     ...
     {'city': 'required',
      'country_area': 'required',
      'postal_code': 'required',
      'street_address': 'required'}
 
@@ -80,23 +110,23 @@
      'sorting_code': '',
      'street_address': '1600 Amphitheatre Pkwy'}
 
 Postal code/zip code validation example:
 
 .. code:: python
 
-    >>> from i18naddress import InvalidAddress, normalize_address
+    >>> from i18naddress import InvalidAddressError, normalize_address
     >>> try:
     ...     address = normalize_address({
     ...         'country_code': 'US',
     ...         'country_area': 'California',
     ...         'city': 'Mountain View',
     ...         'postal_code': '74043',
     ...         'street_address': '1600 Amphitheatre Pkwy'})
-    ... except InvalidAddress as e:
+    ... except InvalidAddressError as e:
     ...     print(e.errors)
     ...
     {'postal_code': 'invalid'}
 
 
 Address latinization
 ~~~~~~~~~~~~~~~~~~~~
@@ -274,15 +304,15 @@
 
 Django forms will return only required address fields in ``form.cleaned_data`` dict. So addresses in the database will be normalized.
 
 .. code:: python
 
     from django import forms
 
-    from i18naddress import InvalidAddress, normalize_address, get_validation_rules
+    from i18naddress import InvalidAddressError, normalize_address, get_validation_rules
 
 
     class AddressForm(forms.Form):
 
         COUNTRY_CHOICES = [
             ('PL', 'Poland'),
             ('AE', 'United Arab Emirates'),
@@ -319,19 +349,17 @@
             return valid_address or clean_data
 
 
 .. image:: https://ga-beacon.appspot.com/UA-10159761-14/mirumee/google-i18n-address?pixel
 
 .. |codecov.io| image:: https://img.shields.io/codecov/c/github/mirumee/google-i18n-address.svg
    :target: https://codecov.io/github/mirumee/google-i18n-address?branch=master
-.. |Circle CI| image:: https://img.shields.io/circleci/project/mirumee/google-i18n-address.svg
-   :target: https://circleci.com/gh/mirumee/google-i18n-address/tree/master
+.. |GH Actions| image:: https://github.com/mirumee/google-i18n-address/actions/workflows/python-package.yml/badge.svg?branch=master
+   :target: https://github.com/mirumee/google-i18n-address/actions?query=branch%3Amaster+
 .. |PyPi downloads| image:: https://img.shields.io/pypi/dm/google-i18n-address.svg
    :target: https://pypi.python.org/pypi/google-i18n-address
 .. |PyPi pythons| image:: https://img.shields.io/pypi/pyversions/google-i18n-address.svg
    :target: https://pypi.python.org/pypi/google-i18n-address
 .. |PyPi version| image:: https://img.shields.io/pypi/v/google-i18n-address.svg
    :target: https://pypi.python.org/pypi/google-i18n-address
 .. |GitHub| image:: https://img.shields.io/github/stars/mirumee/google-i18n-address.svg?style=social
    :target: https://github.com/mirumee/google-i18n-address
-.. |requires.io| image:: https://img.shields.io/requires/github/mirumee/google-i18n-address.svg
-   :target: https://requires.io/github/mirumee/google-i18n-address/requirements/?branch=master
```

### Comparing `google-i18n-address-2.5.2/i18naddress/__init__.py` & `google_i18n_address-3.0.0/i18naddress/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-from __future__ import unicode_literals
-
-import io
 import json
 import os
 import re
 from collections import OrderedDict
 
 VALID_COUNTRY_CODE = re.compile(r"^\w{2,3}$")
 VALIDATION_DATA_DIR = os.path.join(os.path.dirname(__file__), "data")
@@ -22,31 +19,31 @@
 }
 
 KNOWN_FIELDS = set(FIELD_MAPPING.values()) | {"country_code"}
 
 
 def load_validation_data(country_code="all"):
     if not VALID_COUNTRY_CODE.match(country_code):
-        raise ValueError("%r is not a valid country code" % (country_code,))
+        raise ValueError(f"{country_code!r} is not a valid country code")
     country_code = country_code.lower()
     try:
         # VALIDATION_DATA_PATH may have '%' symbols
         # for backwards compatability if VALIDATION_DATA_PATH is imported
         # by consumers of this package.
         path = VALIDATION_DATA_PATH % (country_code,)
     except TypeError:
         path = os.path.join(VALIDATION_DATA_DIR, "%s.json" % country_code)
 
     if not os.path.exists(path):
-        raise ValueError("%r is not a valid country code" % (country_code,))
-    with io.open(path, encoding="utf-8") as data:
+        raise ValueError(f"{country_code!r} is not a valid country code")
+    with open(path, encoding="utf-8") as data:
         return json.load(data)
 
 
-class ValidationRules(object):
+class ValidationRules:
     __slots__ = [
         "country_code",
         "country_name",
         "address_format",
         "address_latin_format",
         "allowed_fields",
         "required_fields",
@@ -100,32 +97,31 @@
         self.postal_code_matchers = postal_code_matchers
         self.postal_code_examples = postal_code_examples
         self.postal_code_prefix = postal_code_prefix
 
     def __repr__(self):
         return (
             "ValidationRules("
-            "country_code=%r, "
-            "country_name=%r, "
-            "address_format=%r, "
-            "address_latin_format=%r, "
-            "allowed_fields=%r, "
-            "required_fields=%r, "
-            "upper_fields=%r, "
-            "country_area_type=%r, "
-            "country_area_choices=%r, "
-            "city_type=%r, "
-            "city_choices=%r, "
-            "city_area_type=%r, "
-            "city_area_choices=%r, "
-            "postal_code_type=%r, "
-            "postal_code_matchers=%r, "
-            "postal_code_examples=%r, "
-            "postal_code_prefix=%r)"
-            % (
+            "country_code={!r}, "
+            "country_name={!r}, "
+            "address_format={!r}, "
+            "address_latin_format={!r}, "
+            "allowed_fields={!r}, "
+            "required_fields={!r}, "
+            "upper_fields={!r}, "
+            "country_area_type={!r}, "
+            "country_area_choices={!r}, "
+            "city_type={!r}, "
+            "city_choices={!r}, "
+            "city_area_type={!r}, "
+            "city_area_choices={!r}, "
+            "postal_code_type={!r}, "
+            "postal_code_matchers={!r}, "
+            "postal_code_examples={!r}, "
+            "postal_code_prefix={!r})".format(
                 self.country_code,
                 self.country_name,
                 self.address_format,
                 self.address_latin_format,
                 self.allowed_fields,
                 self.required_fields,
                 self.upper_fields,
@@ -174,15 +170,15 @@
             ]
     return choices
 
 
 def _compact_choices(choices):
     value_map = OrderedDict()
     for key, value in choices:
-        if not key in value_map:
+        if key not in value_map:
             value_map[key] = set()
         value_map[key].add(value)
     return [
         (key, value) for key, values in value_map.items() for value in sorted(values)
     ]
 
 
@@ -198,15 +194,15 @@
 
 def _load_country_data(country_code):
     database = load_validation_data("zz")
     country_data = database["ZZ"]
     if country_code:
         country_code = country_code.upper()
         if country_code.lower() == "zz":
-            raise ValueError("%r is not a valid country code" % (country_code,))
+            raise ValueError(f"{country_code!r} is not a valid country code")
         database = load_validation_data(country_code.lower())
         country_data.update(database[country_code])
     return country_data, database
 
 
 def get_validation_rules(address):
     country_code = address.get("country_code", "").upper()
@@ -249,32 +245,28 @@
                     language is None or language == country_data["lang"]
                 )
                 matched_country_area = None
                 matched_city = None
                 if is_default_language:
                     localized_country_data = database[country_code]
                 else:
-                    localized_country_data = database[
-                        "%s--%s" % (country_code, language)
-                    ]
+                    localized_country_data = database[f"{country_code}--{language}"]
                 localized_country_area_choices = _make_choices(localized_country_data)
                 country_area_choices += localized_country_area_choices
                 existing_choice = country_area is not None
                 matched_country_area = country_area = _match_choices(
                     address.get("country_area"), localized_country_area_choices
                 )
                 if matched_country_area:
                     # third level of data is for cities
                     if is_default_language:
-                        country_area_data = database[
-                            "%s/%s" % (country_code, country_area)
-                        ]
+                        country_area_data = database[f"{country_code}/{country_area}"]
                     else:
                         country_area_data = database[
-                            "%s/%s--%s" % (country_code, country_area, language)
+                            f"{country_code}/{country_area}--{language}"
                         ]
                     if not existing_choice:
                         if "zip" in country_area_data:
                             postal_code_matchers.append(
                                 re.compile("^" + country_area_data["zip"])
                             )
                         if "zipex" in country_area_data:
@@ -286,20 +278,19 @@
                         matched_city = city = _match_choices(
                             address.get("city"), localized_city_choices
                         )
                     if matched_city:
                         # fourth level of data is for dependent sublocalities
                         if is_default_language:
                             city_data = database[
-                                "%s/%s/%s" % (country_code, country_area, city)
+                                f"{country_code}/{country_area}/{city}"
                             ]
                         else:
                             city_data = database[
-                                "%s/%s/%s--%s"
-                                % (country_code, country_area, city, language)
+                                f"{country_code}/{country_area}/{city}--{language}"
                             ]
                         if not existing_choice:
                             if "zip" in city_data:
                                 postal_code_matchers.append(
                                     re.compile("^" + city_data["zip"])
                                 )
                             if "zipex" in city_data:
@@ -310,21 +301,19 @@
                             existing_choice = city_area is not None
                             matched_city_area = city_area = _match_choices(
                                 address.get("city_area"), localized_city_area_choices
                             )
                             if matched_city_area:
                                 if is_default_language:
                                     city_area_data = database[
-                                        "%s/%s/%s/%s"
-                                        % (country_code, country_area, city, city_area)
+                                        f"{country_code}/{country_area}/{city}/{city_area}"
                                     ]
                                 else:
                                     city_area_data = database[
-                                        "%s/%s/%s/%s--%s"
-                                        % (
+                                        "{}/{}/{}/{}--{}".format(
                                             country_code,
                                             country_area,
                                             city,
                                             city_area,
                                             language,
                                         )
                                     ]
@@ -358,17 +347,17 @@
         postal_code_type,
         postal_code_matchers,
         postal_code_examples,
         postal_code_prefix,
     )
 
 
-class InvalidAddress(ValueError):
+class InvalidAddressError(ValueError):
     def __init__(self, message, errors):
-        super(InvalidAddress, self).__init__(message)
+        super().__init__(message)
         self.errors = errors
 
 
 def _normalize_field(name, rules, data, choices, errors):
     value = data.get(name)
     if name in rules.upper_fields and value is not None:
         value = value.upper()
@@ -414,15 +403,15 @@
             for matcher in rules.postal_code_matchers:
                 if not matcher.match(postal_code):
                     errors["postal_code"] = "invalid"
                     break
         _normalize_field("street_address", rules, cleaned_data, [], errors)
         _normalize_field("sorting_code", rules, cleaned_data, [], errors)
     if errors:
-        raise InvalidAddress("Invalid address", errors)
+        raise InvalidAddressError("Invalid address", errors)
     return cleaned_data
 
 
 def _format_address_line(line_format, address, rules):
     def _get_field(name):
         value = address.get(name, "")
         if name in rules.upper_fields:
@@ -478,28 +467,28 @@
         address = normalize_address(address)
     cleaned_data = address.copy()
     country_code = address.get("country_code", "").upper()
     dummy_country_data, database = _load_country_data(country_code)
     if country_code:
         country_area = address["country_area"]
         if country_area:
-            key = "%s/%s" % (country_code, country_area)
+            key = f"{country_code}/{country_area}"
             country_area_data = database.get(key)
             if country_area_data:
                 cleaned_data["country_area"] = country_area_data.get(
                     "lname", country_area_data.get("name", country_area)
                 )
                 city = address["city"]
-                key = "%s/%s/%s" % (country_code, country_area, city)
+                key = f"{country_code}/{country_area}/{city}"
                 city_data = database.get(key)
                 if city_data:
                     cleaned_data["city"] = city_data.get(
                         "lname", city_data.get("name", city)
                     )
                     city_area = address["city_area"]
-                    key = "%s/%s/%s/%s" % (country_code, country_area, city, city_area)
+                    key = f"{country_code}/{country_area}/{city}/{city_area}"
                     city_area_data = database.get(key)
                     if city_area_data:
                         cleaned_data["city_area"] = city_area_data.get(
                             "lname", city_area_data.get("name", city_area)
                         )
     return cleaned_data
```

### Comparing `google-i18n-address-2.5.2/i18naddress/data/ad.json` & `google_i18n_address-3.0.0/i18naddress/data/ad.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/ae.json` & `google_i18n_address-3.0.0/i18naddress/data/ae.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/all.json` & `google_i18n_address-3.0.0/i18naddress/data/all.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9964948274980572%*

 * *Differences: {"'BH'": "{'zip': '(?:^|\\\\b)(?:1[0-2]|[1-9])\\\\d{2}(?:$|\\\\b)'}",*

 * * "'CL'": "{'sub_mores': "*

 * *         "'true~true~true~true~true~true~true~true~true~true~true~true~true~true~true~true'}",*

 * * "'CL/Ñuble'": "{'sub_keys': 'Bulnes~Chillán~Coelemu~Coihueco~Quillón~Quirihue~San Carlos~Yungay'}",*

 * * "'CL/Ñuble/Bulnes'": "OrderedDict([('id', 'data/CL/Ñuble/Bulnes'), ('key', 'Bulnes'), ('lang', "*

 * *                      "'es')])",*

 * * "'CL/Ñuble/Chillán'": "OrderedDict([('id', 'data/CL/Ñuble/Chillán'), ('key', 'Chillán'), […]*

```diff
@@ -720,15 +720,15 @@
         "zipex": "1000,1700"
     },
     "BH": {
         "fmt": "%N%n%O%n%A%n%C %Z",
         "id": "data/BH",
         "key": "BH",
         "name": "BAHRAIN",
-        "zip": "(?:\\d|1[0-2])\\d{2}",
+        "zip": "(?:^|\\b)(?:1[0-2]|[1-9])\\d{2}(?:$|\\b)",
         "zipex": "317"
     },
     "BI": {
         "id": "data/BI",
         "key": "BI",
         "name": "BURUNDI"
     },
@@ -29380,15 +29380,15 @@
         "key": "CL",
         "lang": "es",
         "languages": "es",
         "name": "CHILE",
         "posturl": "https://www.correos.cl/web/guest/codigo-postal",
         "sub_isoids": "AN~AR~AP~AT~AI~BI~CO~LI~LL~LR~MA~ML~RM~NB~TA~VS",
         "sub_keys": "Antofagasta~Araucan\u00eda~Arica y Parinacota~Atacama~Ays\u00e9n~Biob\u00edo~Coquimbo~O'Higgins~Los Lagos~Los R\u00edos~Magallanes~Maule~Regi\u00f3n Metropolitana~\u00d1uble~Tarapac\u00e1~Valpara\u00edso",
-        "sub_mores": "true~true~true~true~true~true~true~true~true~true~true~true~true~false~true~true",
+        "sub_mores": "true~true~true~true~true~true~true~true~true~true~true~true~true~true~true~true",
         "sub_names": "Antofagasta~Araucan\u00eda~Arica y Parinacota~Atacama~Ays\u00e9n del General Carlos Ib\u00e1\u00f1ez del Campo~Biob\u00edo~Coquimbo~Libertador General Bernardo O'Higgins~Los Lagos~Los R\u00edos~Magallanes y de la Ant\u00e1rtica Chilena~Maule~Metropolitana de Santiago~\u00d1uble~Tarapac\u00e1~Valpara\u00edso",
         "zip": "\\d{7}",
         "zipex": "8340457,8720019,1230000,8329100"
     },
     "CL/Antofagasta": {
         "id": "data/CL/Antofagasta",
         "isoid": "AN",
@@ -31240,15 +31240,56 @@
         "lang": "es"
     },
     "CL/\u00d1uble": {
         "id": "data/CL/\u00d1uble",
         "isoid": "NB",
         "key": "\u00d1uble",
         "lang": "es",
-        "name": "\u00d1uble"
+        "name": "\u00d1uble",
+        "sub_keys": "Bulnes~Chill\u00e1n~Coelemu~Coihueco~Quill\u00f3n~Quirihue~San Carlos~Yungay"
+    },
+    "CL/\u00d1uble/Bulnes": {
+        "id": "data/CL/\u00d1uble/Bulnes",
+        "key": "Bulnes",
+        "lang": "es"
+    },
+    "CL/\u00d1uble/Chill\u00e1n": {
+        "id": "data/CL/\u00d1uble/Chill\u00e1n",
+        "key": "Chill\u00e1n",
+        "lang": "es"
+    },
+    "CL/\u00d1uble/Coelemu": {
+        "id": "data/CL/\u00d1uble/Coelemu",
+        "key": "Coelemu",
+        "lang": "es"
+    },
+    "CL/\u00d1uble/Coihueco": {
+        "id": "data/CL/\u00d1uble/Coihueco",
+        "key": "Coihueco",
+        "lang": "es"
+    },
+    "CL/\u00d1uble/Quill\u00f3n": {
+        "id": "data/CL/\u00d1uble/Quill\u00f3n",
+        "key": "Quill\u00f3n",
+        "lang": "es"
+    },
+    "CL/\u00d1uble/Quirihue": {
+        "id": "data/CL/\u00d1uble/Quirihue",
+        "key": "Quirihue",
+        "lang": "es"
+    },
+    "CL/\u00d1uble/San Carlos": {
+        "id": "data/CL/\u00d1uble/San Carlos",
+        "key": "San Carlos",
+        "lang": "es"
+    },
+    "CL/\u00d1uble/Yungay": {
+        "id": "data/CL/\u00d1uble/Yungay",
+        "key": "Yungay",
+        "lang": "es"
     },
     "CM": {
         "id": "data/CM",
         "key": "CM",
         "name": "CAMEROON"
     },
     "CN": {
@@ -43963,20 +44004,28 @@
     },
     "CN/\u5e7f\u4e1c\u7701/\u6df1\u5733\u5e02": {
         "id": "data/CN/\u5e7f\u4e1c\u7701/\u6df1\u5733\u5e02",
         "key": "\u6df1\u5733\u5e02",
         "lang": "zh",
         "lname": "Shenzhen Shi",
         "name": "\u6df1\u5733\u5e02",
-        "sub_keys": "\u5b9d\u5b89\u533a~\u798f\u7530\u533a~\u9f99\u5c97\u533a~\u9f99\u534e\u533a~\u7f57\u6e56\u533a~\u5357\u5c71\u533a~\u576a\u5c71\u65b0\u533a~\u76d0\u7530\u533a",
-        "sub_lnames": "Bao'an Qu~Futian Qu~Longgang Qu~Longhua Qu~Luohu Qu~Nanshan Qu~Pingshan Qu~Yantian Qu",
-        "sub_names": "\u5b9d\u5b89\u533a~\u798f\u7530\u533a~\u9f99\u5c97\u533a~\u9f99\u534e\u533a~\u7f57\u6e56\u533a~\u5357\u5c71\u533a~\u576a\u5c71\u65b0\u533a~\u76d0\u7530\u533a",
-        "sub_zipexs": "518101~518033~518116~518110~518001~518052~518118~518083",
+        "sub_keys": "\u5b9d\u5b89\u533a~\u798f\u7530\u533a~\u5149\u660e\u533a~\u9f99\u5c97\u533a~\u9f99\u534e\u533a~\u7f57\u6e56\u533a~\u5357\u5c71\u533a~\u576a\u5c71\u65b0\u533a~\u76d0\u7530\u533a",
+        "sub_lnames": "Bao'an Qu~Futian Qu~Guangming Qu~Longgang Qu~Longhua Qu~Luohu Qu~Nanshan Qu~Pingshan Qu~Yantian Qu",
+        "sub_names": "\u5b9d\u5b89\u533a~\u798f\u7530\u533a~\u5149\u660e\u533a~\u9f99\u5c97\u533a~\u9f99\u534e\u533a~\u7f57\u6e56\u533a~\u5357\u5c71\u533a~\u576a\u5c71\u65b0\u533a~\u76d0\u7530\u533a",
+        "sub_zipexs": "518101~518033~518107~518116~518110~518001~518052~518118~518083",
         "zipex": "518027"
     },
+    "CN/\u5e7f\u4e1c\u7701/\u6df1\u5733\u5e02/\u5149\u660e\u533a": {
+        "id": "data/CN/\u5e7f\u4e1c\u7701/\u6df1\u5733\u5e02/\u5149\u660e\u533a",
+        "key": "\u5149\u660e\u533a",
+        "lang": "zh",
+        "lname": "Guangming Qu",
+        "name": "\u5149\u660e\u533a",
+        "zipex": "518107"
+    },
     "CN/\u5e7f\u4e1c\u7701/\u6df1\u5733\u5e02/\u5357\u5c71\u533a": {
         "id": "data/CN/\u5e7f\u4e1c\u7701/\u6df1\u5733\u5e02/\u5357\u5c71\u533a",
         "key": "\u5357\u5c71\u533a",
         "lang": "zh",
         "lname": "Nanshan Qu",
         "name": "\u5357\u5c71\u533a",
         "zipex": "518052"
@@ -62108,24 +62157,226 @@
         "key": "\u9f99\u6c99\u533a",
         "lang": "zh",
         "lname": "Longsha Qu",
         "name": "\u9f99\u6c99\u533a",
         "zipex": "161000"
     },
     "CO": {
-        "fmt": "%N%n%O%n%A%n%C, %S, %Z",
+        "fmt": "%N%n%O%n%A%n%D%n%C, %S, %Z",
         "id": "data/CO",
         "key": "CO",
+        "lang": "es",
+        "languages": "es",
         "name": "COLOMBIA",
         "posturl": "http://www.codigopostal.gov.co/",
         "require": "AS",
         "state_name_type": "department",
+        "sub_isoids": "AMA~ANT~ARA~ATL~DC~BOL~BOY~CAL~CAQ~CAS~CAU~CES~CHO~COR~CUN~GUA~GUV~HUI~LAG~MAG~MET~NAR~NSA~PUT~QUI~RIS~SAP~SAN~SUC~TOL~VAC~VAU~VID",
+        "sub_keys": "Amazonas~Antioquia~Arauca~Atl\u00e1ntico~Bogot\u00e1~Bol\u00edvar~Boyac\u00e1~Caldas~Caquet\u00e1~Casanare~Cauca~Cesar~Choc\u00f3~C\u00f3rdoba~Cundinamarca~Guain\u00eda~Guaviare~Huila~La Guajira~Magdalena~Meta~Nari\u00f1o~Norte de Santander~Putumayo~Quind\u00edo~Risaralda~San Andr\u00e9s y Providencia~Santander~Sucre~Tolima~Valle del Cauca~Vaup\u00e9s~Vichada",
         "zip": "\\d{6}",
         "zipex": "111221,130001,760011"
     },
+    "CO/Amazonas": {
+        "id": "data/CO/Amazonas",
+        "isoid": "AMA",
+        "key": "Amazonas",
+        "lang": "es"
+    },
+    "CO/Antioquia": {
+        "id": "data/CO/Antioquia",
+        "isoid": "ANT",
+        "key": "Antioquia",
+        "lang": "es"
+    },
+    "CO/Arauca": {
+        "id": "data/CO/Arauca",
+        "isoid": "ARA",
+        "key": "Arauca",
+        "lang": "es"
+    },
+    "CO/Atl\u00e1ntico": {
+        "id": "data/CO/Atl\u00e1ntico",
+        "isoid": "ATL",
+        "key": "Atl\u00e1ntico",
+        "lang": "es"
+    },
+    "CO/Bogot\u00e1": {
+        "id": "data/CO/Bogot\u00e1",
+        "isoid": "DC",
+        "key": "Bogot\u00e1",
+        "lang": "es"
+    },
+    "CO/Bol\u00edvar": {
+        "id": "data/CO/Bol\u00edvar",
+        "isoid": "BOL",
+        "key": "Bol\u00edvar",
+        "lang": "es"
+    },
+    "CO/Boyac\u00e1": {
+        "id": "data/CO/Boyac\u00e1",
+        "isoid": "BOY",
+        "key": "Boyac\u00e1",
+        "lang": "es"
+    },
+    "CO/Caldas": {
+        "id": "data/CO/Caldas",
+        "isoid": "CAL",
+        "key": "Caldas",
+        "lang": "es"
+    },
+    "CO/Caquet\u00e1": {
+        "id": "data/CO/Caquet\u00e1",
+        "isoid": "CAQ",
+        "key": "Caquet\u00e1",
+        "lang": "es"
+    },
+    "CO/Casanare": {
+        "id": "data/CO/Casanare",
+        "isoid": "CAS",
+        "key": "Casanare",
+        "lang": "es"
+    },
+    "CO/Cauca": {
+        "id": "data/CO/Cauca",
+        "isoid": "CAU",
+        "key": "Cauca",
+        "lang": "es"
+    },
+    "CO/Cesar": {
+        "id": "data/CO/Cesar",
+        "isoid": "CES",
+        "key": "Cesar",
+        "lang": "es"
+    },
+    "CO/Choc\u00f3": {
+        "id": "data/CO/Choc\u00f3",
+        "isoid": "CHO",
+        "key": "Choc\u00f3",
+        "lang": "es"
+    },
+    "CO/Cundinamarca": {
+        "id": "data/CO/Cundinamarca",
+        "isoid": "CUN",
+        "key": "Cundinamarca",
+        "lang": "es"
+    },
+    "CO/C\u00f3rdoba": {
+        "id": "data/CO/C\u00f3rdoba",
+        "isoid": "COR",
+        "key": "C\u00f3rdoba",
+        "lang": "es"
+    },
+    "CO/Guain\u00eda": {
+        "id": "data/CO/Guain\u00eda",
+        "isoid": "GUA",
+        "key": "Guain\u00eda",
+        "lang": "es"
+    },
+    "CO/Guaviare": {
+        "id": "data/CO/Guaviare",
+        "isoid": "GUV",
+        "key": "Guaviare",
+        "lang": "es"
+    },
+    "CO/Huila": {
+        "id": "data/CO/Huila",
+        "isoid": "HUI",
+        "key": "Huila",
+        "lang": "es"
+    },
+    "CO/La Guajira": {
+        "id": "data/CO/La Guajira",
+        "isoid": "LAG",
+        "key": "La Guajira",
+        "lang": "es"
+    },
+    "CO/Magdalena": {
+        "id": "data/CO/Magdalena",
+        "isoid": "MAG",
+        "key": "Magdalena",
+        "lang": "es"
+    },
+    "CO/Meta": {
+        "id": "data/CO/Meta",
+        "isoid": "MET",
+        "key": "Meta",
+        "lang": "es"
+    },
+    "CO/Nari\u00f1o": {
+        "id": "data/CO/Nari\u00f1o",
+        "isoid": "NAR",
+        "key": "Nari\u00f1o",
+        "lang": "es"
+    },
+    "CO/Norte de Santander": {
+        "id": "data/CO/Norte de Santander",
+        "isoid": "NSA",
+        "key": "Norte de Santander",
+        "lang": "es"
+    },
+    "CO/Putumayo": {
+        "id": "data/CO/Putumayo",
+        "isoid": "PUT",
+        "key": "Putumayo",
+        "lang": "es"
+    },
+    "CO/Quind\u00edo": {
+        "id": "data/CO/Quind\u00edo",
+        "isoid": "QUI",
+        "key": "Quind\u00edo",
+        "lang": "es"
+    },
+    "CO/Risaralda": {
+        "id": "data/CO/Risaralda",
+        "isoid": "RIS",
+        "key": "Risaralda",
+        "lang": "es"
+    },
+    "CO/San Andr\u00e9s y Providencia": {
+        "id": "data/CO/San Andr\u00e9s y Providencia",
+        "isoid": "SAP",
+        "key": "San Andr\u00e9s y Providencia",
+        "lang": "es"
+    },
+    "CO/Santander": {
+        "id": "data/CO/Santander",
+        "isoid": "SAN",
+        "key": "Santander",
+        "lang": "es"
+    },
+    "CO/Sucre": {
+        "id": "data/CO/Sucre",
+        "isoid": "SUC",
+        "key": "Sucre",
+        "lang": "es"
+    },
+    "CO/Tolima": {
+        "id": "data/CO/Tolima",
+        "isoid": "TOL",
+        "key": "Tolima",
+        "lang": "es"
+    },
+    "CO/Valle del Cauca": {
+        "id": "data/CO/Valle del Cauca",
+        "isoid": "VAC",
+        "key": "Valle del Cauca",
+        "lang": "es"
+    },
+    "CO/Vaup\u00e9s": {
+        "id": "data/CO/Vaup\u00e9s",
+        "isoid": "VAU",
+        "key": "Vaup\u00e9s",
+        "lang": "es"
+    },
+    "CO/Vichada": {
+        "id": "data/CO/Vichada",
+        "isoid": "VID",
+        "key": "Vichada",
+        "lang": "es"
+    },
     "CR": {
         "fmt": "%N%n%O%n%A%n%S, %C%n%Z",
         "id": "data/CR",
         "key": "CR",
         "name": "COSTA RICA",
         "posturl": "https://correos.go.cr/codigo-postal/",
         "require": "ACS",
@@ -62389,15 +62640,15 @@
         "name": "ECUADOR",
         "posturl": "http://www.codigopostal.gob.ec/",
         "upper": "CZ",
         "zip": "\\d{6}",
         "zipex": "090105,092301"
     },
     "EE": {
-        "fmt": "%N%n%O%n%A%n%Z %C",
+        "fmt": "%N%n%O%n%A%n%Z %C %S",
         "id": "data/EE",
         "key": "EE",
         "name": "ESTONIA",
         "posturl": "https://www.omniva.ee/era/sihtnumbrite_otsing",
         "require": "ACZ",
         "zip": "\\d{5}",
         "zipex": "69501,11212"
@@ -62681,60 +62932,60 @@
         "lang": "es",
         "languages": "es~ca~gl~eu",
         "name": "SPAIN",
         "posturl": "http://www.correos.es/contenido/13-MenuRec2/04-MenuRec24/1010_s-CodPostal.asp",
         "require": "ACSZ",
         "sub_keys": "VI~AB~A~AL~O~AV~BA~B~BU~CC~CA~S~CS~CE~CR~CO~CU~GI~GR~GU~SS~H~HU~PM~J~C~LO~GC~LE~L~LU~M~MA~ML~MU~NA~OR~P~PO~SA~TF~SG~SE~SO~T~TE~TO~V~VA~BI~ZA~Z",
         "sub_names": "\u00c1lava~Albacete~Alicante~Almer\u00eda~Asturias~\u00c1vila~Badajoz~Barcelona~Burgos~C\u00e1ceres~C\u00e1diz~Cantabria~Castell\u00f3n~Ceuta~Ciudad Real~C\u00f3rdoba~Cuenca~Girona~Granada~Guadalajara~Guip\u00fazcoa~Huelva~Huesca~Islas Baleares~Ja\u00e9n~La Coru\u00f1a~La Rioja~Las Palmas~Le\u00f3n~L\u00e9rida~Lugo~Madrid~M\u00e1laga~Melilla~Murcia~Navarra~Ourense~Palencia~Pontevedra~Salamanca~Santa Cruz de Tenerife~Segovia~Sevilla~Soria~Tarragona~Teruel~Toledo~Valencia~Valladolid~Vizcaya~Zamora~Zaragoza",
-        "sub_zips": "01~02~03~04~33~05~06~08~09~10~11~39~12~51~13~14~16~17~18~19~20~21~22~07~23~15~26(?!.*127)~35~24~25~27~28~29~52~30~31~32~34~36~37~38~40~41~26127|42~43~44~45~46~47~48~49~50",
+        "sub_zips": "01~02~03~04~33~05~06~08~09~10~11~39~12~51~13~14~16~17~18~19~20~21~22~07~23~15~26~35~24~25~27~28~29~52~30~31~32~34~36~37~38~40~41~26127|42~43~44~45~46~47~48~49~50",
         "upper": "CS",
         "zip": "\\d{5}",
         "zipex": "28039,28300,28070"
     },
     "ES--ca": {
         "fmt": "%N%n%O%n%A%n%Z %C %S",
         "id": "data/ES--ca",
         "key": "ES",
         "lang": "ca",
         "name": "SPAIN",
         "posturl": "http://www.correos.es/contenido/13-MenuRec2/04-MenuRec24/1010_s-CodPostal.asp",
         "require": "ACSZ",
         "sub_keys": "A~AB~AL~VI~O~AV~BA~B~BI~BU~CC~CA~S~CS~CE~CR~CO~CU~GI~GR~GU~SS~H~HU~PM~J~C~LO~GC~LE~L~LU~M~MA~ML~MU~NA~OR~P~PO~SA~TF~SG~SE~SO~T~TE~TO~V~VA~ZA~Z",
         "sub_names": "Alacant~Albacete~Almeria~Araba~Asturias~\u00c0vila~Badajoz~Barcelona~Bizkaia~Burgos~C\u00e1ceres~Cadis~Cantabria~Castell\u00f3~Ceuta~Ciudad Real~C\u00f3rdoba~Cuenca~Girona~Granada~Guadalajara~Guip\u00fascoa~Huelva~Huesca~Illes Balears~Ja\u00e9n~La Corunya~La Rioja~Las Palmas~Le\u00f3n~Lleida~Lugo~Madrid~M\u00e1laga~Melilla~Murcia~Navarra~Ourense~Palencia~Pontevedra~Salamanca~Santa Cruz de Tenerife~Segovia~Sevilla~Soria~Tarragona~Teruel~Toledo~Val\u00e8ncia~Valladolid~Zamora~Zaragoza",
-        "sub_zips": "03~02~04~01~33~05~06~08~48~09~10~11~39~12~51~13~14~16~17~18~19~20~21~22~07~23~15~26(?!.*127)~35~24~25~27~28~29~52~30~31~32~34~36~37~38~40~41~26127|42~43~44~45~46~47~49~50",
+        "sub_zips": "03~02~04~01~33~05~06~08~48~09~10~11~39~12~51~13~14~16~17~18~19~20~21~22~07~23~15~26~35~24~25~27~28~29~52~30~31~32~34~36~37~38~40~41~26127|42~43~44~45~46~47~49~50",
         "upper": "CS",
         "zip": "\\d{5}",
         "zipex": "28039,28300,28070"
     },
     "ES--eu": {
         "fmt": "%N%n%O%n%A%n%Z %C %S",
         "id": "data/ES--eu",
         "key": "ES",
         "lang": "eu",
         "name": "SPAIN",
         "posturl": "http://www.correos.es/contenido/13-MenuRec2/04-MenuRec24/1010_s-CodPostal.asp",
         "require": "ACSZ",
         "sub_keys": "A~AB~AL~VI~O~AV~BA~B~BI~BU~CC~CA~S~CS~CE~CR~C~CU~SS~GI~GR~GU~H~HU~PM~J~CO~LO~GC~LE~L~LU~M~MA~ML~MU~NA~OR~P~PO~SA~TF~SG~SE~SO~T~TE~TO~V~VA~ZA~Z",
         "sub_names": "Alacant~Albacete~Almer\u00eda~Araba~Asturias~\u00c1vila~Badajoz~Barcelona~Bizkaia~Burgos~C\u00e1ceres~C\u00e1diz~Cantabria~Castell\u00f3~Ceuta~Ciudad Real~Coru\u00f1a~Cuenca~Gipuzkoa~Girona~Granada~Guadalajara~Huelva~Huesca~Illes Balears~Ja\u00e9n~Kordoba~La Rioja~Las Palmas~Le\u00f3n~Lleida~Lugo~Madrid~M\u00e1laga~Melilla~Murtzia~Nafarroa~Ourense~Palentzia~Pontevedra~Salamanca~Santa Cruz Tenerifekoa~Segovia~Sevilla~Soria~Tarragona~Teruel~Toledo~Valentzia~Valladolid~Zamora~Zaragoza",
-        "sub_zips": "03~02~04~01~33~05~06~08~48~09~10~11~39~12~51~13~15~16~20~17~18~19~21~22~07~23~14~26(?!.*127)~35~24~25~27~28~29~52~30~31~32~34~36~37~38~40~41~26127|42~43~44~45~46~47~49~50",
+        "sub_zips": "03~02~04~01~33~05~06~08~48~09~10~11~39~12~51~13~15~16~20~17~18~19~21~22~07~23~14~26~35~24~25~27~28~29~52~30~31~32~34~36~37~38~40~41~26127|42~43~44~45~46~47~49~50",
         "upper": "CS",
         "zip": "\\d{5}",
         "zipex": "28039,28300,28070"
     },
     "ES--gl": {
         "fmt": "%N%n%O%n%A%n%Z %C %S",
         "id": "data/ES--gl",
         "key": "ES",
         "lang": "gl",
         "name": "SPAIN",
         "posturl": "http://www.correos.es/contenido/13-MenuRec2/04-MenuRec24/1010_s-CodPostal.asp",
         "require": "ACSZ",
         "sub_keys": "C~A~VI~AB~AL~GC~O~AV~BA~B~BI~BU~CC~CA~S~CS~CE~CR~CO~CU~GR~GU~SS~H~HU~PM~LO~LE~L~LU~M~MA~ML~MU~NA~OR~P~PO~SA~TF~SG~SE~SO~T~TE~TO~V~VA~J~GI~ZA~Z",
         "sub_names": "A Coru\u00f1a~Alacant~\u00c1lava~Albacete~Almer\u00eda~As Palmas~Asturias~\u00c1vila~Badaxoz~Barcelona~Biscaia~Burgos~C\u00e1ceres~C\u00e1diz~Cantabria~Castell\u00f3~Ceuta~Cidade Real~C\u00f3rdoba~Cuenca~Granada~Guadalajara~Guip\u00fascoa~Huelva~Huesca~Illas Baleares~La Rioja~Le\u00f3n~Lleida~Lugo~Madrid~M\u00e1laga~Melilla~Murcia~Navarra~Ourense~Palencia~Pontevedra~Salamanca~Santa Cruz de Tenerife~Segovia~Sevilla~Soria~Tarragona~Teruel~Toledo~Valencia~Valladolid~Xa\u00e9n~Xirona~Zamora~Zaragoza",
-        "sub_zips": "15~03~01~02~04~35~33~05~06~08~48~09~10~11~39~12~51~13~14~16~18~19~20~21~22~07~26(?!.*127)~24~25~27~28~29~52~30~31~32~34~36~37~38~40~41~26127|42~43~44~45~46~47~23~17~49~50",
+        "sub_zips": "15~03~01~02~04~35~33~05~06~08~48~09~10~11~39~12~51~13~14~16~18~19~20~21~22~07~26~24~25~27~28~29~52~30~31~32~34~36~37~38~40~41~26127|42~43~44~45~46~47~23~17~49~50",
         "upper": "CS",
         "zip": "\\d{5}",
         "zipex": "28039,28300,28070"
     },
     "ES/A": {
         "id": "data/ES/A",
         "key": "A",
@@ -63436,36 +63687,36 @@
         "zip": "24"
     },
     "ES/LO": {
         "id": "data/ES/LO",
         "key": "LO",
         "lang": "es",
         "name": "La Rioja",
-        "zip": "26(?!.*127)"
+        "zip": "26"
     },
     "ES/LO--ca": {
         "id": "data/ES/LO--ca",
         "key": "LO",
         "lang": "ca",
         "name": "La Rioja",
-        "zip": "26(?!.*127)"
+        "zip": "26"
     },
     "ES/LO--eu": {
         "id": "data/ES/LO--eu",
         "key": "LO",
         "lang": "eu",
         "name": "La Rioja",
-        "zip": "26(?!.*127)"
+        "zip": "26"
     },
     "ES/LO--gl": {
         "id": "data/ES/LO--gl",
         "key": "LO",
         "lang": "gl",
         "name": "La Rioja",
-        "zip": "26(?!.*127)"
+        "zip": "26"
     },
     "ES/LU": {
         "id": "data/ES/LU",
         "key": "LU",
         "lang": "es",
         "name": "Lugo",
         "zip": "27"
@@ -70470,15 +70721,15 @@
         "isoid": "28",
         "key": "\uc778\ucc9c\uad11\uc5ed\uc2dc",
         "lang": "ko",
         "lname": "Incheon",
         "name": "\uc778\ucc9c",
         "sub_keys": "\uac15\ud654\uad70~\uacc4\uc591\uad6c~\ub0a8\uad6c~\ub0a8\ub3d9\uad6c~\ub3d9\uad6c~\ubd80\ud3c9\uad6c~\uc11c\uad6c~\uc5f0\uc218\uad6c~\uc639\uc9c4\uad70~\uc911\uad6c",
         "sub_lnames": "Ganghwa-gun~Gyeyang-gu~Nam-gu~Namdong-gu~Dong-gu~Bupyeong-gu~Seo-gu~Yeonsu-gu~Ongjin-gun~Jung-gu",
-        "sub_zips": "230~21[01]~22[12]~21[5-7]~225~21[34]~22[6-8]~2(?:19|20)~231~223",
+        "sub_zips": "230~21[01]~22[12]~21[5-7]~225~21[34]~22[6-8]~2(?:19|20)~231~22[34]",
         "zip": "2[1-3]\\d{2}",
         "zipex": "23024"
     },
     "KR/\uc778\ucc9c\uad11\uc5ed\uc2dc/\uac15\ud654\uad70": {
         "id": "data/KR/\uc778\ucc9c\uad11\uc5ed\uc2dc/\uac15\ud654\uad70",
         "key": "\uac15\ud654\uad70",
         "lang": "ko",
@@ -70542,15 +70793,15 @@
         "zip": "231"
     },
     "KR/\uc778\ucc9c\uad11\uc5ed\uc2dc/\uc911\uad6c": {
         "id": "data/KR/\uc778\ucc9c\uad11\uc5ed\uc2dc/\uc911\uad6c",
         "key": "\uc911\uad6c",
         "lang": "ko",
         "lname": "Jung-gu",
-        "zip": "223"
+        "zip": "22[34]"
     },
     "KR/\uc804\ub77c\ub0a8\ub3c4": {
         "id": "data/KR/\uc804\ub77c\ub0a8\ub3c4",
         "isoid": "46",
         "key": "\uc804\ub77c\ub0a8\ub3c4",
         "lang": "ko",
         "lname": "Jeollanam-do",
@@ -71228,15 +71479,15 @@
         "id": "data/LS",
         "key": "LS",
         "name": "LESOTHO",
         "zip": "\\d{3}",
         "zipex": "100"
     },
     "LT": {
-        "fmt": "%O%n%N%n%A%nLT-%Z %C",
+        "fmt": "%O%n%N%n%A%nLT-%Z %C %S",
         "id": "data/LT",
         "key": "LT",
         "name": "LITHUANIA",
         "postprefix": "LT-",
         "posturl": "http://www.post.lt/lt/?id=316",
         "require": "ACZ",
         "zip": "\\d{5}",
@@ -71250,15 +71501,15 @@
         "postprefix": "L-",
         "posturl": "https://www.post.lu/fr/grandes-entreprises/solutions-postales/rechercher-un-code-postal",
         "require": "ACZ",
         "zip": "\\d{4}",
         "zipex": "4750,2998"
     },
     "LV": {
-        "fmt": "%N%n%O%n%A%n%C, %Z",
+        "fmt": "%N%n%O%n%A%n%S%n%C, %Z",
         "id": "data/LV",
         "key": "LV",
         "name": "LATVIA",
         "posturl": "http://www.pasts.lv/lv/uzzinas/nodalas/",
         "require": "ACZ",
         "zip": "LV-\\d{4}",
         "zipex": "LV-1073,LV-1000"
@@ -72385,15 +72636,15 @@
     "NL": {
         "fmt": "%O%n%N%n%A%n%Z %C",
         "id": "data/NL",
         "key": "NL",
         "name": "NETHERLANDS",
         "posturl": "http://www.postnl.nl/voorthuis/",
         "require": "ACZ",
-        "zip": "\\d{4} ?[A-Z]{2}",
+        "zip": "[1-9]\\d{3} ?(?:[A-RT-Z][A-Z]|S[BCE-RT-Z])",
         "zipex": "1234 AB,2490 AA"
     },
     "NO": {
         "fmt": "%N%n%O%n%A%n%Z %C",
         "id": "data/NO",
         "key": "NO",
         "locality_name_type": "post_town",
@@ -73394,15 +73645,15 @@
         "isoid": "ZAS",
         "key": "Zamboanga del Sur",
         "lang": "en",
         "zip": "70[0-4]",
         "zipex": "7000,7043"
     },
     "PK": {
-        "fmt": "%N%n%O%n%A%n%C-%Z",
+        "fmt": "%N%n%O%n%A%n%D%n%C-%Z",
         "id": "data/PK",
         "key": "PK",
         "name": "PAKISTAN",
         "posturl": "http://www.pakpost.gov.pk/postcode.php",
         "zip": "\\d{5}",
         "zipex": "44000"
     },
@@ -73499,15 +73750,15 @@
         "posturl": "http://www.laposte.fr/Particulier/Utiliser-nos-outils-pratiques/Outils-et-documents/Trouvez-un-code-postal",
         "require": "ACZ",
         "upper": "ACX",
         "zip": "9[78]4\\d{2}",
         "zipex": "97400"
     },
     "RO": {
-        "fmt": "%N%n%O%n%A%n%Z %C",
+        "fmt": "%N%n%O%n%A%n%Z %S %C",
         "id": "data/RO",
         "key": "RO",
         "name": "ROMANIA",
         "posturl": "http://www.posta-romana.ro/zip_codes",
         "require": "ACZ",
         "upper": "AC",
         "zip": "\\d{6}",
@@ -76172,14 +76423,15 @@
     "TW": {
         "fmt": "%Z%n%S%C%n%A%n%O%n%N",
         "id": "data/TW",
         "key": "TW",
         "lang": "zh-Hant",
         "languages": "zh-Hant",
         "lfmt": "%N%n%O%n%A%n%C, %S %Z",
+        "locality_name_type": "district",
         "name": "TAIWAN",
         "posturl": "http://www.post.gov.tw/post/internet/f_searchzone/index.jsp?ID=190102",
         "require": "ACSZ",
         "state_name_type": "county",
         "sub_isoids": "TXG~TPE~TTT~TNN~ILA~HUA~~NAN~PIF~MIA~TAO~KHH~KEE~~YUN~NWT~HSZ~HSQ~CYI~CYQ~CHA~PEN",
         "sub_keys": "\u53f0\u4e2d\u5e02~\u53f0\u5317\u5e02~\u53f0\u6771\u7e23~\u53f0\u5357\u5e02~\u5b9c\u862d\u7e23~\u82b1\u84ee\u7e23~\u91d1\u9580\u7e23~\u5357\u6295\u7e23~\u5c4f\u6771\u7e23~\u82d7\u6817\u7e23~\u6843\u5712\u5e02~\u9ad8\u96c4\u5e02~\u57fa\u9686\u5e02~\u9023\u6c5f\u7e23~\u96f2\u6797\u7e23~\u65b0\u5317\u5e02~\u65b0\u7af9\u5e02~\u65b0\u7af9\u7e23~\u5609\u7fa9\u5e02~\u5609\u7fa9\u7e23~\u5f70\u5316\u7e23~\u6f8e\u6e56\u7e23",
         "sub_lnames": "Taichung City~Taipei City~Taitung County~Tainan City~Yilan County~Hualien County~Kinmen County~Nantou County~Pingtung County~Miaoli County~Taoyuan City~Kaohsiung City~Keelung City~Lienchiang County~Yunlin County~New Taipei City~Hsinchu City~Hsinchu County~Chiayi City~Chiayi County~Changhua County~Penghu County",
```

### Comparing `google-i18n-address-2.5.2/i18naddress/data/am.json` & `google_i18n_address-3.0.0/i18naddress/data/am.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/ar.json` & `google_i18n_address-3.0.0/i18naddress/data/ar.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/au.json` & `google_i18n_address-3.0.0/i18naddress/data/au.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/br.json` & `google_i18n_address-3.0.0/i18naddress/data/br.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/bs.json` & `google_i18n_address-3.0.0/i18naddress/data/bs.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/ca.json` & `google_i18n_address-3.0.0/i18naddress/data/ca.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/cl.json` & `google_i18n_address-3.0.0/i18naddress/data/cl.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.978160204575299%*

 * *Differences: {"'CL'": "{'sub_mores': "*

 * *         "'true~true~true~true~true~true~true~true~true~true~true~true~true~true~true~true'}",*

 * * "'CL/Ñuble'": "{'sub_keys': 'Bulnes~Chillán~Coelemu~Coihueco~Quillón~Quirihue~San Carlos~Yungay'}",*

 * * "'CL/Ñuble/Bulnes'": "OrderedDict([('id', 'data/CL/Ñuble/Bulnes'), ('key', 'Bulnes'), ('lang', "*

 * *                      "'es')])",*

 * * "'CL/Ñuble/Chillán'": "OrderedDict([('id', 'data/CL/Ñuble/Chillán'), ('key', 'Chillán'), ('lang', "*

 * *                       "'es')])",*

 * * "'CL/Ñuble/Coelemu'": " […]*

```diff
@@ -5,15 +5,15 @@
         "key": "CL",
         "lang": "es",
         "languages": "es",
         "name": "CHILE",
         "posturl": "https://www.correos.cl/web/guest/codigo-postal",
         "sub_isoids": "AN~AR~AP~AT~AI~BI~CO~LI~LL~LR~MA~ML~RM~NB~TA~VS",
         "sub_keys": "Antofagasta~Araucan\u00eda~Arica y Parinacota~Atacama~Ays\u00e9n~Biob\u00edo~Coquimbo~O'Higgins~Los Lagos~Los R\u00edos~Magallanes~Maule~Regi\u00f3n Metropolitana~\u00d1uble~Tarapac\u00e1~Valpara\u00edso",
-        "sub_mores": "true~true~true~true~true~true~true~true~true~true~true~true~true~false~true~true",
+        "sub_mores": "true~true~true~true~true~true~true~true~true~true~true~true~true~true~true~true",
         "sub_names": "Antofagasta~Araucan\u00eda~Arica y Parinacota~Atacama~Ays\u00e9n del General Carlos Ib\u00e1\u00f1ez del Campo~Biob\u00edo~Coquimbo~Libertador General Bernardo O'Higgins~Los Lagos~Los R\u00edos~Magallanes y de la Ant\u00e1rtica Chilena~Maule~Metropolitana de Santiago~\u00d1uble~Tarapac\u00e1~Valpara\u00edso",
         "zip": "\\d{7}",
         "zipex": "8340457,8720019,1230000,8329100"
     },
     "CL/Antofagasta": {
         "id": "data/CL/Antofagasta",
         "isoid": "AN",
@@ -1865,10 +1865,51 @@
         "lang": "es"
     },
     "CL/\u00d1uble": {
         "id": "data/CL/\u00d1uble",
         "isoid": "NB",
         "key": "\u00d1uble",
         "lang": "es",
-        "name": "\u00d1uble"
+        "name": "\u00d1uble",
+        "sub_keys": "Bulnes~Chill\u00e1n~Coelemu~Coihueco~Quill\u00f3n~Quirihue~San Carlos~Yungay"
+    },
+    "CL/\u00d1uble/Bulnes": {
+        "id": "data/CL/\u00d1uble/Bulnes",
+        "key": "Bulnes",
+        "lang": "es"
+    },
+    "CL/\u00d1uble/Chill\u00e1n": {
+        "id": "data/CL/\u00d1uble/Chill\u00e1n",
+        "key": "Chill\u00e1n",
+        "lang": "es"
+    },
+    "CL/\u00d1uble/Coelemu": {
+        "id": "data/CL/\u00d1uble/Coelemu",
+        "key": "Coelemu",
+        "lang": "es"
+    },
+    "CL/\u00d1uble/Coihueco": {
+        "id": "data/CL/\u00d1uble/Coihueco",
+        "key": "Coihueco",
+        "lang": "es"
+    },
+    "CL/\u00d1uble/Quill\u00f3n": {
+        "id": "data/CL/\u00d1uble/Quill\u00f3n",
+        "key": "Quill\u00f3n",
+        "lang": "es"
+    },
+    "CL/\u00d1uble/Quirihue": {
+        "id": "data/CL/\u00d1uble/Quirihue",
+        "key": "Quirihue",
+        "lang": "es"
+    },
+    "CL/\u00d1uble/San Carlos": {
+        "id": "data/CL/\u00d1uble/San Carlos",
+        "key": "San Carlos",
+        "lang": "es"
+    },
+    "CL/\u00d1uble/Yungay": {
+        "id": "data/CL/\u00d1uble/Yungay",
+        "key": "Yungay",
+        "lang": "es"
     }
 }
```

### Comparing `google-i18n-address-2.5.2/i18naddress/data/cn.json` & `google_i18n_address-3.0.0/i18naddress/data/cn.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999696384211979%*

 * *Differences: {"'CN/广东省/深圳市'": "{'sub_keys': '宝安区~福田区~光明区~龙岗区~龙华区~罗湖区~南山区~坪山新区~盐田区', 'sub_lnames': "*

 * *                 '"Bao\'an Qu~Futian Qu~Guangming Qu~Longgang Qu~Longhua Qu~Luohu Qu~Nanshan '*

 * *                 'Qu~Pingshan Qu~Yantian Qu", \'sub_names\': '*

 * *                 "'宝安区~福田区~光明区~龙岗区~龙华区~罗湖区~南山区~坪山新区~盐田区', 'sub_zipexs': "*

 * *                 "'518101~518033~518107~518116~518110~518001~518052~518118~518083'}",*

 * * "'CN/广东省/深圳市/光明区'": "OrderedDict([('id', 'data/CN/广东省/深圳市/光明区'), ('key', '光明区'), ('lang', 'zh'), "*

 * *        […]*

```diff
@@ -12711,20 +12711,28 @@
     },
     "CN/\u5e7f\u4e1c\u7701/\u6df1\u5733\u5e02": {
         "id": "data/CN/\u5e7f\u4e1c\u7701/\u6df1\u5733\u5e02",
         "key": "\u6df1\u5733\u5e02",
         "lang": "zh",
         "lname": "Shenzhen Shi",
         "name": "\u6df1\u5733\u5e02",
-        "sub_keys": "\u5b9d\u5b89\u533a~\u798f\u7530\u533a~\u9f99\u5c97\u533a~\u9f99\u534e\u533a~\u7f57\u6e56\u533a~\u5357\u5c71\u533a~\u576a\u5c71\u65b0\u533a~\u76d0\u7530\u533a",
-        "sub_lnames": "Bao'an Qu~Futian Qu~Longgang Qu~Longhua Qu~Luohu Qu~Nanshan Qu~Pingshan Qu~Yantian Qu",
-        "sub_names": "\u5b9d\u5b89\u533a~\u798f\u7530\u533a~\u9f99\u5c97\u533a~\u9f99\u534e\u533a~\u7f57\u6e56\u533a~\u5357\u5c71\u533a~\u576a\u5c71\u65b0\u533a~\u76d0\u7530\u533a",
-        "sub_zipexs": "518101~518033~518116~518110~518001~518052~518118~518083",
+        "sub_keys": "\u5b9d\u5b89\u533a~\u798f\u7530\u533a~\u5149\u660e\u533a~\u9f99\u5c97\u533a~\u9f99\u534e\u533a~\u7f57\u6e56\u533a~\u5357\u5c71\u533a~\u576a\u5c71\u65b0\u533a~\u76d0\u7530\u533a",
+        "sub_lnames": "Bao'an Qu~Futian Qu~Guangming Qu~Longgang Qu~Longhua Qu~Luohu Qu~Nanshan Qu~Pingshan Qu~Yantian Qu",
+        "sub_names": "\u5b9d\u5b89\u533a~\u798f\u7530\u533a~\u5149\u660e\u533a~\u9f99\u5c97\u533a~\u9f99\u534e\u533a~\u7f57\u6e56\u533a~\u5357\u5c71\u533a~\u576a\u5c71\u65b0\u533a~\u76d0\u7530\u533a",
+        "sub_zipexs": "518101~518033~518107~518116~518110~518001~518052~518118~518083",
         "zipex": "518027"
     },
+    "CN/\u5e7f\u4e1c\u7701/\u6df1\u5733\u5e02/\u5149\u660e\u533a": {
+        "id": "data/CN/\u5e7f\u4e1c\u7701/\u6df1\u5733\u5e02/\u5149\u660e\u533a",
+        "key": "\u5149\u660e\u533a",
+        "lang": "zh",
+        "lname": "Guangming Qu",
+        "name": "\u5149\u660e\u533a",
+        "zipex": "518107"
+    },
     "CN/\u5e7f\u4e1c\u7701/\u6df1\u5733\u5e02/\u5357\u5c71\u533a": {
         "id": "data/CN/\u5e7f\u4e1c\u7701/\u6df1\u5733\u5e02/\u5357\u5c71\u533a",
         "key": "\u5357\u5c71\u533a",
         "lang": "zh",
         "lname": "Nanshan Qu",
         "name": "\u5357\u5c71\u533a",
         "zipex": "518052"
```

### Comparing `google-i18n-address-2.5.2/i18naddress/data/cu.json` & `google_i18n_address-3.0.0/i18naddress/data/cu.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/cv.json` & `google_i18n_address-3.0.0/i18naddress/data/cv.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/eg.json` & `google_i18n_address-3.0.0/i18naddress/data/eg.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/es.json` & `google_i18n_address-3.0.0/i18naddress/data/es.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9987002384408045%*

 * *Differences: {"'ES'": "{'sub_zips': "*

 * *         "'01~02~03~04~33~05~06~08~09~10~11~39~12~51~13~14~16~17~18~19~20~21~22~07~23~15~26~35~24~25~27~28~29~52~30~31~32~34~36~37~38~40~41~26127|42~43~44~45~46~47~48~49~50'}",*

 * * "'ES--ca'": "{'sub_zips': "*

 * *             "'03~02~04~01~33~05~06~08~48~09~10~11~39~12~51~13~14~16~17~18~19~20~21~22~07~23~15~26~35~24~25~27~28~29~52~30~31~32~34~36~37~38~40~41~26127|42~43~44~45~46~47~49~50'}",*

 * * "'ES--eu'": "{'sub_zips': "*

 * *             "'03~02~04~01~33~05~06~08~48~09~10~11~39~12~51~13~15~16~20 […]*

```diff
@@ -6,60 +6,60 @@
         "lang": "es",
         "languages": "es~ca~gl~eu",
         "name": "SPAIN",
         "posturl": "http://www.correos.es/contenido/13-MenuRec2/04-MenuRec24/1010_s-CodPostal.asp",
         "require": "ACSZ",
         "sub_keys": "VI~AB~A~AL~O~AV~BA~B~BU~CC~CA~S~CS~CE~CR~CO~CU~GI~GR~GU~SS~H~HU~PM~J~C~LO~GC~LE~L~LU~M~MA~ML~MU~NA~OR~P~PO~SA~TF~SG~SE~SO~T~TE~TO~V~VA~BI~ZA~Z",
         "sub_names": "\u00c1lava~Albacete~Alicante~Almer\u00eda~Asturias~\u00c1vila~Badajoz~Barcelona~Burgos~C\u00e1ceres~C\u00e1diz~Cantabria~Castell\u00f3n~Ceuta~Ciudad Real~C\u00f3rdoba~Cuenca~Girona~Granada~Guadalajara~Guip\u00fazcoa~Huelva~Huesca~Islas Baleares~Ja\u00e9n~La Coru\u00f1a~La Rioja~Las Palmas~Le\u00f3n~L\u00e9rida~Lugo~Madrid~M\u00e1laga~Melilla~Murcia~Navarra~Ourense~Palencia~Pontevedra~Salamanca~Santa Cruz de Tenerife~Segovia~Sevilla~Soria~Tarragona~Teruel~Toledo~Valencia~Valladolid~Vizcaya~Zamora~Zaragoza",
-        "sub_zips": "01~02~03~04~33~05~06~08~09~10~11~39~12~51~13~14~16~17~18~19~20~21~22~07~23~15~26(?!.*127)~35~24~25~27~28~29~52~30~31~32~34~36~37~38~40~41~26127|42~43~44~45~46~47~48~49~50",
+        "sub_zips": "01~02~03~04~33~05~06~08~09~10~11~39~12~51~13~14~16~17~18~19~20~21~22~07~23~15~26~35~24~25~27~28~29~52~30~31~32~34~36~37~38~40~41~26127|42~43~44~45~46~47~48~49~50",
         "upper": "CS",
         "zip": "\\d{5}",
         "zipex": "28039,28300,28070"
     },
     "ES--ca": {
         "fmt": "%N%n%O%n%A%n%Z %C %S",
         "id": "data/ES--ca",
         "key": "ES",
         "lang": "ca",
         "name": "SPAIN",
         "posturl": "http://www.correos.es/contenido/13-MenuRec2/04-MenuRec24/1010_s-CodPostal.asp",
         "require": "ACSZ",
         "sub_keys": "A~AB~AL~VI~O~AV~BA~B~BI~BU~CC~CA~S~CS~CE~CR~CO~CU~GI~GR~GU~SS~H~HU~PM~J~C~LO~GC~LE~L~LU~M~MA~ML~MU~NA~OR~P~PO~SA~TF~SG~SE~SO~T~TE~TO~V~VA~ZA~Z",
         "sub_names": "Alacant~Albacete~Almeria~Araba~Asturias~\u00c0vila~Badajoz~Barcelona~Bizkaia~Burgos~C\u00e1ceres~Cadis~Cantabria~Castell\u00f3~Ceuta~Ciudad Real~C\u00f3rdoba~Cuenca~Girona~Granada~Guadalajara~Guip\u00fascoa~Huelva~Huesca~Illes Balears~Ja\u00e9n~La Corunya~La Rioja~Las Palmas~Le\u00f3n~Lleida~Lugo~Madrid~M\u00e1laga~Melilla~Murcia~Navarra~Ourense~Palencia~Pontevedra~Salamanca~Santa Cruz de Tenerife~Segovia~Sevilla~Soria~Tarragona~Teruel~Toledo~Val\u00e8ncia~Valladolid~Zamora~Zaragoza",
-        "sub_zips": "03~02~04~01~33~05~06~08~48~09~10~11~39~12~51~13~14~16~17~18~19~20~21~22~07~23~15~26(?!.*127)~35~24~25~27~28~29~52~30~31~32~34~36~37~38~40~41~26127|42~43~44~45~46~47~49~50",
+        "sub_zips": "03~02~04~01~33~05~06~08~48~09~10~11~39~12~51~13~14~16~17~18~19~20~21~22~07~23~15~26~35~24~25~27~28~29~52~30~31~32~34~36~37~38~40~41~26127|42~43~44~45~46~47~49~50",
         "upper": "CS",
         "zip": "\\d{5}",
         "zipex": "28039,28300,28070"
     },
     "ES--eu": {
         "fmt": "%N%n%O%n%A%n%Z %C %S",
         "id": "data/ES--eu",
         "key": "ES",
         "lang": "eu",
         "name": "SPAIN",
         "posturl": "http://www.correos.es/contenido/13-MenuRec2/04-MenuRec24/1010_s-CodPostal.asp",
         "require": "ACSZ",
         "sub_keys": "A~AB~AL~VI~O~AV~BA~B~BI~BU~CC~CA~S~CS~CE~CR~C~CU~SS~GI~GR~GU~H~HU~PM~J~CO~LO~GC~LE~L~LU~M~MA~ML~MU~NA~OR~P~PO~SA~TF~SG~SE~SO~T~TE~TO~V~VA~ZA~Z",
         "sub_names": "Alacant~Albacete~Almer\u00eda~Araba~Asturias~\u00c1vila~Badajoz~Barcelona~Bizkaia~Burgos~C\u00e1ceres~C\u00e1diz~Cantabria~Castell\u00f3~Ceuta~Ciudad Real~Coru\u00f1a~Cuenca~Gipuzkoa~Girona~Granada~Guadalajara~Huelva~Huesca~Illes Balears~Ja\u00e9n~Kordoba~La Rioja~Las Palmas~Le\u00f3n~Lleida~Lugo~Madrid~M\u00e1laga~Melilla~Murtzia~Nafarroa~Ourense~Palentzia~Pontevedra~Salamanca~Santa Cruz Tenerifekoa~Segovia~Sevilla~Soria~Tarragona~Teruel~Toledo~Valentzia~Valladolid~Zamora~Zaragoza",
-        "sub_zips": "03~02~04~01~33~05~06~08~48~09~10~11~39~12~51~13~15~16~20~17~18~19~21~22~07~23~14~26(?!.*127)~35~24~25~27~28~29~52~30~31~32~34~36~37~38~40~41~26127|42~43~44~45~46~47~49~50",
+        "sub_zips": "03~02~04~01~33~05~06~08~48~09~10~11~39~12~51~13~15~16~20~17~18~19~21~22~07~23~14~26~35~24~25~27~28~29~52~30~31~32~34~36~37~38~40~41~26127|42~43~44~45~46~47~49~50",
         "upper": "CS",
         "zip": "\\d{5}",
         "zipex": "28039,28300,28070"
     },
     "ES--gl": {
         "fmt": "%N%n%O%n%A%n%Z %C %S",
         "id": "data/ES--gl",
         "key": "ES",
         "lang": "gl",
         "name": "SPAIN",
         "posturl": "http://www.correos.es/contenido/13-MenuRec2/04-MenuRec24/1010_s-CodPostal.asp",
         "require": "ACSZ",
         "sub_keys": "C~A~VI~AB~AL~GC~O~AV~BA~B~BI~BU~CC~CA~S~CS~CE~CR~CO~CU~GR~GU~SS~H~HU~PM~LO~LE~L~LU~M~MA~ML~MU~NA~OR~P~PO~SA~TF~SG~SE~SO~T~TE~TO~V~VA~J~GI~ZA~Z",
         "sub_names": "A Coru\u00f1a~Alacant~\u00c1lava~Albacete~Almer\u00eda~As Palmas~Asturias~\u00c1vila~Badaxoz~Barcelona~Biscaia~Burgos~C\u00e1ceres~C\u00e1diz~Cantabria~Castell\u00f3~Ceuta~Cidade Real~C\u00f3rdoba~Cuenca~Granada~Guadalajara~Guip\u00fascoa~Huelva~Huesca~Illas Baleares~La Rioja~Le\u00f3n~Lleida~Lugo~Madrid~M\u00e1laga~Melilla~Murcia~Navarra~Ourense~Palencia~Pontevedra~Salamanca~Santa Cruz de Tenerife~Segovia~Sevilla~Soria~Tarragona~Teruel~Toledo~Valencia~Valladolid~Xa\u00e9n~Xirona~Zamora~Zaragoza",
-        "sub_zips": "15~03~01~02~04~35~33~05~06~08~48~09~10~11~39~12~51~13~14~16~18~19~20~21~22~07~26(?!.*127)~24~25~27~28~29~52~30~31~32~34~36~37~38~40~41~26127|42~43~44~45~46~47~23~17~49~50",
+        "sub_zips": "15~03~01~02~04~35~33~05~06~08~48~09~10~11~39~12~51~13~14~16~18~19~20~21~22~07~26~24~25~27~28~29~52~30~31~32~34~36~37~38~40~41~26127|42~43~44~45~46~47~23~17~49~50",
         "upper": "CS",
         "zip": "\\d{5}",
         "zipex": "28039,28300,28070"
     },
     "ES/A": {
         "id": "data/ES/A",
         "key": "A",
@@ -761,36 +761,36 @@
         "zip": "24"
     },
     "ES/LO": {
         "id": "data/ES/LO",
         "key": "LO",
         "lang": "es",
         "name": "La Rioja",
-        "zip": "26(?!.*127)"
+        "zip": "26"
     },
     "ES/LO--ca": {
         "id": "data/ES/LO--ca",
         "key": "LO",
         "lang": "ca",
         "name": "La Rioja",
-        "zip": "26(?!.*127)"
+        "zip": "26"
     },
     "ES/LO--eu": {
         "id": "data/ES/LO--eu",
         "key": "LO",
         "lang": "eu",
         "name": "La Rioja",
-        "zip": "26(?!.*127)"
+        "zip": "26"
     },
     "ES/LO--gl": {
         "id": "data/ES/LO--gl",
         "key": "LO",
         "lang": "gl",
         "name": "La Rioja",
-        "zip": "26(?!.*127)"
+        "zip": "26"
     },
     "ES/LU": {
         "id": "data/ES/LU",
         "key": "LU",
         "lang": "es",
         "name": "Lugo",
         "zip": "27"
```

### Comparing `google-i18n-address-2.5.2/i18naddress/data/gb.json` & `google_i18n_address-3.0.0/i18naddress/data/gb.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/hk.json` & `google_i18n_address-3.0.0/i18naddress/data/hk.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/id.json` & `google_i18n_address-3.0.0/i18naddress/data/id.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/ie.json` & `google_i18n_address-3.0.0/i18naddress/data/ie.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/in.json` & `google_i18n_address-3.0.0/i18naddress/data/in.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/ir.json` & `google_i18n_address-3.0.0/i18naddress/data/ir.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/it.json` & `google_i18n_address-3.0.0/i18naddress/data/it.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/jm.json` & `google_i18n_address-3.0.0/i18naddress/data/jm.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/jp.json` & `google_i18n_address-3.0.0/i18naddress/data/jp.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/kp.json` & `google_i18n_address-3.0.0/i18naddress/data/kp.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/kr.json` & `google_i18n_address-3.0.0/i18naddress/data/kr.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997583811537298%*

 * *Differences: {"'KR/인천광역시'": "{'sub_zips': '230~21[01]~22[12]~21[5-7]~225~21[34]~22[6-8]~2(?:19|20)~231~22[34]'}",*

 * * "'KR/인천광역시/중구'": "{'zip': '22[34]'}"}*

```diff
@@ -1586,15 +1586,15 @@
         "isoid": "28",
         "key": "\uc778\ucc9c\uad11\uc5ed\uc2dc",
         "lang": "ko",
         "lname": "Incheon",
         "name": "\uc778\ucc9c",
         "sub_keys": "\uac15\ud654\uad70~\uacc4\uc591\uad6c~\ub0a8\uad6c~\ub0a8\ub3d9\uad6c~\ub3d9\uad6c~\ubd80\ud3c9\uad6c~\uc11c\uad6c~\uc5f0\uc218\uad6c~\uc639\uc9c4\uad70~\uc911\uad6c",
         "sub_lnames": "Ganghwa-gun~Gyeyang-gu~Nam-gu~Namdong-gu~Dong-gu~Bupyeong-gu~Seo-gu~Yeonsu-gu~Ongjin-gun~Jung-gu",
-        "sub_zips": "230~21[01]~22[12]~21[5-7]~225~21[34]~22[6-8]~2(?:19|20)~231~223",
+        "sub_zips": "230~21[01]~22[12]~21[5-7]~225~21[34]~22[6-8]~2(?:19|20)~231~22[34]",
         "zip": "2[1-3]\\d{2}",
         "zipex": "23024"
     },
     "KR/\uc778\ucc9c\uad11\uc5ed\uc2dc/\uac15\ud654\uad70": {
         "id": "data/KR/\uc778\ucc9c\uad11\uc5ed\uc2dc/\uac15\ud654\uad70",
         "key": "\uac15\ud654\uad70",
         "lang": "ko",
@@ -1658,15 +1658,15 @@
         "zip": "231"
     },
     "KR/\uc778\ucc9c\uad11\uc5ed\uc2dc/\uc911\uad6c": {
         "id": "data/KR/\uc778\ucc9c\uad11\uc5ed\uc2dc/\uc911\uad6c",
         "key": "\uc911\uad6c",
         "lang": "ko",
         "lname": "Jung-gu",
-        "zip": "223"
+        "zip": "22[34]"
     },
     "KR/\uc804\ub77c\ub0a8\ub3c4": {
         "id": "data/KR/\uc804\ub77c\ub0a8\ub3c4",
         "isoid": "46",
         "key": "\uc804\ub77c\ub0a8\ub3c4",
         "lang": "ko",
         "lname": "Jeollanam-do",
```

### Comparing `google-i18n-address-2.5.2/i18naddress/data/ky.json` & `google_i18n_address-3.0.0/i18naddress/data/ky.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/mx.json` & `google_i18n_address-3.0.0/i18naddress/data/mx.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/my.json` & `google_i18n_address-3.0.0/i18naddress/data/my.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/mz.json` & `google_i18n_address-3.0.0/i18naddress/data/mz.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/ng.json` & `google_i18n_address-3.0.0/i18naddress/data/ng.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/ni.json` & `google_i18n_address-3.0.0/i18naddress/data/ni.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/nr.json` & `google_i18n_address-3.0.0/i18naddress/data/nr.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/pe.json` & `google_i18n_address-3.0.0/i18naddress/data/pe.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/ph.json` & `google_i18n_address-3.0.0/i18naddress/data/ph.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/ru.json` & `google_i18n_address-3.0.0/i18naddress/data/ru.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/so.json` & `google_i18n_address-3.0.0/i18naddress/data/so.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/sr.json` & `google_i18n_address-3.0.0/i18naddress/data/sr.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/sv.json` & `google_i18n_address-3.0.0/i18naddress/data/sv.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/th.json` & `google_i18n_address-3.0.0/i18naddress/data/th.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/tr.json` & `google_i18n_address-3.0.0/i18naddress/data/tr.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/tv.json` & `google_i18n_address-3.0.0/i18naddress/data/tv.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/tw.json` & `google_i18n_address-3.0.0/i18naddress/data/tw.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999330387036293%*

 * *Differences: {"'TW'": "{'locality_name_type': 'district'}"}*

```diff
@@ -2,14 +2,15 @@
     "TW": {
         "fmt": "%Z%n%S%C%n%A%n%O%n%N",
         "id": "data/TW",
         "key": "TW",
         "lang": "zh-Hant",
         "languages": "zh-Hant",
         "lfmt": "%N%n%O%n%A%n%C, %S %Z",
+        "locality_name_type": "district",
         "name": "TAIWAN",
         "posturl": "http://www.post.gov.tw/post/internet/f_searchzone/index.jsp?ID=190102",
         "require": "ACSZ",
         "state_name_type": "county",
         "sub_isoids": "TXG~TPE~TTT~TNN~ILA~HUA~~NAN~PIF~MIA~TAO~KHH~KEE~~YUN~NWT~HSZ~HSQ~CYI~CYQ~CHA~PEN",
         "sub_keys": "\u53f0\u4e2d\u5e02~\u53f0\u5317\u5e02~\u53f0\u6771\u7e23~\u53f0\u5357\u5e02~\u5b9c\u862d\u7e23~\u82b1\u84ee\u7e23~\u91d1\u9580\u7e23~\u5357\u6295\u7e23~\u5c4f\u6771\u7e23~\u82d7\u6817\u7e23~\u6843\u5712\u5e02~\u9ad8\u96c4\u5e02~\u57fa\u9686\u5e02~\u9023\u6c5f\u7e23~\u96f2\u6797\u7e23~\u65b0\u5317\u5e02~\u65b0\u7af9\u5e02~\u65b0\u7af9\u7e23~\u5609\u7fa9\u5e02~\u5609\u7fa9\u7e23~\u5f70\u5316\u7e23~\u6f8e\u6e56\u7e23",
         "sub_lnames": "Taichung City~Taipei City~Taitung County~Tainan City~Yilan County~Hualien County~Kinmen County~Nantou County~Pingtung County~Miaoli County~Taoyuan City~Kaohsiung City~Keelung City~Lienchiang County~Yunlin County~New Taipei City~Hsinchu City~Hsinchu County~Chiayi City~Chiayi County~Changhua County~Penghu County",
```

### Comparing `google-i18n-address-2.5.2/i18naddress/data/ua.json` & `google_i18n_address-3.0.0/i18naddress/data/ua.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/us.json` & `google_i18n_address-3.0.0/i18naddress/data/us.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/uy.json` & `google_i18n_address-3.0.0/i18naddress/data/uy.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/ve.json` & `google_i18n_address-3.0.0/i18naddress/data/ve.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/data/vn.json` & `google_i18n_address-3.0.0/i18naddress/data/vn.json`

 * *Files identical despite different names*

### Comparing `google-i18n-address-2.5.2/i18naddress/downloader.py` & `google_i18n_address-3.0.0/i18naddress/downloader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,103 +1,98 @@
-from __future__ import unicode_literals
-
-import io
 import json
 import logging
 import os
 from multiprocessing import JoinableQueue, Manager
 from multiprocessing.pool import ThreadPool
 
 import requests
 
-from . import VALIDATION_DATA_DIR
+from i18naddress import VALIDATION_DATA_DIR
 
-MAIN_URL = 'https://chromium-i18n.appspot.com/ssl-address/data'
-DATA_PATH = os.path.join(VALIDATION_DATA_DIR, '%s.json')
+MAIN_URL = "https://chromium-i18n.appspot.com/ssl-address/data"
+DATA_PATH = os.path.join(VALIDATION_DATA_DIR, "%s.json")
 
 logger = logging.getLogger(__name__)
 work_queue = JoinableQueue()
 manager = Manager()
 
 
 def fetch(url):  # pragma: no cover
     logger.debug(url)
     data = requests.get(url).json()
     return data
 
 
 def get_countries():  # pragma: no cover
-    return fetch(MAIN_URL)['countries'].split('~') + ['ZZ']
+    return fetch(MAIN_URL)["countries"].split("~") + ["ZZ"]
 
 
 def process(key, language):
-    full_key = '%s--%s' % (key, language) if language else key
-    url = '%s/%s' % (MAIN_URL, full_key)
+    full_key = f"{key}--{language}" if language else key
+    url = f"{MAIN_URL}/{full_key}"
     data = fetch(url)
-    lang = data.get('lang')
-    languages = data.get('languages')
+    lang = data.get("lang")
+    languages = data.get("languages")
     if languages is not None:
-        langs = languages.split('~')
+        langs = languages.split("~")
         langs.remove(lang)
         for lang in langs:
             work_queue.put((key, lang))
-    if 'sub_keys' in data:
-        sub_keys = data['sub_keys'].split('~')
+    if "sub_keys" in data:
+        sub_keys = data["sub_keys"].split("~")
         for sub_key in sub_keys:
-            work_queue.put(('%s/%s' % (key, sub_key), language))
+            work_queue.put((f"{key}/{sub_key}", language))
     return full_key, data
 
 
 def worker(data):  # pragma: no cover
     while True:
         try:
             key, lang = work_queue.get()
         except EOFError:
             break
         try:
             full_key, address_data = process(key, lang)
         except Exception:
-            logger.exception('Can\'t download %s', key)
+            logger.exception("Can't download %s", key)
             work_queue.put((key, lang))
         else:
             data[full_key] = address_data
         work_queue.task_done()
 
 
 def serialize(obj, path):
-    with io.open(path, 'w', encoding='utf8') as output:
+    with open(path, "w", encoding="utf8") as output:
         data_str = json.dumps(dict(obj), ensure_ascii=False, sort_keys=True)
         output.write(data_str)
         return data_str
 
 
 def download(country=None, processes=16):
     if not os.path.exists(VALIDATION_DATA_DIR):
         os.mkdir(VALIDATION_DATA_DIR)
     data = manager.dict()
     countries = get_countries()
     if country:
         country = country.upper()
         if country not in countries:
-            raise ValueError(
-                '%s is not supported country code' % country)
+            raise ValueError("%s is not supported country code" % country)
         countries = [country]
     for country in countries:
         work_queue.put((country, None))
     workers = ThreadPool(processes, worker, initargs=(data,))
     work_queue.join()
     workers.terminate()
-    logger.debug('Queue finished')
-    with io.open(DATA_PATH % 'all', 'w', encoding='utf8') as all_output:
-        all_output.write(u'{')
+    logger.debug("Queue finished")
+    with open(DATA_PATH % "all", "w", encoding="utf8") as all_output:
+        all_output.write("{")
         for country in countries:
             country_dict = {}
             for key, address_data in data.items():
                 if key[:2] == country:
                     country_dict[key] = address_data
-            logger.debug('Saving %s', country)
-            country_json = serialize(
-                country_dict, DATA_PATH % country.lower())
+            logger.debug("Saving %s", country)
+            country_json = serialize(country_dict, DATA_PATH % country.lower())
             all_output.write(country_json[1:-1])
             if country != countries[-1]:
-                all_output.write(u',')
-        all_output.write(u'}')
+                all_output.write(",")
+        all_output.write("}")
```

