# Comparing `tmp/SFcalculator_torch-0.1.7.tar.gz` & `tmp/SFcalculator_torch-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SFcalculator_torch-0.1.7.tar", last modified: Wed Apr  5 18:48:18 2023, max compression
+gzip compressed data, was "SFcalculator_torch-0.1.8.tar", last modified: Mon Jun  5 13:08:35 2023, max compression
```

## Comparing `SFcalculator_torch-0.1.7.tar` & `SFcalculator_torch-0.1.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 18:48:18.566742 SFcalculator_torch-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-05 18:48:06.000000 SFcalculator_torch-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-05 18:48:18.566742 SFcalculator_torch-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-05 18:48:06.000000 SFcalculator_torch-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 18:48:18.562741 SFcalculator_torch-0.1.7/SFC_Torch/
--rw-r--r--   0 runner    (1001) docker     (123)    46295 2023-04-05 18:48:06.000000 SFcalculator_torch-0.1.7/SFC_Torch/Fmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-05 18:48:06.000000 SFcalculator_torch-0.1.7/SFC_Torch/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-05 18:48:06.000000 SFcalculator_torch-0.1.7/SFC_Torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10111 2023-04-05 18:48:06.000000 SFcalculator_torch-0.1.7/SFC_Torch/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-04-05 18:48:06.000000 SFcalculator_torch-0.1.7/SFC_Torch/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-05 18:48:06.000000 SFcalculator_torch-0.1.7/SFC_Torch/packingscore.py
--rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-04-05 18:48:06.000000 SFcalculator_torch-0.1.7/SFC_Torch/patterson.py
--rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-04-05 18:48:06.000000 SFcalculator_torch-0.1.7/SFC_Torch/symmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     9482 2023-04-05 18:48:06.000000 SFcalculator_torch-0.1.7/SFC_Torch/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-04-05 18:48:06.000000 SFcalculator_torch-0.1.7/SFC_Torch/voxel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 18:48:18.566742 SFcalculator_torch-0.1.7/SFcalculator_torch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-05 18:48:18.000000 SFcalculator_torch-0.1.7/SFcalculator_torch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-05 18:48:18.000000 SFcalculator_torch-0.1.7/SFcalculator_torch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 18:48:18.000000 SFcalculator_torch-0.1.7/SFcalculator_torch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-05 18:48:18.000000 SFcalculator_torch-0.1.7/SFcalculator_torch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-05 18:48:18.000000 SFcalculator_torch-0.1.7/SFcalculator_torch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-05 18:48:06.000000 SFcalculator_torch-0.1.7/license
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-05 18:48:18.566742 SFcalculator_torch-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-05 18:48:06.000000 SFcalculator_torch-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 18:48:18.566742 SFcalculator_torch-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 18:48:06.000000 SFcalculator_torch-0.1.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-05 18:48:06.000000 SFcalculator_torch-0.1.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-05 18:48:06.000000 SFcalculator_torch-0.1.7/tests/test_Fmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-05 18:48:06.000000 SFcalculator_torch-0.1.7/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-05 18:48:06.000000 SFcalculator_torch-0.1.7/tests/test_patterson.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-04-05 18:48:06.000000 SFcalculator_torch-0.1.7/tests/test_voxel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:08:35.624087 SFcalculator_torch-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-05 13:08:20.000000 SFcalculator_torch-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-05 13:08:35.624087 SFcalculator_torch-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-05 13:08:20.000000 SFcalculator_torch-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:08:35.624087 SFcalculator_torch-0.1.8/SFC_Torch/
+-rw-r--r--   0 runner    (1001) docker     (123)    50763 2023-06-05 13:08:20.000000 SFcalculator_torch-0.1.8/SFC_Torch/Fmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 13:08:20.000000 SFcalculator_torch-0.1.8/SFC_Torch/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-05 13:08:20.000000 SFcalculator_torch-0.1.8/SFC_Torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10111 2023-06-05 13:08:20.000000 SFcalculator_torch-0.1.8/SFC_Torch/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-06-05 13:08:20.000000 SFcalculator_torch-0.1.8/SFC_Torch/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-05 13:08:20.000000 SFcalculator_torch-0.1.8/SFC_Torch/packingscore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-06-05 13:08:20.000000 SFcalculator_torch-0.1.8/SFC_Torch/patterson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-06-05 13:08:20.000000 SFcalculator_torch-0.1.8/SFC_Torch/symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9482 2023-06-05 13:08:20.000000 SFcalculator_torch-0.1.8/SFC_Torch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-06-05 13:08:20.000000 SFcalculator_torch-0.1.8/SFC_Torch/voxel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:08:35.624087 SFcalculator_torch-0.1.8/SFcalculator_torch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-05 13:08:35.000000 SFcalculator_torch-0.1.8/SFcalculator_torch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-05 13:08:35.000000 SFcalculator_torch-0.1.8/SFcalculator_torch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:08:35.000000 SFcalculator_torch-0.1.8/SFcalculator_torch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-05 13:08:35.000000 SFcalculator_torch-0.1.8/SFcalculator_torch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-05 13:08:35.000000 SFcalculator_torch-0.1.8/SFcalculator_torch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-05 13:08:20.000000 SFcalculator_torch-0.1.8/license
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-05 13:08:35.624087 SFcalculator_torch-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-05 13:08:20.000000 SFcalculator_torch-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:08:35.624087 SFcalculator_torch-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 13:08:20.000000 SFcalculator_torch-0.1.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-05 13:08:20.000000 SFcalculator_torch-0.1.8/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-06-05 13:08:20.000000 SFcalculator_torch-0.1.8/tests/test_Fmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-05 13:08:20.000000 SFcalculator_torch-0.1.8/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-06-05 13:08:20.000000 SFcalculator_torch-0.1.8/tests/test_patterson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-06-05 13:08:20.000000 SFcalculator_torch-0.1.8/tests/test_voxel.py
```

### Comparing `SFcalculator_torch-0.1.7/README.md` & `SFcalculator_torch-0.1.8/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -11,7 +11,16 @@
 
 2. Install [Pytorch](https://pytorch.org/get-started/locally/)
 
 3. Install `SFcalculator-torch`
     ```bash
     pip install SFcalculator-torch
     ```
+ 
+### Citation
+
+We are in the process of writing a paper about this work, if you are interested in using the tool, please contact the authors for a discussion at the first place
+
+Minhuan Li, minhuanli@g.harvard.edu
+
+Doeke Hekstra, doeke_hekstra@harvard.edu
+
```

### Comparing `SFcalculator_torch-0.1.7/SFC_Torch/Fmodel.py` & `SFcalculator_torch-0.1.8/SFC_Torch/Fmodel.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         self,
         PDBfile_dir,
         mtzfile_dir=None,
         dmin=None,
         anomalous=False,
         wavelength=None,
         set_experiment=True,
-        nansubset=["FP", "SIGFP"],
+        expcolumns=["FP", "SIGFP"],
         freeflag="FreeR_flag",
         testset_value=0,
     ):
         """
         Initialize with necessary reusable information, like spacegroup, unit cell info, HKL_list, et.c.
 
         Parameters:
@@ -61,19 +61,19 @@
         anomalous: Boolean, default False
             Whether or not to include anomalous scattering in the calculation
 
         wavelength: None or float
             The wavelength of scattering source in A
 
         set_experiment: Boolean, default True
-            Whether or not to set Fo and SigF, r_free, r_work from the experimental mtz file. It only works when
+            Whether or not to set Fo, SigF, free_flag and Outlier from the experimental mtz file. It only works when
             the mtzfile_dir is not None
 
-        nansubset: list of str, default ['FP', 'SIGFP']
-            list of column names to examine the nan values
+        expcolumns: list of str, default ['FP', 'SIGFP']
+            list of column names used as expeimental data
         """
         structure = gemmi.read_pdb(PDBfile_dir)  # gemmi.Structure object
         self.unit_cell = structure.cell  # gemmi.UnitCell object
         self.space_group = gemmi.SpaceGroup(
             structure.spacegroup_hm
         )  # gemmi.SpaceGroup object
         self.operations = self.space_group.operations()  # gemmi.GroupOps object
