# Comparing `tmp/linuxnet-iptables-5.2.0.tar.gz` & `tmp/linuxnet-iptables-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linuxnet-iptables-5.2.0.tar", last modified: Sun Jun  4 01:22:27 2023, max compression
+gzip compressed data, was "linuxnet-iptables-5.3.0.tar", last modified: Mon Jun  5 00:26:37 2023, max compression
```

## Comparing `linuxnet-iptables-5.2.0.tar` & `linuxnet-iptables-5.3.0.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-04 01:22:27.703190 linuxnet-iptables-5.2.0/
--rw-r--r--   0 panos     (1001) users      (100)    18810 2023-01-01 01:13:07.000000 linuxnet-iptables-5.2.0/.pylintrc
--rw-r--r--   0 panos     (1001) users      (100)     2692 2023-06-04 01:14:51.000000 linuxnet-iptables-5.2.0/CHANGELOG.md
--rw-r--r--   0 panos     (1001) users      (100)    32387 2023-01-01 01:13:10.000000 linuxnet-iptables-5.2.0/LICENSE
--rw-r--r--   0 panos     (1001) users      (100)      284 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/MANIFEST.in
--rw-r--r--   0 panos     (1001) users      (100)     5164 2023-01-01 01:13:07.000000 linuxnet-iptables-5.2.0/Makefile
--rw-r--r--   0 panos     (1001) users      (100)     4132 2023-06-04 01:22:27.703190 linuxnet-iptables-5.2.0/PKG-INFO
--rw-r--r--   0 panos     (1001) users      (100)     3237 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/README.md
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-04 01:22:27.690189 linuxnet-iptables-5.2.0/docs/
--rw-r--r--   0 panos     (1001) users      (100)      905 2023-01-01 01:13:06.000000 linuxnet-iptables-5.2.0/docs/Makefile
--rw-r--r--   0 panos     (1001) users      (100)     1491 2023-03-01 20:08:53.000000 linuxnet-iptables-5.2.0/docs/chain.rst
--rw-r--r--   0 panos     (1001) users      (100)     2850 2023-01-27 18:52:21.000000 linuxnet-iptables-5.2.0/docs/conf.py
--rw-r--r--   0 panos     (1001) users      (100)     1061 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/exception.rst
--rw-r--r--   0 panos     (1001) users      (100)     8374 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/extensibility.rst
--rw-r--r--   0 panos     (1001) users      (100)     3319 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/index.rst
--rw-r--r--   0 panos     (1001) users      (100)     3187 2023-03-01 20:08:53.000000 linuxnet-iptables-5.2.0/docs/iptables_api.rst
--rw-r--r--   0 panos     (1001) users      (100)     3176 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/match-example.py
--rw-r--r--   0 panos     (1001) users      (100)     2258 2023-02-08 00:19:00.000000 linuxnet-iptables-5.2.0/docs/match.rst
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-04 01:22:27.694189 linuxnet-iptables-5.2.0/docs/matches/
--rw-r--r--   0 panos     (1001) users      (100)     1431 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/matches/commentmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)      990 2023-02-05 23:48:23.000000 linuxnet-iptables-5.2.0/docs/matches/connmarkmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1583 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/matches/conntrackmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1899 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/matches/icmpmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1861 2023-02-20 17:08:37.000000 linuxnet-iptables-5.2.0/docs/matches/limitmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1439 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/matches/markmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1965 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/matches/ownermatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     2447 2023-02-08 00:19:00.000000 linuxnet-iptables-5.2.0/docs/matches/packetmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1511 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/matches/packettypematch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1312 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/matches/statematch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1492 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/matches/tcpmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1382 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/matches/tcpmssmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1521 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/matches/ttlmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1280 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/matches/udpmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)      873 2023-03-01 20:08:53.000000 linuxnet-iptables-5.2.0/docs/rule.rst
--rw-r--r--   0 panos     (1001) users      (100)      903 2023-02-05 23:48:29.000000 linuxnet-iptables-5.2.0/docs/table.rst
--rw-r--r--   0 panos     (1001) users      (100)     1129 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/target-example.py
--rw-r--r--   0 panos     (1001) users      (100)     1201 2023-02-08 00:19:00.000000 linuxnet-iptables-5.2.0/docs/target.rst
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-04 01:22:27.697189 linuxnet-iptables-5.2.0/docs/targets/
--rw-r--r--   0 panos     (1001) users      (100)      903 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/targets/chaintarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      912 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/targets/connmarktarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/targets/dnattarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      897 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/targets/logtarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/targets/marktarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      912 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/targets/masqueradetarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      902 2023-06-04 01:12:58.000000 linuxnet-iptables-5.2.0/docs/targets/notracktarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      906 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/targets/rejecttarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/targets/snattarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      896 2023-06-04 01:12:58.000000 linuxnet-iptables-5.2.0/docs/targets/tracetarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      897 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/docs/targets/ttltarget.rst
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-04 01:22:27.697189 linuxnet-iptables-5.2.0/linuxnet/
--rw-r--r--   0 panos     (1001) users      (100)        0 2023-01-01 01:13:07.000000 linuxnet-iptables-5.2.0/linuxnet/__init__.py
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-04 01:22:27.698190 linuxnet-iptables-5.2.0/linuxnet/iptables/
--rw-r--r--   0 panos     (1001) users      (100)     1170 2023-03-01 20:08:53.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/__init__.py
--rw-r--r--   0 panos     (1001) users      (100)    24908 2023-03-01 20:08:53.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/chain.py
--rw-r--r--   0 panos     (1001) users      (100)      854 2023-02-20 17:08:37.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/deps.py
--rw-r--r--   0 panos     (1001) users      (100)     1825 2023-02-05 23:48:20.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/exceptions.py
--rw-r--r--   0 panos     (1001) users      (100)     1340 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/extension.py
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-04 01:22:27.700190 linuxnet-iptables-5.2.0/linuxnet/iptables/matches/
--rw-r--r--   0 panos     (1001) users      (100)     1295 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/matches/__init__.py
--rw-r--r--   0 panos     (1001) users      (100)     2889 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/matches/commentmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     2271 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/matches/connmarkmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     5226 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/matches/conntrackmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     9769 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/matches/icmpmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     4667 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/matches/limitmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     3852 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/matches/markmatch.py
--rw-r--r--   0 panos     (1001) users      (100)    14678 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/matches/match.py
--rw-r--r--   0 panos     (1001) users      (100)     7798 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/matches/ownermatch.py
--rw-r--r--   0 panos     (1001) users      (100)     7343 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/matches/packetmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     2844 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/matches/packettypematch.py
--rw-r--r--   0 panos     (1001) users      (100)     3155 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/matches/statematch.py
--rw-r--r--   0 panos     (1001) users      (100)    10665 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/matches/tcpmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     3833 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/matches/tcpmssmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     4322 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/matches/ttlmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     2724 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/matches/udpmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     5060 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/matches/util.py
--rw-r--r--   0 panos     (1001) users      (100)      918 2023-06-04 01:12:57.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/metadata.py
--rw-r--r--   0 panos     (1001) users      (100)     7810 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/parsing.py
--rw-r--r--   0 panos     (1001) users      (100)    16442 2023-03-01 20:08:53.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/rule.py
--rw-r--r--   0 panos     (1001) users      (100)    29087 2023-06-04 01:12:57.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/table.py
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-04 01:22:27.702190 linuxnet-iptables-5.2.0/linuxnet/iptables/targets/
--rw-r--r--   0 panos     (1001) users      (100)     1165 2023-06-04 01:12:57.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/targets/__init__.py
--rw-r--r--   0 panos     (1001) users      (100)     7386 2023-03-05 20:39:10.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/targets/connmarktarget.py
--rw-r--r--   0 panos     (1001) users      (100)     6518 2023-02-08 00:19:00.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/targets/logtarget.py
--rw-r--r--   0 panos     (1001) users      (100)     6551 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/targets/marktarget.py
--rw-r--r--   0 panos     (1001) users      (100)     4133 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/targets/masqueradetarget.py
--rw-r--r--   0 panos     (1001) users      (100)     8146 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/targets/nattarget.py
--rw-r--r--   0 panos     (1001) users      (100)     1414 2023-06-04 01:12:58.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/targets/notracktarget.py
--rw-r--r--   0 panos     (1001) users      (100)     2124 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/targets/rejecttarget.py
--rw-r--r--   0 panos     (1001) users      (100)    10896 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/targets/target.py
--rw-r--r--   0 panos     (1001) users      (100)     1396 2023-06-04 01:12:58.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/targets/tracetarget.py
--rw-r--r--   0 panos     (1001) users      (100)     4873 2023-02-06 17:07:04.000000 linuxnet-iptables-5.2.0/linuxnet/iptables/targets/ttltarget.py
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-04 01:22:27.703190 linuxnet-iptables-5.2.0/linuxnet_iptables.egg-info/
--rw-r--r--   0 panos     (1001) users      (100)     4132 2023-06-04 01:22:27.000000 linuxnet-iptables-5.2.0/linuxnet_iptables.egg-info/PKG-INFO
--rw-r--r--   0 panos     (1001) users      (100)     2625 2023-06-04 01:22:27.000000 linuxnet-iptables-5.2.0/linuxnet_iptables.egg-info/SOURCES.txt
--rw-r--r--   0 panos     (1001) users      (100)        1 2023-06-04 01:22:27.000000 linuxnet-iptables-5.2.0/linuxnet_iptables.egg-info/dependency_links.txt
--rw-r--r--   0 panos     (1001) users      (100)        9 2023-06-04 01:22:27.000000 linuxnet-iptables-5.2.0/linuxnet_iptables.egg-info/top_level.txt
--rw-r--r--   0 panos     (1001) users      (100)       38 2023-06-04 01:22:27.703190 linuxnet-iptables-5.2.0/setup.cfg
--rw-r--r--   0 panos     (1001) users      (100)     6659 2023-02-20 17:08:37.000000 linuxnet-iptables-5.2.0/setup.py
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-04 01:22:27.703190 linuxnet-iptables-5.2.0/tests/
--rw-r--r--   0 panos     (1001) users      (100)        0 2023-01-01 01:13:07.000000 linuxnet-iptables-5.2.0/tests/__init__.py
--rw-r--r--   0 panos     (1001) users      (100)    58452 2023-06-04 01:12:57.000000 linuxnet-iptables-5.2.0/tests/iptables_test.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-05 00:26:37.286196 linuxnet-iptables-5.3.0/
+-rw-r--r--   0 panos     (1001) users      (100)    18810 2023-01-01 01:13:07.000000 linuxnet-iptables-5.3.0/.pylintrc
+-rw-r--r--   0 panos     (1001) users      (100)     2807 2023-06-05 00:21:56.000000 linuxnet-iptables-5.3.0/CHANGELOG.md
+-rw-r--r--   0 panos     (1001) users      (100)    32387 2023-01-01 01:13:10.000000 linuxnet-iptables-5.3.0/LICENSE
+-rw-r--r--   0 panos     (1001) users      (100)      284 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/MANIFEST.in
+-rw-r--r--   0 panos     (1001) users      (100)     5164 2023-01-01 01:13:07.000000 linuxnet-iptables-5.3.0/Makefile
+-rw-r--r--   0 panos     (1001) users      (100)     4132 2023-06-05 00:26:37.286196 linuxnet-iptables-5.3.0/PKG-INFO
+-rw-r--r--   0 panos     (1001) users      (100)     3237 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/README.md
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-05 00:26:37.274196 linuxnet-iptables-5.3.0/docs/
+-rw-r--r--   0 panos     (1001) users      (100)      905 2023-01-01 01:13:06.000000 linuxnet-iptables-5.3.0/docs/Makefile
+-rw-r--r--   0 panos     (1001) users      (100)     1491 2023-03-01 20:08:53.000000 linuxnet-iptables-5.3.0/docs/chain.rst
+-rw-r--r--   0 panos     (1001) users      (100)     2850 2023-01-27 18:52:21.000000 linuxnet-iptables-5.3.0/docs/conf.py
+-rw-r--r--   0 panos     (1001) users      (100)     1061 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/exception.rst
+-rw-r--r--   0 panos     (1001) users      (100)     8374 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/extensibility.rst
+-rw-r--r--   0 panos     (1001) users      (100)     3319 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/index.rst
+-rw-r--r--   0 panos     (1001) users      (100)     3187 2023-03-01 20:08:53.000000 linuxnet-iptables-5.3.0/docs/iptables_api.rst
+-rw-r--r--   0 panos     (1001) users      (100)     3176 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/match-example.py
+-rw-r--r--   0 panos     (1001) users      (100)     2258 2023-02-08 00:19:00.000000 linuxnet-iptables-5.3.0/docs/match.rst
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-05 00:26:37.278196 linuxnet-iptables-5.3.0/docs/matches/
+-rw-r--r--   0 panos     (1001) users      (100)     1431 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/matches/commentmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)      990 2023-02-05 23:48:23.000000 linuxnet-iptables-5.3.0/docs/matches/connmarkmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1583 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/matches/conntrackmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1899 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/matches/icmpmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1861 2023-02-20 17:08:37.000000 linuxnet-iptables-5.3.0/docs/matches/limitmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1439 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/matches/markmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1965 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/matches/ownermatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     2447 2023-02-08 00:19:00.000000 linuxnet-iptables-5.3.0/docs/matches/packetmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1511 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/matches/packettypematch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1312 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/matches/statematch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1492 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/matches/tcpmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1382 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/matches/tcpmssmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1521 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/matches/ttlmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1280 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/matches/udpmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)      873 2023-03-01 20:08:53.000000 linuxnet-iptables-5.3.0/docs/rule.rst
+-rw-r--r--   0 panos     (1001) users      (100)      903 2023-02-05 23:48:29.000000 linuxnet-iptables-5.3.0/docs/table.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1129 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/target-example.py
+-rw-r--r--   0 panos     (1001) users      (100)     1201 2023-02-08 00:19:00.000000 linuxnet-iptables-5.3.0/docs/target.rst
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-05 00:26:37.280196 linuxnet-iptables-5.3.0/docs/targets/
+-rw-r--r--   0 panos     (1001) users      (100)      903 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/targets/chaintarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      912 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/targets/connmarktarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/targets/dnattarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      897 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/targets/logtarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/targets/marktarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      912 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/targets/masqueradetarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      902 2023-06-04 01:25:41.000000 linuxnet-iptables-5.3.0/docs/targets/notracktarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      906 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/targets/rejecttarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/targets/snattarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      896 2023-06-04 01:25:41.000000 linuxnet-iptables-5.3.0/docs/targets/tracetarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      897 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/docs/targets/ttltarget.rst
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-05 00:26:37.280196 linuxnet-iptables-5.3.0/linuxnet/
+-rw-r--r--   0 panos     (1001) users      (100)        0 2023-01-01 01:13:07.000000 linuxnet-iptables-5.3.0/linuxnet/__init__.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-05 00:26:37.281196 linuxnet-iptables-5.3.0/linuxnet/iptables/
+-rw-r--r--   0 panos     (1001) users      (100)     1170 2023-03-01 20:08:53.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/__init__.py
+-rw-r--r--   0 panos     (1001) users      (100)    25090 2023-06-05 00:20:02.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/chain.py
+-rw-r--r--   0 panos     (1001) users      (100)      854 2023-02-20 17:08:37.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/deps.py
+-rw-r--r--   0 panos     (1001) users      (100)     1825 2023-02-05 23:48:20.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/exceptions.py
+-rw-r--r--   0 panos     (1001) users      (100)     1340 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/extension.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-05 00:26:37.284196 linuxnet-iptables-5.3.0/linuxnet/iptables/matches/
+-rw-r--r--   0 panos     (1001) users      (100)     1295 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/matches/__init__.py
+-rw-r--r--   0 panos     (1001) users      (100)     2889 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/matches/commentmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     2271 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/matches/connmarkmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     5226 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/matches/conntrackmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     9769 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/matches/icmpmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     4667 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/matches/limitmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     3852 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/matches/markmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)    14678 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/matches/match.py
+-rw-r--r--   0 panos     (1001) users      (100)     7798 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/matches/ownermatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     7343 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/matches/packetmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     2844 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/matches/packettypematch.py
+-rw-r--r--   0 panos     (1001) users      (100)     3155 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/matches/statematch.py
+-rw-r--r--   0 panos     (1001) users      (100)    10665 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/matches/tcpmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     3833 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/matches/tcpmssmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     4322 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/matches/ttlmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     2724 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/matches/udpmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     5060 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/matches/util.py
+-rw-r--r--   0 panos     (1001) users      (100)      918 2023-06-05 00:20:02.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/metadata.py
+-rw-r--r--   0 panos     (1001) users      (100)     7810 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/parsing.py
+-rw-r--r--   0 panos     (1001) users      (100)    16442 2023-03-01 20:08:53.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/rule.py
+-rw-r--r--   0 panos     (1001) users      (100)    29087 2023-06-04 01:25:41.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/table.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-05 00:26:37.285196 linuxnet-iptables-5.3.0/linuxnet/iptables/targets/
+-rw-r--r--   0 panos     (1001) users      (100)     1165 2023-06-04 01:25:41.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/targets/__init__.py
+-rw-r--r--   0 panos     (1001) users      (100)     7386 2023-03-05 20:39:10.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/targets/connmarktarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     6518 2023-02-08 00:19:00.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/targets/logtarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     6551 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/targets/marktarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     4133 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/targets/masqueradetarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     8146 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/targets/nattarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     1414 2023-06-04 01:25:41.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/targets/notracktarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     2124 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/targets/rejecttarget.py
+-rw-r--r--   0 panos     (1001) users      (100)    10896 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/targets/target.py
+-rw-r--r--   0 panos     (1001) users      (100)     1396 2023-06-04 01:25:41.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/targets/tracetarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     4873 2023-02-06 17:07:04.000000 linuxnet-iptables-5.3.0/linuxnet/iptables/targets/ttltarget.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-05 00:26:37.286196 linuxnet-iptables-5.3.0/linuxnet_iptables.egg-info/
+-rw-r--r--   0 panos     (1001) users      (100)     4132 2023-06-05 00:26:37.000000 linuxnet-iptables-5.3.0/linuxnet_iptables.egg-info/PKG-INFO
+-rw-r--r--   0 panos     (1001) users      (100)     2625 2023-06-05 00:26:37.000000 linuxnet-iptables-5.3.0/linuxnet_iptables.egg-info/SOURCES.txt
+-rw-r--r--   0 panos     (1001) users      (100)        1 2023-06-05 00:26:37.000000 linuxnet-iptables-5.3.0/linuxnet_iptables.egg-info/dependency_links.txt
+-rw-r--r--   0 panos     (1001) users      (100)        9 2023-06-05 00:26:37.000000 linuxnet-iptables-5.3.0/linuxnet_iptables.egg-info/top_level.txt
+-rw-r--r--   0 panos     (1001) users      (100)       38 2023-06-05 00:26:37.286196 linuxnet-iptables-5.3.0/setup.cfg
+-rw-r--r--   0 panos     (1001) users      (100)     6662 2023-06-05 00:20:19.000000 linuxnet-iptables-5.3.0/setup.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-06-05 00:26:37.286196 linuxnet-iptables-5.3.0/tests/
+-rw-r--r--   0 panos     (1001) users      (100)        0 2023-01-01 01:13:07.000000 linuxnet-iptables-5.3.0/tests/__init__.py
+-rw-r--r--   0 panos     (1001) users      (100)    58452 2023-06-04 01:25:41.000000 linuxnet-iptables-5.3.0/tests/iptables_test.py
```

### Comparing `linuxnet-iptables-5.2.0/.pylintrc` & `linuxnet-iptables-5.3.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/CHANGELOG.md` & `linuxnet-iptables-5.3.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Change Log
 ==========
 
