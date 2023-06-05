# Comparing `tmp/ztfidr-0.9.3.tar.gz` & `tmp/ztfidr-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ztfidr-0.9.3.tar", last modified: Wed May 24 14:01:56 2023, max compression
+gzip compressed data, was "ztfidr-0.9.4.tar", last modified: Mon Jun  5 13:32:46 2023, max compression
```

## Comparing `ztfidr-0.9.3.tar` & `ztfidr-0.9.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-24 14:01:56.242895 ztfidr-0.9.3/
--rwxrwxrwx   0 rigault   (2358) staff       (20)    11357 2022-04-07 08:06:46.000000 ztfidr-0.9.3/LICENSE
--rw-r--r--   0 rigault   (2358) staff       (20)      234 2023-05-24 14:01:56.242761 ztfidr-0.9.3/PKG-INFO
--rwxrwxrwx   0 rigault   (2358) staff       (20)     2186 2022-04-30 12:26:28.000000 ztfidr-0.9.3/README.md
--rw-r--r--   0 rigault   (2358) staff       (20)       38 2023-05-24 14:01:56.242938 ztfidr-0.9.3/setup.cfg
--rwxrwxrwx   0 rigault   (2358) staff       (20)      609 2023-05-24 14:01:27.000000 ztfidr-0.9.3/setup.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-24 14:01:56.242021 ztfidr-0.9.3/ztfidr/
--rwxrwxrwx   0 rigault   (2358) staff       (20)      127 2023-05-24 14:01:22.000000 ztfidr-0.9.3/ztfidr/__init__.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    14854 2023-05-19 12:46:56.000000 ztfidr-0.9.3/ztfidr/io.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    22044 2023-03-20 14:23:14.000000 ztfidr-0.9.3/ztfidr/lightcurve.py
--rw-r--r--   0 rigault   (2358) staff       (20)    18672 2023-05-23 08:15:23.000000 ztfidr-0.9.3/ztfidr/linefitter.py
--rw-r--r--   0 rigault   (2358) staff       (20)     3434 2023-05-24 12:50:01.000000 ztfidr-0.9.3/ztfidr/plotting.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)     1893 2022-04-07 08:06:50.000000 ztfidr-0.9.3/ztfidr/salt2.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    31049 2023-05-15 15:49:11.000000 ztfidr-0.9.3/ztfidr/sample.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)      629 2022-05-02 15:53:23.000000 ztfidr-0.9.3/ztfidr/script.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    10255 2023-05-24 11:57:29.000000 ztfidr-0.9.3/ztfidr/snid.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    21063 2023-05-15 15:36:52.000000 ztfidr-0.9.3/ztfidr/spectroscopy.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    10043 2022-11-19 14:22:02.000000 ztfidr-0.9.3/ztfidr/target.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    23610 2023-05-22 12:14:03.000000 ztfidr-0.9.3/ztfidr/typing.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)     4034 2023-03-24 07:32:25.000000 ztfidr-0.9.3/ztfidr/utils.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-24 14:01:56.242612 ztfidr-0.9.3/ztfidr.egg-info/
--rwxrwxrwx   0 rigault   (2358) staff       (20)      234 2023-05-24 14:01:56.000000 ztfidr-0.9.3/ztfidr.egg-info/PKG-INFO
--rwxrwxrwx   0 rigault   (2358) staff       (20)      377 2023-05-24 14:01:56.000000 ztfidr-0.9.3/ztfidr.egg-info/SOURCES.txt
--rwxrwxrwx   0 rigault   (2358) staff       (20)        1 2023-05-24 14:01:56.000000 ztfidr-0.9.3/ztfidr.egg-info/dependency_links.txt
--rwxrwxrwx   0 rigault   (2358) staff       (20)        7 2023-05-24 14:01:56.000000 ztfidr-0.9.3/ztfidr.egg-info/top_level.txt
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-05 13:32:46.739952 ztfidr-0.9.4/
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    11357 2022-04-07 08:06:46.000000 ztfidr-0.9.4/LICENSE
+-rw-r--r--   0 rigault   (2358) staff       (20)      234 2023-06-05 13:32:46.739821 ztfidr-0.9.4/PKG-INFO
+-rwxrwxrwx   0 rigault   (2358) staff       (20)     2186 2022-04-30 12:26:28.000000 ztfidr-0.9.4/README.md
+-rw-r--r--   0 rigault   (2358) staff       (20)       38 2023-06-05 13:32:46.739991 ztfidr-0.9.4/setup.cfg
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      609 2023-06-05 13:32:25.000000 ztfidr-0.9.4/setup.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-05 13:32:46.739021 ztfidr-0.9.4/ztfidr/
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      127 2023-06-05 13:32:21.000000 ztfidr-0.9.4/ztfidr/__init__.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    14949 2023-06-04 13:51:50.000000 ztfidr-0.9.4/ztfidr/io.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    22044 2023-03-20 14:23:14.000000 ztfidr-0.9.4/ztfidr/lightcurve.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    18672 2023-05-23 08:15:23.000000 ztfidr-0.9.4/ztfidr/linefitter.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    10098 2023-06-04 12:12:27.000000 ztfidr-0.9.4/ztfidr/plotting.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)     1893 2022-04-07 08:06:50.000000 ztfidr-0.9.4/ztfidr/salt2.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    29089 2023-06-04 14:04:07.000000 ztfidr-0.9.4/ztfidr/sample.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      629 2022-05-02 15:53:23.000000 ztfidr-0.9.4/ztfidr/script.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    10255 2023-05-24 11:57:29.000000 ztfidr-0.9.4/ztfidr/snid.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    21063 2023-05-15 15:36:52.000000 ztfidr-0.9.4/ztfidr/spectroscopy.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    10043 2022-11-19 14:22:02.000000 ztfidr-0.9.4/ztfidr/target.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    23610 2023-05-22 12:14:03.000000 ztfidr-0.9.4/ztfidr/typing.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)     4034 2023-03-24 07:32:25.000000 ztfidr-0.9.4/ztfidr/utils.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-05 13:32:46.739670 ztfidr-0.9.4/ztfidr.egg-info/
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      234 2023-06-05 13:32:46.000000 ztfidr-0.9.4/ztfidr.egg-info/PKG-INFO
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      377 2023-06-05 13:32:46.000000 ztfidr-0.9.4/ztfidr.egg-info/SOURCES.txt
+-rwxrwxrwx   0 rigault   (2358) staff       (20)        1 2023-06-05 13:32:46.000000 ztfidr-0.9.4/ztfidr.egg-info/dependency_links.txt
+-rwxrwxrwx   0 rigault   (2358) staff       (20)        7 2023-06-05 13:32:46.000000 ztfidr-0.9.4/ztfidr.egg-info/top_level.txt
```

### Comparing `ztfidr-0.9.3/LICENSE` & `ztfidr-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.3/README.md` & `ztfidr-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.3/setup.py` & `ztfidr-0.9.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 from distutils.core import setup
 from setuptools import setup, find_packages
 
 
 packages = find_packages()
 
