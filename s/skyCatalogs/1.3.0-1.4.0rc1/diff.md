# Comparing `tmp/skyCatalogs-1.3.0.tar.gz` & `tmp/skyCatalogs-1.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skyCatalogs-1.3.0.tar", last modified: Mon Feb 13 23:43:33 2023, max compression
+gzip compressed data, was "skyCatalogs-1.4.0rc1.tar", last modified: Mon Jun  5 20:22:58 2023, max compression
```

## Comparing `skyCatalogs-1.3.0.tar` & `skyCatalogs-1.4.0rc1.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-02-13 23:43:33.506713 skyCatalogs-1.3.0/
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     1569 2021-09-30 21:55:06.000000 skyCatalogs-1.3.0/LICENSE
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     1427 2023-02-13 23:43:33.506315 skyCatalogs-1.3.0/PKG-INFO
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     1082 2021-09-30 21:55:06.000000 skyCatalogs-1.3.0/README.md
--rw-rw----   0 jrbogart (71218) jrbogart (71218)      716 2023-02-13 23:24:59.000000 skyCatalogs-1.3.0/pyproject.toml
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-02-13 23:43:33.482466 skyCatalogs-1.3.0/python/
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-02-13 23:43:33.486174 skyCatalogs-1.3.0/python/desc/
--rw-rw----   0 jrbogart (71218) jrbogart (71218)       66 2022-05-06 00:22:58.000000 skyCatalogs-1.3.0/python/desc/__init__.py
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-02-13 23:43:33.488922 skyCatalogs-1.3.0/python/desc/skycatalogs/
--rw-rw----   0 jrbogart (71218) jrbogart (71218)      280 2023-02-13 23:24:59.000000 skyCatalogs-1.3.0/python/desc/skycatalogs/__init__.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    34060 2023-01-17 00:30:52.000000 skyCatalogs-1.3.0/python/desc/skycatalogs/catalog_creator.py
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-02-13 23:43:33.491675 skyCatalogs-1.3.0/python/desc/skycatalogs/objects/
--rw-rw----   0 jrbogart (71218) jrbogart (71218)       27 2022-04-22 19:59:14.000000 skyCatalogs-1.3.0/python/desc/skycatalogs/objects/__init__.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    28347 2022-12-12 00:51:42.000000 skyCatalogs-1.3.0/python/desc/skycatalogs/objects/base_object.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     3748 2021-11-09 20:13:55.000000 skyCatalogs-1.3.0/python/desc/skycatalogs/objects/galaxy_object.py
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-02-13 23:43:33.493293 skyCatalogs-1.3.0/python/desc/skycatalogs/readers/
--rw-rw----   0 jrbogart (71218) jrbogart (71218)       30 2022-04-22 19:59:14.000000 skyCatalogs-1.3.0/python/desc/skycatalogs/readers/__init__.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     2379 2022-11-08 20:21:20.000000 skyCatalogs-1.3.0/python/desc/skycatalogs/readers/parquet_reader.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    32692 2022-11-11 20:07:55.000000 skyCatalogs-1.3.0/python/desc/skycatalogs/skyCatalogs.py
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-02-13 23:43:33.501039 skyCatalogs-1.3.0/python/desc/skycatalogs/utils/
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     1077 2021-09-30 21:55:07.000000 skyCatalogs-1.3.0/python/desc/skycatalogs/utils/SED_parquet.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)      174 2022-11-08 20:21:20.000000 skyCatalogs-1.3.0/python/desc/skycatalogs/utils/__init__.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     2008 2022-07-13 01:54:07.000000 skyCatalogs-1.3.0/python/desc/skycatalogs/utils/common_utils.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     9666 2023-02-03 01:12:14.000000 skyCatalogs-1.3.0/python/desc/skycatalogs/utils/config_utils.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)      533 2022-07-13 01:54:07.000000 skyCatalogs-1.3.0/python/desc/skycatalogs/utils/exceptions.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     1211 2021-09-30 21:55:07.000000 skyCatalogs-1.3.0/python/desc/skycatalogs/utils/make_fake.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     5373 2023-02-03 01:12:14.000000 skyCatalogs-1.3.0/python/desc/skycatalogs/utils/parquet_schema_utils.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     8165 2022-12-12 00:51:42.000000 skyCatalogs-1.3.0/python/desc/skycatalogs/utils/sed_tools.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     9870 2022-07-13 01:54:07.000000 skyCatalogs-1.3.0/python/desc/skycatalogs/utils/translate_utils.py
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-02-13 23:43:33.503756 skyCatalogs-1.3.0/python/skyCatalogs.egg-info/
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     1427 2023-02-13 23:43:33.502020 skyCatalogs-1.3.0/python/skyCatalogs.egg-info/PKG-INFO
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     1073 2023-02-13 23:43:33.502546 skyCatalogs-1.3.0/python/skyCatalogs.egg-info/SOURCES.txt
--rw-rw----   0 jrbogart (71218) jrbogart (71218)        1 2023-02-13 23:43:33.503005 skyCatalogs-1.3.0/python/skyCatalogs.egg-info/dependency_links.txt
--rw-rw----   0 jrbogart (71218) jrbogart (71218)       82 2023-02-13 23:43:33.503427 skyCatalogs-1.3.0/python/skyCatalogs.egg-info/requires.txt
--rw-rw----   0 jrbogart (71218) jrbogart (71218)        5 2023-02-13 23:43:33.503860 skyCatalogs-1.3.0/python/skyCatalogs.egg-info/top_level.txt
--rw-rw----   0 jrbogart (71218) jrbogart (71218)       38 2023-02-13 23:43:33.506836 skyCatalogs-1.3.0/setup.cfg
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-02-13 23:43:33.505079 skyCatalogs-1.3.0/tests/
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    11941 2022-11-10 00:01:22.000000 skyCatalogs-1.3.0/tests/test_API.py
--rw-r--r--   0 jrbogart (71218) jrbogart (71218)      642 2021-12-17 00:54:24.000000 skyCatalogs-1.3.0/tests/test_skyCatalogs.py
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-06-05 20:22:58.756411 skyCatalogs-1.4.0rc1/
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     1569 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/LICENSE
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     1430 2023-06-05 20:22:58.756004 skyCatalogs-1.4.0rc1/PKG-INFO
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     1082 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/README.md
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)      720 2023-06-05 20:06:34.000000 skyCatalogs-1.4.0rc1/pyproject.toml
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-06-05 20:22:58.732546 skyCatalogs-1.4.0rc1/python/
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-06-05 20:22:58.735867 skyCatalogs-1.4.0rc1/python/desc/
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)       66 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/python/desc/__init__.py
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-06-05 20:22:58.738060 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)      337 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/__init__.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    36150 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/catalog_creator.py
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-06-05 20:22:58.740542 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/objects/
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)       27 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/objects/__init__.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    29080 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/objects/base_object.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     3748 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/objects/galaxy_object.py
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-06-05 20:22:58.741992 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/readers/
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)       30 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/readers/__init__.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     2379 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/readers/parquet_reader.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    33685 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/skyCatalogs.py
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-06-05 20:22:58.751677 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/utils/
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     1077 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/utils/SED_parquet.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)      198 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/utils/__init__.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     2008 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/utils/common_utils.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    11009 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/utils/config_utils.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)      533 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/utils/exceptions.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     1211 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/utils/make_fake.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     7656 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/utils/parquet_schema_utils.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     8165 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/utils/sed_tools.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     1411 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/utils/sn_tools.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     9870 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/python/desc/skycatalogs/utils/translate_utils.py
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-06-05 20:22:58.753996 skyCatalogs-1.4.0rc1/python/skyCatalogs.egg-info/
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     1430 2023-06-05 20:22:58.752608 skyCatalogs-1.4.0rc1/python/skyCatalogs.egg-info/PKG-INFO
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     1115 2023-06-05 20:22:58.752963 skyCatalogs-1.4.0rc1/python/skyCatalogs.egg-info/SOURCES.txt
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)        1 2023-06-05 20:22:58.753338 skyCatalogs-1.4.0rc1/python/skyCatalogs.egg-info/dependency_links.txt
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)       82 2023-06-05 20:22:58.753696 skyCatalogs-1.4.0rc1/python/skyCatalogs.egg-info/requires.txt
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)        5 2023-06-05 20:22:58.754046 skyCatalogs-1.4.0rc1/python/skyCatalogs.egg-info/top_level.txt
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)       38 2023-06-05 20:22:58.756495 skyCatalogs-1.4.0rc1/setup.cfg
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2023-06-05 20:22:58.755185 skyCatalogs-1.4.0rc1/tests/
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    11941 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/tests/test_API.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)      642 2023-06-05 19:26:34.000000 skyCatalogs-1.4.0rc1/tests/test_skyCatalogs.py
```

### Comparing `skyCatalogs-1.3.0/LICENSE` & `skyCatalogs-1.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.3.0/PKG-INFO` & `skyCatalogs-1.4.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skyCatalogs
-Version: 1.3.0
+Version: 1.4.0rc1
 Summary: Writes, reads catalogs input to LSST DESC simulations
 Author-email: Joanne Bogart <jrb@slac.stanford.edu>
 Keywords: desc,python,catalog,simulation
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `skyCatalogs-1.3.0/README.md` & `skyCatalogs-1.4.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.3.0/pyproject.toml` & `skyCatalogs-1.4.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"] # PEP 621 compliant
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "skyCatalogs"
-version = "1.3.0"
+version = "1.4.0-rc1"
 description = "Writes, reads catalogs input to LSST DESC simulations"
 readme = "README.md"
 authors = [{ name = "Joanne Bogart", email = "jrb@slac.stanford.edu" }]
 license = { file = "LICENCE" }
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
```