+5.3.0 (2023-06-04)
+------------------
+
+- added Chain.iter_rules() method
+- removed use of distutils from setup.py
+
 5.2.0 (2023-06-03)
 ------------------
 
 - added NoTrackTarget class to support the iptables NOTRACK target
 - added TraceTarget class to support the iptables TRACE target
 
 5.0.4 (2023-03-05)
```

### Comparing `linuxnet-iptables-5.2.0/LICENSE` & `linuxnet-iptables-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/Makefile` & `linuxnet-iptables-5.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/PKG-INFO` & `linuxnet-iptables-5.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linuxnet-iptables
-Version: 5.2.0
+Version: 5.3.0
 Summary: programmatic access to Linux iptables
 Home-page: https://gitlab.com/panos-tools/linuxnet-iptables
 Author: Panagiotis (Panos) Tsirigotis
 Author-email: ptsirigotis01@gmail.com
 License: AGPLv3
 Project-URL: Source, https://gitlab.com/panos-tools/linuxnet-iptables
 Project-URL: Documentation, https://linuxnet-iptables.readthedocs.io/en/latest/index.html
```

### Comparing `linuxnet-iptables-5.2.0/README.md` & `linuxnet-iptables-5.3.0/README.md`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/docs/Makefile` & `linuxnet-iptables-5.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/docs/chain.rst` & `linuxnet-iptables-5.3.0/docs/chain.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/docs/conf.py` & `linuxnet-iptables-5.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/docs/exception.rst` & `linuxnet-iptables-5.3.0/docs/exception.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/docs/extensibility.rst` & `linuxnet-iptables-5.3.0/docs/extensibility.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/docs/index.rst` & `linuxnet-iptables-5.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/docs/iptables_api.rst` & `linuxnet-iptables-5.3.0/docs/iptables_api.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/docs/match-example.py` & `linuxnet-iptables-5.3.0/docs/match-example.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/docs/match.rst` & `linuxnet-iptables-5.3.0/docs/match.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/docs/matches/commentmatch.rst` & `linuxnet-iptables-5.3.0/docs/matches/commentmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/docs/matches/connmarkmatch.rst` & `linuxnet-iptables-5.3.0/docs/matches/connmarkmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/docs/matches/conntrackmatch.rst` & `linuxnet-iptables-5.3.0/docs/matches/conntrackmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/docs/matches/icmpmatch.rst` & `linuxnet-iptables-5.3.0/docs/matches/icmpmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/docs/matches/limitmatch.rst` & `linuxnet-iptables-5.3.0/docs/matches/limitmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/docs/matches/markmatch.rst` & `linuxnet-iptables-5.3.0/docs/matches/markmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/docs/matches/ownermatch.rst` & `linuxnet-iptables-5.3.0/docs/matches/ownermatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/docs/matches/packetmatch.rst` & `linuxnet-iptables-5.3.0/docs/matches/packetmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/docs/matches/packettypematch.rst` & `linuxnet-iptables-5.3.0/docs/matches/packettypematch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/docs/matches/statematch.rst` & `linuxnet-iptables-5.3.0/docs/matches/statematch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/docs/matches/tcpmatch.rst` & `linuxnet-iptables-5.3.0/docs/matches/tcpmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/docs/matches/tcpmssmatch.rst` & `linuxnet-iptables-5.3.0/docs/matches/tcpmssmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/docs/matches/ttlmatch.rst` & `linuxnet-iptables-5.3.0/docs/matches/ttlmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/docs/matches/udpmatch.rst` & `linuxnet-iptables-5.3.0/docs/matches/udpmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/docs/rule.rst` & `linuxnet-iptables-5.3.0/docs/rule.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/docs/table.rst` & `linuxnet-iptables-5.3.0/docs/table.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/docs/target-example.py` & `linuxnet-iptables-5.3.0/docs/target-example.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/docs/target.rst` & `linuxnet-iptables-5.3.0/docs/target.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/docs/targets/chaintarget.rst` & `linuxnet-iptables-5.3.0/docs/targets/chaintarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/docs/targets/connmarktarget.rst` & `linuxnet-iptables-5.3.0/docs/targets/connmarktarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/docs/targets/dnattarget.rst` & `linuxnet-iptables-5.3.0/docs/targets/dnattarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/docs/targets/logtarget.rst` & `linuxnet-iptables-5.3.0/docs/targets/logtarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/docs/targets/marktarget.rst` & `linuxnet-iptables-5.3.0/docs/targets/marktarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/docs/targets/masqueradetarget.rst` & `linuxnet-iptables-5.3.0/docs/targets/masqueradetarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/docs/targets/notracktarget.rst` & `linuxnet-iptables-5.3.0/docs/targets/notracktarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/docs/targets/rejecttarget.rst` & `linuxnet-iptables-5.3.0/docs/targets/rejecttarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/docs/targets/snattarget.rst` & `linuxnet-iptables-5.3.0/docs/targets/snattarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/docs/targets/tracetarget.rst` & `linuxnet-iptables-5.3.0/docs/targets/tracetarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/docs/targets/ttltarget.rst` & `linuxnet-iptables-5.3.0/docs/targets/ttltarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/linuxnet/iptables/__init__.py` & `linuxnet-iptables-5.3.0/linuxnet/iptables/__init__.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/linuxnet/iptables/chain.py` & `linuxnet-iptables-5.3.0/linuxnet/iptables/chain.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # <https://www.gnu.org/licenses/>.
 
 """This module provides the Chain class
 """
 
 import traceback
 
-from typing import Callable, List, Optional
+from typing import Callable, Iterator, List, Optional
 
 from .exceptions import (IptablesError, IptablesParsingError)
 from .rule import ChainRule
 from .targets import Target, Targets, ChainTarget
 from .deps import get_logger
 
 _logger = get_logger('linuxnet.iptables.chain')
@@ -102,14 +102,19 @@
         return count
 
     def get_rules(self) -> List[ChainRule]:
         """Returns a list that contains the chain rules.
         """
         return self.__rule_list[:]
 
+    def iter_rules(self) -> Iterator[ChainRule]:
+        """Returns an iterator for the chain rules.
+        """
+        return iter(self.__rule_list)
+
     def _set_rule_list(self, rule_list: List[ChainRule]) -> None:
         """Set the rule list.
         This method is only used by the parsing code, so it does not
         update any chain reference counts.
         """
         for rulenum, rule in enumerate(rule_list, 1):
             rule._set_chain(self, rulenum)   # pylint: disable=protected-access
@@ -526,21 +531,20 @@
     @classmethod
     def create_from_existing(cls, line_list: List[str],
                 pft: 'IptablesPacketFilterTable',
                 log_parsing_failures=True) -> 'Chain':
         """Parse a set of lines from the output of ``iptables -xnv``
         into a :class:`Chain` object.
 
-        It returns a :class:`Chain` object.
-
         It raises an :exc:`IptablesParsingError` if there is a parsing error.
 
         :param line_list: list of **iptables(8)** output lines
         :param pft: an :class:`IptablesPacketFilterTable` object
         :param log_parsing_failures: if ``True``, log any parsing failures
+        :rtype: a :class:`Chain` object
         """
         line_iter = iter(line_list)
         chain = cls.__parse_chain_line(next(line_iter).rstrip())
         # The next line contains the headers - skip it
         try:
             _ = next(line_iter)
         except StopIteration as stopit:
@@ -588,15 +592,16 @@
         self.__policy_packet_count = packet_count
         self.__policy_byte_count = byte_count
 
     def __str__(self):
         return f'BuiltinChain({self.__real_chain_name})'
 
     def is_builtin(self) -> bool:
-        """Always ``True``
+        """
+        :rtype: always returns ``True``
         """
         return True
 
     def get_policy(self) -> Target:
         """Returns the policy target of this builtin chain
         """
         return self.__policy
```