-VERSION = '0.9.3'
+VERSION = '0.9.4'
         
 setup(name='ztfidr',
       version=VERSION,
       description='Tools for ZTF Ia *Internal*DataReleases',
       author='Mickael Rigault',
       author_email='m.rigault@ipnl.in2p3.fr',
       url='https://github.com/MickaelRigault/ztfdr',
```

### Comparing `ztfidr-0.9.3/ztfidr/io.py` & `ztfidr-0.9.4/ztfidr/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,56 +145,54 @@
     # or get them all:
     redshift_dir = os.path.join(IDR_PATH, "tables", ".dataset_creation/redshifts")
     redshifts = {}
 
     
     # Emission lines
     sedm_em = pandas.read_csv(os.path.join(redshift_dir,
-                                            "specfile_sedm_emissionlines.csv"),
+                                            "ztfdr2_sedmhanii_redshift.csv"),
                                   index_col=0)
-    sedm_em = sedm_em.set_index("ztfname")[["sedmredshift","sedmredshift_err"]].copy()#.rename("sedmredshift","sedm_em", axis=1)
-    sedm_em.columns = sedm_em.columns.str.replace("sedmredshift","sedm_em")
+    sedm_em.columns = sedm_em.columns.str.replace("redshift","sedm")
     
     
     
     nosedm_em = pandas.read_csv(os.path.join(redshift_dir,
-                                                    "specfile_nonsedm_emissionlines.csv"),
+                                                    "ztfdr2_nonsedmhanii_redshift.csv"),
                                      index_col=0)
