# Comparing `tmp/pypkamd-0.5.0.tar.gz` & `tmp/pypkamd-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypkamd-0.5.0.tar", max compression
+gzip compressed data, was "pypkamd-0.5.1.tar", max compression
```

## Comparing `pypkamd-0.5.0.tar` & `pypkamd-0.5.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     2115 2022-01-19 12:13:48.383820 pypkamd-0.5.0/README.md
--rw-r--r--   0        0        0    24268 2022-06-03 09:10:14.510824 pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/atomtypes.atp
--rw-r--r--   0        0        0   102989 2022-06-03 09:10:14.526823 pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/cmap.itp
--rw-r--r--   0        0        0  1207981 2022-09-20 09:12:56.785759 pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/ffbonded.itp
--rw-r--r--   0        0        0  1854528 2022-09-19 17:32:23.091945 pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/ffnonbonded.itp
--rw-r--r--   0        0        0    10332 2022-06-03 09:10:15.066820 pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/forcefield.doc
--rw-r--r--   0        0        0      650 2022-06-03 09:10:15.070820 pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/forcefield.itp
--rw-r--r--   0        0        0     1873 2022-06-03 09:10:15.074820 pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/gb.itp
--rw-r--r--   0        0        0     1568 2022-06-03 09:10:15.078820 pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/ions.itp
--rw-r--r--   0        0        0       78 2022-06-03 09:10:15.082820 pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/merged.arn
--rw-r--r--   0        0        0     2350 2022-09-27 10:28:28.305371 pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/merged.c.tdb
--rw-r--r--   0        0        0    21532 2022-08-30 09:29:16.058060 pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/merged.hdb
--rw-r--r--   0        0        0     2744 2022-06-03 11:02:39.066983 pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/merged.n.tdb
--rw-r--r--   0        0        0      161 2022-06-03 09:10:15.186819 pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/merged.r2b
--rw-r--r--   0        0        0  3127722 2022-08-30 08:54:13.946151 pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/merged.rtp
--rw-r--r--   0        0        0     4292 2022-06-03 09:10:15.546816 pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/merged.vsd
--rw-r--r--   0        0        0  3129435 2022-08-29 12:16:25.329851 pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/merged_original.rtp.bak
--rw-r--r--   0        0        0     4727 2022-06-03 09:10:15.550816 pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/nbfix.itp
--rw-r--r--   0        0        0    54970 2022-06-03 09:10:15.558816 pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/old_c36_cmap.itp
--rw-r--r--   0        0        0     5000 2022-09-27 10:30:59.689633 pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/protstates.dic
--rw-r--r--   0        0        0     2723 2022-08-30 08:41:41.975365 pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/residuetypes.dat
--rw-r--r--   0        0        0      484 2022-06-03 09:10:15.566816 pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/spc.itp
--rw-r--r--   0        0        0      490 2022-06-03 09:10:15.562816 pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/spce.itp
--rw-r--r--   0        0        0      817 2022-06-03 09:10:15.570816 pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/tip3p.itp
--rw-r--r--   0        0        0     1011 2022-06-03 09:10:15.574816 pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/tip4p.itp
--rw-r--r--   0        0        0      198 2022-06-03 09:10:15.578816 pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/watermodels.dat
--rw-r--r--   0        0        0     1395 2021-09-24 15:33:14.669398 pypkamd-0.5.0/pypkamd/G54A7pH.ff/aminoacids.c.tdb
--rw-r--r--   0        0        0     1393 2021-04-20 15:50:28.363716 pypkamd-0.5.0/pypkamd/G54A7pH.ff/aminoacids.c_old.tdb
--rw-r--r--   0        0        0     4407 2021-06-18 15:21:31.300924 pypkamd-0.5.0/pypkamd/G54A7pH.ff/aminoacids.hdb
--rw-r--r--   0        0        0     2115 2021-04-20 15:54:42.157889 pypkamd-0.5.0/pypkamd/G54A7pH.ff/aminoacids.n.tdb
--rw-r--r--   0        0        0     2209 2021-04-20 15:49:50.387990 pypkamd-0.5.0/pypkamd/G54A7pH.ff/aminoacids.n_old.tdb
--rw-r--r--   0        0        0      132 2021-03-09 11:38:23.640424 pypkamd-0.5.0/pypkamd/G54A7pH.ff/aminoacids.r2b
--rw-r--r--   0        0        0   332237 2022-06-21 12:34:12.777623 pypkamd-0.5.0/pypkamd/G54A7pH.ff/aminoacids.rtp
--rw-r--r--   0        0        0   321668 2021-04-20 15:42:34.095136 pypkamd-0.5.0/pypkamd/G54A7pH.ff/aminoacids.rtp.old
--rw-r--r--   0        0        0     3584 2021-03-09 11:38:23.636424 pypkamd-0.5.0/pypkamd/G54A7pH.ff/aminoacids.vsd
--rw-r--r--   0        0        0     2566 2021-03-09 11:38:23.636424 pypkamd-0.5.0/pypkamd/G54A7pH.ff/atomtypes.atp
--rw-r--r--   0        0        0     9588 2021-03-09 11:38:23.628424 pypkamd-0.5.0/pypkamd/G54A7pH.ff/dppc.itp
--rw-r--r--   0        0        0     1224 2021-03-09 11:38:23.628424 pypkamd-0.5.0/pypkamd/G54A7pH.ff/ff_dum.itp
--rw-r--r--   0        0        0    13752 2021-03-09 11:38:23.624424 pypkamd-0.5.0/pypkamd/G54A7pH.ff/ffbonded.itp
--rw-r--r--   0        0        0   116315 2021-03-09 11:38:23.620424 pypkamd-0.5.0/pypkamd/G54A7pH.ff/ffnonbonded.itp
--rw-r--r--   0        0        0      115 2021-03-09 11:38:23.616424 pypkamd-0.5.0/pypkamd/G54A7pH.ff/forcefield.doc
--rw-r--r--   0        0        0      176 2021-03-09 11:38:23.616424 pypkamd-0.5.0/pypkamd/G54A7pH.ff/forcefield.itp
--rw-r--r--   0        0        0     1014 2021-03-09 11:38:23.612424 pypkamd-0.5.0/pypkamd/G54A7pH.ff/ions.itp
--rw-r--r--   0        0        0    10066 2021-03-09 11:38:23.608424 pypkamd-0.5.0/pypkamd/G54A7pH.ff/popc.itp
--rw-r--r--   0        0        0     3990 2022-07-08 13:21:45.044961 pypkamd-0.5.0/pypkamd/G54A7pH.ff/protstates.dic
--rw-r--r--   0        0        0     2691 2022-07-20 08:16:28.853139 pypkamd-0.5.0/pypkamd/G54A7pH.ff/residuetypes.dat
--rw-r--r--   0        0        0      815 2021-03-09 11:38:23.608424 pypkamd-0.5.0/pypkamd/G54A7pH.ff/spc.itp
--rw-r--r--   0        0        0      815 2021-03-09 11:38:23.604424 pypkamd-0.5.0/pypkamd/G54A7pH.ff/spce.itp
--rw-r--r--   0        0        0      636 2021-03-09 11:38:23.600424 pypkamd-0.5.0/pypkamd/G54A7pH.ff/tip3p.itp
--rw-r--r--   0        0        0     1148 2021-03-09 11:38:23.600424 pypkamd-0.5.0/pypkamd/G54A7pH.ff/tip4p.itp
--rw-r--r--   0        0        0    21767 2021-03-09 11:38:23.596424 pypkamd-0.5.0/pypkamd/G54A7pH.ff/tmcl.itp
--rw-r--r--   0        0        0       90 2021-03-09 11:38:23.592424 pypkamd-0.5.0/pypkamd/G54A7pH.ff/watermodels.dat
--rw-r--r--   0        0        0       99 2022-11-22 09:29:19.332249 pypkamd-0.5.0/pypkamd/__init__.py
--rw-r--r--   0        0        0      260 2022-12-01 09:59:08.487076 pypkamd-0.5.0/pypkamd/__main__.py
--rw-r--r--   0        0        0       22 2023-01-31 13:42:20.691918 pypkamd-0.5.0/pypkamd/_version.py
--rw-r--r--   0        0        0     1793 2022-03-02 14:43:53.710684 pypkamd-0.5.0/pypkamd/cli.py
--rwxr-xr-x   0        0        0     8441 2023-01-31 13:07:41.322832 pypkamd-0.5.0/pypkamd/configs.py
--rw-r--r--   0        0        0      189 2021-07-19 08:16:16.715637 pypkamd-0.5.0/pypkamd/constants.py
--rwxr-xr-x   0        0        0    16752 2022-09-27 11:23:09.785677 pypkamd-0.5.0/pypkamd/cphmd.py
--rwxr-xr-x   0        0        0    22600 2022-11-22 09:39:48.249200 pypkamd-0.5.0/pypkamd/fixbox/fixbox
--rw-r--r--   0        0        0    23006 2021-03-09 11:32:18.967137 pypkamd-0.5.0/pypkamd/fixbox/fixbox.c
--rwxr-xr-x   0        0        0    35072 2021-03-09 11:37:03.921016 pypkamd-0.5.0/pypkamd/fixbox/fixbox_
--rwxr-xr-x   0        0        0     1810 2022-06-21 18:48:18.083062 pypkamd-0.5.0/pypkamd/misc.py
--rwxr-xr-x   0        0        0    21003 2022-06-23 15:24:20.364534 pypkamd-0.5.0/pypkamd/topology.py
--rw-r--r--   0        0        0      896 2023-01-31 13:42:20.691918 pypkamd-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3029 2023-01-31 13:43:58.446823 pypkamd-0.5.0/setup.py
--rw-r--r--   0        0        0     2977 2023-01-31 13:43:58.447594 pypkamd-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     2115 2022-01-19 12:13:48.383820 pypkamd-0.5.1/README.md
+-rw-r--r--   0        0        0    24268 2022-06-03 09:10:14.510824 pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/atomtypes.atp
+-rw-r--r--   0        0        0   102989 2022-06-03 09:10:14.526823 pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/cmap.itp
+-rw-r--r--   0        0        0  1207981 2022-09-20 09:12:56.785759 pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/ffbonded.itp
+-rw-r--r--   0        0        0  1854528 2022-09-19 17:32:23.091945 pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/ffnonbonded.itp
+-rw-r--r--   0        0        0    10332 2022-06-03 09:10:15.066820 pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/forcefield.doc
+-rw-r--r--   0        0        0      650 2022-06-03 09:10:15.070820 pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/forcefield.itp
+-rw-r--r--   0        0        0     1873 2022-06-03 09:10:15.074820 pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/gb.itp
+-rw-r--r--   0        0        0     1568 2022-06-03 09:10:15.078820 pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/ions.itp
+-rw-r--r--   0        0        0       78 2022-06-03 09:10:15.082820 pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/merged.arn
+-rw-r--r--   0        0        0     2350 2022-09-27 10:28:28.305371 pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/merged.c.tdb
+-rw-r--r--   0        0        0    21532 2022-08-30 09:29:16.058060 pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/merged.hdb
+-rw-r--r--   0        0        0     2744 2022-06-03 11:02:39.066983 pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/merged.n.tdb
+-rw-r--r--   0        0        0      161 2022-06-03 09:10:15.186819 pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/merged.r2b
+-rw-r--r--   0        0        0  3127722 2022-08-30 08:54:13.946151 pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/merged.rtp
+-rw-r--r--   0        0        0     4292 2022-06-03 09:10:15.546816 pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/merged.vsd
+-rw-r--r--   0        0        0  3129435 2022-08-29 12:16:25.329851 pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/merged_original.rtp.bak
+-rw-r--r--   0        0        0     4727 2022-06-03 09:10:15.550816 pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/nbfix.itp
+-rw-r--r--   0        0        0    54970 2022-06-03 09:10:15.558816 pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/old_c36_cmap.itp
+-rw-r--r--   0        0        0     5000 2022-09-27 10:30:59.689633 pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/protstates.dic
+-rw-r--r--   0        0        0     2723 2022-08-30 08:41:41.975365 pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/residuetypes.dat
+-rw-r--r--   0        0        0      484 2022-06-03 09:10:15.566816 pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/spc.itp
+-rw-r--r--   0        0        0      490 2022-06-03 09:10:15.562816 pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/spce.itp
+-rw-r--r--   0        0        0      817 2022-06-03 09:10:15.570816 pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/tip3p.itp
+-rw-r--r--   0        0        0     1011 2022-06-03 09:10:15.574816 pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/tip4p.itp
+-rw-r--r--   0        0        0      198 2022-06-03 09:10:15.578816 pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/watermodels.dat
+-rw-r--r--   0        0        0     1395 2021-09-24 15:33:14.669398 pypkamd-0.5.1/pypkamd/G54A7pH.ff/aminoacids.c.tdb
+-rw-r--r--   0        0        0     1393 2021-04-20 15:50:28.363716 pypkamd-0.5.1/pypkamd/G54A7pH.ff/aminoacids.c_old.tdb
+-rw-r--r--   0        0        0     4407 2021-06-18 15:21:31.300924 pypkamd-0.5.1/pypkamd/G54A7pH.ff/aminoacids.hdb
+-rw-r--r--   0        0        0     2115 2021-04-20 15:54:42.157889 pypkamd-0.5.1/pypkamd/G54A7pH.ff/aminoacids.n.tdb
+-rw-r--r--   0        0        0     2209 2021-04-20 15:49:50.387990 pypkamd-0.5.1/pypkamd/G54A7pH.ff/aminoacids.n_old.tdb
+-rw-r--r--   0        0        0      132 2021-03-09 11:38:23.640424 pypkamd-0.5.1/pypkamd/G54A7pH.ff/aminoacids.r2b
+-rw-r--r--   0        0        0   332237 2022-06-21 12:34:12.777623 pypkamd-0.5.1/pypkamd/G54A7pH.ff/aminoacids.rtp
+-rw-r--r--   0        0        0   321668 2021-04-20 15:42:34.095136 pypkamd-0.5.1/pypkamd/G54A7pH.ff/aminoacids.rtp.old
+-rw-r--r--   0        0        0     3584 2021-03-09 11:38:23.636424 pypkamd-0.5.1/pypkamd/G54A7pH.ff/aminoacids.vsd
+-rw-r--r--   0        0        0     2566 2021-03-09 11:38:23.636424 pypkamd-0.5.1/pypkamd/G54A7pH.ff/atomtypes.atp
+-rw-r--r--   0        0        0     9588 2021-03-09 11:38:23.628424 pypkamd-0.5.1/pypkamd/G54A7pH.ff/dppc.itp
+-rw-r--r--   0        0        0     1224 2021-03-09 11:38:23.628424 pypkamd-0.5.1/pypkamd/G54A7pH.ff/ff_dum.itp
+-rw-r--r--   0        0        0    13752 2021-03-09 11:38:23.624424 pypkamd-0.5.1/pypkamd/G54A7pH.ff/ffbonded.itp
+-rw-r--r--   0        0        0   116315 2021-03-09 11:38:23.620424 pypkamd-0.5.1/pypkamd/G54A7pH.ff/ffnonbonded.itp
+-rw-r--r--   0        0        0      115 2021-03-09 11:38:23.616424 pypkamd-0.5.1/pypkamd/G54A7pH.ff/forcefield.doc
+-rw-r--r--   0        0        0      176 2021-03-09 11:38:23.616424 pypkamd-0.5.1/pypkamd/G54A7pH.ff/forcefield.itp
+-rw-r--r--   0        0        0     1014 2021-03-09 11:38:23.612424 pypkamd-0.5.1/pypkamd/G54A7pH.ff/ions.itp
+-rw-r--r--   0        0        0    10066 2021-03-09 11:38:23.608424 pypkamd-0.5.1/pypkamd/G54A7pH.ff/popc.itp
+-rw-r--r--   0        0        0     3990 2022-07-08 13:21:45.044961 pypkamd-0.5.1/pypkamd/G54A7pH.ff/protstates.dic
+-rw-r--r--   0        0        0     2691 2022-07-20 08:16:28.853139 pypkamd-0.5.1/pypkamd/G54A7pH.ff/residuetypes.dat
+-rw-r--r--   0        0        0      815 2021-03-09 11:38:23.608424 pypkamd-0.5.1/pypkamd/G54A7pH.ff/spc.itp
+-rw-r--r--   0        0        0      815 2021-03-09 11:38:23.604424 pypkamd-0.5.1/pypkamd/G54A7pH.ff/spce.itp
+-rw-r--r--   0        0        0      636 2021-03-09 11:38:23.600424 pypkamd-0.5.1/pypkamd/G54A7pH.ff/tip3p.itp
+-rw-r--r--   0        0        0     1148 2021-03-09 11:38:23.600424 pypkamd-0.5.1/pypkamd/G54A7pH.ff/tip4p.itp
+-rw-r--r--   0        0        0    21767 2021-03-09 11:38:23.596424 pypkamd-0.5.1/pypkamd/G54A7pH.ff/tmcl.itp
+-rw-r--r--   0        0        0       90 2021-03-09 11:38:23.592424 pypkamd-0.5.1/pypkamd/G54A7pH.ff/watermodels.dat
+-rw-r--r--   0        0        0       99 2022-11-22 09:29:19.332249 pypkamd-0.5.1/pypkamd/__init__.py
+-rw-r--r--   0        0        0      260 2022-12-01 09:59:08.487076 pypkamd-0.5.1/pypkamd/__main__.py
+-rw-r--r--   0        0        0       22 2023-06-05 19:16:31.976347 pypkamd-0.5.1/pypkamd/_version.py
+-rw-r--r--   0        0        0     1793 2022-03-02 14:43:53.710684 pypkamd-0.5.1/pypkamd/cli.py
+-rwxr-xr-x   0        0        0     8441 2023-01-31 13:07:41.322832 pypkamd-0.5.1/pypkamd/configs.py
+-rw-r--r--   0        0        0      189 2021-07-19 08:16:16.715637 pypkamd-0.5.1/pypkamd/constants.py
+-rwxr-xr-x   0        0        0    16752 2022-09-27 11:23:09.785677 pypkamd-0.5.1/pypkamd/cphmd.py
+-rwxr-xr-x   0        0        0    22600 2022-11-22 09:39:48.249200 pypkamd-0.5.1/pypkamd/fixbox/fixbox
+-rw-r--r--   0        0        0    23006 2021-03-09 11:32:18.967137 pypkamd-0.5.1/pypkamd/fixbox/fixbox.c
+-rwxr-xr-x   0        0        0    35072 2021-03-09 11:37:03.921016 pypkamd-0.5.1/pypkamd/fixbox/fixbox_
+-rwxr-xr-x   0        0        0     1811 2023-06-05 19:14:40.373570 pypkamd-0.5.1/pypkamd/misc.py
+-rwxr-xr-x   0        0        0    21003 2022-06-23 15:24:20.364534 pypkamd-0.5.1/pypkamd/topology.py
+-rw-r--r--   0        0        0      896 2023-06-05 19:16:03.096663 pypkamd-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3029 2023-06-05 19:17:06.882022 pypkamd-0.5.1/setup.py
+-rw-r--r--   0        0        0     2977 2023-06-05 19:17:06.882805 pypkamd-0.5.1/PKG-INFO
```

### Comparing `pypkamd-0.5.0/README.md` & `pypkamd-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/atomtypes.atp` & `pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/atomtypes.atp`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/cmap.itp` & `pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/cmap.itp`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/ffbonded.itp` & `pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/ffbonded.itp`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/ffnonbonded.itp` & `pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/ffnonbonded.itp`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/forcefield.doc` & `pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/forcefield.doc`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/forcefield.itp` & `pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/forcefield.itp`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/gb.itp` & `pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/gb.itp`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/ions.itp` & `pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/ions.itp`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/merged.c.tdb` & `pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/merged.c.tdb`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/merged.hdb` & `pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/merged.hdb`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/merged.n.tdb` & `pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/merged.n.tdb`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/merged.rtp` & `pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/merged.rtp`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/merged.vsd` & `pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/merged.vsd`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/merged_original.rtp.bak` & `pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/merged_original.rtp.bak`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/nbfix.itp` & `pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/nbfix.itp`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/old_c36_cmap.itp` & `pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/old_c36_cmap.itp`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/protstates.dic` & `pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/protstates.dic`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/residuetypes.dat` & `pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/residuetypes.dat`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/tip3p.itp` & `pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/tip3p.itp`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/CHARMM36mpH.ff/tip4p.itp` & `pypkamd-0.5.1/pypkamd/CHARMM36mpH.ff/tip4p.itp`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/G54A7pH.ff/aminoacids.c.tdb` & `pypkamd-0.5.1/pypkamd/G54A7pH.ff/aminoacids.c.tdb`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/G54A7pH.ff/aminoacids.c_old.tdb` & `pypkamd-0.5.1/pypkamd/G54A7pH.ff/aminoacids.c_old.tdb`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/G54A7pH.ff/aminoacids.hdb` & `pypkamd-0.5.1/pypkamd/G54A7pH.ff/aminoacids.hdb`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/G54A7pH.ff/aminoacids.n.tdb` & `pypkamd-0.5.1/pypkamd/G54A7pH.ff/aminoacids.n.tdb`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/G54A7pH.ff/aminoacids.n_old.tdb` & `pypkamd-0.5.1/pypkamd/G54A7pH.ff/aminoacids.n_old.tdb`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/G54A7pH.ff/aminoacids.rtp` & `pypkamd-0.5.1/pypkamd/G54A7pH.ff/aminoacids.rtp`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/G54A7pH.ff/aminoacids.rtp.old` & `pypkamd-0.5.1/pypkamd/G54A7pH.ff/aminoacids.rtp.old`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/G54A7pH.ff/aminoacids.vsd` & `pypkamd-0.5.1/pypkamd/G54A7pH.ff/aminoacids.vsd`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/G54A7pH.ff/atomtypes.atp` & `pypkamd-0.5.1/pypkamd/G54A7pH.ff/atomtypes.atp`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/G54A7pH.ff/dppc.itp` & `pypkamd-0.5.1/pypkamd/G54A7pH.ff/dppc.itp`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/G54A7pH.ff/ff_dum.itp` & `pypkamd-0.5.1/pypkamd/G54A7pH.ff/ff_dum.itp`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/G54A7pH.ff/ffbonded.itp` & `pypkamd-0.5.1/pypkamd/G54A7pH.ff/ffbonded.itp`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/G54A7pH.ff/ffnonbonded.itp` & `pypkamd-0.5.1/pypkamd/G54A7pH.ff/ffnonbonded.itp`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/G54A7pH.ff/ions.itp` & `pypkamd-0.5.1/pypkamd/G54A7pH.ff/ions.itp`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/G54A7pH.ff/popc.itp` & `pypkamd-0.5.1/pypkamd/G54A7pH.ff/popc.itp`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/G54A7pH.ff/protstates.dic` & `pypkamd-0.5.1/pypkamd/G54A7pH.ff/protstates.dic`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/G54A7pH.ff/residuetypes.dat` & `pypkamd-0.5.1/pypkamd/G54A7pH.ff/residuetypes.dat`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/G54A7pH.ff/spc.itp` & `pypkamd-0.5.1/pypkamd/G54A7pH.ff/spc.itp`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/G54A7pH.ff/spce.itp` & `pypkamd-0.5.1/pypkamd/G54A7pH.ff/spce.itp`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/G54A7pH.ff/tip3p.itp` & `pypkamd-0.5.1/pypkamd/G54A7pH.ff/tip3p.itp`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/G54A7pH.ff/tip4p.itp` & `pypkamd-0.5.1/pypkamd/G54A7pH.ff/tip4p.itp`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/G54A7pH.ff/tmcl.itp` & `pypkamd-0.5.1/pypkamd/G54A7pH.ff/tmcl.itp`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/cli.py` & `pypkamd-0.5.1/pypkamd/cli.py`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/configs.py` & `pypkamd-0.5.1/pypkamd/configs.py`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/cphmd.py` & `pypkamd-0.5.1/pypkamd/cphmd.py`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/fixbox/fixbox` & `pypkamd-0.5.1/pypkamd/fixbox/fixbox`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/fixbox/fixbox.c` & `pypkamd-0.5.1/pypkamd/fixbox/fixbox.c`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/fixbox/fixbox_` & `pypkamd-0.5.1/pypkamd/fixbox/fixbox_`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pypkamd/misc.py` & `pypkamd-0.5.1/pypkamd/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     with open("tmp.pdb") as f:
         for line in f:
             if line.startswith("ATOM "):
                 atom, _, res, chain, resnumb, *_ = read_pdb_line(line)
                 if resnumb in sites["A"] and res == "CYS":
                     if resnumb not in potential:
                         potential.append(resnumb)