### Comparing `linuxnet-iptables-5.2.0/linuxnet/iptables/deps.py` & `linuxnet-iptables-5.3.0/linuxnet/iptables/deps.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/linuxnet/iptables/exceptions.py` & `linuxnet-iptables-5.3.0/linuxnet/iptables/exceptions.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/linuxnet/iptables/extension.py` & `linuxnet-iptables-5.3.0/linuxnet/iptables/extension.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/linuxnet/iptables/matches/__init__.py` & `linuxnet-iptables-5.3.0/linuxnet/iptables/matches/__init__.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/linuxnet/iptables/matches/commentmatch.py` & `linuxnet-iptables-5.3.0/linuxnet/iptables/matches/commentmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/linuxnet/iptables/matches/connmarkmatch.py` & `linuxnet-iptables-5.3.0/linuxnet/iptables/matches/connmarkmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/linuxnet/iptables/matches/conntrackmatch.py` & `linuxnet-iptables-5.3.0/linuxnet/iptables/matches/conntrackmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/linuxnet/iptables/matches/icmpmatch.py` & `linuxnet-iptables-5.3.0/linuxnet/iptables/matches/icmpmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/linuxnet/iptables/matches/limitmatch.py` & `linuxnet-iptables-5.3.0/linuxnet/iptables/matches/limitmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/linuxnet/iptables/matches/markmatch.py` & `linuxnet-iptables-5.3.0/linuxnet/iptables/matches/markmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/linuxnet/iptables/matches/match.py` & `linuxnet-iptables-5.3.0/linuxnet/iptables/matches/match.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/linuxnet/iptables/matches/ownermatch.py` & `linuxnet-iptables-5.3.0/linuxnet/iptables/matches/ownermatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/linuxnet/iptables/matches/packetmatch.py` & `linuxnet-iptables-5.3.0/linuxnet/iptables/matches/packetmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/linuxnet/iptables/matches/packettypematch.py` & `linuxnet-iptables-5.3.0/linuxnet/iptables/matches/packettypematch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/linuxnet/iptables/matches/statematch.py` & `linuxnet-iptables-5.3.0/linuxnet/iptables/matches/statematch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/linuxnet/iptables/matches/tcpmatch.py` & `linuxnet-iptables-5.3.0/linuxnet/iptables/matches/tcpmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/linuxnet/iptables/matches/tcpmssmatch.py` & `linuxnet-iptables-5.3.0/linuxnet/iptables/matches/tcpmssmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/linuxnet/iptables/matches/ttlmatch.py` & `linuxnet-iptables-5.3.0/linuxnet/iptables/matches/ttlmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/linuxnet/iptables/matches/udpmatch.py` & `linuxnet-iptables-5.3.0/linuxnet/iptables/matches/udpmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/linuxnet/iptables/matches/util.py` & `linuxnet-iptables-5.3.0/linuxnet/iptables/matches/util.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/linuxnet/iptables/metadata.py` & `linuxnet-iptables-5.3.0/linuxnet/iptables/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,10 +18,10 @@
 """
 Metadata information intended to be used by setup.py and the
 Sphinx conf.py
 """
 
 # pylint: disable=invalid-name
 