-    nosedm_em = nosedm_em.set_index("ztfname")[["value","error"]].copy()#.rename("sedmredshift","sedm_em", axis=1)
-    nosedm_em.columns = ["nonsedm_em", "nonsedm_em_err"]
+    nosedm_em.columns = nosedm_em.columns.str.replace("redshift","nonsedm")
     
     # SNID
     snidauto = pandas.read_csv(os.path.join(redshift_dir,
                                                     "ztfdr2_snid_redshifts.csv"),
                                      index_col=0)
-    snidauto.columns = snidauto.columns.str.replace("redshift","snidauto")
+    snidauto.columns = snidauto.columns.str.replace("redshift", "snid")
     
     # Host-Z
     hostz = pandas.read_csv(os.path.join(redshift_dir,
-                                                    "ztfdr2_hostz_redshifts.csv"),
+                                                    "ztfdr2_galcat_redshifts.csv"),
                                      index_col=0)
-    hostz = hostz[["redshift"]]
-    hostz.columns = ["host_cat"]
-    hostz["host_cat_err"] = 1e-5
+    hostz = hostz[["z"]]
+    hostz.columns = ["gal"]
+    hostz["gal_err"] = 1e-5
 
 
     
     # override
-    override = pandas.read_csv(os.path.join(redshift_dir,
-                                                    "ztfdr2_override_redshifts.csv"),
-                                     index_col=0)
-    override.columns = ["override"]
+#    override = pandas.read_csv(os.path.join(redshift_dir,
+#                                                    "ztfdr2_override_redshifts.csv"),
+#                                     index_col=0)
+#    override.columns = ["override"]
 
     # merge them
     
     data = data.join(sedm_em, on="ztfname")
     data = data.join(nosedm_em, on="ztfname")
     data = data.join(snidauto, on="ztfname")
     data = data.join(hostz, on="ztfname")