@@ -109,17 +109,17 @@
             device=try_gpu(),
         ).type(torch.float32)
 
         # Generate ASU HKL array and Corresponding d*^2 array
         if mtzfile_dir:
             mtz_reference = rs.read_mtz(mtzfile_dir)
             try:
-                mtz_reference.dropna(axis=0, subset=nansubset, inplace=True)
+                mtz_reference.dropna(axis=0, subset=expcolumns, inplace=True)
             except:
-                raise ValueError(f"{nansubset} columns not included in the mtz file!")
+                raise ValueError(f"{expcolumns} columns not included in the mtz file!")
             if anomalous:
                 # Try to get the wavelength from MTZ file
                 try:
                     mtz_wavelength = mtz_reference.dataset(0).wavelength
                     assert mtz_wavelength > 0.05
                     if self.wavelength is not None:
                         assert np.isclose(mtz_wavelength, self.wavelength, atol=0.05)
@@ -145,16 +145,18 @@
             assert (
                 diff_array(self.HKL_array, self.Hasu_array) == set()
             ), "HKL_array should be equal or subset of the Hasu_array!"
             self.asu2HKL_index = asu2HKL(self.Hasu_array, self.HKL_array)
             # d*^2 array according to the HKL list, [N]
             self.dr2asu_array = self.unit_cell.calculate_1_d2_array(self.Hasu_array)
             self.dr2HKL_array = self.unit_cell.calculate_1_d2_array(self.HKL_array)
+            # assign reslution bins
+            self.assign_resolution_bins()
             if set_experiment:
-                self.set_experiment(mtz_reference, freeflag, testset_value)
+                self.set_experiment(mtz_reference, expcolumns, freeflag, testset_value)
         else:
             if not dmin:
                 raise ValueError(
                     "high_resolution dmin OR a reference mtz file should be provided!"
                 )
             else:
                 self.dmin = dmin