-_version_ = "5.2.0"
+_version_ = "5.3.0"
 _author_ = "Panagiotis (Panos) Tsirigotis"
 _package_ = "linuxnet.iptables"
```

### Comparing `linuxnet-iptables-5.2.0/linuxnet/iptables/parsing.py` & `linuxnet-iptables-5.3.0/linuxnet/iptables/parsing.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/linuxnet/iptables/rule.py` & `linuxnet-iptables-5.3.0/linuxnet/iptables/rule.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/linuxnet/iptables/table.py` & `linuxnet-iptables-5.3.0/linuxnet/iptables/table.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/linuxnet/iptables/targets/__init__.py` & `linuxnet-iptables-5.3.0/linuxnet/iptables/targets/__init__.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/linuxnet/iptables/targets/connmarktarget.py` & `linuxnet-iptables-5.3.0/linuxnet/iptables/targets/connmarktarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/linuxnet/iptables/targets/logtarget.py` & `linuxnet-iptables-5.3.0/linuxnet/iptables/targets/logtarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/linuxnet/iptables/targets/marktarget.py` & `linuxnet-iptables-5.3.0/linuxnet/iptables/targets/marktarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/linuxnet/iptables/targets/masqueradetarget.py` & `linuxnet-iptables-5.3.0/linuxnet/iptables/targets/masqueradetarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/linuxnet/iptables/targets/nattarget.py` & `linuxnet-iptables-5.3.0/linuxnet/iptables/targets/nattarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/linuxnet/iptables/targets/notracktarget.py` & `linuxnet-iptables-5.3.0/linuxnet/iptables/targets/notracktarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/linuxnet/iptables/targets/rejecttarget.py` & `linuxnet-iptables-5.3.0/linuxnet/iptables/targets/rejecttarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/linuxnet/iptables/targets/target.py` & `linuxnet-iptables-5.3.0/linuxnet/iptables/targets/target.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/linuxnet/iptables/targets/tracetarget.py` & `linuxnet-iptables-5.3.0/linuxnet/iptables/targets/tracetarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/linuxnet/iptables/targets/ttltarget.py` & `linuxnet-iptables-5.3.0/linuxnet/iptables/targets/ttltarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/linuxnet_iptables.egg-info/PKG-INFO` & `linuxnet-iptables-5.3.0/linuxnet_iptables.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linuxnet-iptables
-Version: 5.2.0
+Version: 5.3.0
 Summary: programmatic access to Linux iptables
 Home-page: https://gitlab.com/panos-tools/linuxnet-iptables
 Author: Panagiotis (Panos) Tsirigotis
 Author-email: ptsirigotis01@gmail.com
 License: AGPLv3
 Project-URL: Source, https://gitlab.com/panos-tools/linuxnet-iptables
 Project-URL: Documentation, https://linuxnet-iptables.readthedocs.io/en/latest/index.html