-    data = data.join(override, on="ztfname")
+ #   data = data.join(override, on="ztfname")
     data
     
     return data
     
 def get_snidauto_redshift(load=True, **kwargs):
     """ """
     filepath = os.path.join(IDR_PATH,"tables",
@@ -323,27 +321,25 @@
             return None
 
     return fullpath
 
 
 def get_phase_coverage(load=True, warn=True, **kwargs):
     """ """
-    filepath = os.path.join(IDR_PATH, "tables", "phase_coverage.csv")
+    filepath = os.path.join(IDR_PATH, "tables", "phase_coverage.parquet")
     if not load:
         return filepath
 
     if not os.path.isfile(filepath):
         if warn:
             warnings.warn(
                 "No phase_coverage file. build one using ztfidr.Sample().build_phase_coverage(store=True)")
         return None
 
-    return pandas.read_csv(filepath, index_col=0, **kwargs
-                           ).reset_index().rename({"index": "name"}, axis=1
-                                                  ).set_index(["name", "filter"])["phase"]
+    return pandas.read_parquet(filepath, **kwargs)#.set_index(["ztfname", "filter"])
 
 
 # ================== #
 #                    #
 #   Spectra          #
 #                    #
 # ================== #
@@ -352,14 +348,24 @@
     filepath = os.path.join(IDR_PATH, "tables",
                             ".dataset_creation/sample_def/spec_class/autotyping.csv")
     if not load:
         return filepath
     return pandas.read_csv(filepath, index_col=index_col, **kwargs)
 
 
+def get_lightcurve_datafile(contains=None):
+    """ """
+    from glob import glob
+    glob_format = "*" if contains is None else f"*{contains}*"
+    files = glob(os.path.join(IDR_PATH, "lightcurves", glob_format))
+    datafile = pandas.DataFrame(files, columns=["fullpath"])
+    datafile["basename"] = datafile["fullpath"].str.split(pat="/", expand=True).iloc[:, -1]
+    datafile["ztfname"] = datafile["basename"].str.split(pat="_", expand=True).iloc[:, 0]
+    return datafile
+    
 def get_spectra_datafile(contains=None, startswith=None,
                          snidres=False, extension=None, use_dask=False,
                          add_phase=True, data=None):
     """ """
     from glob import glob
     glob_format = "*" if not startswith else f"{startswith}*"
     if snidres and extension is None:
```

### Comparing `ztfidr-0.9.3/ztfidr/lightcurve.py` & `ztfidr-0.9.4/ztfidr/lightcurve.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.3/ztfidr/linefitter.py` & `ztfidr-0.9.4/ztfidr/linefitter.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.3/ztfidr/salt2.py` & `ztfidr-0.9.4/ztfidr/salt2.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.3/ztfidr/sample.py` & `ztfidr-0.9.4/ztfidr/sample.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,26 @@
 from . import io
 from astropy import time
         
 def get_sample(**kwargs):
     """ Short to to Sample.load() """
     return Sample.load(**kwargs)
 
+def _get_coverage_(phase_df, prefix=None):
+    """ """
+    if prefix is None:
+        prefix = ""
+
+    n_points  = phase_df.groupby(level=0).size().to_frame(f"n_{prefix}points")
+    n_bands   = ((phase_df.groupby(level=[0,1]).size()>0).groupby(level=0).sum()).to_frame(f"n_{prefix}bands")
+    n_points_g = phase_df.xs("ztfg", level=1).groupby(level=0).size().to_frame(f"n_{prefix}points_ztfg")
+    n_points_r = phase_df.xs("ztfr", level=1).groupby(level=0).size().to_frame(f"n_{prefix}points_ztfr")
+    n_points_i = phase_df.xs("ztfi", level=1).groupby(level=0).size().to_frame(f"n_{prefix}points_ztfi")
+    dfs = [n_points, n_bands, n_points_g, n_points_r, n_points_i]
+    return pandas.concat(dfs, axis=1).fillna(0).astype( int )
 
 class Sample():
 
     
     def __init__(self, data=None):
         """ """
         self.set_data(data)
@@ -102,15 +114,15 @@
                 rebuild = True
                 
         if rebuild:
             phase_df = self.build_phase_coverage(min_detection=min_detection,
                                                     groupby=groupby,
                                                     client=client, store=True, **kwargs)
         self._phase_df = phase_df
-
+        
     def load_fiedid(self):
         """ compute the fields containing the targets using 
         ztfquery.fields.get_fields_containing_target().
         This take quite some time.
 
         the 'fieldid' entry is added to self.data
         """
@@ -151,19 +163,21 @@
                                  **kwargs})
         
     # ------- #
     # GETTER  #
     # ------- #
     def get_data(self, clean_t0nan=True,
                      t0_range=None, x1_range=None, c_range=None,
-                     redshift_range=None, z_quality=None, redshift_source=None,
+                     redshift_range=None,
+                     redshift_source=None,
                      t0_err_range=None, c_err_range=None, x1_err_range=None,
                      exclude_targets=None, in_targetlist=None,
                      ndetections=None,
                      goodcoverage=None, coverage_prop={},
+                     classification=None,
                      first_spec_phase=None, query=None, data=None):
         """ 
         *_range: [None or [min, max]] -optional-
             cut to be applied to the data for
             t0, x1, c, (and there error) and redshift.
             boundaries are mandatory. For instance, redshift range lower than 0.06
             should be: redshift_range = (0, 0.06).
@@ -234,19 +248,21 @@
         # Redshift Cuts
         # - Redshift range
         if redshift_range is not None:
             data = data[data["redshift"].between(*redshift_range)]
             
         # -  redshift origin
         if redshift_source is not None:
-            data = data[data["redshift"].isin(*np.atleast_1d(redshift_source))]
-            
-        if z_quality is not None and z_quality not in ["any","all","*"]:
-            data = data[data["z_quality"].isin(np.atleast_1d(z_quality))]
+            data = data[data["source"].isin(np.atleast_1d(redshift_source))]
+
 
+        # Classification
+        if classification is not None:
+            data = data[data["classification"].isin(np.atleast_1d(classification))]
+            
         # Target cuts
         # - in given list
         if in_targetlist is not None:
             data = data.loc[np.asarray(in_targetlist)[np.in1d(in_targetlist, data.index.astype("string"))] ]
 
         if exclude_targets is not None:
             data = data.loc[~data.index.isin(exclude_targets)]
@@ -276,27 +292,31 @@
 
         # Additional Query
         if query:
             data = data.query(query)
             
         return data
 
-    def get_ianorm(self, incl_snia=False):
-        """ get the list targets that are ia-norm (or sn ia if incl_snia=True)
+    def get_phases(self, one_per_day=False,
+                         phase_range=None,
+                         detection=5):
+        """ """
+        if detection is not None:
+            phase_df = self.phase_df[(self.phase_df["detection"]>detection)]["phase"].copy()
+        else:
+            phase_df = self.phase_df["phase"]
         