@@ -162,14 +164,15 @@
                     self.unit_cell, self.space_group, self.dmin
                 )
                 self.dHasu = self.unit_cell.calculate_d_array(self.Hasu_array).astype(
                     "float32"
                 )
                 self.dr2asu_array = self.unit_cell.calculate_1_d2_array(self.Hasu_array)
                 self.HKL_array = None
+                self.assign_resolution_bins()
 
         self.orth2frac_tensor = torch.tensor(
             self.unit_cell.fractionalization_matrix.tolist(), device=try_gpu()
         ).type(torch.float32)
         self.frac2orth_tensor = torch.tensor(
             self.unit_cell.orthogonalization_matrix.tolist(), device=try_gpu()
         ).type(torch.float32)
@@ -259,53 +262,71 @@
         else:
             self.fullsf_tensor = torch.tensor(
                 np.array([self.full_atomic_sf_asu[atom] for atom in self.atom_name]),
                 device=try_gpu(),
             ).type(torch.float32)
         self.inspected = False
 
-    def set_experiment(self, exp_mtz, freeflag="FreeR_flag", testset_value=0):
+    def set_experiment(self, exp_mtz, expcolumns=["FP", "SIGFP"], freeflag="FreeR_flag", testset_value=0):
         """
-        Set experimental data in the refinement
+        Set experimental data for refinement,
+        including Fo, SigF, free_flag, Outlier
 
         exp_mtz, rs.Dataset, mtzfile read by reciprocalspaceship
         """
         try:
-            self.Fo = torch.tensor(exp_mtz["FP"].to_numpy(), device=try_gpu()).type(
+            self.Fo = torch.tensor(exp_mtz[expcolumns[0]].to_numpy(), device=try_gpu()).type(
                 torch.float32
             )
             self.SigF = torch.tensor(
-                exp_mtz["SIGFP"].to_numpy(), device=try_gpu()
+                exp_mtz[expcolumns[1]].to_numpy(), device=try_gpu()
             ).type(torch.float32)
         except:
-            print("MTZ file doesn't contain 'FP' or 'SIGFP'! Check your data!")
+            print(f"MTZ file doesn't contain {expcolumns[0]} or {expcolumns[1]}! Check your data!")
+
         try:
             self.free_flag = np.where(
                 exp_mtz[freeflag].values == testset_value, True, False
             )
         except:
             print("No Free Flag! Check your data!")
 
+        # label outliers
+        exp_mtz.label_centrics(inplace=True)
+        exp_mtz.compute_multiplicity(inplace=True)
+        exp_mtz["SIGN"] = 0.0
+        for i in range(self.n_bins):
+            index_i = self.bins == i
+            exp_mtz.loc[index_i, "SIGN"] = np.mean(
+                exp_mtz[index_i]["FP"].to_numpy() ** 2
+                / exp_mtz[index_i]["EPSILON"].to_numpy()
+            )
+        exp_mtz["EP"] = exp_mtz["FP"] / np.sqrt(exp_mtz["EPSILON"] * exp_mtz["SIGN"])
+        self.Outlier = (
+            (exp_mtz["CENTRIC"] & (exp_mtz["EP"] > 4.89))
+            | ((~exp_mtz["CENTRIC"]) & (exp_mtz["EP"] > 3.72))
+        ).to_numpy(dtype=bool)
+
     def assign_resolution_bins(
-        self, bins=10, Nmin=100, return_labels=True, format_str=".2f"
+        self, bins=10, Nmin=100, return_labels=False, format_str=".2f"
     ):
         """Assign reflections in HKL_array to resolution bins with logarithmic algorithm.
         The labels will be stored in self.bins
 
         Urzhumtsev, A., et al. Acta Crystallographica Section D: Biological Crystallography 65.12 (2009)
 
         Parameters
         ----------
         bins : int, optional
             Number of bins, by default 10
         Nmin : int, optional
             Minimum number of reflections for the first two low-resolution ranges, by default 100
         return_labels : bool, optional
             Whether to return a list of labels corresponding to the edges
-            of each resolution bin, by default True
+            of each resolution bin, by default False
         format_str : str, optional
             Format string for constructing bin labels, by default ".2f"
 
         Returns
         -------
         None or list of labels
         """
@@ -313,27 +334,27 @@
             assert hasattr(
                 self, "dHKL"
             ), "Must have resolution stored in dHKL attribute!"
             d = self.dHKL
         else:
             assert hasattr(
                 self, "dHasu"
-            ), "Must have resolution stored in dHKL attribute!"
+            ), "Must have resolution stored in dHasu attribute!"
             d = self.dHasu
         assignments, edges = bin_by_logarithmic(d, bins, Nmin)
         self.n_bins = bins
         self.bins = assignments
         self.bin_labels = [
             f"{e1:{format_str}} - {e2:{format_str}}"
             for e1, e2 in zip(edges[:-1], edges[1:])
         ]
         if return_labels:
             return self.bin_labels
 