### Comparing `skyCatalogs-1.3.0/python/desc/skycatalogs/catalog_creator.py` & `skyCatalogs-1.4.0rc1/python/desc/skycatalogs/catalog_creator.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from multiprocessing import Process, Pipe
 from astropy.coordinates import SkyCoord
 import sqlite3
 from desc.skycatalogs.utils.common_utils import print_date
 from desc.skycatalogs.utils.sed_tools import ObservedSedFactory, get_star_sed_path
 from desc.skycatalogs.utils.config_utils import create_config, assemble_SED_models
 from desc.skycatalogs.utils.config_utils import assemble_MW_extinction, assemble_cosmology, assemble_object_types, assemble_provenance, write_yaml
-from desc.skycatalogs.utils.parquet_schema_utils import make_galaxy_schema, make_galaxy_flux_schema, make_star_schema, make_star_flux_schema
+from desc.skycatalogs.utils.parquet_schema_utils import make_galaxy_schema, make_galaxy_flux_schema, make_star_flux_schema, make_pointsource_schema
 from desc.skycatalogs.objects.base_object import LSST_BANDS, BaseObject
 
 from desc.skycatalogs.objects.base_object import ObjectCollection
 
 # from dm stack
 from dustmaps.sfd import SFDQuery
 
@@ -101,14 +101,15 @@
         send_conn.send(out_dict)
     else:
         return out_dict
 
 class CatalogCreator:
     def __init__(self, parts, area_partition, skycatalog_root=None,
                  catalog_dir='.', galaxy_truth=None,
+                 star_truth=None, sn_truth=None,
                  config_path=None, catalog_name='skyCatalog',
                  output_type='parquet', mag_cut=None,
                  sed_subdir='galaxyTopHatSED', knots_mag_cut=27.0,
                  knots=True, logname='skyCatalogs.creator',
                  pkg_root=None, skip_done=False, flux_only=False,
                  main_only=False, flux_parallel=16, provenance=None,
                  dc2=False):
