# Comparing `tmp/waveformtools-2023.6.3.tar.gz` & `tmp/waveformtools-2023.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waveformtools-2023.6.3.tar", last modified: Sat Jun  3 11:00:01 2023, max compression
+gzip compressed data, was "waveformtools-2023.6.5.tar", last modified: Mon Jun  5 10:03:38 2023, max compression
```

## Comparing `waveformtools-2023.6.3.tar` & `waveformtools-2023.6.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 11:00:01.870920 waveformtools-2023.6.3/
--rwxrwxrwx   0 root         (0) root         (0)     1075 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8758 2023-06-03 11:00:01.869918 waveformtools-2023.6.3/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      106 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/README
--rwxrwxrwx   0 root         (0) root         (0)     8103 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1089 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-03 11:00:01.870920 waveformtools-2023.6.3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1396 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 11:00:01.868916 waveformtools-2023.6.3/waveformtools/
--rw-rw-rw-   0 root         (0) root         (0)     5392 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/waveformtools/BMS.py
--rw-rw-rw-   0 root         (0) root         (0)     8709 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/waveformtools/CoM.py
--rwxrwxrwx   0 root         (0) root         (0)     1306 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/waveformtools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11540 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/waveformtools/compare.py
--rw-rw-rw-   0 root         (0) root         (0)    53234 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/waveformtools/dataIO.py
--rw-rw-rw-   0 root         (0) root         (0)     1712 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/waveformtools/diagnostics.py
--rw-rw-rw-   0 root         (0) root         (0)    27426 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/waveformtools/differentiate.py
--rw-rw-rw-   0 root         (0) root         (0)     9304 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/waveformtools/extrapolate.py
--rw-rw-rw-   0 root         (0) root         (0)    13790 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/waveformtools/grids.py
--rw-rw-rw-   0 root         (0) root         (0)    11033 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/waveformtools/integrate.py
--rw-rw-rw-   0 root         (0) root         (0)    29963 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/waveformtools/legacy.py
--rw-rw-rw-   0 root         (0) root         (0)    56776 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/waveformtools/simulations.py
--rw-rw-rw-   0 root         (0) root         (0)     6443 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/waveformtools/spherical.py
--rw-rw-rw-   0 root         (0) root         (0)    12205 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/waveformtools/transforms.py
--rw-rw-rw-   0 root         (0) root         (0)    65808 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/waveformtools/waveforms.py
--rw-rw-rw-   0 root         (0) root         (0)    91309 2023-06-03 10:59:26.000000 waveformtools-2023.6.3/waveformtools/waveformtools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 11:00:01.869918 waveformtools-2023.6.3/waveformtools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8758 2023-06-03 11:00:01.000000 waveformtools-2023.6.3/waveformtools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      654 2023-06-03 11:00:01.000000 waveformtools-2023.6.3/waveformtools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-03 11:00:01.000000 waveformtools-2023.6.3/waveformtools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      102 2023-06-03 11:00:01.000000 waveformtools-2023.6.3/waveformtools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-03 11:00:01.000000 waveformtools-2023.6.3/waveformtools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:03:38.526371 waveformtools-2023.6.5/
+-rwxrwxrwx   0 root         (0) root         (0)     1075 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8758 2023-06-05 10:03:38.526371 waveformtools-2023.6.5/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      106 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/README
+-rwxrwxrwx   0 root         (0) root         (0)     8103 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 10:03:38.526371 waveformtools-2023.6.5/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1396 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:03:38.524371 waveformtools-2023.6.5/waveformtools/
+-rw-rw-rw-   0 root         (0) root         (0)     5480 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/waveformtools/BMS.py
+-rw-rw-rw-   0 root         (0) root         (0)     9130 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/waveformtools/CoM.py
+-rwxrwxrwx   0 root         (0) root         (0)     1284 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/waveformtools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10895 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/waveformtools/compare.py
+-rw-rw-rw-   0 root         (0) root         (0)    44315 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/waveformtools/dataIO.py
+-rw-rw-rw-   0 root         (0) root         (0)     1698 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/waveformtools/diagnostics.py
+-rw-rw-rw-   0 root         (0) root         (0)    27085 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/waveformtools/differentiate.py
+-rw-rw-rw-   0 root         (0) root         (0)     9322 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/waveformtools/extrapolate.py
+-rw-rw-rw-   0 root         (0) root         (0)    14069 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/waveformtools/grids.py
+-rw-rw-rw-   0 root         (0) root         (0)    10952 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/waveformtools/integrate.py
+-rw-rw-rw-   0 root         (0) root         (0)    28886 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/waveformtools/legacy.py
+-rw-rw-rw-   0 root         (0) root         (0)    54027 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/waveformtools/simulations.py
+-rw-rw-rw-   0 root         (0) root         (0)     6476 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/waveformtools/spherical.py
+-rw-rw-rw-   0 root         (0) root         (0)    12506 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/waveformtools/transforms.py
+-rw-rw-rw-   0 root         (0) root         (0)    56079 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/waveformtools/waveforms.py
+-rw-rw-rw-   0 root         (0) root         (0)    91151 2023-06-05 10:03:05.000000 waveformtools-2023.6.5/waveformtools/waveformtools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 10:03:38.525371 waveformtools-2023.6.5/waveformtools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8758 2023-06-05 10:03:38.000000 waveformtools-2023.6.5/waveformtools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      654 2023-06-05 10:03:38.000000 waveformtools-2023.6.5/waveformtools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 10:03:38.000000 waveformtools-2023.6.5/waveformtools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      102 2023-06-05 10:03:38.000000 waveformtools-2023.6.5/waveformtools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-05 10:03:38.000000 waveformtools-2023.6.5/waveformtools.egg-info/top_level.txt
```

### Comparing `waveformtools-2023.6.3/LICENSE` & `waveformtools-2023.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `waveformtools-2023.6.3/PKG-INFO` & `waveformtools-2023.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waveformtools
-Version: 2023.6.3
+Version: 2023.6.5
 Summary:  Tools for working with numerical relativity and waveforms data 
 Home-page: https://gitlab.com/vaishakp/waveformtools
 Author: Vaishak Prasad
 Author-email: Vaishak Prasad <vaishakprasad@gmail.com>
 Project-URL: Homepage, https://gitlab.com/vaishakp/waveformtools
 Project-URL: Bug Tracker, https://gitlab.com/vaishakp/waveformtools/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `waveformtools-2023.6.3/README.md` & `waveformtools-2023.6.5/README.md`

 * *Files identical despite different names*

### Comparing `waveformtools-2023.6.3/pyproject.toml` & `waveformtools-2023.6.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `waveformtools-2023.6.3/setup.py` & `waveformtools-2023.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # requiremnts directly from toml
 # mreq, oreq = get_requirements()
 
 
 
 setuptools.setup(
     name="waveformtools",
- 	version="2023.06.03",
+ 	version="2023.06.05",
     author="Vaishak Prasad",
     author_email="vaishakprasad@gmail.com",
     description="Functions for handling waveform and numerical relativity data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/vaishakp/waveformtools",
     packages=setuptools.find_packages(),
```

### Comparing `waveformtools-2023.6.3/waveformtools/BMS.py` & `waveformtools-2023.6.5/waveformtools/BMS.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,42 +12,40 @@
 def compute_conformal_k(vec_v, theta, phi, spin_phase=0):
     """Compute the conformal factor for the boost transformation
             :math:`k = \\exp(-2i \\lambda) \\gamma^3
             (1 - \\mathbf{v} \\cdot \\mathbf{r})^3`
 
     Parameters
     ----------
-    vec_v : list
-            The velocity vector.
+    vec_v: list
+                    The velocity vector.
 
-    theta : float
-            The polar angle :math:`\\theta' in radians.
+    theta: float
+                    The polar angle :math:`\\theta' in radians.
 
-    phi : float
-          The azimuthal angle :math:`\\phi' in radians.
+    phi: float
+                            The azimuthal angle :math:`\\phi' in radians.
 
-    spin_phase : float, optional
-                 The spin phase :math:`\\lambda'. Defaults to 0.
+    spin_phase: float, optional
+                             The spin phase :math:`\\lambda'. Defaults to 0.
 
     Returns
     -------
-    conformal_k : float
-                  The conformal factor for the
-                  boost transformation as defined above.
+    conformal_k:	float
+                    The conformal factor for the
+                    boost transformation as defined above.
     """
 
     # unpack the velocity vector
     vel_x, vel_y, vel_z = vec_v
 
     # magnitude of velocity
     mag_v = np.sqrt(vel_x**2 + vel_y**2 + vel_z**2)
     # compute the dot product
-    v_dot_r = np.sin(theta) * (
-        vel_x * np.cos(phi) + vel_y * np.sin(phi)
-    ) + vel_z * np.cos(theta)
+    v_dot_r = np.sin(theta) * (vel_x * np.cos(phi) + vel_y * np.sin(phi)) + vel_z * np.cos(theta)
 
     # Lorentz factor
     gamma = 1.0 / np.sqrt(1 - mag_v**2)
 
     # spin_phase
     spin_factor = np.exp(-2 * 1j * spin_phase)
 
@@ -62,29 +60,33 @@
     :math:`\\alpha(\\theta, \\phi)` given its modes. This method
     just multiplies the alpha modes with their corresponding spherical
     harmonic basis functions and returns the summed result.
 
 
     Parameters
     ----------
-    supertransl_alpha_modes : dict
-                              A dictionary of lists, each sublist
-                              containing the set of super-translation
-                              modes corresponding to a particular
-                              :math:`\\ell'.
-    theta : float
-            The polar angle :math:`\\theta'.
-    phi : float
-          The azimuthal angle :math:`\\phi'.
+
+    supertransl_alpha_modes:	dict
+                                A dictionary of lists, each sublist
+                                containing the set of super-translation
+                                modes corresponding to a particular
+                                :math:`\\ell'.
+    theta:		float
+                            The polar angle :math:`\\theta'.
+    phi:	float
+                    The azimuthal angle :math:`\\phi'.
 
     Returns
     --------
-    supertransl_alpha_sphere : func
-                               A function on the sphere
-                               (arguments :math:`\\theta', math:`\\phi').
+
+    supertransl_alpha_sphere:		func
+                                    A function on the sphere
+                                    (arguments :math:`\\theta', math:`\\phi').
+
+
     """
 
     # For partial evaluation of functions
     # from functools import partial
     message(supertransl_alpha_modes.keys())
     # Find the extreme ell values.
     keys_list = sorted(list(supertransl_alpha_modes.keys()))
@@ -104,55 +106,57 @@
     theta = np.pi / 2
     phi = 0.0
     for item in keys_list:
         ell = int(item[1])
         for m_index in range(2 * ell + 1):
             emm = m_index - ell
             message("ell is", ell, type(ell), "emm is ", emm)
-            supertransl_alpha_sphere += supertransl_alpha_modes[item][
-                m_index
-            ] * Yslm(spin_weight, ell, emm, theta, phi)
+            supertransl_alpha_sphere += supertransl_alpha_modes[item][m_index] * Yslm(spin_weight, ell, emm, theta, phi)
 
     return supertransl_alpha_sphere
 
 
 def boost_waveform(unboosted_waveform, conformal_factor):
     """Boost the waveform given the unboosted waveform and the boost conformal factor.
 
     Parameters
     ----------
-    non_boosted_waveform : list
-                           A list with a single floating point number
-                           or a numpy array of the unboosted waveform.
-                           The waveform can have angular as well as
-                           time dimentions.
-
-                           The nesting order should be that, given the
-                           list `non_boosted_waveform', each item in the
-                           list refers to an array defined on the sphere
-                           at a particular time or frequency. The subitem
-                           will have dimensions [ntheta, nphi].
-    conformal_factor : float/array
-                       The conformal factor for the Lorentz transformation.
-                       It may be a single floating point number or an array
-                       on a spherical grid. The array will be of dimensions
-                       [ntheta, nphi]
-
-    gridinfo : class instance
-               The class instance that contains the properties
-               of the spherical grid.
+
+    non_boosted_waveform:	list
+                            A list with a single floating point number
+                            or a numpy array of the unboosted waveform.
+                            The waveform can have angular as well as
+                            time dimentions.
+
+                            The nesting order should be that, given the
+                            list `non_boosted_waveform', each item in the
+                            list refers to an array defined on the sphere
+                            at a particular time or frequency. The subitem
+                            will have dimensions [ntheta, nphi].
+
+
+
+    conformal_factor:		float/array
+                            The conformal factor for the Lorentz transformation.
+                            It may be a single floating point number or an array
+                            on a spherical grid. The array will be of dimensions
+                            [ntheta, nphi]
+
+    gridinfo:		class instance
+                    The class instance that contains the properties
+                    of the spherical grid.
 
     """
 
     # Find out if the unboosted waveform is a single number or defined on a spherical grid.
     # onepoint = isinstance(unboosted_waveform[0], float)
 
     # if not onepoint:
     # Get the spherical grid shape.
-    #   ntheta, nphi = np.array(unboosted_waveform[0]).shape
+    # 	ntheta, nphi = np.array(unboosted_waveform[0]).shape
 
     # Compute the meshgrid for theta and phi.
     # theta, phi = gridinfo.meshgrid
 
     # A list to store the boosted waveform.
     boosted_waveform = []
```

### Comparing `waveformtools-2023.6.3/waveformtools/CoM.py` & `waveformtools-2023.6.5/waveformtools/CoM.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,55 +8,45 @@
 
 
 def X_com_moments(time_axis, Xcom, order):
     """Compute the nth order temporal moment of the COM coordinates.
 
     Parameters
     ----------
-    time_axis : 1d array
-                The time axis.
-    Xcom : list of arrays
-           A list of three 1d arrays, each a 1d array containing the
-           time series of the x, y and z co-ordinates in that order.
-    order : int
-            The order of the moment.
+
+    time_axis:		1d array
+                                    The time axis.
+    Xcom:		list
+                            A list of three 1d arrays, each a 1d array containing the
+                            time series of the x, y and z co-ordinates in that order.
+    order:		int
+                            The order of the moment.
 
     Returns
     -------
-    moments : list
-              A list containing three real numbers, one each for the moment
-              of x, y and z locations.
+
+    moments:	list
+                            A list containing three real numbers, one each for the moment
+                            of x, y and z locations.
 
     """
     # Initial and final times
     time_i = time_axis[0]
     time_f = time_axis[-1]
 
     duration_t = time_f - time_i
     # Split the data
     x_all, y_all, z_all = Xcom
 
     # Interpolate
     from scipy.interpolate import interp1d
 
-    x_all_int_fun = interp1d(
-        time_axis,
-        np.power(time_axis, order) * x_all / duration_t,
-        kind="quadratic",
-    )
-    y_all_int_fun = interp1d(
-        time_axis,
-        np.power(time_axis, order) * y_all / duration_t,
-        kind="quadratic",
-    )
-    z_all_int_fun = interp1d(
-        time_axis,
-        np.power(time_axis, order) * z_all / duration_t,
-        kind="quadratic",
-    )
+    x_all_int_fun = interp1d(time_axis, np.power(time_axis, order) * x_all / duration_t, kind="quadratic")
+    y_all_int_fun = interp1d(time_axis, np.power(time_axis, order) * y_all / duration_t, kind="quadratic")
+    z_all_int_fun = interp1d(time_axis, np.power(time_axis, order) * z_all / duration_t, kind="quadratic")
 
     int_funcs = [x_all_int_fun, y_all_int_fun, z_all_int_fun]
 
     # Integrate
     from scipy.integrate import quad
 
     moments = {}
@@ -74,107 +64,109 @@
 
 def compute_com_alpha(time_i, time_f, Xcom_0, Xcom_1):
     """Computes the CoM correction alpha parameter: the mean displacement of the system,
     of the COM correction as defined in Woodford et al. 2019 (Phys. Rev. D 100, 124010).
 
     Parameters
     ----------
-    time_i : float
-             initial time
-    time_f : float
-             final time
-    Xcom_0 : list
-             A list containing the zeroth order moments of the COM.
-    Xcom_1 : list
-             A list containing the first order moments of the COM.
+
+    time_i:	float
+                            initial time
+    time_f:	float
+                            final time
+    Xcom_0:	list
+                            A list containing the zeroth order moments of the COM.
+    Xcom_1:	list
+                            A list containing the first order moments of the COM.
 
     Returns
     -------
-    com_alpha : list
-                The list containig the alpha parameter vector
+
+    com_alpha:		list
+                                    The list containig the alpha parameter vector
 
     """
 
     com_alpha = (
-        4 * (time_f**2 + time_f * time_i + time_i**2) * np.array(Xcom_0)
-        - 6 * (time_f + time_i) * np.array(Xcom_1)
+        4 * (time_f**2 + time_f * time_i + time_i**2) * np.array(Xcom_0) - 6 * (time_f + time_i) * np.array(Xcom_1)
     ) / (time_f - time_i) ** 2
 
     return com_alpha
 
 
 def compute_com_beta(time_i, time_f, Xcom_0, Xcom_1):
     """Computes the CoM beta parameter: the mean drift of the system,
     of the COM correction as defined in Woodford et al. 2019 (Phys. Rev. D 100, 124010).
 
     Parameters
     ----------
-    time_i : float
-             initial time
-    time_f : float
-             final time
-    Xcom_0 : list
-             A list containing the zeroth order moments of the COM.
-    Xcom_1 : list
-             A list containing the first order moments of the COM.
+
+    time_i:	 float
+                             initial time
+    time_f:	float
+                            final time
+    Xcom_0:	list
+                            A list containing the zeroth order moments of the COM.
+    Xcom_1:	list
+                            A list containing the first order moments of the COM.
 
     Returns
     -------
-    com_beta : list
-                The list containig the alpha parameter vector
+
+    com_beta:		list
+                            The list containig the alpha parameter vector
 
     """
 
-    com_beta = (12 * (Xcom_1) - 6 * (time_f + time_i) * Xcom_0) / (
-        time_f - time_i
-    ) ** 2
+    com_beta = (12 * (Xcom_1) - 6 * (time_f + time_i) * Xcom_0) / (time_f - time_i) ** 2
 
     return com_beta
 
 
 def compute_conformal_k(vec_v, info, spin_phase=0):
     """Compute the conformal factor for the boost transformation
             :math:`k = \\exp(-2i \\lambda) \\gamma^3 (1 - \\mathbf{v} \\cdot \\mathbf{r})^3
 
-    Parameters
-    ----------
-    vec_v : list
-            A list of 2d arrays containing
-            the velocity vector in the form
-            [vec_x, vec_y, vec_z].
-
-    spin_phase : float, optional
-                 The spin phase :math:`\\lambda'. Defaults to 0.
-    info : class instance
-           An instance of the class `grids.sp_grid`
-           that contains information about the
-           spherical grid being used for the
-           transformations.
+    Inputs
+    ------
 
+    vec_v:		list
+                            A list of 2d arrays containing
+                            the velocity vector in the form
+                            [vec_x, vec_y, vec_z].
+
+    spin_phase:	float, optional
+                                    The spin phase :math:`\\lambda'. Defaults to 0.
+
+    info:		class instance
+                            An instance of the class `grids.sp_grid`
+                            that contains information about the
+                            spherical grid being used for the
+                            transformations.
     Returns
     --------
-    conformal_k : 2d array
-                  The conformal factor for the boost transformation
-                  as defined above.
+
+    conformal_k:	2d array
+                                    The conformal factor for the boost transformation
+                                    as defined above.
+
 
     """
 
     # unpack the velocity vector
     vel_x, vel_y, vel_z = vec_v
 
     # magnitude of velocity
     mag_v = np.sqrt(vel_x**2 + vel_y**2 + vel_z**2)
 
     # Compute the 2d co-ordinate axis on the sphere
     theta, phi = info.meshgrid
 
     # compute the dot product
-    v_dot_r = np.sin(theta) * (
-        vel_x * np.cos(phi) + vel_y * np.sin(phi)
-    ) + vel_z * np.cos(theta)
+    v_dot_r = np.sin(theta) * (vel_x * np.cos(phi) + vel_y * np.sin(phi)) + vel_z * np.cos(theta)
 
     # Lorentz factor
     gamma = 1.0 / np.sqrt(1 - mag_v**2)
 
     # spin_phase
     spin_factor = np.exp(-2 * 1j * spin_phase)
 
@@ -187,26 +179,28 @@
 def compute_translation_alpha_modes(time_axis, com_alpha, com_beta):
     """Compute the translation scalar :math:`\\alpha` in its spherical harmonic
     components given the mean motion of the centre of mass. These are basically
     the quantities in Eq. (4-5d) in the reference Woodford et al. 2019.
 
     Parameters
     ----------
-    time_axis : 1d array
-                The 1D array containing the time axis of the simulation.
-    alpha : 1d array
-            The 1D array containing the mean co-ordinate displacement of the COM of the system.
-    beta : 1d array
-           The 1D array containing the mean co-ordinate velocity of the COM.
+
+    time_axis:		1d array
+                                    The 1D array containing the time axis of the simulation.
+    alpha:		1d array
+                            The 1D array containing the mean co-ordinate displacement of the COM of the system.
+    beta:		1d array
+                            The 1D array containing the mean co-ordinate velocity of the COM.
 
     Returns
     -------
-    alpha_modes : modes_array
-                  A `waveforms.modes_array` object containing the SH
-                  decomposition of the 'Alpha' supertranslation variable.
+
+    alpha_modes :   modes_array
+                    A `waveforms.modes_array` object containing the SH
+                    decomposition of the 'Alpha' supertranslation variable.
 
     """
 
     # Define the total displacement
     delta_t = 0
     delta_x = com_alpha[0] + com_beta[0] * time_axis
     delta_y = com_alpha[1] + com_beta[1] * time_axis
@@ -233,64 +227,64 @@
     alpha_modes.set_mode_data(ell_value=1, emm_value=-1, data=Alpha_1m1)
     # l1m0
     alpha_modes.set_mode_data(ell_value=1, emm_value=0, data=Alpha_10)
     # l1m1
     alpha_modes.set_mode_data(ell_value=1, emm_value=1, data=Alpha_11)
 
     # Combine into one list
-    # modes    = { 'l0' : [Alpha_00], 'l1' : [Alpha_1m1, Alpha_10, Alpha_11]}
+    # modes	   = { 'l0' : [Alpha_00], 'l1' : [Alpha_1m1, Alpha_10, Alpha_11]}
     modes_list = [[0, [0]], [1, [-1, 0, 1]]]
     alpha_modes.modes_list = modes_list
     alpha_modes.time_axis = time_axis
     alpha_modes.ell_max = 1
     alpha_modes.spin_weight = -1
     return alpha_modes
 
 
 def boost_waveform(unboosted_waveform, conformal_factor):
     """Boost the waveform given the unboosted waveform and the boost conformal factor.
 
     Parameters
     ----------
-    unboosted_waveform : spherical_array
-                         A class instance of `spherical array`.
 
-    conformal_factor : 2d array
-                       The conformal factor for the Lorentz transformation.
-                       It may be a single floating point number or an array
-                       on a spherical grid. The array will be of dimensions
-                       [ntheta, nphi].
+    unboosted_waveform:		spherical_array
+                                                            A class instance of `spherical array`.
+
+    conformal_factor:		2d array
+                            The conformal factor for the Lorentz transformation.
+                            It may be a single floating point number or an array
+                            on a spherical grid. The array will be of dimensions
+                            [ntheta, nphi].
+
+    gridinfo:		class instance
+                    The class instance that contains the properties of the spherical grid.
 
-    gridinfo : class instance
-               The class instance that contains the properties of the spherical grid.
 
     Returns
     -------
-    boosted_waveform : sp_array
-                       The class instance `sp_array` that
-                       contains the boosted waveform.
+
+    boosted_waveform:	  sp_array
+                                              The class instance `sp_array` that
+                                              contains the boosted waveform.
     """
 
     from waveforms import spherical_array
 
     # Compute the meshgrid for theta and phi.
     # theta, phi = unboosted_waveform.gridinfo.meshgrid
-    #   = unboosted_waveform.gridinfo.phi
+    # 	= unboosted_waveform.gridinfo.phi
     # A list to store the boosted waveform.
     boosted_waveform_data = []
 
     for item in unboosted_waveform.data:
         # Compute the boosted waveform on the spherical grid on all the elements.
 
         # conformal_k_on_sphere = compute_conformal_k(vec_v, theta, phi)
         boosted_waveform_item = conformal_factor * item
 
         boosted_waveform_data.append(boosted_waveform_item)
 
     # Construct a 2d waveform array object
-    boosted_waveform = spherical_array(
-        gridinfo=unboosted_waveform.gridinfo,
-        data=np.array(boosted_waveform_data),
-    )
+    boosted_waveform = spherical_array(gridinfo=unboosted_waveform.gridinfo, data=np.array(boosted_waveform_data))
     boosted_waveform.label = "boosted"
 
     return boosted_waveform
```

### Comparing `waveformtools-2023.6.3/waveformtools/__init__.py` & `waveformtools-2023.6.5/waveformtools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,15 @@
     # print(package_directory)
     # Open the file
     vers = "-1"
     try:
         with open(package_directory + "/../public/version", "r") as vers_file:
             vers = vers_file.readlines()[0]
     except Exception as excep:
-        print(
-            "This is not a git repo! please use the version attribute instead!"
-        )
+        print("This is not a git repo! please use the version attribute instead!")
     # with open(package_directory + "/../public/date.txt", "r") as vers_file:
     # vers = vers_file.read()[:10]
 
     return vers
 
 
-__version__ = "2023.06.03"
+__version__ = "2023.06.05"
```

### Comparing `waveformtools-2023.6.3/waveformtools/compare.py` & `waveformtools-2023.6.5/waveformtools/compare.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,37 +23,29 @@
 # plt.rcParams.update({"axes.labelweight" : "bold"})
 plt.rcParams.update({"font.style": "normal"})
 plt.rcParams.update({"legend.markerscale": 9})
 
 # from waveformtools.waveforms import modes_array
 
 
-def plot_modes(
-    wf1,
-    nmodes=3,
-    save_fig=False,
-    xlim=[-1200, 100],
-    ylim="auto",
-    nstop=1,
-    plot22=False,
-):
+def plot_modes(wf1, nmodes=3, save_fig=False, xlim=[-1200, 100], ylim="auto", nstop=1, plot22=False):
     """Plot the first `nmodes` dominant modes of
     the input waveforms
 
     Parameters
     ----------
-    wf : modes_array
-         The list of `modes_array` waveforms
-         to plot.
-    nmodes : int
-             The number of modes to plot.
+    wf:           modes_array
+                              The list of `modes_array` waveforms
+                              to plot.
+    nmodes:     int
+                            The number of modes to plot.
     xlim : list
            [xmin, xmax] limits to plot.
-    tol : float
-          The tolerance to detect the modes.
+    tol:    float
+                    The tolerance to detect the modes.
 
     Returns
     -------
     Plots.
     """
 
     from waveformtools.waveformtools import xtract_cphase
@@ -105,50 +97,28 @@
         for emm in emm_list:
             mode_values = wf1.mode(ell, emm)
             mode_amp = np.absolute(mode_values)
             max_mode_value = np.amax(mode_values)
 
             mode_phase = xtract_cphase(mode_values.real, mode_values.imag)
 
-            ax1.scatter(
-                wf1.time_axis[:],
-                mode_amp[:],
-                label=rf"$\ell${ell}$m${emm}",
-                s=1,
-                alpha=0.2 * abs(emm) % 1,
-            )
-            ax2.scatter(
-                wf1.time_axis[:],
-                abs(mode_phase[:]),
-                label=rf"$\ell${ell}$m${emm}",
-                s=1,
-            )
+            ax1.scatter(wf1.time_axis[:], mode_amp[:], label=rf"$\ell${ell}$m${emm}", s=1, alpha=0.2 * abs(emm) % 1)
+            ax2.scatter(wf1.time_axis[:], abs(mode_phase[:]), label=rf"$\ell${ell}$m${emm}", s=1)
 
     if plot22:
         ell = 2
         emm = 2
         mode_values = wf1.mode(ell, emm)
         mode_amp = np.absolute(mode_values)
         max_mode_value = np.amax(mode_values)
 
         mode_phase = xtract_cphase(mode_values.real, mode_values.imag)
 
-        ax1.scatter(
-            wf1.time_axis[:],
-            mode_amp[:],
-            label=rf"$\ell${ell}$m${emm}",
-            s=1,
-            alpha=0.2 * abs(emm) % 1,
-        )
-        ax2.scatter(
-            wf1.time_axis[:],
-            abs(mode_phase[:]),
-            label=rf"$\ell${ell}$m${emm}",
-            s=1,
-        )
+        ax1.scatter(wf1.time_axis[:], mode_amp[:], label=rf"$\ell${ell}$m${emm}", s=1, alpha=0.2 * abs(emm) % 1)
+        ax2.scatter(wf1.time_axis[:], abs(mode_phase[:]), label=rf"$\ell${ell}$m${emm}", s=1)
 
     ax1.grid(which="both")
     ax2.grid(which="both")
     ax1.legend()
     ax2.legend()
     plt.tight_layout()
     ax1.set_xlabel("t/M")
@@ -173,34 +143,28 @@
         fig1.savefig(f"{wf1.label}_waveform_amp_modes.pdf")
         fig2.savefig(f"{wf1.label}_waveform_phase_modes.pdf")
 
     plt.show()
 
 
 def plot_mode_differences(
-    waveforms,
-    nmodes=3,
-    save_fig=False,
-    xlabel="t/M",
-    ylabel=r"r\Psi_{4}^{(\ell m)}",
-    labels=None,
-    xlim=[-1000, 100],
+    waveforms, nmodes=3, save_fig=False, xlabel="t/M", ylabel=r"r\Psi_{4}^{(\ell m)}", labels=None, xlim=[-1000, 100]
 ):
     """Plot the fractional difference of the first `nmodes`
     dominant modes of the input waveforms.
 
     Parameters
     ----------
-    waveforms : modes_array
-                The list of `modes_array` waveforms
-                to plot.
-    nmodes : int
-             The number of modes to plot.
-    tol : float
-          The tolerance to detect the modes.
+    waveforms:    modes_array
+                              The list of `modes_array` waveforms
+                              to plot.
+    nmodes:     int
+                            The number of modes to plot.
+    tol:    float
+                    The tolerance to detect the modes.
 
     Returns
     -------
     Plots.
     """
 
     # For phase computation.
@@ -306,17 +270,15 @@
             mode_phase_resam0 = mode_phase_int_fun0(new_time_axis)
 
             for index, wfx in enumerate(waveforms[1:]):
                 label = wfx.label  # labels[index+1]
 
                 mode_valuesx = wfx.mode(ell, emm)
                 mode_ampx = np.absolute(mode_valuesx)
-                mode_phasex = xtract_cphase(
-                    mode_valuesx.real, mode_valuesx.imag
-                )
+                mode_phasex = xtract_cphase(mode_valuesx.real, mode_valuesx.imag)
 
                 mode_amp_int_funx = interp1d(wfx.time_axis, mode_ampx)
                 mode_amp_resamx = mode_amp_int_funx(new_time_axis)
 
                 mode_phase_int_funx = interp1d(wfx.time_axis, mode_phasex)
                 mode_phase_resamx = mode_phase_int_funx(new_time_axis)
 
@@ -330,54 +292,35 @@
                 )
 
                 # mean_phase_shift = np.mean(
                 #   mode_phase_resamx - mode_phase_resam0
                 # )
 
                 # message(mean_phase_shift)
-                delta_mode_ampx = (
-                    mode_amp_resamx - mode_amp_resam0
-                ) / mode_amp_resam0
-                delta_mode_phasex = (
-                    mode_phase_resamx - mode_phase_resam0 - mean_phase_shift
-                ) / mode_phase_resam0
+                delta_mode_ampx = (mode_amp_resamx - mode_amp_resam0) / mode_amp_resam0
+                delta_mode_phasex = (mode_phase_resamx - mode_phase_resam0 - mean_phase_shift) / mode_phase_resam0
 
-                rms_amp_diff = np.sqrt(
-                    np.sum(delta_mode_ampx**2) / (len(delta_mode_ampx))
-                )
-                rms_phase_diff = np.sqrt(
-                    np.sum(delta_mode_phasex**2) / (len(delta_mode_phasex))
-                )
+                rms_amp_diff = np.sqrt(np.sum(delta_mode_ampx**2) / (len(delta_mode_ampx)))
+                rms_phase_diff = np.sqrt(np.sum(delta_mode_phasex**2) / (len(delta_mode_phasex)))
                 max_phase_diff = np.amax(np.absolute(delta_mode_phasex))
                 max_phase_diff_loc = np.argmax(np.absolute(delta_mode_phasex))
                 max_phase_diff_time = new_time_axis[max_phase_diff_loc]
                 cumulative_diff.update(
-                    {
-                        f"l{ell}m{emm}": [
-                            rms_amp_diff,
-                            rms_phase_diff,
-                            [max_phase_diff, max_phase_diff_time],
-                        ]
-                    }
+                    {f"l{ell}m{emm}": [rms_amp_diff, rms_phase_diff, [max_phase_diff, max_phase_diff_time]]}
                 )
                 max_mode_value = np.amax(mode_values)
 
             ax1.scatter(
                 new_time_axis[:],
                 abs(delta_mode_ampx[:]),
                 label=rf"{label} $\ell${ell}$m${emm}",
                 s=1,
                 alpha=0.2 * abs(emm) % 1,
             )
-            ax2.scatter(
-                new_time_axis[:],
-                abs(delta_mode_phasex[:]),
-                label=rf"{label} $\ell${ell}$m${emm}",
-                s=1,
-            )
+            ax2.scatter(new_time_axis[:], abs(delta_mode_phasex[:]), label=rf"{label} $\ell${ell}$m${emm}", s=1)
 
     ax1.grid(which="both")
     ax2.grid(which="both")
     ax1.legend()
     ax2.legend()
     plt.tight_layout()
     ax1.set_xlabel(xlabel)
```

### Comparing `waveformtools-2023.6.3/waveformtools/dataIO.py` & `waveformtools-2023.6.5/waveformtools/simulations.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,1780 +1,1467 @@
-""" Functions for handling data IO operations from waveforms class
+""" Data container for Numerical Relativity data """
 
-"""
-
-#########################
+###############################################
 # Imports
-#########################
-
-import json
-import re
-import sys
+##############################################
 
-import h5py
+import config
 import numpy as np
-from scipy.interpolate import InterpolatedUnivariateSpline as interp
-from scipy.interpolate import interp1d
-
-from waveformtools.waveformtools import (
-    cleandata,
-    interp_resam_wfs,
-    message,
-    xtract_camp_phase,
-)
-
-##########################
-# RIT data
-##########################
-
-
-def _key_gen(ell, emm, extras=None):
-	"""Generates strings to be used as keys for
-	managing h5 datasets.
-
-    Parameters
-    ----------
-    ell : int
-          The polar angular mode number
-          :math:`\\ell`.
-    emm : int
-          The aximuthal angular mode number
-          :math:`m`.
-    extras : str
-             Any extra string to be appended
-             to the end of the key.
-
-    Returns
-    -------
-    key : str
-          A key string.
-    """
 
-	key = f"l{ell}_m{emm}"
+from waveformtools.waveformtools import cleandata, message
 
-	if extras is not None:
-		key += f"_{extras}"
-		# message('adding rext')
+# import waveformtools
 
-	return key
 
+class sim:
+    """A data container for simulation data.
 
-def get_ell_max_from_keys(all_keys):
-	"""Get ell max from a list of keys.
-
-    Parameters
+    Arrtibutes
     ----------
-    all_keys : list
-               A list of strings string containing the modes keys.
-    Returns
-    -------
-    ell_max : int
-              The maximum available ell.
-    """
 
-	# available mode numbers
-	all_ell_modes = set({})
+    ROOTDIR:	string
+                            Root directory as a string containing the simulation folders.
 
-	# Get mode numbers
-	for item in all_keys:
-		this_match = re.search("\_l\d\_", item)
+    WAVDIR:	string
+                            Root directory as a string containing the simulation directies containing the wavefom data.
 
-		if this_match is None:
-			# message(f'Skipped file {item}')
-			continue
+    data_dir:	string
+                            The path of the folder containing data relative to the simulation direcory.
 
-        # message('Match found', this_match.string)
-        s1, s2 = this_match.span()
-        this_ell = int(this_match.string[s1 + 2 : s2 - 1])
-        # message(this_ell)
+    strain_dir:	string
+                                    The path of the folder containing the waveform data relative to the strain directory.
 
-		all_ell_modes.add(this_ell)
+    aliases:	a list of strings
+                            The names/aliases for the simulations.
 
-	ell_max = max(all_ell_modes)
-	return ell_max
+    multipoles:	dict of lists
+                                    The multipole moments of the simulation as a dictionary.
+                                    Each entry is a list of width 4 with axis 0 the timeaxis of multipoles.
 
+    mass1:	dict of floats
+                    The BH1 horizon mass.
 
-def get_ell_max_from_file(data_dir, var_type="Psi4", file_name="*.h5"):
-    """Get the largest available mode number from available data in files.
+    mass2:	dict of floats)
+                    The BH2 horizon mass.
 
-    Parameters
-    ----------
-    data_dir : string
-               A string containing the directory path where the mode files can be found.
-    var_type : string, optional
-               A string that denotes the variable
-               that is being loaded. Options are Psi4
-               and strain. The former is the default.
-    file_name : string, optional
-                The h5 file that contains the modes data.
-                It defaults to the only file in the directory.
-                If there are multiple files, it throws an error.
+    mass3:	dict of floats
+                    The BH3 horizon mass.
 
-    Returns
-    -------
-    ell_max : int
-              The maximum available ell.
-    keys_list : list
-                A list of data access keys.
-
-    Notes
-    -----
-    Reads in various ASCII dat files for RIT Psi4, h5 files for RIT strain and gen strain.
-    """
+    delta_t:	dict of floats
+                            The time stepping in simulation units (delta_t/M).
 
-    if var_type == "Psi4":
-        import os
+    timeaxis:	dict of 1d arrays
+                            The timeaxis of the simulations.
 
-        # Get files
-        all_fnames = os.listdir(data_dir)
-        # Get only files
-        all_fnames = [
-            item for item in all_fnames if os.path.isfile(f"{data_dir}/{item}")
-        ]
+    distance:	dict of 1d arrays
+                            The distances of simulations.
 
-    elif var_type == "Strain":
-        # import h5py
-        message("Fetching all keys from H5 file", message_verbosity=2)
-        data_file = h5py.File(f"{data_dir}/{file_name}")
-        all_fnames = list(data_file.keys())
-        data_file.close()
-        # message(all_fnames)
+    merger_ind:	dict of ints
+                                    The merger index/ common horizon formation index of simulations.
 
-    # Parse ell values
-    # Filter the keys.
-    all_fnames = [item for item in all_fnames if "_l" in item]
+    dinit:	dict of floats
+                    The initial distances.
 
-    message("All files found", all_fnames, message_verbosity=3)
+    multipoles:	dict of lists
+                                    The two sets of  mass multipoles of the three horizons. Axis 0 is usuall the time array.
 
-    ell_max = get_ell_max_from_keys(all_fnames)
+    mass_multipoles:	dict of lists
+                                            The mass multipoles upto (ell=8).
 
-    return ell_max, all_fnames
+    spin_multipoles:	dict of lists
+                                            The spin multipoles upto (l=8).
 
+    data_length:	dict of float
+                                    The data length of the multipole simulation data loaded.
 
-def _get_modes_list_from_keys(keys_list, r_ext):
-	"""Get the modes list from the keys list
-	of an hdf file.
+    dist_data_length:	dict of ints
+                                            The data length of distances of simulations.
 
-    Parameters
-    ----------
-    keys_list : list
-                The list containing all the keys
-    r_ext : float
-            The extraction radius of the data.
+    merger_distance:	dict of floats
+                                            The distance between the blackholes at the merger index.
 
-    Returns
-    -------
-    modes_list : list
-                 The list of modes.
-    """
-
-	# Sort the keys to ensure a nice
-	# modes list structure.
-	keys_list_orig = sorted(keys_list)
-
-	if r_ext != -1:
-		keys_list = [item for item in keys_list_orig if f"r{r_ext}" in item]
-
-        if keys_list == []:
-            message(
-                "Got an empty list. Searching for r_ext value in key string"
-            )
-            keys_list = [item for item in keys_list_orig if f"{r_ext}" in item]
-
-	# message('List of keys received', keys_list)
-	# The list of modes.
-	modes_list = []
-
-	# Initialize the emm modes sublist.
-	emm_modes_for_ell = []
+    true_merger_dist:	dict of floats
+                                            The true merger distance (non-normalized).
 
-	# Present ell value to
-	# initialize the mode concatenation.
-	ell_old = 0
+    sampling_f:	dict of floats
+                                    The sampling frequency of simulations (1/delta_t).
 
-	for key in keys_list:
-		# message(key)
-		# Get the ell value
-		ell_value, emm_value = _get_ell_emm_from_key(key)
+    merger_time:	dict of floats
+                                    The cctk_time stamp at merger.
 
-		if ell_value != ell_old:
-			# If the ell value has changed,
-			# update the modes list before moving
-			# onto the next ell value.
-			modes_list.append([ell_old, emm_modes_for_ell])
-			# The present ell value is the old
-			# ell value.
-			ell_old = ell_value
+    massratio:	dict of floats
+                            The massratio of the simulations.
 
-			# Reset the ell_mode list.
-			emm_modes_for_ell = []
+    chirpmass:	dict of floats
+                            The chirpmass of the simulations.
 
-		# Update it with the new emm mode.
-		emm_modes_for_ell.append(emm_value)
+    totalmass:	dict of floats
+                            The total mass of the simulations.
 
-	modes_list.append([ell_value, emm_modes_for_ell])
+    log_multipoles:	dict of lists
+                    The natural logarithm of the negative
+                    of the multipole moments as
+                    a list [time, multipole1, multipole2, multipole3(if exists)].
 
-	return modes_list
+    data_duration:	dict of floats
+                    The total cctk_time units of simulations present.
+    BH_locations:	dict of lists.
+                    A dictionary of values containing BH
+                    locations of every simulation. Each
+                    simulation has three lists, one for
+                    each black hole.
 
+    CoM_locations:	dict of lists
+                    A dictionary of lists containing the
+                    X, Y and Z locations of the CoM of the simulations.
+    NP_1d:	dict
+                    A dict of dicts of lists containig
+                    the 1d Newman Penrose data from simulations.
 
-def _get_ell_emm_from_key(key):
-	"""Get the :math:`\\ell` and :math:`m` values
-	from a given key string of an hdf file.
-
-    Parameters
-    ----------
-    key : str
-          The input key string
-
-    Returns
+    Methods
     -------
-    ell_value : int
-                The :math:`\\ell` value
-    emm_value : int
-                The :math:`m` value.
-
-    Notes
-    -----
-    Assumes that the input string has :math:`\\ell` and :math:`m` values
-    in the form `l{int}m{int}`.
-
-	"""
-
-	import re
-
-    str_match = re.search("l\d*", key)
-    ell_str_start = str_match.start()
-    ell_str_end = str_match.end()
-    ell_value = int(key[ell_str_start + 1 : ell_str_end])
+    calc_ref_multipoles
+            Calculate the reference multipoles
+            as time average of first few timesclices
+            of (2) multipole moment data.
+
+            Assignes/Updates:
+                    * ref_multipoles.
+
+    calc_log_multipoles
+            Calculate the natural logarithm
+            of the negative of the two sets
+            of multipole moment.
+            Assignes/ Updates:
+                    * log_multipoles.
+
+    calc_delta_multipoles
+            Calculate the two delta multipoles - ref multipoles.
+            Assignes/ Updates:
+                    * delta_multipoles.
+
+    calc_amp_phase
+            Extract the amplitudes and phases of the strain waveforms.
+            Assignes/Updates:
+                    * strain_amp
+                    * strain_phase.
+
+    load_data
+            Load the multipole and distance data of the simulations.
+            Assignes/Updates:
+                    * distance.
+                    * dinit.
+                    * mass1.
+                    * mass2.
+                    * merger_index.
+                    * merger_time.
+                    * merger_distance.
+                    * true_merger_distance.
+                    * data_length.
+                    * data_duration.
+                    * multipoles.
+                    * mass_multipoles.
+                    * spin_multipoles.
+
+    load_strain
+            Load the strain data of the simulations from waveform directories.
+            Assignes/Updates:
+                    * strain.
+                    * strain_amp.
+                    * strain_phase.
+                    * strain_shift.
+
+    load_shears
+            Load the shear data at a pole of
+            respective horizons of the simulations
+            from waveform directories.
+            Assignes/Updates:
+                    * shear.
+                    * shear_amp.
+                    * shear_phase.
+                    * shear_shift.
+
+    ret_horizon_radii
+            A method to retrieve the areal radii of the horizons.
+            Assigns/Updates
+                    * areal_radii
+
+    _resize_multipoles
+            Private method to resize the
+            sim.multipoles after retrieving
+            the length of distance.
+
+    _ifreversal
+            Private method to reverse the data
+            of BH 1 and 2 if mass2 > mass1.
 
-    str_match = re.search("m-*\d*", key)
-    emm_str_start = str_match.start()
-    emm_str_end = str_match.end()
-    emm_value = int(key[emm_str_start + 1 : emm_str_end])
-
-	return ell_value, emm_value
-
-
-def get_iteration_numbers_from_keys(keys_list):
-	"""Get the iteration number from keys.
-
-    Parameters
-    ----------
-    keys_list : list
-                The list of keys.
-
-    Returns
-    -------
-    iteration_numbers : list
-                        The list containing the iteration
-                        numbers.
     """
-    import re
-
-	iteration_numbers = []
-
-    for key in keys_list:
-        str_match = re.search(" it=\d* ", key)
-        it_str_start = str_match.start()
-        it_str_end = str_match.end()
-        it_value = int(key[it_str_start + 4 : it_str_end])
-        iteration_numbers.append(it_value)
-
-	return iteration_numbers
-
-
-def construct_mode_list(ell_max, spin_weight):
-    """Construct a modes list in the form
-    [[ell1, [emm1, emm2, ...], [ell2, [emm..]],..]
-    given the :math:`\\ell_{max}.`
-
-    Parameters
-    ----------
-    spin_weight : int
-                  The spin weight of the modes.
-    ell_max : int
-              The :math:`\\ell_{max}` of the modes list.
-
-    Returns
-    -------
-    modes_list : list
-                 A list containg the mode indices lists.
 
-	Notes
-	-----
-	The modes list is the form which the `waveform` object understands.
-	"""
+    def __init__(
+        self,
+        # Variables for initialization.
+        aliases=None,
+        multipoles=None,
+        mass_multipoles=None,
+        spin_multipoles=None,
+        mass1=None,
+        mass2=None,
+        mass3=None,
+        delta_t=None,
+        merger_ind=None,
+        actmerger_time=None,
+        timeaxis=None,
+        dinit=None,
+        distance=None,
+        ROOTDIR=None,
+        WAVDIR=None,
+        simdir=None,
+        data_dir="data/primary/",
+        data_length=None,
+        dist_data_length=None,
+        comm_data_length=None,
+        strain_dir="output/",
+        strain=None,
+        strain_phase=None,
+        strain_frequency=None,
+        strain_amplitude=None,
+        strain_indexshifts=None,
+        indexjn=None,
+        distjn=None,
+        areal_radii={},
+        log_deltamultipoles2=None,
+        log_multipoles2=None,
+        log_deltamultipoles=None,
+        log_multipoles=None,
+        ref_multipoles=None,
+        indjn=None,
+        NP_1d=None,
+    ):
+        # Load the variables at initialization.
+        self.aliases = aliases or {}
+        self.multipoles = multipoles or {}
+        self.spin_multipoles = spin_multipoles or {}
+        self.mass_multipoles = mass_multipoles or {}
+        self.mass1 = mass1 or {}
+        self.mass2 = mass2 or {}
+        self.mass3 = mass3 or {}
+        self.delta_t = delta_t or {}
+        self.timeaxis = timeaxis or {}
+        self.distance = distance or {}
+        self.merger_ind = merger_ind or {}
+        self.actmerger_time = actmerger_time or {}
+        self.dinit = dinit or {}
+        self.data_length = data_length or {}
+        self.dist_data_length = dist_data_length or {}
+        self.comm_data_length = comm_data_length or {}
+        self.strain = strain or {}
+        self.strain_phase = strain_phase or {}
+        self.strain_frequency = strain_frequency or {}
+        self.strain_amplitude = strain_amplitude or {}
+        self.strain_indexshifts = strain_indexshifts or {}
+        self.indexjn = indexjn or {}
+        self.distjn = distjn or {}
+        self.ROOTDIR = ROOTDIR
+        self.WAVDIR = WAVDIR
+        self.simdir = simdir
+        self.strain_dir = strain_dir
+        self.data_dir = data_dir
+        self.areal_radii = areal_radii
+        self.log_deltamultipoles2 = log_deltamultipoles2
+        self.log_multipoles2 = log_multipoles2
+        self.log_deltamultipoles = log_deltamultipoles
+        self.log_multipoles = log_multipoles
+        self.ref_multipoles = ref_multipoles
+        self.indjn = indjn
+        self.NP_1d = NP_1d
+
+    @property
+    def data_duration(self):
+        """Compute and return the data duration of the simulations."""
+        return {alias: self.data_length[alias] * self.delta_t[alias] for alias in self.aliases}
+
+    @property
+    def comm_data_duration(self):
+        """Compute and return the duration of
+        the common data (multipole and Bhdiag/distance)
+        of the simulations."""
+        return {alias: self.comm_data_length[alias] * self.delta_t[alias] for alias in self.aliases}
+
+    @property
+    def pm_data_duration(self):
+        """Compute and return the duration
+        of post-merger data present in the simulations."""
+        return {alias: self.data_duration[alias] - self.merger_time[alias] for alias in self.aliases}
+
+    @property
+    def pm_data_length(self):
+        """Compute and return the post merger
+        data length avaialable for all simulations."""
+        return {alias: self.data_length[alias] - self.merger_ind[alias] for alias in self.aliases}
+
+    @property
+    def merger_distance(self):
+        """Compute and return the distance
+        at the merger index of the simulations."""
+        merger_dist = {}
+        for alias in self.aliases:
+            try:
+                merger_dist.update({alias: self.distance[alias][self.merger_ind[alias]]})
+            except IndexError:
+                if (self.merger_ind[alias] - len(self.distance[alias])) == 1:
+                    merger_dist.update({alias: self.distance[alias][self.merger_ind[alias] - 1]})
+                else:
+                    message("%s :Distance upto merger not defined. Setting final value" % alias)
+                    merger_dist.update({alias: self.distance[alias][-1]})
+        return merger_dist
+
+    @property
+    def true_merger_distance(self):
+        """Compute and return the true
+        (i.e. non-normalized) distance at merger for the simulations."""
+        return {alias: self.dinit[alias] * self.merger_distance[alias] for alias in self.aliases}
+
+    @property
+    def sampling_f(self):
+        """Compute and return the sampling frequency of the simulations."""
+        return {alias: 1.0 / self.delta_t[alias] for alias in self.aliases}
+
+    @property
+    def merger_time(self):
+        """Compute and return the
+        cctk_time stamp at the merger
+        for the simulations."""
+        return {alias: self.merger_ind[alias] * self.delta_t[alias] for alias in self.aliases}
+
+    @property
+    def massratio(self):
+        """Compute and return the massratio of the simulations."""
+        return {alias: self.mass2[alias] / self.mass1[alias] for alias in self.aliases}
+
+    @property
+    def chirpmass(self):
+        """Compute and return the chirp mass of the simulations."""
+        return {
+            alias: ((self.mass1[alias] * self.mass2[alias]) ** (3.0 / 5))
+            / (self.mass1[alias] + self.mass2[alias]) ** (1.0 / 5)
+            for alias in self.aliases
+        }
+
+    @property
+    def totalmass(self):
+        """Compute and return the total mass of the simulations."""
+        return {alias: self.mass1[alias] + self.mass2[alias] for alias in self.aliases}
+
+    def calc_junkend(self, tjn=200.0):
+        """Compute the indices and the starting distances
+        of the system at timestamp t = 200.
+
+        Parameters
+        ----------
+
+        tjn:	float
+                        The definition of time end of junk radiation. Default is 200.
+
+        Notes
+        -----
+        Computes:
+
+        self.indjn:	dict
+                                        A dictionary containing the index location
+                                        corresponding to timestamp tjn.
+        self.distjn:	dict
+                                        A dictionary containing the normalized co-ordinate
+                                        distance between the two BHs at tjn.
+
+        """
+
+        # Find the starting distance at t = 200M.
+        # Initialize the directory.
+        self.indjn = {}
+        for alias in self.aliases:
+            # Iterate over simulations.
+            # Find the index corresponding to the timestamp tjn.
+            indjn = np.argmin(np.absolute(self.timeaxis[alias] - tjn))
+            # Update the sjn dictionary.
+            self.indjn.update({alias: indjn})
+            # message(len(sim_A.distance[alias]), ind)
+            # Update th djn dictionary.
+            self.distjn.update({alias: self.distance[alias][1][indjn]})
+        # Return 1
+        return 1
+
+    def calc_ref_multipoles(self):
+        """Compute and assign the reference (l=2) multuipoles to sim.ref_multipoles of the simulations."""
+        refmult = {}
+        # index = 0
+        for alias in self.aliases:
+            message(alias)
+            item = np.transpose(self.multipoles[alias])
+            ml_length = len(item[:, 0])
+            if ml_length < self.comm_data_length[alias]:
+                self.comm_data_length[alias] = ml_length
+                self.distance[alias] = self.distance[alias][:ml_length]
+            message(item.shape)
+            """Unpack data as 1d arrays"""
+            _, Ml12, Ml22, Ml32 = (
+                item[: self.comm_data_length[alias], 0],
+                item[: self.comm_data_length[alias], 1],
+                item[: self.comm_data_length[alias], 2],
+                item[self.merger_ind[alias] :, 3],
+            )
+            """Compute delta multipoles"""
+            Ml12_ref = np.mean(Ml12[30:100])
+            Ml22_ref = np.mean(Ml22[30:100])
+            Ml32_ref = np.mean(Ml32[-100:])
+
+            refmult.update({alias: [Ml12_ref, Ml22_ref, Ml32_ref]})
+            self.ref_multipoles = refmult
+
+    def calc_log_multipoles(self):
+        """Compute and assign the natural logarithm of the (l=2) multipoles to sim.log_multipoles of the simulations."""
+        log_mult = {}
+        for alias in self.aliases:
+            message(alias)
+            item = np.transpose(self.multipoles[alias])
+            ml_length = len(item[:, 0])
+            if ml_length < self.comm_data_length[alias]:
+                self.comm_data_length[alias] = ml_length
+                self.distance[alias] = self.distance[alias][:ml_length]
+            message(item.shape)
+            log_mult.update(
+                {
+                    alias: [
+                        item[: self.comm_data_length[alias], 0],
+                        np.log(np.absolute(-item[: self.comm_data_length[alias], 1])),
+                        np.log(np.absolute(-item[: self.comm_data_length[alias], 2])),
+                        np.log(np.absolute(-item[self.merger_ind[alias] :, 3])),
+                    ]
+                }
+            )
+        self.log_multipoles = log_mult
 
-	# The modes list.
-	modes_list = []
+    def calc_delta_multipoles(self):
+        """Compute and return the delta multipoles (w.r.t. reference (l=2) multipoles)"""
+        log_deltmult = {}
+        for alias in self.aliases:
+            message(alias)
+            # Multipole data
+            item = np.transpose(self.multipoles[alias])
+            """Length of multipoles"""
+            ml_length = len(item[:, 0])
+            """Check the lengths of multipole and distance data"""
+            if ml_length < self.comm_data_length[alias]:
+                """Reset the datalengths"""
+                self.comm_data_length[alias] = ml_length
+                """Resize the distance array"""
+                self.distance[alias] = self.distance[alias][:ml_length]
+            message(item.shape)
+            """Unpack data as 1d arrays"""
+            time, Ml12, Ml22, Ml32 = (
+                item[: self.comm_data_length[alias], 0],
+                item[: self.comm_data_length[alias], 1],
+                item[: self.comm_data_length[alias], 2],
+                item[self.merger_ind[alias] :, 3],
+            )
+            """Compute delta multipoles"""
+            Ml12_ref = np.mean(Ml12[30:100])
+            Ml22_ref = np.mean(Ml22[30:100])
+            Ml32_ref = np.mean(Ml32[-100:])
+            dMl12 = Ml12 - Ml12_ref
+            dMl22 = Ml22 - Ml22_ref
+            dMl32 = Ml32 - Ml32_ref
 
-	for ell_index in range(abs(spin_weight), ell_max + 1):
-		# Append all emm modes for each ell mode.
-		modes_list.append([ell_index, list(range(-ell_index, ell_index + 1))])
+            log_deltmult.update(
+                {alias: [time, np.log(np.absolute(-dMl12)), np.log(np.absolute(-dMl22)), np.log(np.absolute(-dMl32))]}
+            )
 
-	return modes_list
+        self.log_deltamultipoles = log_deltmult
 
+    def calc_log_multipoles2(self):
+        """Compute and assign the natural logarithm of the (l=2) multipoles to sim.log_multipoles of the simulations."""
+        log_mult = {}
+        for alias in self.aliases:
+            message(alias)
+            item = np.transpose(self.multipoles[alias])
+            ml_length = len(item[:, 0])
+            if ml_length < self.comm_data_length[alias]:
+                self.comm_data_length[alias] = ml_length
+                self.distance[alias] = self.distance[alias][:ml_length]
+            message(item.shape)
+            log_mult.update(
+                {
+                    alias: [
+                        item[: self.comm_data_length[alias], 0],
+                        np.log(-item[: self.comm_data_length[alias], 1]),
+                        np.log(-item[: self.comm_data_length[alias], 2]),
+                        np.log(-item[self.merger_ind[alias] :, 3]),
+                    ]
+                }
+            )
+        self.log_multipoles2 = log_mult
 
-def sort_keys(modes_keys_list):
-    """Sort the keys in a list based on
-    its iteration number
+    def calc_delta_multipoles2(self):
+        """Compute and return the delta multipoles (w.r.t. reference (l=2) multipoles)"""
+        log_deltmult = {}
+        for alias in self.aliases:
+            message(alias)
+            # Multipole data
+            item = np.transpose(self.multipoles[alias])
+            """Length of multipoles"""
+            ml_length = len(item[:, 0])
+            """Check the lengths of multipole and distance data"""
+            if ml_length < self.comm_data_length[alias]:
+                """Reset the datalengths"""
+                self.comm_data_length[alias] = ml_length
+                """Resize the distance array"""
+                self.distance[alias] = self.distance[alias][:ml_length]
+            message(item.shape)
+            """Unpack data as 1d arrays"""
+            time, Ml12, Ml22, Ml32 = (
+                item[: self.comm_data_length[alias], 0],
+                item[: self.comm_data_length[alias], 1],
+                item[: self.comm_data_length[alias], 2],
+                item[self.merger_ind[alias] :, 3],
+            )
+            """Compute delta multipoles"""
+            Ml12_ref = np.mean(Ml12[30:100])
+            Ml22_ref = np.mean(Ml22[30:100])
+            Ml32_ref = np.mean(Ml32[-100:])
+            dMl12 = Ml12 - Ml12_ref
+            dMl22 = Ml22 - Ml22_ref
+            dMl32 = Ml32 - Ml32_ref
+
+            log_deltmult.update({alias: [time, np.log(-dMl12), np.log(-dMl22), np.log(dMl32)]})
+
+        self.log_deltamultipoles2 = log_deltmult
+
+    def load_data(self):
+        """Load data of the simulations.
+
+        Notes
+        -----
+
+        Data is assigned to
+
+                        multipoles:	list
+                        mass_multipoles:	list
+                        spin_multipoles:	list
+                        timeaxis:	list
+                        mass1:	float
+                        mass2:	float
+                        mass3:	float
+                        delta_t:	float
+                        distance:	list
+                        merger_ind:	int
+                        actmerger_time:	float
+                        dinit:	float
+                        data_length:	int
+                        dist_data_length:	int
+
+        """
+        """ Common variables """
+        multipoles_one = []
+        masses_one = []
+        masses_one_all = []
+        M1_one = []
+        M2_one = []
+        M3_one = []
+        delta_t_one = []
+        timeaxis_one = []
+        # Multipole variables
+
+        all_mass_multipoles_one = []
+        all_spin_multipoles_one = []
+
+        # Load Distances
+        d_one = []
+        timeaxis_one = []
+        act_shape_one = []
+        d0_one = []
+        merger_time_one = []
+
+        ml_data_length = []
+
+        dist_data_length = []
+        all_mass_multipoles_1 = []
+        all_mass_multipoles_2 = []
+        all_mass_multipoles_3 = []
+
+        all_spin_multipoles_1 = []
+        all_spin_multipoles_2 = []
+        all_spin_multipoles_3 = []
+
+        # simulation directories.
+        sim1 = [item + "/" for item in self.aliases]
+        # Array for merger index.
+        ind_merger_one = np.zeros(len(self.aliases), dtype=np.int) - 1
+
+        for sim_index in range(0, len(self.aliases)):
+            # Loop over simulations.
+
+            message(self.aliases[sim_index])
+            message("------------------")
+
+            # Load the qlm_multipole moment data.
+            file0 = np.genfromtxt(
+                self.ROOTDIR + sim1[sim_index] + self.data_dir + "quasilocalmeasures-qlm_multipole_moments..asc"
+            )
 
-    Parameters
-    ----------
-    modes_keys_list : str
-                      The list of keys.
+            # Assign the timeaxis.
+            cctk_time = file0[:, 8]
 
-    Returns
-    -------
-    sorted_modes_keys_list : str
-                             The sorted list.
-    """
+            # Assign the multipole data lengths to a list.
+            ml_data_length.append(len(cctk_time))
 
-	iteration_numbers = get_iteration_numbers_from_keys(modes_keys_list)
+            # Assign the timeaxis to a list.
+            timeaxis_one.append(cctk_time)
+            # Assign the time stepping to a list.
+            delta_t_one.append(cctk_time[1] - cctk_time[0])
+            # Load the BH horizon masses.
+            M1_one_all = file0[:, 12]
+            M2_one_all = file0[:, 13]
+            M3_one_all = file0[:, 14]
+
+            ###################################################################
+            # I.
+            # 	1. Load multipole data.
+            # 	2. Mass data.
+            # 	3. Find merger index.
+            ###################################################################
+
+            # Lists to hold mass multipole data of the three horizons of a
+            # simulation.
+            amm1 = []
+            amm2 = []
+            amm3 = []
+
+            # Lists to hold spin multipole data of the three horizons of a
+            # simulation.
+            asm1 = []
+            asm2 = []
+            asm3 = []
+
+            for col in range(0, 9):
+                # Extract the mass multipole data.
+                amm1.append(file0[:, 12 + col * 3])
+                amm2.append(file0[:, 13 + col * 3])
+                amm3.append(file0[:, 14 + col * 3])
+
+                # Extract the spin multipole data.
+                asm1.append(file0[:, 39 + col * 3])
+                asm2.append(file0[:, 40 + col * 3])
+                asm3.append(file0[:, 41 + col * 3])
+
+            # check for data continuity
+            # Load a set of data to chek into a list.
+            data0 = [cctk_time, M1_one_all, M2_one_all, M3_one_all]
+
+            # Prepend the timeaxis to the mass multipoles.
+            data1 = [cctk_time] + amm1
+            data2 = [cctk_time] + amm2
+            data3 = [cctk_time] + amm3
+
+            # Prepend the timeaxis to the spin multipoles
+            # message(len(data1), len(amm1))
+
+            data4 = [cctk_time] + asm1
+            data5 = [cctk_time] + asm2
+            data6 = [cctk_time] + asm3
+
+            # Clean the data using handles.cleandata.
+            # Collect the data set 1.
+            cctk_time, M1_one_all, M2_one_all, M3_one_all = cleandata(data0)
+
+            # Collect the cleaned data set 2 and 3.
+            cctk_time, *amm1 = cleandata(data1)
+            cctk_time, *amm2 = cleandata(data2)
+            cctk_time, *amm3 = cleandata(data3)
+
+            cctk_time, *asm1 = cleandata(data4)
+            cctk_time, *asm2 = cleandata(data5)
+            cctk_time, *asm3 = cleandata(data6)
+
+            # Find the merger index.
+            # Note: This may not work if no merger has happened. This captures
+            # the length of data in that case.
+
+            # Use the first non-zero index of mass3 array common horizon as the
+            # merger index.
+
+            # Append to merger_one_a.
+            try:
+                # Try to find the non-zero index of horizon mass3.
+                merger_one_a = np.where(M3_one_all != 0)[0]
+
+            except BaseException:
+                # Else set merger_one_a to length of mass3.
+                merger_one_a = len(M3_one_all)
+                message(
+                    "Mass3 not non-zero anywhere in the data."
+                    "Merger has probably not happened yet."
+                    " Reverting to data length."
+                )
+            # When merger happens, the BH horizon masses
+            # mass1 and mass2 acquire the same mass as the
+            # common horizon. Find the index where mass1
+            # jumps by more than 0.1.
+            # Assign to merger_one.
+
+            try:
+                # Try to find the jump location of the horizon mass1 data.
+                merger_one = np.where(np.diff(M1_one_all) > 0.1)[0]
+
+            except BaseException:
+                merger_one = len(M1_one_all)
+                message("Mass1 has no jumps. Merger has probably not happened. Reverting to data length.")
+
+            message("Merger index (through jump in mass1):", merger_one)
+
+            if merger_one_a.any() and merger_one.any():
+                # If both indices have been found, select the least of the two
+                # as merger index.
+                merger_one = min(merger_one_a[0], merger_one[0])
 
-	sargs = np.argsort(iteration_numbers)
+                if merger_one == merger_one_a[0]:
+                    message("Merger data set from Mass3.")
 
-	sorted_modes_keys_list = np.array(modes_keys_list)[sargs]
+                else:
+                    message("Merger data set from Mass1 jump.")
 
-	return sorted_modes_keys_list
+            elif not merger_one_a.any() and not merger_one.any():
+                # If index of non-zero mass3 and mass1 jump was not found,
+                # declare no merger data exists.
+                message("No merger data exists")
+                merger_one = -1
 
+            else:
+                # If both indices are not equal, declare inconsistency but
+                # accept the result from either.
 
-def load_RIT_Psi4_data_from_disk(
-	wfa=None,
-	data_dir="./",
-	label="RIT_rPsi4inf",
-	ell_max=None,
-	modes_list=None,
-	save_as_ma=False,
-	spin_weight=-2,
-	resam_type="finest",
-	interp_kind="cubic",
-	crop=False,
-	centre=False,
-):
-    """Load the Psi4 waveforms from the RIT catalogue
-    from ASCII files from disk.
+                message("Merger index inconsistency found. Mergertime may not be correct")
 
-    Parameters
-    ----------
-    wfa : waveforms
-          An instance of the waveforms class. Updates this instance
-          if provided, else creates a new instance.
-    data_dir : string
-               A string containing the directory path where
-               the mode files can be found.
-    label : string, optional
-            The label of the modes_array object.
-    ell_max : int, optional
-              The maximum mode number to load. If not specified,
-              then all available modes are loaded.
-    save_as_ma : bool, optional
-                 Save to disk again as a modes_array h5 file?
-    spin_weight : int, optional
-                  The spin weight of the object. Used for filtering modes.
-                  Defaults to -2.
-    resam_type : string, float, optional
-                 The type of resampling to do. Options are the
-                 `finest` and `coarsest`, or user input float.
-    interp_kind : string, optional
-                  The interpolation type to use. Default is cubic.
+                try:
+                    # First try with non-zero mass3 index.
+                    merger_one = merger_one[0]
+                    message("Merger time set from Mass3")
+                except BaseException:
+                    # Else assign from mass1 jump.
+                    merger_one = merger_one_a[0]
+                    message("Merger time set from Mass1 jump")
 
-    Returns
-    -------
-    rit_modes_array : modes_array
-                      A modes_array instance containing the loaded modes.
+            # Declare merger time.
+            message("Merger time:", delta_t_one[sim_index] * merger_one)
+            message("Merger index:", merger_one)
 
-    Notes
-    -----
-    It seems like the time axis of individual modes are
-    identical to each other. Hence, one need not worry about
-    choosing the time domain. This may change in future.
-    """
-    message("Loading RIT Psi4 type data.", message_verbosity=1)
-    from waveformtools.waveforms import modes_array
+            # Update the merger index of the simulation.
+            ind_merger_one[sim_index] = merger_one
 
-    if not wfa:
-        wfa = modes_array(label=label, data_dir=data_dir, modes_list=modes_list)
+            # Load the masses.
 
-    if modes_list is None:
-        # Max available mode l.
-        if ell_max is None:
-            ell_max, _ = get_ell_max_from_file(data_dir)
-
-        # Construct a modes list
-        wf_modes_list = construct_mode_list(
-            ell_max=ell_max, spin_weight=spin_weight
-        )
-
-        message("The modes list is", wf_modes_list, message_verbosity=2)
-
-    else:
-        ell_max = max([item[0] for item in modes_list])
-        wf_modes_list = modes_list
-
-    wfa.ell_max = ell_max
-    wfa.modes_list = wf_modes_list
-    wfa.r_ext = np.inf
-    # For interpolation
-    from scipy.interpolate import interp1d
-
-    # Alias of the modes_array
-    # label = 'q1a0_a'
-    # Create a modes array
-    # Enforce only l>2 modes.
-    wf_modes_list = [
-        item for item in wf_modes_list if item[0] >= abs(spin_weight)
-    ]
-
-    # tend = []
-    # tstart = []
-
-    ##########################################
-    # Read in the data
-    #########################################
-
-    message("Reading in modes...")
-    for ell, emm_list in wf_modes_list:
-        for emm in emm_list:
-            message("Loading", ell, emm)
-            # Construct file path
-            wf_psi4_file_path = data_dir + f"/rPsi4_l{ell}_m{emm}_rInf.asc"
-            # Read in the data
-            wf_psi4_file = np.genfromtxt(wf_psi4_file_path)
-
-            # Get time axis
-            wf_psi4_time = wf_psi4_file[:, 0]
-            # tend.append(len(wf_psi4_time))
-            # tstart.append(wf_psi4_time[0])
-            # tend.append(wf_psi4_time[-1])
-
-            # message(f'Tmin {wf_psi4_time[0]}, tmax{wf_psi4_time[-1]}')
-            # Create modes_array on first run
-
-            # message(wfa.modes_data)
-            if wfa.modes_data.all() == np.array(None):
-                message("Creating modes data")
-
-                min_dt = round(min(np.diff(wf_psi4_time)), 2)
-                max_dt = round(max(np.diff(wf_psi4_time)), 2)
-                message(f"Min dt {min_dt} and Max dt {max_dt}")
-
-                if resam_type == "finest":
-                    # Choose finest available timestep
-                    # for upto 3 decimal digits.
-                    m_dt = min_dt
-                    message("Resampling at the finest timestep", m_dt)
-                if resam_type == "coarsest":
-                    m_dt = max_dt
-                    message("Resampling at the coarsest timestep", m_dt)
-
-                if isinstance(resam_type, float):
-                    m_dt = resam_type
-                    message("Resampling at user defined timestep", m_dt)
-
-                # New (resampled) time axis
-                time_axis = np.arange(
-                    wf_psi4_time[0], wf_psi4_time[-1] + m_dt, m_dt
-                )
+            M1_one.append(np.mean(M1_one_all[200:300]))
+            M2_one.append(np.mean(M2_one_all[200:300]))
+            M3_one.append(np.mean(M3_one_all[-100:]))
 
-                # Length of data.
-                data_len = len(time_axis)
+            # Load the (l=2) multipoles.
+            Ml12_one = file0[:, 18]
+            Ml22_one = file0[:, 19]
+            Ml32_one = file0[:, 20]
 
-                # Create a modes array object
-                wfa.create_modes_array(ell_max=ell_max, data_len=data_len)
+            # message('Ml32_one', len(Ml32_one))
 
-                # Assign to it the time axis
-                wfa.time_axis = time_axis
+            # Update the mass multipoles for all l.
+            all_mass_multipoles_1.append(amm1)
+            all_mass_multipoles_2.append(amm2)
+            all_mass_multipoles_3.append(amm3)
 
-            # message(wfa.time_axis - wf_psi4_time)
-            # continue
-            ###################################
-            # Uniform sampling
-            ###################################
-            # message('Wfa time axis', wfa.time_axis)
-
-            ###############################
-            # Load the phase data
-            ##############################
-
-            Yphase = wf_psi4_file[:, 4]
-            Yphase_interp_fun = interp1d(wf_psi4_time, Yphase, kind=interp_kind)
-
-            # Resample
-
-			Yphase_resam = Yphase_interp_fun(time_axis)
-
-			###########################
-			# Load the amplitude data
-			###########################
-			Yamp = wf_psi4_file[:, 3]
-			Yamp_interp_fun = interp1d(wf_psi4_time, Yamp, kind=interp_kind)
-
-			# Resample
-			Yamp_resam = Yamp_interp_fun(time_axis)
-			wfmode = Yamp_resam * np.exp(1j * Yphase_resam)
-
-			###################################
-			# Load the modes data
-			###################################
-
-			wfa.set_mode_data(ell, emm, wfmode)
-
-	wfa.actions += "->load_modes"
-
-	if crop is not False or centre is True:
-		# Trim or recenter
-		if crop is True or centre is True:
-			wfa.trim(trim_upto_time=0)
-			wfa.centered = True
-			wfa.actions += "->recenter"
-
-		elif isinstance(crop, float):
-			wfa.trim(trim_upto_time=crop)
-			wfa.actions += "->crop"
-
-		if save_as_ma is True:
-			# Save the modes array as waveforms hdf file
-			wfa.save_modes(out_file_name="{label}_resam.h5")
-			wfa.actions += "->save_as_wfh5"
-	return wfa
-
-
-def load_RIT_Strain_data_from_disk(
-	wfa=None,
-	data_dir="./",
-	file_name="*",
-	label="RIT_strain",
-	spin_weight=-2,
-	ell_max="auto",
-	resam_type="auto",
-	interp_kind="cubic",
-	save_as_ma=False,
-	modes_list=None,
-	crop=False,
-	centre=True,
-	r_ext_factor=1,
-	debug=False,
-):
-    """Load the RIT or strain waveforms from the RIT/ MAYA catalogue data,
-    from hdf5 files from disk.
+            # Update the spin multipoles for all l.
+            all_spin_multipoles_1.append(asm1)
+            all_spin_multipoles_2.append(asm2)
+            all_spin_multipoles_3.append(asm3)
 
-    Parameters
-    ----------
-    wfa : modes_array
-          An instance of the waveforms class. Creates a new one if not provided.
-    data_dir : string
-               A string containing the directory path where the mode files can be found.
-    label : string, optional
-            The label of the modes_array object.
-    ell_max : int, optional
-              The maximum mode number to load. If not specified,
-              then all available modes are loaded.
-    save_as_ma : bool, optional
-                 Save to disk again as a modes_array h5 file?
-    spin_weight : int, optional
-                  The spin weight of the object. Used for filtering modes.
-                  Defaults to -2.
-    resam_type : string, float, optional
-                 The type of resampling to do. Options are the `finest` and `coarsest`,
-                 and user input float.
-    interp_kind : string, optional
-                  The interpolation type to use. Default is cubic.
+            # Gather the mass and spin multipoles together.
+            all_mass_multipoles_one.append([amm1, amm2, amm3])
+            all_spin_multipoles_one.append([asm1, asm2, asm3])
 
-    Returns
-    -------
-    rit_modes_array : modes_array
-                      A modes_array instance containing the loaded modes.
+            # message(len(cctk_time))
 
-    Notes
-    -----
-    It seems like the time axis of individual modes are identical
-    to each other. Hence, one need not worry about choosing
-    the time domain. This may change in future.
-    """
-    message("Loading RIT strain data.", message_verbosity=1)
+            # Gather the l=2 mass multipoles.
+            multipoles_one.append(np.array([cctk_time, Ml12_one, Ml22_one, Ml32_one]))
 
-    from functools import partial
+            # Gather the masses.
+            masses_one.append([M1_one, M2_one, M3_one])
+            masses_one_all.append([M1_one_all, M2_one_all, M3_one_all])
 
-    # Initialize the interpolator
-    if isinstance(interp_kind, int):
-        message(
-            "Interpolating using InterpolatedUnivariateSpline",
-            message_verbosity=2,
-        )
-        interpolator = partial(interp, k=interp_kind)
-
-    elif isinstance(interp_kind, str):
-        from scipy.interpolate import interp1d
-
-        message("Interpolating using interp1d", message_verbosity=2)
-        interpolator = partial(interp1d, kind=interp_kind)
-
-    from waveformtools.waveforms import modes_array
-
-    # Max available mode l.
-    ell_max_act, keys_list = get_ell_max_from_file(
-        data_dir=data_dir, var_type="Strain", file_name=file_name
-    )
-
-    ####################################
-    # Set variables with priorities
-    # Note: rework this in dictionaries
-    ####################################
-
-    if ell_max == "auto":
-        ell_max = ell_max_act
-    if ell_max is None:
-        message("ell_max not provided.")
+            ###################################################################
+            # II . Load the distance data.
+            # Compute the distance using the coordinate positions in BHdiagnostics files.
+            ###################################################################
+            temp0 = np.genfromtxt(self.ROOTDIR + sim1[sim_index] + self.data_dir + "BH_diagnostics.ah1.gp")
+            temp1 = np.genfromtxt(self.ROOTDIR + sim1[sim_index] + self.data_dir + "BH_diagnostics.ah2.gp")
 
-        if wfa is not None:
-            wfa_ell_max = wfa.ell_max
-        else:
-            wfa_ell_max = None
+            t_coord_0 = temp0[:, 1]
+            x_coord_0_locs = temp0[:, 2]
+            y_coord_0_locs = temp0[:, 3]
 
-        if wfa_ell_max is None:
-            message("modes array not provided. Setting ell_max from file...")
-            ell_max = ell_max_act
-        else:
-            message("Setting ell_max from given modes_array")
-            ell_max = wfa.ell_max
+            message("Coord len", len(t_coord_0))
+            t_coord_1 = temp1[:, 1]
+            x_coord_1_locs = temp1[:, 2]
+            y_coord_1_locs = temp1[:, 3]
 
-    message("Chosen ell max", ell_max, "Available ell_max", ell_max_act)
+            temp0 = np.transpose(np.array([t_coord_0, x_coord_0_locs, y_coord_0_locs]))
+            temp1 = np.transpose(np.array([t_coord_1, x_coord_1_locs, y_coord_1_locs]))
 
-    if not wfa:
-        # Create a modes array
-        wfa = modes_array(label=label, ell_max=ell_max, modes_list=modes_list)
-    # wfa = modes_array(label=label, data_dir=data_dir, modes_list=modes_list)
-    if debug is True:
-        wf_nl = modes_array(
-            label=label + "_nl", ell_max=ell_max, modes_list=modes_list
-        )
-
-    if not data_dir:
-        data_dir = wfa.data_dir
-    else:
-        wfa.data_dir = data_dir
-
-    if not file_name:
-        file_name = wfa.file_name
-    else:
-        wfa.file_name = file_name
-
-    if not ell_max:
-        ell_max = wfa.ell_max
-    else:
-        wfa.ell_max = ell_max
-
-    # ell_max        = 12
-    if not modes_list:
-        if not wfa.modes_list:
-            message("Constructing the modes list")
-            modes_list = construct_mode_list(
-                ell_max=ell_max, spin_weight=wfa.spin_weight
-            )
-        else:
-            modes_list = wfa.modes_list
-    else:
-        wfa.modes_list = modes_list
-
-    # For interpolation
-    from scipy.interpolate import interp1d
-
-    # Alias of the modes_array
-    # label = 'q1a0_a'
-    # Enforce only l>abs(spin_Weight) modes.
-    # wf_modes_list = [item for item in wf_modes_list if item[0]>=abs(spin_weight)]
-    # tend = []
-    # tstart = []
-    ##########################################
-    # Read in the data
-    #########################################
-    # message(file_name)
-    # Get the time axis
-    # import h5py
-    data_file = h5py.File(f"{data_dir}/{file_name}")
-
-    try:
-        # For RIT data type
-        time_axis = data_file["NRTimes"][...]
-        # dt_auto = time_axis[1]-time_axis[0]
-        from scipy.stats import mode
-
-        dt_auto = mode(np.diff(time_axis))[0][0]
-
-    except Exception as excep:
-        dt_auto = None
-        message(
-            "NRTimes not present. Will compute dt auto from mode time axis",
-            excep,
-            message_verbosity=2,
-        )
-
-    message("Reading in modes...")
-    for ell, emm_list in modes_list:
-        for emm in emm_list:
-            this_amp_key = f"amp_l{ell}_m{emm}"
-            this_phase_key = f"phase_l{ell}_m{emm}"
-
-            message("Loading", ell, emm, message_verbosity=3)
-            # Construct file path
-
-            # Create modes_array on first run
-
-            ###############################
-            # Load the phase data
-            ##############################
-            Tphase = data_file[this_phase_key]["X"][...]
-
-            Yphase = data_file[this_phase_key]["Y"][...]
-
-            # message(wfa.modes_data)
-            if wfa.modes_data.all() == np.array(None):
-                message("Creating modes data")
-
-                if dt_auto is None:
-                    # For MAYA data type
-                    time_axis = Tphase
-                    # dt_auto = time_axis[1]-time_axis[0]
-                    from scipy.stats import mode
-
-                    dt_auto = mode(np.diff(time_axis))[0][0]
-
-                min_dt = round(min(np.diff(time_axis)), 2)
-                max_dt = round(max(np.diff(time_axis)), 2)
-                message(f"Default dt is {dt_auto}", message_verbosity=2)
-
-                if resam_type == "auto":
-                    # Choose finest available timestep
-                    # for upto 3 decimal digits.
-                    m_dt = dt_auto
-                    message(
-                        "Sampling at the default timestep",
-                        m_dt,
-                        message_verbosity=2,
-                    )
-
-                elif resam_type == "finest":
-                    m_dt = min_dt
-                    message(
-                        "Sampling at the finest available timestep",
-                        m_dt,
-                        message_verbosity=2,
-                    )
-
-                elif resam_type == "coarsest":
-                    m_dt = max_dt
-                    message(
-                        "Sampling at the coarsest available timestep",
-                        m_dt,
-                        message_verbosity=2,
-                    )
-
-                elif isinstance(resam_type, float):
-                    m_dt = resam_type
-                    message(
-                        "Resampling at user defined timestep",
-                        m_dt,
-                        message_verbosity=2,
-                    )
+            message("Dist shapes", temp0.shape, temp1.shape)
+            # check for data continuity.
+            # Load data.
+            data0 = temp0
+            data1 = temp1
 
-					# New (resampled) time axis
-					time_axis = np.arange(time_axis[0], time_axis[-1], m_dt)
+            # Clean the data.
+            temp0 = cleandata(data0)
+            temp1 = cleandata(data1)
 
-                else:
-                    raise NotImplementedError(
-                        f"Unknown resampling parameter {resam_type}"
-                    )
+            message("Dist shapes after cleaning", temp0.shape, temp1.shape)
 
-				# Length of data.
-				data_len = len(time_axis)
+            # Retrieve shape.
+            shape0 = temp0.shape
+            shape1 = temp1.shape
 
-				# Create a modes array object
-				wfa.create_modes_array(ell_max=ell_max, data_len=data_len)
+            # Retrieve timestepping.
+            delta_t = np.diff(temp0[:, 0])[0]
 
-				# Assign to it the time axis
-				wfa.time_axis = time_axis
-				# message(wfa.time_axis)
-			# message(wfa.time_axis - wf_psi4_time)
-			# continue
-			###################################
-			# Uniform sampling
-			###################################
-			# message('Wfa time axis', wfa.time_axis)
+            # message('Time step',delta_t)
 
-			Yphase_interp_fun = interpolator(Tphase, Yphase)
-			# Yphase_interp_fun = interpolator(Tphase, Yphase, k=3)
+            # Retrieve merger index.
+            mergerind = ind_merger_one[sim_index]
 
-			# Resample
+            # Update the merger time list.
+            merger_time_one.append(ind_merger_one[sim_index] * delta_t_one[sim_index])
 
-			Yphase_resam = Yphase_interp_fun(time_axis)
+            # Find the shorter data. BHdiag1,2 or multipole data.
+            act_len = min(shape0[0], shape1[0], ml_data_length[sim_index])
 
-			###########################
-			# Load the amplitude data
-			###########################
-			Tamp = data_file[this_amp_key]["X"][...]
+            # If BHdiag 1 and 2 are equal in length and equal to multipole
+            # length:
+            if shape0[0] == shape1[0] and shape0[0] == ml_data_length[sim_index]:
+                message("BH_data length is consistent with multipole data length")
 
-			Yamp = data_file[this_amp_key]["Y"][...]
+            # If the shortest data length is different from multipole length.
+            if act_len == shape0[0] or act_len == shape1[0]:
+                message("BH_diagnostics data is shorter")
 
-			Yamp_interp_fun = interpolator(Tamp, Yamp)
-			# Yamp_interp_fun = interpolator(Tamp, Yamp, k=3)
+            # If multipole data is shorter.
+            else:
+                message("Multipole data is shorter")
 
-			# wf_c = Yamp*np.exp(1j*Yphase)
+            # Update the actual length array.
+            act_shape_one.append(act_len)
 
-			# Resample
+            # message('Data length',act_len)
 
-			Yamp_resam = Yamp_interp_fun(time_axis)
+            # act_shape_one.append()#
+            # act_shape_one.append(min(shape1[0],shape2[0]))
+            # message(temp0.shape,temp1.shape)
+
+            # Try to load BHdiag3 file if present.
+            try:
+                # Try to load the BH_diagnostics file for BH3.
+                temp2 = np.genfromtxt(self.ROOTDIR + sim1[sim_index] + self.data_dir + "BH_diagnostics.ah3.gp")[
+                    :, np.r_[1, 2, 3]
+                ]
+
+                # If merger index is not found from masses set using BH_diag3.
+
+                # If the merger_ind from masses is greater than the BHdiag3
+                # data length.
+
+                if mergerind * delta_t >= int(temp2[0, 0]):
+                    merger_time_one[sim_index] = temp2[0, 0]
+                    mergerind = int(temp2[0, 0] / delta_t)
+                    ind_merger_one[sim_index] = mergerind
+                    message("Merger time acquired from BHdiag3", mergerind * delta_t)
+                    message("Merger index has been updated with info from BHdiag3")
+            except BaseException:
+                message("Merger time acquired from masses", mergerind * delta_t)
+
+            message("Merger index", mergerind)
+
+            # FInd shape of data.
+            shape0 = temp0.shape
+            shape1 = temp1.shape
+
+            # if shape0[0] < shape0[1]:
+            # 	 temp1 = np.transpose(temp1)
+
+            # if shape1[0] < shape1[1]:
+            # 	 temp2 = np.transpose(temp2)
+
+            # Assign the centroid locations to variables.
+
+            # t_coord_0 = t_coord_0  # temp0[:, 0]
+            x_coord_0 = x_coord_0_locs  # temp0[:, 1]
+            y_coord_0 = y_coord_0_locs  # temp0[:, 2]
+
+            # t_coord_1 = t_coord_1  # temp1[:, 0]
+            x_coord_1 = x_coord_1_locs  # temp1[:, 1]
+            y_coord_1 = y_coord_1_locs  # temp1[:, 2]
+
+            # t_coord_0		 =	 temp0[:, 0]
+            # x_coord_0		 =	 temp0[:, 1]
+            # y_coord_0		 =	 temp0[:, 2]
+            #
+            # t_coord_1		 =	 temp1[:, 0]
+            # x1		 =	 temp1[:, 1]
+            # y1		 =	 temp1[:, 2]
+
+            # if int((x_coord_0-x_coord_0_locs)[0])!=0:
+            # 	 message('ERRORRRRRRR!')
+            # 	 sys.exit(0)
+            # Compute lengths
+
+            len_0 = len(t_coord_0)
+            len_1 = len(t_coord_1)
+
+            # Find minimum
+            lmin = min(len_0, len_1)
+            timeaxis_one.append(t_coord_0)
+
+            # Crop data
+
+            if len_0 < len_1:
+                t_coord_1 = t_coord_1[:lmin]
+                x_coord_1 = x_coord_1[:lmin]
+                y_coord_1 = y_coord_1[:lmin]
+
+            elif len_1 < len_0:
+                t_coord_0 = t_coord_0[:lmin]
+                x_coord_0 = x_coord_0[:lmin]
+                y_coord_0 = y_coord_0[:lmin]
+
+            # Compute differences
+
+            delta_x = x_coord_0 - x_coord_1
+            delta_y = y_coord_0 - y_coord_1
+
+            # if sim_index==3:
+            # d.append(np.sqrt((temp0[:3014,1]-temp1[:ind_merger[sim_index],1])**2
+            # + (temp0[:3014,2]-temp1[:ind_merger[sim_index],2])**2))
+
+            # Compute the Eucledian distance.
+            d_sim = np.sqrt(np.power(delta_x, 2) + np.power(delta_y, 2))
+            d_sim = np.array(d_sim)
+            d0_sim = d_sim[0]
+            message("Initial true distance", d0_sim)
+            d0_one.append(d0_sim)
+            d_sim = d_sim / d0_sim
+            # d_one.append(np.sqrt((temp0[:act_shape_one[sim_index],1]-temp1[:act_shape_one[sim_index],1])**2
+            # + (temp0[:act_shape_one[sim_index],2]-temp1[:act_shape_one[sim_index],2])**2))
+            d_one.append([t_coord_0, d_sim])
+            message(
+                "ml_timeaxis_length: %d, Multipole data length: %d, BHdiag length: %d, Distance length: %d"
+                % (len(timeaxis_one[sim_index]), ml_data_length[sim_index], shape1[0], len(d_one[sim_index]))
+            )
+            dist_data_length.append(len(d_sim))
 
-			wfmode = Yamp_resam * np.exp(1j * Yphase_resam)
+        # multipoles = np.array(multipoles)
+        # Convert the acquired data lists into numpy arrays.
+        masses_one = np.array(masses_one)
+        M1_one = np.array(M1_one)
+        M2_one = np.array(M2_one)
+        M3_one = np.array(M3_one)
+
+        # message('Multipoles shape',multipoles.shape)
+
+        # message('Masses shape:',masses_one.shape)
+
+        d_one = np.array(d_one)
+        # d_one.shape
+        # d_one.append(np.sqrt((temp0[:act_shape_one[sim_index],1]-temp1[:act_shape_one[sim_index],1])**2
+        # + (temp0[:act_shape_one[sim_index],2]-temp1[:act_shape_one[sim_index],2])**2))
+        # d_one=np.array(d_one)
+
+        # d_one.shape
+
+        # Plot the distance
+        # message('multipoles length',len(multipoles_one))
+
+        # Assign data to sim variables.
+        for sim_index in range(0, len(self.aliases)):
+            self.multipoles.update({self.aliases[sim_index]: multipoles_one[sim_index]})
+            self.mass_multipoles.update({self.aliases[sim_index]: all_mass_multipoles_one[sim_index]})
+            self.spin_multipoles.update({self.aliases[sim_index]: all_spin_multipoles_one[sim_index]})
+            self.timeaxis.update({self.aliases[sim_index]: timeaxis_one[sim_index]})
+            self.mass1.update({self.aliases[sim_index]: M1_one[sim_index]})
+            self.mass2.update({self.aliases[sim_index]: M2_one[sim_index]})
+            self.mass3.update({self.aliases[sim_index]: M3_one[sim_index]})
+            self.delta_t.update({self.aliases[sim_index]: delta_t_one[sim_index]})
+            self.distance.update({self.aliases[sim_index]: d_one[sim_index]})
+            self.merger_ind.update({self.aliases[sim_index]: ind_merger_one[sim_index]})
+            self.actmerger_time.update({self.aliases[sim_index]: merger_time_one[sim_index]})
+            self.dinit.update({self.aliases[sim_index]: d0_one[sim_index]})
+            self.data_length.update({self.aliases[sim_index]: ml_data_length[sim_index]})
+            self.comm_data_length.update({self.aliases[sim_index]: act_shape_one[sim_index]})
+            self.dist_data_length.update({self.aliases[sim_index]: dist_data_length[sim_index]})
+        # message(self.multipoles)
+
+        # Resize the multipoles data if merger index was updated from BHdiag3.
+        self._resize_multipoles()
+        # Reverse the BH1 and BH2 data if BH mass2>mass1.
+        self._ifreversal()
+
+        import matplotlib.pyplot as plt
+
+        # Plot the distances.
+        for alias in self.aliases:
+            x_coord = self.distance[alias][0]
+            y_coord = self.distance[alias][1]
+            length = min(len(x_coord), len(y_coord))
+            x_coord = x_coord[:length]
+            y_coord = y_coord[:length]
+            # message(x,y)
+
+            plt.plot(x_coord, y_coord)
+            plt.title("Distance vs t/M " + alias)
+            plt.grid(which="both", axis="both")
+            plt.xlabel("t")
+            plt.ylabel(r"$d/d_{init}$")
+            plt.show()
+
+    def _resize_multipoles(self):
+        """Private method to resize the (l=2) multipole data. Useful when merger index was updated from BHdiag3."""
+        for alias in self.aliases:
+            # Loop over simulations.
+            # message(alias)
+            # self.timeaxis[alias] = [item[:self.dist_data_length[alias]] for item in self.timeaxis[alias]]
+            # Resize the lengths of the data.
+            self.multipoles[alias] = [item[: self.dist_data_length[alias]] for item in self.multipoles[alias]]
+            # self.data_length.update({alias : len(self.multipoles[alias][0])})
+            # self.mass_multipoles[alias] = [item[:self.dist_data_length[alias] for item in self.mass_multipoles[alias]]]
+            # self.spin_multipoles[alias] = [item[:self.dist_data_length[alias]
+            # for item in self.spin_multipoles[alias]]]
+
+    def _ifreversal(self):
+        """Private method to reverse the (l=2) multipole data if mass2>mass1.
+
+        Notes
+        -----
+        Updates:
+
+                sim.multipoles : Resized (l=2) multipole moment data.
+        """
+
+        # Flag to identify if reversal is required.
+        flag = 0
+
+        for alias in self.aliases:
+            # Loop over simulations.
+            message("Check for puncture reversal, %s" % alias)
+            if alias != "q1a0_a" and alias != "q1a0_b":
+                # Condition for reversal decision.
+                if self.mass1[alias] < self.mass2[alias]:
+                    # Toggle the flag.
+                    flag = 1
+                    message("**************************************************")
+                    message("BH 1 and 2 reversal found!!! \n Reversing data...")
+                    message("**************************************************")
+                    message("original mass1:%f, mass2: %f" % (self.mass1[alias], self.mass2[alias]))
+                    # Reverse the data.
+                    self.mass1[alias], self.mass2[alias] = self.mass2[alias], self.mass1[alias]
+                    # Unpack the multipoles data.
+                    time, multipole1, multipole2, multipole3 = self.multipoles[alias]
+                    # Reverse the multipole data.
+                    multipole1, multipole2 = multipole2, multipole1
+                    # Repack the data.
+                    self.multipoles[alias] = np.array([time, multipole1, multipole2, multipole3])
+            if not flag:
+                message("Data O.K.")
+            return 1.0
+
+    def load_strain(self, start_index=0):
+        """Method to load the shear data of simulations."""
+
+        for sim_index in range(0, len(self.aliases)):
+            # Loop over simulations.
+            alias = self.aliases[sim_index]
+            # Set the starting index for data.
+            start_index = 0  # start_index = 0#int(190/deltat[j])
+            # Load the strain data.
+            sim_strain_data = np.genfromtxt(
+                self.WAVDIR
+                + self.aliases[sim_index]
+                + "/"
+                + self.strain_dir
+                + "/strain_"
+                + str(alias)
+                + "_wavextcpm.dat"
+            )
 
-            # if not (Tphase==Tamp).all():
-            #    raise ValueError('The time axis of the amps and phase are different!')
+            # Load the timeaxis, plus and cross polarized data.
+            htdat = sim_strain_data[start_index:, 0]
+            hpdat = sim_strain_data[start_index:, 1]
+            hxdat = sim_strain_data[start_index:, 2]
 
-			# wfmode = interp_resam_wfs(wf_c, Tphase, time_axis, k=4)
+            message("The strain file is")
+            message(
+                self.WAVDIR
+                + self.aliases[sim_index]
+                + "/"
+                + self.strain_dir
+                + "/strain_"
+                + str(alias)
+                + "_wavextcpm.dat"
+            )
 
-			###################################
-			# Load the modes data
-			###################################
+            # Align the peak of the strain with the formation of the common
+            # horizon (merger index).
 
-			wfa.set_mode_data(ell, emm, r_ext_factor * wfmode)
+            Lpeak_loc = np.argmax(np.diff(hpdat) ** 2 + np.diff(hxdat) ** 2)
 
-	data_file.close()
+            # Load the common horizon location.
+            commhor_loc = self.merger_ind[alias]
+            # Compute the shift betweeen the Luminosity peak index and common
+            # horizon formation location.
+            shift = Lpeak_loc - commhor_loc
+
+            # Update the strain_indexshifts.
+            self.strain_indexshifts.update({alias: shift})
+
+            # Load the time stepping.
+            # delta_t = self.delta_t[alias]
+
+            # Shift the timeaxis and clip the beginning of data.
+            htdat = htdat[start_index:-shift]
+            hpdat = hpdat[start_index + shift :]
+            hxdat = hxdat[start_index + shift :]
+
+            # Update the sim.strain
+            self.strain.update({alias: [htdat, hpdat, hxdat]})
+
+            if config.print_verbosity > 1:
+                import matplotlib.pyplot as plt
+
+                # Plot the strains.
+                plt.plot(htdat, hpdat, label="data " + alias)
+                plt.ylabel("Strain")
+                plt.xlabel("Time (s)")
+                plt.grid(which="both", axis="both")
+                # plt.xlim(-600,400)
+                plt.legend()
+                plt.show()
+
+        return 1
+
+    def calc_amp_phase(self):
+        """Extract the amplitude and the phase from strain data."""
+        from waveformtools.waveformtools import xtract_camp, xtract_cphase
+
+        for alias in self.aliases:
+            # Loop over simulations.
+
+            # Load the plus and cross polarized strain data.
+            hpdat = self.strain[alias][1]
+            hxdat = self.strain[alias][2]
+            # Load the time stepping.
+            delta_t = self.delta_t[alias]
+            # Extract and update the amplitude and phases.
+            self.strain_phase.update({alias: (xtract_cphase(hpdat, hxdat, delta_t=delta_t, to_plot="yes"))})
+            self.strain_amplitude.update({alias: xtract_camp(hpdat, hxdat)})
+            self.strain_frequency.update({alias: np.diff(self.strain_phase[alias]) / delta_t})
+        return 1
+
+    def ret_horizon_radii(self):
+        """Retrieve the radius of the common horizon at the time of formation."""
+
+        # Dictionary to hold the areal radii of the horizons.
+        self.areal_radii = {}
+        for alias in self.aliases:
+            # Loop over simulations.
+
+            # Load the BHdiagnostics file to load the radius.
+            ar_rad0 = np.genfromtxt(self.ROOTDIR + alias + "/" + self.data_dir + "BH_diagnostics.ah1.gp")[:, 27]
+            ar_rad1 = np.genfromtxt(self.ROOTDIR + alias + "/" + self.data_dir + "BH_diagnostics.ah2.gp")[:, 27]
+            ar_rad2 = 1.75
+            try:
+                ar_rad2 = np.genfromtxt(self.ROOTDIR + alias + "/" + self.data_dir + "BH_diagnostics.ah3.gp")[:, 27]
+            except BaseException:
+                message("No BHdiagnostics 3 file found for %s" % alias)
+
+            # Load the data for this simulation in to a dictionary.
+            self.areal_radii.update({alias: [ar_rad0, ar_rad1, ar_rad2]})
+
+        return 1
+
+    def get_BH_locations(self, alias=None):
+        """Get the co-ordinate locations of the BHs.
+
+        Parameters
+        ----------
+
+        alias  :    str, optional.
+                                The simulation label. If not specified, then
+                                all available simulationswill be processed.
+
+        Returns
+        -------
 
-	#####################
-	# Finishing touches
-	#####################
-	wfa.actions += "->load_modes"
 
-	# Trim or recenter
-	if centre is True:
-		wfa.trim(trim_upto_time=0)
-		wfa.actions += "->center"
+        """
 
-	if isinstance(crop, float):
-		wfa.trim(trim_upto_time=crop)
-		wfa.actions += "->crop"
+        # A dictionary to store BH location data
+        self.BH_locations = {}
 
-	if save_as_ma is True:
-		# Save the modes array as waveforms hdf file
-		wfa.save_modes(out_file_name=f"{label}_resam.h5")
-		wfa.actions += "->save_as_wfh5"
+        if not alias:
+            list_of_aliases = self.aliases
 
-	if debug is True:
-		return wfa, wf_nl
-	else:
-		return wfa
+        else:
+            list_of_aliases = [alias]
 
+        for alias in list_of_aliases:
+            # Load the data
+            # alias = 'q1a0_a'
+            # sim_index = 0
+
+            # Masses of the horizons
+            m1 = self.mass1[alias]
+            m2 = self.mass2[alias]
+            # M = m1 + m2
+
+            flag = 1
+            bh1 = np.genfromtxt(self._get_file_path_from_str(string="*.ah1.gp", alias=alias))
+            bh2 = np.genfromtxt(self._get_file_path_from_str(string="*.ah2.gp", alias=alias))
+            try:
+                bh3 = np.genfromtxt(self._get_file_path_from_str(string="*.ah3.gp", alias=alias))
+            except Exception as excep:
+                message("BH3 file not found!", excep)
+                flag = -1
+
+            # Read co-ordinates.
+
+            bhd1_time = bh1[:, 1]
+            bhd1_x = bh1[:, 2]
+            bhd1_y = bh1[:, 3]
+            bhd1_z = bh1[:, 4]
+
+            bhd2_time = bh2[:, 1]
+            bhd2_x = bh2[:, 2]
+            bhd2_y = bh2[:, 3]
+            bhd2_z = bh2[:, 4]
+
+            if flag != -1:
+                bhd3_time = bh3[:, 1]
+                bhd3_x = bh3[:, 2]
+                bhd3_y = bh3[:, 3]
+                bhd3_z = bh3[:, 4]
+            else:
+                bhd3_time = None
+                bhd3_x = None
+                bhd3_y = None
+                bhd3_z = None
 
-#################################################################
-# Generic data type
-#################################################################
+            bh1_loc = [bhd1_time, bhd1_x, bhd1_y, bhd1_z]
+            bh2_loc = [bhd2_time, bhd2_x, bhd2_y, bhd2_z]
+            bh3_loc = [bhd3_time, bhd3_x, bhd3_y, bhd3_z]
 
+            self.BH_locations.update({alias: [bh1_loc, bh2_loc, bh3_loc]})
 
-def load_gen_data_from_disk(
-	wfa=None,
-	label="generic waveform",
-	data_dir="./",
-	file_name="*.h5",
-	r_ext=None,
-	ell_max=8,
-	pre_key=None,
-	modes_list=None,
-	crop=False,
-	centre=True,
-	key_ex=None,
-	r_ext_factor=1,
-	*args,
-	**kwargs,
-):
-    """Load the RIT strain waveforms from the RIT catalogue,
-    from hdf5 files from disk.
+    def get_CoM_locations(self, alias=None):
+        """Get the CoM location of the given simulation.
 
-    Parameters
-    ----------
-    data_dir : string
-               A string containing the directory path
-               where the mode files can be found.
-    label : string, optional
-            The label of the modes_array object.
-    ell_max : int, optional
-              The maximum mode number to load. If not specified,
-              then all available modes are loaded.
-    save_as_ma : bool, optional
-                 Save to disk again as a modes_array h5 file?
-    spin_weight : int, optional
-                  The spin weight of the object. Used for filtering modes.
-                  Defaults to -2.
-    resam_type : string, float, optional
-                 The type of resampling to do. Options are the `finest` and `coarsest`,
-                 and user input float.
-    interp_kind : string, optional
-                  The interpolation type to use. Default is cubic.
+        Parameters
+        ----------
 
-    Returns
-    -------
+        alias  :    str, optional.
+                                The simulation label. If not specified, then
+                                all available simulationswill be processed.
 
-    rit_modes_array : modes_array
-                      A modes_array instance containing the loaded modes.
+        Returns
+        -------
 
-    Notes
-    -----
-    It seems like the time axis of individual modes are identical to each other.
-    Hence, one need not worry about choosing the time domain. This may change
-    in future.
+        self.CoM_locations :    dict
+                                                        A dictionary of lists containing
+                                                        CoM locations of the simulations.
 
-    """
-    message("Loading generic data.", message_verbosity=1)
-    from waveformtools.waveforms import modes_array
+        Notes
+        -----
 
-    # Max available mode l.
-    if not wfa:
-        # Create a modes array
-        wfa = modes_array(
-            label=label,
-            data_dir=data_dir,
-            modes_list=modes_list,
-            ell_max=ell_max,
-        )
-
-    # if not data_dir:
-    #   data_dir = wfa.data_dir
-    # else:
-    #   wfa.data_dir = data_dir
-
-    # if not file_name:
-    #   file_name = wfa.file_name
-    # else:
-    #   wfa.file_name = file_name
-
-    # if not ell_max:
-    #   ell_max = wfa.ell_max
-    # else:
-    #   wfa.ell_max = ell_max
-
-    # if not label:
-    #   label = wfa.label
-    # ell_max        = 12
-    # Max available mode l.
-
-    full_path = f"{data_dir}/{file_name}"
-    message(f"Loading data from {full_path}")
-    # Enforce only l>2 modes.
-    # wf_modes_list = [item for item in wf_modes_list if item[0]>=abs(spin_weight)]
-
-    # Open the modes file.
-    # import h5py, json
-    full_path = wfa.data_dir + "/" + wfa.file_name
-
-    # message(wfa.file_name)
-    with h5py.File(full_path, "r") as wfile:
-        #################################
-        # Get metadata
-        ###############################
+        This fetches the location of the BHs from data files.
+        """
 
-        # Load metadata if present.
-        try:
-            # if 1:
-            metadata_bytes = bytes(np.void(wfile["metadata"])).decode()
-            metadata = json.loads(metadata_bytes)
-            # Import the metadata.
-            for key, val in metadata.items():
-                if val is not None:
-                    wfa.__dict__.update({key: val})
-            message("Metadata loaded", message_verbosity=2)
-            message(
-                "Waveform meta data:", wfa.get_metadata(), message_verbosity=1
-            )
+        # Storage for CoM locations
+        self.CoM_locations = {}
 
-        except Exception as ex:
-            # If no metadata found, pass empty dict for updation.
-            message("No metadata found!", ex)
-            metadata = {}
-            pass
-        # message(wfa.file_name)
-        # data = np.array(wfile['l0_m0_r500.00'])
-        # message(data)
-        # Get the list of keys.
-        modes_keys_list = list(wfile.keys())
-        # message('Keys ', modes_keys_list)
-        # message(wfa.get_metadata())
-        # Check and filter for particular key string pattern
-
-        if key_ex is not None:
-            # Filter the keys according to key_ex if specified.
-            message("Filtering as per", key_ex)
-            wfa.key_ex = key_ex
-            modes_keys_list = [
-                item for item in modes_keys_list if key_ex in item
-            ]
-            # message(modes_keys_list)
+        # Aliases to run over.
+        if not alias:
+            list_of_aliases = self.aliases
 
         else:
-            message("key_ex is not specified. Proceeding without filtering..")
+            list_of_aliases = [alias]
 
-        modes_keys_list = sorted(modes_keys_list)
+        for alias in list_of_aliases:
+            try:
+                BH_locs_sim = self.BH_locations[alias]
+            except Exception as excep:
+                message(excep)
+                self.get_BH_locations(alias)
+                BH_locs_sim = self.BH_locations[alias]
 
-        # message('Modes keys', modes_keys_list)
-        wfa.mode_keys_list = modes_keys_list
+            # Unpack the location data.
+            BH1_loc, BH2_loc, _ = BH_locs_sim
 
-        # Construct the list of modes if it doesnt exist.
+            bh1_time, bh1_x, bh1_y, bh1_z = BH1_loc
+            bh2_time, bh2_x, bh2_y, bh2_z = BH2_loc
+            # bh3_time, bh3_x, bh3_y, bh3_z = BH3_loc
 
-        ##########################
-        # Construct modes list
-        ##########################
-        if r_ext:
-            wfa.r_ext = r_ext
-        elif wfa.r_ext is not None:
-            r_ext = wfa.r_ext
-        else:
-            message("Unable to parse extraction radius!")
-            sys.exit(0)
-        if not modes_list:
-            # Check if modes list is given for which mode to load.
-            # If the list of modes is not given then construct the list of modes.
-
-            if not ell_max:
-                # If ell max is also not specified,
-                # construct the list of modes using
-                # the list of modes h5 file keys.
-                modes_list = _get_modes_list_from_keys(modes_keys_list, r_ext)
-                # message(modes_list)
-                # Get the ell max
-                ell_max = max([item[0] for item in modes_list])
+            # The masses.
+            mass1 = self.mass1[alias]
+            mass2 = self.mass2[alias]
+            total_mass = mass1 + mass2
 
-                # metadata.update({ell_max : ell_max })
-                wfa.ell_max = ell_max
+            # End time
+            max_len = min(self.merger_ind[alias], len(bh1_time), len(bh2_time))
 
-            else:
-                # self.ell_max = ell_max
-                # If ell max is given, construct the
-                # list of modes directly.
-                modes_list = construct_mode_list(ell_max)
+            # CoM location
+            T_com = bh1_time[:max_len]
+            X_com = (mass1 * bh1_x[:max_len] + mass2 * bh2_x[:max_len]) / (total_mass)
+            Y_com = (mass1 * bh1_y[:max_len] + mass2 * bh2_y[:max_len]) / (total_mass)
+            Z_com = (mass1 * bh1_z[:max_len] + mass2 * bh2_z[:max_len]) / (total_mass)
 
-                # set the modes list attr.
-                wfa.modes_list = modes_list
+            self.CoM_locations.update({alias: [T_com, X_com, Y_com, Z_com]})
 
-        else:
-            # self.modes_list = modes_list
-            # If modes list is given, get ell_max from it.
-            if not ell_max:
-                # Get the ell max
-                ell_max = max([item[0] for item in modes_list])
-
-        # Set the ell_max attribute if not already.
-        if not wfa.ell_max:
-            wfa.ell_max = ell_max
-
-        #################################################
-        # Load modes
-        #################################################
-        # Modes array created flag
-        cflag = 0
-        # Load the modes listed in mode_numbers list
-        for item in modes_list:
-            # For every ell mode list in modes_list
+    def get_CoM_mean_motion(self, alias=None):
+        """Get the mean motion of the CoM.
 
-            ell_value, emm_list = item
+        Parameters
+        ----------
 
-            for emm_index, emm_value in enumerate(emm_list):
-                # For every (ell, emm) mode.
+        alias  :    str, optional.
+                                The simulation label. If not specified, then
+                                all available simulationswill be processed.
 
-                # Find the key corresponding to the mode
-                try:
-                    key = str(
-                        [
-                            item
-                            for item in modes_keys_list
-                            if re.search(
-                                f"l{ell_value}_m{emm_value}_r{r_ext}", item
-                            )
-                        ][0]
-                    )
-                    # message('The loaded key is ', key, type(key))
-                    # message('The loaded key is ', key, type(key))
-                    # if key=='l0_m0_r500.00':
-                    # message('Its alright')
-                except Exception as ex:
-                    message(
-                        f"Waveform dataset for l{ell_value}, m{emm_value} not found",
-                        ex,
-                    )
-                    sys.exit(0)
-
-                # Get the data
-                data = np.array(wfile[key])
-
-                # set the time and data axis
-                time_axis, data_re = cleandata([data[:, 0], data[:, 1]])
-                time_axis, data_im = cleandata([data[:, 0], data[:, 2]])
-
-                # create flag
-                if not cflag:
-                    if wfa.modes_data.all() == np.array(None):
-                        if crop:
-                            # Crop the beginning portion.
-                            # delta_t = time_axis[1] - time_axis[0]
-                            # shift = int(wfa.r_ext / delta_t)
-                            raise NotImplementedError(
-                                "Not implemented! Please contact the developers!"
-                            )
-
-                        else:
-                            shift = 0
-                        data_len = len(time_axis) - shift
-                        wfa.data_len = data_len
-                        # Delete the attribute
-                        # del self.modes_data
-                        # Create an array for the waveform mode object
-                        wfa.create_modes_array(wfa.ell_max, data_len)
-                        # self.modes_data = np.zeros([ell_max+1, 2*(ell_max+1) +1, data_len], dtype=np.complex128)
-                        # self.modes_data = np.zeros([ell_max+1, 2*(ell_max+1) +1, data_len], dtype=np.complex128)
-
-                        cflag = 1
-
-                        # set the time axis.
-                        # wfa.time_axis = time_axis[shift:]
-                        wfa._time_axis = time_axis
-
-                # wfa.set_mode_data(ell_value, emm_value, r_ext_factor*(data_re[shift:] + 1j * data_im[shift:]))
-                wfa.set_mode_data(
-                    ell_value,
-                    emm_value,
-                    r_ext_factor * (data_re + 1j * data_im),
-                )
+        Returns
+        -------
 
-        ##############################
-        # Recenter axis
-        ##############################
-        # Trim or recenter
-        if centre:
-            crop_time = 0
-            if crop:
-                crop_time = wfa.r_ext
-
-            wfa.trim(trim_upto_time=crop_time)
-
-        # maxloc = np.argmax(np.absolute(self.mode(2, 2)))
-        # maxtime = time_axis[shift + maxloc]
-
-        # if wfa.maxtime is None:
-        #    wfa.maxtime = maxtime
-        # message("Max time is", maxtime)
-
-        # if centre:
-        #    wfa.time_axis = time_axis[shift:] - maxtime
-        # message(wfa.file_name)
-        return wfa
-
-
-########################################################################################################################
-# SpEC
-########################################################################################################################
-
-
-def load_SpEC_data_from_disk(
-	wfa=None,
-	label="SXS Strain",
-	data_dir="./",
-	file_name="rhOverM_Extrapolated_N5_CoM_Mem.h5",
-	extrap_order=4,
-	r_ext=None,
-	ell_max=None,
-	centre=True,
-	modes_list=None,
-	save_as_ma="False",
-	resam_type="auto",
-	interp_kind="cubic",
-	compression_opts=0,
-	r_ext_factor=1,
-	debug=False,
-):
-    """Load the SpEC waveform to modes_array,from hdf5 files from disk.
+        alpha :     dict
+                                A dictionary containing the
+                                mean CoM displacement array.
 
-    Parameters
-    ----------
-    wfa : modes_array, optional
-          The modes array to which to store the loaded waveform to.
-          A new modes array will be returned if not provided.
-    data_dir : string
-               A string containing the directory path
-               where the mode files can be found.
-    file_name : string
-                The name of the file containing the waveform data.
-    label : string, optional
-            The label of the modes_array object.
-    ell_max : int, optional
-              The maximum mode number to load. If not specified,
-              then all available modes are loaded.
-    save_as_ma : bool, optional
-                 Save to disk again as a modes_array h5 file?
-    resam_type : string, float, optional
-                 The type of resampling to do. Options are
-                 the `fines`t and `coarsest`, and user input float.
-    interp_kind : string, optional
-                  The interpolation type to use. Default is cubic.
+        beta :     dict
+                           A dictionary containing the
+                           mean CoM velocity array.
 
-    Returns
-    -------
-    modes_array : modes_array
-                  A modes_array instance containing the loaded modes.
+        """
+        CoM_motion_params = {}
+        # Aliases to run over.
 
-    """
-    message("Loading SpEC data.", message_verbosity=1)
+        from waveformtools.CoM import X_com_moments, compute_com_alpha, compute_com_beta
 
-    from waveformtools.waveforms import modes_array
+        if not alias:
+            list_of_aliases = self.aliases
 
-    # Load SXS waveforms to modes_array.
-    # Spectra infinty
+        else:
+            list_of_aliases = [alias]
 
-    full_path = f"{data_dir}/{file_name}"
+        for alias in list_of_aliases:
+            try:
+                taxis, X_com, Y_com, Z_com = self.CoM_locations[alias]
+            except Exception as excep:
+                message(excep)
+                self.get_CoM_locations(alias)
+                taxis, X_com, Y_com, Z_com = self.CoM_locations[alias]
 
-    # Key pattern
-    gkey = f"Extrapolated_N{extrap_order}.dir"
+            all_coords = [X_com, Y_com, Z_com]
 
-    wf_f0 = h5py.File(full_path)
-    wf_file = wf_f0[gkey]
-    all_keys = list(wf_file.keys())
+            zeroth_moments = X_com_moments(taxis, all_coords, 0)
+            first_moments = X_com_moments(taxis, all_coords, 1)
 
-    # Max available mode l.
-    ell_max_act = get_ell_max_from_keys(all_keys)
-    # message(ell_max_act)
+            Xcom_0 = np.array([zeroth_moments[label][0] for label in zeroth_moments.keys()])
+            Xcom_1 = np.array([first_moments[label][0] for label in zeroth_moments.keys()])
 
-    ####################################
-    # Set variables with priorities
-    # Note: rework this in dictionaries
-    ####################################
+            ti = taxis[0]
+            tf = taxis[-1]
 
-    if ell_max == "auto":
-        ell_max = ell_max_act
-    if ell_max is None:
-        message("ell_max not provided.")
+            alpha = compute_com_alpha(ti, tf, Xcom_0, Xcom_1)
+            beta = compute_com_beta(ti, tf, Xcom_0, Xcom_1)
 
-        if wfa is not None:
-            wfa_ell_max = wfa.ell_max
-        else:
-            wfa_ell_max = None
+            CoM_motion_params.update({alias: [alpha, beta]})
+        return CoM_motion_params
 
-        if wfa_ell_max is None:
-            message("modes array not provided. Setting ell_max from file...")
-            ell_max = ell_max_act
-        else:
-            message("Setting ell_max from given modes_array")
-            ell_max = wfa.ell_max
+    def _get_file_path_from_str(self, alias, string=None):
+        """Get the path of a file that contains
+        the given string in its name.
 
-    message("Chosen ell max", ell_max, "Available ell_max", ell_max_act)
+        Parameters
+        ----------
 
-    if not wfa:
-        # Create a modes array
-        wfa = modes_array(label=label, ell_max=ell_max, modes_list=modes_list)
-    # wfa = modes_array(label=label, data_dir=data_dir, modes_list=modes_list)
-    if debug is True:
-        wf_nl = modes_array(
-            label=label + "_nl", ell_max=ell_max, modes_list=modes_list
-        )
-
-    wfa.extrap_order = extrap_order
-    message(f"Using extrap order {extrap_order}")
-
-    if not data_dir:
-        data_dir = wfa.data_dir
-    else:
-        wfa.data_dir = data_dir
-
-    if not file_name:
-        file_name = wfa.file_name
-    else:
-        wfa.file_name = file_name
-
-    if not ell_max:
-        ell_max = wfa.ell_max
-    else:
-        wfa.ell_max = ell_max
-
-    # ell_max        = 12
-    if not modes_list:
-        if not wfa.modes_list:
-            message("Constructing the modes list")
-            # sys.exit(0)
-            modes_list = construct_mode_list(
-                ell_max=ell_max, spin_weight=wfa.spin_weight
-            )
-        else:
-            modes_list = wfa.modes_list
-    else:
-        wfa.modes_list = modes_list
-
-    # Filter
-    modes_list = [item for item in modes_list if item[0] >= 2]
-    ############################################################
-
-    # create flag
-    # flag = None
-
-    # get auto dt
-    from scipy.stats import mode
-
-    # Load modes
-    for ell, emm_list in modes_list:
-        for emm in emm_list:
-            # message(ell, emm)
-
-            this_key = f"Y_l{ell}_m{emm}.dat"
-
-            # Input waveform from disk
-            wf_data = wf_file[this_key]
-            wf_time = wf_data[:, 0]
-            wf_data_re = wf_data[:, 1]
-            wf_data_im = wf_data[:, 2]
-            wf_data_c = wf_data_re + 1j * wf_data_im
-
-            # wf_amp, wf_phase = xtract_camp_phase(wf_data_re, wf_data_im)
-
-            # message(type(wfa.modes_data))
-            if wfa.modes_data.all() == np.array(None):
-                time_axis = wf_time
-                message("Creating modes data")
-
-                # min_dt = round(min(np.diff(wf_psi4_time)), 2)
-                # max_dt = round(max(np.diff(wf_psi4_time)), 2)
-                # dt_auto = (time_axis[-1] - time_axis[0])/len(time_axis)
-                # dt_auto = int(dt_auto*100)/100
-                # dt_auto = round(mode(np.diff(time_axis))[0][0], 4)
-                dt_auto = mode(np.diff(time_axis))[0][0]
-
-                # message(f'Default dt is {dt_auto}')
-
-                # min_dt = round(min(np.diff(time_axis)), 2)
-                # max_dt = round(max(np.diff(time_axis)), 2)
-
-                min_dt = min(np.diff(time_axis))
-                max_dt = max(np.diff(time_axis))
-
-                message(f"Min dt {min_dt} and Max dt {max_dt}")
-
-                if resam_type == "finest":
-                    # Choose finest available timestep
-                    # for upto 3 decimal digits.
-                    m_dt = min_dt
-                    message("Resampling at the finest timestep", m_dt)
-                if resam_type == "coarsest":
-                    m_dt = max_dt
-                    message("Resampling at the coarsest timestep", m_dt)
-
-                if isinstance(resam_type, float):
-                    m_dt = resam_type
-                    message("Resampling at user defined timestep", m_dt)
-
-                if resam_type == "auto":
-                    # Choose the most popular timestep
-                    m_dt = dt_auto
-                    message("Resampling at the default timestep", m_dt)
-
-                message("Chosen resampling fineness:", resam_type)
-                # New (resampled) time axis
-                time_axis = np.arange(time_axis[0], time_axis[-1], m_dt)
-
-				# Length of data.
-				data_len = len(time_axis)
-				# message(data_len)
-
-				wfa.create_modes_array(ell_max=ell_max, data_len=data_len)
-				# message(wfa.mode(0,0).shape)
-				wfa.time_axis = time_axis
-
-			# Interpolate and resamplea
-			# Note
-			# Interpolating in amplitude and phase is better
-			# and has lower interpolation errors
-			# but is slower due to unwrapping of phases.
-
-            wf_int = interp_resam_wfs(
-                wf_data_c, wf_time, time_axis, kind="cubic", k=None
-            )
+        alias  :    str, optional.
+                                The simulation label. If not specified, then
+                                all available simulationswill be processed.
 
-			# amp_int = interp_resam_wfs(wf_amp, wf_time, time_axis)
-			# phase_int = interp_resam_wfs(wf_phase, wf_time, time_axis)
+        string :    str
+                                The string of a part of a file name.
 
-			# re_int = interp1d(wf_time, wf_data_re)
-			# message(wf_time[0], wf_time[-1], time_axis[0], time_axis[-1])
-			# re_dat = re_int(time_axis)
-
-			# im_int = interp1d(wf_time, wf_data_im)
-			# im_dat = im_int(time_axis)
-
-			# wfa.set_mode_data(ell, emm, data=re_dat + 1j * im_dat)
-			wfa.set_mode_data(ell, emm, data=wf_int)
-
-	if debug is True:
-		for ell, emm_list in modes_list:
-			for emm in emm_list:
-				this_key = f"Y_l{ell}_m{emm}.dat"
-
-				# Input waveform from disk
-				wf_data = wf_file[this_key]
-				wf_time = wf_data[:, 0]
-				wf_data_re = wf_data[:, 1]
-				wf_data_im = wf_data[:, 2]
-
-                if wf_nl.modes_data.all() == np.array(None):
-                    wf_nl.create_modes_array(
-                        ell_max=ell_max, data_len=len(wf_time)
-                    )
-                    wf_nl.time_axis = wf_time
-                    wf_nl.data_len = len(wf_time)
-
-				wf_nl.set_mode_data(ell, emm, data=wf_data_re + 1j * wf_data_im)
-
-	if centre:
-		wfa.trim(trim_upto_time=0)
-
-    if save_as_ma is True:
-        # Save the modes array as waveforms hdf file
-        wfa.save_modes(
-            out_file_name=f"{label}_resam.h5", compression_opts=compression_opts
-        )
-
-	wf_f0.close()
-
-	if debug is True:
-		return wfa, wf_nl
-	else:
-		return wfa
-
-
-########################################################################################################################
-# SpECTRE
-########################################################################################################################
-
-
-def load_SpECTRE_data_from_disk(
-	wfa=None,
-	label="SpECTRE Strain",
-	data_dir="./",
-	file_name="rhOverM_Extrapolated_N5_CoM_Mem.h5",
-	r_ext=None,
-	ell_max=12,
-	centre=True,
-	modes_list=None,
-	r_ext_factor=1,
-	save_as_ma="False",
-	resam_type="auto",
-	kind="cubic",
-	compression_opts=0,
-):
-    """Load the SpECTRE or SpEC CCE waveform to modes_array,from hdf5 files from disk.
+        Returns
+        -------
 
-    Parameters
-    ----------
-    wfa : modes_array, optional
-          The modes array to which to store the loaded waveform to.
-          A new modes array will be returned if not provided.
-    data_dir : string
-               A string containing the directory path where the mode files can be found.
-    file_name : string
-                The name of the file containing the waveform data.
-    label : string, optional
-            The label of the modes_array object.
-    ell_max : int, optional
-              The maximum mode number to load. If not specified,
-              then all available modes are loaded.
-    save_as_ma : bool, optional
-                 Save to disk again as a modes_array h5 file?
-    resam_type : string, float, optional
-                 The type of resampling to do. Options are
-                 the `finest` and `coarsest`, and user input float.
-    interp_kind : string, optional
-                  The interpolation type to use. Default is cubic.
-
-    Returns
-    -------
-    modes_array : modes_array
-                  A modes_array instance containing the loaded modes.
+        file_path : str
+                                The full path of the file
 
+        Notes
+        -----
 
-    """
-    spin_weight = -2
-    message("Loading SpECTRE data.", message_verbosity=1)
-    from waveformtools.waveforms import modes_array
-
-    # Load SXS waveforms to modes_array.
-    # Spectra infinty
-
-    full_path = f"{data_dir}/{file_name}"
-
-    try:
-        import scri
-    except Exception as ex:
-        message(
-            "scri module is required for reading in SXS waveforms. Please install and try again",
-            ex,
-        )
-        sys.exit(0)
-
-    wf_file = scri.rpxmb.load(full_path)[0].to_inertial_frame()
-    ell_max_act = wf_file.ell_max
-    # Add readinf ell max from file
-
-    if ell_max is None:
-        if wfa is None:
-            wfa_ell_max = None
-        else:
-            wfa_ell_max = wfa.ell_max
+        The first occuring instance of the file is returned
+        if there are multiple files found.
+        """
 
-        if wfa_ell_max is None:
-            ell_max = ell_max_act
-        else:
-            ell_max = wfa_ell_max
+        from pathlib import Path
 
-    if not wfa:
-        # Create a modes array
-        wfa = modes_array(label=label, ell_max=ell_max, modes_list=modes_list)
-
-    if not data_dir:
-        data_dir = wfa.data_dir
-    else:
-        wfa.data_dir = data_dir
-
-    if not file_name:
-        file_name = wfa.file_name
-    else:
-        wfa.file_name = file_name
-
-    if not ell_max:
-        ell_max = wfa.ell_max
-    else:
-        wfa.ell_max = ell_max
-
-    # ell_max        = 12
-    if not modes_list:
-        if not wfa.modes_list:
-            message("Constructing the modes list")
-            # sys.exit(0)
-            modes_list = construct_mode_list(
-                ell_max=ell_max, spin_weight=spin_weight
-            )
-        else:
-            modes_list = wfa.modes_list
-    else:
-        wfa.modes_list = modes_list
-
-    # flag = None
-
-    from scipy.stats import mode
-
-    for ell, emm_list in modes_list:
-        for emm in emm_list:
-            # message(ell, emm)
-            wf_data = wf_file.data[:, wf_file.index(ell, emm)]
-            wf_data_re = wf_data.real
-            wf_data_im = wf_data.imag
-
-            wf_time = wf_file.t
-            # message(type(wfa.modes_data))
-            if wfa.modes_data.all() == np.array(None):
-                time_axis = wf_time
-                message("Creating modes data")
-
-                # min_dt = round(min(np.diff(wf_psi4_time)), 2)
-                # max_dt = round(max(np.diff(wf_psi4_time)), 2)
-                # dt_auto = (time_axis[-1] - time_axis[0])/len(time_axis)
-                # dt_auto = int(dt_auto*100)/100
-                dt_auto = mode(np.diff(time_axis))[0][0]
-                # message(f'Default dt is {dt_auto}')
+        # The directory to look into.
+        path = self.ROOTDIR + alias
 
-                # min_dt = round(min(np.diff(time_axis)), 2)
-                # max_dt = round(max(np.diff(time_axis)), 2)
+        dir = Path(path)
+        # The path of the file.
+        # message(list(dir.rglob(string)))
+        try:
+            file_path = list(dir.rglob(string))[0]
+        except Exception as excep:
+            message("File not found!", excep)
 
-                min_dt = min(np.diff(time_axis))
-                max_dt = max(np.diff(time_axis))
+        return file_path
 
-                message(
-                    f"Min dt {min_dt} and Max dt {max_dt}", message_verbosity=2
-                )
+    def load_NP_1d_data(self, np_qty="sigma", source="qlm"):
+        """Load the 1d NP quantities."""
 
-                if resam_type == "finest":
-                    # Choose finest available timestep
-                    # for upto 3 decimal digits.
-                    m_dt = min_dt
-                    message(
-                        "Resampling at the finest timestep",
-                        m_dt,
-                        message_verbosity=1,
-                    )
-                if resam_type == "coarsest":
-                    m_dt = max_dt
-                    message(
-                        "Resampling at the coarsest timestep",
-                        m_dt,
-                        message_verbosity=1,
-                    )
-
-                if isinstance(resam_type, float):
-                    m_dt = resam_type
-                    message(
-                        "Resampling at user defined timestep",
-                        m_dt,
-                        message_verbosity=1,
-                    )
-
-                if resam_type == "auto":
-                    # Choose finest available timestep
-                    # for upto 3 decimal digits.
-                    m_dt = dt_auto
-                    message(
-                        "Resampling at the default timestep",
-                        m_dt,
-                        message_verbosity=1,
-                    )
-
-				# New (resampled) time axis
-				time_axis = np.arange(time_axis[0], time_axis[-1], m_dt)
-
-				# Length of data.
-				data_len = len(time_axis)
-				# message(data_len)
-
-				wfa.create_modes_array(ell_max=ell_max, data_len=data_len)
-				# message(wfa.mode(0,0).shape)
-				wfa.time_axis = time_axis
-
-			re_int = interp1d(wf_time, wf_data_re, kind=kind)
-			# message(wf_time[0], wf_time[-1], time_axis[0], time_axis[-1])
-			re_dat = re_int(time_axis)
-
-			im_int = interp1d(wf_time, wf_data_im, kind=kind)
-			im_dat = im_int(time_axis)
-
-			wfa.set_mode_data(ell, emm, data=re_dat + 1j * im_dat)
-
-	if centre:
-		wfa.trim(trim_upto_time=0)
-
-    if save_as_ma is True:
-        # Save the modes array as waveforms hdf file
-        wfa.save_modes(
-            out_file_name=f"{label}_resam.h5", compression_opts=compression_opts
-        )
-
-	return wfa
-
-
-########################################################################################################################
-# Output
-########################################################################################################################
-
-
-def save_modes_data_to_gen(
-	wfa,
-	ell_max=None,
-	pre_key=None,
-	key_format=None,
-	modes_to_save=None,
-	out_file_name="mp_new_modes.h5",
-	r_ext_factor=None,
-	compression_opts=0,
-	r_ext=None,
-):
-    """Save the waveform mode data to an hdf file.
+        import re
 
-    Parameters
-    ----------
-    pre_key : str, optional
-              A string containing the key of the group in
-              the HDF file in which the modes` dataset exists.
-              It defaults to `None`.
-    mode_numbers : list
-                   The mode numbers to load from the file.
-                   Each item in the list is a list that
-                   contains two integrer numbers, one for
-                   the mode index :math:`\\ell` and the
-                   other for the mode index :math:`m`.
+        np_data_dict = {}
 
-    Returns
-    -------
-    waveform_obj : 3d array
-                   Sets the three dimensional array `waveform.modes`
-                   that contains the required :math:`\\ell, m` modes.
-
-    Examples
-    --------
-    >>> from waveformtools.waveforms import modes_array
-    >>> wf = modes_array()
-    >>> wf.data_dir = './'
-    >>> wf.filename = 'data_file.h5'
-    >>> wf.modes_list = [[2, 2], [3, 3]]
-    >>> wf.load_gen_data()
-    """
-    # from waveformtools.waveforms import modes_array
+        if self.NP_1d is None:
+            self.NP_1d = {}
 
-    #############################
-    # I/O assignments.
-    #############################
-
-    wfa.out_file_name = wfa.label + "_" + out_file_name
-    wfa.out_file_name = wfa.out_file_name.replace(" ", "_")
-    wfa.out_file_name = wfa.out_file_name.replace("->", "_")
-
-    # get the full path.
-    full_path = wfa.data_dir + "/" + wfa.out_file_name
-
-    if r_ext is None:
-        if wfa.r_ext is None:
-            r_ext = 500
-        else:
-            r_ext = wfa.r_ext
+        np_data_alias_dict = {}
 
-    if r_ext_factor is None:
-        r_ext_factor = wfa.r_ext
+        for alias in self.aliases:
+            if source == "qlm":
+                file_string = f"{self.data_dir}quasilocalmeasures-qlm_newman_penrose..asc"
+            elif source == "ih":
+                file_string = f"{self.data_dir}isolatedhorizon-ih_newman_penrose..asc"
 
-    ###################################
-    # Identify the modes to save.
-    ###################################
-
-    if not modes_to_save:
-        if ell_max is not None:
-            modes_to_save = wfa.modes_list[:ell_max]
+            full_file_path = self._get_file_path_from_str(alias, string=file_string)
 
-        else:
-            modes_to_save = wfa.modes_list
+            with open(full_file_path, "r") as file:
+                for line_index in range(15):
+                    fline = next(file)
+                    # message(fline)
+                    str_match = re.search(f"\d\d:qlm_np{np_qty}", fline)
+                    # message(str_match)
+                    if str_match is not None:
+                        start_col = int(str_match[0][:2])
+                        # message(start_col)
+                        break
 
-    ##########################
-    # Create the modes file.
-    ##########################
-    message("Saving waveform", wfa.label, message_verbosity=2)
-    with h5py.File(full_path, "w") as wfile:
-        # Create the metadata dataset.
-        metadata = wfa.get_metadata()
-
-        message(metadata, message_verbosity=1)
-
-        metadata_bytes = json.dumps(metadata).encode()
-
-        # dt = h5py.special_dtype(vlen=str)
-        # metadata=np.asarray([metadata_bytes], dtype=dt)
-        wfile.create_dataset(
-            "metadata", data=metadata_bytes, compression_opts=compression_opts
-        )
-
-        # Load the modes listed in mode_numbers list
-        for item in modes_to_save:
-            # For every ell mode list in modes_list
-
-            ell_value, emm_list = item
-
-            for emm_value in emm_list:
-                # For every (ell, emm) mode.
-
-                data = wfa.mode(ell_value, emm_value)
-                # set the time and data axis
-                data_re = data.real
-                data_im = data.imag
+            NP_all_data = np.genfromtxt(full_file_path)[
+                :, np.r_[8, start_col - 1, start_col, start_col + 1, start_col + 2, start_col + 3, start_col + 4]
+            ]
 
-                save_data = np.transpose(
-                    np.array([wfa.time_axis, data_re, data_im])
-                )
-                # Make the key
-                key = _key_gen(ell_value, emm_value, extras=f"r{r_ext:.2f}")
-                # message('Processing key', key)
-                # Create data set
-                wfile.create_dataset(key, data=save_data)
+            np_data_alias_dict.update({alias: NP_all_data})
 
-    return 1
+        self.NP_1d.update({np_qty: np_data_alias_dict})
```

### Comparing `waveformtools-2023.6.3/waveformtools/diagnostics.py` & `waveformtools-2023.6.5/waveformtools/diagnostics.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 import numpy as np
 
 
 class method_info:
     """The methods for integration ,differential to be passed on
     for operations."""
 
-    def __init__(
-        self, int_method="MP", diff_method="SH", ell_max=8, degree=8, reg=True
-    ):
+    def __init__(self, int_method="MP", diff_method="SH", ell_max=8, degree=8, reg=True):
         self.int_method = int_method
         self.diff_method = diff_method
         self.ell_max = ell_max
         self.reg = reg
         self.degree = degree
```

### Comparing `waveformtools-2023.6.3/waveformtools/differentiate.py` & `waveformtools-2023.6.5/waveformtools/differentiate.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,19 +64,15 @@
             x_uniform = np.linspace(x_data[0], x_data[-1], 2 * len(x_data))
             y_uniform = interp1d(x_data, y_data, kind="cubic")(x_uniform)
 
         delta_x = np.diff(x_uniform)[0]
 
         if method == "FS":
             dydx_new, _, x_new, _ = Fourier_differential(
-                delta_x=delta_x,
-                udata_x=y_uniform,
-                order=1,
-                zero_mode=0,
-                taper=False,
+                delta_x=delta_x, udata_x=y_uniform, order=1, zero_mode=0, taper=False
             )
 
         elif method == "FD":
             if degree == 1:
                 dydx_new = differentiate(y_uniform, delta_x)
             elif degree == 2:
                 dydx_new = differentiate2(y_uniform, delta_x)
@@ -140,76 +136,72 @@
     """Differentiate a function using the Chebyshev expansion.
 
 
     Parameters
     ----------
 
 
-    x_data: 1d array
+    x_data:	1d array
                                                     The x data.
-    y_data: 1d array
+    y_data:	1d array
                                     The y data.
 
-    order:  int
+    order:	int
                                     The number of times to differentiate.
 
-    degree: int
+    degree:	int
                                                     The number of basis functions to use.
 
 
     Returns
     -------
 
-    dydx_data:  1d array
+    dydx_data:	1d array
                                                     The differentiated data.
 
     """
 
     # Find the basis coefficients.
     from numpy.polynomial.chebyshev import chebder, chebfit, chebval
 
     # L2errs = []
     # p_res = 1e21
     # for deg_index in range(degree):
-    #   cheb_coeffs, result = chebfit(x_data, y_data, deg=deg_index, full=True)
-    #   res = result[0][0]
+    # 	cheb_coeffs, result = chebfit(x_data, y_data, deg=deg_index, full=True)
+    # 	res = result[0][0]
     # if res%2==0:
-    #   L2errs.append(res)
+    # 	L2errs.append(res)
     # print(x_data, y_data)
     cheb_coeffs, result = chebfit(x_data, y_data, deg=degree, full=True)
 
     message("Result", result, result[0], message_verbosity=1)
     res = result[0][0]
 
     # L2errs = [(a + b)  for a, b in zip(L2errs[::2], L2errs[1::2])]
 
     # best_deg = 2*np.argmin(L2errs)+2
     # if best_deg<degree:
     # plt.plot(L2errs)
     # plt.show()
 
-    #   print(f'Optimizing degree to {best_deg}')
-    #   degree=best_deg
-    #   cheb_coeffs, result = chebfit(x_data, y_data, deg=degree, full=True)
+    # 	print(f'Optimizing degree to {best_deg}')
+    # 	degree=best_deg
+    # 	cheb_coeffs, result = chebfit(x_data, y_data, deg=degree, full=True)
 
-    #   res = result[0][0]
+    # 	res = result[0][0]
     if res >= 1e-3:
         if res <= 1e-1 and res >= 1e-3:
             message(f"Residue warning {res}")
         elif res > 1e-1:
             import traceback
 
             traceback.print_stack()
             y_fit_data = chebval(x_data, cheb_coeffs)
-            plt.scatter(
-                x_data, y_data, label="Input", s=3, c="magenta", marker="o"
-            )
-            plt.scatter(
-                x_data, y_fit_data, label="fit", s=3, c="blue", marker="X"
-            )
+            plt.scatter(x_data, y_data, label="Input", s=3, c="magenta", marker="o")
+            plt.scatter(x_data, y_fit_data, label="fit", s=3, c="blue", marker="X")
             plt.grid()
             plt.legend()
             plt.show()
 
             message(f"Residue warning {res}: Bad fit!")
 
     # compute the derivative
@@ -222,64 +214,56 @@
 
 
 ########################################################
 # Fourier differentiation
 ########################################################
 
 
-def Fourier_differential(
-    delta_x,
-    udata_x=None,
-    utilde_conven=None,
-    omega0=np.inf,
-    order=1,
-    zero_mode=0,
-    taper=True,
-):
+def Fourier_differential(delta_x, udata_x=None, utilde_conven=None, omega0=np.inf, order=1, zero_mode=0, taper=True):
     """Fixed frequency differentiation, the inverse of the
     Fixed frequency integration as presented in Reisswig et al.
     This function takes in a function and returns its nth order
     derivative differential taken in the frequency domain.
 
 
     Parameters
     ----------
-    xaxis:  1d array
+    xaxis:	1d array
                     The co-ordinate space axis.
-    udata_x:    1d array
+    udata_x:	1d array
                             The data to be differentiated,
                             expressed in coordinate space.
-    omega0: float, optional
+    omega0:	float, optional
                     The cutoff angular frequency in the integration.
                     Must be lower than the starting angular frequency
                     of the input waveform.
-    order:  int, optional
+    order:	int, optional
                     The number of times to differentiate
                     the integrand in time.
-    zero_mode:  float, optional
+    zero_mode:	float, optional
                             The zero mode amplitude of the FFT required.
-    taper:  bool
+    taper:	bool
                     Whether or not to taper the real co-ordinate space data.
 
     Returns
     -------
-    udata_differentiated:   1d array
+    udata_differentiated:	1d array
                                                     The input waveform in time-space, integrated
                                                     in frequency space using FFI.
 
-    utilde_differentiated:  1d array
+    utilde_differentiated:	1d array
                                                     The FFT of the frixed frequency
                                                     differentiated array in good conventions.
 
 
-    new_x_axis: 1d array
+    new_x_axis:	1d array
                             The new x-axis, assuming the
                             data may have been changed in length
 
-    freq_axis:  1d array
+    freq_axis:	1d array
                             The frequency axis of the FFT of data.
 
     Notes
     -----
 
     The returned differentiated function of a real udata_x
     in real co-ordinate space is a complex number
@@ -366,23 +350,23 @@
 
 def differentiate(data, delta_t):
     """Central difference derivative calculator. Forward/ backward Euler near the boundaries.
 
     Parameters
     ----------
 
-    data:   1d array
+    data:	1d array
                                     The 1d data.
-    delta_t:    float
+    delta_t:	float
                                                     The time step in units of t/M.
 
     Returns
     -------
 
-    dAdt:   1d array
+    dAdt:	1d array
                                     The derivative.
 
     """
 
     # A list to hold the derivatives.
     dAdt = []
 
@@ -406,23 +390,23 @@
 def differentiate2(data, delta_t):
     """Five point difference derivative calculator.  Not accurate near the boundaries.
 
 
     Parameters
     ----------
 
-    data:   1d array
+    data:	1d array
                                     The 1d data.
-    delta_t:    float
+    delta_t:	float
                                                     The time step in t/M.
 
     Returns
     -------
 
-    dAdt:   1d array
+    dAdt:	1d array
                                     The derivative.
 
     """
 
     # Number of points on right side.
     order = 2
 
@@ -461,23 +445,23 @@
 def differentiate3(data, delta_t):
     """Seven point difference derivative calculator. Not accurate near the boundaries.
 
 
     Parameters
     ----------
 
-    data:   1d array
+    data:	1d array
                                     The 1d data.
-    delta_t:    float
+    delta_t:	float
                                                     The time step in t/M.
 
     Returns
     -------
 
-    dAdt:   1d array
+    dAdt:	1d array
                                     The derivative.
 
     """
 
     # The number of points on one direction.
     order = 3
     # The seven point stencil.
@@ -527,23 +511,23 @@
 def differentiate4(data, delta_t):
     """Nine point difference derivative calculator. Not accurate near the boundaries.
 
 
     Parameters
     ----------
 
-    data:   1d array
+    data:	1d array
                                     The 1d data.
-    delta_t:    float
+    delta_t:	float
                                                     The time step in t/M.
 
     Returns
     -------
 
-    dAdt:   1d array
+    dAdt:	1d array
                                     The derivative.
 
     """
 
     # The number of points on one side.
     order = 4
     # THe stencil.
@@ -609,23 +593,23 @@
 def differentiate5(data, delta_t):
     """Eleven point difference derivative calculator. Not accurate near the boundaries.
 
 
     Parameters
     ----------
 
-    data:   1d array
+    data:	1d array
                                     The 1d data.
-    delta_t:    float
+    delta_t:	float
                                                     The time step in t/M.
 
     Returns
     -------
 
-    dAdt:   1d array
+    dAdt:	1d array
                                     The derivative of the data.
 
     """
 
     # The number of points on one side.
     order = 5
     # The stencil.
@@ -705,23 +689,23 @@
 def differentiate5_vec_nonumba(data, delta_t):
     """Eleven point difference derivative calculator. Not accurate near the boundaries.
 
 
     Parameters
     ----------
 
-    data:   1d array
+    data:	1d array
                                     The 1d data.
-    delta_t:    float
+    delta_t:	float
                                                     The time step in t/M.
 
     Returns
     -------
 
-    dAdt:   1d array
+    dAdt:	1d array
                                     The derivative of the data.
 
     """
 
     # import pdb
     # pdb.set_trace()
 
@@ -795,17 +779,15 @@
     # der_data = np.append(der_data, [der4], axis=aax)
     der_data[4] = der4
     for index in range(order, len(data) - order):
         # For the interior points.
         data_subarray = data[index - order : index + order + 1]
         # der_data = np.append(der_data, [np.tensordot(coeffs, data_subarray, axes=((0), (0)))
         # / (divide * delta_t)], axis=aax)
-        der_data[index] = np.tensordot(
-            coeffs, data_subarray, axes=((0), (0))
-        ) / (divide * delta_t)
+        der_data[index] = np.tensordot(coeffs, data_subarray, axes=((0), (0))) / (divide * delta_t)
 
     # der_data = np.append(der_data, [derNm5], axis=aax)
     der_data[-5] = derNm5
     # der_data = np.append(der_data, [derNm4], axis=aax)
     der_data[-4] = derNm4
     # der_data = np.append(der_data, [derNm3], axis=aax)
     der_data[-3] = derNm3
@@ -822,23 +804,23 @@
 def differentiate5_vec_numba(data, delta_t):
     """Eleven point difference derivative calculator. Not accurate near the boundaries.
 
 
     Parameters
     ----------
 
-    data:   1d array
+    data:	1d array
                                     The 1d data.
-    delta_t:    float
+    delta_t:	float
                                                     The time step in t/M.
 
     Returns
     -------
 
-    dAdt:   1d array
+    dAdt:	1d array
                                     The derivative of the data.
 
     """
 
     # import pdb
     # pdb.set_trace()
 
@@ -931,17 +913,15 @@
     for index in range(order, len(data) - order):
         # For the interior points.
         data_subarray = data[index - order : index + order + 1]
         # der_data = np.append(der_data, [np.tensordot(coeffs, data_subarray, axes=((0), (0)))
         # / (divide * delta_t)], axis=aax)
         # der_data[index] = np.tensordot(coeffs, data_subarray, axes=((0), (0))) / (divide * delta_t)
         for inner_index, val in enumerate(coeffs):
-            der_data[index] += (
-                val * data_subarray[inner_index] / (divide * delta_t)
-            )
+            der_data[index] += val * data_subarray[inner_index] / (divide * delta_t)
 
     # der_data = np.append(der_data, [derNm5], axis=aax)
     # der_data[-5] = derNm5
     # der_data = np.append(der_data, [derNm4], axis=aax)
     # der_data[-4] = derNm4
     # der_data = np.append(der_data, [derNm3], axis=aax)
     # der_data[-3] = derNm3
@@ -960,42 +940,34 @@
 
 
 def differentiate_cwaveform(time_axis, waveform, method="SP", degree=5):
     """Differentiate a given waveform by differentiating the Amplitude-Phase form.
 
     Parameters
     ----------
-    time_axis:  1d array
+    time_axis:	1d array
                 The time axis of the waveform.
 
-    waveform:   1d array
+    waveform:	1d array
                 The complex 1d array of the waveform timeseries.
 
 
     Returns
     -------
-    differentiated_waveform:    1d array
+    differentiated_waveform:	1d array
                                 The waveform differentiated in time.
 
     """
 
     # Get the amplitude and phase of the complex 1d waveform.
     from waveformtools.waveformtools import xtract_camp_phase
 
-    waveform_amp, waveform_phase = xtract_camp_phase(
-        waveform.real, waveform.imag
-    )
+    waveform_amp, waveform_phase = xtract_camp_phase(waveform.real, waveform.imag)
 
     # Differentiate the waveform.
 
-    Amplitude_dot = derivative(
-        time_axis, waveform_amp, method=method, degree=degree
-    )
-    Phase_dot = derivative(
-        time_axis, waveform_phase, method=method, degree=degree
-    )
-
-    differentiated_waveform = (
-        Amplitude_dot + waveform_amp * 1j * Phase_dot
-    ) * np.exp(1j * waveform_phase)
+    Amplitude_dot = derivative(time_axis, waveform_amp, method=method, degree=degree)
+    Phase_dot = derivative(time_axis, waveform_phase, method=method, degree=degree)
+
+    differentiated_waveform = (Amplitude_dot + waveform_amp * 1j * Phase_dot) * np.exp(1j * waveform_phase)
 
     return differentiated_waveform
```

### Comparing `waveformtools-2023.6.3/waveformtools/extrapolate.py` & `waveformtools-2023.6.5/waveformtools/extrapolate.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,283 +9,276 @@
 
 ###############################################
 # Basic utilities
 ###############################################
 
 
 def r_to_ra_conversion(coord_radius, mass=1, spin=0):
-    """Convert the isotropic co-ordinate radius parameter `r`
-    in the ETK simulations into the approximate areal radius.
+    """Convert the isotropic co-ordinate radius parameter `r` in the ETK simulations
+            into the approximate areal radius.
 
     Parameters
     ----------
-    coord_radius : float
-                   The coordinate radius in the Einstein toolkit
-    mass : float, optional
-           The sum of the quasi-local (Christodolou) horizon masses
-           of the black holes. Defaults to 1.
-    spin : float, optional
-           The magnitude of the spin of the system, as approximated
-           by a single Kerr black hole far away from the system.
-           Defaults to 0.
+
+    coord_radius:	float
+                                    The coordinate radius in the Einstein toolkit
+
+    mass:	float, optional
+                    The sum of the quasi-local horizon (Christodolou) masses of the black holes.
+                    Defaults to 1.
+
+    spin:	float, optional
+                    The magnitude of the spin of the system, as approximated by a single Kerr black hole
+                    far away from the system. Defaults to 0.
+
 
     Returns
     -------
-    areal_radius : float
-                   The appriximate areal radius of the sphere.
+
+    areal_radius:	float
+                                    The appriximate areal radius of the sphere.
 
 
     Notes
     -----
-    Assumes that the system interoir to the sphere at co-ordinate radius `r_coord`
-    is well approximated by a deformed Kerr black hole.
+
+    Assumes that the system interoir to the sphere at co-ordinate radius `r_coord` is well approximated by a
+    Kerr black hole.
+
+
 
     References
     ----------
 
-    Nakano et al., (2015),  Phys. Rev. D 91, 104022, in-text below Eq.[30].
+    Nakano et al., (2015),	Phys. Rev. D 91, 104022, in-text below Eq.[30].
     """
 
-    areal_radius = (
-        coord_radius
-        * (1 + (mass + spin) / (2 * coord_radius))
-        * (1 + (mass - spin) / (2 * coord_radius))
-    )
+    areal_radius = coord_radius * (1 + (mass + spin) / (2 * coord_radius)) * (1 + (mass - spin) / (2 * coord_radius))
 
     return areal_radius
 
 
 ############################################################################
 # Perturbative extraction
 ############################################################################
 
 
 def waveextract_to_inf_perturbative_twop5_order(
-    rPsi4_rlm,
-    delta_t,
-    areal_radius=500,
-    mass=1,
-    spin=0,
-    ell=2,
-    emm=2,
-    degree=24,
-    method="CS",
+    rPsi4_rlm, delta_t, areal_radius=500, mass=1, spin=0, ell=2, emm=2, degree=24, method="CS"
 ):
     """Extract a numerical waveform to null infinity using perturbative techniques. This is :
             * accurate to second order in :math:`1/r`.
             * accurate to first order in Kerr mass and spin.
             * corrects for spheroidal harmonics
 
+
+
     Parameters
     ----------
-    rPsi4_rlm : 1d array
-                The extracted Weyl scalar :math:`r\\Psi_{4\\ell m}` data array
-    delta_t : float
-              The time stepping.
-    areal_radius : 1d array
-                   The areal radius of the extraction sphere.
-    mass : float
-           The total horizon mass of the system.
-    spin : float, optional
-           The effective spin of the spacetime. Defaults to 0.
-    ell : int
-          The polar quantum number :math:`\\ell`.
-    emm : int
-          The azimuthal quantum number :math:`m`.
-    method : str
-             The method to use for differentiation.
-    degree : int
-             The degree to use for dfferentiation.
 
+    rPsi4_rlm:	1d array
+                            The extracted Weyl scalar :math:`r\\Psi_{4\\ell m}` data array
+    delta_t:	float
+                            The time stepping.
+    areal_radius:	1d array
+                                    The areal radius of the extraction sphere.
+    mass:	float
+                    The total horizon mass of the system.
+    spin:	float, optional
+                    The effective spin of the spacetime. Defaults to 0.
+    ell:	int
+                    The polar quantum number :math:`\\ell`.
+    emm:	int
+                    The azimuthal quantum number :math:`m`.
+        method: str
+                        The method to use for differentiation.
+        degree: int
+                        The degree to use for dfferentiation.
     Returns
     -------
-    rPsi4_inflm : 1d array
-                  The waveform extracted to
-                  null infninity :math:`\\mathcal{I}^+`
+
+    rPsi4_inflm:	1d array
+                            The waveform extracted to null infninity :math:`\\mathcal{I}^+`
+
 
     References
     ----------
-    This implements the definition in Nakano et al., (2015),
-    Phys. Rev. D 91, 104022 Eq.[29].
+
+    This implements the definition in Nakano et al., (2015),  Phys. Rev. D 91, 104022 Eq.[29].
+
+
     """
 
     from waveformtools.differentiate import differentiate_cwaveform
     from waveformtools.integrate import fixed_frequency_integrator
 
     # Timeaxis
 
     timeaxis = np.arange(0, len(rPsi4_rlm) * delta_t, delta_t)
     # Assigning the terms. Each set of subterms in a pair of paranthesis is a term.
     term_1_prefac = 1 - 2 * mass / areal_radius
     subterm_1_1 = rPsi4_rlm
     subterm_1_2_prefac = (ell - 1) * (ell + 2) / (2 * areal_radius)
-    subterm_1_2, _ = fixed_frequency_integrator(
-        rPsi4_rlm, delta_t, omega0=0.015
-    )  # Integral_rPsi4_rlm
-    subterm_1_3_prefac = (
-        (ell - 1) * (ell + 2) * (ell**2 + ell - 4) / (8 * areal_radius**2)
-    )
-    subterm_1_3, _ = fixed_frequency_integrator(
-        rPsi4_rlm, delta_t, order=2, omega0=0.015
-    )  # Double_integral_rPsi4_rlm
-
-    term_1 = term_1_prefac * (
-        subterm_1_1
-        + subterm_1_2_prefac * subterm_1_2
-        + subterm_1_3_prefac * subterm_1_3
-    )
+    subterm_1_2, _ = fixed_frequency_integrator(rPsi4_rlm, delta_t, omega0=0.015)  # Integral_rPsi4_rlm
+    subterm_1_3_prefac = (ell - 1) * (ell + 2) * (ell**2 + ell - 4) / (8 * areal_radius**2)
+    subterm_1_3, _ = fixed_frequency_integrator(rPsi4_rlm, delta_t, order=2, omega0=0.015)  # Double_integral_rPsi4_rlm
+
+    term_1 = term_1_prefac * (subterm_1_1 + subterm_1_2_prefac * subterm_1_2 + subterm_1_3_prefac * subterm_1_3)
 
     term_2_prefac = (2 * 1j * spin / (ell + 1) ** 2) * np.sqrt(
-        (ell + 3)
-        * (ell - 1)
-        * (ell + emm + 1)
-        * (ell - emm + 1)
-        / ((2 * ell + 1) * (2 * ell + 3))
+        (ell + 3) * (ell - 1) * (ell + emm + 1) * (ell - emm + 1) / ((2 * ell + 1) * (2 * ell + 3))
     )
-    subterm_2_1 = differentiate_cwaveform(
-        timeaxis, rPsi4_rlm, method=method, degree=degree
-    )  # Differential of waveform
+    subterm_2_1 = differentiate_cwaveform(timeaxis, rPsi4_rlm, method=method, degree=degree)  # Differential of waveform
     subterm_2_2_prefac = -ell * (ell + 3) / areal_radius
     subterm_2_2 = subterm_1_1
 
     term_2 = term_2_prefac * (subterm_2_1 + subterm_2_2_prefac * subterm_2_2)
 
     term_3_prefac = (-2 * 1j * spin / ell**2) * np.sqrt(
-        ((ell + 2) * (ell - 2) * (ell + emm) * (ell - emm))
-        / ((2 * ell - 1) * (2 * ell + 1))
+        ((ell + 2) * (ell - 2) * (ell + emm) * (ell - emm)) / ((2 * ell - 1) * (2 * ell + 1))
     )
     subterm_3_1 = subterm_2_1
     subterm_3_2_prefac = -(ell - 2) * (ell + 1) / areal_radius
     subterm_3_2 = subterm_1_1
 
     term_3 = term_3_prefac * (subterm_3_1 + subterm_3_2_prefac * subterm_3_2)
 
     rPsi4_inflm = term_1 + term_2 + term_3
 
     return rPsi4_inflm
 
 
-def waveextract_to_inf_perturbative_two_order(
-    rPsi4_rlm, delta_t, areal_radius=500, mass=1, ell=2
-):
+def waveextract_to_inf_perturbative_two_order(rPsi4_rlm, delta_t, areal_radius=500, mass=1, ell=2):
     """Extract a numerical waveform to null infinity using perturbative techniques. This is :
             * accurate to second order in :math:`1/r`.
             * accurate to first order in Kerr mass and spin.
             * corrects for spheroidal harmonics
 
+
+
     Parameters
     ----------
-    rPsi4_rlm : 1d array
-                The extracted Weyl scalar :math:`r\\Psi_{4\\ell m}` data array.
-    delta_t : float
-              The time stepping.
-    areal_radius : 1d array
-                   The areal radius of the extraction sphere.
-    mass : float
-           The total horizon mass of the system.
-
-    spin : float, optional
-           The effective spin of the spacetime. Defaults to 0.
-    ell : int
-          The polar quantum number :math:`\\ell`.
-    emm : int
-          The azimuthal quantum number :math:`m`.
+
+    rPsi4_rlm:	1d array
+                            The extracted Weyl scalar :math:`r\\Psi_{4\\ell m}` data array.
+
+    delta_t:	float
+                            The time stepping.
+
+    areal_radius:	1d array
+                                    The areal radius of the extraction sphere.
+
+
+    mass:	float
+                    The total horizon mass of the system.
+
+    spin:	float, optional
+                    The effective spin of the spacetime. Defaults to 0.
+
+    ell:	int
+                    The polar quantum number :math:`\\ell`.
+
+    emm:	int
+                    The azimuthal quantum number :math:`m`.
 
     Returns
     -------
-    rPsi4_inflm : 1d array
-                  The waveform extracted to
-                  null infninity :math:`\\mathcal{I}^+`
+
+    rPsi4_inflm:	1d array
+                            The waveform extracted to null infninity :math:`\\mathcal{I}^+`
+
 
     References
     ----------
-    This implements the definition in Nakano et al., (2015),
-    Phys. Rev. D 91, 104022 Eq.[29].
+
+    This implements the definition in Nakano et al., (2015),  Phys. Rev. D 91, 104022 Eq.[29].
+
+
     """
 
     from integrate import fixed_frequency_integrator
 
     # Assigning the terms. Each set of subterms in a pair of paranthesis is a term.
     term_1 = rPsi4_rlm
 
     term_2_prefac = -(ell - 1) * (ell + 2) / (2 * areal_radius)
-    subterm_2_1, _ = fixed_frequency_integrator(
-        rPsi4_rlm, delta_t, omega0=0.015
-    )  # Integral_rPsi4_rlm
+    subterm_2_1, _ = fixed_frequency_integrator(rPsi4_rlm, delta_t, omega0=0.015)  # Integral_rPsi4_rlm
     term_2 = term_2_prefac * subterm_2_1
 
-    term_3_prefac = (
-        (ell - 1) * (ell + 2) * (ell**2 + ell - 4) / (8 * areal_radius**2)
-    )
-    subterm_3_1, _ = fixed_frequency_integrator(
-        rPsi4_rlm, delta_t, order=2, omega0=0.015
-    )  # Double_Integral_rPsi4_rlm
+    term_3_prefac = (ell - 1) * (ell + 2) * (ell**2 + ell - 4) / (8 * areal_radius**2)
+    subterm_3_1, _ = fixed_frequency_integrator(rPsi4_rlm, delta_t, order=2, omega0=0.015)  # Double_Integral_rPsi4_rlm
     term_3 = term_3_prefac * subterm_3_1
 
     term_4_prefac = -3 * mass / (2 * areal_radius**2)
     subterm_4_1 = subterm_2_1
     term_4 = term_4_prefac * subterm_4_1
 
     rPsi4_inflm = term_1 + term_2 + term_3 + term_4
 
     return rPsi4_inflm
 
 
-def waveextract_to_inf_perturbative_one_order(
-    u_ret, rPsi4_rlm, areal_radius=500, ell=2
-):
+def waveextract_to_inf_perturbative_one_order(u_ret, rPsi4_rlm, areal_radius=500, ell=2):
     """Extract a numerical waveform to null infinity using perturbative techniques. This is :
             * accurate to second order in :math:`1/r`.
             * accurate to first order in Kerr mass and spin.
             * corrects for spheroidal harmonics
 
+
+
     Parameters
     ----------
-    u_ret : 1d array
-            The retarted time array at the location r = areal_radius.
-    rPsi4_rlm : 1d array
-                The extracted Weyl scalar :math:`r\\Psi_{4\\ell m}` data array
-    areal_radius : 1d array
-                   The areal radius of the extraction sphere.
-    mass : float
-           The total horizon mass of the system.
-    ell : int
-          The polar quantum number :math:`\\ell`.
-    emm : int
-          The azimuthal quantum number :math:`m`.
+
+    u_ret:	1d array
+                    The retarted time array at the location r = areal_radius.
+
+    rPsi4_rlm:	1d array
+                            The extracted Weyl scalar :math:`r\\Psi_{4\\ell m}` data array
+
+    areal_radius:	1d array
+                                    The areal radius of the extraction sphere.
+
+
+    mass:	float
+                    The total horizon mass of the system.
+
+    ell:	int
+                    The polar quantum number :math:`\\ell`.
+
+    emm:	int
+                    The azimuthal quantum number :math:`m`.
 
     Returns
     -------
-    rPsi4_inflm : 1d array
-                  The waveform extracted to
-                  null infninity :math:`\\mathcal{I}^+`
+
+    rPsi4_inflm:	1d array
+                            The waveform extracted to null infninity :math:`\\mathcal{I}^+`
+
 
     References
     ----------
-    This implements the definition in
-    Nakano et al., (2015),  Phys. Rev. D 91, 104022 Eq.[29].
+
+    This implements the definition in Nakano et al., (2015),  Phys. Rev. D 91, 104022 Eq.[29].
+
+
     """
 
     # Get the amplitude and phase
     A_lm, _ = waveformtools.xtract_camp_phase(rPsi4_rlm.real, rPsi4_rlm.imag)
 
     # Get the time stepping
     delta_t = u_ret[1] - u_ret[0]
 
     # Get the waveform instantaneous frequency
-    omega_lm = waveformtools.get_waveform_angular_frequency(
-        rPsi4_rlm, delta_t=delta_t, timeaxis=u_ret
-    )
+    omega_lm = waveformtools.get_waveform_angular_frequency(rPsi4_rlm, delta_t=delta_t, timeaxis=u_ret)
 
     # Assigning the terms. Each set of subterms in a pair of paranthesis is a term.
 
     # The amplitude correction factor
-    A_lm_correction = 0.5 * np.power(
-        ((ell * (ell + 1) / (2 * omega_lm * areal_radius))), 2
-    )
+    A_lm_correction = 0.5 * np.power(((ell * (ell + 1) / (2 * omega_lm * areal_radius))), 2)
 
     # The phase correction factor.
     sin_Phase_correction = ell * (ell + 1) / (2 * omega_lm * areal_radius)
     cos_Phase_correction = np.sqrt(1 - np.power(sin_Phase_correction, 2))
     Phase_correction = cos_Phase_correction + 1j * sin_Phase_correction
 
     # The extrapolated waveform
```

### Comparing `waveformtools-2023.6.3/waveformtools/grids.py` & `waveformtools-2023.6.5/waveformtools/grids.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,64 +8,65 @@
 gl_grid : grid info
           Stores a Gauss-Legendre type grid on a spherical surface.
 """
 
 import numpy as np
 
 # from numba import jit, njit
+
 # import numba as nb
+
 # from numba.experimental import jitclass
 
 
 class spherical_grid:
     """A class to store the coordinate grid on a sphere.
 
     Attributes
     ----------
-    ntheta : int
-             The number of angular points in the :math:`\\theta`
-             direction, including ghost zones.
-    nphi : int
-           The number of angular points in the :math:`\\phi`
-           direction, including ghost zones.
-    nghosts : int
-              The number of ghost zones at the end of
-              each direction.
-    meshgrid : tuple of 2d array
-               The 2d array containing the meshgrid of
-               (:math:`\\theta, \\phi`) angular points.
-    theta_1d : 1d array
-               The 1d array of angular points
-               along the :math:`\\theta` axis.
-    phi_1d : 1d array
-             The 1d array of angular points
-             along the :math:`\\phi` axis.
-    dtheta : float
-             The angular step size in the :math:`\\theta`
-             direction.
-    dphi : float
-           The angular step size in the :math:`\\phi`
-           direction.
-    npix_act : int
-               The total number of gridpoints on the sphere,
-               excluding the ghost points.
-    meshgrid : 2darray (2)
-               Get the 2d angular grid.
+    ntheta: int
+                            The number of angular points in the :math:`\\theta`
+                            direction, including ghost zones.
+    nphi:   int
+                    The number of angular points in the :math:`\\phi`
+                    direction, including ghost zones.
+    nghosts:    int
+                            The number of ghost zones at the end of
+                            each direction.
+    meshgrid:   tuple of 2d array
+                            The 2d array containing the meshgrid of
+                            (:math:`\\theta, \\phi`) angular points.
+    theta_1d:   1d array
+                            The 1d array of angular points
+                            along the :math:`\\theta` axis.
+    phi_1d: 1d array
+                            The 1d array of angular points
+                            along the :math:`\\phi` axis.
+    dtheta: float
+                            The angular step size in the :math:`\\theta`
+                            direction.
+    dphi:   float
+                    The angular step size inthe :math:`\\phi`
+                    direction.
+    npix_act:   int
+                            The total number of gridpoints on the sphere,
+                            excluding the ghost points.
+    meshgrid:
+                            Get the 2d angular grid.
 
     Methods
     -------
-    theta_1d :
-               Get the :math:`\\theta` axis.
-    phi_1d :
-               Get the :math:`\\phi` axis.
+    theta_1d:
+                            Get the :math:`\\theta` axis.
+    phi_1d:
+                            Get the :math:`\\phi` axis.
+
     """
 
-    def __init__(
-        self, nphi=80, ntheta=41, nphimax=124, nthetamax=66, nghosts=2
-    ):
+    def __init__(self, nphi=80, ntheta=41, nphimax=124, nthetamax=66, nghosts=2):
         # Number of gridpoints along phi direction including ghost points.
         self.nphi = nphi
         # Number of gridpoints along theta direction including ghost points.
         self.ntheta = ntheta
         # Total length of phi array used by ETK.
         self.nphimax = nphimax
         # Total length of theta array used by ETK.
@@ -129,71 +130,72 @@
         the coordinate index. The coordinate index
         ranges from (0, ntheta). The actual indices
         without the ghost and extra zones
         is (nghosts, ntheta-nghosts).
 
         Parameters
         -----------
-        theta_index : int or 1d array
-                      The theta coordinate index or axis.
+
+        theta_index:    int/ 1d array
+                                        The theta coordinate index or axis.
 
         Returns
         -------
-        theta_1d : float
-                   The coordinate(s) :math:`\\theta` on the sphere.
+
+        theta_1d:   float
+                                The coordinate(s) :math:`\\theta` on the sphere.
+
         """
 
         if not theta_index:
             theta_index = np.arange(self.nghosts, self.ntheta - self.nghosts)
 
-        return (
-            (theta_index - self.nghosts + 0.5)
-            * np.pi
-            / (self.ntheta - 2 * self.nghosts)
-        )
+        return (theta_index - self.nghosts + 0.5) * np.pi / (self.ntheta - 2 * self.nghosts)
 
     def phi_1d(self, phi_index=None):
         """Returns the coordinate value theta
         given the coordinate index. The coordinate
         index lies in (0, nphi). The actual indices
         without the ghost and extra zones
         is (nghosts, nphi-nghosts).
 
         Parameters
         -----------
-        phi_1d : int / 1d array
-                 The phi coordinate index or axis.
+
+        phi_1d: int / 1d array
+                                The phi coordinate index or axis.
 
         Returns
         -------
-        phi_1d : float or 1d array
-                 The coordinate(s) :math:`\\phi` on the sphere.
+
+        phi_1d: float or 1d array
+                                The coordinate(s) :math:`\\phi` on the sphere.
+
         """
 
         if not phi_index:
             phi_index = np.arange(self.nghosts, self.nphi - self.nghosts)
 
-        return (
-            (phi_index - self.nghosts)
-            * 2
-            * np.pi
-            / (self.nphi - 2 * self.nghosts)
-        )
+        return (phi_index - self.nghosts) * 2 * np.pi / (self.nphi - 2 * self.nghosts)
 
     @property
     def meshgrid(self):
         """The (:math:`\\theta, \\phi)`: coordinate meshes.
-        Excludes the ghost zones.
+                Excludes the ghost zones.
+
 
         Returns
         -------
-        theta : 2d array
-                The :math:`\\theta` coordinate matrix for vectorization.
-        phi : 2d array
-              The :math:`\\phi` coordinate matrix for vectorization.
+
+        theta:  2d array
+                        The :math:`\\theta` coordinate matrix for vectorization.
+
+        phi:    2d array
+                        The :math:`\\phi` coordinate matrix for vectorization.
+
         """
 
         theta, phi = np.meshgrid(self.theta_1d(), self.phi_1d())
 
         # theta = np.zeros((self.ntheta_act, self.nphi_act))
         # phi   = np.zeros((self.ntheta_act, self.nphi_act))
 
@@ -206,60 +208,61 @@
 
 
 class gl_grid:
     """A class to store the coordinate grid on a sphere.
 
     Attributes
     ----------
-    ntheta : int
-             The number of angular points in the :math:`\\theta`
-             direction, including ghost zones.
-    nphi : int
-           The number of angular points in the :math:`\\phi`
-           direction, including ghost zones.
-    nghosts : int
-              The number of ghost zones at the end of
-              each direction.
-    meshgrid : tuple of 2d array
-               The 2d array containing the meshgrid of
-               (:math:`\\theta, \\phi`) angular points.
-    theta_1d : 1d array
-               The 1d array of angular points
-               along the :math:`\\theta` axis.
-    phi_1d : 1d array
-             The 1d array of angular points
-             along the :math:`\\phi` axis.
-    dtheta : float
-             The angular step size in the :math:`\\theta`
-             direction.
-    dphi : float
-           The angular step size inthe :math:`\\phi`
-           direction.
-    npix_act : int
-               The total number of gridpoints on the sphere,
-               excluding the ghost points.
-    meshgrid :
-               Get the 2d angular grid.
+    ntheta: int
+                The number of angular points in the :math:`\\theta`
+                direction, including ghost zones.
+    nphi:   int
+            The number of angular points in the :math:`\\phi`
+            direction, including ghost zones.
+    nghosts:    int
+                The number of ghost zones at the end of
+                each direction.
+    meshgrid:   tuple of 2d array
+                The 2d array containing the meshgrid of
+                (:math:`\\theta, \\phi`) angular points.
+    theta_1d:   1d array
+                The 1d array of angular points
+                along the :math:`\\theta` axis.
+    phi_1d: 1d array
+                The 1d array of angular points
+                along the :math:`\\phi` axis.
+    dtheta: float
+                The angular step size in the :math:`\\theta`
+                direction.
+    dphi:   float
+            The angular step size inthe :math:`\\phi`
+            direction.
+    npix_act:   int
+                The total number of gridpoints on the sphere,
+                excluding the ghost points.
+    meshgrid:
+                Get the 2d angular grid.
 
     Methods
     -------
-    theta_1d :
-               Get the :math:`\\theta` axis.
-    phi_1d :
-             Get the :math:`\\phi` axis.
+    theta_1d:
+                Get the :math:`\\theta` axis.
+    phi_1d:
+                Get the :math:`\\phi` axis.
 
     Notes
     -----
+
     The total number of points on the sphere is assumed to be :math:`(L+1)^2`
 
     :math:`N_\theta = L+1`
 
     :math:`N_\phi = 2(L+1)`
 
-    This integrates out spherical harmonics of degree `L` exactly,
+    This integrates out spherical harmonics of degree L exactly,
     given a regular function on the sphere.
     """
 
     def __init__(self, nphi=None, ntheta=None, L=47, nghosts=2):
         # Number of gridpoints along phi direction including ghost points.
         self._nphi = nphi
         # Number of gridpoints along theta direction including ghost points.
@@ -291,17 +294,15 @@
                 raise ValueError("Please specify L or angular points!")
             else:
                 self.L = self.ntheta - 1
                 assert nphi % 2 == 0
 
         from scipy.special import roots_legendre
 
-        cpoints, self._weights, self._sum_of_weights = roots_legendre(
-            L + 1, mu=True
-        )
+        cpoints, self._weights, self._sum_of_weights = roots_legendre(L + 1, mu=True)
 
         # xpoints = (np.pi-np.arccos(cpoints))
         xpoints = np.arccos(cpoints[::-1])
         self._theta_1d = xpoints
 
         dphi = 2 * np.pi / self._nphi_act
 
@@ -404,53 +405,61 @@
     def theta_1d(self):
         """Returns the coordinate values theta given the coordinate index.
         The coordinate index ranges from (0, ntheta). The actual indices
         without the ghost and extra zones is (nghosts, ntheta-nghosts).
 
         Parameters
         -----------
-        theta_index : int/ 1d array
-                      The theta coordinate index or axis.
+
+        theta_index:    int/ 1d array
+                        The theta coordinate index or axis.
 
         Returns
         -------
-        theta_1d : float
-                   The coordinate(s) :math:`\\theta` on the sphere.
+
+        theta_1d:   float
+                    The coordinate(s) :math:`\\theta` on the sphere.
+
         """
 
         return self._theta_1d
 
     @property
     def phi_1d(self):
         """Returns the coordinate values phi given the coordinate index.
         The coordinate index lies in (0, nphi). The actual indices without
         the ghost and extra zones is (nghosts, nphi-nghosts).
 
         Parameters
         -----------
-        phi_1d : int / 1d array
-                 The phi coordinate index or axis.
+
+        phi_1d: int / 1d array
+                    The phi coordinate index or axis.
 
         Returns
         -------
-        phi_1d : float or 1d array
-                 The coordinate(s) :math:`\\phi` on the sphere.
+
+        phi_1d: float or 1d array
+                    The coordinate(s) :math:`\\phi` on the sphere.
+
         """
 
         return self._phi_1d
 
     @property
     def meshgrid(self):
         """The (:math:`\\theta, \\phi)`: coordinate meshes.
-        Excludes the ghost zones.
+            Excludes the ghost zones.
 
 
         Returns
         -------
-        theta : 2d array
+
+        theta:  2d array
                 The :math:`\\theta` coordinate matrix for vectorization.
 
-        phi : 2d array
-              The :math:`\\phi` coordinate matrix for vectorization.
+        phi:    2d array
+                The :math:`\\phi` coordinate matrix for vectorization.
+
         """
 
         return self._meshgrid
```

### Comparing `waveformtools-2023.6.3/waveformtools/integrate.py` & `waveformtools-2023.6.5/waveformtools/integrate.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,64 +9,63 @@
 from waveformtools.waveformtools import message
 
 ##################################################
 # Fixed frequency integration
 ##################################################
 
 
-def fixed_frequency_integrator(
-    udata_time, delta_t, utilde_conven=None, omega0=0, order=1, zero_mode=0
-):
+def fixed_frequency_integrator(udata_time, delta_t, utilde_conven=None, omega0=0, order=1, zero_mode=0):
     """Fixed frequency integrator as presented in Reisswig et. al.
 
 
     Parameters
     ----------
-    udata_time : 1d array
-                 The input data in time.
-    delta_t : float
-              The time stepping.
-
-    utilde_conven : 1d array, optional
-                    The conventional FFT of the samples udata_time.
-    omega0 : float, optional
-             The cutoff angular frequency in the integration.
-             Must be lower than the starting angular frequency
-             of the input waveform. All frequencies whose absolute
-             value is below this value will be neglected.
-             The default cutoff-value is 0.
-
-    order : int, optional
-            The number of times to integrate
-            the integrand in time. Defaults to 1.
-
-    zero_mode : float, optional
-                The zero mode amplitude of the FFT required.
-                Defaults to 0 i.e. the zero mode is removed.
+    udata_time:	1d array
+                            The input data in time.
+    delta_t:	float
+                            The time stepping.
+
+    utilde_conven:		1d array, optional
+                                            The conventional FFT of the samples udata_time.
+    omega0:	float, optional
+            The cutoff angular frequency in the integration.
+            Must be lower than the starting angular frequency
+            of the input waveform. All frequencies whose absolute
+            value is below this value will be neglected.
+            The default cutoff-value is 0.
+
+    order:		int, optional
+                The number of times to integrate
+                the integrand in time. Defaults to 1.
+
+    zero_mode:	float, optional
+                            The zero mode amplitude of the FFT required.
+                            Defaults to 0 i.e. the zero mode is removed.
 
     Returns
     -------
-    u_integ_n_time : 1d array
-                     The input waveform in time-space,
-                     integrated in frequency space using FFI.
 
-    u_integ_integ_n : 1d array
-                      The integrated u samples in Fourier space.
+    u_integ_n_time:	1d array
+                                            The input waveform in time-space, integrated in frequency space using FFI.
+
+    u_integ_integ_n:	1d array
+                                            The integrated u samples in Fourier space.
+
     """
 
     if not utilde_conven:
         # Compute the FFT of data
         from numpy.fft import ifft
 
         from waveformtools.transforms import compute_fft, unset_fft_conven
 
         # from waveformtools import taper
         # udata_x_re = taper(u_time.real, delta_t=delta_t)
         # udata_x_im = taper(u_time.imag, delta_t=delta_t)
-        # udata_x      = np.array(udata_x_re) + 1j * np.array(udata_x_im)
+        # udata_x	   = np.array(udata_x_re) + 1j * np.array(udata_x_im)
         # x_axis = udata_x_re.sample_times
         # udata_x = np.array(udata_x)
         freq_axis, utilde_conven = compute_fft(udata_time, delta_t)
 
         # Find the length of the input data.
         Nlen = len(udata_time)
 
@@ -127,18 +126,18 @@
 
 def TwoDIntegral(func, info, method="DH"):
     """Integrate a function over a sphere.
 
     Parameters
     ----------
     func : function
-           The function to be integrated
+            The function to be integrated
     NTheta, NPhi : int
-                   The number of grid points in the theta and phi directions.
-                   Note that NTheta must be even.
+             The number of grid points in the theta and phi directions.
+             Note that NTheta must be even.
     ht, hp : float
              The grid spacings.
     method : string
              The method to use for the integration. Options are DH (Driscoll Healy), SP (Simpson's), MP (Midpoint).
 
     Returns
     -------
@@ -172,19 +171,19 @@
     """Evaulate the 2D surface integral using the midpoint rule.
 
     Parameters
     ----------
     func : ndarray
            The data to be integrated
     info : surface_grid_info
-           An instance of the surface grid info class containing information about the grid.
+            An instance of the surface grid info class containing information about the grid.
     Returns
     -------
      integ : float
-             The function f integrated over the sphere.
+            The function f integrated over the sphere.
     """
 
     ht = info.dtheta
     hp = info.dphi
 
     theta_grid, _ = info.meshgrid
 
@@ -297,46 +296,31 @@
     assert NTheta % 2 == 0
     assert NPhi % 2 == 0
 
     Px = int(NTheta / 2)
     Py = int(NPhi / 2)
 
     # Around corners
-    integrand_sum += (
-        func[0, 0]
-        + func[NTheta - 1, 0]
-        + func[0, NPhi - 1]
-        + func[NTheta - 1, NPhi - 1]
-    )
+    integrand_sum += func[0, 0] + func[NTheta - 1, 0] + func[0, NPhi - 1] + func[NTheta - 1, NPhi - 1]
 
     # Arount edges
     for index_phi in range(1, Py):
-        integrand_sum += (
-            4 * func[0, 2 * index_phi - 1]
-            + 4 * func[NTheta - 1, 2 * index_phi - 1]
-        )
+        integrand_sum += 4 * func[0, 2 * index_phi - 1] + 4 * func[NTheta - 1, 2 * index_phi - 1]
 
     # for (iy = 1; iy <= py-1; iy++)
     for index_phi in range(1, Py - 1):
-        integrand_sum += (
-            2 * func[0, 2 * index_phi] + 2 * func[NTheta - 1, 2 * index_phi]
-        )
+        integrand_sum += 2 * func[0, 2 * index_phi] + 2 * func[NTheta - 1, 2 * index_phi]
 
     # for (ix = 1; ix <= px; ix++)
     for index_theta in range(1, Px):
-        integrand_sum += (
-            4 * func[2 * index_theta - 1, 0]
-            + 4 * func[2 * index_theta - 1, NPhi - 1]
-        )
+        integrand_sum += 4 * func[2 * index_theta - 1, 0] + 4 * func[2 * index_theta - 1, NPhi - 1]
 
     # for (ix = 1; ix <= px-1; ix++)
     for index_theta in range(1, Px - 1):
-        integrand_sum += (
-            2 * func[2 * index_theta, 0] + 2 * func[2 * index_theta, NPhi - 1]
-        )
+        integrand_sum += 2 * func[2 * index_theta, 0] + 2 * func[2 * index_theta, NPhi - 1]
 
     # In the Interiors
     # for (iy = 1; iy <= py; iy++)
     for index_phi in range(1, Py):
         # for (ix = 1; ix <= px; ix++)
         for index_theta in range(1, Px):
             integrand_sum += 16 * func[2 * index_theta - 1, 2 * index_phi - 1]
@@ -366,18 +350,18 @@
     """Evaulate the 2D surface integral using the Gauss-Legendre rule.
 
     Parameters
     ----------
     func : ndarray
            The data to be integrated
     info : surface_grid_info
-           An instance of the surface grid info class containing information about the grid.
+            An instance of the surface grid info class containing information about the grid.
     Returns
     -------
-    integ : float
+     integ : float
             The function f integrated over the sphere.
     """
 
     # NTheta = info.ntheta_act
     # NPhi  = info.nphi_act
 
     # NTheta, NPhi = func.shape
```

### Comparing `waveformtools-2023.6.3/waveformtools/legacy.py` & `waveformtools-2023.6.5/waveformtools/legacy.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,56 +65,50 @@
                                                     h. Append the match details to an array
                                                     [ waveform list, [ match score, shift, start_index, end_index]]
     2. Retun the match details for all the waveforms.
 
 
     Parameters
     ----------
-    waveforms:  list
+    waveforms:	list
                 A List of pairs [waveform A, waveform B].
 
     Notes
     -----
     Assumes that the sampling rate is the  same for each pair.
 
     Returns
     -------
-    match:  a list of dicts
+    match:	a list of dicts
             A list of dictionaries in the format
             {match score (float), shift (number), start_index, end_index}
     """
     # Iterate over (signal,template) pairs in waveforms
     for waveformdat in waveforms:
         # Carryout the match
         if not delt:
             try:
                 delt = waveformdat[0].delta_t
             except BaseException:
-                message(
-                    "Waveform is not a pycbc TimeSeries. Please provide the gridspacing delt"
-                )
+                message("Waveform is not a pycbc TimeSeries. Please provide the gridspacing delt")
                 sys.exit(0)
         # Match procedure
 
         # signaldat = lengtheq(waveformdat[0], waveformdat[1], delt)
 
         # waveform1 = signaldat[0]
         # waveform2 = signaldat[1]
-        waveform1, waveform2, _ = lengtheq(
-            waveformdat[0], waveformdat[1], delt, is_ts=True
-        )
+        waveform1, waveform2, _ = lengtheq(waveformdat[0], waveformdat[1], delt, is_ts=True)
 
         # alignedwvs = pycbc.waveform.utils.coalign_waveforms(signaldat,hpa)
         # Compute the match to calculate match and shift.
         # Note: The match function from pycbc returns the match of the
         # normalized templates
 
-        (match_score, shift) = pycbc.filter.matchedfilter.match(
-            waveform1, waveform2
-        )
+        (match_score, shift) = pycbc.filter.matchedfilter.match(waveform1, waveform2)
 
         message("Priliminary match", match_score, shift)
         # Shift the matched data against the template using the shift obtained
         # above
         waveform1 = roll(np.array(waveform1), int(shift))
         # waveform1 = shiftmatched(np.array(waveform1), int(shift), delt)
         # Compute the start and end of the non-zero signal
@@ -127,26 +121,22 @@
             message("Absolute startend not found. Fixing approximate startend")
         # Match procedure
 
         # signaldat = lengtheq(waveformdat[0], waveformdat[1], delt)
 
         # waveform1 = signaldat[0]
         # waveform2 = signaldat[1]
-        waveform1, waveform2, _ = lengtheq(
-            waveformdat[0], waveformdat[1], delt, is_ts=True
-        )
+        waveform1, waveform2, _ = lengtheq(waveformdat[0], waveformdat[1], delt, is_ts=True)
 
         # alignedwvs = pycbc.waveform.utils.coalign_waveforms(signaldat,hpa)
         # Compute the match to calculate match and shift.
         # Note: The match function from pycbc returns the match of the
         # normalized templates
 
-        (match_score, shift) = pycbc.filter.matchedfilter.match(
-            waveform1, waveform2
-        )
+        (match_score, shift) = pycbc.filter.matchedfilter.match(waveform1, waveform2)
 
         message("Priliminary match", match_score, shift)
         # Shift the matched data against the template using the shift obtained
         # above
         waveform1 = roll(np.array(waveform1), int(shift))
         # waveform1 = shiftmatched(np.array(waveform1), int(shift), delt)
         # Compute the start and end of the non-zero signal
@@ -156,62 +146,42 @@
         try:
             starti, endi = startend(waveform1)
         except BaseException:
             message("Absolute startend not found. Fixing approximate startend")
             starti, endi = apxstartend(waveform1)
             message("starti, endi")
 
-        message(
-            "The approximate start and end indices are",
-            starti,
-            endi,
-            "length",
-            endi - starti,
-        )
+        message("The approximate start and end indices are", starti, endi, "length", endi - starti)
         # Convert the non-zero portion of the signal and template to
         # time-series
         message("Converting shifted vectors to time series")
         signal = pycbc.types.timeseries.TimeSeries(
-            np.array(waveform1)[starti:endi]
-            / np.linalg.norm(np.array(waveform1)[starti:endi]),
-            delt,
+            np.array(waveform1)[starti:endi] / np.linalg.norm(np.array(waveform1)[starti:endi]), delt
         )
         template = pycbc.types.timeseries.TimeSeries(
-            np.array(waveform2)[starti:endi]
-            / np.linalg.norm(np.array(waveform2)[starti:endi]),
-            delt,
+            np.array(waveform2)[starti:endi] / np.linalg.norm(np.array(waveform2)[starti:endi]), delt
         )
         # Sanity check: The template and the signal must be of the same length
         # at this point in execution
         if len(signal) != len(template):
             message("Error\n")
-            message(
-                "Length of data, template after truncation are %d,%d"
-                % (len(signal), len(template))
-            )
+            message("Length of data, template after truncation are %d,%d" % (len(signal), len(template)))
             sys.exit(0)
         # Compute the match, shift again on the truncated data
         # message("length of data %d, aligned data %d, template %d",
         # (len(signaldat),len(alignedwvs[0]),len(alignedwvs[1])))
 
         try:
-            (match_score, shift) = pycbc.filter.matchedfilter.match(
-                signal, template
-            )
+            (match_score, shift) = pycbc.filter.matchedfilter.match(signal, template)
         except BaseException:
             message("Final match couldn't be found!")
             match_score = None
             shift = None
 
-        match = {
-            "Match score": match_score,
-            "Shift": shift,
-            "Start index": starti,
-            "End index": endi,
-        }
+        match = {"Match score": match_score, "Shift": shift, "Start index": starti, "End index": endi}
     return match
 
 
 def iscontinuous_old(timeaxis, delta_t=0):
     """Check if the data has discontinuities. This checks for repetitive time rows and jumps.
 
     Notes
@@ -220,19 +190,19 @@
 
     0: Continuous.
     1: Repetitive rows.
     2: Jumps in timeaxis.
 
     Parameters
     ----------
-    timeaxis:   list
+    timeaxis:	list
                 Input as a single 1d time axis
                 or a list of 1d arrays [time, data1, data2, ...].
                 All the data share the common time axis `time`
-    delta_t:    float
+    delta_t:	float
                 The time stepping.
     toldt : float
             The tolerance for error in checking.
             Defaluts to toldt=1e-3.
 
     Returns
     -------
@@ -271,17 +241,15 @@
             # Repetitive rows
             if timestamp < timeaxis[0] + epoch_index * delta_t:
                 discontinuity_type = 1
             # Missing rows
             elif epoch > timeaxis[0] + epoch_index + delta_t:
                 discontinuity_type = 2
             # Append [index location,correct timestamp
-            discontinuity_details.append(
-                [epoch_index, timeaxis[epoch_index], discontinuity_type]
-            )
+            discontinuity_details.append([epoch_index, timeaxis[epoch_index], discontinuity_type])
         epoch_index += 1
         # message("Progress: %f%%\r"%(epoch_index*100./len(timeaxis)))
 
     # Print the result
     # changed discontinuity_timestamps to discontinuity details May 5 2022
     if len(discontinuity_details) != 0:
         message("The data is discontinuous!")
@@ -292,25 +260,25 @@
 
 
 def cleandata_old(data, verbose=False):
     """Old version. Check the data (time,datar,datai) for repetetive rows and remove them.
 
     Parameters
     ----------
-    data : list
-           Input as a list of 1d arrays [time, data1, data2, ...].
-           All the data share the common time axis `time`
-    verbose : bool
-              A verbosity flag.
+    data:	list
+            Input as a list of 1d arrays [time, data1, data2, ...].
+            All the data share the common time axis `time`
+    verbose:   bool
+                A verbosity flag.
 
     Returns
     -------
-    cleaned_data : ndarray
-                   The cleaned data array with repetitive
-                   rows and gaps (if bridge=True) removed
+    cleaned_data:	ndarray
+                    The cleaned data array with repetitive
+                    rows and gaps (if bridge=True) removed
     """
 
     # Ensure data as numpy array
     data = np.array(data)
     if verbose == "yes":
         message("Data shape:", data.shape)
     # Set axis along which to remove
@@ -354,22 +322,16 @@
     while ii_index < ki_index - 1:
         # Repetition condition :if the successive time stamp is less than or
         # equal to the present, delete the row.
         if (time[ii_index + 1] - time[ii_index]) <= -0.1 * delta_t:
             # Set flag to 1 if repetition condition is met.
             rep_row_index = 1
             if verbose == "yes":
-                message(
-                    "found a repeating row at %d, time %f\n"
-                    % (ii_index + 1, time[ii_index + 1])
-                )
-                message(
-                    "timei: %f timef %f\n"
-                    % (time[ii_index], time[ii_index + 1])
-                )
+                message("found a repeating row at %d, time %f\n" % (ii_index + 1, time[ii_index + 1]))
+                message("timei: %f timef %f\n" % (time[ii_index], time[ii_index + 1]))
             # ci = ci+1
             # Delete the entire row
             time = np.delete(time, ii_index + 1)
             # data = np.delete(data,ii_index,1)
             # data = [np.delete(item,ii_index+1) for item in data]
             data = np.delete(data, ii_index + 1, axis)
             # Append the deleted index to the bookkeeping array
@@ -387,39 +349,39 @@
         else:
             message("No points removed\n")
         # message("++++++++++++++++++++++++++++++++++++++++++++++++++++++\n")
     # Return the "cleaned" data matrix
     cleaned_data = data
     # cleaned_data=[time]
     # for item in data:
-    #    cleaned_data.append(item)
+    # 	 cleaned_data.append(item)
     # cleaned_data.append(item for item in data)
     # Transpose the data back to original shape
     if shapes[0] > shapes[1]:
         cleaned_data = np.transpose(cleaned_data)
     return cleaned_data
 
 
 def cleandata(data, toldt=1e-3, bridge="no"):
     """Check the data (time,datar,datai) for repetetive rows and remove them.
 
     Parameters
     ----------
-    data:   list
+    data:	list
             Input as a list of 1d arrays [time, data1, data2, ...].
             All the data share the common time axis `time`
     toldt : float
             The tolerance for error in checking. defaluts to toldt=1e-3.
     bridge : bool
             A bridge flag to decide whether or not to interpolate and
             resample to fill in jump discontinuities.
 
     Returns
     -------
-    cleaned_data:   list
+    cleaned_data:	list
                     The cleaned data array with repetitive
                     rows and gaps (if bridge=True) removed.
     """
 
     # Check the data (time,datar,datai) for repetetive rows and remove them.
     # Ensure data as numpy array
     data = np.array(data)
@@ -466,31 +428,22 @@
     # rowcounter
     counter = 0
 
     # Iterate over rows
     while ii_index < ki_index - 1:
         # Repetition condition :if the successive time stamp is less than or
         # equal to the present, delete the row.
-        if (time[ii_index + 1] == time[ii_index]) or (
-            time[ii_index] - time[ii_index + 1]
-        ) >= toldt * delta_t:
+        if (time[ii_index + 1] == time[ii_index]) or (time[ii_index] - time[ii_index + 1]) >= toldt * delta_t:
             # if time[ii_index]-time[ii_index+1]<=0.01*delta_t:
-            #        message("Error!!",message_verbosity=0)
+            # 		 message("Error!!",message_verbosity=0)
             # Set flag to 1 if repetition condition is met.
             rep_row_index = 1
             counter += 1
-            message(
-                "found a repeating row at %d, time %f\n"
-                % (ii_index + 1, time[ii_index + 1]),
-                message_verbosity=3,
-            )
-            message(
-                "timei: %f timef %f\n" % (time[ii_index], time[ii_index + 1]),
-                message_verbosity=3,
-            )
+            message("found a repeating row at %d, time %f\n" % (ii_index + 1, time[ii_index + 1]), message_verbosity=3)
+            message("timei: %f timef %f\n" % (time[ii_index], time[ii_index + 1]), message_verbosity=3)
             # ci = ci+1
             # Delete the entire row
             time = np.delete(time, ii_index + 1, 0)
             # data = np.delete(data,ii_index,1)
             # data = [np.delete(item,ii_index+1) for item in data]
             data = np.delete(data, ii_index + 1, axis)
             # Append the deleted index to the bookkeeping array
@@ -510,18 +463,15 @@
     else:
         message("No points removed\n", message_verbosity=2)
         # message("++++++++++++++++++++++++++++++++++++++++++++++++++++++\n")
     # Return the "cleaned" data matrix
     cleaned_data = data
 
     if bridge and iscontinuous(cleaned_data)[-1] >= 2:
-        message(
-            "The data will be interpolated to bridge the gaps",
-            message_verbosity=2,
-        )
+        message("The data will be interpolated to bridge the gaps", message_verbosity=2)
 
         # from scipy import interpolate
 
         # Interpolate the data to fill in the discontinuities
         t_final = time[-1]
         t_initial = time[0]
 
@@ -545,15 +495,15 @@
 
         cleaned_data = np.array(interp_data)
         message("The data has been interpolated", message_verbosity=2)
     message("Cleaned!", message_verbosity=2)
 
     # cleaned_data=[time]
     # for item in data:
-    #    cleaned_data.append(item)
+    # 	 cleaned_data.append(item)
     # cleaned_data.append(item for item in data)
     # Transpose the data back to original shape
 
     if axis > 0:
         if shapes[0] > shapes[1]:
             cleaned_data = np.transpose(cleaned_data)
     return cleaned_data
@@ -568,25 +518,25 @@
 
     0: Continuous.
     1: Repetitive rows.
     2: Jumps in timeaxis.
 
     Parameters
     ----------
-    data:   list
+    data:	list
             Input as a list of 1d arrays [time, data1, data2, ...].
             All the data share the common time axis `time`
-    delta_t:    float
+    delta_t:	float
                 The time stepping.
     toldt : float
             The tolerance for error in checking. defaluts to toldt=1e-3.
 
     Returns
     -------
-    discontinuity_details:  a list.
+    discontinuity_details:	a list.
                             It contains:
                                 1. A list. details of discontinuity.
                                     index location of original array,
                                     the corresponding discinbtinuity type.
                                 2. A float. the global discontinuity type.
     """
 
@@ -608,15 +558,15 @@
         message("The time axis is :%s" % timeaxis, message_verbosity=3)
     else:
         timeaxis = data
     message("shape of data:", (data.shape), message_verbosity=3)
 
     # If data array is supplied, assign first column as timeaxis
     # if np.array(timeaxis).ndim>1:
-    #        timeaxis=np.array([item[0] for item in timeaxis])
+    # 		 timeaxis=np.array([item[0] for item in timeaxis])
     # message('Timeaxis`,timeaxis,message_verbosity=3)
     # Check data for continuity.
     # If delta_t is not supplied
 
     if delta_t == 0:
         # delta_t = statistics.mode(np.diff(timeaxis))
         import scipy.stats.mode as stat_mode
@@ -664,47 +614,38 @@
             epoch_index = index
             # Check for type of discontinuity
             # Repetitive rows
             if (original_timestamp == recentered_timestamp) or (
                 recentered_timestamp - original_timestamp
             ) >= toldt * delta_t:
                 # if recentered_timestamp-original_timestamp<=0.01*delta_t:
-                #        message("Error!!",message_verbosity=0)
+                # 		 message("Error!!",message_verbosity=0)
                 repetition = 1
                 discont_type = repetition
                 message(
-                    "Repetitive rows found at index: %d,timestamp: %f"
-                    % (index, original_timestamp),
+                    "Repetitive rows found at index: %d,timestamp: %f" % (index, original_timestamp),
                     message_verbosity=3,
                 )
                 message(
-                    "Repetition at timestamp original: %f correct %f\n"
-                    % (original_timestamp, recentered_timestamp),
+                    "Repetition at timestamp original: %f correct %f\n" % (original_timestamp, recentered_timestamp),
                     message_verbosity=3,
                 )
                 repetition_counter += 1
             # Missing rows
-            if (original_timestamp - recentered_timestamp) >= (
-                1.0 + toldt
-            ) * delta_t:
+            if (original_timestamp - recentered_timestamp) >= (1.0 + toldt) * delta_t:
                 discont = 2
                 discont_type = discont
                 message(
-                    "Jump discountinuity in data found at index:%d,timestamp:%f"
-                    % (index, original_timestamp),
+                    "Jump discountinuity in data found at index:%d,timestamp:%f" % (index, original_timestamp),
                     message_verbosity=2,
                 )
                 message("delta_t=%f" % delta_t, message_verbosity=1)
                 message(
                     "Jump at timestamp original: %f correct %f\n Dt = %f"
-                    % (
-                        original_timestamp,
-                        recentered_timestamp,
-                        (original_timestamp - recentered_timestamp) / delta_t,
-                    ),
+                    % (original_timestamp, recentered_timestamp, (original_timestamp - recentered_timestamp) / delta_t),
                     message_verbosity=1,
                 )
                 discont_counter += 1
             # message("timei: %f timef %f\n"%(timeaxis[index-1],timeaxis[index]),message_verbosity=3)
 
             # discont_type=repetition+discont
             discont_type_details.append([index, discont_type])
@@ -716,29 +657,19 @@
     # discont_type=(repetition+discont)
     # Print the result
     if discont_type:
         message("The data is not clean!", message_verbosity=1)
         global_discont_type = repetition + discont
         message("Discontinuity type:", global_discont_type, message_verbosity=1)
         if global_discont_type == 1:
-            message(
-                "The data has repetitive rows at %d locations"
-                % repetition_counter,
-                message_verbosity=1,
-            )
+            message("The data has repetitive rows at %d locations" % repetition_counter, message_verbosity=1)
         elif global_discont_type == 2:
-            message(
-                "The data has %d discontinuities" % discont_counter,
-                message_verbosity=1,
-            )
+            message("The data has %d discontinuities" % discont_counter, message_verbosity=1)
         else:
-            message(
-                "The data has repetitive rows and is discontinious",
-                message_verbosity=1,
-            )
+            message("The data has repetitive rows and is discontinious", message_verbosity=1)
 
         discontinuity_details = [discont_type_details, global_discont_type]
     else:
         message("Data is continuous", message_verbosity=2)
         discontinuity_details = [[0, 0], 0]
     # Return the details of discontinuity
 
@@ -746,30 +677,30 @@
 
 
 def remove_repeated_rows(data, delta_t, toldt=1e-3):
     """Remove repeated rows in the data
 
     Parameters
     ----------
-    data : ndarray
-           Data array where the first axis refers to different
-           columns of data. The zeroth column is time axis.
-           The second axis refers to entries at different time
-           steps.
+    data: ndarray
+              Data array where the first axis refers to different
+              columns of data. The zeroth column is time axis.
+              The second axis refers to entries at different time
+              steps.
 
-    delta_t : float
-              The tim stepping.
+    delta_t: float
+                     The tim stepping.
     toldt : float
-            The tolerance for error in checking. defaluts to toldt=1e-3.
+                    The tolerance for error in checking. defaluts to toldt=1e-3.
 
     Returns
     -------
-    cleaned_data : list
-                   The cleaned data array with repetitive
-                   rows removed.
+    cleaned_data:	list
+                                                                    The cleaned data array with repetitive
+                                                                    rows removed.
 
     """
     message("Checking data for repetative rows...\n", message_verbosity=2)
 
     time = data[0]
 
     # Index of ros to delete
@@ -789,31 +720,22 @@
     # rowcounter
     counter = 0
 
     # Iterate over rows
     while ii_index < ki_index - 1:
         # Repetition condition :if the successive time stamp is less than or
         # equal to the present, delete the row.
-        if (time[ii_index + 1] == time[ii_index]) or (
-            time[ii_index] - time[ii_index + 1]
-        ) >= toldt * delta_t:
+        if (time[ii_index + 1] == time[ii_index]) or (time[ii_index] - time[ii_index + 1]) >= toldt * delta_t:
             # if time[ii_index]-time[ii_index+1]<=0.01*delta_t:
-            #        message("Error!!",message_verbosity=0)
+            # 		 message("Error!!",message_verbosity=0)
             # Set flag to 1 if repetition condition is met.
             rep_row_index = 1
             counter += 1
-            message(
-                "found a repeating row at %d, time %f\n"
-                % (ii_index + 1, time[ii_index + 1]),
-                message_verbosity=3,
-            )
-            message(
-                "timei: %f timef %f\n" % (time[ii_index], time[ii_index + 1]),
-                message_verbosity=3,
-            )
+            message("found a repeating row at %d, time %f\n" % (ii_index + 1, time[ii_index + 1]), message_verbosity=3)
+            message("timei: %f timef %f\n" % (time[ii_index], time[ii_index + 1]), message_verbosity=3)
             # ci = ci+1
             # Delete the entire row
             time = np.delete(time, ii_index + 1, 0)
             # data = np.delete(data,ii_index,1)
             # data = [np.delete(item,ii_index+1) for item in data]
             data = np.delete(data, ii_index + 1, axis)
             # Append the deleted index to the bookkeeping array
```

### Comparing `waveformtools-2023.6.3/waveformtools/spherical.py` & `waveformtools-2023.6.5/waveformtools/spherical.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,52 +3,58 @@
 ##################################
 # Imports
 #################################
 
 import numpy as np
 
 
-def decompose_in_SWSHs(
-    waveform, gridinfo, spin_weight=-2, ell_max=8, emm_list="all"
-):
+def decompose_in_SWSHs(waveform, gridinfo, spin_weight=-2, ell_max=8, emm_list="all"):
     """Decompose a given function on a sphere in Spin Weighted Spherical Harmonics
 
     Parameters
     ----------
-    waveform : list
-               A list that contains as its items the waveform
-               defined on the sphere as an array of shape
-               [ntheta, nphi]. Each item in the list may denote
-               an instant of time or frequency.
-    spin_weight : int, optional
-                  The spin weight of the waveform.
-                  It defaults to -2 for a gravitational waveform.
-    ell_max : int, optional
-              The maximum value of the :math:`\\ell'
-              polar quantum number. Defaults to 6=8.
-    gridinfo : class instance
-               The class instance that contains
-               the properties of the spherical grid.
+
+    waveform:		list
+                    A list that contains as its items the waveform
+                    defined on the sphere as an array of shape
+                    [ntheta, nphi]. Each item in the list may denote
+                    an instant of time or frequency.
+
+    spin_weight:	 int, optional
+                    The spin weight of the waveform.
+                    It defaults to -2 for a gravitational waveform.
+
+    ell_max:	int, optional
+                The maximum value of the :math:`\\ell'
+                polar quantum number. Defaults to 6=8.
+
+    gridinfo:		class instance
+                    The class instance that contains
+                    the properties of the spherical grid.
+
 
     Returns
     -------
-    SWSH_coeffs : list
-                  The SWSH coefficients of the waveform.
-                  It may be a list composed of a single
-                  floating point number or a 1d array
-                  (denoting time or frequency dimension).
-                  The waveform can have angular as well
-                  as time dimentions. The nesting order
-                  will be that, given the list
-                  `non_boosted_waveform', each
-                  item refers to a one dimensional array in
-                  time/ frequency of SWSH coefficients.
+
+    SWSH_coeffs:	list
+                    The SWSH coefficients of the waveform.
+                    It may be a list composed of a single
+                    floating point number or a 1d array
+                    (denoting time or frequency dimension).
+                    The waveform can have angular as well
+                    as time dimentions. The nesting order
+                    will be that, given the list
+                    `non_boosted_waveform', each
+                    item refers to a one dimensional array in
+                    time/ frequency of SWSH coefficients.
+
 
     Notes
     -----
+
     Assumes that the sphere on which this decomposition is carried out is so far out
     that the coordinate system is spherical polar and the poper area is the
     same as its co-ordinate area.
 
     """
 
     # Find out if the unboosted waveform is a single number or defined on a spherical grid.
@@ -105,58 +111,61 @@
             for emm_index in range(len(emm_list)):
                 # Decompose into seperate m modes.
 
                 # m value.
                 emm_val = int(emm_list[emm_index])
 
                 # Spin weighted spherical harmonic function at (theta, phi)
-                Ybasis_fun = Yslm_vec(
-                    spin_weight, ell_index, emm_val, theta, phi
-                )
+                Ybasis_fun = Yslm_vec(spin_weight, ell_index, emm_val, theta, phi)
 
                 # Integrate to obtain the multipole of order l.
 
                 # Integration for real and imaginary parts of the data separately.
                 # Integrate the function
 
                 # Using quad
-                multipole_emm = quad_on_sphere(
-                    integrand_ij * Ybasis_fun * darea, gridinfo
-                )
-                # multipole_emm  =   np.sum(integrand_ij * Ybasis_fun * darea)
+                multipole_emm = quad_on_sphere(integrand_ij * Ybasis_fun * darea, gridinfo)
+                # multipole_emm	 =	 np.sum(integrand_ij * Ybasis_fun * darea)
 
                 multipoles_ell.update({emm_val: multipole_emm})
             multipoles_all.update({ell_index: multipoles_ell})
 
         # Return the computed multipole.
         return multipoles_all
 
 
 def quad_on_sphere(integrand, gridinfo, kind="third"):
     """Integrate on a sphere using the scipy.quad method
 
     Parameters
     ----------
-    integrand : 2d array
-                The two dimensional integrand array defined on the sphere.
-    info : class instance
-           The class instance that contains the properties of the spherical grid.
-    kind : str
-           The interpolation order to use in integration.
 
+    integrand:		2d array
+                                    The two dimensional integrand array defined on the sphere.
+
+    info:		class instance
+                            The class instance that contains the properties of the spherical grid.
+
+    kind:		str
+                            The interpolation order to use in integration.
     Returns
     -------
+
     final_integral : float
-                     The given integrand integrated over the sphere.
-    final_errs : float
-                 The accumulated errors.
+                              The given integrand integrated over the sphere.
+
+    final_errs:	float
+                                    The accumulated errors.
 
     Notes
     -----
+
     Assumes that the sphere is a unit round sphere.
+
+
     """
 
     # Step 0: Get the grid properties
 
     # Compute the meshgrid for theta and phi.
     theta_1d = gridinfo.theta_1d
     # theta
@@ -174,31 +183,27 @@
         # Interpolate the integrand.
 
         integrand_phi = integrand[:, phi_index]
 
         integrand_phi_interp_func = interp1d(theta_1d, integrand_phi, kind=kind)
 
         # Integrate on the phi plane
-        integral_phi_vals, integral_phi_errs = quad(
-            integrand_phi_interp_func, 0, np.pi
-        )
+        integral_phi_vals, integral_phi_errs = quad(integrand_phi_interp_func, 0, np.pi)
 
         theta_first_integral_vals.append(integral_phi_vals)
         theta_first_integral_errs.append(integral_phi_errs)
 
     # Step 2: integrate along the phi direction
 
     # Interpolate the integrand.
 
     integrand_theta = theta_first_integral_vals
 
     integrand_theta_interp_func = interp1d(phi_1d, integrand_theta, kind=kind)
 
     # Integrate on the theta plane
-    final_integral, semi_final_errs = quad(
-        integrand_theta_interp_func, 0, 2 * np.pi
-    )
+    final_integral, semi_final_errs = quad(integrand_theta_interp_func, 0, 2 * np.pi)
 
     # Get final errors
     final_errs = semi_final_errs + np.sum(np.array(theta_first_integral_errs))
 
     return final_integral, final_errs
```

### Comparing `waveformtools-2023.6.3/waveformtools/transforms.py` & `waveformtools-2023.6.5/waveformtools/transforms.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,110 +9,121 @@
 
 # @njit(parallel=True)
 def compute_fft(udata_x, delta_x):
     """Find the FFT of the samples in time-space, and return with the frequencies.
 
     Parameters
     ----------
-    udata_x : 1d array
-              The samples in time-space.
-    delta_x : float
-              The stepping delta_x
+
+    udata_x:	1d array
+                                                    The samples in time-space.
+
+    delta_x:	float
+                                                    The stepping delta_x
 
     Returns
     -------
-    freqs : 1d array
-            The frequency axis, shifted approriately.
-    utilde : 1d array
-             The samples in frequency space, with conventions applied.
+
+    freqs:	1d array
+                                    The frequency axis, shifted approriately.
+    utilde:	1d array
+                                                    The samples in frequency space, with conventions applied.
+
     """
 
     # import necessary libraries.
     from numpy.fft import fft
 
     # FFT
     utilde_orig = fft(udata_x)
 
     # Apply conventions.
     utilde = set_fft_conven(utilde_orig)
 
     # Get frequency axes.
     Nlen = len(utilde)
     # message(Nlen)
-    # Naxis         = np.arange(Nlen)
-    # freq_orig     = fftfreq(Nlen)
-    # freq_axis     = fftshift(freq_orig)*Nlen
-    # delta_x        = xdata[1] - xdata[0]
+    # Naxis			= np.arange(Nlen)
+    # freq_orig		= fftfreq(Nlen)
+    # freq_axis		= fftshift(freq_orig)*Nlen
+    # delta_x		 = xdata[1] - xdata[0]
 
-    # Naxis          = np.arange(Nlen)
+    # Naxis			 = np.arange(Nlen)
     freq_axis = np.linspace(-0.5 / delta_x, 0.5 / delta_x, Nlen)
 
     return freq_axis, utilde
 
 
 # @njit(parallel=True)
 def compute_ifft(utilde, delta_f):
     """Find the inverse FFT of the samples in frequency-space, and return with the time axis.
 
     Parameters
     ----------
-    utilde : 1d array
-             The samples in frequency-space.
-    delta_f : float
-              The frequency stepping
+
+    utilde	:	1d array
+                                                    The samples in frequency-space.
+
+    delta_f:	float
+                                                    The frequency stepping
 
     Returns
     -------
-    time_axis : 1d array
-                The time axis.
-    udata_time : 1d array
-                 The samples in time domain.
+
+    time_axis:	1d array
+                                                    The time axis.
+
+    udata_time:	1d array
+                                                                    The samples in time domain.
+
     """
 
     # import necessary libraries.
     from numpy.fft import ifft
 
     # FFT
     utilde_orig = unset_fft_conven(utilde)
 
     # Inverse transform
     udata_time = ifft(utilde_orig)
 
     # Get frequency axes.
     Nlen = len(udata_time)
     # message(Nlen)
-    # Naxis         = np.arange(Nlen)
-    # freq_orig     = fftfreq(Nlen)
-    # freq_axis     = fftshift(freq_orig)*Nlen
-    # delta_x        = xdata[1] - xdata[0]
+    # Naxis			= np.arange(Nlen)
+    # freq_orig		= fftfreq(Nlen)
+    # freq_axis		= fftshift(freq_orig)*Nlen
+    # delta_x		 = xdata[1] - xdata[0]
 
-    # Naxis          = np.arange(Nlen)
+    # Naxis			 = np.arange(Nlen)
     delta_t = 1.0 / (delta_f * Nlen)
-    # Dt                = Nlen * delta_f/2
+    # Dt				= Nlen * delta_f/2
 
     time_axis = np.linspace(0, delta_t * Nlen, Nlen)
 
     return time_axis, udata_time
 
 
 # @njit(parallel=True)
 def set_fft_conven(utilde_orig):
     """Make a numppy fft consistent with the chosen conventions.
                     This takes care of the zero mode factor and array position.
                     Also, it shifts the negative frequencies using numpy's fftshift.
 
     Parameters
     ----------
-    utilde_orig : 1d array
-                  The result of a numpy fft.
+
+    utilde_orig:	1d array
+                                                                    The result of a numpy fft.
 
     Returns
     -------
-    utilde_conven : 1d array
-                    The fft with set conventions.
+
+    utilde_conven:	1d array
+                                                                    The fft with set conventions.
     """
 
     # Multiply by 2, take conjugate.
     utilde_conven = 2 * np.conj(utilde_orig) / len(utilde_orig)
     # Restore the zero mode.
     utilde_conven[0] = utilde_conven[0] / 2
     # Shift the frequency axis.
@@ -120,26 +131,27 @@
 
     return utilde_conven
 
 
 # @njit(parallel=True)
 def unset_fft_conven(utilde_conven):
     """Make an actual conventional fft consistent with numpy's conventions.
-    The inverse of set_conv.
+                    The inverse of set_conv.
 
 
     Parameters
     ----------
-    utilde_conven : 1d array
-                    The conventional fft data vector.
+
+    utilde_conven:	1d array
+                                                                    The conventional fft data vector.
 
     Returns
     -------
-    utilde_np : 1darray
-                The fft in numpy convention
+
+    utilde_np
     """
 
     utilde_np = np.fft.ifftshift(utilde_conven)
 
     utilde_np = len(utilde_np) * np.conj(utilde_np) / 2
     # message(utilde_original[0])
     utilde_np[0] *= 2
@@ -149,33 +161,35 @@
 
 
 def Yslm(spin_weight, ell, emm, theta, phi):
     """Spin-weighted spherical harmonics fast evaluation.
 
     Parameters
     ----------
-    spin_weight : int
-                  The Spin weight.
-    ell : int
-          The mode number :math:`\\ell'.
-    emm : int
-          The azimuthal mode number :math:`m'.
+
+    spin_weight :	int
+                                    The Spin weight.
+    ell :	int
+                    The mode number :math:`\\ell'.
+    emm :	int
+                    The azimuthal mode number :math:`m'.
     theta : float
-            The polar angle  :math:`\\theta` in radians,
-    phi : float
-          The aximuthal angle :math:`\\phi' in radians.
+                    The polar angle  :math:`\\theta` in radians,
+    phi :	float
+                    The aximuthal angle :math:`\\phi' in radians.
 
     Returns
     --------
-    Yslm : float
-           The value of Yslm at :math:`\\theta, phi'.
+    Yslm :	float
+                    The value of Yslm at :math:`\\theta, phi'.
+
+            Note
+            ----
+            This is accurate upto 14 decimals for L upto 25.
 
-    Notes
-    -----
-    This is accurate upto 14 decimals for L upto 25.
     """
     import sympy as sp
 
     # theta, phi = sp.symbols('theta phi')
 
     fact = np.math.factorial
     # fact = sp.factorial
@@ -186,74 +200,66 @@
         factor = (-1) ** ell
         theta = np.pi - theta
         phi += np.pi
 
     abs_spin_weight = abs(spin_weight)
 
     for aar in range(ell - abs_spin_weight + 1):
-        if (aar + abs_spin_weight - emm) < 0 or (
-            ell - aar - abs_spin_weight
-        ) < 0:
+        if (aar + abs_spin_weight - emm) < 0 or (ell - aar - abs_spin_weight) < 0:
             message(f"Skippin r {aar}", message_verbosity=3)
             continue
         else:
             Sum += (
                 sp.binomial(ell - abs_spin_weight, aar)
-                * sp.binomial(
-                    ell + abs_spin_weight, aar + abs_spin_weight - emm
-                )
+                * sp.binomial(ell + abs_spin_weight, aar + abs_spin_weight - emm)
                 * np.power((-1), (ell - aar - abs_spin_weight))
                 * np.exp(1j * emm * phi)
                 / np.power(np.tan(theta / 2), (2 * aar + abs_spin_weight - emm))
             )
 
     Sum = complex(Sum)
     Yslm = (-1) ** emm * (
         np.sqrt(
             fact(ell + emm)
             * fact(ell - emm)
             * (2 * ell + 1)
-            / (
-                4
-                * np.pi
-                * fact(ell + abs_spin_weight)
-                * fact(ell - abs_spin_weight)
-            )
+            / (4 * np.pi * fact(ell + abs_spin_weight) * fact(ell - abs_spin_weight))
         )
         * np.sin(theta / 2) ** (2 * ell)
         * Sum
     )
 
     return factor * Yslm
 
 
 def Yslm_vec(spin_weight, ell, emm, theta_grid, phi_grid):
     """Spin-weighted spherical harmonics fast evaluations on numpy arrays for vectorized evaluations.
 
-    Parameters
-    ----------
-    spin_weight : int
-                  The Spin weight.
-    ell : int
-          The mode number :math:`\\ell'.
-    emm : int
-          The azimuthal mode number :math:`m'.
+    Inputs
+    -----------
+
+    spin_weight :	int
+                                    The Spin weight.
+    ell :	int
+                    The mode number :math:`\\ell'.
+    emm :	int
+                    The azimuthal mode number :math:`m'.
     theta : float
-            The polar angle  :math:`\\theta` in radians,
-    phi : float
-          The aximuthal angle :math:`\\phi' in radians.
+                    The polar angle  :math:`\\theta` in radians,
+    phi :	float
+                    The aximuthal angle :math:`\\phi' in radians.
 
     Returns
-    -------
-    Yslm : float
-           The value of Yslm at :math:`\\theta, phi'.
+    --------
+    Yslm :	float
+                    The value of Yslm at :math:`\\theta, phi'.
 
-    Notes
-    -----
-    This is accurate upto 14 decimals for `L` upto 25.
+            Note
+            ----
+            This is accurate upto 14 decimals for L upto 25.
     """
 
     from math import comb
 
     fact = np.math.factorial
 
     theta_grid = np.array(theta_grid)
@@ -268,115 +274,106 @@
         phi_grid += np.pi
 
     abs_spin_weight = abs(spin_weight)
 
     for aar in range(0, ell - abs_spin_weight + 1):
         subterm = 0
 
-        if (aar + abs_spin_weight - emm) < 0 or (
-            ell - aar - abs_spin_weight
-        ) < 0:
+        if (aar + abs_spin_weight - emm) < 0 or (ell - aar - abs_spin_weight) < 0:
             message(f"Skipping r {aar}", message_verbosity=3)
             continue
         else:
             term1 = comb(ell - abs_spin_weight, aar)
             term2 = comb(ell + abs_spin_weight, aar + abs_spin_weight - emm)
             term3 = np.power(float(-1), (ell - aar - abs_spin_weight))
             term4 = np.exp(1j * emm * phi_grid)
-            term5 = np.power(
-                np.tan(theta_grid / 2), (-2 * aar - abs_spin_weight + emm)
-            )
+            term5 = np.power(np.tan(theta_grid / 2), (-2 * aar - abs_spin_weight + emm))
             subterm = term1 * term2 * term3 * term4 * term5
 
             Sum += subterm
 
     Yslmv = float(-1) ** emm * (
         np.sqrt(
             fact(ell + emm)
             * fact(ell - emm)
             * (2 * ell + 1)
-            / (
-                4
-                * np.pi
-                * fact(ell + abs_spin_weight)
-                * fact(ell - abs_spin_weight)
-            )
+            / (4 * np.pi * fact(ell + abs_spin_weight) * fact(ell - abs_spin_weight))
         )
         * np.sin(theta_grid / 2) ** (2 * ell)
         * Sum
     )
 
     return factor * Yslmv
 
 
 def Yslm_prec(spin_weight, ell, emm, theta, phi, prec=24):
     """Spin-weighted spherical harmonics function with precise computations.
                             Uses a symbolic method evaluated at the degree of precision requested
                             by the user.
     Parameters
     ----------
-    spin_weight : int
-                  The Spin weight.
-    ell : int
-          The mode number :math:`\\ell'.
-    emm : int
-          The azimuthal mode number :math:`m'.
+
+    spin_weight :	int
+                                    The Spin weight.
+    ell :	int
+                    The mode number :math:`\\ell'.
+    emm :	int
+                    The azimuthal mode number :math:`m'.
     theta : float
-            The polar angle  :math:`\\theta` in radians,
-    phi : float
-          The aximuthal angle :math:`\\phi' in radians.
+                    The polar angle  :math:`\\theta` in radians,
+    phi :	float
+                    The aximuthal angle :math:`\\phi' in radians.
     pres : int, optional
-           The precision i.e. number of digits to compute
-           upto. Default value is 16.
-
+               The precision i.e. number of digits to compute
+               upto. Default value is 16.
     Returns
     --------
-    Yslm : float
-           The value of Yslm at :math:`\\theta, phi'.
+    Yslm :	float
+                    The value of Yslm at :math:`\\theta, phi'.
+
     """
     import sympy as sp
 
     # tv, pv = theta, phi
     th, ph = sp.symbols("theta phi")
 
     Yslm_expr = Yslm_prec_sym(spin_weight, ell, emm)
 
     if spin_weight < 0:
         theta = np.pi - theta
         phi = np.pi + phi
 
-    return Yslm_expr.evalf(
-        prec, subs={th: sp.Float(f"{theta}"), ph: sp.Float(f"{phi}")}
-    )
+    return Yslm_expr.evalf(prec, subs={th: sp.Float(f"{theta}"), ph: sp.Float(f"{phi}")})
 
 
 def Yslm_prec_sym(spin_weight, ell, emm):
     """Spin-weighted spherical harmonics precise, symbolic computation for deferred evaluations.
        Is dependent on variables th: theta and ph:phi.
-
     Parameters
     ----------
-    spin_weight : int
-                  The Spin weight.
-    ell : int
-          The mode number :math:`\\ell'.
-    emm : int
-          The azimuthal mode number :math:`m'.
+
+    spin_weight :	int
+                                    The Spin weight.
+    ell :	int
+                    The mode number :math:`\\ell'.
+    emm :	int
+                    The azimuthal mode number :math:`m'.
     theta : float
-            The polar angle  :math:`\\theta` in radians,
-    phi : float
-          The aximuthal angle :math:`\\phi' in radians.
+                    The polar angle  :math:`\\theta` in radians,
+    phi :	float
+                    The aximuthal angle :math:`\\phi' in radians.
     pres : int, optional
-           The precision i.e. number of digits to compute
-           upto. Default value is 16.
+               The precision i.e. number of digits to compute
+               upto. Default value is 16.
 
     Returns
     --------
-    Yslm : sym
-           The value of Yslm at :math:`\\theta, phi'.
+    Yslm :	sym
+                    The value of Yslm at :math:`\\theta, phi'.
+
     """
     import sympy as sp
 
     th, ph = sp.symbols("theta phi")
 
     fact = sp.factorial
     Sum = 0
@@ -385,17 +382,15 @@
     # To get negative spin weight SWSH
     # in terms of positive spin weight
     factor = 1
     if spin_weight < 0:
         factor = sp.Pow(-1, ell)
 
     for aar in range(ell - abs_spin_weight + 1):
-        if (aar + abs_spin_weight - emm) < 0 or (
-            ell - aar - abs_spin_weight
-        ) < 0:
+        if (aar + abs_spin_weight - emm) < 0 or (ell - aar - abs_spin_weight) < 0:
             # message('Continuing')
             continue
         else:
             # message('r, l, s, m', r, l, s, m)
             # a1 = sp.binomial(ell - spin_weight, aar)
             # message(a1)
             # a2 = sp.binomial(ell + spin_weight, aar + spin_weight - emm)
@@ -403,33 +398,26 @@
             # a3 = sp.exp(1j * emm * phi)
             # message(a3)
             # a4 = sp.tan(theta / 2)
             # message(a4)
 
             Sum += (
                 sp.binomial(ell - abs_spin_weight, aar)
-                * sp.binomial(
-                    ell + abs_spin_weight, aar + abs_spin_weight - emm
-                )
+                * sp.binomial(ell + abs_spin_weight, aar + abs_spin_weight - emm)
                 * sp.Pow((-1), (ell - aar - abs_spin_weight))
                 * sp.exp(sp.I * emm * ph)
                 * sp.Pow(sp.cot(th / 2), (2 * aar + abs_spin_weight - emm))
             )
 
     Yslm_expr = sp.Pow(-1, emm) * (
         sp.sqrt(
             fact(ell + emm)
             * fact(ell - emm)
             * (2 * ell + 1)
-            / (
-                4
-                * sp.pi
-                * fact(ell + abs_spin_weight)
-                * fact(ell - abs_spin_weight)
-            )
+            / (4 * sp.pi * fact(ell + abs_spin_weight) * fact(ell - abs_spin_weight))
         )
         * sp.Pow(sp.sin(th / 2), (2 * ell))
         * Sum
     )
 
     Yslm_expr = factor * sp.simplify(Yslm_expr)
 
@@ -439,25 +427,25 @@
 def rotate_polarizations(wf, alpha):
     """Rotate the polarizations of the time domain
     observer waveform by :math:`2\alpha`
 
     Parameters
     ----------
     wf : 1d array
-         The complex observer waveform to rotate.
+             The complex observer waveform to rotate.
     alpha : float
-            The coordinate angle to rotate the polarizations
-            in radians. Note that the polarizarions would
-            rotate by :math:`2 \alpha` on a cordinate
-            rotation of :math:`\alpha`.
+                    The coordinate angle to rotate the polarizations
+                    in radians. Note that the polarizarions would
+                    rotate by :math:`2 \alpha` on a cordinate
+                    rotation of :math:`\alpha`.
 
     Returns
     -------
     rot_wf : 1d array
-             The rotated waveform.
+                     The rotated waveform.
     """
 
     h1, h2 = wf.real, wf.imag
 
     rh1 = np.cos(2 * alpha) * h1 - np.sin(2 * alpha) * h2
     rh2 = np.sin(2 * alpha) * h1 + np.cos(2 * alpha) * h2
```

### Comparing `waveformtools-2023.6.3/waveformtools/waveforms.py` & `waveformtools-2023.6.5/waveformtools/waveforms.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,464 +1,452 @@
 """ Classes for handling the waveform modes or data defined on spheres.
 
 
 Classes
 -------
-spherical_array : A 2D data-type.
-                  Stores and manages two-dimensional data on surfaces of spherical topology.
-modes_array : A data-type.
-              Handle and work with mode coefficients.
+spherical_array:	A 2D data-type.
+					Stores and manages two-dimensional data on surfaces of spherical topology.
+modes_array: A data-type.
+			 Handle and work with mode coefficients.
 """
 
 import sys
 
 import h5py
 import numpy as np
 
 from waveformtools import dataIO
-from waveformtools.dataIO import (
-    construct_mode_list,
-    get_iteration_numbers_from_keys,
-    sort_keys,
-)
+from waveformtools.dataIO import construct_mode_list, get_iteration_numbers_from_keys, sort_keys
 from waveformtools.grids import spherical_grid
 from waveformtools.transforms import Yslm_vec
 from waveformtools.waveformtools import interp_resam_wfs, message
 
 #####################
 # Units
 #####################
+
 G = 6.67428 * 10 ** (-11.0)  # m^3 /kg /s^2
 # c = 3.0 * 10**8  # m/s
 c = 299_792_458.0  # m/s
 # Msun = 1.32712440041e20
 Msun = 1.988500 * 10**30.0	# g, SI
 muc = c**2 / (G * Msun)  # g, NR to SI
 tuc = G * Msun / (c**3)  # s, NR to SI
 # dMpc = 3.0857 * 10 ** (22)  # m
 dMpc = 3.0856775814913672789139379577965e22
 
+#################################################
+# Spherical array class
+################################################
+
+
 # @jitclass(spec_sp)
 class spherical_array:
-    """A class for handling waveforms on a sphere.
+	"""A class for handling waveforms on a sphere.
+
+
+	Attributes
+	----------
+	label:	str
+									The label of the waveform data.
+	time_axis:	1d array
+													The time axis of the data.
+	frequency_axis: 1d array
+																	The frequency axis if the data
+																	is represented in frequency domain.
+	grid_info:	spherical_grid
+													An instance of the `spherical_grid` class.
+	data_len:	int
+													The length of the data along the time axis.
+
+	Methods
+	-------
+	delta_t:
+									Fetch the time stepping `delta_t`.
+	to_modes_array:
+																	Find the waveform expressed in the
+																	SWSH basis.
+	boost:
+					Boost the waveform.
+	supertranslate:
+													Supertranslate the waveform.
+	"""
+
+	def __init__(
+		self,
+		label=None,
+		time_axis=None,
+		frequency_axis=None,
+		data=None,
+		data_dir=None,
+		file_name=None,
+		grid_info=None,
+		spin_weight=2,
+	):
+		self.label = label
+		# self.base_dir = base_dir	# The base directory containing the
+		self.data = data
+		self.file_name = file_name
+		self.data_dir = data_dir
+		self.time_axis = time_axis
+		self.frequency_axis = frequency_axis
+		self.grid_info = grid_info
+		self.spin_weight = spin_weight
+
+	def delta_t(self, value=None):
+		"""Sets and returns the value of time stepping :math:`dt`.
+
+		Parameters
+		----------
+		value : float, optional
+										The value of :math:`dt`
+										to set to the attribute.
+
+		Returns
+		-------
+		delta_t:	float
+														Sets the attribute.
+		"""
+
+		# if not self.delta_t:
+		if not value:
+			try:
+				delta_t = self.time_axis[1] - self.time_axis[0]
+			except Exception as ex:
+				message("Please input the value of `delta_t` or supply the `time_axis` to the waveform.", ex)
+		else:
+			delta_t = value
+
+		return delta_t
+
+	@property
+	def data_len(self):
+		"""Returns the length of the time/frequency axis.
+
+		Returns
+		-------
+		data_len:	int
+														The length of the time/frequency axis.
+		"""
+
+		try:
+			data_len = len(self.time_axis)
+
+		except Exception as ex:
+			data_len = len(self.frequency_axis)
+			message(ex)
+
+		return data_len
+
+	def to_modes_array(self, grid_info=None, spin_weight=None, ell_max=8):
+		"""Decompose a given spherical array function on a sphere
+		into Spin Weighted Spherical Harmonic modes.
+
+		Parameters
+		----------
+		spin_weight:	int, optional
+																		The spin weight of the waveform. It defaults to -2 for a gravitational waveform.
+		ell_max:	int, optional
+														The maximum value of the :math:`\\ell` polar quantum number. Defaults to 8.
+		grid_info:	class instance
+														The class instance that contains the properties of the spherical grid.
+
+		Returns
+		-------
+		waveforms_modes:	modes_array
+																						An instance of the `modes_array` class containing the decomposed modes.
+
+		Notes
+		-----
+		1. Assumes that the sphere on which this decomposition is carried out is so far out
+		   that the coordinate system is spherical polar on a round sphere.
+		2. Assumes that the poper area is the same as its co-ordinate area.
+		3. Ensure that the label of the input spherical array indicates whether
+		   it is a time domain data or frequency domain data.
+		"""
+
+		if grid_info is None:
+			if self.grid_info is None:
+				message("Please specify the grid specs. Assuming defaults.")
+				grid_info = spherical_grid()
+				self.grid_info = grid_info
+			else:
+				grid_info = self.grid_info
+
+		if spin_weight is None:
+			if self.spin_weight is None:
+				message("Please specify spin weight. Assuming 2")
+				spin_weight = 2
+				self.spin_weight = spin_weight
+
+			else:
+				spin_weight = self.spin_weight
+
+		spin_weight = abs(spin_weight)
+		# Compute the meshgrid for theta and phi.
+		theta, phi = grid_info.meshgrid
+
+		# Create a modes array object
+
+		# Create a modes list.
+		modes_list = construct_mode_list(ell_max, spin_weight=spin_weight)
+
+		if not self.label:
+			label = "decomposed_time_domain"
+		else:
+			label = self.label
+
+		# Create a mode array for the decomposed_waveform
+		waveform_modes = modes_array(label=label, ell_max=ell_max, spin_weight=spin_weight)
+
+		# Inherit the time or frequency axis.
+		if "time" in label:
+			# axis = self.time_axis
+			waveform_modes.time_axis = self.time_axis
+		else:
+			# axis = self.frequency_axis
+			waveform_modes.frequency_axis = self.frequency_axis
+
+		# Create the modes_array
+		waveform_modes.create_modes_array(ell_max=ell_max, data_len=self.data_len)
+		waveform_modes.modes_list = modes_list
+		# The area element on the sphere
+		# Compute the meshgrid for theta and phi.
+		theta, phi = grid_info.meshgrid
+
+		# sqrt_met_det = np.sin(theta)
+		sqrt_met_det = np.sqrt(np.power(np.sin(theta), 2))
+
+		darea = sqrt_met_det * grid_info.dtheta * grid_info.dphi
+
+		modes_list = [item for item in modes_list if item[0] >= spin_weight]
+
+		for mode in modes_list:
+			ell_value, all_emm_values = mode
+
+			for emm_value in all_emm_values:
+				# m value.
+
+				# Spin weighted spherical harmonic function at (theta, phi)
+
+				Ybasis_fun = np.conj(
+					Yslm_vec(spin_weight, ell=ell_value, emm=emm_value, theta_grid=theta, phi_grid=phi)
+				)
+
+				Ydarea = Ybasis_fun * darea
+				# print(Ydarea.shape)
+				# print(full_integrand)
+				# Using quad
+				multipole_ell_emm = np.tensordot(self.data, Ydarea, axes=((0, 1), (0, 1)))
+
+				# print(f'l{ell_value}m{emm_value}', multipole_ell_emm)
+
+				waveform_modes.set_mode_data(ell_value, emm_value, multipole_ell_emm)
+
+		return waveform_modes
+
+	def boost(self, conformal_factor, grid_info=None):
+		"""Boost the waveform given the unboosted
+		waveform and the boost conformal factor.
+
+		Parameters
+		----------
+
+		self:	spherical_array
+										A class instance of `spherical array`.
+
+		conformal_factor:	2d array
+																						The conformal factor for the Lorentz transformation.
+																						It may be a single floating point number or an array
+																						on a spherical grid. The array will be of dimensions
+																						[ntheta, nphi]
+
+		grid_info:	class instance
+														The class instance that contains the properties of the spherical grid.
+
+
+		Returns
+		-------
+		boosted_waveform:	sp_array
+																						The class instance `sp_array` that
+																						contains the boosted waveform.
+		"""
+
+		from waveformtools.waveforms import spherical_array
+
+		if grid_info is None:
+			grid_info = self.grid_info
+
+		# Compute the boosted waveform on the spherical grid on all the elements.
+
+		boosted_waveform_data = np.transpose(self.data, (2, 0, 1)) * conformal_factor
+		# boosted_waveform_data = np.multiply(self.data, conformal_factor[:, :, None])
+		# boosted_waveform_data = boosted_waveform_item
+		# boosted_waveform_data = np.array([np.transpose(item)*conformal_factor
+		# for item in np.transpose(self.data)])
+
+		# Construct a 2d waveform array object
+		boosted_waveform = spherical_array(
+			grid_info=grid_info, data=np.transpose(np.array(boosted_waveform_data), (1, 2, 0))
+		)
+
+		# Assign other attributes.
+		boosted_waveform.label = "boosted " + self.label
+		boosted_waveform.time_axis = self.time_axis
+
+		return boosted_waveform
+
+	def supertranslate(self, supertransl_alpha_sp, order=1):
+		"""Supertranslate the :math:`\\Psi_{4\\ell m}` waveform modes, give the,
+		the supertranslation parameter and the order.
+
+		Parameters
+		----------
+		supertransl_alpha_modes :	modes_array
+																														The modes_array containing the
+																														supertranslation mode coefficients.
+		grid_info:	class instance
+														The class instance that contains
+														the properties of the spherical grid
+														using which the computations are
+														carried out.
+		order:	int
+										The number of terms to use to
+										approximate the supertranslation.
+
+		Returns
+		-------
+		Psi4_supertransl:	modes_array
+																						A class instance containg the
+																						modes of the supertranslated
+																						waveform :math:`\\Psi_4`.
+		"""
+
+		# Create a spherical_array to hold the supertranslated waveform
+		Psi4_supertransl_sp = spherical_array(
+			grid_info=self.grid_info, label="{} -> supertranslated time".format(self.label)
+		)
+
+		delta_t = float(self.delta_t())
+
+		# Set the data.
+		data = 0
+		# data = self.data
+		# Psi4_supertransl_sp.data = self.data
+		# delta = 0
+		# count = 0
+		from waveformtools.differentiate import differentiate5_vec_numba
+
+		for index in range(order):
+			# print(f'{index} loop')
+			dPsidu = self.data
+			for dorder in range(index + 1):
+				# print(f'differentiating {dorder+1} times')
+				dPsidu = differentiate5_vec_numba(dPsidu, delta_t)
+
+			message("Incrementing...")
+			# delta = np.power(supertransl_alpha_sp.data, index+1) * dPsidu / np.math.factorial(index+1)
+			# print(delta/self.data)
+
+			data += np.power(supertransl_alpha_sp.data, index + 1) * dPsidu / np.math.factorial(index + 1)	# delta
+
+		data += self.data
+		message("Equal to original waveform?", (data == self.data).all())
+
+		Psi4_supertransl_sp.data = data
+		Psi4_supertransl_sp.time_axis = self.time_axis
+		message("Done.")
+		return Psi4_supertransl_sp
+
+	def load_qlm_data(self, data_dir=None, grid_info=None, bh=0, variable="sigma"):
+		"""Load the 2D shear data from h5 files.
+
+		Parameters
+		----------
+		file_name:	str
+														The name of the file containing data.
+		data_dir:	str
+														The name of the directory containing data.
+		grid_info:	class instance
+														An instance of the grid_info class.
+		bh: int
+						The black hole number (0, 1 or 2)
+		"""
+
+		if data_dir is None:
+			if self.data_dir is None:
+				print("Please supply the data directory!")
+			else:
+				data_dir = self.data_dir
+		else:
+			if self.data_dir is None:
+				self.data_dir = data_dir
+
+		if grid_info is None:
+			if self.grid_info is None:
+				message("Please supply the grid spec!")
+			else:
+				grid_info = self.grid_info
+		else:
+			if self.grid_info is None:
+				self.grid_info = grid_info
+		# get the full path.
+
+		file_name = f"qlm_{variable}[{bh}].xy.h5"
+
+		full_path = self.data_dir + file_name
+
+		# cflag = 0
+
+		nghosts = grid_info.nghosts
+		ntheta = grid_info.ntheta
+		nphi = grid_info.nphi
+
+		# Open the modes file.
+		with h5py.File(full_path, "r") as wfile:
+			# Get all the mode keys.
+			modes_keys_list = list(wfile.keys())
+			# modes_keys_list = sorted(modes_keys_list)
+
+			# Get the mode keys containing the data.
+			modes_keys_list = [item for item in modes_keys_list if "it=" in item]
+
+			# Get the itaration numbers.
+			iteration_numbers = sorted(get_iteration_numbers_from_keys(modes_keys_list))
+			# sargs = np.argsort(iteration_numbers)
+			# iteration_numbers = iteration_numbers[sargs]
+			modes_keys_list = sort_keys(modes_keys_list)
+			# Construct the data array.
+
+			data_array = []
+
+			for key in modes_keys_list:
+				# data_item = np.array(wfile[key])
+				# print(data_item.shape)
+				data_item = np.array(wfile[key])[nghosts : nphi - nghosts, nghosts : ntheta - nghosts]
+				try:
+					data_item = data_item["real"] + 1j * data_item["imag"]
+				except Exception as ex:
+					message(ex)
+					pass
+
+				data_array.append(data_item)
 
-    Attributes
-    ----------
-    label : str
-            The label of the waveform data.
-    time_axis : 1d array
-                The time axis of the data.
-    frequency_axis : 1d array
-                     The frequency axis if the data
-                     is represented in frequency domain.
-    grid_info : spherical_grid
-                An instance of the `spherical_grid` class.
-    data_len : int
-               The length of the data along the time axis.
-
-    Methods
-    -------
-    delta_t
-        Fetch the time stepping `delta_t`.
-    to_modes_array
-            Find the waveform expressed in the SWSH basis.
-    boost
-        Boost the waveform.
-    supertranslate
-                Supertranslate the waveform.
-    """
-
-    def __init__(
-        self,
-        label=None,
-        time_axis=None,
-        frequency_axis=None,
-        data=None,
-        data_dir=None,
-        file_name=None,
-        grid_info=None,
-        spin_weight=2,
-    ):
-        self.label = label
-        # self.base_dir = base_dir  # The base directory containing the
-        self.data = data
-        self.file_name = file_name
-        self.data_dir = data_dir
-        self.time_axis = time_axis
-        self.frequency_axis = frequency_axis
-        self.grid_info = grid_info
-        self.spin_weight = spin_weight
-
-    def delta_t(self, value=None):
-        """Sets and returns the value of time stepping :math:`dt`.
-
-        Parameters
-        ----------
-        value : float, optional
-                The value of :math:`dt`
-                to set to the attribute.
-
-        Returns
-        -------
-        delta_t : float
-                  Sets the attribute.
-        """
-
-        # if not self.delta_t:
-        if not value:
-            try:
-                delta_t = self.time_axis[1] - self.time_axis[0]
-            except Exception as ex:
-                message(
-                    "Please input the value of `delta_t` or supply the `time_axis` to the waveform.",
-                    ex,
-                )
-        else:
-            delta_t = value
-
-        return delta_t
-
-    @property
-    def data_len(self):
-        """Returns the length of the time/frequency axis.
-
-        Returns
-        -------
-        data_len : int
-                   The length of the time/frequency axis.
-        """
-
-        try:
-            data_len = len(self.time_axis)
-
-        except Exception as ex:
-            data_len = len(self.frequency_axis)
-            message(ex)
-
-        return data_len
-
-    def to_modes_array(self, grid_info=None, spin_weight=None, ell_max=8):
-        """Decompose a given spherical array function on a sphere
-        into Spin Weighted Spherical Harmonic modes.
-
-        Parameters
-        ----------
-        spin_weight : int, optional
-                      The spin weight of the waveform. It defaults
-                      to -2 for a gravitational waveform.
-        ell_max : int, optional
-                  The maximum value of the :math:`\\ell`
-                  polar quantum number. Defaults to 8.
-        grid_info : class instance
-                    The class instance that contains
-                    the properties of the spherical grid.
-
-        Returns
-        -------
-        waveforms_modes : modes_array
-                          An instance of the `modes_array`
-                          class containing the decomposed modes.
-
-        Notes
-        -----
-        1. Assumes that the sphere on which this decomposition is carried out is so far out
-           that the coordinate system is spherical polar on a round sphere.
-        2. Assumes that the poper area is the same as its co-ordinate area.
-        3. Ensure that the label of the input spherical array indicates whether
-           it is a time domain data or frequency domain data.
-        """
-
-        if grid_info is None:
-            if self.grid_info is None:
-                message("Please specify the grid specs. Assuming defaults.")
-                grid_info = spherical_grid()
-                self.grid_info = grid_info
-            else:
-                grid_info = self.grid_info
-
-        if spin_weight is None:
-            if self.spin_weight is None:
-                message("Please specify spin weight. Assuming 2")
-                spin_weight = 2
-                self.spin_weight = spin_weight
-
-            else:
-                spin_weight = self.spin_weight
-
-        spin_weight = abs(spin_weight)
-        # Compute the meshgrid for theta and phi.
-        theta, phi = grid_info.meshgrid
-
-        # Create a modes array object
-
-        # Create a modes list.
-        modes_list = construct_mode_list(ell_max, spin_weight=spin_weight)
-
-        if not self.label:
-            label = "decomposed_time_domain"
-        else:
-            label = self.label
-
-        # Create a mode array for the decomposed_waveform
-        waveform_modes = modes_array(
-            label=label, ell_max=ell_max, spin_weight=spin_weight
-        )
-
-        # Inherit the time or frequency axis.
-        if "time" in label:
-            # axis = self.time_axis
-            waveform_modes.time_axis = self.time_axis
-        else:
-            # axis = self.frequency_axis
-            waveform_modes.frequency_axis = self.frequency_axis
-
-        # Create the modes_array
-        waveform_modes.create_modes_array(
-            ell_max=ell_max, data_len=self.data_len
-        )
-        waveform_modes.modes_list = modes_list
-        # The area element on the sphere
-        # Compute the meshgrid for theta and phi.
-        theta, phi = grid_info.meshgrid
-
-        # sqrt_met_det = np.sin(theta)
-        sqrt_met_det = np.sqrt(np.power(np.sin(theta), 2))
-
-        darea = sqrt_met_det * grid_info.dtheta * grid_info.dphi
-
-        modes_list = [item for item in modes_list if item[0] >= spin_weight]
-
-        for mode in modes_list:
-            ell_value, all_emm_values = mode
-
-            for emm_value in all_emm_values:
-                # m value.
-
-                # Spin weighted spherical harmonic function at (theta, phi)
-
-                Ybasis_fun = np.conj(
-                    Yslm_vec(
-                        spin_weight,
-                        ell=ell_value,
-                        emm=emm_value,
-                        theta_grid=theta,
-                        phi_grid=phi,
-                    )
-                )
-
-                Ydarea = Ybasis_fun * darea
-                # print(Ydarea.shape)
-                # print(full_integrand)
-                # Using quad
-                multipole_ell_emm = np.tensordot(
-                    self.data, Ydarea, axes=((0, 1), (0, 1))
-                )
-
-                # print(f'l{ell_value}m{emm_value}', multipole_ell_emm)
-
-                waveform_modes.set_mode_data(
-                    ell_value, emm_value, multipole_ell_emm
-                )
-
-        return waveform_modes
-
-    def boost(self, conformal_factor, grid_info=None):
-        """Boost the waveform given the unboosted
-        waveform and the boost conformal factor.
-
-        Parameters
-        ----------
-        self : spherical_array
-               A class instance of `spherical array`.
-        conformal_factor : 2d array
-                           The conformal factor for the Lorentz transformation.
-                           It may be a single floating point number or an array
-                           on a spherical grid. The array will be of dimensions
-                           [ntheta, nphi]
-
-        grid_info : class instance
-                    The class instance that contains the properties of the spherical grid.
-
-        Returns
-        -------
-        boosted_waveform : sp_array
-                           The class instance `sp_array` that
-                           contains the boosted waveform.
-        """
+		self.data = np.transpose(np.array(data_array), (2, 1, 0))
 
-        from waveformtools.waveforms import spherical_array
+		self.iteration_axis = np.array(iteration_numbers)
+
+		#########################################################
+		# Load inv_coords data
+		#########################################################
 
 		inv_file_name = f"qlm_inv_z[{bh}].xy.h5"
 
-        boosted_waveform_data = (
-            np.transpose(self.data, (2, 0, 1)) * conformal_factor
-        )
-        # boosted_waveform_data = np.multiply(self.data, conformal_factor[:, :, None])
-        # boosted_waveform_data = boosted_waveform_item
-        # boosted_waveform_data = np.array([np.transpose(item)*conformal_factor
-        # for item in np.transpose(self.data)])
-
-        # Construct a 2d waveform array object
-        boosted_waveform = spherical_array(
-            grid_info=grid_info,
-            data=np.transpose(np.array(boosted_waveform_data), (1, 2, 0)),
-        )
-
-        # Assign other attributes.
-        boosted_waveform.label = "boosted " + self.label
-        boosted_waveform.time_axis = self.time_axis
-
-        return boosted_waveform
-
-    def supertranslate(self, supertransl_alpha_sp, order=1):
-        """Supertranslate the :math:`\\Psi_{4\\ell m}` waveform modes, give the,
-        the supertranslation parameter and the order.
-
-        Parameters
-        ----------
-        supertransl_alpha_modes : modes_array
-                                  The modes_array containing the
-                                  supertranslation mode coefficients.
-        grid_info : class instance
-                    The class instance that contains
-                    the properties of the spherical grid
-                    using which the computations are
-                    carried out.
-        order : int
-                The number of terms to use to
-                approximate the supertranslation.
-
-        Returns
-        -------
-        Psi4_supertransl : modes_array
-                           A class instance containg the
-                           modes of the supertranslated
-                           waveform :math:`\\Psi_4`.
-        """
-
-        # Create a spherical_array to hold the supertranslated waveform
-        Psi4_supertransl_sp = spherical_array(
-            grid_info=self.grid_info,
-            label="{} -> supertranslated time".format(self.label),
-        )
-
-        delta_t = float(self.delta_t())
-
-        # Set the data.
-        data = 0
-        # data = self.data
-        # Psi4_supertransl_sp.data = self.data
-        # delta = 0
-        # count = 0
-        from waveformtools.differentiate import differentiate5_vec_numba
-
-        for index in range(order):
-            # print(f'{index} loop')
-            dPsidu = self.data
-            for dorder in range(index + 1):
-                # print(f'differentiating {dorder+1} times')
-                dPsidu = differentiate5_vec_numba(dPsidu, delta_t)
-
-            message("Incrementing...")
-            # delta = np.power(supertransl_alpha_sp.data, index+1) * dPsidu / np.math.factorial(index+1)
-            # print(delta/self.data)
-
-            data += (
-                np.power(supertransl_alpha_sp.data, index + 1)
-                * dPsidu
-                / np.math.factorial(index + 1)
-            )  # delta
-
-        data += self.data
-        message("Equal to original waveform?", (data == self.data).all())
-
-        Psi4_supertransl_sp.data = data
-        Psi4_supertransl_sp.time_axis = self.time_axis
-        message("Done.")
-        return Psi4_supertransl_sp
-
-    def load_qlm_data(
-        self, data_dir=None, grid_info=None, bh=0, variable="sigma"
-    ):
-        """Load the 2D shear data from h5 files.
-
-        Parameters
-        ----------
-        file_name : str
-                    The name of the file containing data.
-        data_dir : str
-                   The name of the directory containing data.
-        grid_info : class instance
-                    An instance of the grid_info class.
-        bh : int
-             The black hole number (0, 1 or 2)
-        """
-
-        if data_dir is None:
-            if self.data_dir is None:
-                print("Please supply the data directory!")
-            else:
-                data_dir = self.data_dir
-        else:
-            if self.data_dir is None:
-                self.data_dir = data_dir
-
-        if grid_info is None:
-            if self.grid_info is None:
-                message("Please supply the grid spec!")
-            else:
-                grid_info = self.grid_info
-        else:
-            if self.grid_info is None:
-                self.grid_info = grid_info
-        # get the full path.
-
-        file_name = f"qlm_{variable}[{bh}].xy.h5"
-
-        full_path = self.data_dir + file_name
-
-        # cflag = 0
-
-        nghosts = grid_info.nghosts
-        ntheta = grid_info.ntheta
-        nphi = grid_info.nphi
-
-        # Open the modes file.
-        with h5py.File(full_path, "r") as wfile:
-            # Get all the mode keys.
-            modes_keys_list = list(wfile.keys())
-            # modes_keys_list = sorted(modes_keys_list)
-
-            # Get the mode keys containing the data.
-            modes_keys_list = [
-                item for item in modes_keys_list if "it=" in item
-            ]
-
-            # Get the itaration numbers.
-            iteration_numbers = sorted(
-                get_iteration_numbers_from_keys(modes_keys_list)
-            )
-            # sargs = np.argsort(iteration_numbers)
-            # iteration_numbers = iteration_numbers[sargs]
-            modes_keys_list = sort_keys(modes_keys_list)
-            # Construct the data array.
-
-            data_array = []
-
-            for key in modes_keys_list:
-                # data_item = np.array(wfile[key])
-                # print(data_item.shape)
-                data_item = np.array(wfile[key])[
-                    nghosts : nphi - nghosts, nghosts : ntheta - nghosts
-                ]
-                try:
-                    data_item = data_item["real"] + 1j * data_item["imag"]
-                except Exception as ex:
-                    message(ex)
-                    pass
+		# get the full path.
+		full_path = self.data_dir + inv_file_name
 
 		# Open the modes file.
 		with h5py.File(full_path, "r") as wfile:
 			# Get all the mode keys.
 			modes_keys_list = list(wfile.keys())
 			# modes_keys_list = sorted(modes_keys_list)
 
@@ -479,1357 +467,1282 @@
 		# Load metric determinant  data
 		#########################################################
 
 		twometric_qtt_file_name = f"qlm_qtt[{bh}].xy.h5"
 		twometric_qtp_file_name = f"qlm_qtp[{bh}].xy.h5"
 		twometric_qpp_file_name = f"qlm_qpp[{bh}].xy.h5"
 
-            # Get the mode keys containing the data.
-            modes_keys_list = [
-                item for item in modes_keys_list if "it=" in item
-            ]
+		# set the full path.
+		full_path = self.data_dir + twometric_qtt_file_name
 
 		# Open the modes file.
 		with h5py.File(full_path, "r") as wfile:
 			# Get all the mode keys.
 			modes_keys_list = list(wfile.keys())
 			# modes_keys_list = sorted(modes_keys_list)
 
-            for key in modes_keys_list:
-                data_item = np.array(wfile[key])[
-                    nghosts : nphi - nghosts, nghosts : ntheta - nghosts
-                ]
-                # data_item = data_item['real'] + 1j*data_item['imag']
-                data_array.append(data_item)
-
-        self.invariant_coordinates_data = np.transpose(
-            np.array(data_array), (2, 1, 0)
-        )
+			# Get the mode keys containing the data.
+			modes_keys_list = [item for item in modes_keys_list if "it=" in item]
+
+			modes_keys_list = sort_keys(modes_keys_list)
 
 			qtt_data_array = []
 
 			for key in modes_keys_list:
 				data_item = np.array(wfile[key])[nghosts : nphi - nghosts, nghosts : ntheta - nghosts]
 				# data_item = data_item['real'] + 1j*data_item['imag']
 				qtt_data_array.append(data_item)
 
 		qtt_data_array = np.array(qtt_data_array)
 		qtt_data_array = np.transpose(qtt_data_array, (2, 1, 0))
 
 		# set the full path.
 		full_path = self.data_dir + twometric_qtp_file_name
 
-            # Get the mode keys containing the data.
-            modes_keys_list = [
-                item for item in modes_keys_list if "it=" in item
-            ]
+		# Open the modes file.
+		with h5py.File(full_path, "r") as wfile:
+			# Get all the mode keys.
+			modes_keys_list = list(wfile.keys())
+			# modes_keys_list = sorted(modes_keys_list)
 
 			# Get the mode keys containing the data.
 			modes_keys_list = [item for item in modes_keys_list if "it=" in item]
 
 			modes_keys_list = sort_keys(modes_keys_list)
 
-            for key in modes_keys_list:
-                data_item = np.array(wfile[key])[
-                    nghosts : nphi - nghosts, nghosts : ntheta - nghosts
-                ]
-                # data_item = data_item['real'] + 1j*data_item['imag']
-                qtt_data_array.append(data_item)
+			qtp_data_array = []
 
 			for key in modes_keys_list:
 				data_item = np.array(wfile[key])[nghosts : nphi - nghosts, nghosts : ntheta - nghosts]
 				# data_item = data_item['real'] + 1j*data_item['imag']
 				qtp_data_array.append(data_item)
 
 		qtp_data_array = np.array(qtp_data_array)
 		qtp_data_array = np.transpose(qtp_data_array, (2, 1, 0))
 
 		# set the full path.
 		full_path = self.data_dir + twometric_qpp_file_name
 
-            # Get the mode keys containing the data.
-            modes_keys_list = [
-                item for item in modes_keys_list if "it=" in item
-            ]
+		# Open the modes file.
+		with h5py.File(full_path, "r") as wfile:
+			# Get all the mode keys.
+			modes_keys_list = list(wfile.keys())
+			# modes_keys_list = sorted(modes_keys_list)
 
 			# Get the mode keys containing the data.
 			modes_keys_list = [item for item in modes_keys_list if "it=" in item]
 
 			modes_keys_list = sort_keys(modes_keys_list)
 
-            for key in modes_keys_list:
-                data_item = np.array(wfile[key])[
-                    nghosts : nphi - nghosts, nghosts : ntheta - nghosts
-                ]
-                # data_item = data_item['real'] + 1j*data_item['imag']
-                qtp_data_array.append(data_item)
-
-        qtp_data_array = np.array(qtp_data_array)
-        qtp_data_array = np.transpose(qtp_data_array, (2, 1, 0))
-
-        # set the full path.
-        full_path = self.data_dir + twometric_qpp_file_name
-
-        # Open the modes file.
-        with h5py.File(full_path, "r") as wfile:
-            # Get all the mode keys.
-            modes_keys_list = list(wfile.keys())
-            # modes_keys_list = sorted(modes_keys_list)
-
-            # Get the mode keys containing the data.
-            modes_keys_list = [
-                item for item in modes_keys_list if "it=" in item
-            ]
-
-            modes_keys_list = sort_keys(modes_keys_list)
-
-            qpp_data_array = []
-
-            for key in modes_keys_list:
-                data_item = np.array(wfile[key])[
-                    nghosts : nphi - nghosts, nghosts : ntheta - nghosts
-                ]
-                # data_item = data_item['real'] + 1j*data_item['imag']
-                qpp_data_array.append(data_item)
-
-        qpp_data_array = np.array(qpp_data_array)
-        qpp_data_array = np.transpose(qpp_data_array, (2, 1, 0))
-
-        sqrt_met_det = np.sqrt(
-            np.linalg.det(
-                np.transpose(
-                    np.array(
-                        [
-                            [qtt_data_array, qtp_data_array],
-                            [qtp_data_array, qpp_data_array],
-                        ]
-                    ),
-                    (2, 3, 4, 0, 1),
-                )
-            )
-        )
+			qpp_data_array = []
+
+			for key in modes_keys_list:
+				data_item = np.array(wfile[key])[nghosts : nphi - nghosts, nghosts : ntheta - nghosts]
+				# data_item = data_item['real'] + 1j*data_item['imag']
+				qpp_data_array.append(data_item)
+
+		qpp_data_array = np.array(qpp_data_array)
+		qpp_data_array = np.transpose(qpp_data_array, (2, 1, 0))
+
+		sqrt_met_det = np.sqrt(
+			np.linalg.det(
+				np.transpose(
+					np.array([[qtt_data_array, qtp_data_array], [qtp_data_array, qpp_data_array]]), (2, 3, 4, 0, 1)
+				)
+			)
+		)
+
+		self.sqrt_met_det_data = sqrt_met_det
+
+	def to_shear_modes_array(self, grid_info=None, spin_weight=None, ell_max=8):
+		"""Decompose a given spherical array function on a sphere
+		into Spin Weighted Spherical Harmonic modes.
+
+		Parameters
+		----------
+		spin_weight:	int, optional
+																		The spin weight of the waveform. It defaults to -2 for a gravitational waveform.
+		ell_max:	int, optional
+														The maximum value of the :math:`\\ell` polar quantum number. Defaults to 8.
+		grid_info:	class instance
+														The class instance that contains the properties of the spherical grid.
+
+		Returns
+		-------
+		waveforms_modes:	modes_array
+																						An instance of the `modes_array` class containing the decomposed modes.
+
+		Notes
+		-----
+		1. Assumes that the sphere on which this decomposition is carried out is so far out
+		   that the coordinate system is spherical polar on a round sphere.
+		2. Assumes that the poper area is the same as its co-ordinate area.
+		3. Ensure that the label of the input spherical array indicates whether
+		   it is a time domain data or frequency domain data.
+		"""
 
-        self.sqrt_met_det_data = sqrt_met_det
+		if grid_info is None:
+			if self.grid_info is None:
+				message("Please specify the grid specs. Assuming defaults.")
+				grid_info = spherical_grid()
+				self.grid_info = grid_info
+			else:
+				grid_info = self.grid_info
+
+		if spin_weight is None:
+			if self.spin_weight is None:
+				message("Please specify spin weight. Assuming 2")
+				spin_weight = 2
+				self.spin_weight = spin_weight
+
+			else:
+				spin_weight = self.spin_weight
+
+		spin_weight = abs(spin_weight)
+		# Compute the meshgrid for theta and phi.
+		theta, phi = grid_info.meshgrid
+
+		# Create a modes array object
+
+		# Create a modes list.
+		modes_list = construct_mode_list(ell_max, spin_weight=spin_weight)
+
+		if not self.label:
+			label = "decomposed_time_domain"
+		else:
+			label = self.label
+
+		# Create a mode array for the decomposed_waveform
+		waveform_modes = modes_array(label=label, ell_max=ell_max, spin_weight=spin_weight)
+
+		# Inherit the time or frequency axis.
+		if "time" in label:
+			# axis = self.time_axis
+			waveform_modes.time_axis = self.time_axis
+		else:
+			# axis = self.frequency_axis
+			waveform_modes.frequency_axis = self.frequency_axis
+
+		# Create the modes_array
+		waveform_modes.time_axis = self.time_axis[:]
+		# sargs = np.argsort(waveform_modes.time_axis)
+		# message(sargs)
+		waveform_modes.time_axis = waveform_modes.time_axis
+
+		waveform_modes.create_modes_array(ell_max=ell_max, data_len=self.data_len)
+		waveform_modes.modes_list = modes_list
+		# The area element on the sphere
+		# Compute the meshgrid for theta and phi.
+		theta, phi = grid_info.meshgrid
+
+		phi = np.transpose(np.array([phi for index in range(len(self.time_axis))]), (1, 2, 0))
+
+		# sqrt_met_det = np.sin(theta)
+		# sqrt_met_det = np.sqrt(np.power(np.sin(theta), 2))
+
+		darea = self.sqrt_met_det_data * grid_info.dtheta * grid_info.dphi
+
+		theta = np.emath.arccos(self.invariant_coordinates_data)
+
+		modes_list = [item for item in modes_list if item[0] >= spin_weight]
+
+		for mode in modes_list:
+			ell_value, all_emm_values = mode
+
+			for emm_value in all_emm_values:
+				# m value.
+				# message(f'Processing l{ell_value} m{emm_value}')
+				# Spin weighted spherical harmonic function at (theta, phi)
+
+				Ybasis_fun = np.conj(
+					Yslm_vec(spin_weight=spin_weight, ell=ell_value, emm=emm_value, theta_grid=theta, phi_grid=phi)
+				)
+				# Ybasis_fun = np.array([np.conj(Yslm_vec(spin_weight=spin_weight,
+				# ell=ell_value, emm=emm_value, theta_grid=theta[:, :, index],
+				# phi_grid=phi[:, :, index])) for index in range(self.data_len)])
+				# Ybasis_fun = np.transpose(Ybasis_fun, (1, 2, 0))
+				# message('Ybasis_fun', Ybasis_fun.shape)
+				Ydarea = Ybasis_fun * darea
+				# message('Ydarea', Ydarea.shape)
+				# message(full_integrand)
+				# Using quad
+				# message('self.data', self.data.shape)
+				# multipole_ell_emm = np.tensordot(self.data, Ydarea, axes=((0, 1), (0, 1)))
+				multipole_ell_emm = np.sum(self.data * Ydarea, (0, 1))
+
+				# message(f'l{ell_value}m{emm_value}', multipole_ell_emm)
+
+				# message('multipole_ell_emm', multipole_ell_emm.shape)
+				waveform_modes.set_mode_data(ell_value, emm_value, data=multipole_ell_emm)
+
+		return waveform_modes
 
 
 # @jitclass(spec_ma)
 class modes_array:
-    """A class that holds mode array of waveforms
+	"""A class that holds mode array of waveforms
+
+	Attributes
+	----------
+	label:	str
+									The label of the modes array.
+	r_ext:	float
+									The extraction radius.
+	modes_list: list
+													The list of available modes
+													in the format [l1, [m values], [l2, [m values], ...]]
+	ell_max:	int
+													The maximum :math:`\\ell` mode available.
+	modes_data: 3d array
+													The three dimensional array
+													containing modes in time/frequency
+													space. The axis of the array is
+													(:math:`\\ell`, :math:`m`, time/freq).
+	base_dir:	str
+													The base directory containing the
+													modes data.
+	data_dir:	str
+													The subdirectory in which to look
+													for the data.
+	filename:	str
+													The filename containg the modes data.
+
+	Methods
+	-------
+	get_metadata:
+													Get the metadata associated with the modes_array.
+	mode:
+					Get the data for the given :math:`\\ell, m` mode.
+	create_modes_array:
+																	A private method to create an empty modes_array of given shape.
+	delta_t:
+									Set the attribute `delta_t` and/ or return its value.
+	load_modes:
+									Load the waveform modes from a specified h5 file.
+	save_modes:
+									Save the waveform modes to a specified h5 file.
+	set_mode_data:
+									Set the `mode` data of specified modes.
+	to_frequency_basis:
+									Get the `modes_array` in frequency basis from its time basis representation.
+	to_time_basis:
+									Get the `modes_array` in temporal basis from its frequency basis representation.
+	extrap_to_inf:
+									Extrapolate the modes to infinity.
+	supertranslate:
+									Supertranslate the waveform modes.
+	boost:
+					Boost the waveform modes.
+	"""
+
+	def __init__(
+		self,
+		data_dir=None,
+		file_name=None,
+		modes_data=None,
+		time_axis=None,
+		frequency_axis=None,
+		key_format=None,
+		ell_max=None,
+		modes_list=None,
+		label=None,
+		r_ext=np.inf,
+		out_file_name=None,
+		maxtime=None,
+		date=None,
+		time=None,
+		key_ex=None,
+		spin_weight=-2,
+		actions="empty",
+	):
+		self.label = label
+		self.data_dir = data_dir
+		self.file_name = file_name
+		self.modes_data = modes_data
+		self.key_format = key_format
+		self.ell_max = ell_max
+		self.modes_list = modes_list
+		self.r_ext = r_ext
+		self.time_axis = time_axis
+		self.frequency_axis = frequency_axis
+		self.out_file_name = out_file_name
+		self.maxtime = maxtime
+		self.date = date
+		self.time = time
+		self.key_ex = key_ex
+		self.spin_weight = spin_weight
+		self.actions = actions
+
+	def get_metadata(self):
+		"""Get the metadata associated with the instance.
+
+		Returns
+		-------
+		metadata:	dict
+														A dictionary of metedata.
+		"""
+		# The metadata dict
+		unnecessary_keys = ["_time_axis", "_modes_data", "freq_axis"]
+
+		# Get all attributes
+		# metadata = self.__dict__
+		metadata = {}
+
+		for key, val in self.__dict__.items():
+			if key in unnecessary_keys:
+				pass
+			else:
+				metadata.update({key: val})
+
+		# for item in unnecessary_keys:
+		# metadata.pop(item, None)
+
+		# self.metadata = metadata
+
+		return metadata
+
+	def mode(self, ell, emm):
+		"""The modes array data structure to hold waveform modes.
+
+		Parameters
+		----------
+		ell:	int
+										The :math:`\\ell` index of the mode.
+		emm:	int
+										The :math:`m` index of the mode.
 
-    Attributes
-    ----------
-    label : str
-            The label of the modes array.
-    r_ext : float
-            The extraction radius.
-    modes_list : list
-                 The list of available modes
-                 in the format [l1, [m values], [l2, [m values], ...]]
-    ell_max : int
-              The maximum :math:`\\ell` mode available.
-    modes_data : 3d array
-                 The three dimensional array
-                 containing modes in time/frequency
-                 space. The axis of the array is
-                 (:math:`\\ell`, :math:`m`, time/freq).
-    base_dir : str
-               The base directory containing the
-               modes data.
-    data_dir : str
-               The subdirectory in which to look
-               for the data.
-    filename : str
-               The filename containg the modes data.
-
-    Methods
-    -------
-    get_metadata
-            Get the metadata associated with the modes_array.
-    mode
-        Get the data for the given :math:`\\ell, m` mode.
-    create_modes_array
-                A private method to create an empty modes_array of given shape.
-    delta_t
-        Set the attribute `delta_t` and/ or return its value.
-    load_modes
-            Load the waveform modes from a specified h5 file.
-    save_modes
-            Save the waveform modes to a specified h5 file.
-    set_mode_data
-            Set the `mode` data of specified modes.
-    to_frequency_basis
-            Get the `modes_array` in frequency basis from its time basis representation.
-    to_time_basis
-            Get the `modes_array` in temporal basis from its frequency basis representation.
-    extrap_to_inf
-            Extrapolate the modes to infinity.
-    supertranslate
-            Supertranslate the waveform modes.
-    boost
-        Boost the waveform modes.
-    """
-
-    def __init__(
-        self,
-        data_dir=None,
-        file_name=None,
-        modes_data=None,
-        time_axis=None,
-        frequency_axis=None,
-        key_format=None,
-        ell_max=None,
-        modes_list=None,
-        label=None,
-        r_ext=np.inf,
-        out_file_name=None,
-        maxtime=None,
-        date=None,
-        time=None,
-        key_ex=None,
-        spin_weight=-2,
-        actions="empty",
-    ):
-        self.label = label
-        self.data_dir = data_dir
-        self.file_name = file_name
-        self.modes_data = modes_data
-        self.key_format = key_format
-        self.ell_max = ell_max
-        self.modes_list = modes_list
-        self.r_ext = r_ext
-        self.time_axis = time_axis
-        self.frequency_axis = frequency_axis
-        self.out_file_name = out_file_name
-        self.maxtime = maxtime
-        self.date = date
-        self.time = time
-        self.key_ex = key_ex
-        self.spin_weight = spin_weight
-        self.actions = actions
-
-    def get_metadata(self):
-        """Get the metadata associated with the instance.
-
-        Returns
-        -------
-        metadata : dict
-                   A dictionary of metedata.
-        """
-        # The metadata dict
-        unnecessary_keys = ["_time_axis", "_modes_data", "freq_axis"]
-
-        # Get all attributes
-        # metadata = self.__dict__
-        metadata = {}
-
-        for key, val in self.__dict__.items():
-            if key in unnecessary_keys:
-                pass
-            else:
-                metadata.update({key: val})
-
-        # for item in unnecessary_keys:
-        # metadata.pop(item, None)
-
-        # self.metadata = metadata
-
-        return metadata
-
-    def mode(self, ell, emm):
-        """The modes array data structure to hold waveform modes.
-
-        Parameters
-        ----------
-        ell : int
-              The :math:`\\ell` index of the mode.
-        emm : int
-              The :math:`m` index of the mode.
-
-        Returns
-        -------
-        mode_data : array
-                    The array of the requested mode.
-        """
-
-        emm_index = ell + emm
-
-        return self.modes_data[ell, emm_index, :]
-
-    @property
-    def time_axis(self):
-        """The time axis"""
-        return np.array(self._time_axis)
-
-    @time_axis.setter
-    def time_axis(self, time_axis):
-        self._time_axis = time_axis
-
-    @property
-    def modes_data(self):
-        """The modes array"""
-        return np.array(self._modes_data)
-
-    @modes_data.setter
-    def modes_data(self, modes_data):
-        self._modes_data = modes_data
-
-    def create_modes_array(self, ell_max=None, data_len=None):
-        """Create a modes array and initialize it with zeros.
-
-        Parameters
-        ----------
-        ell_max : int
-                  The maximum :math:`\\ell` value of the modes.
-        data_len : int
-                   The number of points along the third (time / frequency) axis.
-
-        Returns
-        -------
-        self.modes_array : modes_array
-                           sets the `self.modes_array` attribute.
-        """
-        import datetime
-        import time
-
-        # Check ell_max
-        if ell_max is None:
-            try:
-                ell_max = self.ell_max
-            except Exception as ex:
-                message(ex)
-                raise NameError("Please supply ell_max")
-
-        if data_len is None:
-            try:
-                data_len = self.data_len
-            except Exception as ex:
-                message(ex)
-                raise NameError("Please supply data_len")
-
-        if self.modes_list is None:
-            self.modes_list = construct_mode_list(
-                ell_max=ell_max, spin_weight=self.spin_weight
-            )
-
-        # self.modes_data = np.zeros([ell_max + 1, 2 * (ell_max + 1) + 1, data_len], dtype=np.complex128)
-        self.modes_data = np.zeros(
-            (ell_max + 1, 2 * (ell_max + 1) + 1, data_len), dtype=np.complex128
-        )
-
-        # Set the time metadata
-        time_now = time.localtime()
-        time_now = time.strftime("%H:%M:%S", time_now)
-
-        date_now = str(datetime.date.today())
-
-        if self.time is None:
-            # Assign time and date stamp if it doesnt exist
-            self.time = time_now
-            self.date = date_now
-
-    @property
-    def data_len(self):
-        """Returns the length of the time/frequency axis.
-
-        Returns
-        -------
-        data_len : int
-                   The length of the time/frequency axis.
-        """
-
-        try:
-            data_len = len(self.time_axis)
-
-        except Exception as ex:
-            message(ex)
-            data_len = len(self.frequency_axis)
-
-        return data_len
-
-    @data_len.setter
-    def data_len(self, data_len):
-        self._data_len = data_len
-
-    def delta_t(self, value=None):
-        """Sets and returns the value of time stepping :math:`dt`.
-
-        Parameters
-        ----------
-        value : float, optional
-                The value of :math:`dt`
-                to set to the attribute.
-
-        Returns
-        -------
-        self.delta_t : float
-                       Sets the attribute.
-        """
-
-        if not value:
-            try:
-                delta_t = self.time_axis[1] - self.time_axis[0]
-            except Exception as ex:
-                message(
-                    "Please input the value of `delta_t` or supply the `time_axis` to the waveform.",
-                    ex,
-                )
-        else:
-            delta_t = value
-
-        return delta_t
-
-    @property
-    def delta_f(self, value=None):
-        """Sets and returns the value of frequency stepping :math:`df`.
-
-        Parameters
-        ----------
-        value : float, optional
-                The value of :math:`df`
-                to set to the attribute.
-
-        Returns
-        -------
-        delta_f : float
-                  Sets the attribute.
-        """
-
-        # if not self.delta_t:
-        if not value:
-            try:
-                delta_f = self.frequency_axis[1] - self.frequency_axis[0]
-            except Exception as ex:
-                message(
-                    "Please input the value of `delta_f` or supply the `frequency_axis` to the waveform.",
-                    ex,
-                )
-        else:
-            delta_f = value
-
-        return delta_f
-
-    def load_modes(
-        self,
-        label=None,
-        data_dir=None,
-        file_name=None,
-        ftype="generic",
-        var_type="Psi4",
-        resam_type="finest",
-        interp_kind="cubic",
-        extrap_order=4,
-        r_ext=None,
-        ell_max=None,
-        pre_key=None,
-        modes_list=None,
-        crop=False,
-        centre=True,
-        key_ex=None,
-        save_as_ma=False,
-        compression_opts=None,
-        r_ext_factor=1,
-        debug=False,
-    ):
-        """Load the waveform mode data from an hdf file.
-
-        Parameters
-        ----------
-        extrap_order : int, optional
-                       For SpEC waveforms only. This is the order of extrapolation to use.
-
-        pre_key : str, optional
-                  A string containing the key of the group in
-                  the HDF file in which the modes` dataset exists.
-                  It defaults to `None`.
-        mode_numbers : list
-                       The mode numbers to load from the file.
-                       Each item in the list is a list that
-                       contains two integrer numbers, one for
-                       the mode index :math:`\\ell` and the
-                       other for the mode index :math:`m`.
-        crop : bool
-               Whether or not to crop the beginning of the input
-               waveform. If yes, the first :math:`t=r_{ext}`
-               length of data will be discarded.
-
-        Returns
-        -------
-        waveform_obj : 3d array
-                       Sets the three dimensional array `waveform.modes` that contains
-                       the required :math:`\\ell, m` modes.
-
-        Examples
-        --------
-        # Note
-        # Update this!
-        #>>> from waveformtools.waveforms import modes_array
-        #>>> wf = modes_array(label='wf', spin_weight=-2)
-        #>>> wf.data_dir = './'
-        #>>> wf.filename = 'wf_file.h5'
-        #>>> wf.modes_list = [[2, -2, -1, 0, 1, 2], [3, -3, 3]]
-        #>>> waveform.load_modes()
-        """
-
-        if debug is False:
-            wfs_nl = 1
-        if not data_dir:
-            data_dir = self.data_dir
-        else:
-            self.data_dir = data_dir
-
-        if not file_name:
-            file_name = self.file_name
-        else:
-            self.file_name = file_name
-
-        if not ell_max:
-            ell_max = self.ell_max
-        else:
-            self.ell_max = ell_max
-
-        if not label:
-            label = self.label
-
-        # if self.data_dir is not None:
-        # data_dir = self.data_dir
-
-        # if self.file_name is not None:
-        # file_name = self.file_name
-        message(f"Passing {data_dir}/{file_name}", message_verbosity=2)
-
-        if ftype == "generic":
-            dataIO.load_gen_data_from_disk(
-                self,
-                label,
-                data_dir,
-                file_name,
-                r_ext,
-                ell_max,
-                pre_key,
-                modes_list,
-                crop,
-                centre,
-                key_ex,
-                r_ext_factor,
-            )
-
-        elif (ftype) == "RIT" or (ftype == "GT"):
-            if var_type == "Psi4":
-                dataIO.load_RIT_Psi4_data_from_disk(
-                    wfa=self,
-                    data_dir=data_dir,
-                    resam_type=resam_type,
-                    interp_kind=interp_kind,
-                    ell_max=ell_max,
-                    modes_list=modes_list,
-                    crop=crop,
-                    centre=centre,
-                )
-            elif var_type == "Strain":
-                # message(file_name)
-                dataIO.load_RIT_Strain_data_from_disk(
-                    self,
-                    data_dir=data_dir,
-                    file_name=file_name,
-                    label=label,
-                    resam_type=resam_type,
-                    interp_kind=interp_kind,
-                    ell_max=ell_max,
-                    save_as_ma=save_as_ma,
-                    modes_list=modes_list,
-                    crop=crop,
-                    centre=centre,
-                    r_ext_factor=r_ext_factor,
-                    debug=debug,
-                )
-            else:
-                message(f"Data {ftype} {var_type} not supported yet!")
-                sys.exit(0)
-
-        elif ftype == "SpEC":
-            wfs_nl = dataIO.load_SpEC_data_from_disk(
-                self,
-                label,
-                data_dir,
-                file_name,
-                extrap_order,
-                r_ext,
-                ell_max,
-                centre,
-                modes_list,
-                save_as_ma,
-                resam_type,
-                interp_kind,
-                compression_opts,
-                r_ext_factor,
-                debug,
-            )
-        elif ftype == "SpECTRE":
-            dataIO.load_SpECTRE_data_from_disk(
-                self,
-                label=label,
-                data_dir=data_dir,
-                file_name=file_name,
-                r_ext=r_ext,
-                ell_max=ell_max,
-                centre=centre,
-                modes_list=modes_list,
-                save_as_ma=save_as_ma,
-                resam_type=resam_type,
-                kind=interp_kind,
-                compression_opts=compression_opts,
-                r_ext_factor=r_ext_factor,
-            )
-        else:
-            message(f"Data {ftype} {var_type} not supported yet!")
-            sys.exit(0)
-
-        return wfs_nl
-
-    def save_modes(
-        self,
-        ell_max=None,
-        pre_key=None,
-        key_format=None,
-        modes_to_save=None,
-        out_file_name="mp_new_modes.h5",
-        r_ext_factor=None,
-        compression_opts=0,
-        r_ext=None,
-    ):
-        """Save the waveform mode data to an hdf file.
-
-        Parameters
-        ----------
-        pre_key : str, optional
-                  A string containing the key of the group in
-                  the HDF file in which the modes` dataset exists.
-                  It defaults to `None`.
-        mode_numbers : list
-                       The mode numbers to load from the file.
-                       Each item in the list is a list that
-                       contains two integrer numbers, one for
-                       the mode index :math:`\\ell` and the
-                       other for the mode index :math:`m`.
-
-        Returns
-        -------
-        waveform_obj : 3d array
-                       Sets the three dimensional array `waveform.modes`
-                       that contains the required :math:`\\ell, m` modes.
-
-        Examples
-        --------
-        >>> from waveformtools.waveforms import waveform
-        >>> waveform.set_basedir('./')
-        >>> waveform.set_datadir('data/')
-        >>> mode_numbers = [[2, 2], [3, 3]]
-        >>> waveform.load_data(mode_numbers=mode_numbers)
-        """
-        # import dataIO
-        from waveformtools import dataIO
-
-        dataIO.save_modes_data_to_gen(
-            self,
-            ell_max=None,
-            pre_key=None,
-            key_format=None,
-            modes_to_save=None,
-            out_file_name="mp_new_modes.h5",
-            r_ext_factor=None,
-            compression_opts=0,
-            r_ext=None,
-        )
-
-    def resample(self, new_time_axis=None, new_delta_t=None):
-        """Resample all the waveform modes in time"""
-
-        raise NotImplementedError
-
-    def set_mode_data(self, ell_value, emm_value, data):
-        """Set the mode array data for the respective :math:`(\\ell, m)` mode.
-
-        Parameters
-        ----------
-        ell_value : int
-                    The :math:`\\ell` polar mode number.
-        emm_value : int
-                    The :math:`emm` azimuthal mode number.
-        data : 1d array
-               The array consisting of mode data for the requested mode.
-
-        Returns
-        -------
-        self.mode_data : modes_data
-                         The updated modes data.
-        """
-        # Compute the emm index given ell.
-        emm_index = emm_value + ell_value
-
-        # Set the mode data.
-        self._modes_data[ell_value, emm_index] = data
-
-    def to_spherical_array(self, grid_info, meth_info, spin_weight=None):
-        """Obtain the spherical array from the modes array.
-
-        Parameters
-        ----------
-        grid_info : cls instance
-                    An instance of the "spherical_grid" class
-                    to hold the grid info.
-        meth_info : cls instance
-                    An instance of the class waveformtools.diagnostics.method_info that
-                    provides information on what methods to use for integration.
-
-        Returns
-        -------
-        waveform_sp : spherical_array
-                      A member of the "spherical_array" class
-                      constructed from the given "modes_rray".
-        """
-
-        # Create a spherical array.
-        waveform_sp = spherical_array(label=self.label, grid_info=grid_info)
-
-        if spin_weight is None:
-            if self.spin_weight is not None:
-                spin_weight = self.spin_weight
-            else:
-                spin_weight = -2
-                self.spin_weight = spin_weight
-
-        spin_weight = abs(spin_weight)
-        waveform_sp.spin_weight = spin_weight
-        # Set the time-axis
-        try:
-            waveform_sp.time_axis = self.time_axis
-        except Exception as ex:
-            message(ex)
-            waveform_sp.frequency_axis = self.frequency_axis
-
-        # Get the coordinate meshgrid
-        theta, phi = grid_info.meshgrid
-
-        s1, s2 = theta.shape
-        s3 = self.data_len
-        sp_data = np.zeros((s1, s2, s3), dtype=np.complex128)
-
-        modes_list = [
-            item for item in self.modes_list if item[0] >= spin_weight
-        ]
-        for item in modes_list:
-            # Get modes.
-            ell, emm_list = item
-            # if ell<spin_weight:
-            # continue
-
-            for emm in emm_list:
-                # For every l, m
-                sp_data += np.multiply.outer(
-                    Yslm_vec(
-                        spin_weight,
-                        ell=ell,
-                        emm=emm,
-                        theta_grid=theta,
-                        phi_grid=phi,
-                    ),
-                    self.mode(ell, emm),
-                )
-                # message(sp_data)
-        # Set the data of the spherical array.
-        waveform_sp.data = sp_data
-        try:
-            waveform_sp.time_axis = self.time_axis
-        except Exception as ex:
-            message(ex)
-            waveform_sp.frequency_axis = self.frequency_axis
-        return waveform_sp
-
-    def trim(self, trim_upto_time=None):
-        """Trim the modes_array at the beginning and center about
-        the peak of the 2,2 mode.
-
-        Parameters
-        ----------
-        time : float
-               The time unit upto which to discard.
-
-        Returns
-        -------
-        Re-sets the `time_axis` and `modes_array` data.
-        """
-        if trim_upto_time is None:
-            trim_upto_time = self.r_ext
-
-        # Compute the start index
-        start = int(trim_upto_time / self.delta_t())
-
-        # Trim the time axis
-        self._time_axis = self.time_axis[start:]
-
-        # Trim the data
-        self._modes_data = self.modes_data[:, :, start:]
-
-        # Recenter the time axis
-        max_ind = np.argmax(np.absolute(self.mode(2, 2)))
-        self._time_axis = self.time_axis - self.time_axis[max_ind]
-
-    def to_frequency_basis(self):
-        """Compute the modes in frequency basis.
-
-        Returns
-        -------
-        waveform_tilde_modes : modes_array
-                               A modes_array containing the modes
-                               in frequency basis.
-        """
-
-        # Create a new modes array
-        waveform_tilde_modes = modes_array(
-            label=f"{self.label} -> frequency_domain"
-        )
-        waveform_tilde_modes.create_modes_array(
-            ell_max=self.ell_max, data_len=self.data_len
-        )
-
-        from waveformtools.transforms import compute_fft
-
-        for mode in self.modes_list:
-            # Extrapolate every mode
-
-            # Ge the ell value
-            ell_value, emm_list = mode
-
-            for emm_value in emm_list:
-                freq_axis, freq_data = compute_fft(
-                    self.mode(ell_value, emm_value), self.delta_t()
-                )
-
-                waveform_tilde_modes.set_mode_data(
-                    ell_value, emm_value, freq_data
-                )
-
-        waveform_tilde_modes.frequency_axis = freq_axis
-        waveform_tilde_modes.ell_max = self.ell_max
-        waveform_tilde_modes.modes_list = self.modes_list
-        return waveform_tilde_modes
-
-    def to_time_basis(self):
-        """Compute the modes in time basis.
-
-        Returns
-        -------
-        waveform_modes: modes_array
-                        A modes_array containing the modes
-                        in frequency basis.
-        """
-
-        # Create a new modes array
-        waveform_modes = modes_array(label=f"{self.label} -> time_domain")
-        waveform_modes.create_modes_array(
-            ell_max=self.ell_max, data_len=self.data_len
-        )
-
-        from waveformtools.transforms import compute_ifft
-
-        for mode in self.modes_list:
-            # Extrapolate every mode
-
-            # Ge the ell value
-            ell_value, emm_list = mode
-
-            for emm_value in emm_list:
-                time_axis, time_data = compute_ifft(
-                    self.mode(ell_value, emm_value), self.delta_f
-                )
-
-                waveform_modes.set_mode_data(ell_value, emm_value, time_data)
-
-        try:
-            maxloc = np.argmax(np.absolute(waveform_modes.mode(2, 2)))
-        except Exception as ex:
-            message(ex)
-            maxloc = 0
-
-        maxtime = time_axis[maxloc]
-
-        waveform_modes.time_axis = time_axis - maxtime
-
-        return waveform_modes
-
-    def extrap_to_inf(
-        self,
-        mass=1,
-        spin=None,
-        modes_list="all",
-        method="SIO",
-        r_ext_factor=1,
-        diff_method="CS",
-        diff_degree=24,
-    ):
-        """Extrapolate the :math:`\\Psi_4` modes to infinity
-        using the perturbative improved second order method.
-
-        Parameters
-        ----------
-        mass : float
-               The effective total mass of the system.
-        spin : float
-               The effective spin of the system.
-        modes : modes array, optional
-                The modes to extrapolate. Defaults
-                to `all` if not specified.
-        method : str
-                 The method to use for extrapolation. The available methods are:
-
-        +------------+--------------------------------------+
-        | Method str | Name                                 |
-        +------------+--------------------------------------+
-        |'FO'        | First order                          |
-        |'SO'        | Second order                         |
-        |'SIO'       | Second improved order                |
-        |'NM'        | Numerical method (not ready yet)     |
-        +------------+--------------------------------------+
-
-        Returns
-        -------
-        waveform_inf_modes : modes array
-                             A new modes array that contains the extrapolated modes.
-        """
-
-        from functools import partial
-
-        # Prepare the extrapolating method.
-        if method == "SIO":
-            from waveformtools.extrapolate import (
-                waveextract_to_inf_perturbative_twop5_order,
-            )
-
-            extrap_method = partial(
-                waveextract_to_inf_perturbative_twop5_order,
-                delta_t=self.delta_t(),
-                areal_radius=self.r_ext,
-                mass=mass,
-                spin=spin,
-                method=diff_method,
-                degree=diff_degree,
-            )
-
-        if method == "SO":
-            from waveformtools.extrapolate import (
-                waveextract_to_inf_perturbative_two_order,
-            )
-
-            extrap_method = partial(
-                waveextract_to_inf_perturbative_two_order,
-                delta_t=self.delta_t(),
-                areal_radius=self.r_ext,
-                mass=mass,
-                spin=spin,
-            )
-
-        if method == "FO":
-            from waveformtools.extrapolate import (
-                waveextract_to_inf_perturbative_one_order,
-            )
-
-            extrap_method = partial(
-                waveextract_to_inf_perturbative_one_order,
-                u_ret=self.time_axis,
-                areal_radius=self.r_ext,
-                mass=mass,
-            )
-
-        if method == "NM":
-            message("This method is not available yet! ")
-
-        # Prepare the modes to be extrapolated.
-        if modes_list == "all":
-            modes_list = construct_mode_list(self.ell_max, self.spin_weight)
-
-        # Create a mode array for the extrapolated waveform.
-        extrap_wf = modes_array(
-            label=f"{self.label} -> rPsi4_inf",
-            modes_list=self.modes_list,
-            ell_max=self.ell_max,
-            r_ext=self.r_ext,
-        )
-
-        extrap_wf.create_modes_array(
-            ell_max=self.ell_max, data_len=self.data_len
-        )
-
-        # Retain the time axis.
-        extrap_wf.time_axis = self.time_axis
-        for mode in modes_list:
-            # Extrapolate every mode
-
-            # Ge the ell value
-            ell_value, emm_list = mode
-
-            for emm_value in emm_list:
-                # For every emm value
-                message(f"Processing l{ell_value}, m{emm_value}")
-                # Compute rPsi4_lm
-                mode_data = r_ext_factor * self.mode(ell_value, emm_value)
-
-                # Extrapolate
-                # import ipdb; ipdb.set_trace()
-                extrap_mode_data = extrap_method(rPsi4_rlm=mode_data)
-
-                # Assign data to new modes array
-                extrap_wf.set_mode_data(ell_value, emm_value, extrap_mode_data)
-
-        message("Done!")
-        return extrap_wf
-
-    def supertranslate(self, supertransl_alpha_modes, grid_info, order=4):
-        """Supertranslate the :math:`\\Psi_{4\\ell m}` waveform modes, give the,
-        the supertranslation parameter and the order.
-
-        Parameters
-        ----------
-        supertransl_alpha_modes : modes_array
-                                  The modes_array containing the supertranslation
-                                  mode coefficients.
-        grid_info : grids class instance
-                    The class instance that contains
-                    the properties of the spherical grid
-                    using which the computations are carried out.
-        order : int
-                The number of terms to use to approximate the supertranslation.
-
-        Returns
-        -------
-        Psi4_supertransl : modes_array
-                           A class instance containg the
-                           modes of the supertranslated
-                           waveform :math:`\\Psi_4`.
-        """
-
-        import BMS
-
-        ell_max = self.ell_max
-        # Step 0: Get the grid properties for integrations
-
-        # Compute the meshgrid for theta and phi.
-        theta, phi = grid_info.meshgrid
-        # theta
-        # Step 1: get the grid function for supertranslation parameter
-        supertransl_alpha_sphere = BMS.compute_supertransl_alpha(
-            supertransl_alpha_modes, theta, phi
-        )
-
-        # The supertranslation is carried out in frequency space.
-        # Step 2: get the FFT of the mode coefficients of Psi4
-        Psi4_tilde_modes = self.to_frequency_basis()
-
-        # Get the 2d angular frequency array
-        omega_axis_2d = Psi4_tilde_modes.omega
-
-        # Construct the supertranslation factor
-        supertransl_factor = np.sum(
-            np.array(
-                [
-                    np.power(
-                        (-1j * omega_axis_2d * supertransl_alpha_sphere), index
-                    )
-                    for index in range(order)
-                ]
-            ),
-            axis=0,
-        )
-
-        # Multiply with the fourier modes.
-        supertransl_spherical_factor = Psi4_tilde_modes.multiply(
-            supertransl_factor
-        )
-
-        # Reconstruct the modes
-
-        # Check!
-        supertransl_spherical_grid = np.zeros(
-            supertransl_spherical_factor.shape, dtype=np.complex128
-        )
-
-        for ell_value in range(ell_max + 1):
-            for emm_value in range(-ell_value, ell_value + 1):
-                # Multiply with the SWSH basis.
-                supertransl_spherical_grid += (
-                    supertransl_spherical_factor
-                    * Yslm_vec(
-                        spin_weight=-2,
-                        ell=ell_value,
-                        emm=emm_value,
-                        theta=theta,
-                        phi=phi,
-                    )
-                )
-
-                # Step 3: Reconstruct the function on the sphere
-
-        # Create a spherical_array to hold the supertranslated waveform
-        supertransl_spherical_waveform = spherical_array(grid_info=grid_info)
-
-        # Set the data.
-        supertransl_spherical_waveform.data = supertransl_spherical_grid
-
-        # Get modes_array from spherical_array
-        Psi4_supertransl_modes = supertransl_spherical_waveform.to_modes_array(
-            ell_max=ell_max
-        )
-
-        return Psi4_supertransl_modes
-
-    def boost(self, conformal_factor, grid_info=None):
-        """Boost the waveform given the unboosted waveform and the boost conformal factor.
-
-        Parameters
-        ----------
-        conformal_factor : 2d array
-                           The conformal factor for the Lorentz transformation.
-                           It may be a single floating point number or an array
-                           on a spherical grid. The array will be of dimensions
-                           [ntheta, nphi]
-
-        Returns
-        -------
-        boosted_waveform : spherical_array
-                           The class instance `spherical_array`
-                           that contains the boosted waveform.
-        """
-
-        from waveformtools.grids import spherical_grid
-
-        # Construct a spherical grid.
-        if grid_info is None:
-            grid_info = spherical_grid()
-
-        # Get spherical array from modes.
-        unboosted_waveform = self.to_spherical_array(grid_info)
-
-        boosted_waveform_data = unboosted_waveform.boost(conformal_factor)
-
-        # Construct a 2d waveform array object
-        boosted_waveform = spherical_array(
-            grid_info=unboosted_waveform.grid_info,
-            data=np.array(boosted_waveform_data),
-        )
-        boosted_waveform.label = "boosted"
-
-        # Get modes from spherical data.
-        # boosted_waveform_modes = boosted_waveform.to_modes_array()
-
-        # return boosted_waveform_modes
-        return boosted_waveform
-
-    def get_strain_from_psi4(self, omega0="auto"):
-        """Get the strain `modes_array` from :math:`\\Psi_4` by
-        fixed frequency integration.
-
-        Parameters
-        ----------
-        omega0 : float, optional
-                 The lower cutoff angular frequency for FFI.
-                 By default, it computes this from the mode data.
-
-        Returns
-        -------
-        strain_waveform : modes_array
-                          The computed strain modes.
-        """
-
-        # Initialize a mode array for strain.
-        strain_waveform = modes_array(
-            label="{} strain from Psi4".format(self.label),
-            r_ext=self.r_ext,
-            ell_max=8,
-            modes_list=self.modes_list,
-        )
-
-        strain_waveform.time_axis = self.time_axis
-        strain_waveform.ell_max = self.ell_max
-
-        data_len = self.data_len
-
-        strain_waveform.create_modes_array(
-            ell_max=self.ell_max, data_len=data_len
-        )
-
-        # Integrate,
-        from waveformtools.integrate import fixed_frequency_integrator
-        from waveformtools.waveformtools import (
-            get_starting_angular_frequency as sang_f,
-        )
-
-        omega_st = omega0
-        for item in self.modes_list[:]:
-            ell, emm_list = item
-            for emm in emm_list:
-                mode_data = self.mode(ell, emm)
-                if omega0 == "auto":
-                    omega_st = (
-                        abs(sang_f(mode_data, delta_t=self.delta_t())) / 10
-                    )
-                strain_mode_data, _ = fixed_frequency_integrator(
-                    udata_time=mode_data,
-                    delta_t=self.delta_t(),
-                    omega0=omega_st,
-                    order=2,
-                )
-                strain_waveform.set_mode_data(ell, emm, data=strain_mode_data)
-
-        return strain_waveform
-
-    def get_news_from_psi4(self, omega0="auto"):
-        """Get the News `modes_array` from :math:`\\Psi_4` by
-        fixed frequency integration.
-
-        Parameters
-        ----------
-        omega0 : float, optional
-                 The lower cutoff angular frequency for FFI.
-                 By default, it computes this as one tenth of
-                 the starting frequency of the mode data.
-
-        Returns
-        -------
-        news_waveform : modes_array
-                        The computed strain modes.
-        """
-
-        # Initialize a mode array for strain.
-        # news_waveform = modes_array(label=f'{self.label} news from Psi4', r_ext=500, ell_max=8, modes_list=self.modes_list)
-        news_waveform = modes_array(
-            label="{} news from Psi4".format(self.label),
-            r_ext=500,
-            ell_max=8,
-            modes_list=self.modes_list,
-        )
-
-        news_waveform.time_axis = self.time_axis
-        news_waveform.ell_max = self.ell_max
-
-        data_len = self.data_len
-
-        news_waveform.create_modes_array(
-            ell_max=self.ell_max, data_len=data_len
-        )
-
-        # Integrate,
-        from waveformtools.integrate import fixed_frequency_integrator
-        from waveformtools.waveformtools import (
-            get_starting_angular_frequency as sang_f,
-        )
-
-        omega_st = omega0
-        for item in self.modes_list[:]:
-            ell, emm_list = item
-            for emm in emm_list:
-                mode_data = self.mode(ell, emm)
-                if omega0 == "auto":
-                    omega_st = (
-                        abs(sang_f(mode_data, delta_t=self.delta_t())) / 10
-                    )
-                news_mode_data, _ = fixed_frequency_integrator(
-                    udata_time=mode_data,
-                    delta_t=self.delta_t(),
-                    omega0=omega_st,
-                    order=1,
-                )
-                news_waveform.set_mode_data(ell, emm, data=news_mode_data)
-
-        return news_waveform
-
-    def taper(self, zeros="auto"):
-        """Taper a waveform at both ends and insert zeros if needed
-
-        Parameters
-        ----------
-        zeros : int
-                The number of zeros to add at rach end
-
-        Returns
-        -------
-        tapered_modes : modes_array
-                        Modes array with tapered mode data.
-        """
-
-        from waveformtools.waveformtools import taper
-
-        if zeros == "auto":
-            # Decide the number of zeros
-            data_len = self.data_len
-
-            nearest_power = int(np.log(data_len) / np.log(2))
-            req_len = np.power(2, nearest_power + 1)
-            zeros = req_len - data_len
-            message("num_zeros", zeros)
-
-        # New modes array.
-
-        tapered_modes = None
-
-        for item in self.modes_list[:]:
-            ell, emm_list = item
-            for emm in emm_list:
-                input_data_re = self.mode(ell, emm).real
-                input_data_im = self.mode(ell, emm).imag
-
-                tapered_data_re = taper(input_data_re, zeros=zeros)
-                tapered_data_im = taper(input_data_im, zeros=zeros)
-
-                # tapered_data_re = taper_tanh(input_data_re, delta_t=self.delta_t())
-                # tapered_data_im = taper_tanh(input_data_im, delta_t=self.delta_t())
-
-                new_data_len = len(tapered_data_re)
-
-                if tapered_modes is None:
-                    tapered_modes = modes_array(
-                        label="tapered {}".format(self.label),
-                        r_ext=self.r_ext,
-                        modes_list=self.modes_list,
-                        ell_max=self.ell_max,
-                    )
-
-                    tapered_modes.create_modes_array(
-                        ell_max=self.ell_max, data_len=new_data_len
-                    )
-                tapered_data = tapered_data_re + 1j * tapered_data_im
-
-                # message(len(tapered_data_re))
-                tapered_modes.set_mode_data(ell, emm, data=tapered_data)
-
-        # Set the time axis
-        new_time_axis = np.arange(
-            0, new_data_len * self.delta_t(), self.delta_t()
-        )
-
-        tapered_modes.time_axis = new_time_axis
-
-        # Recenter the modes.
-        tapered_modes.trim(trim_upto_time=0)
-
-        return tapered_modes
-
-    def taper_tanh(
-        self, time_axis=None, zeros="auto", duration=10, sides="both"
-    ):
-        """Taper a waveform at both ends and insert zeros if needed
-
-        Parameters
-        ----------
-        zeros : int
-                The number of zeros to add at rach end
-
-        Returns
-        -------
-        tapered_modes : modes_array
-                        Modes array with tapered mode data.
-        """
+		Returns
+		-------
+		mode_data:	array
+														The array of the requested mode.
+		"""
+
+		emm_index = ell + emm
+
+		return self.modes_data[ell, emm_index, :]
+
+	@property
+	def time_axis(self):
+		"""The time axis"""
+		return np.array(self._time_axis)
+
+	@time_axis.setter
+	def time_axis(self, time_axis):
+		self._time_axis = time_axis
+
+	@property
+	def modes_data(self):
+		"""The modes array"""
+		return np.array(self._modes_data)
+
+	@modes_data.setter
+	def modes_data(self, modes_data):
+		self._modes_data = modes_data
+
+	def create_modes_array(self, ell_max=None, data_len=None):
+		"""Create a modes array and initialize it with zeros.
+
+		Parameters
+		----------
+		ell_max:	int
+														The maximum :math:`\\ell` value of the modes.
+		data_len:	int
+														The number of points along the third (time / frequency) axis.
+
+		Returns
+		-------
+		self.modes_array:	modes_array
+																						sets the `self.modes_array` attribute.
+		"""
+		import datetime
+		import time
+
+		# Check ell_max
+		if ell_max is None:
+			try:
+				ell_max = self.ell_max
+			except Exception as ex:
+				message(ex)
+				raise NameError("Please supply ell_max")
+
+		if data_len is None:
+			try:
+				data_len = self.data_len
+			except Exception as ex:
+				message(ex)
+				raise NameError("Please supply data_len")
+
+		if self.modes_list is None:
+			self.modes_list = construct_mode_list(ell_max=ell_max, spin_weight=self.spin_weight)
+
+		# self.modes_data = np.zeros([ell_max + 1, 2 * (ell_max + 1) + 1, data_len], dtype=np.complex128)
+		self.modes_data = np.zeros((ell_max + 1, 2 * (ell_max + 1) + 1, data_len), dtype=np.complex128)
+
+		# Set the time metadata
+		time_now = time.localtime()
+		time_now = time.strftime("%H:%M:%S", time_now)
+
+		date_now = str(datetime.date.today())
+
+		if self.time is None:
+			# Assign time and date stamp if it doesnt exist
+			self.time = time_now
+			self.date = date_now
+
+	@property
+	def data_len(self):
+		"""Returns the length of the time/frequency axis.
+
+		Returns
+		-------
+		data_len:	int
+														The length of the time/frequency axis.
+		"""
+
+		try:
+			data_len = len(self.time_axis)
+
+		except Exception as ex:
+			message(ex)
+			data_len = len(self.frequency_axis)
+
+		return data_len
+
+	@data_len.setter
+	def data_len(self, data_len):
+		self._data_len = data_len
+
+	def delta_t(self, value=None):
+		"""Sets and returns the value of time stepping :math:`dt`.
+
+		Parameters
+		----------
+		value : float, optional
+										The value of :math:`dt`
+										to set to the attribute.
+
+		Returns
+		-------
+		self.delta_t:	float
+																		Sets the attribute.
+		"""
+
+		if not value:
+			try:
+				delta_t = self.time_axis[1] - self.time_axis[0]
+			except Exception as ex:
+				message("Please input the value of `delta_t` or supply the `time_axis` to the waveform.", ex)
+		else:
+			delta_t = value
+
+		return delta_t
+
+	@property
+	def delta_f(self, value=None):
+		"""Sets and returns the value of frequency stepping :math:`df`.
+
+		Parameters
+		----------
+		value:	float, optional
+										The value of :math:`df`
+										to set to the attribute.
+
+		Returns
+		-------
+		delta_f:	float
+														Sets the attribute.
+		"""
+
+		# if not self.delta_t:
+		if not value:
+			try:
+				delta_f = self.frequency_axis[1] - self.frequency_axis[0]
+			except Exception as ex:
+				message("Please input the value of `delta_f` or supply the `frequency_axis` to the waveform.", ex)
+		else:
+			delta_f = value
+
+		return delta_f
+
+	def load_modes(
+		self,
+		label=None,
+		data_dir=None,
+		file_name=None,
+		ftype="generic",
+		var_type="Psi4",
+		resam_type="finest",
+		interp_kind="cubic",
+		extrap_order=4,
+		r_ext=None,
+		ell_max=None,
+		pre_key=None,
+		modes_list=None,
+		crop=False,
+		centre=True,
+		key_ex=None,
+		save_as_ma=False,
+		compression_opts=None,
+		r_ext_factor=1,
+		debug=False,
+	):
+		"""Load the waveform mode data from an hdf file.
+
+		Parameters
+		----------
+		extrap_order:	int, optional
+																																										For SpEC waveforms only. This is the order of extrapolation to use.
+
+		pre_key:	str, optional
+																																		A string containing the key of the group in
+																																		the HDF file in which the modes` dataset exists.
+																																		It defaults to `None`.
+		mode_numbers:	list
+																																										The mode numbers to load from the file.
+																																										Each item in the list is a list that
+																		contains two integrer numbers, one for
+																																										the mode index :math:`\\ell` and the
+																																										other for the mode index :math:`m`.
+		crop:	bool
+										Whether or not to crop the beginning of the input
+										waveform. If yes, the first :math:`t=r_{ext}`
+																										length of data will be discarded.
+
+		Returns
+		-------
+		waveform_obj:	3d array
+																																										Sets the three dimensional array `waveform.modes` that contains
+																		the required :math:`\\ell, m` modes.
+
+		Examples
+		--------
+		# Note
+		# Update this!
+		#>>> from waveformtools.waveforms import waveform
+		#>>> waveform.set_basedir('./')
+		#>>> waveform.set_datadir('data/')
+		#>>> mode_numbers = [[2, 2], [3, 3]]
+		#>>> waveform.load_data(mode_numbers=mode_numbers)
+		"""
+
+		if debug is False:
+			wfs_nl = 1
+		if not data_dir:
+			data_dir = self.data_dir
+		else:
+			self.data_dir = data_dir
+
+		if not file_name:
+			file_name = self.file_name
+		else:
+			self.file_name = file_name
+
+		if not ell_max:
+			ell_max = self.ell_max
+		else:
+			self.ell_max = ell_max
+
+		if not label:
+			label = self.label
+
+		# if self.data_dir is not None:
+		# data_dir = self.data_dir
+
+		# if self.file_name is not None:
+		# file_name = self.file_name
+		message(f"Passing {data_dir}/{file_name}", message_verbosity=2)
+
+		if ftype == "generic":
+			dataIO.load_gen_data_from_disk(
+				self,
+				label,
+				data_dir,
+				file_name,
+				r_ext,
+				ell_max,
+				pre_key,
+				modes_list,
+				crop,
+				centre,
+				key_ex,
+				r_ext_factor,
+			)
+
+		elif (ftype) == "RIT" or (ftype == "GT"):
+			if var_type == "Psi4":
+				dataIO.load_RIT_Psi4_data_from_disk(
+					wfa=self,
+					data_dir=data_dir,
+					resam_type=resam_type,
+					interp_kind=interp_kind,
+					ell_max=ell_max,
+					modes_list=modes_list,
+					crop=crop,
+					centre=centre,
+				)
+			elif var_type == "Strain":
+				# message(file_name)
+				dataIO.load_RIT_Strain_data_from_disk(
+					self,
+					data_dir=data_dir,
+					file_name=file_name,
+					label=label,
+					resam_type=resam_type,
+					interp_kind=interp_kind,
+					ell_max=ell_max,
+					save_as_ma=save_as_ma,
+					modes_list=modes_list,
+					crop=crop,
+					centre=centre,
+					r_ext_factor=r_ext_factor,
+					debug=debug,
+				)
+			else:
+				message(f"Data {ftype} {var_type} not supported yet!")
+				sys.exit(0)
+
+		elif ftype == "SpEC":
+			wfs_nl = dataIO.load_SpEC_data_from_disk(
+				self,
+				label,
+				data_dir,
+				file_name,
+				extrap_order,
+				r_ext,
+				ell_max,
+				centre,
+				modes_list,
+				save_as_ma,
+				resam_type,
+				interp_kind,
+				compression_opts,
+				r_ext_factor,
+				debug,
+			)
+		elif ftype == "SpECTRE":
+			dataIO.load_SpECTRE_data_from_disk(
+				self,
+				label=label,
+				data_dir=data_dir,
+				file_name=file_name,
+				r_ext=r_ext,
+				ell_max=ell_max,
+				centre=centre,
+				modes_list=modes_list,
+				save_as_ma=save_as_ma,
+				resam_type=resam_type,
+				kind=interp_kind,
+				compression_opts=compression_opts,
+				r_ext_factor=r_ext_factor,
+			)
+		else:
+			message(f"Data {ftype} {var_type} not supported yet!")
+			sys.exit(0)
+
+		return wfs_nl
+
+	def save_modes(
+		self,
+		ell_max=None,
+		pre_key=None,
+		key_format=None,
+		modes_to_save=None,
+		out_file_name="mp_new_modes.h5",
+		r_ext_factor=None,
+		compression_opts=0,
+		r_ext=None,
+	):
+		"""Save the waveform mode data to an hdf file.
+
+		Parameters
+		----------
+		pre_key:	str, optional
+																																		A string containing the key of the group in
+																																		the HDF file in which the modes` dataset exists.
+																																		It defaults to `None`.
+		mode_numbers:	list
+																																										The mode numbers to load from the file.
+																																										Each item in the list is a list that
+																																										contains two integrer numbers, one for
+																		the mode index :math:`\\ell` and the
+																		other for the mode index :math:`m`.
+
+		Returns
+		-------
+		waveform_obj:	3d array
+																																										Sets the three dimensional array `waveform.modes`
+																																										that contains the required :math:`\\ell, m` modes.
+
+		Examples
+		--------
+		>>> from waveformtools.waveforms import waveform
+		>>> waveform.set_basedir('./')
+		>>> waveform.set_datadir('data/')
+		>>> mode_numbers = [[2, 2], [3, 3]]
+		>>> waveform.load_data(mode_numbers=mode_numbers)
+		"""
+		# import dataIO
+		from waveformtools import dataIO
+
+		dataIO.save_modes_data_to_gen(
+			self,
+			ell_max=None,
+			pre_key=None,
+			key_format=None,
+			modes_to_save=None,
+			out_file_name="mp_new_modes.h5",
+			r_ext_factor=None,
+			compression_opts=0,
+			r_ext=None,
+		)
+
+	def resample(self, new_time_axis=None, new_delta_t=None):
+		"""Resample all the waveform modes in time"""
+
+		raise NotImplementedError
+
+	def set_mode_data(self, ell_value, emm_value, data):
+		"""Set the mode array data for the respective :math:`(\\ell, m)` mode.
+
+		Parameters
+		----------
+		ell_value:	int
+																																		The :math:`\\ell` polar mode number.
+		emm_value:	int
+																																		The :math:`emm` azimuthal mode number.
+		data:	1d array
+																										The array consisting of mode data for the requested mode.
+
+		Returns
+		-------
+		self.mode_data:	modes_data
+																		The updated modes data.
+		"""
+		# Compute the emm index given ell.
+		emm_index = emm_value + ell_value
+
+		# Set the mode data.
+		self._modes_data[ell_value, emm_index] = data
+
+	def to_spherical_array(self, grid_info, meth_info, spin_weight=None):
+		"""Obtain the spherical array from the modes array.
+
+		Parameters
+		----------
+
+		grid_info:	cls instance
+														An instance of the "spherical_grid" class
+																																		to hold the grid info.
+		meth_info:	cls instance
+														An instance of the class waveformtools.diagnostics.method_info that
+														provides information on what methods to use for integration.
+
+		Returns
+		-------
+		waveform_sp:	spherical_array
+																		A member of the "spherical_array" class
+																																										constructed from the given "modes_rray".
+		"""
+
+		# Create a spherical array.
+		waveform_sp = spherical_array(label=self.label, grid_info=grid_info)
+
+		if spin_weight is None:
+			if self.spin_weight is not None:
+				spin_weight = self.spin_weight
+			else:
+				spin_weight = -2
+				self.spin_weight = spin_weight
+
+		spin_weight = abs(spin_weight)
+		waveform_sp.spin_weight = spin_weight
+		# Set the time-axis
+		try:
+			waveform_sp.time_axis = self.time_axis
+		except Exception as ex:
+			message(ex)
+			waveform_sp.frequency_axis = self.frequency_axis
+
+		# Get the coordinate meshgrid
+		theta, phi = grid_info.meshgrid
+
+		s1, s2 = theta.shape
+		s3 = self.data_len
+		sp_data = np.zeros((s1, s2, s3), dtype=np.complex128)
+
+		modes_list = [item for item in self.modes_list if item[0] >= spin_weight]
+		for item in modes_list:
+			# Get modes.
+			ell, emm_list = item
+			# if ell<spin_weight:
+			# continue
+
+			for emm in emm_list:
+				# For every l, m
+				sp_data += np.multiply.outer(
+					Yslm_vec(spin_weight, ell=ell, emm=emm, theta_grid=theta, phi_grid=phi), self.mode(ell, emm)
+				)
+				# message(sp_data)
+		# Set the data of the spherical array.
+		waveform_sp.data = sp_data
+		try:
+			waveform_sp.time_axis = self.time_axis
+		except Exception as ex:
+			message(ex)
+			waveform_sp.frequency_axis = self.frequency_axis
+		return waveform_sp
+
+	def trim(self, trim_upto_time=None):
+		"""Trim the modes_array at the beginning and center about
+		the peak of the 2,2 mode.
+
+		Parameters
+		----------
+		time:	float
+										The time unit upto which to discard.
+
+		Returns
+		-------
+		Re-sets the `time_axis` and `modes_array` data.
+		"""
+		if trim_upto_time is None:
+			trim_upto_time = self.r_ext
+
+		# Compute the start index
+		start = int(trim_upto_time / self.delta_t())
+
+		# Trim the time axis
+		self._time_axis = self.time_axis[start:]
+
+		# Trim the data
+		self._modes_data = self.modes_data[:, :, start:]
+
+		# Recenter the time axis
+		max_ind = np.argmax(np.absolute(self.mode(2, 2)))
+		self._time_axis = self.time_axis - self.time_axis[max_ind]
+
+	def to_frequency_basis(self):
+		"""Compute the modes in frequency basis.
+
+		Returns
+		-------
+		waveform_tilde_modes:	modes_array
+																																																										A modes_array containing the modes
+																										in frequency basis.
+		"""
+
+		# Create a new modes array
+		waveform_tilde_modes = modes_array(label=f"{self.label} -> frequency_domain")
+		waveform_tilde_modes.create_modes_array(ell_max=self.ell_max, data_len=self.data_len)
+
+		from waveformtools.transforms import compute_fft
+
+		for mode in self.modes_list:
+			# Extrapolate every mode
+
+			# Ge the ell value
+			ell_value, emm_list = mode
+
+			for emm_value in emm_list:
+				freq_axis, freq_data = compute_fft(self.mode(ell_value, emm_value), self.delta_t())
+
+				waveform_tilde_modes.set_mode_data(ell_value, emm_value, freq_data)
+
+		waveform_tilde_modes.frequency_axis = freq_axis
+		waveform_tilde_modes.ell_max = self.ell_max
+		waveform_tilde_modes.modes_list = self.modes_list
+		return waveform_tilde_modes
+
+	def to_time_basis(self):
+		"""Compute the modes in time basis.
+
+		Returns
+		-------
+		waveform_modes:	modes_array
+																																										A modes_array containing the modes
+																		in frequency basis.
+		"""
+
+		# Create a new modes array
+		waveform_modes = modes_array(label=f"{self.label} -> time_domain")
+		waveform_modes.create_modes_array(ell_max=self.ell_max, data_len=self.data_len)
+
+		from waveformtools.transforms import compute_ifft
+
+		for mode in self.modes_list:
+			# Extrapolate every mode
+
+			# Ge the ell value
+			ell_value, emm_list = mode
+
+			for emm_value in emm_list:
+				time_axis, time_data = compute_ifft(self.mode(ell_value, emm_value), self.delta_f)
+
+				waveform_modes.set_mode_data(ell_value, emm_value, time_data)
+
+		try:
+			maxloc = np.argmax(np.absolute(waveform_modes.mode(2, 2)))
+		except Exception as ex:
+			message(ex)
+			maxloc = 0
+
+		maxtime = time_axis[maxloc]
+
+		waveform_modes.time_axis = time_axis - maxtime
+
+		return waveform_modes
+
+	def extrap_to_inf(
+		self, mass=1, spin=None, modes_list="all", method="SIO", r_ext_factor=1, diff_method="CS", diff_degree=24
+	):
+		"""Extrapolate the :math:`\\Psi_4` modes to infinity
+		using the perturbative improved second order method.
+
+		Parameters
+		----------
+		mass:		float
+														The effective total mass of the system.
+		spin:		float
+														The effective spin of the system.
+		modes:		modes array, optional
+														The modes to extrapolate. Defaults
+														to `all` if not specified.
+		method:		str
+														The method to use for extrapolation. The available methods are:
+
+		+------------+--------------------------------------+
+		| Method str | Name									|
+		+------------+--------------------------------------+
+		|'FO'		 | First order							|
+		|'SO'		 | Second order							|
+		|'SIO'		 | Second improved order				|
+		|'NM'		 | Numerical method (not ready yet)		|
+		+------------+--------------------------------------+
+
+		Returns
+		-------
+		waveform_inf_modes: modes array
+																						A new modes array that contains the extrapolated modes.
+		"""
+
+		from functools import partial
+
+		# Prepare the extrapolating method.
+		if method == "SIO":
+			from waveformtools.extrapolate import (
+				waveextract_to_inf_perturbative_twop5_order,
+			)
+
+			extrap_method = partial(
+				waveextract_to_inf_perturbative_twop5_order,
+				delta_t=self.delta_t(),
+				areal_radius=self.r_ext,
+				mass=mass,
+				spin=spin,
+				method=diff_method,
+				degree=diff_degree,
+			)
+
+		if method == "SO":
+			from waveformtools.extrapolate import (
+				waveextract_to_inf_perturbative_two_order,
+			)
+
+			extrap_method = partial(
+				waveextract_to_inf_perturbative_two_order,
+				delta_t=self.delta_t(),
+				areal_radius=self.r_ext,
+				mass=mass,
+				spin=spin,
+			)
+
+		if method == "FO":
+			from waveformtools.extrapolate import (
+				waveextract_to_inf_perturbative_one_order,
+			)
+
+			extrap_method = partial(
+				waveextract_to_inf_perturbative_one_order, u_ret=self.time_axis, areal_radius=self.r_ext, mass=mass
+			)
+
+		if method == "NM":
+			message("This method is not available yet! ")
+
+		# Prepare the modes to be extrapolated.
+		if modes_list == "all":
+			modes_list = construct_mode_list(self.ell_max, self.spin_weight)
+
+		# Create a mode array for the extrapolated waveform.
+		extrap_wf = modes_array(
+			label=f"{self.label} -> rPsi4_inf", modes_list=self.modes_list, ell_max=self.ell_max, r_ext=self.r_ext
+		)
+
+		extrap_wf.create_modes_array(ell_max=self.ell_max, data_len=self.data_len)
+
+		# Retain the time axis.
+		extrap_wf.time_axis = self.time_axis
+		for mode in modes_list:
+			# Extrapolate every mode
+
+			# Ge the ell value
+			ell_value, emm_list = mode
+
+			for emm_value in emm_list:
+				# For every emm value
+				message(f"Processing l{ell_value}, m{emm_value}")
+				# Compute rPsi4_lm
+				mode_data = r_ext_factor * self.mode(ell_value, emm_value)
+
+				# Extrapolate
+				# import ipdb; ipdb.set_trace()
+				extrap_mode_data = extrap_method(rPsi4_rlm=mode_data)
+
+				# Assign data to new modes array
+				extrap_wf.set_mode_data(ell_value, emm_value, extrap_mode_data)
+
+		message("Done!")
+		return extrap_wf
+
+	def supertranslate(self, supertransl_alpha_modes, grid_info, order=4):
+		"""Supertranslate the :math:`\\Psi_{4\\ell m}` waveform modes, give the,
+		the supertranslation parameter and the order.
+
+		Parameters
+		----------
+		supertransl_alpha_modes:	 modes_array
+																																																																		The modes_array containing the
+																																																																		supertranslation mode coefficients.
+		grid_info:	class instance
+														The class instance that contains
+																																		the properties of the spherical grid
+																																		using which the computations are carried out.
+		order:		int
+																																		The number of terms to use to approximate the supertranslation.
+
+		Returns
+		-------
+		Psi4_supertransl:	modes_array
+																																																		A class instance containg the
+																																																		modes of the supertranslated
+																																																		waveform :math:`\\Psi_4`.
+		"""
+
+		import BMS
+
+		ell_max = self.ell_max
+		# Step 0: Get the grid properties for integrations
+
+		# Compute the meshgrid for theta and phi.
+		theta, phi = grid_info.meshgrid
+		# theta
+		# Step 1: get the grid function for supertranslation parameter
+		supertransl_alpha_sphere = BMS.compute_supertransl_alpha(supertransl_alpha_modes, theta, phi)
+
+		# The supertranslation is carried out in frequency space.
+		# Step 2: get the FFT of the mode coefficients of Psi4
+		Psi4_tilde_modes = self.to_frequency_basis()
+
+		# Get the 2d angular frequency array
+		omega_axis_2d = Psi4_tilde_modes.omega
+
+		# Construct the supertranslation factor
+		supertransl_factor = np.sum(
+			np.array([np.power((-1j * omega_axis_2d * supertransl_alpha_sphere), index) for index in range(order)]),
+			axis=0,
+		)
+
+		# Multiply with the fourier modes.
+		supertransl_spherical_factor = Psi4_tilde_modes.multiply(supertransl_factor)
+
+		# Reconstruct the modes
+
+		# Check!
+		supertransl_spherical_grid = np.zeros(supertransl_spherical_factor.shape, dtype=np.complex128)
+
+		for ell_value in range(ell_max + 1):
+			for emm_value in range(-ell_value, ell_value + 1):
+				# Multiply with the SWSH basis.
+				supertransl_spherical_grid += supertransl_spherical_factor * Yslm_vec(
+					spin_weight=-2, ell=ell_value, emm=emm_value, theta=theta, phi=phi
+				)
+
+				# Step 3: Reconstruct the function on the sphere
+
+		# Create a spherical_array to hold the supertranslated waveform
+		supertransl_spherical_waveform = spherical_array(grid_info=grid_info)
+
+		# Set the data.
+		supertransl_spherical_waveform.data = supertransl_spherical_grid
+
+		# Get modes_array from spherical_array
+		Psi4_supertransl_modes = supertransl_spherical_waveform.to_modes_array(ell_max=ell_max)
+
+		return Psi4_supertransl_modes
+
+	def boost(self, conformal_factor, grid_info=None):
+		"""Boost the waveform given the unboosted waveform and the boost conformal factor.
+
+		Parameters
+		----------
+		conformal_factor:	2d array
+																						The conformal factor for the Lorentz transformation.
+																						It may be a single floating point number or an array
+																						on a spherical grid. The array will be of dimensions
+																																																		[ntheta, nphi]
+
+		Returns
+		-------
+		boosted_waveform:	spherical_array
+																						The class instance `spherical_array`
+																						that contains the boosted waveform.
+		"""
+
+		from waveformtools.grids import spherical_grid
+
+		# Construct a spherical grid.
+		if grid_info is None:
+			grid_info = spherical_grid()
+
+		# Get spherical array from modes.
+		unboosted_waveform = self.to_spherical_array(grid_info)
+
+		boosted_waveform_data = unboosted_waveform.boost(conformal_factor)
+
+		# Construct a 2d waveform array object
+		boosted_waveform = spherical_array(grid_info=unboosted_waveform.grid_info, data=np.array(boosted_waveform_data))
+		boosted_waveform.label = "boosted"
+
+		# Get modes from spherical data.
+		# boosted_waveform_modes = boosted_waveform.to_modes_array()
+
+		# return boosted_waveform_modes
+		return boosted_waveform
+
+	def get_strain_from_psi4(self, omega0="auto"):
+		"""Get the strain `modes_array` from :math:`\\Psi_4` by
+		fixed frequency integration.
+
+		Parameters
+		----------
+		omega0: float, optional
+										The lower cutoff angular frequency for FFI.
+										By default, it computes this from the mode data.
+
+		Returns
+		-------
+		strain_waveform:	modes_array
+																																																		The computed strain modes.
+		"""
+
+		# Initialize a mode array for strain.
+		strain_waveform = modes_array(
+			label="{} strain from Psi4".format(self.label), r_ext=self.r_ext, ell_max=8, modes_list=self.modes_list
+		)
+
+		strain_waveform.time_axis = self.time_axis
+		strain_waveform.ell_max = self.ell_max
+
+		data_len = self.data_len
+
+		strain_waveform.create_modes_array(ell_max=self.ell_max, data_len=data_len)
+
+		# Integrate,
+		from waveformtools.integrate import fixed_frequency_integrator
+		from waveformtools.waveformtools import get_starting_angular_frequency as sang_f
+
+		omega_st = omega0
+		for item in self.modes_list[:]:
+			ell, emm_list = item
+			for emm in emm_list:
+				mode_data = self.mode(ell, emm)
+				if omega0 == "auto":
+					omega_st = abs(sang_f(mode_data, delta_t=self.delta_t())) / 10
+				strain_mode_data, _ = fixed_frequency_integrator(
+					udata_time=mode_data, delta_t=self.delta_t(), omega0=omega_st, order=2
+				)
+				strain_waveform.set_mode_data(ell, emm, data=strain_mode_data)
+
+		return strain_waveform
+
+	def get_news_from_psi4(self, omega0="auto"):
+		"""Get the News `modes_array` from :math:`\\Psi_4` by
+		fixed frequency integration.
+
+		Parameters
+		----------
+		omega0:	float, optional
+																										The lower cutoff angular frequency for FFI.
+										By default, it computes this as one tenth of
+										the starting frequency of the mode data.
+
+		Returns
+		-------
+		news_waveform:	modes_array
+																		The computed strain modes.
+		"""
+
+		# Initialize a mode array for strain.
+		# news_waveform = modes_array(label=f'{self.label} news from Psi4', r_ext=500, ell_max=8, modes_list=self.modes_list)
+		news_waveform = modes_array(
+			label="{} news from Psi4".format(self.label), r_ext=500, ell_max=8, modes_list=self.modes_list
+		)
+
+		news_waveform.time_axis = self.time_axis
+		news_waveform.ell_max = self.ell_max
+
+		data_len = self.data_len
+
+		news_waveform.create_modes_array(ell_max=self.ell_max, data_len=data_len)
+
+		# Integrate,
+		from waveformtools.integrate import fixed_frequency_integrator
+		from waveformtools.waveformtools import get_starting_angular_frequency as sang_f
+
+		omega_st = omega0
+		for item in self.modes_list[:]:
+			ell, emm_list = item
+			for emm in emm_list:
+				mode_data = self.mode(ell, emm)
+				if omega0 == "auto":
+					omega_st = abs(sang_f(mode_data, delta_t=self.delta_t())) / 10
+				news_mode_data, _ = fixed_frequency_integrator(
+					udata_time=mode_data, delta_t=self.delta_t(), omega0=omega_st, order=1
+				)
+				news_waveform.set_mode_data(ell, emm, data=news_mode_data)
+
+		return news_waveform
+
+	def taper(self, zeros="auto"):
+		"""Taper a waveform at both ends and insert zeros if needed
+
+		Parameters
+		----------
+		zeros:	int
+																										The number of zeros to add at rach end
+
+		Returns
+		-------
+		tapered_modes:	modes_array
+																		Modes array with tapered mode data.
+		"""
+
+		from waveformtools.waveformtools import taper
+
+		if zeros == "auto":
+			# Decide the number of zeros
+			data_len = self.data_len
+
+			nearest_power = int(np.log(data_len) / np.log(2))
+			req_len = np.power(2, nearest_power + 1)
+			zeros = req_len - data_len
+			message("num_zeros", zeros)
+
+		# New modes array.
+
+		tapered_modes = None
 
 		for item in self.modes_list[:]:
 			ell, emm_list = item
 			for emm in emm_list:
 				input_data_re = self.mode(ell, emm).real
 				input_data_im = self.mode(ell, emm).imag
 
@@ -1851,44 +1764,31 @@
 
 					tapered_modes.create_modes_array(ell_max=self.ell_max, data_len=new_data_len)
 				tapered_data = tapered_data_re + 1j * tapered_data_im
 
 				# message(len(tapered_data_re))
 				tapered_modes.set_mode_data(ell, emm, data=tapered_data)
 
-                _, tapered_data_re = taper_tanh(
-                    input_data_re,
-                    delta_t=self.delta_t(),
-                    duration=duration,
-                    sides=sides,
-                )
-                _, tapered_data_im = taper_tanh(
-                    input_data_im,
-                    delta_t=self.delta_t(),
-                    duration=duration,
-                    sides=sides,
-                )
+		# Set the time axis
+		new_time_axis = np.arange(0, new_data_len * self.delta_t(), self.delta_t())
 
 		tapered_modes.time_axis = new_time_axis
 
 		# Recenter the modes.
 		tapered_modes.trim(trim_upto_time=0)
 
-                    tapered_modes.create_modes_array(
-                        ell_max=self.ell_max, data_len=new_data_len
-                    )
-                tapered_data = tapered_data_re + 1j * tapered_data_im
+		return tapered_modes
 
 	def taper_tanh(self, time_axis=None, zeros="auto", duration=10, sides="both"):
 		"""Taper a waveform at both ends and insert zeros if needed
 
-        # Set the time axis
-        new_time_axis = np.arange(
-            0, new_data_len * self.delta_t(), self.delta_t()
-        )
+		Parameters
+		----------
+		zeros:	int
+										The number of zeros to add at rach end
 
 		Returns
 		-------
 		tapered_modes:	modes_array
 																																										Modes array with tapered mode data.
 		"""
 
@@ -1899,101 +1799,90 @@
 			data_len = self.data_len
 
 			nearest_power = int(np.log(data_len) / np.log(2))
 			req_len = np.power(2, nearest_power + 1)
 			zeros = req_len - data_len
 			# message('num_zeros', zeros)
 
-        Parameters
-        ----------
-        order : int, optional
-                The order of the butterworth filter.
-        omega0 : float, optional
-                The cutoff frequency of the butterworth filter.
-
-        Returns
-        --------
-        filtered_modes : modes_array
-                         A modes array object containing filtered modes.
-        """
+		# New modes array.
+
+		tapered_modes = None
+
+		for item in self.modes_list[:]:
+			ell, emm_list = item
+			for emm in emm_list:
+				input_data_re = self.mode(ell, emm).real
+				input_data_im = self.mode(ell, emm).imag
 
 				# tapered_data_re = taper(input_data_re, zeros=zeros)
 				# tapered_data_im = taper(input_data_im, zeros=zeros)
 
 				_, tapered_data_re = taper_tanh(input_data_re, delta_t=self.delta_t(), duration=duration, sides=sides)
 				_, tapered_data_im = taper_tanh(input_data_im, delta_t=self.delta_t(), duration=duration, sides=sides)
 
 				new_data_len = len(tapered_data_re)
 
-                    filtered_modes.create_modes_array(
-                        ell_max=self.ell_max, data_len=self.data_len
-                    )
-
-                # Get filtered mode data.
-                filtered_data = low_cut_filter(
-                    self.mode(ell, emm),
-                    self.frequency_axis,
-                    omega0=omega0,
-                    order=order,
-                )
+				if tapered_modes is None:
+					tapered_modes = modes_array(
+						label="tapered {}".format(self.label),
+						r_ext=self.r_ext,
+						modes_list=self.modes_list,
+						ell_max=self.ell_max,
+					)
+
+					tapered_modes.create_modes_array(ell_max=self.ell_max, data_len=new_data_len)
+				tapered_data = tapered_data_re + 1j * tapered_data_im
 
 				# message(len(tapered_data_re))
 				tapered_modes.set_mode_data(ell, emm, data=tapered_data)
 
 		# Set the time axis
 		new_time_axis = np.arange(0, new_data_len * self.delta_t(), self.delta_t())
 
 		tapered_modes.time_axis = new_time_axis
 
-    def to_td_waveform(
-        self,
-        Mtotal=1,
-        theta=0,
-        phi=0,
-        alpha=None,
-        distance=1,
-        delta_t=None,
-        method="precise",
-        k=None,
-    ):
-        """Get the plus and cross polarizations of
-        of the waveform time series by summing the modes.
-
-        Parameters
-        ----------
-        theta, phi : float
-                     The inclination and the azimuthal
-                     angular position of the observer
-                     in the NR coodinate system.
-
-        distance : float
-                   The distance to the source
-
-        method : str
-                 The method to use to generate
-                 the SWSH basis. This can be
-                 `precise` or `fast`.
-
-        Returns
-        -------
-        taxis, hp, hc : 1d arrays
-                        The 1d arrays of the time axis and
-                        the polarizations of the waveforms.
-
-        Notes
-        -----
-        This does not rotate the polarizations. The rotation
-        must be done separately using the `rotate_polarizations`
-        function of `waveformtools.transforms`
-
-        For precessing systems and to obtain the waveform
-        in the LAL convention, one should use the
-        nrcatalogtools package to obtain the correct
-        angles first.
-        """
+		# Recenter the modes.
+		tapered_modes.trim(trim_upto_time=0)
+
+		return tapered_modes
+
+	def low_cut(self, omega0=0.03, order=2):
+		"""Apply the low cut filter from waveformtools.low_cut_filter
+
+		Parameters
+		----------
+		order:	int, optional
+										The order of the butterworth filter.
+		omega0:	float, optional
+										The cutoff frequency of the butterworth filter.
+
+		Returns:
+		--------
+		filtered_modes:	modes_array
+																																										A modes array object containing filtered modes.
+		"""
+
+		# modes_array for filtered data.
+		filtered_modes = None
+
+		# Import the filter
+		from waveformtools.waveformtools import low_cut_filter
+
+		for item in self.modes_list:
+			# Iterate over available modes.
+			ell, emm_list = item
+			for emm in emm_list:
+				if filtered_modes is None:
+					# Create filtered_modes
+					filtered_modes = modes_array(
+						label="lc filtered {}".format(self.label),
+						r_ext=self.r_ext,
+						modes_list=self.modes_list,
+						ell_max=self.ell_max,
+					)
 
 					filtered_modes.create_modes_array(ell_max=self.ell_max, data_len=self.data_len)
 
 				# Get filtered mode data.
 				filtered_data = low_cut_filter(self.mode(ell, emm), self.frequency_axis, omega0=omega0, order=order)
 
 				# Set the mode data.
```

### Comparing `waveformtools-2023.6.3/waveformtools/waveformtools.py` & `waveformtools-2023.6.5/waveformtools/waveformtools.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,52 +38,48 @@
 
 # matplotlib.use('Agg')
 from matplotlib import pyplot as plt
 from termcolor import colored
 
 
 def message(
-    *args,
-    message_verbosity=2,
-    print_verbosity=config.print_verbosity,
-    log_verbosity=config.log_verbosity,
-    **kwargs,
+    *args, message_verbosity=2, print_verbosity=config.print_verbosity, log_verbosity=config.log_verbosity, **kwargs
 ):
     """The print function with verbosity levels and logging facility.
 
     Notes
     -----
     Verbosity choices:
 
-    * message_verbosity : Each message carries with it a verbosity level.
-                          More the verbosity less the priority.
-                          Default value is 2 i.e. informational.
-    * print_verbosity : prints all messages above this level of verbosity.
-    * log_verbosity : logs all messages above this level of verbosity.
-
-    Verbosity  levels :
-    * 0 : Errors
-    * 1 : Warnings
-    * 2 : Information
+    * message_verbosity :   Each message carries with it a verbosity level.
+                                                    More the verbosity less the priority.
+                                                    Default value is 2 i.e. informational.
+    * print_verbosity   :   prints all messages above this level of verbosity.
+    * log_verbosity     :   logs all messages above this level of verbosity.
+
+    Verbosity  levels:
+    * 0: Errors
+    * 1: Warnings
+    * 2: Information
 
     Parameters
     ----------
-    ``*args` : non-keyword arguments
-               same arguments as to that of the print functions,
-    message_verbosity : int
-    print_verbosity : int
-    log_verbosity : int
-    ``**kwargs`` : keyword arguments
-                   Same as that of the print function.
+    ``*args`            :   non-keyword arguments
+                                                    same arguments as to that of the print functions,
+    message_verbosity   :   int
+    print_verbosity     :   int
+    log_verbosity       :   int
+    ``**kwargs``        :   keyword arguments
+                                                    Same as that of the print function.
 
     Returns
     -------
-    1 : int
-        messages to stdout and logging of messages,
-        while the function returns 1.
+    1                   :   int
+                                                    messages to stdout and logging of messages,
+                                                    while the function returns 1.
     """
 
     # If message verbosity matches the global verbosity level, then print
     if message_verbosity <= print_verbosity:
         print(*args, **kwargs)
     if log_verbosity <= message_verbosity:
         now = str(datetime.datetime.now())
@@ -94,66 +90,69 @@
             os.mkdir("logs")
 
         with open("logs/" + tstamp + ".log", "a") as log_file:
             if message_verbosity == -1:
                 for line in traceback.format_stack():
                     log_file.write(line.strip())
             log_file.write("\n")
-            log_file.write(
-                "{}:{}\t{}".format(caller.filename, caller.lineno, *args)
-            )
+            log_file.write("{}:{}\t{}".format(caller.filename, caller.lineno, *args))
             log_file.write("\n")
     return 1
 
 
 def mode(a_list):
     """Find the mode of a list
 
     Parameters
     ----------
-    a_list : list
-             The list whose mode is to be found
+    a_list: list
+                    The list whose mode is to be found
 
     Returns
     -------
-    list_mode : float
-                The mode of the list.
+    list_mode:  float
+                            The mode of the list.
+
     """
 
     a_list = list(a_list)
 
     return max(set(a_list), key=a_list.count)
 
 
+# Data I/O functions
+
+
 def save_obj(obj, name, obj_dir="./", protocol=pickle.HIGHEST_PROTOCOL):
     """A function to save python objects to disk using pickle.
 
     Parameters
     ----------
-    obj : object
-          The python object to be saved.
-    name : string
-           The filename.
-    obj_dir : string
-              The path to directory to be saved in. Defaults to PWD
-    protocol : int
-               The protocol to be used to save. Default is binary.
+    obj :   object
+                    The python object to be saved.
+    name :  string
+                    The filename.
+    obj_dir :   string
+                            The path to directory to be saved in. Defaults to PWD
+    protocol :  int
+                            The protocol to be used to save. Default is binary.
 
     Notes
     -----
     Protocols:
 
     * 0 : Text
     * 5 : Binary
 
     See the man page of pickle for more details.
 
     Returns
     -------
     Nothing (other than saving the data to the disk).
+
     """
 
     # Create the directory dir if it doesn't exist.
     if not os.path.isdir(obj_dir):
         os.mkdir(obj_dir)
 
     # Pickle the file to disk.
@@ -163,23 +162,23 @@
 
 def load_obj(name, obj_dir="./"):
     """A function to load python objects from the disk using pickle.
 
     Parameters
     ----------
 
-    name : string
-           The filename.
-    obj_dir : string
-              The path to directory in which file exists. Defaults to PWD.
+    name :  string
+                    The filename.
+    obj_dir :   string
+                            The path to directory in which file exists. Defaults to PWD.
 
     Returns
     -------
-    obj : object
-          A python object with the contents of the file.
+    obj :   object
+                    A python object with the contents of the file.
     """
 
     # Load the pickled data
     with open(obj_dir + name + ".pkl", "rb") as data_file:
         return pickle.load(data_file)
 
 
@@ -187,23 +186,23 @@
     """Remove Nans from (xdata,ydata) data pair.
     Removes Nans in xdata and ydata and the
     corresponding y and x entries.
 
     Parameters
     ----------
     xdata : 1d array
-            The x axis of the data.
+                    The x axis of the data.
     ydata : 1d array
-            The y axis of the data.
+                    The y axis of the data.
 
     Returns
     -------
-    x_no_nan : 1d array
-    y_no_nan : 1d array
-               The data pair x,y with Nans removed.
+    x_no_nan :  1d array
+    y_no_nan :  1d,array
+                            The data pair x,y with Nans removed.
     """
 
     # Find the location of x Nans to be removed.
     nan_locs = np.where(np.isnan(xdata))[0]
     # Remove the xdata and the corresponding y entries.
     xdata = np.delete(xdata, nan_locs)
     ydata = np.delete(ydata, nan_locs)
@@ -228,83 +227,77 @@
 
 
 def differentiate(data, delta_t=None, TS=False):
     """Differentiate a timeseries in time domain using the Simple Euler method
 
     Parameters
     ----------
-    data : 1d array
-           a pycbc TimeSeries object
-           The time series to be differentiated.
-    delta_t : float
-              The grid spacing delta_t.
-              Supplying delta_t overrides
-              the delta_t attribute of TimeSeries.
+    data :  1d array
+                    a pycbc TimeSeries object
+                    The time series to be differentiated.
+    delta_t :   float
+                            The grid spacing delta_t.
+                            Supplying delta_t overrides
+                            the delta_t attribute of TimeSeries.
 
     Returns
     -------
-    ddt_data : pycbc TimeSeries object
-               The differentiated 1d data
-               as pycbc TimeSeries"""
+    ddt_data :  pycbc TimeSeries object
+                            The differentiated 1d data
+                            as pycbc TimeSeries"""
 
     if not delta_t:
         try:
             delta_t = data.delta_t
         except BaseException:
-            message(
-                "Input is not a TimeSeries. Please supply gridspacing as delta_t",
-                message_verbosity=0,
-            )
+            message("Input is not a TimeSeries. Please supply gridspacing as delta_t", message_verbosity=0)
 
     dydx = np.diff((np.array(data))) / delta_t
 
     if TS is True:
         dydx = pycbc.types.timeseries.TimeSeries(dydx, delta_t)
 
     return dydx
 
 
-def integrate_first_order(
-    data, t_start=None, t_end=None, delta_t=None, to_taper=False, TS=False
-):
+def integrate_first_order(data, t_start=None, t_end=None, delta_t=None, to_taper=False, TS=False):
     """Integrate a timeseries using first order method.
 
     Notes
     -----
-    Capabilities:
-        Simple Euler integrator, option to taper the ends.
+    Capabilities
+
+    Simple Euler integrator, option to taper the ends.
 
     Parameters
     ----------
-    data : 1d array or a pycbc TimeSeries object
-           The input function to be integrated.
-    delta_t : float
-              The grid spacing delta_t,
-    to_taper : bool
-               True or False. Whether or not
-               to taper the input series.
+    data :  1d array or a pycbc TimeSeries object
+                    The input function to be integrated.
+    delta_t :   float
+                            The grid spacing delta_t,
+    to_taper :  bool
+                            True or False. Whether or not
+                            to taper the input series.
 
     Returns
     -------
-    int_data : a pycbc TimeSeries object
-               TimeSeries of the time integrated data"""
+    int_data :  a pycbc TimeSeries object
+                            TimeSeries of the time integrated data"""
 
     # Check if object is pycbc timeseries. Recover delta_t, t_start, t_end if yes.
     if not delta_t:
         try:
             # Find sampling time_step
             delta_t = data.delta_t
             data_time = data.sample_times
             t_start_dat, t_end_dat = data_time[0], data_time[-1]
 
         except BaseException:
             message(
-                "Input is not a TimeSeries."
-                "Please input a pycbc TimeSeries"
-                "or supply gridspacing as delta_t",
+                "Input is not a TimeSeries." "Please input a pycbc TimeSeries" "or supply gridspacing as delta_t",
                 message_verbosity=0,
             )
     else:
         t_start_dat = 0
         t_end_dat = len(data) * delta_t
 
     if not t_start:
@@ -338,132 +331,138 @@
 
     data = np.array(data)
 
     for i in range(1, end_index - start_index):
         integdat[i] = integdat[i - 1] + (data[start_index + i - 1]) * delta_t
 
     if TS is True:
-        integdat = pycbc.types.timeseries.TimeSeries(
-            integdat, delta_t, epoch=t_start
-        )
+        integdat = pycbc.types.timeseries.TimeSeries(integdat, delta_t, epoch=t_start)
 
     return integdat
 
 
 def compute_frequencies(t_coal, t_val, chirp_mass):
     """Compute the Newtonian instantaneous frequency
     of strain waveform from coalescence time and
     chirp mass, from the Finn-Chernoff model.
 
     Parameters
     ----------
-    t_coal : float
-             The coalescence time,
+    t_coal :    float
+                            The coalescence time,
     t_val : 1d array
-            The time,
-    chirp_mass : float
-                 The chirpmass.
+                    The time,
+    chirp_mass :    float
+                                    The chirpmass.
 
     Returns
     -------
     freqs : float
-            The instantaneous frequency of the strain waveform."""
-    freqs = (
-        (1.0 / (np.pi * chirp_mass))
-        * (5.0 / 256) ** (3.0 / 8)
-        * (chirp_mass / (t_coal - t_val)) ** (3.0 / 8)
-    )
+                    The instantaneous frequency of the strain waveform."""
+    freqs = (1.0 / (np.pi * chirp_mass)) * (5.0 / 256) ** (3.0 / 8) * (chirp_mass / (t_coal - t_val)) ** (3.0 / 8)
 
     return freqs
 
 
 def totalmass(mass_ratio, chirp_mass):
     """Find total mass from mass ratio and chirpmass.
 
     Parameters
     ----------
-    mass_ratio : float
-                 The mass ratio of the system.
-    mchirp : float
-             The chirp mass of the system.
+    mass_ratio :    float
+                                    The mass ratio of the system.
+    mchirp :    float
+                            The chirp mass of the system.
 
     Returns
     -------
-    total_mass : float
-                 The total mass of the system.
+    total_mass :    float
+                                    The total mass of the system.
     """
 
-    return (chirp_mass * (1.0 + mass_ratio) ** (6.0 / 5)) / mass_ratio ** (
-        3.0 / 5
-    )
+    return (chirp_mass * (1.0 + mass_ratio) ** (6.0 / 5)) / mass_ratio ** (3.0 / 5)
 
 
 def massratio(chirp_mass):
     """Compute the mass ratio from chirpmass. Assumes total mass to be 1.
 
     Parameters
     ----------
-    mchirp : float
-             The chirp mass of the system.
+    mchirp :    float
+                            The chirp mass of the system.
 
     Returns
     -------
-    mass_ratio : float
-                 The Mass ratio of the system
+    mass_ratio :    float
+                                    The Mass ratio of the system
     """
     mass_ratio = (
-        chirp_mass ** (1.0 / 3)
-        - 2.0 * chirp_mass**2.0
-        - np.sqrt(chirp_mass ** (2.0 / 3) - 4.0 * chirp_mass ** (7.0 / 3))
+        chirp_mass ** (1.0 / 3) - 2.0 * chirp_mass**2.0 - np.sqrt(chirp_mass ** (2.0 / 3) - 4.0 * chirp_mass ** (7.0 / 3))
     ) / (2.0 * chirp_mass**2.0)
 
     return mass_ratio
 
 
+# Defining function for calculating Chirpmass from a2
+
+
 def compute_chirp_mass(a2_param):
     """Compute the chirpmass from a2, the coefficient of time of the Finn-Chernoff waform model.
 
     Parameters
     ----------
-    a2_param : 1d array or float
-               The a2 parameter in the Finn Chernoff model.
+
+    a2_param :  1d array \\ float
+                            The a2 parameter in the Finn Chernoff model.
 
     Returns
     -------
-    chirp_mass : float
-                 The chirp mass
+    chirp_mass :    float
+                                    The chirp mass
     """
     chirp_mass = 2 ** (8.0 / 5) / (5 * np.array(a2_param) ** (8.0 / 5))
     return chirp_mass
 
 
 def lengtheq(data_a, data_b, delta_t=None, is_ts=False):
     """Equalize the length of two timeseries/array by
     appending zeros at the end of the array. No tapering.
 
+    Procedure
+    ---------
+
+    1. Check if input data are timeseries.
+       If not then construct timeseries using delta_t.
+    2. Check data length.
+       If they are already equal then skip and return the inputs.
+    3. Check if data_a is smaller then data_b ( or vice versa).
+       Then augment zeroes at either ends of array to data_a
+       (data_b) and return.
+
+
     Parameters
     ----------
-    data_a : list
-             The input waveform A
-    data_b : list
-             The input waveform B.
-    delta_t : float
-              The time steping. Defaults to `None`.
-    is_ts : bool
-            To determine whether the given data
-            is a pycbc TimeSeries.
+    data_a :    list
+                            The input waveform A
+    data_b :    list
+                            The input waveform B.
+    delta_t :   float
+                            The time steping. Defaults to `None`.
+    is_ts :     bool
+                            To determine whether the given data
+                            is a pycbc TimeSeries.
     Returns
     -------
     equalized_signals : list
-                        The Tapered, length equalized waveforms data_a and data_b,
-                        and a flag denoting which waveform was changed, `a` or `b`.
+                                            The Tapered, length equalized waveforms data_a and data_b,
+                                            and a flag denoting which waveform was changed, `a` or `b`.
 
     Notes
     -----
-    Recommended usage :
+    Recommended usage:
 
             Change length of waveform `a` to match with that of waveform `b`.
 
     """
 
     # Check if input data vectors are pycbc TimeSeries. If yes, create a copy
     # of data and extract delta_t.
@@ -505,32 +504,24 @@
         lflag = "ab"
 
     # If data_a < data_b
     elif len(data_a) < len(data_b):
         # add zeros to data_a when a is smaller
         lflag = "a"
         zers = len(data_b) - len(data_a)
-        signala = np.transpose(
-            np.concatenate(
-                (np.transpose(data_a), np.transpose(np.zeros([zers])))
-            )
-        )
+        signala = np.transpose(np.concatenate((np.transpose(data_a), np.transpose(np.zeros([zers])))))
         # signala = pycbc.types.timeseries.TimeSeries(signala, delta_t)
         # return pycbc.types.timeseries.TimeSeries(signalb,delta_t),lflag
     # If data_b < data_a
     else:
         # message("Error!")
         # add zeros to b when b is smaller
         lflag = "b"
         zers = len(data_a) - len(data_b)
-        signalb = np.transpose(
-            np.concatenate(
-                (np.transpose(data_b), np.transpose(np.zeros([zers])))
-            )
-        )
+        signalb = np.transpose(np.concatenate((np.transpose(data_b), np.transpose(np.zeros([zers])))))
         # signalb = pycbc.types.timeseries.TimeSeries(signalb, delta_t)
         # return pycbc.types.timeseries.TimeSeries(signala,delta_t),lflag
 
     # Returns a list containing the length equalized arrays and the flag.
     if not is_ts:
         signala = np.array(signala)
         signalb = np.array(signalb)
@@ -539,27 +530,27 @@
 
 
 def taperlengtheq(data_a, data_b, delta_t=None):
     """Taper and equalize the lengths of two arrays.
 
     Parameters
     ----------
-    data_a : list
-             The input waveform A.
-    data_b : list
-             The input waveform B.
-    delta_t : float
-              The time steping.
+    data_a :    list
+                            The input waveform A.
+    data_b :    list
+                            The input waveform B.
+    delta_t :   float
+                            The time steping.
 
     Returns
     -------
     equalized_signals : list
-                        The Tapered, length equalized waveforms
-                        data_a and data_b, and a flag denoting
-                        which waveform was changed, `a` or `b`.
+                                            The Tapered, length equalized waveforms
+                                            data_a and data_b, and a flag denoting
+                                            which waveform was changed, `a` or `b`.
     """
 
     # Check if input data is pycbc TimeSeries. If yes, then ectract delta_t.
     if not delta_t:
         signala = data_a
         signalb = data_b
 
@@ -567,17 +558,15 @@
             delta_t = signala.delta_t
 
         except AttributeError:
             try:
                 delta_t = signalb.delta_t
             except BaseException:
                 message(
-                    "Input is not a TimeSeries."
-                    "Please supply a pycbc TimeSeries object "
-                    "or the gridspacing as delta_t",
+                    "Input is not a TimeSeries." "Please supply a pycbc TimeSeries object " "or the gridspacing as delta_t",
                     message_verbosity=0,
                 )
 
     # Ensure data is numpy array.
     signalb = np.array(data_b)
     # Taper waveform A.
     signala = np.array(taper(data_a, delta_t))
@@ -596,36 +585,29 @@
 
     0: Continuous.
     1: Repetitive rows.
     2: Jumps in timeaxis.
 
     Parameters
     ----------
-    data : list
-           Input as a list of 1d arrays [time, data1, data2, ...].
-           All the data share the common time axis `time`
-    delta_t : float
-              The time stepping.
-    toldt : float
-            The tolerance for error in checking. defaluts to toldt=1e-3.
+    data:   list
+                    Input as a list of 1d arrays [time, data1, data2, ...].
+                    All the data share the common time axis `time`
+    delta_t:    float
+                            The time stepping.
+    toldt:  float
+                    The tolerance for error in checking. defaluts to toldt=1e-3.
 
     Returns
     -------
-    discontinuity_details : dict.
-                            It contains a dict of the details
-                            of discontinuity type. For each
-                            discontinuity type:
-                                1. Repetitiion
-                                2. Jumps
-                            It contains a list whose elements
-                            are
-                                1. a flag denoting if the discontinuity
-                                   of the given type exists (1).
-                                2. index locations of discontinuities
-                                    in the original array.
+    discontinuity_details:  a list.
+                                                    It contains:
+                                                            1. A list. details of discontinuity:  index location of original array,
+                                                            the corresponding discinbtinuity type.
+                                                    2. A float. the global discontinuity type.
     """
 
     time_axis = np.sort(time_axis)
 
     dt_axis = np.diff(time_axis)
 
     if not delta_t:
@@ -658,22 +640,22 @@
 def sort_data(data):
     """Sort the data according to its
     time axis. The first axis is assumend to be
     the time axis.
 
     Parameters
     ----------
-    data : ndarray
-           The data array with shape (naxis, time_steps)
-           The first axis is assumed to be the time axis.
+    data:   ndarray
+                    The data array with shape (naxis, time_steps)
+                    The first axis is assumed to be the time axis.
 
     Returns
     -------
-    sorted_data : ndarray
-                  The sorted data array
+    sorted_data:    ndarray
+                                    The sorted data array
     """
 
     data = np.array(data)
 
     # message("Data shape:", (data.shape), message_verbosity=3)
     # Set axis along which to remove
     axis = data.ndim - 1
@@ -694,37 +676,37 @@
     if axis > 0:
         sorted_data = data[:, order]
     else:
         sorted_data = np.sort(time)
 
     return sorted_data
 
-    return sorted_data
 
 def remove_repetitive_rows(data, delta_t=1, toldt=1e-3):
     """Remove repeated rows in the data
 
     Parameters
     ----------
-    data : ndarray
-           Data array where the first axis refers to different
-           columns of data. The zeroth column is time axis.
-           The second axis refers to entries at different time
-           steps.
-
-    delta_t : float
-              The tim stepping.
-    toldt : float
-            The tolerance for error in checking. defaluts to toldt=1e-3.
+    data:   ndarray
+                    Data array where the first axis refers to different
+                    columns of data. The zeroth column is time axis.
+                    The second axis refers to entries at different time
+                    steps.
+
+    delta_t:    float
+                            The tim stepping.
+    toldt:  float
+                    The tolerance for error in checking. defaluts to toldt=1e-3.
 
     Returns
     -------
-    cleaned_data : list
-                   The cleaned data array with repetitive
-                   rows removed.
+    cleaned_data:   list
+                                    The cleaned data array with repetitive
+                                    rows removed.
+
     """
     message("Checking data for repetative rows...\n", message_verbosity=2)
     data = sort_data(data)
 
     # message("Data shape:", (data.shape), message_verbosity=3)
     # Set axis along which to remove
     axis = data.ndim - 1
@@ -762,29 +744,30 @@
 
 
 def fill_gaps_in_data(data, k=5):
     """Fill gaps in data by interpolation
 
     Parameters
     ----------
-    data : list
-           Input as a list of 1d arrays [time, data1, data2, ...].
-           All the data share the common time axis `time`
-    k : int, optional
-        The interpolation order. Defaults to 5
+    data:   list
+                    Input as a list of 1d arrays [time, data1, data2, ...].
+                    All the data share the common time axis `time`
+    k:  int, optional
+            The interpolation order. Defaults to 5
 
     Returns
     -------
-    cleaned_data : list
-                   The cleaned data array with repetitive
-                   rows and gaps (if bridge=True) removed.
+    cleaned_data:   list
+                                    The cleaned data array with repetitive
+                                    rows and gaps (if bridge=True) removed.
 
     See Also
     --------
     scipy.interpolate.InterpolatedUnivariateSpline
+
     """
 
     data = sort_data(data)
     time = data[0]
 
     s1, l = data.shape
 
@@ -794,66 +777,61 @@
 
     discontinuities = iscontinuous_new(time)
 
     gaps = bool(discontinuties["gaps"][0])
 
     if gaps:
         gap_rows = discontinuoties["gaps"][1]
-        message(
-            "The data will be interpolated to bridge the gaps",
-            message_verbosity=2,
-        )
+        message("The data will be interpolated to bridge the gaps", message_verbosity=2)
 
         # Interpolate the data to fill in the discontinuities
         t_final = time[-1]
         t_initial = time[0]
 
         proper_timeaxis = np.arange(t_initial, t_final, delta_t)
 
         interp_data = []
         interp_data.append(proper_timeaxis)
 
-        from scipy.interpolate import (
-            InterpolatedUnivariateSpline as interpolator,
-        )
+        from scipy.interpolate import InterpolatedUnivariateSpline as interpolator
 
         for index in range(1, s1):
-            interp_data.append(
-                interpolator(time, data[index, :], k=k)(proper_timeaxis)
-            )
+            interp_data.append(interpolator(time, data[index, :], k=k)(proper_timeaxis))
 
         cleaned_data = np.array(interp_data)
         message("The data has been interpolated", message_verbosity=3)
     else:
         message("No jumps found in the data", message_verbosity=2)
 
     return cleaned_data
 
 
 def cleandata(data, toldt=1e-3, bridge=False, k=5):
     """Check the data (time,datar,datai) for repetetive rows and remove them.
 
     Parameters
     ----------
-    data : list
-           Input as a list of 1d arrays [time, data1, data2, ...].
-           All the data share the common time axis `time`
-    toldt : float
-            The tolerance for error in checking. defaluts to toldt=1e-3.
-    bridge : bool
-             A bridge flag to decide whether or not to interpolate and
-             resample to fill in jump discontinuities.
-    k : int, optional
-        The interpolation order. Defaults to 5
+
+    data:   list
+                    Input as a list of 1d arrays [time, data1, data2, ...].
+                    All the data share the common time axis `time`
+    toldt:  float
+                    The tolerance for error in checking. defaluts to toldt=1e-3.
+    bridge: bool
+                            A bridge flag to decide whether or not to interpolate and
+                            resample to fill in jump discontinuities.
+    k:  int, optional
+            The interpolation order. Defaults to 5
 
     Returns
     -------
-    cleaned_data : list
-                   The cleaned data array with repetitive
-                   rows and gaps (if bridge=True) removed.
+    cleaned_data:   list
+                                    The cleaned data array with repetitive
+                                    rows and gaps (if bridge=True) removed.
+
     """
 
     # Check the data (time,datar,datai) for repetetive rows and remove them.
     # Ensure data as numpy array
     data = np.array(data)
 
     # message("Data shape:", (data.shape), message_verbosity=3)
@@ -892,63 +870,56 @@
     """Timeshift an array. IMP: After timeshifting, the original
     length of the array is retained by clipping last(first) when
     ind > 0(ind <0) `ind` number of points!!. Make sure the input array
     already has number of zeros z > ind (z<ind) initially at the end.
 
     Parameters
     ----------
-    hdat : 1d array or a pycbc TimeSeries object
-           The input waveform to be shifted in time.
-    ind : int
-          The numper of places to shift the input waveform.
-    delta_t : int
-              the grid spacing in time.
+    hdat:   1d array or a pycbc TimeSeries object
+                    The input waveform to be shifted in time.
+    ind:    int
+                    The numper of places to shift the input waveform.
+    delta_t:    int
+                            the grid spacing in time.
 
     Returns
     -------
-    shifted_wf : a pycbc TimeSeries object
-                 The waveform array of same length timeshifted by
-                 `ind` units by prepending zeros.
+    shifted_wf: a pycbc TimeSeries object
+                            The waveform array of same length timeshifted by
+                            `ind` units by prepending zeros.
     """
 
     if is_ts:
         if not delta_t:
             try:
                 delta_t = hdat.delta_t
             except BaseException:
-                message(
-                    "Input is not a TimeSeries. Please supply gridspacing as delta_t",
-                    message_verbosity=0,
-                )
+                message("Input is not a TimeSeries. Please supply gridspacing as delta_t", message_verbosity=0)
 
     if ind > 0:
         # ind>0 case for shifting array to the right
         # message hdat
         # Length of the data
         # l = len(hdat)
         # Array holding zeroes to be appended
         zeros = np.zeros([ind])
         # The shifted array
-        shifted_wf = np.transpose(
-            np.concatenate((np.transpose(zeros), np.transpose(hdat)))
-        )[:-ind]
+        shifted_wf = np.transpose(np.concatenate((np.transpose(zeros), np.transpose(hdat))))[:-ind]
         # message msig
         # message msig[:-ind]
         # Return the clipped, shifted timeseries
 
     elif ind < 0:
         # ind <0 case for shifting array to the left
         # Length of the data
         # l = len(hdat)
         # Array holding zeroes to be appended
         zeros = np.zeros([ind])
         # The shifted array
-        shifted_wf = np.transpose(
-            np.concatenate((np.transpose(hdat), np.transpose(zeros)))
-        )[ind:]
+        shifted_wf = np.transpose(np.concatenate((np.transpose(hdat), np.transpose(zeros))))[ind:]
         # message msig
         # message msig[:-ind]
         # Return a timeseries
 
     else:
         shifted_wf = hdat
 
@@ -961,21 +932,22 @@
 @njit
 def unwrap_phase(phi0):
     """Unwrap the phase by finding turning points in phi0.
     Finding turning points for unwrapping arctan2 function
 
     Parameters
     ----------
-    phi0 : 1darray
-           The wrapped phase which takes values in the
-           range (0, 2pi).
+    phi0:   1darray
+                    The wrapped phase which takes values in the
+                    range (0, 2pi).
     Returns
     -------
-    phic : 1darray
-           The unwrapped phase.
+    phic:   1darray
+                    The unwrapped phase.
+
     """
 
     # Bookkeeping for upper (tpu) and lower (tpd) turning points
     tpu = []
     tpd = []
     # j = 0
     # k = 0
@@ -1017,25 +989,25 @@
 
 # Complex Phase-Amplitude representation of data
 def xtract_cphase(tsdata_p, tsdata_x, delta_t=None, to_plot=False):
     """Given real and imaginary parts of a complex timeseries, extract the phase of the waveform :arctan_(Img(data)/Re(data))
 
     Parameters
     ----------
-    tsdata_p, tsdata_x : 1d array / a pycbc TimeSeries
-                         The plus and cross polarized components of the waveforms.
-    delta_t : float, optional
-              The time step. Overrides the timestep from pycbc TS object if given.
-    to_plot : bool, optional
-              True or False. Whether to plot the data or not
+    tsdata_p, tsdata_x: 1d array / a pycbc TimeSeries
+                                            The plus and cross polarized components of the waveforms.
+    delta_t:    float, optional
+                            The time step. Overrides the timestep from pycbc TS object if given.
+    to_plot:    bool, optional
+                            True or False. Whether to plot the data or not
 
     Returns
     -------
-    phic : 1d array
-           The 1d array of the phase of the waveform.
+    phic:   1d array
+                    The 1d array of the phase of the waveform.
     """
 
     # Assign the timestep. Real and imaginary parts are assumed to have same timestep.
     # if not delta_t:
     #   try:
     #       delta_t = tsdata_p.delta_t
     #   except AttributeError:
@@ -1086,23 +1058,23 @@
 def xtract_camp(tsdata_p, tsdata_x, to_plot=False):
     """Given real and imaginary parts of a complex timeseries,
     extract the amplitude of the complex data vector
     : (tsdata_p + i * tsdata_x)
 
     Parameters
     ----------
-    tsdata_p, tsdata_x : pycbc TimeSeries/1darray
-                         The plus and cross polarized components of the waveforms.
-    to_plot : bool
-              True or False. Whether to plot the data or not
+    tsdata_p, tsdata_x: pycbc TimeSeries/1darray
+                                            The plus and cross polarized components of the waveforms.
+    to_plot:    bool
+                            True or False. Whether to plot the data or not
 
     Returns
     -------
-    camp : 1d array
-           The 1d array of extracted amplitudes of the waveform.
+    camp:   1d array
+                    The 1d array of extracted amplitudes of the waveform.
     """
 
     # Assign the timestep. Real and imaginary parts are assumed to have same timestep.
     # Complex modulous of the data
     camp = np.sqrt(np.array(tsdata_p) ** 2 + np.array(tsdata_x) ** 2)
 
     if to_plot:
@@ -1119,70 +1091,72 @@
 
 
 def xtract_camp_phase(tsdata_1, tsdata_2):
     """Wrapper for extracting the amplitude and the phase of the complex vector.
 
     Parameters
     ----------
-    tsdata_1, tsdata_2 : 1d array or pycbc TimeSeries object
-                         The two input waveforms as timeseries
-                         vectors, the plus and cross polarized
-                         components.
-    delta_t : float
-              The timestepping delta_t.
+    tsdata_1, tsdata_2: 1d array or pycbc TimeSeries object
+                                            The two input waveforms as timeseries
+                                            vectors, the plus and cross polarized
+                                            components.
+    delta_t:    float
+                            The timestepping delta_t.
 
     Returns
     -------
-    amplitude : 1d array
-                A list containing complex amplitude
-                (list) and phase (list).
+    amplitude:  1d array
+                            A list containing complex amplitude
+                            (list) and phase (list).
     """
 
     return xtract_camp(tsdata_1, tsdata_2), xtract_cphase(tsdata_1, tsdata_2)
 
 
-def get_waveform_angular_frequency(
-    waveform, delta_t, timeaxis=None, method="FD"
-):
+def get_waveform_angular_frequency(waveform, delta_t, timeaxis=None, method="FD"):
     """Get the angular frequency of the waveform given
     the complex waveform time step. The phase is
     extracted and is differentiated using one of
     the available methods to compute the angular
     frequency.
 
     Parameters
     ----------
-    waveform : 1d array
-               The 1d complex array of the input waveform.
-    delta_t : float
-              The time step.
-    timeaxis : 1d array, optional
-               The time axis of the waveform.
-               Recommended especially when the sampling
-               is non-uniform and Chebyshev method is chosen.
-    method : str
-             The method for computing the derivative.
-             Can be `FD` or `CS`. See below for more
-             information.
+    waveform:   1d array
+                            The 1d complex array of the input waveform.
+
+    delta_t:    float
+                            The time step.
+
+    timeaxis:   1d array, optional
+                            The time axis of the waveform.
+                            Recommended especially when the sampling
+                            is non-uniform and Chebyshev method is chosen.
+    method:     str
+                            The method for computing the derivative.
+                            Can be `FD` or `CS`. See below for more
+                            information.
 
     Returns
     -------
-    omega : 1d array
-            The real instantaneous frequency of the waveform.
+    omega:      1d array
+                            The real instantaneous frequency of the waveform.
+
+
 
     Notes
     -----
     Available methods
 
-    Chebyshev series (`CS`) : The phase is expanded in
-                              a Chebyshev series and
-    Finite Differencing (`FD`) : A 11 point finite difference
-                                 scheme is used to differentiate
-                                 the phase, and is then smoothened
-                                 using the Savgol filter.
+    Chebyshev series (`CS`):    The phase is expanded in
+                                                            a Chebyshev series and
+    Finite Differencing (`FD`): A 11 point finite difference
+                                                            scheme is used to differentiate
+                                                            the phase, and is then smoothened
+                                                            using the Savgol filter.
     """
     # Get the real and imaginary parts.
     waveform_p = waveform.real
     waveform_x = waveform.imag
     # Get the phase
     phase = xtract_cphase(waveform_p, waveform_x)
     # Compute the derivative
@@ -1217,25 +1191,26 @@
 
 def get_starting_angular_frequency(waveform, delta_t, npoints=400):
     """Get the approximate starting frequency of the
     input data by averaging over the first `npoints` number of points.
 
     Parameters
     ----------
-    waveform : 1d array
-               The 1d complex array of the input waveform.
-    delta_t : float
-              The time step.
-    npoints : int
-              The number of points to average over.
+    waveform:   1d array
+                            The 1d complex array of the input waveform.
+    delta_t:    float
+                            The time step.
+    npoints:    int
+                            The number of points to average over.
 
     Returns
     -------
-    omega0 : float
-             The approximate starting angular frequency.
+    omega0:     float
+                            The approximate starting angular frequency.
+
 
     Notes
     -----
     Please suppy a conditioned input waveform that is neatly clipped,
     and not tapered.
     """
 
@@ -1250,23 +1225,24 @@
 
 # Simple overlap. #Error. Add frequency domain overlap computation.
 def olap(data1, data2, psd=1):
     """Calcuate the overlap between two data vectors weighted by the given psd.
 
     Parameters
     ----------
-    data1, data2 : 1d array or a pycbc RimeSeries object
-                   The input waveforms
-    psd : 1d array
-          The power spectral density to weight.
+
+    data1, data2:   1d array or a pycbc RimeSeries object
+                                    The input waveforms
+    psd:            1d array
+                                    The power spectral density to weight.
 
     Returns
     -------
-    overlap : float
-              The overlap divided by the psd.
+    overlap:        float
+                                    The overlap divided by the psd.
     """
 
     if psd == 1:
         data1 = np.array(data1)
         data2 = np.array(data2)
         overlap = np.sum(data1 * data2) / psd
 
@@ -1277,23 +1253,23 @@
 
 
 def norm(hdat, psd=1.0):
     """Calculate the norm of a vector.
 
     Parameters
     ----------
-    hdat : 1d array or a pycbc TimeSeries object.
-           The input waveform.
-    psa : 1d array
-          The noise power spectral density of the inner product.
+    hdat:   1d array or a pycbc TimeSeries object.
+                    The input waveform.
+    psa:    1d array
+                    The noise power spectral density of the inner product.
 
     Returns
     -------
-    norm_f : float
-             The norm with weighting by the psd.
+    norm_f: float
+                    The norm with weighting by the psd.
     """
 
     hdat = np.array(hdat)
 
     norm_f = np.sqrt(np.sum(hdat * hdat) / np.array(psd))
 
     # message("Norm is %f"%normfa)
@@ -1349,27 +1325,21 @@
                              The pair of indices denoting the start
                              and end points of an array
     """
 
     try:
         start_index = np.where(np.array(data) != 0)[0][0]
     except BaseException:
-        message(
-            colored("Warning! Start index not found!!", "red"),
-            message_verbosity=1,
-        )
+        message(colored("Warning! Start index not found!!", "red"), message_verbosity=1)
         start_index = 0
 
     try:
         end_index = np.where(np.array(data) != 0)[0][-1] + 1
     except BaseException:
-        message(
-            colored("Warning! End index not found!!", "red"),
-            message_verbosity=1,
-        )
+        message(colored("Warning! End index not found!!", "red"), message_verbosity=1)
         end_index = 0
     return start_index, end_index
 
 
 def apxstartend(data, tol=1e-5):
     """Identify the Approximate start and endpoints of the data.
 
@@ -1416,23 +1386,19 @@
            The waveform data as list or numpy array or pycbc timeseries.
     zeros : int
             The number of zeros to be added.
 
     Returns
     -------
     data : 1darray
-           data with `zeros` number of zeros concatenated
+           data with `zeros` number of zeros concatenated 
            at the end as numpy 1d array
     """
 
-    return np.transpose(
-        np.concatenate(
-            (np.transpose(np.array(data)), np.transpose(np.zeros([zeros])))
-        )
-    )
+    return np.transpose(np.concatenate((np.transpose(np.array(data)), np.transpose(np.zeros([zeros])))))
 
 
 def removezeros(data, delta_t):
     """Remove zeros from the input waveform from either sides.
     Similar to startend but return the truncated array.
 
     Parameters
@@ -1441,36 +1407,30 @@
            The input waveform.
     delta_t : float, optional
               The time stepping.
 
     Returns
     -------
     short_ts : a list
-               A list containing waveforms with zeros
+               A list containing waveforms with zeros 
                removed on either sides,
                the start and end indices in the format [short_ts, [start_index, end_index]]
 
     """
 
     # Assign the timestep. Real and imaginary parts are assumed to have same
     # timestep.
     if not delta_t:
         try:
             delta_t = data.delta_t
         except BaseException:
-            message(
-                "Input is not a TimeSeries."
-                " Please supply gridspacing as delta_t",
-                message_verbosity=0,
-            )
+            message("Input is not a TimeSeries." " Please supply gridspacing as delta_t", message_verbosity=0)
 
     starti, endi = startend(data)
-    ret_data = pycbc.types.timeseries.TimeSeries(
-        np.array(data)[starti:endi], delta_t
-    )
+    ret_data = pycbc.types.timeseries.TimeSeries(np.array(data)[starti:endi], delta_t)
 
     short_ts = [ret_data, [starti, endi]]
 
     return short_ts
 
 
 def shorten(tsdata, start, end, delta_t=None):
@@ -1497,30 +1457,22 @@
     # are assumed to have same
 
     # timestep.
     if not delta_t:
         try:
             delta_t = tsdata.delta_t
         except BaseException:
-            message(
-                "Input is not a TimeSeries."
-                "Please supply gridspacing as delta_t",
-                message_verbosity=0,
-            )
+            message("Input is not a TimeSeries." "Please supply gridspacing as delta_t", message_verbosity=0)
 
-    short_ts = pycbc.types.timeseries.TimeSeries(
-        np.array(tsdata)[start:end], delta_t
-    )
+    short_ts = pycbc.types.timeseries.TimeSeries(np.array(tsdata)[start:end], delta_t)
 
     return short_ts
 
 
-def taper_tanh(
-    waveform, time_axis=None, delta_t=None, duration=10, sides="both"
-):
+def taper_tanh(waveform, time_axis=None, delta_t=None, duration=10, sides="both"):
     """
     Taper a waveform with a :math:`tanh` function
     at either ends
 
     Parameters
     ----------
     waveform : 1d array
@@ -1580,44 +1532,33 @@
     # end_axis   = np.linspace(1, -1, nend_points)
 
     # norm_time_axis = time_axis/max(time_axis)
 
     # n_delta_t = delta_t/data_len
 
     # from scipy.interpolate import interpolate
-    waveform_widened = np.concatenate(
-        (np.zeros([nstart_points]), waveform, np.zeros([nend_points - 1]))
-    )
+    waveform_widened = np.concatenate((np.zeros([nstart_points]), waveform, np.zeros([nend_points - 1])))
     new_time_axis = np.linspace(
-        time_axis[0] - nstart_points * delta_t,
-        time_axis[-1] + nend_points * delta_t,
-        len(waveform_widened),
+        time_axis[0] - nstart_points * delta_t, time_axis[-1] + nend_points * delta_t, len(waveform_widened)
     )
 
-    start_win = (
-        np.tanh(3 * (new_time_axis - duration / 2) / (duration / 2)) + 1
-    ) / 2
-    end_win = (
-        np.tanh(3 * (-new_time_axis + (tfinal - duration / 2)) / (duration / 2))
-        + 1
-    ) / 2
+    start_win = (np.tanh(3 * (new_time_axis - duration / 2) / (duration / 2)) + 1) / 2
+    end_win = (np.tanh(3 * (-new_time_axis + (tfinal - duration / 2)) / (duration / 2)) + 1) / 2
 
     # plt.scatter(new_time_axis, waveform_widened, s=1)
     # plt.show()
 
     if sides == "both":
         tapered_waveform = start_win * end_win * waveform_widened
     elif sides == "beg":
         tapered_waveform = start_win * waveform_widened
     elif sides == "end":
         tapered_waveform = end_win * waveform_widened
     else:
-        message(
-            "Please specify valid sides argument. Sides can be beg, end or both."
-        )
+        message("Please specify valid sides argument. Sides can be beg, end or both.")
 
     # plt.scatter(new_time_axis, tapered_waveform, s=1)
     # plt.show()
 
     return new_time_axis, tapered_waveform
 
 
@@ -1664,21 +1605,17 @@
 
     # Append the zeros
     tapered_data = np.array(tapered_data)
 
     # Pad ends with extra zeros
     zeros = np.zeros([zeros])
     # Prepend with z zeros
-    tapered_data = np.transpose(
-        np.concatenate((np.transpose(zeros), np.transpose(tapered_data)))
-    )
+    tapered_data = np.transpose(np.concatenate((np.transpose(zeros), np.transpose(tapered_data))))
     # Append with extra zeros
-    tapered_data = np.transpose(
-        np.concatenate((np.transpose(tapered_data), np.transpose(zeros)))
-    )
+    tapered_data = np.transpose(np.concatenate((np.transpose(tapered_data), np.transpose(zeros))))
 
     # Convert back to timeseries if the input was a time series.
     tapered_data = pycbc.types.timeseries.TimeSeries(tapered_data, delta_t)
 
     # Return the timeseries
     return tapered_data
 
@@ -1754,53 +1691,47 @@
     if not delta_t:
         try:
             delta_t = wvp.delta_t
         except AttributeError:
             try:
                 delta_t = wvc.delta_t
             except BaseException:
-                message(
-                    "Input is not a TimeSeries."
-                    "Please supply gridspacing as delta_t",
-                    message_verbosity=0,
-                )
+                message("Input is not a TimeSeries." "Please supply gridspacing as delta_t", message_verbosity=0)
 
     datap = np.array(wvp)
     datac = np.array(wvc)
 
     # Assign the complex amplitude
     amp = np.power(datap, 2) + np.power(datac, 2)
     # Find the location of the max amplitude
     ind = np.where(amp == np.max(amp))[0][0]
     # Calculate the epoch
     tlim = [-ind * delta_t, (len(datap) - ind) * delta_t]
     # Returns the centered wvp and wvc if wvc was provided else returns just
     # the former.
 
     if flag == 1:
-        centered_wf = pycbc.types.timeseries.TimeSeries(
-            datap, delta_t, epoch=tlim[0]
-        )
+        centered_wf = pycbc.types.timeseries.TimeSeries(datap, delta_t, epoch=tlim[0])
     else:
         centered_wf = (
             pycbc.types.timeseries.TimeSeries(datap, delta_t, epoch=tlim[0]),
             pycbc.types.timeseries.TimeSeries(datac, delta_t, epoch=tlim[0]),
         )
 
     return centered_wf
 
 
 def get_centered_taxis(time_ax, amps):
-    """Get the time axis of the waveform centered
+    """Get the time axis of the waveform centered 
     at its maximum absolute amplitude.
 
     Parameters
     ----------
     time_ax : 1d array
-              The 1d array containg the original
+              The 1d array containg the original 
               (uncentered)time axis of the wveform.
 
     amps : 1d array
            The amplitude of the waveform.
 
     Returns
     -------
@@ -1844,17 +1775,16 @@
     plt.xlabel("xdata")
     plt.ylabel("f(x)")
     if save != "no":
         plt.savefig(save + ".pdf")
     plt.show()
     return 1
 
-
 def coalignwfs(tsdata1, tsdata2, delta_t=None):
-    """Coalign two timeseries. Wrapper and modification around
+    """Coalign two timeseries. Wrapper and modification around 
     pycbc functions with some additional functionalities.
 
     Parameters
     ----------
     tsdata1, tsdata2 : list, 1d array or a pycbc TimeSeries
                        The two data vectors as 1d lists or
                        numpy arrays or pycbc TimeSeries
@@ -1889,19 +1819,15 @@
     if not delta_t:
         try:
             delta_t = tsdata1.delta_t
         except AttributeError:
             try:
                 delta_t = tsdata2.delta_t
             except BaseException:
-                message(
-                    "Input is not a TimeSeries."
-                    "Please supply gridspacing as delta_t",
-                    message_verbosity=0,
-                )
+                message("Input is not a TimeSeries." "Please supply gridspacing as delta_t", message_verbosity=0)
 
     tsdata1, tsdata2, _ = lengtheq(tsdata1, tsdata2, delta_t, is_ts=True)
 
     # Calculate complex SNR using pycbc function. Note: This complex SNR is
     # actually the complex SNR * norm of the timeseries.
     csnr = pycbc.filter.matchedfilter.matched_filter(tsdata1, tsdata2)
     # Find the absolute value of the complex SNR timeseries
@@ -1996,48 +1922,34 @@
 
     # match,shift=pycbc.filter.matchedfilter.match(tsdata1,tsdata2)
 
     # Normalize the waveforms
     norm1 = norm(np.array(tsdata1[start:end]))
     norm2 = norm(np.array(tsdata2[start:end]))
 
-    tsdata1_cropped = pycbc.types.timeseries.TimeSeries(
-        np.array(tsdata1[start:end]) / norm1, delta_t
-    )
-    tsdata2_cropped = pycbc.types.timeseries.TimeSeries(
-        np.array(tsdata2[start:end]) / norm2, delta_t
-    )
+    tsdata1_cropped = pycbc.types.timeseries.TimeSeries(np.array(tsdata1[start:end]) / norm1, delta_t)
+    tsdata2_cropped = pycbc.types.timeseries.TimeSeries(np.array(tsdata2[start:end]) / norm2, delta_t)
 
-    max_match, max_shift = pycbc.filter.matchedfilter.match(
-        tsdata1_cropped, tsdata2_cropped
-    )
+    max_match, max_shift = pycbc.filter.matchedfilter.match(tsdata1_cropped, tsdata2_cropped)
 
-    tsdata1 = pycbc.types.timeseries.TimeSeries(
-        np.array(tsdata1) / norm1, delta_t
-    )
-    tsdata2 = pycbc.types.timeseries.TimeSeries(
-        np.array(tsdata2) / norm2, delta_t
-    )
+    tsdata1 = pycbc.types.timeseries.TimeSeries(np.array(tsdata1) / norm1, delta_t)
+    tsdata2 = pycbc.types.timeseries.TimeSeries(np.array(tsdata2) / norm2, delta_t)
 
     # Calculate complex SNR using pycbc function. Note: This complex SNR is
     # actually the complex SNR * norm of the timeseries.
     csnr = pycbc.filter.matchedfilter.matched_filter(tsdata1, tsdata2)
 
     # Find the absolute value of the complex SNR timeseries
     acsnr = np.array(np.abs(csnr))
     # message(acsnr,np.max(acsnr))
 
     # Find the location of the maximum element in acsnr
     maxloc = (np.where(acsnr == np.max(acsnr)))[0][0]
     mmatch = np.amax(acsnr)
-    message(
-        f"Max location is {maxloc},"
-        f"match is {mmatch}"
-        f"max shift is {max_shift}"
-    )
+    message(f"Max location is {maxloc}," f"match is {mmatch}" f"max shift is {max_shift}")
 
     # Shift the waveform 1 in time using maxloc
     tsdata1 = shiftmatched(tsdata1, maxloc, delta_t, is_ts=True)
 
     # Phase shift ( rotate) the waveform 1 by multipying
     # the frequency series of waveform 1 with the phase
     # of the max element in acsnr
@@ -2047,27 +1959,19 @@
     rotation = csnr[maxloc] / np.absolute(csnr[maxloc])
 
     # Rotate and take the inverse Fourier transform
     ctsdata1 = (rotation * tsdata1.to_frequencyseries()).to_timeseries()
 
     # Recenter waveform 0 and assign the timeaxis of waveform 0 to waveform1
     ctsdata1, dummy = center(ctsdata1, ctsdata1)
-    tsdata2 = pycbc.types.timeseries.TimeSeries(
-        np.array(tsdata2), tsdata2.delta_t, epoch=ctsdata1.sample_times[0]
-    )
+    tsdata2 = pycbc.types.timeseries.TimeSeries(np.array(tsdata2), tsdata2.delta_t, epoch=ctsdata1.sample_times[0])
 
     # Return the normalized, time and phase shifted waveform 1 to coalign with
     # 2 and waveform 2.
-    aligned_waveforms = {
-        "wf1": ctsdata1,
-        "wf2": tsdata2,
-        "norms": [norm1, norm2],
-        "shift": maxloc,
-        "match": max_match,
-    }
+    aligned_waveforms = {"wf1": ctsdata1, "wf2": tsdata2, "norms": [norm1, norm2], "shift": maxloc, "match": max_match}
 
     return aligned_waveforms
 
 
 def resample_wfs(both_time_axes, both_waveforms, delta_t="auto", Plot=False):
     """Resample the waveform pairs.
 
@@ -2163,15 +2067,15 @@
     Returns
     -------
     match_details : dict
                                                                                                                                                                                                                                                                     A dictionary containing the
                                                                                                                                                                                                                                                                     i). match coeffient
                                                                                                                                                                                                                                                                     ii). time_shift
                                                                                                                                                                                                                                                                     iii). phase shift in radians
-                                                                                                                                                                                                                                                                    iv). normalized, resampled, waveforms
+                                                                                                                                                                                                                                                                    iv). normalized, resampled, waveforms 
                            and their time-axes.
 
     Note
     ----
     The shifts give by how much the first waveform has to be shifted to match with the second.
 
     """
@@ -2192,17 +2096,15 @@
 
             # delta_t = min(delta_t_A, delta_t_B)
         elif delta_t == "A":
             delta_t = delta_t_A
         elif delta_t == "B":
             delta_t = delta_t_B
         else:
-            raise ValueError(
-                f"Did not understand speification for delta_t {delta_t}"
-            )
+            raise ValueError(f"Did not understand speification for delta_t {delta_t}")
 
     # message(type(time_axis1), type(time_axis2))
     # message(time_axis1-time_axis2)
     # message(time_axis1==time_axis2)
 
     # Don't interpolate if the time axis are identical
     Interp = True
@@ -2218,17 +2120,15 @@
             # tsorted = sorted(time_axis1)
             # delta_t = tsorted[0] - tsorted[1]
 
             # delta_t = mode(np.diff(time_axis1))
 
     if Interp is True:
         message("Interpolating time axis")
-        time_axis, wf1, wf2 = resample_wfs(
-            all_time_axes, all_waveforms, delta_t
-        )
+        time_axis, wf1, wf2 = resample_wfs(all_time_axes, all_waveforms, delta_t)
         # message(time_axis, wf1, wf2)
 
     from waveformtools.transforms import compute_fft, compute_ifft
 
     # The Fspace waveforms
     faxis, wf1_tilde = compute_fft(wf1, delta_t)
     _, wf2_tilde = compute_fft(wf2, delta_t)
@@ -2246,17 +2146,15 @@
     # max_snr = np.amax(Acsnr)
 
     Tshift_rec = (len(time_axis) - Tshift_rec_index) * delta_t
     # Phase shift
     Pshift_rec = csnr[Tshift_rec_index] / np.absolute(csnr[Tshift_rec_index])
     Pshift_rec_rad = np.log(Pshift_rec) / (1j)
 
-    message(
-        "-----------------------------------\n Shift information for waveform 2 against 1 \n"
-    )
+    message("-----------------------------------\n Shift information for waveform 2 against 1 \n")
     message(f"Recovered Time shift: {Tshift_rec}")
     message(f"Recovered Phase shift: {Pshift_rec}, {Pshift_rec_rad} in radians")
     message("-----------------------------------")
 
     # Apply the time shift to the second waveform
 
     if Tshift_rec_index != 0:
@@ -2278,17 +2176,15 @@
 
     norm1 = np.sqrt(np.sum(wf1 * np.conjugate(wf1)))
     norm2 = np.sqrt(np.sum(wf2_TPrec * np.conjugate(wf2_TPrec)))
 
     waveform1_aligned = wf1 / norm1
     waveform2_aligned = wf2_TPrec / norm2
 
-    match_score = np.sum(
-        waveform1_aligned * np.conjugate(waveform2_aligned)
-    )  # max_snr/(norm1*norm2)
+    match_score = np.sum(waveform1_aligned * np.conjugate(waveform2_aligned))  # max_snr/(norm1*norm2)
 
     match_details = {
         "match_score": match_score,
         "time_shift": Tshift_rec,
         "phase_shift": Pshift_rec_rad,
         "time": time_axis,
         "aligned_waveforms": [waveform1_aligned, waveform2_aligned],
@@ -2406,17 +2302,15 @@
 
     mlen = min(len(wf1_aligned_cropped), len(wf2_shifted))
 
     waveform1_aligned = wf1_aligned_cropped[:mlen] / norm1
     waveform2_aligned = wf2_shifted[:mlen] / norm2
 
     aligned_time_axis = aligned_time_axis[:mlen]
-    match_score = np.dot(
-        wf1_aligned_cropped[:mlen], np.conjugate(wf2_shifted[:mlen])
-    ) / (norm1 * norm2)
+    match_score = np.dot(wf1_aligned_cropped[:mlen], np.conjugate(wf2_shifted[:mlen])) / (norm1 * norm2)
 
     match_details = {
         "match_score": match_score,
         "time_shift": shift * delta_t,
         "phase_shift": phase_shift,
         "time": aligned_time_axis,
         "aligned_waveforms": [waveform1_aligned, waveform2_aligned],
@@ -2427,86 +2321,69 @@
 
 def simplematch_wfs_old(waveforms, delta_t=None):
     """Simple match the given waveforms. Does not clip the waveforms at either ends.
 
     Parameters
     ----------
     waveforms : list
-                A list of pairs [waveform A, waveform B] of waveforms.
+				A list of pairs [waveform A, waveform B] of waveforms.
     delta_t : float, optional
-              The time stepping.
+			  The time stepping.
 
     Notes
     -----
     The time stepping delta_t is the same for each pair of waveforms in the list.
 
     Returns
     -------
     match : list
             A list of dicts [{ Aligned waveforms} ,
-                            {match score (float), shift (number)}]
-            containing the match information for all the input waveform pairs.
+							{match score (float), shift (number)}]
+			containing the match information for all the input waveform pairs.
     """
 
     match = []
     # Iterate over (signal,template) pairs in waveforms
     for waveformdat in waveforms:
         # Carryout the match
         if not delta_t:
             try:
                 delta_t = waveformdat[0].delta_t
             except BaseException:
-                message(
-                    "Waveform is not a pycbc TimeSeries."
-                    "Please provide the gridspacing delt"
-                )
+                message("Waveform is not a pycbc TimeSeries." "Please provide the gridspacing delt")
                 sys.exit(0)
         # Match procedure
         # signaldat = lengtheq(waveformdat[0], waveformdat[1], delta_t)
-        waveform1, waveform2, _ = lengtheq(
-            waveformdat[0], waveformdat[1], delta_t
-        )
+        waveform1, waveform2, _ = lengtheq(waveformdat[0], waveformdat[1], delta_t)
 
         # waveform1 = signaldat[0]
         # waveform2 = signaldat[1]
 
         # alignedwvs = pycbc.waveform.utils.coalign_waveforms(signaldat,hpa)
         # Compute the match to calculate match and shift.
         # Note: The match function from pycbc returns the match of the
         # normalized templates
-        (match_score, shift) = pycbc.filter.matchedfilter.match(
-            waveform1, waveform2
-        )
+        (match_score, shift) = pycbc.filter.matchedfilter.match(waveform1, waveform2)
 
         # Coalign the waveforms using pycbc coalign.
-        waveform1, waveform2 = pycbc.waveform.utils.coalign_waveforms(
-            waveform1, waveform2
-        )
+        waveform1, waveform2 = pycbc.waveform.utils.coalign_waveforms(waveform1, waveform2)
 
         # Normalize the waveforms
 
         waveform1 = waveform1 / norm(waveform1)
         waveform2 = waveform2 / norm(waveform2)
 
         try:
-            (match_score, shift) = pycbc.filter.matchedfilter.match(
-                waveform1, waveform2
-            )
+            (match_score, shift) = pycbc.filter.matchedfilter.match(waveform1, waveform2)
         except BaseException:
             message("Final match couldn't be found!")
             match_score = None
             shift = None
 
-        match.append(
-            {
-                "Waveforms": [waveform1, waveform2],
-                "Match score": match_score,
-                "Shift": shift,
-            }
-        )
+        match.append({"Waveforms": [waveform1, waveform2], "Match score": match_score, "Shift": shift})
     return match
 
 
 def pmmatch_wfs(waveforms, offset=25, crop=None):
     """
     Match function for post merger waveforms.
 
@@ -2524,22 +2401,22 @@
                 The pairs of waveforms to match
                 in the format
                 [[wf1_pair1, wf2_pair2], [wf1_pair_2, wf2_pair2], ...].
     offset : int
              Number of indices to shift the data.
     crop : string
            A string to decide how to crop the waveforms.
-           The available Options are 1. `signal` 2. `template` 3. `both`.
+		   The available Options are 1. `signal` 2. `template` 3. `both`.
 
     Returns
     -------
     matchdet : a list of dicts
-               A list of dictionaries.
+			   A list of dictionaries.
                Each contains
-                   1. the waveform pair,
+			       1. the waveform pair,
                    2. the match score,
                    3. the shift index. to maximize the match.
 
     """
     matchdet = []
     for waveformdat in waveforms:
         signal, template = waveformdat
@@ -2580,33 +2457,23 @@
             delta_t = template.delta_t
         except BaseException:
             delta_t = 1
             template = pycbc.types.timeseries.TimeSeries(template, delta_t)
 
         # message(type(signal), type(template))
         # Align the waveforms in phase
-        signal_al, template_al = pycbc.waveform.utils.coalign_waveforms(
-            signal, template
-        )
+        signal_al, template_al = pycbc.waveform.utils.coalign_waveforms(signal, template)
 
         # message(np.where(np.array(signalp_al)!=0))
 
         # Compute the match score
-        (matchscore, finalshift) = pycbc.filter.matchedfilter.match(
-            signal_al, template_al
-        )
+        (matchscore, finalshift) = pycbc.filter.matchedfilter.match(signal_al, template_al)
 
         # message('+ The match score, shift are %f, %d'%(matchscore, finalshift))
-        matchdet.append(
-            {
-                "Waveforms": [signal_al, template_al],
-                "Match score": matchscore,
-                "Shift": finalshift,
-            }
-        )
+        matchdet.append({"Waveforms": [signal_al, template_al], "Match score": matchscore, "Shift": finalshift})
 
     return matchdet
 
 
 def roll(tsdata, i_roll, is_ts=False):
     """Roll the data circularly. Circular counterpart of shiftmatched function.
 
@@ -2616,15 +2483,15 @@
             1D data vector in the form of a list/ numpy array or timeseries.
     i_roll : int
              The number of indices to roll the array.
 
     Returns
     -------
     rolled_waveform : 1d array or(pycbc TimeSeries object
-                      The rolled wavefrom.
+					  The rolled wavefrom.
     """
 
     flag = 0
     if is_ts:
         try:
             # Assign the time step.
             delta_t = tsdata.delta_t
@@ -2636,44 +2503,39 @@
     tsdata = np.array(tsdata)
     # Break the array into two parts as last i + first i entries.
     arr1 = tsdata[-i_roll:]
     arr2 = tsdata[:-i_roll]
     # Join the two arrays and return them
     if flag == 1:
         rolled_waveform = pycbc.types.timeseries.TimeSeries(
-            np.transpose(
-                np.concatenate((np.transpose(arr1), np.transpose(arr2)))
-            ),
-            delta_t,
+            np.transpose(np.concatenate((np.transpose(arr1), np.transpose(arr2)))), delta_t
         )
 
     else:
-        rolled_waveform = np.transpose(
-            np.concatenate((np.transpose(arr1), np.transpose(arr2)))
-        )
+        rolled_waveform = np.transpose(np.concatenate((np.transpose(arr1), np.transpose(arr2))))
 
     return rolled_waveform
 
 
 def smoothen(func_x, win, order, xdata=None, to_plot=False):
     """Use the Savitzky-Golay Filter to smoothen the data.
 	Show the plots if plot=`yes`.
 
 	Parameters
     ----------
     func_x : 1d array
-             The y axis.
-    win :  int
-          Window for smoothening. Must be odd.
+			 The y axis.
+	win :  int
+		  Window for smoothening. Must be odd.
     order : int
             The order of the polynomial used for interpolation.
-    x : 1d array, optional.
-        The 1D list or numpy array, to plot the smoothened function.
-        Only required if to_plot=True.
-    to_plot : bool
+	x : 1d array, optional.
+		The 1D list or numpy array, to plot the smoothened function.
+		Only required if to_plot=True.
+	to_plot : bool
               True or False. Whether or not to display the plot.
 
     Returns
     -------
     ydata : 1d array
             The Savgol filtered list.
 
@@ -2697,55 +2559,47 @@
     """Function to bin the data and interpolate it at specified width and order.
 
     Parameters
     ----------
     xdata :  1d array
              1D list or numpy array.
     func_x : 1d array
-             The y axis.
+			 The y axis.
     width : int
-            Window size for smoothening,
+			Window size for smoothening,
     order : int
-            Order of the polynomial used for interpolation.
+			Order of the polynomial used for interpolation.
     to_plot : bool
-              True or False. To plot or not plot the results.
+			  True or False. To plot or not plot the results.
 
     Returns
     -------
     hist : list
            [binloc, yvals], The location of the bins and
-           the y values associated with the bins.
+		   the y values associated with the bins.
 
     """
 
     # Interpolation orders
     kind = [0, "linear", "quadratic", "cubic"]
     # Parse width
     width = int(width)
     # Number of bins
     nbins = int(len(xdata) / width)
     # Location of the bins
-    binloc = [
-        np.mean(xdata[width * index : width * index + width])
-        for index in range(0, nbins + 1)
-    ]
+    binloc = [np.mean(xdata[width * index : width * index + width]) for index in range(0, nbins + 1)]
     # message(binloc)
     # Assigning y values to the bins
-    yvals = [
-        np.mean(func_x[width * index : width * index + width])
-        for index in range(0, nbins + 1)
-    ]
+    yvals = [np.mean(func_x[width * index : width * index + width]) for index in range(0, nbins + 1)]
     # Assigning x values to the smoothened data
     # xf=x[width:-(width)/2]
     y_final = yvals
     # Interpolate if specified order is more than 0
     if order != 0:
-        y_interp_func = scipy.interpolate.interp1d(
-            binloc, yvals, kind=kind[order]
-        )
+        y_interp_func = scipy.interpolate.interp1d(binloc, yvals, kind=kind[order])
     # Reassign yf
     y_final = y_interp_func(binloc)
     # Set xf to binloc if order=0
     # if order==0:
     #       xf=binloc
     # y = signal.savgol_filter(func_x,win,order)
     if to_plot:
@@ -2765,20 +2619,20 @@
     """Function to smoothen data. Moving average over the window width.
 
     Parameters
     ----------
     func_x : 1d array
              A list or numpy array of y axis.
     Width : int
-            The width of the moving average window.
+			The width of the moving average window.
 
     Returns
     -------
     func_x_avgd : 1d array
-                  1D array of moving averaged y axis.
+				  1D array of moving averaged y axis.
 
     """
 
     # message(len(func_x))
     # List to store smoothened data
     func_x_avgd = []
     # Calculate the moving-average upto last but width num of points
@@ -2797,46 +2651,43 @@
 def interpolate_wfs(ts_data, interp_func, delta_t=None, **kwargs):
     """Function to interpolate a list of timeseries data using
     the user specified interp_func function and the keyword arguments.
 
     Parameters
     ----------
     ts_data : list
-              The 1d data. A list of waveforms
-              as a list or numpy array or
-              pycbc TimeSeries.
+			  The 1d data. A list of waveforms
+			  as a list or numpy array or
+		      pycbc TimeSeries.
     interp_fun : function
                 An interpolating function.
     delta_t : float
-              Timestep.
+			  Timestep.
     ``**kwargs`` : keyword arguments
-                   additional arguments to the user specified interp_func.
+				   additional arguments to the user specified interp_func.
 
     Returns
     -------
     interp_data : list
-                  A list containing interpolated data.
+				  A list containing interpolated data.
 
     """
 
     # List for storing the interpolated data function
     interp_data = []
     # Loop over items in input
     for wfs in ts_data:
         if not delta_t:
             try:
                 # Find sampling time_step
                 delta_t = wfs.delta_t
                 timeaxis = wfs.sample_times
 
             except BaseException:
-                message(
-                    "Input is not a TimeSeries. Please supply gridspacing as delta_t",
-                    message_verbosity=0,
-                )
+                message("Input is not a TimeSeries. Please supply gridspacing as delta_t", message_verbosity=0)
         else:
             timeaxis = np.arange(0, len(wfs) * delta_t, delta_t)
 
         # Interpolate using the supplied function. The keyword arguments
         # supplied to the fuction are the keyword arguments to be supplied
         # to the interpolating function)
         # Append to the list of interpolated data function
@@ -2848,90 +2699,78 @@
 def resample(interp_data, new_delta_t, epoch, length, old_delta_t=None):
     """Function to generate timeseries out of the given interpolated data
     function, epoch,sampling frequency, length(duration).
 
     Parameters
     ----------
     interp_data : 1d array
-                  The yaxis to be interpolated.
+				  The yaxis to be interpolated.
     epoch : float
-            The starting point in time.
+			The starting point in time.
     delta_t : float
-              New grid spacing to be sampled at.
+			  New grid spacing to be sampled at.
     length : int
              The duration of x axis.
 
     Returns
     -------
 
     data : list
-           A list containing resampled data as pycbc TimeSeries.
+		   A list containing resampled data as pycbc TimeSeries.
     """
 
     data = []
     # Loop over objects in interp_data
     for i in range(len(interp_data)):
         if not old_delta_t:
             try:
                 old_delta_t = interp_data[i].delta_t
 
             except BaseException:
-                message(
-                    "Input is not a TimeSeries. Please supply gridspacing as delta_t",
-                    message_verbosity=0,
-                )
+                message("Input is not a TimeSeries. Please supply gridspacing as delta_t", message_verbosity=0)
         else:
-            interp_data[i] = pycbc.types.timeseries.TimeSeries(
-                interp_data[i], old_delta_t
-            )
+            interp_data[i] = pycbc.types.timeseries.TimeSeries(interp_data[i], old_delta_t)
 
         # Prepare timeaxis
         timeaxis = np.linspace(epoch, epoch + length, int(length / new_delta_t))
         # Append the timeseries to the data list
         ydata = interp_data[i](timeaxis)
-        data.append(
-            pycbc.types.timeseries.TimeSeries(ydata, new_delta_t, epoch=epoch)
-        )
+        data.append(pycbc.types.timeseries.TimeSeries(ydata, new_delta_t, epoch=epoch))
     # Return the list of samples timeseries
     return data
 
 
 def interp_resam_wfs(wavf_data, old_taxis, new_taxis, kind="cubic", k=None):
     """Wrapper function for interpolation and resampling.
 
     Parameters
     ----------
     wavf_data : 1d array
                 The yaxis to be interpolated,
     old_taxis, new_taxis : 1darray
-                           Old and New time axis.
+						   Old and New time axis.
 
     Returns
     -------
     resam_wf_data : 1d array
                     Interpolated and resampled data.
     """
     # from scipy.interpolate import interp1d
 
     amp, phase = xtract_camp_phase(wavf_data.real, wavf_data.imag)
 
     # Interpolate
     if k is not None:
-        from scipy.interpolate import (
-            InterpolatedUnivariateSpline as interpolator,
-        )
+        from scipy.interpolate import InterpolatedUnivariateSpline as interpolator
 
         interp_amp_data = interpolator(old_taxis, amp, k=k)
         amp_res = interp_amp_data.get_residual()
         interp_phase_data = interpolator(old_taxis, phase, k=k)
         phase_res = interp_phase_data.get_residual()
-        message(
-            f"Amplitude residue {amp_res} \t Phase residue {phase_res}",
-            message_verbosity=2,
-        )
+        message(f"Amplitude residue {amp_res} \t Phase residue {phase_res}", message_verbosity=2)
     else:
         from scipy.interpolate import interp1d as interpolator
 
         interp_amp_data = interpolator(old_taxis, amp, kind=kind)
         interp_phase_data = interpolator(old_taxis, phase, kind=kind)
 
     # Resample
@@ -2959,17 +2798,15 @@
     1 : int
         The progress bar is messageed to stdout.
     """
 
     if normalize == "yes":
         final_progress = 98
         normalized_total_counts = final_progress * 10
-        present_count = int(
-            normalized_total_counts * present_count / total_counts
-        )
+        present_count = int(normalized_total_counts * present_count / total_counts)
         total_counts = normalized_total_counts
 
     # present_count = comm.gather(count,root=rank)
     else:
         final_progress = int(total_counts / 10)
 
     present_stage = int(present_count / 10)
```

### Comparing `waveformtools-2023.6.3/waveformtools.egg-info/PKG-INFO` & `waveformtools-2023.6.5/waveformtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waveformtools
-Version: 2023.6.3
+Version: 2023.6.5
 Summary:  Tools for working with numerical relativity and waveforms data 
 Home-page: https://gitlab.com/vaishakp/waveformtools
 Author: Vaishak Prasad
 Author-email: Vaishak Prasad <vaishakprasad@gmail.com>
 Project-URL: Homepage, https://gitlab.com/vaishakp/waveformtools
 Project-URL: Bug Tracker, https://gitlab.com/vaishakp/waveformtools/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `waveformtools-2023.6.3/waveformtools.egg-info/SOURCES.txt` & `waveformtools-2023.6.5/waveformtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