-    def inspect_data(self, verbose=True):
+    def inspect_data(self, verbose=False):
         """
         Do an inspection of data, for hints about
         1. solvent percentage for mask calculation
         2. suitable grid size
         """
         # solvent percentage
         vdw_rad = vdw_rad_tensor(self.atom_name)
@@ -527,15 +548,15 @@
             self.Fprotein_HKL.conj() * self.Fmask_HKL
             + self.Fprotein_HKL * self.Fmask_HKL.conj()
         )
         us = torch.abs(self.Fprotein_HKL).pow(2)
         Is = self.Fo.pow(2)
 
         for bin_i in np.sort(np.unique(self.bins)):
-            index_i = (~self.free_flag) & (self.bins == bin_i)
+            index_i = (~self.free_flag) & (self.bins == bin_i) & (~self.Outlier)
 
             C2 = torch.sum(ws[index_i] * Is[index_i])
             B2 = 2.0 * torch.sum(vs[index_i] * Is[index_i])
             A2 = torch.sum(us[index_i] * Is[index_i])
             Y2 = torch.sum(Is[index_i].pow(2))
             # They made this wrong in their original paper
             D3 = torch.sum(ws[index_i].pow(2))
@@ -602,45 +623,42 @@
 
             kmasks.append(kmask.requires_grad_(requires_grad))
             kisos.append(kiso.requires_grad_(requires_grad))
         return kmasks, kisos
 
     def _init_uaniso(self, requires_grad=True):
         """
-        Use the analytical solutuon discussed to initialize Uaniso
+        Use the analytical solutuon discussed to initialize Uaniso per resolution bin
         Afonine, P. V., et al. Acta Crystallographica Section D: Biological Crystallography 69.4 (2013): 625-634.
 
         Note: Only work when you have mtz data, self.Fo
         """
-        s = self.HKL_array
-        V = np.concatenate([s**2, 2 * s[:, [0, 2, 1]] * s[:, [1, 0, 2]]], axis=-1)
-        Z = np.zeros((len(s),))
+        uanisos = []
         for bin_i in np.sort(np.unique(self.bins)):