@@ -151,14 +152,17 @@
                         to that for the DC2 run
 
         Might want to add a way to specify template for output file name
         and template for input sedLookup file name.
         """
 
         _cosmo_cat = 'cosmodc2_v1.1.4_image_addon_knots'
+        _star_db = '/global/cfs/cdirs/lsst/groups/SSim/DC2/dc2_stellar_healpixel.db'
+        _sn_db = '/global/cfs/cdirs/lsst/groups/SSim/DC2/cosmoDC2_v1.1.4/sne_cosmoDC2_v1.1.4_MS_DDF_healpix.db'
+
         self._galaxy_stride = 1000000
         if pkg_root:
             self._pkg_root = pkg_root
         else:
             self._pkg_root = os.path.join(os.path.dirname(__file__),
                                           '../../..')
 
@@ -168,16 +172,21 @@
         if output_type != 'parquet':
             raise NotImplementedError(f'CatalogCreator: Output type {output_type} not supported')
 
         self._galaxy_truth = galaxy_truth
         if galaxy_truth is None:
             self._galaxy_truth = _cosmo_cat
 
-        self._sn_truth = None
-        self._star_truth = None
+        self._sn_truth = sn_truth
+        if self._sn_truth is None:
+            self._sn_truth = _sn_db
+
+        self._star_truth = star_truth
+        if self._star_truth is None:
+            self._star_truth = _star_db
         self._cat = None
 
         self._parts = parts
         self._area_partition = area_partition
         if skycatalog_root:
             self._skycatalog_root = skycatalog_root
         else:
@@ -606,41 +615,36 @@
                 rg_written +=1
 
         writer.close()
         self._logger.debug(f'# row groups written to flux file: {rg_written}')
         if self._provenance == 'yaml':
             self.write_provenance_file(output_path)
 
-    def create_pointsource_catalog(self, star_truth=None, sn_truth=None):
+    def create_pointsource_catalog(self):
 
         """
         Parameters
         ----------
         star_truth      Where to find star parameters. If None use default
         sn_truth       Where to find SN parameters.  If None, use default
 
         Might want to add a way to specify template for output file name
 
         Returns
         -------
         None
         """
-
-        # For now fixed location for star, SNe parameter files.
-        _star_db = '/global/cfs/cdirs/lsst/groups/SSim/DC2/dc2_stellar_healpixel.db'
-        _sn_db = '/global/cfs/cdirs/lsst/groups/SSim/DC2/cosmoDC2_v1.1.4/sne_cosmoDC2_v1.1.4_MS_DDF_healpix.db'
-        self._star_truth = _star_db
-        self._sn_truth = _sn_db
-
-        arrow_schema = make_star_schema()
+        arrow_schema = make_pointsource_schema()
         #  Need a way to indicate which object types to include; deal with that
-        #  later.  For now, default is stars only.  Use default star parameter file.
+        #  later.  For now, default is stars + sn
         for p in self._parts:
             self._logger.debug(f'Point sources. Starting on pixel {p}')
-            self.create_pointsource_pixel(p, arrow_schema, star_cat=_star_db)
+            self.create_pointsource_pixel(p, arrow_schema,
+                                          star_cat=self._star_truth,
+                                          sn_cat=self._sn_truth)
             self._logger.debug(f'Completed pixel {p}')
 
     def create_pointsource_pixel(self, pixel, arrow_schema, star_cat=None,
                              sn_cat=None):
         if not star_cat and not sn_cat:
             self._logger.info('No point source inputs specified')
             return
@@ -651,18 +655,22 @@
         if os.path.exists(output_path):
             if not self._skip_done:
                 self._logger.info(f'Overwriting file {output_path}')
             else:
                 self._logger.info(f'Skipping regeneration of {output_path}')
                 return
 
+        writer = pq.ParquetWriter(output_path, arrow_schema)
+
         if star_cat:
             # Get data for this pixel
-            cols = ','.join(['simobjid as id', 'ra', 'decl as dec',
-                             'magNorm as magnorm', 'sedFilename as sed_filepath'])
+            cols = ','.join(['format("%s",simobjid) as id', 'ra', 'decl as dec',
+                             'magNorm as magnorm', 'mura', 'mudecl as mudec',
+                             'radialVelocity as radial_velocity', 'parallax',
+                             'sedFilename as sed_filepath'])
             q = f'select {cols} from stars where hpid={pixel} '
             with sqlite3.connect(star_cat) as conn:
                 star_df = pd.read_sql_query(q, conn)
 
             star_df['sed_filepath'] = get_star_sed_path(star_df['sed_filepath'])
 
             nobj = len(star_df['id'])
@@ -670,26 +678,62 @@
             star_df['object_type'] = np.full((nobj,), 'star')
             star_df['host_galaxy_id'] = np.zeros((nobj,), np.int64())
 
             star_df['MW_rv'] = np.full((nobj,), _MW_rv_constant, np.float32())
 
             star_df['MW_av'] = _make_MW_extinction(np.array(star_df['ra']),
                                                    np.array(star_df['dec']))
+            star_df['variability_model'] = np.full((nobj,), '')
+            star_df['salt2_params'] = np.full((nobj,), None)
             out_table = pa.Table.from_pandas(star_df, schema=arrow_schema)
-            self._logger.debug('Created arrow table from dataframe')
+            self._logger.debug('Created arrow table from star dataframe')
 
-            writer = pq.ParquetWriter(output_path, arrow_schema)
+            #writer = pq.ParquetWriter(output_path, arrow_schema)
             writer.write_table(out_table)
 
-            writer.close()
-            if self._provenance == 'yaml':
-                self.write_provenance_file(output_path)
-
         if sn_cat:
-            raise NotImplementedError('SNe not yet supported. Have a nice day.')
+            # Get data for this pixel
+            cols = ','.join(['snid_in as id', 'snra_in as ra',
+                             'sndec_in as dec', 'galaxy_id as host_galaxy_id'])
+
+            params = ','.join(['z_in as z', 't0_in as t0, x0_in as x0',
+                             'x1_in as x1', 'c_in as c'])
+
+            q1 = f'select {cols} from sne_params where hpid={pixel} '
+            q2 = f'select {params} from sne_params where hpid={pixel} '
+            with sqlite3.connect(sn_cat) as conn:
+                sn_df = pd.read_sql_query(q1, conn)
+                params_df = pd.read_sql_query(q2, conn)
+
+            nobj = len(sn_df['ra'])
+            sn_df['object_type'] = np.full((nobj,), 'sn')
+
+            sn_df['MW_rv'] = np.full((nobj,), _MW_rv_constant, np.float32())
+            sn_df['MW_av'] = _make_MW_extinction(np.array(sn_df['ra']),
+                                                   np.array(sn_df['dec']))
+
+            # Add fillers for columns not relevant for sn
+            sn_df['sed_filepath'] = np.full((nobj),'')
+            sn_df['magnorm'] = np.full((nobj,), None)
+            sn_df['mura'] = np.full((nobj,), None)
+            sn_df['mudec'] = np.full((nobj,), None)
+            sn_df['radial_velocity'] = np.full((nobj,), None)
+            sn_df['parallax'] = np.full((nobj,), None)
+            sn_df['variability_model'] = np.full((nobj,), 'salt2_extended')
+
+            # Form array of struct from params_df
+            sn_df['salt2_params'] = params_df.to_records(index=False)
+            out_table = pa.Table.from_pandas(sn_df, schema=arrow_schema)
+            self._logger.debug('Created arrow table from sn dataframe')
+
+            writer.write_table(out_table)
+
+        writer.close()
+        if self._provenance == 'yaml':
+            self.write_provenance_file(output_path)
 
         return
 
     def create_pointsource_flux_catalog(self, config_file=None):
         '''
         Create a second file per healpixel containing just id and
         LSST fluxes.  Use information in the main file to compute fluxes
```

### Comparing `skyCatalogs-1.3.0/python/desc/skycatalogs/objects/base_object.py` & `skyCatalogs-1.4.0rc1/python/desc/skycatalogs/objects/base_object.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import galsim
 import logging
 from galsim.errors import GalSimRangeError
 
 from desc.skycatalogs.utils.translate_utils import form_object_string
 from desc.skycatalogs.utils.config_utils import Config
 from desc.skycatalogs.utils.sed_tools import ObservedSedFactory
+from desc.skycatalogs.utils.sn_tools import SNObject
 
 '''
 Main object types.   There are also may be subtypes. For example,
 there could be two subtypes for bulge components, differing in the
 form of their associated SEDs
 '''
 
@@ -50,14 +51,15 @@
     Read in lsst bandpasses from standard place, trim, and store in global dict
     Returns: The dict
 
     '''
     global lsst_bandpasses
     lsst_bandpasses = dict()
     rubin_sim_dir = os.getenv('RUBIN_SIM_DATA_DIR', None)
+    bp_dir = None
     if rubin_sim_dir:
         bp_dir = os.path.join(rubin_sim_dir, 'throughputs', 'baseline')
 
         if os.path.exists(bp_dir):
             BaseObject._bp_path = bp_dir
             #logger.info(f'Using rubin sim dir {rubin_sim_dir}')
         else:
@@ -66,20 +68,20 @@
             #logger.info(f'Using rubin sim dir rubin_sim_data under HOME')
             if os.path.exists(bp_dir):
                 BaseObject._bp_path = bp_dir
             else:
                 #logger.info('Using galsim built-in bandpasses')
                 bp_dir = None
                 fname_fmt = 'LSST_{band}.dat'
-        for band in LSST_BANDS:
-            if bp_dir:
-                bp_full_path = os.path.join(bp_dir, f'total_{band}.dat')
-            else:
-                bp_full_path = f'LSST_{band}.dat'
-            lsst_bandpasses[band] = galsim.Bandpass(bp_full_path, 'nm').thin()
+    for band in LSST_BANDS:
+        if bp_dir:
+            bp_full_path = os.path.join(bp_dir, f'total_{band}.dat')
+        else:
+            bp_full_path = f'LSST_{band}.dat'
+        lsst_bandpasses[band] = galsim.Bandpass(bp_full_path, 'nm').thin()
 
     return lsst_bandpasses
 
 class BaseObject(object):
     '''
     Abstract base class for static (in position coordinates) objects.
     Likely need a variant for SSO.
@@ -184,15 +186,15 @@
         Returns: A string formatted like a line in an instance catalog
         '''
         if self.object_type == 'galaxy':
             if component not in self.subcomponents:
                 return ''
         return form_object_string(self, band, component)
 
-    def get_sed(self, component=None, resolution=None):
+    def get_sed(self, component=None, resolution=None, mjd=None):
         '''
         Return sed and mag_norm for a galaxy component or for a star
         Parameters
         ----------
         component    one of 'bulge', 'disk', 'knots' for now. Other components
                      may be supported.  Ignored for stars
         resolution   desired resolution of lambda in nanometers. Ignored
@@ -212,16 +214,24 @@
             mag_norm = self.get_native_attribute('magnorm')
             rel_path = self.get_native_attribute('sed_filepath')
 
             fpath = os.path.join(os.getenv('SIMS_SED_LIBRARY_DIR'),
                                  self.get_native_attribute('sed_filepath'))
 
             return sky_cat.observed_sed_factory.create_pointsource(rel_path), mag_norm
+        elif self._object_type == 'sn':
+            # Make an SNObject and get SED
+            params = self.get_native_attribute('salt2_params')
+            sn = SNObject(params=params)
+            if mjd < sn.mintime() or mjd > sn.maxtime():
+                return None, 0.0
+            # Already normalized so magnorm is zero
+            return sn.get_sed(mjd), 0.0
         if self._object_type != 'galaxy':
-            raise ValueError('get_sed function only available for stars and galaxy components')
+            raise ValueError('get_sed function only available for stars, sne and galaxy components')
         if component not in ['disk', 'bulge', 'knots']:
             raise ValueError(f'Cannot fetch SED for component type {component}')
 
         th_val = self.get_native_attribute(f'sed_val_{component}')
         if  th_val is None:   #  values for this component are not in the file
             raise ValueError(f'{component} not part of this catalog')
 
@@ -229,21 +239,22 @@
         if max(th_val) < np.finfo('float').resolution:
             return None, 0.0
 
         z_h = self.get_native_attribute('redshift_hubble')
         z = self.get_native_attribute('redshift')
 
         sed = sky_cat.observed_sed_factory.create(th_val, z_h, z,
-                                                     resolution=resolution)
+                                                  resolution=resolution)
         magnorm = sky_cat.observed_sed_factory.magnorm(th_val, z_h)
 
         return sed, magnorm
 
-    def write_sed(self, sed_file_path, component=None, resolution=None):
-        sed, _ = self.get_sed(component=component, resolution=None)
+    def write_sed(self, sed_file_path, component=None, resolution=None,
+                  mjd=None):
+        sed, _ = self.get_sed(component=component, resolution=None, mjd=None)
 
         wl = sed.wave_list
         flambda = [sed(w) for w in wl]
 
         with open(sed_file_path, 'w') as sed_file:
             for lam, flam in zip(wl, flambda):
                 sed_file.write(f'{lam} {flam}\n')
@@ -270,15 +281,15 @@
     def get_gsobject_components(self, gsparams=None, rng=None):
         """
         Return a dictionary of the GSObject components for the
         sky catalogs object, keyed by component name.
         """
         if gsparams is not None:
             gsparams = galsim.GSParams(**gsparams)
-        if self.object_type == 'star':
+        if self.object_type == 'star' or self.object_type == 'sn':
             return {None: galsim.DeltaFunction(gsparams=gsparams)}
         if self.object_type != 'galaxy':
             raise RuntimeError("Do not know how to handle object type "
                                f"{self.object_type}")
         obj_dict = {}
         for component in self.subcomponents:
             # knots use the same major/minor axes as the disk component.
@@ -317,139 +328,152 @@
             # in the old code.
             shear = galsim.Shear(g1=-e1, g2=-e2)
             obj = obj._shear(shear)
             g1, g2, mu = self.get_wl_params()
             obj_dict[component] = obj._lens(g1, g2, mu)
         return obj_dict
 
-    def get_observer_sed_component(self, component):
+    def get_observer_sed_component(self, component, mjd=None):
         """
         Return the SED for the specified subcomponent of the SkyCatalog
         object, applying internal extinction, redshift, and Milky Way
         extinction.
 
         For Milky Way extinction, the Fitzpatrick, et al. (2019) (F19)
         model, as implemented in the dust_extinction package, is used.
 
         The SEDs are computed assuming exposure times of 1 second.
         """
         # Create a galsim.SED for this subcomponent.
-        if self._object_type == 'star':   # or other pointsource
-            sed, magnorm = self.get_sed(component=component)
+
+        if self._object_type == 'star':
+            sed, magnorm = self.get_sed(component=component, mjd=mjd)
             # The SED is in units of photons/nm/cm^2/s
             # -0.9210340371976184 = -np.log(10)/2.5. Use to convert mag to flux
             flux_500 = np.exp(-0.9210340371976184 * magnorm)
             sed = sed.withMagnitude(0, self._bp500)
             sed = sed*flux_500
-        else:
-            # For galaxy components sed already has correct normalization
+        elif self._object_type == 'galaxy':
+            # For sn & galaxy components sed already has correct normalization
             sed, _ = self.get_sed(component=component)
             if sed is None:
                 # This subcomponent has zero emission so return None.
                 return None
-
+        elif self._object_type == 'sn':
+            sed, _ = self.get_sed(component=component, mjd=mjd)
+            if sed is None:
+                return None
+        else:
+            # Raise NYI exception?
+            pass
 
         iAv, iRv, mwAv, mwRv = self.get_dust()
         if iAv > 0:
             # Apply internal extinction model, which is assumed
             # to be the same for all subcomponents.
             pass  #TODO add implementation for internal extinction.
 
         # redshift already applied by create or create_pointsource
 
         # Apply Milky Way extinction.
         sed = sky_cat.extinguisher.extinguish(sed, mwAv)
         return sed
 
-    def get_observer_sed_components(self):
+    def get_observer_sed_components(self, mjd=None):
         """
         Return a dictionary of the SEDs, keyed by component name.
         """
         sed_components = {}
         subcomponents = [None] if not self.subcomponents \
             else self.subcomponents
         for component in subcomponents:
-            sed = self.get_observer_sed_component(component)
+            sed = self.get_observer_sed_component(component, mjd=mjd)
             if sed is not None:
                 sed_components[component] = sed
         return sed_components
 
-    def get_total_observer_sed(self):
+    def get_total_observer_sed(self, mjd=None):
         """
         Return the SED summed over SEDs for the individual SkyCatalog
         components.
         """
         sed = None
-        for sed_component in self.get_observer_sed_components().values():
+        for sed_component in self.get_observer_sed_components(mjd=mjd).values():
             if sed is None:
                 sed = sed_component
             else:
                 sed += sed_component
+
+        if sed is None:
+            return sed
         if 'shear_1' in self.native_columns:
             _, _, mu = self.get_wl_params()
             sed *= mu
         return sed
 
-    def get_flux(self, bandpass, sed=None):
+    def get_flux(self, bandpass, sed=None, mjd=None):
         """
         Return the total object flux integrated over the bandpass
         in photons/sec/cm^2
         Use supplied sed if there is one
         """
 
         if not sed:
-            sed = self.get_total_observer_sed()
+            sed = self.get_total_observer_sed(mjd=mjd)
+
+        if sed is None:
+            return 0.0
 
         flux = sed.calculateFlux(bandpass)
 
         return flux
 
-    def get_fluxes(self, bandpasses):
+    def get_fluxes(self, bandpasses, mjd=None):
         # To avoid recomputing sed
-        sed = self.get_total_observer_sed()
+        sed = self.get_total_observer_sed(mjd=mjd)
+        if sed is None:
+            return [0.0 for b in bandpasses]
+
         return [sed.calculateFlux(b) for b in bandpasses]
 
-    def get_LSST_flux(self, band, sed=None, cache=True):
+    def get_LSST_flux(self, band, sed=None, cache=True, mjd=None):
         if not band in LSST_BANDS:
             return None
         att = f'lsst_flux_{band}'
-        # Check if it's already an attribute
-        val = getattr(self, att, None)
-        if val is not None:
-            return val
-
-        if att in self.native_columns:
-            return self.get_native_attribute(att)
+        if mjd is None:
+            # Check if it's already an attribute
+            val = getattr(self, att, None)
+            if val is not None:
+                return val
+
+        # For now exclude sn
+        if self.object_type != 'sn':
+            if att in self.native_columns:
+                return self.get_native_attribute(att)
 
-        val = self.get_flux(lsst_bandpasses[band], sed=sed)
+        val = self.get_flux(lsst_bandpasses[band], sed=sed, mjd=mjd)
 
-        if cache:
+        if cache and mjd is None:
             setattr(self, att, val)
         return val
 
-    def get_LSST_fluxes(self, cache=True, as_dict=True):
+    def get_LSST_fluxes(self, cache=True, as_dict=True, mjd=None):
         '''
         Return a dict of fluxes for LSST bandpasses or, if as_dict is False,
         just a list in the same order as LSST_BANDS
         '''
         fluxes = dict()
-        sed = self.get_total_observer_sed()
-        for band in LSST_BANDS:
-            ##### temporary to debug error, now apparently fixed
-            try:
-                fluxes[band] = self.get_LSST_flux(band, sed=sed, cache=cache)
-            except GalSimRangeError as e:
-                logger = logging.getLogger('skyCatalogs.creator')
-                galaxy_id = self.get_native_attribute('galaxy_id')
-                logger.debug(f'galaxy_id: {galaxy_id}  band: {band}')
-                redshift = self.get_native_attribute('redshift')
-                logger.debug(f'redshift: {redshift}')
-                logger.debug(f'GalSimRangeError: {e}')
+        sed = self.get_total_observer_sed(mjd=mjd)
+        if sed is None:
+            for band in LSST_BANDS:
                 fluxes[band] = 0.0
-
+        else:
+            for band in LSST_BANDS:
+                fluxes[band] = self.get_LSST_flux(band, sed=sed,
+                                                  cache=cache, mjd=mjd)
         if as_dict:
             return fluxes
         else:
             return list(fluxes.values())
 
 class ObjectCollection(Sequence):
     '''
@@ -470,18 +494,15 @@
         sky_catalog instance of SkyCatalog class
         (redshift should probably be ditched; no need for it)
         (similarly for region with current code structure. Information
         needed is encoded in mask)
 
         mask  indices to be masked off, e.g. because region does not
               include the entire healpix pixel
-        readers one per file associated with the type(s). (Galaxy info
-              is stored in two files)
-
-
+        readers one per file associated with the type(s).
         '''
         self._ra = np.array(ra)
         self._dec = np.array(dec)
         self._id = np.array(id)
         self._rdrs = readers
         self._partition_id = partition_id
         self._sky_catalog = sky_catalog   # might not need this
```

### Comparing `skyCatalogs-1.3.0/python/desc/skycatalogs/objects/galaxy_object.py` & `skyCatalogs-1.4.0rc1/python/desc/skycatalogs/objects/galaxy_object.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.3.0/python/desc/skycatalogs/readers/parquet_reader.py` & `skyCatalogs-1.4.0rc1/python/desc/skycatalogs/readers/parquet_reader.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.3.0/python/desc/skycatalogs/skyCatalogs.py` & `skyCatalogs-1.4.0rc1/python/desc/skycatalogs/skyCatalogs.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,25 +112,26 @@
                                    nest=False)
         return pixels
 
     if isinstance(region, PolygonalRegion):
         return healpy.query_polygon(nside, region.get_vertices(),
                                     inclusive=True, nest=False)
 
-def _compress_via_mask(tbl, id_column, region):
+def _compress_via_mask(tbl, id_column, region, galaxy=True):
     '''
     Parameters
     ----------
     tbl          data table including columns named "ra", "dec", and id_column
     id_column    string
     region       mask should restrict to this region (or not at all if None)
 
     Returns
     -------
-    4 values ra, dec, id, mask
+    4 values for galaxies: ra, dec, id, mask
+    5 values for pointsources: ra, dec, id, object_type, mask
     If objects are in the region, ra, dec, id correspond to those objects.
     mask will mask off unused objects
     If there are no objects in the region, all return values are None
 
     '''
     if region is not None:
         if isinstance(region, PolygonalRegion):        # special case
@@ -140,15 +141,18 @@
             ra_min = min([v[0] for v in vertices])
             dec_max = max([v[1] for v in vertices])
             dec_min = min([v[1] for v in vertices])
             bnd_box = Box(ra_min, ra_max, dec_min, dec_max)
             # Compute mask for that box
             mask = _compute_mask(bnd_box, tbl['ra'], tbl['dec'])
             if all(mask): # even bounding box doesn't intersect table rows
-                return None, None, None, None
+                if galaxy:
+                    return None, None, None, None
+                else:
+                    return None, None, None, None, None
 
             # Get compressed ra, dec
             ra_compress = ma.array(tbl['ra'], mask=mask).compressed()
             dec_compress = ma.array(tbl['dec'], mask=mask).compressed()
             poly_mask = _compute_mask(region, ra_compress, dec_compress)
 
             # Get indices of unmasked
@@ -156,22 +160,33 @@
 
             # Update bounding box mask with polygonal mask
             mask[ixes] |= poly_mask
         else:
             mask = _compute_mask(region, tbl['ra'], tbl['dec'])
 
         if all(mask):
-            return None, None, None, None
+            if galaxy:
+                return None, None, None, None
+            else:
+                return None, None, None, None, None
         else:
             ra_compress = ma.array(tbl['ra'], mask=mask).compressed()
             dec_compress = ma.array(tbl['dec'], mask=mask).compressed()
             id_compress = ma.array(tbl[id_column], mask=mask).compressed()
-            return ra_compress, dec_compress, id_compress, mask
+            if galaxy:
+                return ra_compress, dec_compress, id_compress, mask
+            else:
+                object_type_compress = ma.array(tbl['object_type'],
+                                                mask=mask).compressed()
+                return ra_compress, dec_compress, id_compress, object_type_compress, mask
     else:
-        return tbl['ra'], tbl['dec'], tbl[id_column],None
+        if galaxy:
+            return tbl['ra'], tbl['dec'], tbl[id_column],None
+        else:
+            return tbl['ra'], tbl['dec'], tbl[id_column],tbl['object_type'],None
 
 def _compute_mask(region, ra, dec):
     '''
     Compute mask according to region for provided data
     Parameters
     ----------
     region         Supported shape (box, disk)  or None
@@ -234,15 +249,15 @@
             ch = logging.StreamHandler()
             ch.setLevel(loglevel)
             formatter = logging.Formatter('%(asctime)s - %(levelname)s - %(message)s')
             ch.setFormatter(formatter)
             self._logger.addHandler(ch)
 
         self._mp = mp
-        if 'schema_version' not in config:
+        if 'schema_version' not in config and 'schema_version' not in config['provenance']['versioning']:
             self._cat_dir = config['root_directory']
         else:
             sky_root = config['skycatalog_root']        # default
             if skycatalog_root:
                 sky_root = skycatalog_root
             else:
                 sky_root_env = os.getenv('SKYCATALOG_ROOT', None)
@@ -496,22 +511,22 @@
                 if the_reader in rdr_ot:
                     rdr_ot[the_reader].add(ot)
                 else:
                     rdr_ot[the_reader] = set([ot])
 
         # Now get minimal columns for objects using the readers
         galaxy_readers = []
-        star_readers = []
+        pointsource_readers = []
 
         # First make a pass to separate out the readers
         for rdr in rdr_ot:
             if 'galaxy' in rdr_ot[rdr]:
                 galaxy_readers.append(rdr)
-            elif 'star' in rdr_ot[rdr]:
-                star_readers.append(rdr)
+            elif ot in rdr_ot[rdr]:
+                pointsource_readers.append(rdr)
 
         # Make galaxy collections
         for rdr in galaxy_readers:
             if 'ra' not in rdr.columns:
                 continue
 
             # Make a collection for each row group
@@ -528,27 +543,30 @@
                                                       'galaxy', hp, self,
                                                       region=region, mask=mask,
                                                       readers=galaxy_readers,
                                                       row_group=rg)
                     object_list.append_collection(new_collection)
 
         # Make point source collection
-        for rdr in star_readers:
+        for rdr in pointsource_readers:
             if 'ra' not in rdr.columns:
                 continue
-            arrow_t = rdr.read_columns(PS_COLUMNS, None)
 
-            ra_c, dec_c, id_c, mask = _compress_via_mask(arrow_t, 'id', region)
+            # Make a collection for each row group
+            for rg in range(rdr.n_row_groups):
+                arrow_t = rdr.read_columns(PS_COLUMNS, None, rg)
+
+                ra_c, dec_c, id_c, object_type,mask = _compress_via_mask(arrow_t, 'id', region, galaxy=False)
 
-            if ra_c is not None:
-                new_collection = ObjectCollection(ra_c, dec_c, id_c,
-                                                  'star', hp, self,
-                                                  region=region, mask=mask,
-                                                  readers=star_readers)
-                object_list.append_collection(new_collection)
+                if ra_c is not None and object_type[0] in obj_type_set:
+                    new_collection = ObjectCollection(ra_c, dec_c, id_c,
+                                                      object_type[0], hp, self,
+                                                      region=region, mask=mask,
+                                                      readers=pointsource_readers, row_group=rg)
+                    object_list.append_collection(new_collection)
 
         return object_list
 
     # For generator version, do this a row group at a time
     #    but if region cut leaves too small a list, read more rowgroups
     #    to achieve a reasonable size list (or exhaust the file)
     def get_object_iterator_by_hp(self, hp, obj_type_set=None,
```

### Comparing `skyCatalogs-1.3.0/python/desc/skycatalogs/utils/SED_parquet.py` & `skyCatalogs-1.4.0rc1/python/desc/skycatalogs/utils/SED_parquet.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.3.0/python/desc/skycatalogs/utils/common_utils.py` & `skyCatalogs-1.4.0rc1/python/desc/skycatalogs/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.3.0/python/desc/skycatalogs/utils/config_utils.py` & `skyCatalogs-1.4.0rc1/python/desc/skycatalogs/utils/config_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from desc.skycatalogs.utils.exceptions import NoSchemaVersionError, ConfigDuplicateKeyError
 
 from collections import namedtuple
 
 __all__ = ['Config', 'open_config_file', 'Tophat', 'create_config',
            'assemble_SED_models', 'assemble_MW_extinction',
            'assemble_cosmology', 'assemble_object_types', 'assemble_provenance',
-           'write_yaml']
+           'assemble_variability_models', 'write_yaml', 'CURRENT_SCHEMA_VERSION']
 
-_CURRENT_SCHEMA_VERSION='1.1.0'
+CURRENT_SCHEMA_VERSION='1.2.0'
 
 def open_config_file(config_file):
     '''
     Given path to config file, return a Config object
     '''
     with open(config_file) as f:
         return Config(yaml.safe_load(f))
@@ -242,19 +242,18 @@
     Given a schema version specification, return the file path
     where the file describing it belongs
     '''
     fname = f'skycatalogs_schema_{self._cfg["schema_spec"]}'
     here = os.path.dirname(__file__)
     return os.path.join(here, '../../../../cfg', fname)
 
-def create_config(catalog_name, logname=None, schema_version=None):
-    if not schema_version:
-        schema_version = _CURRENT_SCHEMA_VERSION
-    return Config({'catalog_name' : catalog_name,
-                   'schema_version' : schema_version}, logname)
+def create_config(catalog_name, logname=None):
+    return Config({'catalog_name' : catalog_name}, logname)
+#                  'schema_version' : schema_version,
+#                  'code_version' : desc.skycatalogs.__version__}, logname)
 
 def assemble_cosmology(cosmology):
     d = {k : cosmology.__getattribute__(k) for k in ('Om0', 'Ob0', 'sigma8',
                                                      'n_s')}
     d['H0'] = float(cosmology.H0.value)
     return d
 
@@ -275,28 +274,69 @@
 
 def assemble_SED_models(bins):
     tophat_d = { 'units' : 'angstrom', 'bin_parameters' : ['start', 'width']}
     tophat_d['bins'] = bins
     file_nm_d = {'units' : 'nm'}
     return {'tophat' : tophat_d, 'file_nm' : file_nm_d}
 
-def assemble_provenance(pkg_root, inputs={}):
+def assemble_provenance(pkg_root, inputs={}, schema_version=None):
+
+    if not schema_version:
+        schema_version = CURRENT_SCHEMA_VERSION
+    import desc.skycatalogs
+    version_d = {'schema_version' : schema_version}
+    if '__version__' in dir(desc.skycatalogs):
+        code_version = desc.skycatalogs.__version__
+    else:
+        code_version = 'unknown'
+    version_d['code_version'] = code_version
+
     repo = git.Repo(pkg_root)
     has_uncommited = repo.is_dirty()
     has_untracked = (len(repo.untracked_files) > 0)
 
+
     git_d = {}
     git_d['git_hash'] = repo.commit().hexsha
     git_d['git_branch'] = repo.active_branch.name
     status = []
     if has_uncommited:
         status.append('UNCOMMITTED_FILES')
     if has_untracked:
         status.append('UNTRACKED_FILES')
     if len(status) == 0:
         status.append('CLEAN')
     git_d['git_status'] = status
 
     if inputs:
-        return {'skyCatalogs_repo' : git_d, 'inputs' : inputs}
+        return {'versioning' : version_d,'skyCatalogs_repo' : git_d,
+                'inputs' : inputs}
     else:
-        return{'skyCatalogs_repo' : git_d}
+        return{'versioning' : version_d, 'skyCatalogs_repo' : git_d}
+
+# In config just keep track of models by object type. Information
+# about the parameters they require is internal to the code.
+_AGN_MODELS = ['agn_random_walk']
+_SN_MODELS = ['sn_salt2_extended']
+
+def assemble_variability_models(object_types):
+    '''
+    Add information about all known variability models for supplied object
+    types.
+    Parameters
+    ----------
+    object_types: iterable of (pointsource) object type names
+
+    Returns
+    -------
+    A dict with object type names for keys.  Values are also dicts with
+    keys = model name and values defining struct of parameters for that
+    model, e.g. ordered dict with parameter names for keys and parameter
+    data types for values
+    '''
+    models = dict()
+    if 'agn' in object_types:
+        models['agn'] = _AGN_MODELS
+    if 'sn' in object_types:
+        models['sn'] = _SN_MODELS
+
+    return models
```

### Comparing `skyCatalogs-1.3.0/python/desc/skycatalogs/utils/exceptions.py` & `skyCatalogs-1.4.0rc1/python/desc/skycatalogs/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.3.0/python/desc/skycatalogs/utils/make_fake.py` & `skyCatalogs-1.4.0rc1/python/desc/skycatalogs/utils/make_fake.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.3.0/python/desc/skycatalogs/utils/parquet_schema_utils.py` & `skyCatalogs-1.4.0rc1/python/desc/skycatalogs/utils/parquet_schema_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pyarrow as pa
 import logging
 
-__all__ = ['make_galaxy_schema', 'make_galaxy_flux_schema', 'make_star_schema']
+__all__ = ['make_galaxy_schema', 'make_galaxy_flux_schema',
+           'make_star_schema', 'make_pointsource_schema']
 
 # This schema is not the same as the one taken from the data,
 # probably because of the indexing in the schema derived from a pandas df.
 def make_galaxy_schema(logname, sed_subdir=False, knots=True):
     fields = [pa.field('galaxy_id', pa.int64()),
               pa.field('ra', pa.float64() , True),
 ##                       metadata={"units" : "radians"}),
@@ -98,15 +99,67 @@
 def make_star_flux_schema(logname):
     '''
     Will make a separate parquet file with lsst flux for each band
     and id for joining with the main star file
     '''
     logger = logging.getLogger(logname)
     logger.debug('Creating star flux schema')
-    fields = [pa.field('id', pa.int64()),
+    fields = [pa.field('id', pa.string()),
               pa.field('lsst_flux_u', pa.float32() , True),
               pa.field('lsst_flux_g', pa.float32() , True),
               pa.field('lsst_flux_r', pa.float32() , True),
               pa.field('lsst_flux_i', pa.float32() , True),
               pa.field('lsst_flux_z', pa.float32() , True),
               pa.field('lsst_flux_y', pa.float32() , True)]
     return pa.schema(fields)
+
+def make_pointsource_schema():
+    '''
+    Ultimately should handle stars both static and variable, SN, and AGN
+    For now add everything needed for SN and put in some additional
+    star fields, but not structs for star variability models
+    '''
+
+    salt2_fields = [
+        pa.field('z', pa.float64(), True),
+        pa.field('t0', pa.float64(), True),
+        pa.field('x0', pa.float64(), True),
+        pa.field('x1', pa.float64(), True),
+        pa.field('c', pa.float64(), True)]
+    fields = [pa.field('object_type', pa.string(), False),
+              pa.field('id', pa.string(), False),
+              pa.field('ra', pa.float64(), False),
+              pa.field('dec', pa.float64(), False),
+              pa.field('host_galaxy_id', pa.int64(), True),
+              pa.field('magnorm', pa.float64(), True),
+              pa.field('sed_filepath', pa.string(), True),
+              pa.field('MW_rv', pa.float32(), True),
+              pa.field('MW_av', pa.float32(), True),
+              pa.field('mura', pa.float64(), True),
+              pa.field('mudec', pa.float64(), True),
+              pa.field('radial_velocity', pa.float64(), True),
+              pa.field('parallax', pa.float64(), True),
+              pa.field('variability_model', pa.string(), True),
+              pa.field('salt2_params', pa.struct(salt2_fields), True)
+    ]
+    return pa.schema(fields)
+
+def make_pointsource_flux_schema(logname):
+    '''
+    Will make a separate parquet file with lsst flux for each band
+    and id for joining with the main star file.
+    For static sources mjd field could be -1. Or the field could be
+    made nullable.
+    '''
+    logger = logging.getLogger(logname)
+    logger.debug('Creating pointsource flux schema')
+    fields = [pa.field('id', pa.string()),
+              pa.field('lsst_flux_u', pa.float32() , True),
+              pa.field('lsst_flux_g', pa.float32() , True),
+              pa.field('lsst_flux_r', pa.float32() , True),
+              pa.field('lsst_flux_i', pa.float32() , True),
+              pa.field('lsst_flux_z', pa.float32() , True),
+              pa.field('lsst_flux_y', pa.float32() , True),
+              pa.field('mjd', pa.float64() , True)]
+    return pa.schema(fields)
+
+    return pa.schema(fields)
```

### Comparing `skyCatalogs-1.3.0/python/desc/skycatalogs/utils/sed_tools.py` & `skyCatalogs-1.4.0rc1/python/desc/skycatalogs/utils/sed_tools.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.3.0/python/desc/skycatalogs/utils/translate_utils.py` & `skyCatalogs-1.4.0rc1/python/desc/skycatalogs/utils/translate_utils.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.3.0/python/skyCatalogs.egg-info/PKG-INFO` & `skyCatalogs-1.4.0rc1/python/skyCatalogs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skyCatalogs
-Version: 1.3.0
+Version: 1.4.0rc1
 Summary: Writes, reads catalogs input to LSST DESC simulations
 Author-email: Joanne Bogart <jrb@slac.stanford.edu>
 Keywords: desc,python,catalog,simulation
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `skyCatalogs-1.3.0/python/skyCatalogs.egg-info/SOURCES.txt` & `skyCatalogs-1.4.0rc1/python/skyCatalogs.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 python/desc/skycatalogs/utils/__init__.py
 python/desc/skycatalogs/utils/common_utils.py
 python/desc/skycatalogs/utils/config_utils.py
 python/desc/skycatalogs/utils/exceptions.py
 python/desc/skycatalogs/utils/make_fake.py
 python/desc/skycatalogs/utils/parquet_schema_utils.py
 python/desc/skycatalogs/utils/sed_tools.py
+python/desc/skycatalogs/utils/sn_tools.py
 python/desc/skycatalogs/utils/translate_utils.py
 python/skyCatalogs.egg-info/PKG-INFO
 python/skyCatalogs.egg-info/SOURCES.txt
 python/skyCatalogs.egg-info/dependency_links.txt
 python/skyCatalogs.egg-info/requires.txt
 python/skyCatalogs.egg-info/top_level.txt
 tests/test_API.py
```

### Comparing `skyCatalogs-1.3.0/tests/test_API.py` & `skyCatalogs-1.4.0rc1/tests/test_API.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.3.0/tests/test_skyCatalogs.py` & `skyCatalogs-1.4.0rc1/tests/test_skyCatalogs.py`

 * *Files identical despite different names*