```

### Comparing `linuxnet-iptables-5.2.0/linuxnet_iptables.egg-info/SOURCES.txt` & `linuxnet-iptables-5.3.0/linuxnet_iptables.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-5.2.0/setup.py` & `linuxnet-iptables-5.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Affero General Public
 # License for more details.
 #
 # You should have received a copy of the GNU Affero General
 # Public License along with linuxnet-iptables. If not, see
 # <https://www.gnu.org/licenses/>.
 
-import distutils.command.build
+import setuptools.command.build
 import os
 import setuptools
 
 
 from os.path import abspath, dirname
 
 NAME = "linuxnet-iptables"
@@ -38,22 +38,22 @@
 if sphinx_is_available:
     vers = sphinx_version.split('.')
     if (int(vers[0]), int(vers[1])) < (4, 4):
         sphinx_is_available = False
         print(f"** WARNING: need sphinx 4.4 or later; found {sphinx_version}")
 
 
-class LinuxnetIptablesBuild(distutils.command.build.build):
+class LinuxnetIptablesBuild(setuptools.command.build.build):
     """Custom build command that also builds the Sphinx documentation.
     """
 
     def have_sphinx(self) -> bool:
         return sphinx_is_available
 
-    distutils.command.build.build.sub_commands.append(
+    setuptools.command.build.build.sub_commands.append(
                                         ('build_sphinx', have_sphinx))
 
 
 def read_version():
     """Returns the value of the _version_ variable from the
     metadata.py module
     """
```

### Comparing `linuxnet-iptables-5.2.0/tests/iptables_test.py` & `linuxnet-iptables-5.3.0/tests/iptables_test.py`

 * *Files identical despite different names*