-            index_i = self.bins == bin_i
-            Z[index_i] = assert_numpy(
+            index_i = (self.bins == bin_i) & (~self.free_flag) & (~self.Outlier)
+            s = self.HKL_array[index_i]
+            V = np.concatenate([s**2, 2 * s[:, [0, 2, 1]] * s[:, [1, 0, 2]]], axis=-1)
+            Z = assert_numpy(
                 torch.log(
                     self.Fo[index_i]
                     / (
                         self.kisos[bin_i]
                         * torch.abs(
                             self.Fprotein_HKL[index_i]
                             + self.kmasks[bin_i] * self.Fmask_HKL[index_i]
                         )
                     )
                 )
                 / (2.0 * np.pi**2)
             )
-        # use only working set
-        V = V[~self.free_flag]
-        Z = Z[~self.free_flag]
-        M = V.T @ V  # M = np.einsum("ki,kj->ij", V, V)
-        b = -np.sum(Z * V.T, axis=-1)
-        U = np.linalg.inv(M) @ b
-        uaniso = torch.tensor(U).to(self.Fo).requires_grad_(requires_grad)
-        return uaniso
+            M = V.T @ V  # M = np.einsum("ki,kj->ij", V, V)
+            b = -np.sum(Z * V.T, axis=-1)
+            U = np.linalg.inv(M) @ b
+            uanisos.append(torch.tensor(U).to(self.Fo).requires_grad_(requires_grad))
+        return uanisos
 
     def _set_scales(
         self,
         requires_grad,
         kiso=1.0,
         kmask=0.35,
         uaniso=[0.01, 0.01, 0.01, 1e-4, 1e-4, 1e-4],
@@ -650,22 +668,23 @@
             torch.tensor(kmask).to(self.atom_pos_frac).requires_grad_(requires_grad)
             for i in range(self.n_bins)
         ]
         self.kisos = [
             torch.tensor(kiso).to(self.atom_pos_frac).requires_grad_(requires_grad)
             for i in range(self.n_bins)
         ]
-        self.uaniso = (
+        self.uanisos = [
             torch.tensor(uaniso).to(self.atom_pos_frac).requires_grad_(requires_grad)
-        )
+            for i in range(self.n_bins)
+        ]
 
     def init_scales(self, requires_grad=True):
         if hasattr(self, "Fo"):
             self.kmasks, self.kisos = self._init_kmask_kiso(requires_grad=requires_grad)
-            self.uaniso = self._init_uaniso(requires_grad=requires_grad)
+            self.uanisos = self._init_uaniso(requires_grad=requires_grad)
         else:
             self._set_scales(requires_grad)
 
     def _get_scales_lbfgs_LS(
         self, n_steps=3, lr=0.1, verbose=True, initialize=True, return_loss=False
     ):
         """
@@ -677,29 +696,37 @@
             self.init_scales(requires_grad=True)
 
         def closure():
             Fmodel = self.calc_ftotal()
             Fmodel_mag = torch.abs(Fmodel)
             # LS loss
             loss = torch.sum(
-                (self.Fo[~self.free_flag] - Fmodel_mag[~self.free_flag]) ** 2
+                (
+                    self.Fo[(~self.free_flag) & (~self.Outlier)]
+                    - Fmodel_mag[(~self.free_flag) & (~self.Outlier)]
+                )
+                ** 2
             )
             self.lbfgs.zero_grad()
             loss.backward()
             return loss
 
-        params = self.kmasks + self.kisos + [self.uaniso]
+        params = self.kmasks + self.kisos + self.uanisos
         self.lbfgs = torch.optim.LBFGS(params, lr=lr)
         loss_track = []
         for _ in range(n_steps):
             start_time = time.time()
             loss = self.lbfgs.step(closure)
             Fmodel = self.calc_ftotal()
             Fmodel_mag = torch.abs(Fmodel)
-            r_work, r_free = r_factor(self.Fo, Fmodel_mag, self.free_flag)
+            r_work, r_free = r_factor(
+                self.Fo[~self.Outlier],
+                Fmodel_mag[~self.Outlier],
+                self.free_flag[~self.Outlier],
+            )
             loss_track.append(
                 [assert_numpy(loss), assert_numpy(r_work), assert_numpy(r_free)]
             )
             str_ = f"Time: {time.time()-start_time:.3f}"
             if verbose:
                 print(
                     f"Scale, {loss_track[-1][0]:.3f}, {loss_track[-1][1]:.3f}, {loss_track[-1][2]:.3f}",
@@ -722,29 +749,36 @@
             self.init_scales(requires_grad=True)
 
         def closure():
             Fmodel = self.calc_ftotal()
             Fmodel_mag = torch.abs(Fmodel)
             # R factor
             loss = torch.sum(
-                torch.abs(self.Fo[~self.free_flag] - Fmodel_mag[~self.free_flag])
-            ) / torch.sum(self.Fo[~self.free_flag])
+                torch.abs(
+                    self.Fo[(~self.free_flag) & (~self.Outlier)]
+                    - Fmodel_mag[(~self.free_flag) & (~self.Outlier)]
+                )
+            ) / torch.sum(self.Fo[(~self.free_flag) & (~self.Outlier)])
             self.lbfgs.zero_grad()
             loss.backward()
             return loss
 
-        params = self.kmasks + self.kisos + [self.uaniso]
+        params = self.kmasks + self.kisos + self.uanisos
         self.lbfgs = torch.optim.LBFGS(params, lr=lr)
         loss_track = []
         for _ in range(n_steps):
             start_time = time.time()
             loss = self.lbfgs.step(closure)
             Fmodel = self.calc_ftotal()
             Fmodel_mag = torch.abs(Fmodel)
-            r_work, r_free = r_factor(self.Fo, Fmodel_mag, self.free_flag)
+            r_work, r_free = r_factor(
+                self.Fo[~self.Outlier],
+                Fmodel_mag[~self.Outlier],
+                self.free_flag[~self.Outlier],
+            )
             loss_track.append(
                 [assert_numpy(loss), assert_numpy(r_work), assert_numpy(r_free)]
             )
             str_ = f"Time: {time.time()-start_time:.3f}"
             if verbose:
                 print(
                     f"Scale, {loss_track[-1][0]:.3f}, {loss_track[-1][1]:.3f}, {loss_track[-1][2]:.3f}",
@@ -763,23 +797,93 @@
         r_lr=0.1,
         initialize=True,
         verbose=True,
     ):
         self._get_scales_lbfgs_LS(ls_steps, ls_lr, verbose, initialize)
         self._get_scales_lbfgs_r(r_steps, r_lr, verbose, initialize=False)
 
+    def get_scales_adam(
+        self, 
+        lr=0.1, 
+        n_steps=100, 
+        sub_ratio=0.3, 
+        initialize=True, 
+        verbose=False
+    ):
+        def adam_opt_i(
+            bin_i, index_i, sub_ratio=0.3, lr=0.001, n_steps=100, verbose=False
+        ):
+            def adam_stepopt(sub_boolean_mask):
+                Fmodel_i = self._calc_ftotal_bini(
+                    bin_i, index_i, self.HKL_array, self.Fprotein_HKL, self.Fmask_HKL
+                )
+                Fmodel_mag = torch.abs(Fmodel_i)
+                # LS loss with subsampling
+                fo_i_sub = fo_i[sub_boolean_mask]
+                Fmodel_i_sub = Fmodel_mag[sub_boolean_mask]
+                free_flagi_sub = free_flagi[sub_boolean_mask]
+                loss = torch.sum(
+                    (fo_i_sub[~free_flagi_sub] - Fmodel_i_sub[~free_flagi_sub]) ** 2
+                )
+                # loss = torch.sum(torch.abs(fo_i_sub[~free_flagi_sub] - Fmodel_i_sub[~free_flagi_sub]))/torch.sum(Fmodel_i_sub[~free_flagi_sub])
+                r_work, r_free = r_factor(fo_i, Fmodel_mag, free_flagi)
+                adam.zero_grad()
+                loss.backward()
+                adam.step()
+                return loss, r_work, r_free
+
+            params = [self.kmasks[bin_i], self.kisos[bin_i], self.uanisos[bin_i]]
+            adam = torch.optim.Adam(params, lr=lr)
+            for _ in range(n_steps):
+                start_time = time.time()
+                sub_boolean_mask = (
+                    np.random.rand(
+                        np.sum(index_i),
+                    )
+                    < sub_ratio
+                )
+                temp = adam_stepopt(sub_boolean_mask)
+                time_this_round = round(time.time() - start_time, 3)
+                str_ = "Time: " + str(time_this_round)
+                if verbose:
+                    print("Scale", *[assert_numpy(i) for i in temp], str_, flush=True)
+
+        if initialize:
+            self.init_scales(requires_grad=True)
+
+        for bin_i in range(self.n_bins):
+            index_i = (self.bins == bin_i) & (~self.Outlier)
+            fo_i = self.Fo[index_i]
+            free_flagi = self.free_flag[index_i]
+            adam_opt_i(
+                bin_i,
+                index_i,
+                lr=lr,
+                n_steps=n_steps,
+                sub_ratio=sub_ratio,
+                verbose=verbose,
+            )
+
+        Fmodel = self.calc_ftotal()
+        Fmodel_mag = torch.abs(Fmodel)
+        self.r_work, self.r_free = r_factor(
+            self.Fo[~self.Outlier],
+            Fmodel_mag[~self.Outlier],
+            self.free_flag[~self.Outlier],
+        )
+
     def _calc_ftotal_bini(self, bin_i, index_i, HKL_array, Fprotein, Fmask):
         """
         calculate ftotal for bin i
         """
         scaled_fmask_i = Fmask[index_i] * self.kmasks[bin_i]
         fmodel_i = (
             self.kisos[bin_i]
             * aniso_scaling(
-                self.uaniso,
+                self.uanisos[bin_i],
                 self.reciprocal_cell_paras,
                 HKL_array[index_i],
             )
             * (Fprotein[index_i] + scaled_fmask_i)
         )
         return fmodel_i
 
@@ -828,34 +932,36 @@
     def summarize(self):
         """
         Print model quality log like phenix.model_vs_data
         """
         ftotal = self.calc_ftotal(Return=True)
         _, counts = np.unique(self.bins, return_counts=True)
         print(
-            f"{'Resolution':15},{'N_work':>7},{'N_free':>7},{'R_work':>7},{'R_free':>7},{'k_mask':>7},{'k_iso':>7}"
+            f"{'Resolution':15} {'N_work':>7} {'N_free':>7} {'<Fobs>':>7} {'<|Fmodel|>':>9} {'R_work':>7} {'R_free':>7} {'k_mask':>7} {'k_iso':>7}"
         )
         for i in range(self.n_bins):
-            index_i = self.bins == i
+            index_i = (self.bins == i) & (~self.Outlier)
             r_worki, r_freei = r_factor(
                 self.Fo[index_i], torch.abs(ftotal[index_i]), self.free_flag[index_i]
             )
             N_work = counts[i] - np.sum(self.free_flag[index_i])
             N_free = np.sum(self.free_flag[index_i])
             print(
-                f"{self.bin_labels[i]:<15},{N_work:7d},{N_free:7d},{assert_numpy(r_worki):7.3f},{assert_numpy(r_freei):7.3f},{assert_numpy(self.kmasks[i]):7.3f},{assert_numpy(self.kisos[i]):7.3f}"
+                f"{self.bin_labels[i]:<15} {N_work:7d} {N_free:7d} {assert_numpy(torch.mean(self.Fo[index_i])):7.1f} {assert_numpy(torch.mean(torch.abs(ftotal[index_i]))):9.1f} {assert_numpy(r_worki):7.3f} {assert_numpy(r_freei):7.3f} {assert_numpy(self.kmasks[i]):7.3f} {assert_numpy(self.kisos[i]):7.3f}"
             )
+        self.r_work, self.r_free = r_factor(
+            self.Fo[~self.Outlier],
+            torch.abs(ftotal)[~self.Outlier],
+            self.free_flag[~self.Outlier],
+        )
+        print(f"r_work: {assert_numpy(self.r_work):<7.3f}")
+        print(f"r_free: {assert_numpy(self.r_free):<7.3f}")
+        print(f"Number of outliers: {np.sum(self.Outlier):<7d}")
 
-        self.r_work, self.r_free = r_factor(self.Fo, torch.abs(ftotal), self.free_flag)
-        print(f"r_work: {assert_numpy(self.r_work):7.3f}")
-        print(f"r_free: {assert_numpy(self.r_free):7.3f}")
-
-    def calc_fprotein_batch(
-        self, atoms_position_batch, Return=False, PARTITION=20
-    ):
+    def calc_fprotein_batch(self, atoms_position_batch, Return=False, PARTITION=20):
         """
         Calculate the Fprotein with batched models. Most parameters are similar to `Calc_Fprotein`
 
         atoms_positions_batch: torch.float32 tensor, [N_batch, N_atoms, 3]
 
         PARTITION: Int, default 20
             To reduce the memory cost during the computation, we divide the batch into several partitions and loops through them.
@@ -979,15 +1085,15 @@
         """
         calculate ftotal for bin i
         """
         scaled_fmask_i = Fmask[:, index_i] * self.kmasks[bin_i]
         fmodel_i = (
             self.kisos[bin_i]
             * aniso_scaling(
-                self.uaniso,
+                self.uanisos[bin_i],
                 self.reciprocal_cell_paras,
                 HKL_array[index_i],
             )
             * (Fprotein[:, index_i] + scaled_fmask_i)
         )
         return fmodel_i
 
@@ -1092,15 +1198,19 @@
     sym_oped_pos_frac = (
         torch.einsum("oxy,ay->aox", R_G_tensor_stack, atom_pos_frac) + T_G_tensor_stack
     )
     sym_oped_hkl = torch.einsum("rx,oxy->roy", HKL_tensor, R_G_tensor_stack)
     exp_phase = 0.0
     # Loop through symmetry operations instead of fully vectorization, to reduce the memory cost
     for i in range(sym_oped_pos_frac.size(dim=1)):
-        phase_G = 2 * np.pi * torch.einsum("ax,rx->ar", sym_oped_pos_frac[:, i, :], HKL_tensor) # [N_atom, N_HKLs]
+        phase_G = (
+            2
+            * np.pi
+            * torch.einsum("ax,rx->ar", sym_oped_pos_frac[:, i, :], HKL_tensor)
+        )  # [N_atom, N_HKLs]
         dwf_aniso = DWF_aniso(
             atom_aniso_uw, orth2frac_tensor, sym_oped_hkl[:, i, :]
         )  # [N_atom, N_HKLs]
         dwf_all = torch.where(mask_vec[:, None], dwf_iso, dwf_aniso)
         exp_phase = exp_phase + dwf_all * torch.exp(1j * phase_G)
     F_calc = torch.sum(exp_phase * oc_sf, dim=0)
     return F_calc
@@ -1163,17 +1273,19 @@
                 2
                 * torch.pi
                 * torch.tensordot(
                     sym_oped_pos_frac[start:end, :, :, i], HKL_tensor.T, 1
                 )
             )
             dwf_aniso = DWF_aniso(
-            atom_aniso_uw, orth2frac_tensor, sym_oped_hkl[:, i, :]
+                atom_aniso_uw, orth2frac_tensor, sym_oped_hkl[:, i, :]
+            )  # [N_atoms, N_HKLs]
+            dwf_all = torch.where(
+                mask_vec[:, None], dwf_iso, dwf_aniso
             )  # [N_atoms, N_HKLs]