-        Returns
-        -------
-        array
-            list of targetname (data.index)
-        """        
-        classifications = ["snia-norm"]
-        if incl_snia:
-            classifications += ["snia"]
+        if one_per_day:
+            phase_df = phase_df.astype(int).reset_index().drop_duplicates().set_index(["ztfname","filter"])["phase"]
+            
+        if phase_range is not None:
+            phase_df = phase_df[phase_df.between(*phase_df)]
             
-        return np.asarray(self.data[self.data["classification"].isin(classifications)].index)
+        return phase_df
+                                    
     
     # Target | High level
     def get_target(self, name):
         """ """
         from . import target
         lightcurve = self.get_target_lightcurve(name)
         spectra = self.get_target_spectra(name, as_spectra=False)
@@ -319,123 +339,69 @@
     # Spectrum
     def get_target_spectra(self, name, **kwargs):
         """ Get a list with all the Spectra for the given object """
         from . import spectroscopy
         return spectroscopy.Spectrum.from_name(name, **kwargs)
 
     # Extra
-    def get_goodcoverage_targets(self,
-                                     n_early_bands=">=2",
-                                     n_late_bands=">=2",
-                                       n_points=">=7",
-                                       premax_range=[-20,0],
-                                       postmax_range=[0,40],
-                                       phase_range=[-20,30],
-                                       **kwargs):
+    def get_goodcoverage_targets(self, premax_range = [-15,0],
+                                       postmax_range = [0,45],
+                                       phase_range = [-15,45],
+                                      **kwargs):
         """ kwargs should have the same format as the n_early_point='>=2' for instance.
         None means no constrain, like n_bands=None means 'n_bands' is not considered.
         """
-        query = {**dict(n_early_bands=n_early_bands, n_late_bands=n_late_bands,
-                        n_points=n_points),
+        query = {**dict(n_late_bands=">=2", n_points=">=7", n_early_points=">=2"),
                  **kwargs}
         df_query = " and ".join([f"{k}{v}" for k,v in query.items() if v is not None])
-        phase_coverage = self.get_phase_coverage(premax_range=premax_range,
-                                                 postmax_range=postmax_range,
-                                                 phase_range=phase_range)
-        return phase_coverage.query(df_query).index.astype("string")
 
+        phase_coverage = self.get_phase_coverage(premax_range = premax_range,
+                                                 postmax_range = postmax_range,
+                                                 phase_range = phase_range)
+        return phase_coverage.query(df_query).index.astype("string")
     
-    def get_phase_coverage(self,premax_range=[-20,0],
-                                postmax_range=[0,40],
-                                phase_range=[-20,40], min_det_perband=1):
-        """ """        
-        # All
-        phases = self.phase_df[self.phase_df.between(*phase_range)].reset_index().rename({"level_0":"name"},axis=1)
-        n_points = phases.groupby(["name"]).size().to_frame("n_points")
-        n_bands = (phases.groupby(["name", "filter"]).size()>=min_det_perband
-                        ).groupby(level=[0]).sum().to_frame("n_bands")
-        # Pre-Max
-        # - AnyBand
-        premax = self.phase_df[self.phase_df.between(*premax_range)].reset_index().rename({"level_0":"name"},axis=1)
-        n_early_points = premax.groupby(["name"]).size().to_frame("n_early_points")
-        n_early_bands = (premax.groupby(["name", "filter"]).size()>=min_det_perband
-                        ).groupby(level=[0]).sum().to_frame("n_early_bands")
-        # - Per filters
-        n_early_points_perfilter = premax.groupby(["name", "filter"]).size()
-        n_early_points_g = n_early_points_perfilter.xs("p48g", level=1).to_frame("n_early_points_p48g")
-        n_early_points_r = n_early_points_perfilter.xs("p48r", level=1).to_frame("n_early_points_p48r")
-        n_early_points_i = n_early_points_perfilter.xs("p48i", level=1).to_frame("n_early_points_p48i")
-        
-        # Post-Max
-        # - AnyBand        
-        postmax = self.phase_df[self.phase_df.between(*postmax_range)].reset_index().rename({"level_0":"name"},axis=1)
-        n_late_points = postmax.groupby(["name"]).size().to_frame("n_late_points")
-        n_late_bands = (postmax.groupby(["name", "filter"]).size()>=min_det_perband
-                       ).groupby(level=[0]).sum().to_frame("n_late_bands")
-        # - Per filters
-        n_late_points_perfilter = postmax.groupby(["name", "filter"]).size()
-        n_late_points_g = n_late_points_perfilter.xs("p48g", level=1).to_frame("n_late_points_p48g")
-        n_late_points_r = n_late_points_perfilter.xs("p48r", level=1).to_frame("n_late_points_p48r")
-        n_late_points_i = n_late_points_perfilter.xs("p48i", level=1).to_frame("n_late_points_p48i")
-            
-        return pandas.concat([n_points,n_bands,
-                              n_early_points,n_early_bands,n_late_points, n_late_bands,
-                              n_early_points_g, n_early_points_r, n_early_points_i,
-                              n_late_points_g, n_late_points_r, n_late_points_i], axis=1).fillna(0).astype(int)
+    def get_phase_coverage(self, premax_range = [-15,0],
+                                 postmax_range = [0,45],
+                                 phase_range = [-15,45],
+                                 one_per_day=True):
+        """ """
 
+        phase_df = self.get_phases(one_per_day)
         
-    def build_phase_coverage(self, min_detection=5, groupby='filter', client=None, store=True, **kwargs):
+        dfs = _get_coverage_( phase_df[phase_df.between(*phase_range)] )
+        dfs_early = _get_coverage_(phase_df[phase_df.between(*premax_range)], prefix="early_")
+        dfs_late = _get_coverage_(phase_df[phase_df.between(*postmax_range)], prefix="late_")
+        return pandas.concat([dfs, dfs_early, dfs_late], axis=1).reindex(self.data.index).fillna(0).astype(int)
+        
+    def build_phase_coverage(self, groupby='filter', client=None, store=True, **kwargs):
         """ 
         time: 
         - Dask: 45s on a normal laptop | 4 cores 
         - No Dask: 60s on a normal laptop | 4 cores 
         """
+        warnings.warn("building phase coverage takes ~30s.")
+        
         import pandas
         import dask
         from . import lightcurve
-
+        from . import io
         phases = []
-        datalc = self.get_data()
-        datalc = datalc[datalc["redshift"].between(-0.1,0.2)]
-
-        warnings.warn("building phase coverage takes ~30s to 1min.")
-        # - Without Dask
-        if client is None:
-            warnings.warn("loading without Dask (client is None) ; it will be slow")
-            names_ok = []
-            for name in datalc.index:
-                try:
-                    dt = lightcurve.LightCurve.from_name(name)
-                    phases.append( dt.get_obsphase(min_detection=min_detection, groupby=groupby, **kwargs))
-                    names_ok.append(name)
-                except:
-                    warnings.warn(f"get_obsphase did not work for {name}")
-                    continue
-                
-            phase_df = pandas.concat(phases, keys=names_ok)
-
-        # - With Dask
-        else:
-            for name in datalc.index:
-                dt = dask.delayed(lightcurve.LightCurve.from_name)(name)
-                phases.append( dt.get_obsphase(min_detection=min_detection, groupby=groupby, **kwargs)
-                             )
-
-            fphases = client.compute(phases)
-            data_ = client.gather(fphases, "skip") # wait until all is done
-            names = datalc.index[[i for i,f_ in enumerate(fphases) if f_.status=="finished"]]
-            
-            phase_df = pandas.concat(data_, keys=names)
-
-        phase_df_exploded = phase_df.explode()
+        data = self.get_data()
+        
+        lcdata = io.get_lightcurve_datafile().set_index("ztfname").loc[data.index]
+        dfs = pandas.concat([pandas.read_csv(f_, delim_whitespace=True, comment='#') for f_ in lcdata["fullpath"]],
+                                keys=data.index)
+        dfs["phase"] = dfs["mjd"] - data["t0"].reindex(dfs.index, level=0)
+        dfs["detection"] = dfs["flux"]/dfs["flux_err"]
+        phase_df = dfs.reset_index().set_index(["ztfname","filter"])[["phase","detection"]]
         if store:
             filepath = io.get_phase_coverage(load=False)
-            phase_df_exploded.to_csv(filepath)
+            phase_df.to_parquet(filepath)
             
-        return phase_df_exploded
+        return phase_df
     
     
     # ------- #
     # PLOTTER #
     # ------- #
     def show_ideogram(self, key, keyerr=None,
                           ax=None, data=None, dataprop={},
@@ -724,15 +690,15 @@
 
         axt.set_xlim(*axb.get_xlim())
         return fig
 
 
     def show_firstdet_distributions(self, ax=None, restrict_to=[-25,60]):
         """ """
-        phases = self.phase_df[self.phase_df.between(*restrict_to)]
+        phases = self.get_phases(phase_range=restrict_to)
         goodlc = self.get_goodcoverage_targets()
 
         from matplotlib.colors import to_rgba
         if ax is None:
             import matplotlib.pyplot as plt
             fig = plt.figure(figsize=[7, 2.5])
             ax = fig.add_axes([0.08, 0.1, 0.87, 0.8])
@@ -794,16 +760,15 @@
 
     @property
     def hostdata(self):
         """ """
         if not hasattr(self, "_hostdata"):
             self.load_hostdata()
         return self._hostdata
-
-
+    
     @property
     def phase_df(self):
         """ """
         if not hasattr(self, "_phase_df"):
             self.load_phase_df()
         
         return self._phase_df
```

### Comparing `ztfidr-0.9.3/ztfidr/script.py` & `ztfidr-0.9.4/ztfidr/script.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.3/ztfidr/snid.py` & `ztfidr-0.9.4/ztfidr/snid.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.3/ztfidr/spectroscopy.py` & `ztfidr-0.9.4/ztfidr/spectroscopy.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.3/ztfidr/target.py` & `ztfidr-0.9.4/ztfidr/target.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.3/ztfidr/typing.py` & `ztfidr-0.9.4/ztfidr/typing.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.9.3/ztfidr/utils.py` & `ztfidr-0.9.4/ztfidr/utils.py`

 * *Files identical despite different names*