-                    if atom == "HG" and resnumb not in confirmed:
+                    if atom == "HG1" and resnumb not in confirmed:
                         confirmed.append(resnumb)
     to_del = set(potential) - set(confirmed)
     sites = set(sites["A"]) - to_del
 
     return list(sites)
```

### Comparing `pypkamd-0.5.0/pypkamd/topology.py` & `pypkamd-0.5.1/pypkamd/topology.py`

 * *Files identical despite different names*

### Comparing `pypkamd-0.5.0/pyproject.toml` & `pypkamd-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pypkamd"
-version = "0.5.0"
+version = "0.5.1"
 description = "PypKa + GROMACS = an awesome Constant-pH Molecular Dynamics implementation"
 authors = ["Pedro Reis <pdreis@fc.ul.pt>"]
 license = "LGPLv3"
 readme = "README.md"
 homepage = "https://github.com/mms-fcul/PypKa-MD"
 repository = "https://github.com/mms-fcul/PypKa-MD"
 classifiers = [
```

### Comparing `pypkamd-0.5.0/setup.py` & `pypkamd-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['pypka==2.10.0']
 
 entry_points = \
 {'console_scripts': ['pypkamd = pypkamd.__main__:main']}
 
 setup_kwargs = {
     'name': 'pypkamd',
-    'version': '0.5.0',
+    'version': '0.5.1',
     'description': 'PypKa + GROMACS = an awesome Constant-pH Molecular Dynamics implementation',
     'long_description': '# PypKa-MD\n\nPypKa + MD = constant-pH molecular dynamics\n\nImplementation of the stochastic titration method <sup>1</sup>\n\n[1] Baptista *et al.*, J. Chem. Phys. 117, 4184 (2002) DOI: 10.1063/1.1497164\n\n## Installation\n\n```\npython3 -m pip install pypkamd\n```\n\n## Dependencies\n\nBoth PypKa and GROMACS are required to be installed in the system.\n\n- PypKa >= 2.7.1\n- GROMACS >=5.1.5\n\nWhen running in pKAI-MD mode there are extra dependencies:\n\n- pege >= 1.1.1\n- torch_geometric >= 2.0.0\n\nPlease refer to the installation guide of [torch geometric](https://pytorch-geometric.readthedocs.io/en/latest/notes/installation.html) to install the proper version in accordance to your CUDA and OS.\n\n```\npython3 -m pip install pege\n# EXAMPLE FOR CUDA10.2\n# python3 -m pip install torch-scatter torch-sparse torch-cluster torch-spline-conv torch-geometric -f https://data.pyg.org/whl/torch-1.10.0+cu102.html\n```\n\n\n## Usage\n\nUpon installation a PypKa-MD executable should have been added to your bin. You may call it directly giving as an argument a modified GROMACS .mdp input file to include Constant-pH specific variables.\n\n```\npypkamd System.mdp\n```\n\nIn case the executable as not been added to your bin, you may use:\n\n```\npython3 -m pypkamd System.mdp\n```\n\nYou may find an example .mdp file in /utils/cphmd.mdp. \n\n```\n; GROin = system_000.gro     ; input GRO file\n; TOPin = system_000.top     ; input TOP file\n; DATin = fixgro.dat         ; input DAT file (to be removed)\n; NDXin = system.ndx         ; input NDX file\n; sysname = system_001       ; output files root name\n; sites = all                ; to be titrating sites in the protein\n; titrating_group = Protein  ; index group of the protein\n; nCycles = 50               ; number of CpHMD cycles\n                            ;; total simulation time = nCycles * tau_prot\n                            ;; 1ns = 50 * 20ps\n; nCPUs = 4                  ; number of CPUs to be used\n; pH = 7.0                   ; pH value of the protonation states sampling\n; ionicstr = 0.1             ; ionic strength used in PB\n; GroDIR="/gromacs/gromacs-5.1.5_pH_I/bin/" ; GROMACS bin path\n```',
     'author': 'Pedro Reis',
     'author_email': 'pdreis@fc.ul.pt',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/mms-fcul/PypKa-MD',
```

### Comparing `pypkamd-0.5.0/PKG-INFO` & `pypkamd-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypkamd
-Version: 0.5.0
+Version: 0.5.1
 Summary: PypKa + GROMACS = an awesome Constant-pH Molecular Dynamics implementation
 Home-page: https://github.com/mms-fcul/PypKa-MD
 License: LGPLv3
 Author: Pedro Reis
 Author-email: pdreis@fc.ul.pt
 Requires-Python: >=3.6.2,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