-            dwf_all = torch.where(mask_vec[:, None], dwf_iso, dwf_aniso) # [N_atoms, N_HKLs]
             exp_phase_ij = dwf_all * torch.exp(1j * phase_ij)
             # Shape [PARTITION, N_HKLs], sum over atoms
             Fcalc_ij = torch.sum(exp_phase_ij * oc_sf, dim=1)
             # Shape [PARTITION, N_HKLs], sum over symmetry operations
             Fcalc_j = Fcalc_j + Fcalc_ij
         if j == 0:
             F_calc = Fcalc_j
```

### Comparing `SFcalculator_torch-0.1.7/SFC_Torch/io.py` & `SFcalculator_torch-0.1.8/SFC_Torch/io.py`

 * *Files identical despite different names*

### Comparing `SFcalculator_torch-0.1.7/SFC_Torch/mask.py` & `SFcalculator_torch-0.1.8/SFC_Torch/mask.py`

 * *Files identical despite different names*

### Comparing `SFcalculator_torch-0.1.7/SFC_Torch/packingscore.py` & `SFcalculator_torch-0.1.8/SFC_Torch/packingscore.py`

 * *Files identical despite different names*

### Comparing `SFcalculator_torch-0.1.7/SFC_Torch/patterson.py` & `SFcalculator_torch-0.1.8/SFC_Torch/patterson.py`

 * *Files identical despite different names*

### Comparing `SFcalculator_torch-0.1.7/SFC_Torch/symmetry.py` & `SFcalculator_torch-0.1.8/SFC_Torch/symmetry.py`

 * *Files identical despite different names*

### Comparing `SFcalculator_torch-0.1.7/SFC_Torch/utils.py` & `SFcalculator_torch-0.1.8/SFC_Torch/utils.py`

 * *Files identical despite different names*

### Comparing `SFcalculator_torch-0.1.7/SFC_Torch/voxel.py` & `SFcalculator_torch-0.1.8/SFC_Torch/voxel.py`

 * *Files identical despite different names*

### Comparing `SFcalculator_torch-0.1.7/SFcalculator_torch.egg-info/SOURCES.txt` & `SFcalculator_torch-0.1.8/SFcalculator_torch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SFcalculator_torch-0.1.7/license` & `SFcalculator_torch-0.1.8/license`

 * *Files identical despite different names*

### Comparing `SFcalculator_torch-0.1.7/setup.py` & `SFcalculator_torch-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `SFcalculator_torch-0.1.7/tests/conftest.py` & `SFcalculator_torch-0.1.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `SFcalculator_torch-0.1.7/tests/test_Fmodel.py` & `SFcalculator_torch-0.1.8/tests/test_Fmodel.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,19 +41,20 @@
 def test_calc_fall(data_pdb, data_mtz_exp, data_mtz_fmodel_ksol0, data_mtz_fmodel_ksol1, Return, Anomalous):
     sfcalculator = SFcalculator(
         data_pdb, mtzfile_dir=data_mtz_exp, set_experiment=True, anomalous=Anomalous)
     sfcalculator.inspect_data()
     Fprotein = sfcalculator.calc_fprotein(Return=Return)
     Fsolvent = sfcalculator.calc_fsolvent(
         dmin_mask=6.0, dmin_nonzero=3.0, Return=Return)
-    sfcalculator.assign_resolution_bins(return_labels=False)
     sfcalculator.get_scales_lbfgs(ls_steps=2, r_steps=2, ls_lr=0.00001, r_lr=0.00001, verbose=False)
     Ftotal = sfcalculator.calc_ftotal()
     assert len(Ftotal) == 3197
     assert assert_numpy(sfcalculator.r_free) < 0.15
+    sfcalculator.get_scales_adam(lr=0.01, n_steps=20, sub_ratio=0.3, initialize=True, verbose=False)
+    assert assert_numpy(sfcalculator.r_free) < 0.15
 
     Fcalc = rs.read_mtz(data_mtz_fmodel_ksol0)
     Fmodel = rs.read_mtz(data_mtz_fmodel_ksol1)
     assert (Fmodel.get_hkls() == sfcalculator.HKL_array).all()
 
     calc_mag = Fcalc['FMODEL'].to_numpy()
     calc_ph = np.deg2rad(Fcalc['PHIFMODEL'].to_numpy())
@@ -94,17 +95,16 @@
                             Fcalc['FMODEL'].to_numpy())[0] > 0.99
             assert pearsonr(np.abs(Fsolvent_arr),
                             np.abs(Fmask_complex))[0] > 0.84
 
 
 def test_calc_ftotal_nodata(data_pdb):
     sfcalculator = SFcalculator(
-        data_pdb, mtzfile_dir=None, dmin=2.5, set_experiment=True)
+        data_pdb, mtzfile_dir=None, dmin=2.5, set_experiment=False)
     sfcalculator.inspect_data()
-    sfcalculator.assign_resolution_bins(return_labels=False)
     sfcalculator.calc_fprotein(Return=False)
     sfcalculator.calc_fsolvent(
         dmin_mask=6.0, dmin_nonzero=3.0, Return=False)
     sfcalculator.init_scales(requires_grad=False)
     Ftotal = sfcalculator.calc_ftotal()
     assert len(Ftotal) == 1747
 
@@ -121,15 +121,14 @@
     Fsolvent = sfcalculator.calc_fsolvent(
         dmin_mask=6.0, dmin_nonzero=3.0, Return=True)
     Fprotein_batch = sfcalculator.calc_fprotein_batch(
         atoms_pos_batch, Return=True, PARTITION=partition_size)
     Fsolvent_batch = sfcalculator.calc_fsolvent_batch(
         dmin_mask=6.0, dmin_nonzero=3.0, Return=True, PARTITION=partition_size)
     
-    sfcalculator.assign_resolution_bins(return_labels=False)
     sfcalculator.init_scales(requires_grad=False)
     Ftotal = sfcalculator.calc_ftotal()
     Ftotal_batch = sfcalculator.calc_ftotal_batch()
 
     assert len(Fprotein_batch) == 5
     assert np.all(np.isclose(assert_numpy(Fprotein_batch[3]),
                              assert_numpy(Fprotein),
@@ -148,15 +147,14 @@
                              rtol=1e-3, atol=1e1))
 
 
 def test_prepare_dataset(data_pdb, data_mtz_exp):
     sfcalculator = SFcalculator(
         data_pdb, mtzfile_dir=data_mtz_exp, set_experiment=True)
     sfcalculator.inspect_data()
-    sfcalculator.assign_resolution_bins()
     sfcalculator.calc_fprotein(Return=False)
     sfcalculator.calc_fsolvent(
         dmin_mask=6.0, dmin_nonzero=3.0, Return=False)
     sfcalculator.init_scales(requires_grad=False)
     sfcalculator.calc_ftotal()
     ds = sfcalculator.prepare_dataset("HKL_array", "Ftotal_HKL")
     assert len(ds) == 3197
```

### Comparing `SFcalculator_torch-0.1.7/tests/test_io.py` & `SFcalculator_torch-0.1.8/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `SFcalculator_torch-0.1.7/tests/test_patterson.py` & `SFcalculator_torch-0.1.8/tests/test_patterson.py`

 * *Files identical despite different names*

### Comparing `SFcalculator_torch-0.1.7/tests/test_voxel.py` & `SFcalculator_torch-0.1.8/tests/test_voxel.py`

 * *Files identical despite different names*

