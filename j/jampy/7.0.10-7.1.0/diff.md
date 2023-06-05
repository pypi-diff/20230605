# Comparing `tmp/jampy-7.0.10.tar.gz` & `tmp/jampy-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jampy-7.0.10.tar", last modified: Tue Jan 17 13:55:40 2023, max compression
+gzip compressed data, was "jampy-7.1.0.tar", last modified: Mon Jun  5 17:20:37 2023, max compression
```

## Comparing `jampy-7.0.10.tar` & `jampy-7.1.0.tar`

### file list

```diff
@@ -1,43 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-01-17 13:55:40.161073 jampy-7.0.10/
--rw-rw-rw-   0        0        0    47873 2023-01-17 13:55:40.161073 jampy-7.0.10/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-01-17 13:55:40.119930 jampy-7.0.10/jampy/
--rw-rw-rw-   0        0        0    11176 2023-01-17 13:55:25.000000 jampy-7.0.10/jampy/CHANGELOG.rst
--rw-rw-rw-   0        0        0      442 2022-12-26 20:25:49.000000 jampy-7.0.10/jampy/LICENSE.txt
--rw-rw-rw-   0        0        0     3564 2022-10-02 22:25:04.000000 jampy-7.0.10/jampy/README.rst
--rw-rw-rw-   0        0        0       26 2023-01-17 13:55:25.000000 jampy-7.0.10/jampy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-17 13:55:40.150727 jampy-7.0.10/jampy/examples/
--rw-rw-rw-   0        0        0       36 2018-04-16 16:12:03.000000 jampy-7.0.10/jampy/examples/__init__.py
--rw-rw-rw-   0        0        0     1019 2022-02-07 11:29:21.000000 jampy-7.0.10/jampy/examples/cappellari2020_table1.txt
--rw-rw-rw-   0        0        0     3075 2023-01-17 13:32:59.000000 jampy-7.0.10/jampy/examples/jam_axi_intr_example.py
--rw-rw-rw-   0        0        0     4482 2023-01-13 18:55:40.000000 jampy-7.0.10/jampy/examples/jam_axi_proj_example.py
--rw-rw-rw-   0        0        0     6926 2022-06-27 18:41:13.000000 jampy-7.0.10/jampy/examples/jam_black_hole_bayes_example.py
--rw-rw-rw-   0        0        0    10309 2022-10-03 13:56:27.000000 jampy-7.0.10/jampy/examples/jam_dark_halo_bayes_example.py
--rw-rw-rw-   0        0        0     8459 2022-10-02 16:38:44.000000 jampy-7.0.10/jampy/examples/jam_hernquist_model_example.py
--rw-rw-rw-   0        0        0     8544 2018-05-01 13:45:20.000000 jampy-7.0.10/jampy/examples/jam_mock_kinematics_black_hole.txt
--rw-rw-rw-   0        0        0     8592 2021-12-21 19:35:32.000000 jampy-7.0.10/jampy/examples/jam_mock_kinematics_dark_halo.txt
--rw-rw-rw-   0        0        0     2445 2023-01-15 17:31:12.000000 jampy-7.0.10/jampy/examples/jam_sph_proj_example.py
--rw-rw-rw-   0        0        0     2119 2021-09-21 10:34:36.000000 jampy-7.0.10/jampy/examples/mge_vcirc_example.py
--rw-rw-rw-   0        0        0    33702 2023-01-17 13:49:03.000000 jampy-7.0.10/jampy/jam_axi_intr.py
--rw-rw-rw-   0        0        0    44294 2023-01-17 13:54:48.000000 jampy-7.0.10/jampy/jam_axi_proj.py
--rw-rw-rw-   0        0        0     7826 2023-01-16 17:32:37.000000 jampy-7.0.10/jampy/jam_sph_intr.py
--rw-rw-rw-   0        0        0    28116 2023-01-17 12:16:18.000000 jampy-7.0.10/jampy/jam_sph_proj.py
-drwxrwxrwx   0        0        0        0 2023-01-17 13:55:40.161073 jampy-7.0.10/jampy/legacy/
--rw-rw-rw-   0        0        0       36 2018-04-16 16:12:03.000000 jampy-7.0.10/jampy/legacy/__init__.py
--rw-rw-rw-   0        0        0    28671 2023-01-17 13:09:02.000000 jampy-7.0.10/jampy/legacy/jam_axi_rms.py
--rw-rw-rw-   0        0        0    36547 2022-07-15 10:12:52.000000 jampy-7.0.10/jampy/legacy/jam_axi_vel.py
--rw-rw-rw-   0        0        0      192 2022-10-02 21:34:07.000000 jampy-7.0.10/jampy/legacy/jam_sph_rms.py
--rw-rw-rw-   0        0        0     6547 2022-10-09 17:30:15.000000 jampy-7.0.10/jampy/mge_half_light_isophote.py
--rw-rw-rw-   0        0        0     3568 2019-10-24 18:03:59.000000 jampy-7.0.10/jampy/mge_radial_density.py
--rw-rw-rw-   0        0        0     3173 2019-06-12 10:26:52.000000 jampy-7.0.10/jampy/mge_radial_mass.py
--rw-rw-rw-   0        0        0     6845 2023-01-01 15:05:41.000000 jampy-7.0.10/jampy/mge_vcirc.py
--rw-rw-rw-   0        0        0    18627 2023-01-17 13:46:17.000000 jampy-7.0.10/jampy/quad1d.py
--rw-rw-rw-   0        0        0    12204 2023-01-01 15:01:54.000000 jampy-7.0.10/jampy/quad2d.py
-drwxrwxrwx   0        0        0        0 2023-01-17 13:55:40.130228 jampy-7.0.10/jampy.egg-info/
--rw-rw-rw-   0        0        0    47873 2023-01-17 13:55:39.000000 jampy-7.0.10/jampy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1042 2023-01-17 13:55:40.000000 jampy-7.0.10/jampy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-17 13:55:39.000000 jampy-7.0.10/jampy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-01-17 13:55:39.000000 jampy-7.0.10/jampy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-01-17 13:55:39.000000 jampy-7.0.10/jampy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-01-17 13:55:39.000000 jampy-7.0.10/jampy.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-01-17 13:55:40.161073 jampy-7.0.10/setup.cfg
--rw-rw-rw-   0        0        0     1750 2021-06-24 13:30:54.000000 jampy-7.0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 17:20:37.984359 jampy-7.1.0/
+-rw-rw-rw-   0        0        0    50165 2023-06-05 17:20:37.984359 jampy-7.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-05 17:20:37.921410 jampy-7.1.0/jampy/
+-rw-rw-rw-   0        0        0    12746 2023-06-05 16:56:47.000000 jampy-7.1.0/jampy/CHANGELOG.rst
+-rw-rw-rw-   0        0        0      442 2022-12-26 20:25:49.000000 jampy-7.1.0/jampy/LICENSE.txt
+-rw-rw-rw-   0        0        0     3564 2022-10-02 22:25:04.000000 jampy-7.1.0/jampy/README.rst
+-rw-rw-rw-   0        0        0       23 2023-06-05 17:20:30.000000 jampy-7.1.0/jampy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 17:20:37.984359 jampy-7.1.0/jampy/examples/
+-rw-rw-rw-   0        0        0       36 2018-04-16 16:12:03.000000 jampy-7.1.0/jampy/examples/__init__.py
+-rw-rw-rw-   0        0        0     1019 2022-02-07 11:29:21.000000 jampy-7.1.0/jampy/examples/cappellari2020_table1.txt
+-rw-rw-rw-   0        0        0     3060 2023-06-04 08:12:29.000000 jampy-7.1.0/jampy/examples/jam_axi_intr_example.py
+-rw-rw-rw-   0        0        0     4517 2023-06-01 10:17:18.000000 jampy-7.1.0/jampy/examples/jam_axi_proj_example.py
+-rw-rw-rw-   0        0        0     6915 2023-06-05 17:03:23.000000 jampy-7.1.0/jampy/examples/jam_black_hole_bayes_example.py
+-rw-rw-rw-   0        0        0    10298 2023-06-05 17:02:41.000000 jampy-7.1.0/jampy/examples/jam_dark_halo_bayes_example.py
+-rw-rw-rw-   0        0        0    10196 2023-06-04 08:26:08.000000 jampy-7.1.0/jampy/examples/jam_hernquist_model_example.py
+-rw-rw-rw-   0        0        0     8544 2018-05-01 13:45:20.000000 jampy-7.1.0/jampy/examples/jam_mock_kinematics_black_hole.txt
+-rw-rw-rw-   0        0        0     8592 2021-12-21 19:35:32.000000 jampy-7.1.0/jampy/examples/jam_mock_kinematics_dark_halo.txt
+-rw-rw-rw-   0        0        0     2592 2023-05-31 18:23:57.000000 jampy-7.1.0/jampy/examples/jam_sph_proj_example.py
+-rw-rw-rw-   0        0        0     2195 2023-06-05 17:01:53.000000 jampy-7.1.0/jampy/examples/mge_vcirc_example.py
+-rw-rw-rw-   0        0        0    37662 2023-06-05 17:18:24.000000 jampy-7.1.0/jampy/jam_axi_intr.py
+-rw-rw-rw-   0        0        0    48571 2023-06-05 17:18:24.000000 jampy-7.1.0/jampy/jam_axi_proj.py
+-rw-rw-rw-   0        0        0     8141 2023-05-31 18:20:50.000000 jampy-7.1.0/jampy/jam_sph_intr.py
+-rw-rw-rw-   0        0        0    29072 2023-05-31 18:20:50.000000 jampy-7.1.0/jampy/jam_sph_proj.py
+-rw-rw-rw-   0        0        0     6547 2022-10-09 17:30:15.000000 jampy-7.1.0/jampy/mge_half_light_isophote.py
+-rw-rw-rw-   0        0        0     3568 2019-10-24 18:03:59.000000 jampy-7.1.0/jampy/mge_radial_density.py
+-rw-rw-rw-   0        0        0     3173 2019-06-12 10:26:52.000000 jampy-7.1.0/jampy/mge_radial_mass.py
+-rw-rw-rw-   0        0        0     6845 2023-01-01 15:05:41.000000 jampy-7.1.0/jampy/mge_vcirc.py
+-rw-rw-rw-   0        0        0    18603 2023-06-04 08:26:08.000000 jampy-7.1.0/jampy/quad1d.py
+-rw-rw-rw-   0        0        0    12204 2023-01-01 15:01:54.000000 jampy-7.1.0/jampy/quad2d.py
+drwxrwxrwx   0        0        0        0 2023-06-05 17:20:37.953084 jampy-7.1.0/jampy.egg-info/
+-rw-rw-rw-   0        0        0    50165 2023-06-05 17:20:37.000000 jampy-7.1.0/jampy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      933 2023-06-05 17:20:37.000000 jampy-7.1.0/jampy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 17:20:37.000000 jampy-7.1.0/jampy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-06-05 17:20:37.000000 jampy-7.1.0/jampy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-05 17:20:37.000000 jampy-7.1.0/jampy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-06-05 17:20:37.000000 jampy-7.1.0/jampy.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-06-05 17:20:37.984359 jampy-7.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1750 2021-06-24 13:30:54.000000 jampy-7.1.0/setup.py
```

### Comparing `jampy-7.0.10/PKG-INFO` & `jampy-7.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jampy
-Version: 7.0.10
+Version: 7.1.0
 Summary: JamPy: Jeans Anisotropic Models for Galactic Dynamics
 Home-page: https://purl.org/cappellari/software
 Author: Michele Cappellari
 Author-email: michele.cappellari@physics.ox.ac.uk
 License: Other/Proprietary License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -133,22 +133,25 @@
   `Cappellari (2020) <https://ui.adsabs.harvard.edu/abs/2020MNRAS.494.4819C>`_
 
 Calling Sequence
 ----------------
 
 .. code-block:: python
 
+    from jampy.jam_axi_proj import jam_axi_proj
+
     jam = jam_axi_proj(
              surf_lum, sigma_lum, qobs_lum, surf_pot, sigma_pot, qobs_pot,
              inc, mbh, distance, xbin, ybin, align='cyl', analytic_los=True,
              beta=None, data=None, epsrel=1e-2, errors=None, flux_obs=None,
-             gamma=None, goodbins=None, interp=True, kappa=None, ml=None,
-             moment='zz', nang=10, nlos=1500, nodots=False, normpsf=1.,
-             nrad=20, pixang=0., pixsize=0., plot=True, quiet=False,
-             rbh=0.01, sigmapsf=0., step=0., vmax=None, vmin=None)
+             gamma=None, goodbins=None, interp=True, kappa=None,
+             logistic=False, ml=None, moment='zz', nang=10, nlos=1500,
+             nodots=False, normpsf=1., nrad=20, pixang=0., pixsize=0.,
+             plot=True, quiet=False, rbh=0.01, sigmapsf=0., step=0.,
+             vmax=None, vmin=None)
 
     vrms = jam.model  # with moment='zz' the output is the LOS Vrms
 
     jam.plot()   # Generate data/model comparison when data is given
 
 See more examples in the ``jampy/examples`` folder inside
 `site-packages <https://stackoverflow.com/a/46071447>`_.
@@ -251,15 +254,15 @@
 beta: array_like with shape (n,) or (4,)
     Radial anisotropy of the individual kinematic-tracer MGE Gaussians
     (Default: ``beta=np.zeros(n)``)::
 
         beta = 1 - (sigma_th/sigma_r)^2  # with align='sph'
         beta = 1 - (sigma_z/sigma_R)^2   # with align='cyl'
 
-    When ``len(beta) == 4`` the procedure assumes::
+    When ``logistic=True`` the procedure assumes::
 
         beta = [r_a, beta_0, beta_inf, alpha]
 
     and the anisotropy of the whole JAM model varies as a logistic
     function of the logarithmic spherical radius (with ``align='sph'``) or
     of the logarithmic distance from the equatorial plane (with ``align='cyl'``)::
 
@@ -268,14 +271,16 @@
 
     Here ``beta_0`` represents the anisotropy at ``r = 0``, ``beta_inf``
     is the anisotropy at ``r = inf`` and ``r_a`` is the anisotropy
     transition radius, with ``alpha`` controlling the sharpness of the
     transition. In the special case ``beta_0 = 0, beta_inf = 1, alpha = 2``
     the anisotropy variation reduces to the form by Osipkov & Merritt, but
     the extra parameters allow for much more realistic anisotropy profiles.
+    See an application in `Simon, Cappellari & Hartke (2023)
+    <https://ui.adsabs.harvard.edu/abs/2023arXiv230318229S>`_.
 data: array_like with shape (p,), optional
     observed first or second velocity moment used to fit the model.
 
     EXAMPLE: In the common case where one has only line-of-sight velocities
     the second moment is given by::
 
         Vrms = np.sqrt(velBin**2 + sigBin**2)
@@ -304,15 +309,15 @@
 gamma: array_like with shape (n,)
     tangential anisotropy of the individual kinematic-tracer MGE Gaussians
     (Default: ``gamma=np.zeros(n)``)::
 
         gamma = 1 - (sigma_phi/sigma_r)^2  # with align='sph'
         gamma = 1 - (sigma_phi/sigma_R)^2  # with align='cyl'
 
-    When ``len(gamma) == 4`` the procedure assumes::
+    When ``logistic=True`` the procedure assumes::
 
         gamma = [r_a, gamma_0, gamma_inf, alpha]
 
     and the anisotropy of the whole JAM model varies as a logistic
     function of the logarithmic spherical radius (with ``align='sph'``) or
     of the logarithmic distance from the equatorial plane (with ``align='cyl'``)::
 
@@ -346,14 +351,19 @@
     to compute all moments, including proper motions,  simultaneously.
 kappa: float, optional
     When ``kappa=None`` (default) the first velocity moments are scaled in
     such a way that the projected angular momentum of the data and model is
     the same [equation 52 of `Cappellari (2008)`_].
     When ``kappa=1`` the model first velocity moments are output without
     any scaling.
+logistic: bool, optional
+    When ``logistic=True``, JAM interprets the anisotropy parameters
+    ``beta`` and ``gamma`` as defining a 4-parameters logistic function.
+    See the documentation of the anisotropy keywords for details.
+    (Default ``logistic=False``)
 ml: float, optional
     Mass-to-light ratio (M/L) to multiply the values given by ``surf_pot``.
     Setting this keyword is completely equivalent to multiplying the
     output ``model`` by ``np.sqrt(M/L)`` after the fit. This implies that
     the BH mass is also scaled and becomes ``mbh*ml``.
 
     If ``ml=None`` (default) the M/L is fitted from the data and the
@@ -427,15 +437,17 @@
     PSF convolution is not performed.
 plot: bool
     When ``data is not None`` setting this keyword produces a plot with the
     data/model comparison at the end of the calculation.
 quiet: bool
     Set this keyword to avoid printing values on the console.
 rbh: float, optional
-    This scalar gives the sigma in arcsec of the Gaussian representing the
+    This keyword is ignored unless ``align='cyl'`` and `analytic_los=True`.
+    In all other cases JAM assume a point-like central black hole.
+    This scalar gives the sigma in arcsec of the Gaussian approximating the
     central black hole of mass MBH [See Section 3.1.2 of `Cappellari (2008)`_]
     The gravitational potential is indistinguishable from a point source
     for ``radii > 2*rbh``, so the default ``rbh=0.01`` arcsec is appropriate
     in most current situations.
 
     When using different units as input, e.g. pc instead of arcsec, one
     should check that ``rbh`` is not too many order of magnitude smaller
@@ -542,20 +554,22 @@
   `Cappellari (2020) <https://ui.adsabs.harvard.edu/abs/2020MNRAS.494.4819C>`_
 
 Calling Sequence
 ----------------
 
 .. code-block:: python
 
+    from jampy.jam_axi_intr import jam_axi_intr
+
     jam = jam_axi_intr(
              dens_lum, sigma_lum, qintr_lum, dens_pot, sigma_pot, qintr_pot,
-             mbh, Rbin, zbin, align='cyl', beta=None, data=None,
-             epsrel=1e-2, errors=None, gamma=None, goodbins=None,
-             interp=True, ml=None, nang=10, nodots=False, nrad=20,
-             plot=True, proj_cyl=False, quiet=False, rbh=1)
+             mbh, Rbin, zbin, align='cyl', beta=None, data=None, epsrel=1e-2,
+             errors=None, gamma=None, goodbins=None, interp=True,
+             logistic=False, ml=None, nang=10, nodots=False, nrad=20,
+             plot=True, proj_cyl=False, quiet=False)
 
     # The meaning of the output is different depending on `align`
     sig2R, sig2z, sig2phi, v2phi = jam.model  # with align='cyl'
     sig2r, sig2th, sig2phi, v2phi = jam.model  # with align='sph'
 
     jam.plot()   # Generate data/model comparison
 
@@ -611,15 +625,15 @@
 beta: array_like with shape (n,) or (4,)
     Vector with the axial anisotropy of the individual kinematic-tracer
     MGE Gaussians (Default: ``beta=np.zeros(n)``)::
 
         beta = 1 - (sigma_th/sigma_r)^2  # with align='sph'
         beta = 1 - (sigma_z/sigma_R)^2   # with align='cyl'
 
-    When ``len(beta) == 4`` the procedure assumes::
+    When ``logistic=True`` the procedure assumes::
 
         beta = [r_a, beta_0, beta_inf, alpha]
 
     and the anisotropy of the whole JAM model varies as a logistic
     function of the logarithmic spherical radius (with ``align='sph'``) or
     of the logarithmic distance from the equatorial plane (with ``align='cyl'``)::
 
@@ -628,14 +642,16 @@
 
     Here ``beta_0`` represents the anisotropy at ``r = 0``, ``beta_inf``
     is the anisotropy at ``r = inf`` and ``r_a`` is the anisotropy
     transition radius, with ``alpha`` controlling the sharpness of the
     transition. In the special case ``beta_0 = 0, beta_inf = 1, alpha = 2``
     the anisotropy variation reduces to the form by Osipkov & Merritt, but
     the extra parameters allow for much more realistic anisotropy profiles.
+    See an application in `Simon, Cappellari & Hartke (2023)
+    <https://ui.adsabs.harvard.edu/abs/2023arXiv230318229S>`_.
 data: array_like of shape (4, p), optional
     Four input vectors with the observed values of:
 
     - ``[sigR, sigz, sigphi, vrms_phi]`` in ``km/s``, when ``align='cyl'``
       (or ``align='sph'`` and ``proj_cyl=True``).
 
       ``vrms_phi`` is the square root of the velocity second moment in the
@@ -655,15 +671,15 @@
 gamma: array_like with shape (n,)
     Vector with the tangential anisotropy of the individual kinematic-tracer
     MGE Gaussians (Default: ``gamma=np.zeros(n)``)::
 
         gamma = 1 - (sigma_phi/sigma_r)^2  # with align='sph'
         gamma = 1 - (sigma_phi/sigma_R)^2  # with align='cyl'
 
-    When ``len(gamma) == 4`` the procedure assumes::
+    When ``logistic=True`` the procedure assumes::
 
         gamma = [r_a, gamma_0, gamma_inf, alpha]
 
     and the anisotropy of the whole JAM model varies as a logistic
     function of the logarithmic spherical radius (with ``align='sph'``) or
     of the logarithmic distance from the equatorial plane (with ``align='cyl'``)::
 
@@ -681,14 +697,19 @@
     for the bins which have to be included in the fit (if requested) and
     ``chi^2`` calculation (Default: fit all bins).
 interp: bool, optional
     If ``interp=False`` no interpolation is performed and the model is
     computed at every set of input (R, z) coordinates.
     If ``interp=True`` (default), the model is interpolated if the number
     of requested input (R, z) coordinates is larger than ``nang*nrad``.
+logistic: bool, optional
+    When ``logistic=True``, JAM interprets the anisotropy parameters
+    ``beta`` and ``gamma`` as defining a 4-parameters logistic function.
+    See the documentation of the anisotropy keywords for details.
+    (Default ``logistic=False``)
 ml: float, optional
     Mass-to-light ratio M/L. If ``ml=None`` (default) the M/L is fitted to
     the data and the best-fitting value is returned in output.
     The ``mbh`` is also scaled and becomes ``mbh*ml``.
     If ``ml=1`` no scaling is applied to the model.
 nang: int, optional
     The number of linearly-spaced intervals in the eccentric anomaly at
@@ -710,20 +731,14 @@
     ``[sig2R, sig2z, sig2phi, v2phi]`` components as in the case
     ``align='cyl'``. This is useful for a direct comparison of results with
     either the spherical or cylindrical alignment, as it allows one to fit
     the same data with both modelling assumptions.
 quiet: bool, optional
     If ``quiet=False`` (default), print the best-fitting M/L and chi2 at
     the end for the calculation.
-rbh: float, optional
-    This scalar gives the sigma in pc of the Gaussian representing the
-    central black hole of mass ``mbh`` [See Section 3.1.2 of
-    `Cappellari (2008)`_]. The gravitational potential is indistinguishable
-    from a point source for ``radii > 2*rbh``, so the default ``rbh=1`` pc
-    is appropriate for observations taken with current telescopes.
 
 Output Parameters
 -----------------
 
 Returned as attributes of the ``jam_axi_intr`` class.
 
 .chi2: float
@@ -784,14 +799,39 @@
 provided this copyright and disclaimer are included in all 
 copies of the software. All other rights are reserved.
 In particular, redistribution of the code is not allowed.
 
 Changelog
 =========
 
+V7.1.0: MC, Oxford, 1 June 2023
+    - Separated computation for the black hole kinematics for both the
+      cylindrically and spherically-aligned solutions. In both cases this
+      removed one numerical quadrature. This is useful in extreme situations,
+      when the minimum radius one wants to model around the black hole is orders
+      of magnitude smaller than the smallest MGE Gaussian. This change
+      eliminated the need for the ``rbh`` keyword in ``jam_axi_intr``, which I
+      removed. The only case where the black hole is still approximated with a
+      small Gaussian is in ``jam_axi_proj`` when both ``align='cyl'`` and
+      ``analytic_los=True``.
+    - Adopted consistent minimum radius, based on ``step``, for both the
+      intrinsic and projected interpolation grids.
+    - Simplified minimum-inclination test.
+    - Removed ``legacy`` folder with old redundant procedures.
+    - Moved the formalism for the LOS analytic integrand with ``align='cyl'``
+      into ``jam_axi_proj``.
+    - ``jam_axi_proj``, ``jam_axi_intr``, ``jam_sph_proj``, ``jam_sph_intr``:
+      New keyword ``logistic`` to specify when JAM should interpret the input
+      anisotropy parameters ``beta`` and ``gamma`` as defining a logistic
+      function anisotropy profile.
+    - ``jam_axi_intr``: Use DE quadrature from ``[z, inf]`` instead of
+      ``[0, 1]`` with ``align='cyl'`` as already done with ``align='sph'``.
+    - ``jam_hernquist_model_example``: New test against Osipkov-Merritt radial
+      variation of the anisotropy using ``logistic=True``. Revised plot.
+
 V7.0.10: MC, Oxford, 17 January 2023
     - Introduced an analytic radial variation of the anisotropy ``beta``
       and ``gamma`` using a flexible logistic function of logarithmic radius
       ``beta(r) = beta_0 + (beta_inf - beta_0)/[1 + (r_a/r)^alpha]``.
       This function specifies the inner/outer anisotropy ``beta_0`` and
       ``beta_inf``, the anisotropy radius ``r_a`` and the sharpness ``alpha``
       of the transition. This new function is an alternative to assigning
```

### Comparing `jampy-7.0.10/jampy/CHANGELOG.rst` & `jampy-7.1.0/jampy/CHANGELOG.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,35 @@
 Changelog
 =========
 
+V7.1.0: MC, Oxford, 1 June 2023
+    - Separated computation for the black hole kinematics for both the
+      cylindrically and spherically-aligned solutions. In both cases this
+      removed one numerical quadrature. This is useful in extreme situations,
+      when the minimum radius one wants to model around the black hole is orders
+      of magnitude smaller than the smallest MGE Gaussian. This change
+      eliminated the need for the ``rbh`` keyword in ``jam_axi_intr``, which I
+      removed. The only case where the black hole is still approximated with a
+      small Gaussian is in ``jam_axi_proj`` when both ``align='cyl'`` and
+      ``analytic_los=True``.
+    - Adopted consistent minimum radius, based on ``step``, for both the
+      intrinsic and projected interpolation grids.
+    - Simplified minimum-inclination test.
+    - Removed ``legacy`` folder with old redundant procedures.
+    - Moved the formalism for the LOS analytic integrand with ``align='cyl'``
+      into ``jam_axi_proj``.
+    - ``jam_axi_proj``, ``jam_axi_intr``, ``jam_sph_proj``, ``jam_sph_intr``:
+      New keyword ``logistic`` to specify when JAM should interpret the input
+      anisotropy parameters ``beta`` and ``gamma`` as defining a logistic
+      function anisotropy profile.
+    - ``jam_axi_intr``: Use DE quadrature from ``[z, inf]`` instead of
+      ``[0, 1]`` with ``align='cyl'`` as already done with ``align='sph'``.
+    - ``jam_hernquist_model_example``: New test against Osipkov-Merritt radial
+      variation of the anisotropy using ``logistic=True``. Revised plot.
+
 V7.0.10: MC, Oxford, 17 January 2023
     - Introduced an analytic radial variation of the anisotropy ``beta``
       and ``gamma`` using a flexible logistic function of logarithmic radius
       ``beta(r) = beta_0 + (beta_inf - beta_0)/[1 + (r_a/r)^alpha]``.
       This function specifies the inner/outer anisotropy ``beta_0`` and
       ``beta_inf``, the anisotropy radius ``r_a`` and the sharpness ``alpha``
       of the transition. This new function is an alternative to assigning
```

### Comparing `jampy-7.0.10/jampy/README.rst` & `jampy-7.1.0/jampy/README.rst`

 * *Files identical despite different names*

### Comparing `jampy-7.0.10/jampy/examples/cappellari2020_table1.txt` & `jampy-7.1.0/jampy/examples/cappellari2020_table1.txt`

 * *Files identical despite different names*

### Comparing `jampy-7.0.10/jampy/examples/jam_axi_intr_example.py` & `jampy-7.1.0/jampy/examples/jam_axi_intr_example.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,16 +56,16 @@
     """
     rr = np.linspace(0, 16, 32)
     zz = np.linspace(0, 6, 12)
     Rbin, zbin = map(np.ravel, np.meshgrid(rr, zz))
     w = (Rbin == 0) & (zbin == 0)
     Rbin, zbin = Rbin[~w], zbin[~w]  # Remove central singularity
     jampy_dir = path.dirname(path.realpath(jampy_package.__file__))
-    log_dens_lum, log_sigma_lum, qintr_lum = np.loadtxt(jampy_dir + '/examples/cappellari2020_table1.txt', unpack=True)
-    dens_lum, sigma_lum = 10**log_dens_lum, 10**log_sigma_lum
+    lg_dens_lum, lg_sigma_lum, qintr_lum = np.loadtxt(jampy_dir + '/examples/cappellari2020_table1.txt').T
+    dens_lum, sigma_lum = 10**lg_dens_lum, 10**lg_sigma_lum
 
     beta0 = -0.78
     sig2z, v2phi = satoh_solution(Rbin, zbin, beta0)
 
     gamma0 = 0.78
     beta = np.full_like(dens_lum, beta0)
     gamma = np.full_like(dens_lum, gamma0)
```

### Comparing `jampy-7.0.10/jampy/examples/jam_axi_proj_example.py` & `jampy-7.1.0/jampy/examples/jam_axi_proj_example.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     sigma = np.array([0.153, 0.515, 1.58, 4.22, 10, 22.4, 48.8, 105, 227, 525])
     qobs = np.full_like(sigma, 0.57)
 
     distance = 16.5     # Assume Virgo distance in Mpc (Mei et al. 2007)
     mbh = 1e8           # Black hole mass in solar masses
     beta = np.full_like(surf, 0.2)
 
-    # An alternative to setting the anisotropy of each individual Gaussian, one
+    # As alternative to setting the anisotropy of each individual Gaussian, one
     # can specify an analytic radial variation for the anisotropy, of the form
     #
     #   beta(r) = beta_0 + (beta_inf - beta_0)/[1 + (r_a/r)^alpha]    # with align='sph'
     #   beta(z) = beta_0 + (beta_inf - beta_0)/[1 + (z_a/|z|)^alpha]  # with align='cyl'
     #
     # by specifying beta as a list of 4-element as follows (see documentation):
     #
@@ -67,15 +67,15 @@
     # beta_0 = 0.2    # Inner anisotropy
     # beta_inf = 0.4  # Outer anisotropy
     # alpha = 1       # Sharpness of the anisotropy transition
     # beta = [r_a, beta_0, beta_inf, alpha]
 
     # Below I assume mass follows light, but in a real application one
     # will generally include a dark halo in surf_pot, sigma_pot, qobs_pot.
-    # See e.g. Cappellari (2013) for an example
+    # See jam_dark_halo_bayes_example.py and e.g. Cappellari (2013) for an example
     # https://ui.adsabs.harvard.edu/abs/2013MNRAS.432.1709C
 
     surf_lum = surf_pot = surf
     sigma_lum = sigma_pot = sigma
     qobs_lum = qobs_pot = qobs
 
     sigmapsf =  [0.6, 1.2]
```

### Comparing `jampy-7.0.10/jampy/examples/jam_black_hole_bayes_example.py` & `jampy-7.1.0/jampy/examples/jam_black_hole_bayes_example.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     # http://adsabs.harvard.edu/abs/2006MNRAS.366.1126C
     surf = 10**np.array([6.187, 5.774, 5.766, 5.613, 5.311, 4.774, 4.359, 4.087, 3.682, 3.316, 2.744, 1.618])
     sigma = 10**np.array([-1.762, -1.143, -0.839, -0.438, -0.104, 0.232, 0.560, 0.835, 1.160, 1.414, 1.703, 2.249])
     qObs = np.array([0.790, 0.741, 0.786, 0.757, 0.720, 0.724, 0.725, 0.743, 0.751, 0.838, 0.835, 0.720])
 
     # Read mock kinematics with realistic parameters and noise
     jam_dir = path.dirname(path.realpath(jam_package.__file__))
-    xbin, ybin, rms, erms, flux = np.loadtxt(jam_dir + "/examples/jam_mock_kinematics_black_hole.txt", unpack=True)
+    xbin, ybin, rms, erms, flux = np.loadtxt(jam_dir + "/examples/jam_mock_kinematics_black_hole.txt").T
     distance = 0.7   # M32 Distance
 
     # Here assume mass follows light
     surf_lum = surf_pot = surf
     sigma_lum = sigma_pot = sigma
     qobs_lum = qobs_pot = qObs
```

### Comparing `jampy-7.0.10/jampy/examples/jam_dark_halo_bayes_example.py` & `jampy-7.1.0/jampy/examples/jam_dark_halo_bayes_example.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,15 +161,15 @@
     # http://adsabs.harvard.edu/abs/2006MNRAS.366.1126C
     surf_lum = 10**np.array([6.187, 5.774, 5.766, 5.613, 5.311, 4.774, 4.359, 4.087, 3.682, 3.316, 2.744, 1.618])
     sigma_lum = 10**np.array([-1.762, -1.143, -0.839, -0.438, -0.104, 0.232, 0.560, 0.835, 1.160, 1.414, 1.703, 2.249])
     qobs_lum = np.array([0.790, 0.741, 0.786, 0.757, 0.720, 0.724, 0.725, 0.743, 0.751, 0.838, 0.835, 0.720])
 
     # Read mock kinematics with realistic parameters and noise
     jam_dir = path.dirname(path.realpath(jam_package.__file__))
-    xbin, ybin, rms, erms, flux = np.loadtxt(jam_dir + "/examples/jam_mock_kinematics_dark_halo.txt", unpack=True)
+    xbin, ybin, rms, erms, flux = np.loadtxt(jam_dir + "/examples/jam_mock_kinematics_dark_halo.txt").T
     distance = 0.7   # M32 Distance
 
     # The following line tries to *approximately* account for systematic errors.
     # See beginning of Sec.6.1 of Mitzkus+17 for an explanation
     # https://ui.adsabs.harvard.edu/abs/2017MNRAS.464.4789M
     erms *= (2*rms.size)**0.25
```

### Comparing `jampy-7.0.10/jampy/examples/jam_hernquist_model_example.py` & `jampy-7.1.0/jampy/examples/jam_hernquist_model_example.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     V2.0.0: Translated from IDL into Python. MC, Oxford, 9 April 2014
     V2.0.1: Fixed RuntimeWarning. MC, Oxford, 17 March 2017
     V2.0.2: Changed imports for jam as a package. MC, Oxford, 17 April 2018
     V2.1.0: Use the new jampy.jam_axi_proj. MC, Oxford, 28 April 2021
     V2.2.0 Included align='sph' models and plot legend.
         MC, Oxford, 30 April 2021
     V2.2.1: Adapted for new jam_sph_proj. MC Oxford, 3 October 2022
+    V2.3.0: Added Osipkov-Merritt test. MC, Oxford, 1 June 2023
 
 """
 
 import numpy as np
 import matplotlib.pyplot as plt
 
 from mgefit.mge_fit_1d import mge_fit_1d
@@ -54,15 +55,15 @@
     plt.pause(1)
 
     surf = m.sol[0]                 # Surface density in Msun/pc**2
     sigma = m.sol[1]/pc             # Gaussian dispersion in arcsec
     qObs = np.ones_like(surf)    # Assume spherical model
     inc = 90                        # Edge-on view
     npix = 100
-    rad = np.geomspace(0.01, 50, npix) # desired output radii in arcsec (avoid R=0)
+    rad = np.geomspace(0.1, 100, npix) # desired output radii in arcsec (avoid R=0)
     r = rad*pc
 
     ################## Circular Velocity #################
 
     plt.clf()
     plt.subplot(211)
     plt.xlabel('R (arcsec)')
@@ -71,15 +72,15 @@
 
     vcirc = mge_vcirc(surf, sigma, qObs, inc, mbh, distance, rad)
     plt.plot(rad, vcirc, 'C4', label=r'MGE V$_{\rm circ}$')
 
     # Compare with analytic result
     #
     vc = np.sqrt(G*M*r)/(r + a) # H90 equation (16)
-    plt.plot(rad, vc, 'C0-.', label='H90')
+    plt.plot(rad, vc, 'C0-.', label='Analytic')
     plt.text(30, 310, r'$V_{\rm circ}$')
 
     #################### Isotropic Vrms ###################
 
     # Spherical isotropic H90 model
     #
     jam = jam_sph_proj(surf, sigma, surf, sigma, mbh, distance, rad)
@@ -108,15 +109,14 @@
     # Projected second moments of isotropic model from H90
     #
     sigp = np.sqrt(G*M**2/(12*np.pi*a**3*IR) # H90 equation (41)
                  *(0.5/(1 - s**2)**3
                  *(-3*s**2*xs*(8*s**6 - 28*s**4 + 35*s**2 - 20)
                  - 24*s**6 + 68*s**4 - 65*s**2 + 6) - 6*np.pi*s))
     plt.plot(rad, sigp, 'C0-.')
-    plt.text(20, 90, r'$V_{\rm rms}(\beta=0)$ isotropic')
 
     ################### Anisotropic Vrms ##################
 
     # Projected second moments for a H90 model with sigma_R=0.
     # This implies beta=-Infinity but I adopt as an approximation
     # below a large negative beta. This explains why te curves do not
     # overlap perfectly.
@@ -142,18 +142,52 @@
     # Projected second moments of fully tangential model from H90
     #
     sigp = np.sqrt(G*M**2*r**2/(2*np.pi*a**5*IR) # H90 equation (42)
                  *(1./(24*(1 - s**2)**4)
                  *(-xs*(24*s**8 - 108*s**6 + 189*s**4 - 120*s**2 + 120)
                  - 24*s**6 + 92*s**4 - 117*s**2 + 154) + 0.5*np.pi/s))
     plt.plot(rad, sigp, 'C0-.')
-    plt.text(20, 200, r'$V_{\rm rms}(\beta\rightarrow-\infty)$ tangential')
 
     plt.legend()
 
+    ############### Osipkov-Merritt anisotropy variation ##############
+
+    beta0 = 0       # Isotropic in the centre
+    betainf = 1     # Fully radial at infinity
+    ra = a/pc       # anisotropy radius in arcsec
+    alpha = 2       # Osipkov-Merritt exponent
+    beta = [ra, beta0, betainf, alpha]
+    mbh = 0.005*M
+
+    # The 'rani' keyword selects the specialized Osipkov-Merritt analytic solution
+    sigp = jam_sph_proj(surf, sigma, surf, sigma, mbh, distance, rad, rani=ra).model
+
+    # Here I use the generic logistic anisotropy but with Osipkov-Merritt values
+    sigp1 = jam_sph_proj(surf, sigma, surf, sigma, mbh, distance, rad,
+                         beta=beta, logistic=1).model
+
+    # This is the axisymmetric model in the spherical limit and logistic anisotropy
+    vrms_r = jam_axi_proj(surf, sigma, qObs, surf, sigma, qObs, inc, mbh,
+                        distance, rad, rad*0, beta=beta, align='sph', logistic=1).model
+
+    plt.semilogx(rad, sigp1, 'C1')
+    plt.semilogx(rad, sigp, 'C0-.')
+    plt.semilogx(rad, vrms_r, 'C3:')
+
+    plt.annotate('Osipkov-Merritt+BH', xy=(0.8, 236), xycoords='data',
+                 xytext=(0.5, 300), textcoords='data',
+                 arrowprops=dict(facecolor='blue', ec='blue', arrowstyle="->"))
+    plt.annotate('$V_{\\rm rms}(\\beta=-20\\approx-\infty)$\nfully tangential',
+                 xy=(5, 160), xycoords='data', xytext=(2.6, 40), textcoords='data',
+                 arrowprops=dict(facecolor='blue', ec='blue', arrowstyle="->"))
+    plt.annotate('$V_{\\rm rms}(\\beta=0)$\nisotropic', xy=(28, 147),
+                 xycoords='data', xytext=(13, 210), textcoords='data',
+                 arrowprops=dict(facecolor='blue', ec='blue', arrowstyle="->"))
+    plt.axvline(ra, ls='--', c='grey')
+
     ############### Anisotropic models with Black Hole ###############
 
     # Reproduces Fig.4.20 of Binney J., & Tremaine S.D., 2008,
     # Galactic Dynamics, 2nd ed., Princeton University Press
     # See https://books.google.co.uk/books?id=6mF4CKxlbLsC&pg=PA352
 
     plt.subplot(212)
@@ -181,14 +215,15 @@
     # Test the isotropic jam_axi_proj(align='cyl') with Black Hole in the spherical limit
     #
     for bh in bhs:
         vrms = jam_axi_proj(surf, sigma, qObs, surf, sigma, qObs,
                             inc, bh, distance, rad, rad*0, align='cyl').model
         plt.semilogx(rad/a*pc, vrms/cost, 'C2--')
 
+    plt.axvline(1, ls='--', c='grey')
     plt.axis([0.006, 10, 0, 0.6]) # x0, x1, y0, y1
     plt.tight_layout()
 
     plt.text(0.4, 0.5, r'$M_{\rm BH}=[0, 0.2\%, 0.4\%]\, M_*$')
     plt.text(0.03, 0.15, r'$\beta$=-0.5 (tangential)')
     plt.text(.03, 0.35, r'$\beta$=0 (isotropic)')
     plt.text(0.03, 0.5, r'$\beta$=0.5 (radial)')
```

### Comparing `jampy-7.0.10/jampy/examples/jam_mock_kinematics_black_hole.txt` & `jampy-7.1.0/jampy/examples/jam_mock_kinematics_black_hole.txt`

 * *Files identical despite different names*

### Comparing `jampy-7.0.10/jampy/examples/jam_mock_kinematics_dark_halo.txt` & `jampy-7.1.0/jampy/examples/jam_mock_kinematics_dark_halo.txt`

 * *Files identical despite different names*

### Comparing `jampy-7.0.10/jampy/examples/jam_sph_proj_example.py` & `jampy-7.1.0/jampy/examples/jam_sph_proj_example.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 """
 
 import numpy as np
 import matplotlib.pyplot as plt
 
 from jampy.jam_sph_proj import jam_sph_proj
 
+##############################################################################
 def jam_sph_proj_example():
     """
     Usage example for jam_sph_proj().
     It takes about 1s on a 2.5 GHz computer
 
     """
     # Realistic MGE galaxy surface brightness.
@@ -47,16 +48,17 @@
     pixSize = 0.1           # Spaxel size in arcsec
     sigmapsf = [0.1, 0.6]   # sigma of the PSF in arcsec from AO observations
     normpsf = [0.7, 0.3]
     mbh = 2e8               # Black hole mass in solar masses before multiplication by M/L
     distance = 20.          # Mpc
 
     jam = jam_sph_proj(surf_pc, sigma_arcsec, surf_pc, sigma_arcsec, mbh,
-        distance, rad, beta=beta, sigmapsf=sigmapsf, normpsf=normpsf,
-        pixsize=pixSize, data=sig, errors=dsig, plot=True, tensor='los')
+                       distance, rad, beta=beta, sigmapsf=sigmapsf,
+                       normpsf=normpsf, pixsize=pixSize, data=sig, errors=dsig,
+                       plot=True, tensor='los', logistic=True)
     rms = jam.model
 
 ##############################################################################
 
 if __name__ == '__main__':
 
     plt.clf()
```

### Comparing `jampy-7.0.10/jampy/examples/mge_vcirc_example.py` & `jampy-7.1.0/jampy/examples/mge_vcirc_example.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,43 +13,44 @@
 from os import path
 import numpy as np
 import matplotlib.pyplot as plt
 
 import jampy as jampy_package
 from jampy.mge_vcirc import mge_vcirc
 
+##############################################################################
 def mge_vcirc_example():
     """
     Usage example for mge_vcirc()
     It takes a fraction of a second on a 2GHz computer
     
     """
     inc = 60.  # Inclination in degrees
     distance = 0.648/np.pi  # Mpc (adopt distance where 1" = 1pc)
     rad = np.geomspace(0.05, 100, 30)  # Radii in arscec where Vcirc has to be computed
 
     # Compute a projected MGE from the intrinsic one in Table 1 of Cappellari (2020)
     jampy_dir = path.dirname(path.realpath(jampy_package.__file__))
-    lg_dens, lg_sigma, qintr = np.loadtxt(jampy_dir + '/examples/cappellari2020_table1.txt', unpack=True)
+    lg_dens, lg_sigma, qintr = np.loadtxt(jampy_dir + '/examples/cappellari2020_table1.txt').T
     dens, sigma, inc_rad = 10**lg_dens, 10**lg_sigma, np.radians(inc)
     qobs = np.sqrt((qintr*np.sin(inc_rad))**2 + np.cos(inc_rad)**2)  # Eq.(35) Cappellari (2020)
     surf = np.sqrt(2*np.pi)*dens*qintr*sigma/qobs                    # Eq.(38) Cappellari (2020)
 
     G = 0.004301  # (km/s)^2 pc/Msun [6.674e-11 SI units (CODATA2018)]
     mbh = 0.01        # Assume a BH 1% of the galaxy mass M=1
     vtrue = np.sqrt(G*rad**2/(3 + rad**2)**1.5 + G*mbh/rad)  # Analytic V_c for M = a = b = 1
     vcirc = mge_vcirc(surf, sigma, qobs, inc, mbh, distance, rad)
 
-    plt.plot(np.log10(rad), vcirc, '-', label="Analytic")
+    plt.plot(np.log10(rad), vtrue, '-', label="Analytic")
     plt.plot(np.log10(rad), vcirc, 'o', label="MGE approximation")
     plt.xlabel('lg R (arcsec)')
     plt.ylabel(r'$V_{circ}$ (km/s)')
     plt.title(r"Circular velocity of Satoh model with $M=1$ and $M_{\rm BH}=M/100$")
     plt.legend(loc=3)
 
-#----------------------------------------------------------------------
+##############################################################################
 
 if __name__ == '__main__':
     
     plt.clf()
     mge_vcirc_example()
     plt.pause(1)
```

### Comparing `jampy-7.0.10/jampy/jam_axi_intr.py` & `jampy-7.1.0/jampy/jam_axi_intr.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 V1.0.0: Michele Cappellari, Oxford, 08 November 2019
     - Written and tested.
 Vx.x.x: Additional changes are documented in the CHANGELOG of the JamPy package.
 
 """
 import numpy as np
 import matplotlib.pyplot as plt
-from scipy import ndimage
+from scipy import ndimage, special
 from time import perf_counter as clock
 
 from plotbin.plot_velfield import plot_velfield
 from jampy.quad1d import quad1d
 from jampy.quad2d import quad2d
 
 ##############################################################################
@@ -53,94 +53,140 @@
     """ Density for each luminous Gaussian at (R, z) """
 
     nu = dens*np.exp(-0.5/sigma**2*(R**2 + (z/qintr)**2))  # Cappellari (2008) eq.(13)
 
     return nu
 
 ##############################################################################
+def intrinsic_moments_cyl_bh(R, z, dens_lum, sigma_lum, qintr_lum, mbh, beta, gamma):
+    """
+    Compute analytic intrinsic moments for the black hole alone
+
+    """
+    G = 0.004301    # (km/s)^2 pc/Msun [6.674e-11 SI units (CODATA2018)]
+    h = sigma_lum*qintr_lum*np.sqrt(2)
+    r = np.sqrt(R**2 + z**2)
+    nu = density(R, z, dens_lum, sigma_lum, qintr_lum)
+    nu /= nu.sum()
+    sig2z = G*mbh*nu*(1/r - special.erfcx(r/h)*np.sqrt(np.pi)/h)
+
+    bani = 1/(1 - beta)  # Anisotropy ratio b = (sig_R/sig_z)**2
+    sig2R = bani*sig2z
+    sig2phi = (1 - gamma)*sig2R
+    v2phi = G*mbh*R**2/r**3*(1 - bani)*nu \
+            + bani*(1 + (1 - qintr_lum**2)*(R/(sigma_lum*qintr_lum))**2)*sig2z
+
+    return sig2R.sum(), sig2z.sum(), sig2phi.sum(), v2phi.sum()
+
+##############################################################################
 
 def integrand_cyl(u, R, z,
                   dens_lum, sigma_lum, qintr_lum,
                   dens_pot, sigma_pot, qintr_pot,
-                  beta, gamma, component):
+                  beta, gamma, logistic, component):
     """
     Compute all the non-zero JAM first and second intrinsic velocity moments
     using the formulas from Cappellari (2008, MNRAS, 390, 71; hereafter C08).
     https://ui.adsabs.harvard.edu/abs/2008MNRAS.390...71C
 
     """
-    if len(beta) == 4 != dens_lum.size:
-        # Same variable anisotropy for all Gaussians
+    if logistic:        # Variable anisotropy, same for all Gaussians
         zab, beta0, betainf, alpha = beta
         beta = (beta0 + betainf*(abs(z)/zab)**alpha)/(1 + (abs(z)/zab)**alpha)
         bani = 1/(1 - beta)
-    else:
-        # Different but constant anisotropy per Gaussian
+    else:               # Constant anisotropy, different per Gaussian
         bani = 1/(1 - beta[:, None, None]) if np.ptp(beta) else 1/(1 - beta[0])  # Anisotropy ratio b = (sig_R/sig_z)**2
 
-    nu = density(R, z, dens_lum, sigma_lum, qintr_lum)[:, None, None]
-    s2_lum = (sigma_lum**2)[:, None, None]
-    q2_lum = (qintr_lum**2)[:, None, None]
+    dens_lum = dens_lum[:, None, None]
+    sigma_lum = sigma_lum[:, None, None]
+    qintr_lum = qintr_lum[:, None, None]
 
     dens_pot = dens_pot[None, :, None]
-    s2_pot = (sigma_pot**2)[None, :, None]
-    q2_pot = (qintr_pot**2)[None, :, None]
+    sigma_pot = sigma_pot[None, :, None]
+    qintr_pot = qintr_pot[None,:, None]
 
-    u2 = (u**2)[None, None, :]
+    # DE Change of variables for Chandrasekhar u-integral
+    # np.arcsinh(np.log([rmin, rmax])*2/np.pi) -> [0, inf]
+    x = np.exp(np.sinh(u)*np.pi/2)
+    duds = x*np.cosh(u)*np.pi/2
+    u = x[None, None, :]
+
+    # Tracer
+    R2, z2 = R**2, z**2
+    a = -1/(2*sigma_lum**2)
+    b = a/qintr_lum**2
+    exp1 = dens_lum*np.exp(a*R2 + b*z2)
 
-    s2q2_lum = s2_lum*q2_lum
-    e2_pot = 1 - q2_pot
+    # Mass
     G = 0.004301    # (km/s)^2 pc/Msun [6.674e-11 SI units (CODATA2018)]
+    u1, qu = 1 + u, qintr_pot**2 + u
+    tmp = -1/(2*sigma_pot**2)
+    c, d = tmp/u1, tmp/qu
+    upot = 2*np.pi*G*dens_pot*qintr_pot*sigma_pot**2/(u1*np.sqrt(qu))
+    exp2 = upot*np.exp(c*R2 + d*z2)
 
-    # Double summation over (j,k) for all values of integration variable u.
-    # Triple loop in (j,k,u) is replaced by broadcast Numpy array operations
-    p2 = 1 - e2_pot*u2
-    hj = np.exp(-0.5/s2_pot*u2*(R**2 + z**2/p2))/np.sqrt(p2)    # C08 eq.(17)
-    c = e2_pot - s2q2_lum/s2_pot                                # C08 eq.(22)
-    e = np.sqrt(q2_pot)*dens_pot*u2*hj
-    f = nu*(4*np.pi*G/(1 - c*u2))*e                             # Common sub-expression
+    bd = d/(b + d)
+    sig2z = exp1*exp2*bd
 
     if component == 'sig2R':
-        f *= bani*s2q2_lum                                      # C08 eq.(19)
-    elif component == 'sig2z':
-        f *= s2q2_lum
+        sig2z *= bani
     elif component == 'sig2phi':
-        if len(gamma) == 4 != dens_lum.size:
-            # Same variable anisotropy for all Gaussians
+        if logistic:        # Variable anisotropy, same for all Gaussians
             zag, gamma0, gammainf, alpha = gamma
             gamma = (gamma0 + gammainf*(abs(z)/zag)**alpha)/(1 + (abs(z)/zag)**alpha)
-        else:
-            # Different but constant anisotropy per Gaussian
+        else:               # Constant anisotropy, different per Gaussian
             gamma = gamma[:, None, None] if np.ptp(gamma) else gamma[0]  # Anisotropy gamma = 1 - (sig_phi/sig_R)**2
-        f *= (1 - gamma)*bani*s2q2_lum                          # C08 eq.(33)
+        sig2z *= (1 - gamma)*bani
     elif component == 'v2phi':
-        d = 1 - bani*q2_lum - ((1 - bani)*c + e2_pot*bani)*u2   # C08 eq.(23)
-        f *= bani*s2q2_lum + d*R**2                             # C08 eq.(21)
+        sig2z *= bani + 2*R2*((a + c)*bani - c/bd)
 
-    return f.sum((0, 1))
+    return duds*sig2z.sum((0, 1))
 
 ##############################################################################
-
 def intrinsic_moments_cyl(R, z,
                           dens_lum, sigma_lum, qintr_lum,
                           dens_pot, sigma_pot, qintr_pot,
-                          beta, gamma, epsrel):
+                          mbh, beta, gamma, logistic, epsrel):
     """ Numerical quadratures of the Jeans solution """
 
-    args = [R, z, dens_lum, sigma_lum, qintr_lum, dens_pot, sigma_pot, qintr_pot, beta, gamma]
+    mds, mxs = np.median(sigma_lum), np.max(sigma_lum)
+    xlim = np.arcsinh(np.log([1e-7*mds, 1e3*mxs])*2/np.pi)
+
+    args = [R, z, dens_lum, sigma_lum, qintr_lum, dens_pot, sigma_pot, qintr_pot, beta, gamma, logistic]
     nu = density(R, z, dens_lum, sigma_lum, qintr_lum).sum()
-    sig2R, sig2z, sig2phi, v2phi = \
-        [quad1d(integrand_cyl, [0, 1], epsrel=epsrel, singular=1, args=args+[txt]).integ/nu
-         for txt in ['sig2R', 'sig2z', 'sig2phi', 'v2phi']]
+    sig2z = quad1d(integrand_cyl, xlim, epsrel=epsrel, args=args+['sig2z']).integ/nu
+    v2phi = quad1d(integrand_cyl, xlim, epsrel=epsrel, args=args+['v2phi']).integ/nu
+
+    if (not logistic) and (np.ptp(beta) or np.ptp(gamma)):
+        sig2R = quad1d(integrand_cyl, xlim, epsrel=epsrel, args=args+['sig2R']).integ/nu
+        sig2phi = quad1d(integrand_cyl, xlim, epsrel=epsrel, args=args+['sig2phi']).integ/nu
+    else:
+        if logistic:
+            zab, beta0, betainf, alpha = beta
+            beta = (beta0 + betainf*(abs(z)/zab)**alpha)/(1 + (abs(z)/zab)**alpha)
+            zag, gamma0, gammainf, alpha = gamma
+            gamma = (gamma0 + gammainf*(abs(z)/zag)**alpha)/(1 + (abs(z)/zag)**alpha)
+        else:
+            beta = beta[0]
+            gamma = gamma[0]
+        sig2R = sig2z/(1 - beta)
+        sig2phi = sig2R*(1 - gamma)
+
+    if mbh > 0:
+        sig2R_bh, sig2z_bh, sig2phi_bh, v2phi_bh = intrinsic_moments_cyl_bh(
+            R, z, dens_lum, sigma_lum, qintr_lum, mbh, beta, gamma)
+        sig2R += sig2R_bh
+        sig2z += sig2z_bh
+        sig2phi += sig2phi_bh
+        v2phi += v2phi_bh
 
     return sig2R, sig2z, sig2phi, v2phi, nu
 
 ##############################################################################
-
-def integand_tan_dth_pot(u, r, th, dens_pot, sigma_pot, qintr_pot):
+def integand_tan_dth_pot(u, R2, z2, dens_pot, sigma_pot, qintr_pot):
     """
     Returns the integrand of the tan(th)*d(pot)/dth derivative
     of the MGE potential at (r, th).
     This is equation (51) of Cappellari (2020, MNRAS, 494, 4819)
     https://ui.adsabs.harvard.edu/abs/2020MNRAS.494.4819C
 
     """
@@ -149,24 +195,23 @@
     x = np.exp(np.sinh(u)*np.pi/2)
     duds = x*np.cosh(u)*np.pi/2
     u = x[:, None]
 
     G = 0.004301    # (km/s)^2 pc/Msun [6.674e-11 SI units (CODATA2018)]
     qu = qintr_pot**2 + u
     u1 = 1 + u
-    d = 2*np.pi*G*dens_pot*qintr_pot*(qintr_pot**2 - 1)*(r*np.sin(th))**2
-    e = np.exp(-0.5*(r/sigma_pot)**2*(np.sin(th)**2/u1 + np.cos(th)**2/qu))
+    d = 2*np.pi*G*dens_pot*qintr_pot*(qintr_pot**2 - 1)*R2
+    e = np.exp(-0.5/sigma_pot**2*(R2/u1 + z2/qu))
     tan_dth_pot = d*e/(u1**2*qu**1.5)
 
     return duds*tan_dth_pot.sum(1)   # u.size
 
 ##############################################################################
-
-def integrand_sph(s, t, r, th, dens_lum, sigma_lum, qintr_lum,
-                  dens_pot, sigma_pot, qintr_pot, beta, gamma, component):
+def integrand_sph(s, t, r, th, dens_lum, sigma_lum, qintr_lum, beta, gamma,
+                  logistic, dens_pot, sigma_pot, qintr_pot, component):
     """
     Solution of the spherically-aligned Jeans equations for an MGE
     from eq.(52)-(54) of Cappellari (2020, MNRAS, 494, 4819)
     https://ui.adsabs.harvard.edu/abs/2020MNRAS.494.4819C
 
     """
     dens_lum = dens_lum[:, None, None]
@@ -184,22 +229,20 @@
     u = x[None, None, :]
 
     # TANH Change of variables for Jeans r-integral (Sec.6.2 of Cappellari 2020)
     # np.log([rmin, rmax]) -> [r, inf]
     drdt = np.exp(t)
     r1 = r + drdt[None, None, :]
 
-    if len(beta) == 4 != dens_lum.size:
-        # Variable anisotropy, same for all Gaussians
+    if logistic:        # Variable anisotropy, same for all Gaussians
         rab, beta0, betainf, alpha = beta
         fun = (r1/r)**(2*beta0)
         fun *= ((1 + (r1/rab)**alpha)/(1 + (r/rab)**alpha))**(2*(betainf - beta0)/alpha)
         beta = beta0 + (betainf - beta0)/(1 + (rab/r)**alpha)
-    else:
-        # Constant anisotropy, different per Gaussian
+    else:               # Constant anisotropy, different per Gaussian
         beta = beta[:, None, None] if np.ptp(beta) else beta[0]
         fun = (r1/r)**(2*beta)
 
     # Tracer Gaussians
     rs = fun*(r*np.sin(th))**2
     aa = -r1**2/(2*q2_lum*s2_lum)
     bb = (1 - q2_lum)/(2*q2_lum*s2_lum)*rs
@@ -217,77 +260,136 @@
     psi = fun*ex1*ex2
 
     if component == 'sig2r':
         integ = psi
     elif component == 'sig2th':
         integ = psi*(1 - beta)
     elif component == 'sig2phi':
-        if len(gamma) == 4 != dens_lum.size:
-            # Same variable anisotropy for all Gaussians
+        if logistic:    # Variable anisotropy, same for all Gaussians
             rag, gamma0, gammainf, alpha = gamma
             gamma = gamma0 + (gammainf - gamma0)/(1 + (rag/r)**alpha)
-        else:
-            # Different but constant anisotropy per Gaussian
-            gamma = gamma[:, None, None] if np.ptp(gamma) else gamma[0]
+        else:           # Constant anisotropy, different per Gaussian
+            gamma = gamma[:, None, None] if np.ptp(gamma) else gamma[0]  # Anisotropy gamma = 1 - (sig_phi/sig_R)**2
         integ = psi*(1 - gamma)
     elif component == 'v2phi':
         integ = psi*(1 - beta)*(1 + 2*(bb + dd))
 
     return duds*drdt*integ.sum((0, 1))    # u.size == t.size
 
 ##############################################################################
+def integrand_sph_bh(t, r, th, dens_lum, sigma_lum, qintr_lum, beta, gamma, logistic, mbh, component):
+    """
+    Solution of the spherically-aligned Jeans equations for a black hole alone
+
+    """
+    # TANH Change of variables for Jeans r-integral (Sec.6.2 of Cappellari 2020)
+    # np.log([rmin, rmax]) -> [r, inf]
+    drdt = np.exp(t)
+    r1 = r + drdt[:, None]
+
+    if logistic:    # Variable anisotropy, same for all Gaussians
+        rab, beta0, betainf, alpha = beta
+        fun = (r1/r)**(2*beta0)
+        fun *= ((1 + (r1/rab)**alpha)/(1 + (r/rab)**alpha))**(2*(betainf - beta0)/alpha)
+        beta = beta0 + (betainf - beta0)/(1 + (rab/r)**alpha)
+    else:           # Constant anisotropy, different per Gaussian
+        fun = (r1/r)**(2*beta)
+
+    # Tracer Gaussians
+    s2_lum = sigma_lum**2
+    q2_lum = qintr_lum**2
+    rs = fun*(r*np.sin(th))**2
+    aa = -r1**2/(2*q2_lum*s2_lum)
+    bb = (1 - q2_lum)/(2*q2_lum*s2_lum)*rs
+    ex1 = dens_lum*np.exp(aa + bb)
+
+    G = 0.004301    # (km/s)^2 pc/Msun [6.674e-11 SI units (CODATA2018)]
+    psi = G*fun*ex1*mbh/r1**2
+
+    if component == 'sig2r':
+        integ = psi
+    elif component == 'sig2th':
+        integ = psi*(1 - beta)
+    elif component == 'sig2phi':
+        if logistic:    # Variable anisotropy, same for all Gaussians
+            rag, gamma0, gammainf, alpha = gamma
+            gamma = gamma0 + (gammainf - gamma0)/(1 + (rag/r)**alpha)
+        integ = psi*(1 - gamma)
+    elif component == 'v2phi':
+        integ = psi*(1 - beta)*(1 + 2*bb)
 
+    return drdt*integ.sum(1)
+
+##############################################################################
 def intrinsic_moments_sph(R, z,
                           dens_lum, sigma_lum, qintr_lum,
                           dens_pot, sigma_pot, qintr_pot,
-                          beta, gamma, epsrel):
+                          mbh, beta, gamma, logistic, epsrel):
     """ Numerical quadratures of the Jeans solution """
 
     r = np.sqrt(R**2 + z**2)
     th = np.arctan2(R, z)  # Angle from symmetry axis z
 
     mds, mxs = np.median(sigma_lum), np.max(sigma_lum)
     xlim = np.arcsinh(np.log([1e-7*mds, 1e3*mxs])*2/np.pi)
     ylim = np.log([1e-6*mds, 3*mxs])
-    args = [r, th, dens_lum, sigma_lum, qintr_lum, dens_pot, sigma_pot, qintr_pot, beta, gamma]
+    args = [r, th, dens_lum, sigma_lum, qintr_lum, beta, gamma, logistic]
+    args_mge = args + [dens_pot, sigma_pot, qintr_pot]
     nu = density(R, z, dens_lum, sigma_lum, qintr_lum).sum()
-    sig2r, sig2th, sig2phi, v2phi = \
-        [quad2d(integrand_sph, xlim, ylim, epsrel=epsrel, args=args+[txt]).integ/nu
-         for txt in ['sig2r', 'sig2th', 'sig2phi', 'v2phi']]
+
+    sig2r = quad2d(integrand_sph, xlim, ylim, epsrel=epsrel, args=args_mge+['sig2r']).integ/nu
+    v2phi = quad2d(integrand_sph, xlim, ylim, epsrel=epsrel, args=args_mge+['v2phi']).integ/nu
+
+    if mbh > 0:
+        args_bh = args + [mbh]
+        sig2r += quad1d(integrand_sph_bh, ylim, epsrel=epsrel, args=args_bh+['sig2r']).integ/nu
+        v2phi += quad1d(integrand_sph_bh, ylim, epsrel=epsrel, args=args_bh+['v2phi']).integ/nu
+
+    if (not logistic) and (np.ptp(beta) or np.ptp(gamma)):
+        sig2th = quad2d(integrand_sph, xlim, ylim, epsrel=epsrel, args=args_mge+['sig2th']).integ/nu
+        sig2phi = quad2d(integrand_sph, xlim, ylim, epsrel=epsrel, args=args_mge+['sig2phi']).integ/nu
+        if mbh > 0:
+            sig2th += quad1d(integrand_sph_bh, ylim, epsrel=epsrel, args=args_bh+['sig2th']).integ/nu
+            sig2phi += quad1d(integrand_sph_bh, ylim, epsrel=epsrel, args=args_bh+['sig2phi']).integ/nu
+    else:
+        if logistic:
+            rab, beta0, betainf, alpha = beta
+            beta = beta0 + (betainf - beta0)/(1 + (rab/r)**alpha)
+            rag, gamma0, gammainf, alpha = gamma
+            gamma = gamma0 + (gammainf - gamma0)/(1 + (rag/r)**alpha)
+        else:
+            beta = beta[0]
+            gamma = gamma[0]
+        sig2th = sig2r*(1 - beta)
+        sig2phi = sig2r*(1 - gamma)
+
     v2phi += quad1d(integand_tan_dth_pot, xlim, epsrel=epsrel,
-                     args=(r, th, dens_pot, sigma_pot, qintr_pot)).integ
+                     args=(R**2, z**2, dens_pot, sigma_pot, qintr_pot)).integ
 
     return sig2r, sig2th, sig2phi, v2phi, nu
 
 ##############################################################################
-
-def intrinsic_moments(Rbin, zbin,
-                      dens_lum, sigma_lum, qintr_lum,
-                      dens_pot, sigma_pot, qintr_pot,
-                      beta, gamma, nrad, nang, epsrel, interp, proj_cyl, align):
+def intrinsic_moments(Rbin, zbin, dens_lum, sigma_lum, qintr_lum, dens_pot,
+                      sigma_pot, qintr_pot, mbh, beta, gamma, logistic, nrad,
+                      nang, epsrel, interp, proj_cyl, align):
 
     fun = intrinsic_moments_cyl if align == 'cyl' else intrinsic_moments_sph
 
     if nrad*nang > Rbin.size or (not interp):  # Just calculate values
-
         print("Just compute values")
         sig2r, sig2th, sig2phi, v2phi, nu = np.empty((5, Rbin.size))
         for j, (Rj, zj) in enumerate(zip(Rbin, zbin)):  # loop over coordinates
-            sig2r[j], sig2th[j], sig2phi[j], v2phi[j], nu[j] = \
-                fun(Rj, zj, dens_lum, sigma_lum, qintr_lum,
-                    dens_pot, sigma_pot, qintr_pot, beta, gamma, epsrel)
-
+            sig2r[j], sig2th[j], sig2phi[j], v2phi[j], nu[j] = fun(Rj, zj,
+                dens_lum, sigma_lum, qintr_lum, dens_pot, sigma_pot, qintr_pot,
+                mbh, beta, gamma, logistic, epsrel)
     else:
-
         print("Perform interpolation")
-        irp = mom_interp(Rbin, zbin,
-                         dens_lum, sigma_lum, qintr_lum,
-                         dens_pot, sigma_pot, qintr_pot,
-                         beta, gamma, nrad, nang, epsrel=epsrel, align=align)
-
+        irp = mom_interp(Rbin, zbin, dens_lum, sigma_lum, qintr_lum, dens_pot,
+                         sigma_pot, qintr_pot, mbh, beta, gamma, logistic, nrad,
+                         nang, epsrel=epsrel, align=align)
         sig2r, sig2th, sig2phi, v2phi, nu = irp.get_moments(Rbin, zbin)
 
     # Project the velocity dispersion tensor to cylindrical coordinates
     if proj_cyl and (align == 'sph'):
         th = np.arctan2(Rbin, zbin)  # Angle from symmetry axis z
         sig2R = sig2th*np.cos(th)**2 + sig2r*np.sin(th)**2
         sig2z = sig2th*np.sin(th)**2 + sig2r*np.cos(th)**2
@@ -298,15 +400,15 @@
 ##############################################################################
 
 class mom_interp:
 
     def __init__(self, xbin, ybin,
                  dens_lum, sigma_lum, qintr_lum,
                  dens_pot, sigma_pot, qintr_pot,
-                 beta, gamma, nrad, nang, epsrel=1e-2,
+                 mbh, beta, gamma, logistic, nrad, nang, epsrel=1e-2,
                  rmin=None, rmax=None, align='cyl'):
         """
         Initializes model values on a grid for subsequent interpolation
 
         """
         fun = intrinsic_moments_cyl if align == 'cyl' else intrinsic_moments_sph
 
@@ -326,17 +428,17 @@
         self.ang = np.linspace(0, np.pi/2, nang)
         rellGrid, eccGrid = map(np.ravel, np.meshgrid(rad, self.ang))
         R = rellGrid*np.cos(eccGrid)
         z = rellGrid*np.sin(eccGrid)*self.qmed  # ecc=0 on equatorial plane
 
         sig2r, sig2th, sig2phi, v2phi, nu = np.empty((5, R.size))
         for j, (Rj, zj) in enumerate(zip(R, z)):
-            sig2r[j], sig2th[j], sig2phi[j], v2phi[j], nu[j] = \
-                fun(Rj, zj, dens_lum, sigma_lum, qintr_lum,
-                    dens_pot, sigma_pot, qintr_pot, beta, gamma, epsrel)
+            sig2r[j], sig2th[j], sig2phi[j], v2phi[j], nu[j] = fun(Rj, zj,
+                dens_lum, sigma_lum, qintr_lum, dens_pot, sigma_pot, qintr_pot,
+                mbh, beta, gamma, logistic, epsrel)
 
         self.sig2r = sig2r.reshape(nang, nrad)
         self.sig2th = sig2th.reshape(nang, nrad)
         self.sig2phi = sig2phi.reshape(nang, nrad)
         self.v2phi = v2phi.reshape(nang, nrad)
         self.dens_lum = dens_lum
         self.sigma_lum = sigma_lum
@@ -389,20 +491,22 @@
       `Cappellari (2020) <https://ui.adsabs.harvard.edu/abs/2020MNRAS.494.4819C>`_
 
     Calling Sequence
     ----------------
 
     .. code-block:: python
 
+        from jampy.jam_axi_intr import jam_axi_intr
+
         jam = jam_axi_intr(
                  dens_lum, sigma_lum, qintr_lum, dens_pot, sigma_pot, qintr_pot,
-                 mbh, Rbin, zbin, align='cyl', beta=None, data=None,
-                 epsrel=1e-2, errors=None, gamma=None, goodbins=None,
-                 interp=True, ml=None, nang=10, nodots=False, nrad=20,
-                 plot=True, proj_cyl=False, quiet=False, rbh=1)
+                 mbh, Rbin, zbin, align='cyl', beta=None, data=None, epsrel=1e-2,
+                 errors=None, gamma=None, goodbins=None, interp=True,
+                 logistic=False, ml=None, nang=10, nodots=False, nrad=20,
+                 plot=True, proj_cyl=False, quiet=False)
 
         # The meaning of the output is different depending on `align`
         sig2R, sig2z, sig2phi, v2phi = jam.model  # with align='cyl'
         sig2r, sig2th, sig2phi, v2phi = jam.model  # with align='sph'
 
         jam.plot()   # Generate data/model comparison
 
@@ -458,15 +562,15 @@
     beta: array_like with shape (n,) or (4,)
         Vector with the axial anisotropy of the individual kinematic-tracer
         MGE Gaussians (Default: ``beta=np.zeros(n)``)::
 
             beta = 1 - (sigma_th/sigma_r)^2  # with align='sph'
             beta = 1 - (sigma_z/sigma_R)^2   # with align='cyl'
 
-        When ``len(beta) == 4`` the procedure assumes::
+        When ``logistic=True`` the procedure assumes::
 
             beta = [r_a, beta_0, beta_inf, alpha]
 
         and the anisotropy of the whole JAM model varies as a logistic
         function of the logarithmic spherical radius (with ``align='sph'``) or
         of the logarithmic distance from the equatorial plane (with ``align='cyl'``)::
 
@@ -475,14 +579,16 @@
 
         Here ``beta_0`` represents the anisotropy at ``r = 0``, ``beta_inf``
         is the anisotropy at ``r = inf`` and ``r_a`` is the anisotropy
         transition radius, with ``alpha`` controlling the sharpness of the
         transition. In the special case ``beta_0 = 0, beta_inf = 1, alpha = 2``
         the anisotropy variation reduces to the form by Osipkov & Merritt, but
         the extra parameters allow for much more realistic anisotropy profiles.
+        See an application in `Simon, Cappellari & Hartke (2023)
+        <https://ui.adsabs.harvard.edu/abs/2023arXiv230318229S>`_.
     data: array_like of shape (4, p), optional
         Four input vectors with the observed values of:
 
         - ``[sigR, sigz, sigphi, vrms_phi]`` in ``km/s``, when ``align='cyl'``
           (or ``align='sph'`` and ``proj_cyl=True``).
 
           ``vrms_phi`` is the square root of the velocity second moment in the
@@ -502,15 +608,15 @@
     gamma: array_like with shape (n,)
         Vector with the tangential anisotropy of the individual kinematic-tracer
         MGE Gaussians (Default: ``gamma=np.zeros(n)``)::
 
             gamma = 1 - (sigma_phi/sigma_r)^2  # with align='sph'
             gamma = 1 - (sigma_phi/sigma_R)^2  # with align='cyl'
 
-        When ``len(gamma) == 4`` the procedure assumes::
+        When ``logistic=True`` the procedure assumes::
 
             gamma = [r_a, gamma_0, gamma_inf, alpha]
 
         and the anisotropy of the whole JAM model varies as a logistic
         function of the logarithmic spherical radius (with ``align='sph'``) or
         of the logarithmic distance from the equatorial plane (with ``align='cyl'``)::
 
@@ -528,14 +634,19 @@
         for the bins which have to be included in the fit (if requested) and
         ``chi^2`` calculation (Default: fit all bins).
     interp: bool, optional
         If ``interp=False`` no interpolation is performed and the model is
         computed at every set of input (R, z) coordinates.
         If ``interp=True`` (default), the model is interpolated if the number
         of requested input (R, z) coordinates is larger than ``nang*nrad``.
+    logistic: bool, optional
+        When ``logistic=True``, JAM interprets the anisotropy parameters
+        ``beta`` and ``gamma`` as defining a 4-parameters logistic function.
+        See the documentation of the anisotropy keywords for details.
+        (Default ``logistic=False``)
     ml: float, optional
         Mass-to-light ratio M/L. If ``ml=None`` (default) the M/L is fitted to
         the data and the best-fitting value is returned in output.
         The ``mbh`` is also scaled and becomes ``mbh*ml``.
         If ``ml=1`` no scaling is applied to the model.
     nang: int, optional
         The number of linearly-spaced intervals in the eccentric anomaly at
@@ -557,20 +668,14 @@
         ``[sig2R, sig2z, sig2phi, v2phi]`` components as in the case
         ``align='cyl'``. This is useful for a direct comparison of results with
         either the spherical or cylindrical alignment, as it allows one to fit
         the same data with both modelling assumptions.
     quiet: bool, optional
         If ``quiet=False`` (default), print the best-fitting M/L and chi2 at
         the end for the calculation.
-    rbh: float, optional
-        This scalar gives the sigma in pc of the Gaussian representing the
-        central black hole of mass ``mbh`` [See Section 3.1.2 of
-        `Cappellari (2008)`_]. The gravitational potential is indistinguishable
-        from a point source for ``radii > 2*rbh``, so the default ``rbh=1`` pc
-        is appropriate for observations taken with current telescopes.
 
     Output Parameters
     -----------------
 
     Returned as attributes of the ``jam_axi_intr`` class.
 
     .chi2: float
@@ -613,30 +718,33 @@
         ``vphi = np.sqrt(v2phi - sig2phi)``
 
         NOTE: I return squared velocities instead of taking the square root,
         to allow for negative values (unphysical solutions).
 
     ###########################################################################
     """
-    def __init__(self, dens_lum, sigma_lum, qintr_lum, dens_pot, sigma_pot, qintr_pot,
-                 mbh, Rbin, zbin, align='cyl', beta=None, data=None,
+
+    def __init__(self, dens_lum, sigma_lum, qintr_lum, dens_pot, sigma_pot,
+                 qintr_pot, mbh, Rbin, zbin, align='cyl', beta=None, data=None,
                  epsrel=1e-2, errors=None, gamma=None, goodbins=None,
-                 interp=True, ml=None, nang=10, nodots=False, nrad=20,
-                 plot=True, proj_cyl=False, quiet=False, rbh=1):
+                 interp=True, logistic=False, ml=None, nang=10, nodots=False,
+                 nrad=20, plot=True, proj_cyl=False, quiet=False):
 
         assert align in ['sph', 'cyl'], "`align` must be 'sph' or 'cyl'"
         assert (ml is None) or (ml > 0), "The input `ml` must be positive"
         if beta is None:
             beta = np.zeros_like(dens_lum)  # Anisotropy parameter beta = 1 - (sig_th/sig_r)**2  (beta=0-->circle)
-        if gamma is None:
-            gamma = np.zeros_like(dens_lum)  # Anisotropy parameter gamma = 1 - (sig_phi/sig_r)^2 (gamma=0-->circle)
+        if gamma is None:  # Anisotropy parameter beta = 1 - (sig_th/sig_r)**2
+            if logistic:
+                gamma = [1, 0, 0, 1]    # [r_a, gamma_0, gamma_inf, alpha]
+            else:
+                gamma = np.zeros_like(beta)
         assert (dens_lum.size == sigma_lum.size == qintr_lum.size) \
-               and ((len(beta) == 4)^(len(beta) == dens_lum.size)) \
-               and ((len(gamma) == 4)^(len(gamma) == dens_lum.size)), \
-            "The luminous MGE components and anisotropies do not match"
+               and ((len(beta) == 4 and logistic) or (len(beta) == dens_lum.size)) \
+               and (len(beta) == len(gamma)), "The luminous MGE components and anisotropies do not match"
         assert dens_pot.size == sigma_pot.size == qintr_pot.size, "The total mass MGE components do not match"
         assert Rbin.size == zbin.size, "Rbin and zbin do not match"
 
         if data is not None:
             assert len(data) == 4, "`data` must contain four vectors"
             if errors is None:
                 errors = np.full_like(data, 5)  # Constant 5 km/s errors
@@ -649,45 +757,29 @@
                 "(data, errors, goodbins) and (Rbin, zbin) do not match"
         if goodbins is None:
             goodbins = np.ones_like(data, dtype=bool)
         else:
             assert goodbins.dtype == bool, "goodbins must be a boolean vector"
             assert np.any(goodbins), "goodbins must contain some True values"
 
-        # Add a Gaussian with small sigma and the same total mass as the BH.
-        # The Gaussian provides an excellent representation of the second moments
-        # of a point-like mass, to 1% accuracy out to a radius 2*sigmaBH.
-        # The error increases to 14% at 1*sigmaBH, independently of the BH mass.
-        #
-        if mbh > 0:
-            sigmaBH = rbh # Adopt for the BH just a very small size (default 1pc)
-            dens_bh = mbh/(np.sqrt(2*np.pi)*sigmaBH)**3
-            dens_pot = np.append(dens_bh, dens_pot) # Add Gaussian to potential only!
-            sigma_pot = np.append(sigmaBH, sigma_pot)
-            qintr_pot = np.append(1., qintr_pot)  # Make sure vectors do not have extra dimensions
-
         t = clock()
 
         # model contains [sig2r, sig2th, sig2phi, v2phi]
-        *model, nu = intrinsic_moments(
-            Rbin, zbin, dens_lum, sigma_lum, qintr_lum,
-            dens_pot, sigma_pot, qintr_pot, beta, gamma, nrad, nang, epsrel,
-            interp, proj_cyl, align)
+        *model, nu = intrinsic_moments(Rbin, zbin, dens_lum, sigma_lum,
+            qintr_lum, dens_pot, sigma_pot, qintr_pot, mbh, beta, gamma,
+            logistic, nrad, nang, epsrel, interp, proj_cyl, align)
 
         if not quiet:
             print(f'jam_axi_intr_{align} elapsed time (sec): {clock() - t:.2f}')
 
         if data is None:
-
             chi2 = None
             if ml is None:
                 ml = 1.
-
         else:
-
             model0 = np.sqrt(np.clip(model, 0, None))   # sqrt([sig2r, sig2th, sig2phi, v2phi])
 
             # Exclude sig2phi from M/L calculation
             if (ml is None) or (ml <= 0):
                 m = np.delete(model0, 2, 0).ravel()     # sqrt([sig2r, sig2th, v2phi])
                 d = np.delete(data, 2, 0).ravel()
                 e = np.delete(errors, 2, 0).ravel()
```

### Comparing `jampy-7.0.10/jampy/jam_axi_proj.py` & `jampy-7.1.0/jampy/jam_axi_proj.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,22 +27,114 @@
 from scipy import special, signal, ndimage
 from time import perf_counter as clock
 
 from plotbin.plot_velfield import plot_velfield
 from plotbin.symmetrize_velfield import symmetrize_velfield
 
 from jampy.jam_axi_intr import mom_interp
-from jampy.legacy.jam_axi_rms import surf_v2los
+from jampy.quad1d import quad1d
 
 ##############################################################################
+def integrand_cyl_los(u1,
+                      dens_lum, sigma_lum, q_lum,
+                      dens_pot, sigma_pot, q_pot,
+                      x1, y1, inc, beta, tensor):
+    """
+    This routine computes the integrand of Eq.(28) of Cappellari (2008; C08) for
+    a model with constant anisotropy sigma_R**2 = b*sigma_z**2 and <V_R*V_z> = 0.
+    The components of the proper motion dispersions tensor are calculated as
+    described in note 5 of C08.
+    See Cappellari (2012; C12 http://arxiv.org/abs/1211.7009)
+    for explicit formulas for the proper motion tensor.
+    The formulas are also given in Appendix A3 of Cappellari (2020, C20)
+    https://ui.adsabs.harvard.edu/abs/2020MNRAS.494.4819C
+
+
+    """
+    dens_lum = dens_lum[:, None, None]
+    sigma_lum = sigma_lum[:, None, None]
+    q_lum = q_lum[:, None, None]
+    beta = beta[:, None, None]
+
+    dens_pot = dens_pot[None, :, None]
+    sigma_pot = sigma_pot[None, :, None]
+    q_pot = q_pot[None, :, None]
+
+    u = u1[None, None, :]
+
+    kani = 1./(1 - beta)  # Anisotropy ratio b = (sig_R/sig_z)**2
+    ci = np.cos(inc)
+    si = np.sin(inc)
+    si2 = si**2
+    ci2 = ci**2
+    x2 = x1**2
+    y2 = y1**2
+    u2 = u**2
+
+    s2_lum = sigma_lum**2
+    q2_lum = q_lum**2
+    e2_lum = 1 - q2_lum
+    s2q2_lum = s2_lum*q2_lum
+
+    s2_pot = sigma_pot**2
+    e2_pot = 1 - q_pot**2
+
+    # Double summation over (j, k) of eq.(28) for all values of integration variable u.
+    # The triple loop in (j, k, u) is replaced by broadcast Numpy array operations.
+    e2u2_pot = e2_pot*u2
+    a = 0.5*(u2/s2_pot + 1/s2_lum)               # equation (29) in C08
+    b = 0.5*(e2u2_pot*u2/(s2_pot*(1 - e2u2_pot)) + e2_lum/s2q2_lum) # equation (30) in C08
+    c = e2_pot - s2q2_lum/s2_pot                  # equation (22) in C08
+    d = 1 - kani*q2_lum - ((1 - kani)*c + e2_pot*kani)*u2  # equation (23) in C08
+    e = a + b*ci2
+    if tensor == 'xx':
+        f = kani*s2q2_lum + d*((y1*ci*(a+b)/e)**2 + si2/(2*e)) # equation (4) in C12
+    elif tensor == 'yy':
+        f = s2q2_lum*(si2 + kani*ci2) + d*x2*ci2  # equation (5) in C12
+    elif tensor == 'zz':
+        f = s2q2_lum*(ci2 + kani*si2) + d*x2*si2  # z' LOS equation (28) in C08
+    elif tensor == 'xy':
+        f = -d*np.abs(x1*y1)*ci2*(a+b)/e          # equation (6) in C12
+    elif tensor == 'xz':
+        f = -d*np.abs(x1*y1)*si*ci*(a+b)/e         # -equation (7) in C12
+    elif tensor == 'yz':
+        f = -si*ci*(s2q2_lum*(1 - kani) - d*x2)   # -equation (8) in C12
+
+    # arr has the dimensions (q_lum.size, q_pot.size, u.size)
+
+    arr = q_pot*dens_pot*dens_lum*u2*f*np.exp(-a*(x2 + y2*(a + b)/e))/(
+            (1 - c*u2)*np.sqrt((1 - e2u2_pot)*e))
+
+    G = 0.004301  # (km/s)^2 pc/Msun [6.674e-11 SI units (CODATA2018)]
+
+    return 4*np.pi**1.5*G*arr.sum((0, 1))
+
+##############################################################################
+def surf_v2los_cyl(x1, y1, inc,
+                   dens_lum, sigma_lum, qintr_lum,
+                   dens_pot, sigma_pot, qintr_pot,
+                   beta, tensor):
+    """
+    This routine gives the projected weighted second moment Sigma*<V^2_los>
+
+    """
+    sb_mu2 = np.empty_like(x1)
+    for j, (xj, yj) in enumerate(zip(x1, y1)):
+        sb_mu2[j] = quad1d(integrand_cyl_los, [0., 1.], singular=1,
+                           args=(dens_lum, sigma_lum, qintr_lum,
+                                  dens_pot, sigma_pot, qintr_pot,
+                                  xj, yj, inc, beta, tensor)).integ
 
-def vmom_proj(x1, y1, inc,
+    return sb_mu2
+
+##############################################################################
+def vmom_proj(x1, y1, inc, mbh, beta, gamma, logistic,
               dens_lum, sigma_lum, qintr_lum,
               dens_pot, sigma_pot, qintr_pot,
-              beta, gamma, nrad, nang, nlos, epsrel, align):
+              nrad, nang, nlos, epsrel, align, step):
     """
     This routine gives the projected first velocity moments
     and the second velocity moments tensor for a JAM model with
     either cylindrically or spherically-aligned velocity ellipsoid.
     The projection formulas given below are described in
     Sec.3 and the numerical quadrature in Sec.6.2 of
     Cappellari (2020, MNRAS, 494, 4819; hereafter C20)
@@ -57,16 +149,16 @@
     z1 = scale*np.sinh(t)
     dxdt = dt*scale*np.cosh(t)
 
     # Initialize moment values for interpolation
     irp = mom_interp(x1, y1,
                      dens_lum, sigma_lum, qintr_lum,
                      dens_pot, sigma_pot, qintr_pot,
-                     beta, gamma, nrad, nang, epsrel,
-                     rmin=np.min(sigma_lum)/3, rmax=rmax, align=align)
+                     mbh, beta, gamma, logistic, nrad, nang, epsrel,
+                     rmin=step/np.sqrt(2), rmax=rmax, align=align)
 
     x = x1[:, None]
     y = z1*np.sin(inc) + y1[:, None]*np.cos(inc)                    # C20 eq.(29)
     z = z1*np.cos(inc) - y1[:, None]*np.sin(inc)
     R = np.sqrt(x**2 + y**2)
     r = np.sqrt(R**2 + z**2)
     cos_phi, sin_phi, sin_th, cos_th = x/R, y/R, R/r, z/r           # C20 eq.(30)
@@ -100,15 +192,14 @@
     nu_v2los = nu*integ2 @ dxdt     # DE quadrature
     vel = nu_vlos/surf
     vel2 = nu_v2los/surf
 
     return vel, vel2
 
 ##############################################################################
-
 def mge_surf(x, y, surf, sigma, qobs):
     """ MGE surface brightness for a set of coordinates (x, y) """
 
     mge = surf*np.exp(-0.5/sigma**2*(x[..., None]**2 + (y[..., None]/qobs)**2))
 
     return mge.sum(-1)
 
@@ -127,84 +218,76 @@
 
     xi = (nx - 1.)/(xv[-1] - xv[0])*(xout - xv[0])
     yi = (ny - 1.)/(yv[-1] - yv[0])*(yout - yv[0])
 
     return ndimage.map_coordinates(im.T, [xi, yi], order=1, mode='nearest')
 
 ##############################################################################
-
 def rotate_points(x, y, ang):
     """
     Rotates points counter-clockwise by an angle ANG in degrees.
     Michele cappellari, Paranal, 10 November 2013
 
     """
     theta = np.radians(ang)
     xNew = x*np.cos(theta) - y*np.sin(theta)
     yNew = x*np.sin(theta) + y*np.cos(theta)
 
     return xNew, yNew
 
 ##############################################################################
-
 def psf_conv(x, y, inc_deg,
              surf_lum, sigma_lum, qobs_lum,
              surf_pot, sigma_pot, qobs_pot,
-             beta, gamma, moment, align, sigmaPsf, normPsf, pixSize, pixAng,
-             step, nrad, nang, nlos, epsrel, interp, analytic_los):
+             mbh, beta, gamma, logistic, moment, align, sigmaPsf, normPsf,
+             pixSize, pixAng, step, nrad, nang, nlos, epsrel, interp, analytic_los):
     """
     This routine gives the velocity moment after convolution with a PSF.
     The convolution is done using interpolation of the model on a
     polar grid, as described in Appendix A of Cappellari (2008, MNRAS, 390, 71)
     https://ui.adsabs.harvard.edu/abs/2008MNRAS.390...71C
 
     """
     # Axisymmetric deprojection of both luminous and total mass.
     # See equation (12)-(14) of Cappellari (2008)
-    #
     inc = np.radians(inc_deg)
+    qmin = 0.05   # Minimum desired intrinsic axial ratio
+    qobsmin = np.sqrt(np.cos(inc)**2 + (qmin*np.sin(inc))**2)
 
-    qintr_lum = qobs_lum**2 - np.cos(inc)**2
-    if np.any(qintr_lum <= 0):
-        raise RuntimeError('Inclination too low q_lum <= 0')
-    qintr_lum = np.sqrt(qintr_lum)/np.sin(inc)
-    if np.any(qintr_lum < 0.05):
-        raise RuntimeError('Inclination too low q_lum < 0.05')
-    dens_lum = surf_lum*qobs_lum / (sigma_lum*qintr_lum*np.sqrt(2*np.pi))
-
-    qintr_pot = qobs_pot**2 - np.cos(inc)**2
-    if np.any(qintr_pot <= 0):
-        raise RuntimeError('Inclination too low q_pot <= 0')
-    qintr_pot = np.sqrt(qintr_pot)/np.sin(inc)
-    if np.any(qintr_pot < 0.05):
-        raise RuntimeError('Inclination too low q_pot < 0.05')
-    dens_pot = surf_pot*qobs_pot / (sigma_pot*qintr_pot*np.sqrt(2*np.pi))
+    assert np.all(qobs_lum >= qobsmin), f'Inclination too low q_lum < {qmin}'
+    qintr_lum = np.sqrt(qobs_lum**2 - np.cos(inc)**2)/np.sin(inc)
+    dens_lum = surf_lum*qobs_lum/(sigma_lum*qintr_lum*np.sqrt(2*np.pi))
+
+    assert np.all(qobs_pot >= qobsmin), f'Inclination too low q_pot < {qmin}'
+    qintr_pot = np.sqrt(qobs_pot**2 - np.cos(inc)**2)/np.sin(inc)
+    dens_pot = surf_pot*qobs_pot/(sigma_pot*qintr_pot*np.sqrt(2*np.pi))
 
     # Define parameters of polar grid for interpolation
     w = sigma_lum < np.max(np.abs(x))  # Characteristic MGE axial ratio in observed range
     qmed = np.median(qobs_lum) if w.sum() < 3 else np.median(qobs_lum[w])
     rell = np.sqrt(x**2 + (y/qmed)**2)  # Elliptical radius of input (x, y)
 
     psf_convolution = (np.max(sigmaPsf) > 0) and (pixSize > 0)
 
     if not interp or ((nrad*nang > x.size) and (not psf_convolution)):  # Just calculate values
 
         assert np.all((x != 0) | (y != 0)), "One must avoid the singularity at `(xbin, ybin) = (0, 0)`"
 
         x_pol = x
         y_pol = y
+        step = np.min(rell)  # Minimum radius
 
     else:  # Interpolate values on polar grid
 
         # Kernel step is 1/4 of largest between sigma(min) and 1/2 pixel side.
         # Kernel half size is the sum of 3*sigma(max) and 1/2 pixel diagonal.
 
         if psf_convolution:         # PSF convolution
             if step == 0:
-                step = np.min(sigmaPsf)/4.
+                step = np.min(sigmaPsf)/4
             mx = 3*np.max(sigmaPsf) + pixSize/np.sqrt(2)
         else:                       # No convolution
             step = np.min(rell)     # Minimum radius
             mx = 0
 
         # Make linear grid in log of elliptical radius RAD and eccentric anomaly ANG
         # See Appendix A of Cappellari (2008)
@@ -215,25 +298,25 @@
         x_pol = radGrid*np.cos(angGrid)
         y_pol = radGrid*np.sin(angGrid)*qmed
 
     # The model computation is only performed on the polar grid
     # which is then used to interpolate the values at any other location
     if analytic_los:
         # Analytic line-of-sight integral
-        sb_mu2 = surf_v2los(x_pol, y_pol, inc,
-                            dens_lum, sigma_lum, qintr_lum,
-                            dens_pot, sigma_pot, qintr_pot, beta, moment)
+        sb_mu2 = surf_v2los_cyl(x_pol, y_pol, inc,
+                                dens_lum, sigma_lum, qintr_lum,
+                                dens_pot, sigma_pot, qintr_pot, beta, moment)
         model = sb_mu2/mge_surf(x_pol, y_pol, surf_lum, sigma_lum, qobs_lum)
         vel = vel2 = None
     else:
         # Numeric line-of-sight integral
-        vel, vel2 = vmom_proj(x_pol, y_pol, inc,
+        vel, vel2 = vmom_proj(x_pol, y_pol, inc, mbh, beta, gamma, logistic,
                               dens_lum, sigma_lum, qintr_lum,
                               dens_pot, sigma_pot, qintr_pot,
-                              beta, gamma, nrad, nang, nlos, epsrel, align)
+                              nrad, nang, nlos, epsrel, align, step)
         model = {'xx': vel2[0, 0],
                  'yy': vel2[1, 1],
                  'zz': vel2[2, 2],
                  'xy': vel2[0, 1],
                  'xz': vel2[0, 2],
                  'yz': vel2[1, 2],
                  'x': vel[0],
@@ -275,16 +358,15 @@
         sp = np.sqrt(2)*sigmaPsf
         xg, yg = xgrid[..., None], ygrid[..., None]
         kernel = normPsf*(special.erf((dx - xg)/sp) + special.erf((dx + xg)/sp)) \
                         *(special.erf((dx - yg)/sp) + special.erf((dx + yg)/sp))
         kernel = kernel.sum(-1)   # Sum over PSF components
 
         # Seeing and aperture convolution with equation (A3) of Cappellari (2008)
-        m1 = signal.fftconvolve(model_car, kernel, mode='same')
-        m2 = signal.fftconvolve(mge_car, kernel, mode='same')
+        m1, m2 = signal.fftconvolve([model_car, mge_car], kernel[None, ...], mode='same')
         w = m2 > 0   # Allow for rounding errors
         muCar = np.zeros_like(m1)
         muCar[w] = m1[w]/m2[w]
 
         # Interpolate convolved image at observed apertures.
         # Aperture integration was already included in the kernel.
         mu = bilinear_interpolate(x1, y1, muCar, x, y)
@@ -334,22 +416,25 @@
       `Cappellari (2020) <https://ui.adsabs.harvard.edu/abs/2020MNRAS.494.4819C>`_
 
     Calling Sequence
     ----------------
 
     .. code-block:: python
 
+        from jampy.jam_axi_proj import jam_axi_proj
+
         jam = jam_axi_proj(
                  surf_lum, sigma_lum, qobs_lum, surf_pot, sigma_pot, qobs_pot,
                  inc, mbh, distance, xbin, ybin, align='cyl', analytic_los=True,
                  beta=None, data=None, epsrel=1e-2, errors=None, flux_obs=None,
-                 gamma=None, goodbins=None, interp=True, kappa=None, ml=None,
-                 moment='zz', nang=10, nlos=1500, nodots=False, normpsf=1.,
-                 nrad=20, pixang=0., pixsize=0., plot=True, quiet=False,
-                 rbh=0.01, sigmapsf=0., step=0., vmax=None, vmin=None)
+                 gamma=None, goodbins=None, interp=True, kappa=None,
+                 logistic=False, ml=None, moment='zz', nang=10, nlos=1500,
+                 nodots=False, normpsf=1., nrad=20, pixang=0., pixsize=0.,
+                 plot=True, quiet=False, rbh=0.01, sigmapsf=0., step=0.,
+                 vmax=None, vmin=None)
 
         vrms = jam.model  # with moment='zz' the output is the LOS Vrms
 
         jam.plot()   # Generate data/model comparison when data is given
 
     See more examples in the ``jampy/examples`` folder inside
     `site-packages <https://stackoverflow.com/a/46071447>`_.
@@ -452,15 +537,15 @@
     beta: array_like with shape (n,) or (4,)
         Radial anisotropy of the individual kinematic-tracer MGE Gaussians
         (Default: ``beta=np.zeros(n)``)::
 
             beta = 1 - (sigma_th/sigma_r)^2  # with align='sph'
             beta = 1 - (sigma_z/sigma_R)^2   # with align='cyl'
 
-        When ``len(beta) == 4`` the procedure assumes::
+        When ``logistic=True`` the procedure assumes::
 
             beta = [r_a, beta_0, beta_inf, alpha]
 
         and the anisotropy of the whole JAM model varies as a logistic
         function of the logarithmic spherical radius (with ``align='sph'``) or
         of the logarithmic distance from the equatorial plane (with ``align='cyl'``)::
 
@@ -469,14 +554,16 @@
 
         Here ``beta_0`` represents the anisotropy at ``r = 0``, ``beta_inf``
         is the anisotropy at ``r = inf`` and ``r_a`` is the anisotropy
         transition radius, with ``alpha`` controlling the sharpness of the
         transition. In the special case ``beta_0 = 0, beta_inf = 1, alpha = 2``
         the anisotropy variation reduces to the form by Osipkov & Merritt, but
         the extra parameters allow for much more realistic anisotropy profiles.
+        See an application in `Simon, Cappellari & Hartke (2023)
+        <https://ui.adsabs.harvard.edu/abs/2023arXiv230318229S>`_.
     data: array_like with shape (p,), optional
         observed first or second velocity moment used to fit the model.
 
         EXAMPLE: In the common case where one has only line-of-sight velocities
         the second moment is given by::
 
             Vrms = np.sqrt(velBin**2 + sigBin**2)
@@ -505,15 +592,15 @@
     gamma: array_like with shape (n,)
         tangential anisotropy of the individual kinematic-tracer MGE Gaussians
         (Default: ``gamma=np.zeros(n)``)::
 
             gamma = 1 - (sigma_phi/sigma_r)^2  # with align='sph'
             gamma = 1 - (sigma_phi/sigma_R)^2  # with align='cyl'
 
-        When ``len(gamma) == 4`` the procedure assumes::
+        When ``logistic=True`` the procedure assumes::
 
             gamma = [r_a, gamma_0, gamma_inf, alpha]
 
         and the anisotropy of the whole JAM model varies as a logistic
         function of the logarithmic spherical radius (with ``align='sph'``) or
         of the logarithmic distance from the equatorial plane (with ``align='cyl'``)::
 
@@ -547,14 +634,19 @@
         to compute all moments, including proper motions,  simultaneously.
     kappa: float, optional
         When ``kappa=None`` (default) the first velocity moments are scaled in
         such a way that the projected angular momentum of the data and model is
         the same [equation 52 of `Cappellari (2008)`_].
         When ``kappa=1`` the model first velocity moments are output without
         any scaling.
+    logistic: bool, optional
+        When ``logistic=True``, JAM interprets the anisotropy parameters
+        ``beta`` and ``gamma`` as defining a 4-parameters logistic function.
+        See the documentation of the anisotropy keywords for details.
+        (Default ``logistic=False``)
     ml: float, optional
         Mass-to-light ratio (M/L) to multiply the values given by ``surf_pot``.
         Setting this keyword is completely equivalent to multiplying the
         output ``model`` by ``np.sqrt(M/L)`` after the fit. This implies that
         the BH mass is also scaled and becomes ``mbh*ml``.
 
         If ``ml=None`` (default) the M/L is fitted from the data and the
@@ -628,15 +720,17 @@
         PSF convolution is not performed.
     plot: bool
         When ``data is not None`` setting this keyword produces a plot with the
         data/model comparison at the end of the calculation.
     quiet: bool
         Set this keyword to avoid printing values on the console.
     rbh: float, optional
-        This scalar gives the sigma in arcsec of the Gaussian representing the
+        This keyword is ignored unless ``align='cyl'`` and `analytic_los=True`.
+        In all other cases JAM assume a point-like central black hole.
+        This scalar gives the sigma in arcsec of the Gaussian approximating the
         central black hole of mass MBH [See Section 3.1.2 of `Cappellari (2008)`_]
         The gravitational potential is indistinguishable from a point source
         for ``radii > 2*rbh``, so the default ``rbh=0.01`` arcsec is appropriate
         in most current situations.
 
         When using different units as input, e.g. pc instead of arcsec, one
         should check that ``rbh`` is not too many order of magnitude smaller
@@ -716,38 +810,42 @@
         However, for advanced use only, when setting ``interp=False`` and
         ``analytic_los=False``, this attribute contains the full 3x3 second
         velocity moment tensor, *not* PSF convolved, at the sky coordinates
         ``(xbin, ybin)``.
 
     ###########################################################################
     """
-    def __init__(self, surf_lum, sigma_lum, qobs_lum, surf_pot, sigma_pot, qobs_pot,
-                 inc, mbh, distance, xbin, ybin, align='cyl', analytic_los=True,
-                 beta=None, data=None, epsrel=1e-2, errors=None, flux_obs=None,
-                 gamma=None, goodbins=None, interp=True, kappa=None, ml=None,
-                 moment='zz', nang=10, nlos=1500, nodots=False, normpsf=1.,
-                 nrad=20, pixang=0., pixsize=0., plot=True, quiet=False,
-                 rbh=0.01, sigmapsf=0., step=0.):
+
+    def __init__(self, surf_lum, sigma_lum, qobs_lum, surf_pot, sigma_pot,
+                 qobs_pot, inc, mbh, distance, xbin, ybin, align='cyl',
+                 analytic_los=True, beta=None, data=None, epsrel=1e-2,
+                 errors=None, flux_obs=None, gamma=None, goodbins=None,
+                 interp=True, kappa=None, logistic=False, ml=None, moment='zz',
+                 nang=10, nlos=1500, nodots=False, normpsf=1., nrad=20,
+                 pixang=0., pixsize=0., plot=True, quiet=False, rbh=0.01,
+                 sigmapsf=0., step=0.):
 
         str1 = ['x', 'y', 'z']
         str2 =  ['xx', 'yy', 'zz', 'xy', 'xz', 'yz']
         assert moment in str1 + str2, f"`moment` must be one of {str1 + str2}"
         assert align in ['sph', 'cyl'], "`align` must be 'sph' or 'cyl'"
         assert (ml is None) or (ml > 0), "The input `ml` must be positive"
         if beta is None:
             beta = np.zeros_like(surf_lum)  # Anisotropy parameter beta = 1 - (sig_th/sig_r)**2
-        if gamma is None:
-            gamma = np.zeros_like(surf_lum)  # Anisotropy parameter beta = 1 - (sig_th/sig_r)**2
+        if gamma is None:  # Anisotropy parameter beta = 1 - (sig_th/sig_r)**2
+            if logistic:
+                gamma = [1, 0, 0, 1]
+            else:
+                gamma = np.zeros_like(beta)
         assert (surf_lum.size == sigma_lum.size == qobs_lum.size) \
-               and ((len(beta) == 4)^(len(beta) == surf_lum.size)) \
-               and ((len(gamma) == 4)^(len(gamma) == surf_lum.size)),  \
-            "The luminous MGE components and anisotropies do not match"
-        assert surf_pot.size == sigma_pot.size == qobs_pot.size, "The total mass MGE components do not match"
+               and ((len(beta) == 4 and logistic) or (len(beta) == surf_lum.size)) \
+               and (len(beta) == len(gamma)), "The luminous MGE components and anisotropies do not match"
+        assert surf_pot.size == sigma_pot.size == qobs_pot.size, "The total-mass MGE components do not match"
         assert xbin.size == ybin.size, "`xbin` and `ybin` do not match"
-        if (not interp) or (moment in str1) or (align == 'sph') or (len(beta) == 4 != surf_lum.size):
+        if (not interp) or (moment in str1) or (align == 'sph') or logistic:
             analytic_los = False
         if data is not None:
             if errors is None:
                 if moment in str2:
                     errors = np.full_like(data, np.median(data)*0.05)  # Constant ~5% errors
                 else:
                     errors = np.full_like(data, 5.)  # Constant 5 km/s errors
@@ -772,27 +870,27 @@
         sigma_pot_pc = sigma_pot*pc
         xbin_pc = xbin*pc
         ybin_pc = ybin*pc
         pixSize_pc = pixsize*pc
         sigmaPsf_pc = sigmapsf*pc
         step_pc = step*pc
 
-        if len(beta) == 4 != surf_lum.size:  # Assumes beta = [r_a, beta_0, beta_inf, alpha]
+        # Assumes beta = [r_a, beta_0, beta_inf, alpha]
+        #        gamma = [r_a, gamma_0, gamma_inf, alpha]
+        if logistic:
             beta = beta.copy()
-            beta[0] *= pc
-
-        if len(gamma) == 4 != surf_lum.size:  # Assumes gamma = [r_a, gamma_0, gamma_inf, alpha]
             gamma = gamma.copy()
+            beta[0] *= pc
             gamma[0] *= pc
 
         # Add a Gaussian with small sigma and the same total mass as the BH.
         # The Gaussian provides an excellent representation of the second moments
         # of a point-like mass, to 1% accuracy out to a radius 2*sigmaBH.
         # The error increases to 14% at 1*sigmaBH, independently of the BH mass.
-        if mbh > 0:
+        if mbh > 0 and analytic_los:
             tmp = np.concatenate([sigmapsf, [pixsize], sigma_lum])
             assert rbh > 0.01*np.min(tmp[tmp > 0]), "`rbh` is too small"
             sigmaBH_pc = rbh*pc # Adopt for the BH just a very small size
             surfBH_pc = mbh/(2*np.pi*sigmaBH_pc**2)
             surf_pot_pc = np.append(surfBH_pc, surf_pot_pc) # Add Gaussian to potential only!
             sigma_pot_pc = np.append(sigmaBH_pc, sigma_pot_pc)
             qobs_pot = np.append(1., qobs_pot)  # Make sure vectors do not have extra dimensions
@@ -801,16 +899,17 @@
         qobs_pot = qobs_pot.clip(0, 0.999999)
 
         t = clock()
         model, psfConvolution, vel, vel2 = psf_conv(
             xbin_pc, ybin_pc, inc,
             surf_lum_pc, sigma_lum_pc, qobs_lum,
             surf_pot_pc, sigma_pot_pc, qobs_pot,
-            beta, gamma, moment, align, sigmaPsf_pc, normpsf,
-            pixSize_pc, pixang, step_pc, nrad, nang, nlos, epsrel, interp, analytic_los)
+            mbh, beta, gamma, logistic, moment, align, sigmaPsf_pc, normpsf,
+            pixSize_pc, pixang, step_pc, nrad, nang, nlos, epsrel,
+            interp, analytic_los)
 
         if moment in str2[:3]:
             model = np.sqrt(model.clip(0))  # sqrt and clip to allow for rounding errors
 
         # Analytic convolution of the MGE model with an MGE circular PSF
         # using Equations (4,5) of Cappellari (2002, MNRAS, 333, 400).
         # Broadcast triple loop over (n_MGE, n_PSF, n_bins)
```

### Comparing `jampy-7.0.10/jampy/jam_sph_intr.py` & `jampy-7.1.0/jampy/jam_sph_intr.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,26 +31,26 @@
 from scipy import special
 import numpy as np
 
 from jampy.quad1d import quad1d
 
 ##############################################################################
 
-def integrand(t, sigma_lum, sigma_pot, dens_lum, mass, Mbh, r, beta, component):
+def integrand(t, sigma_lum, sigma_pot, dens_lum, mass, Mbh, r, beta, logistic, component):
     """
     Implements the integrand of equation (40) of Cappellari (2008, MNRAS, 390, 71).
     Also allows for an analytic radial variation of the anisotropy.
 
     """ 
     # TANH Change of variables for Jeans r-integral (Sec.6.2 of Cappellari 2020, MNRAS, 494, 4819)
     # np.log([1e-6*mds, 3*mxs]) -> [r, inf]
     drdt = np.exp(t)
     r1 = r + drdt[:, None]    # Broadcast over radii and MGE parameters
 
-    if len(beta) == 4 != dens_lum.size:
+    if logistic:
         # Variable anisotropy, same for all Gaussians
         ra, beta0, betainf, alpha = beta
         fun = (r1/r)**(2*beta0)
         fun *= ((1 + (r1/ra)**alpha)/(1 + (r/ra)**alpha))**(2*(betainf - beta0)/alpha)
         beta = beta0 + (betainf - beta0)/(1 + (ra/r)**alpha)
     else:
         # Constant anisotropy, different per Gaussian
@@ -127,15 +127,15 @@
 
     beta: array_like with shape (n,) or (4,)
         Radial anisotropy of the individual kinematic-tracer MGE Gaussians
         (Default: ``beta=np.zeros(n)``)::
 
             beta = 1 - (sigma_th/sigma_r)^2
 
-        When ``len(beta) == 4`` the procedure assumes::
+        When ``logistic=True`` the procedure assumes::
 
             beta = [r_a, beta_0, beta_inf, alpha]
 
         and the anisotropy of the whole JAM model varies as a logistic
         function of the logarithmic spherical radius::
 
             beta(r) = beta_0 + (beta_inf - beta_0)/[1 + (r_a/r)^alpha]
@@ -145,14 +145,19 @@
         transition radius, with ``alpha`` controlling the sharpness of the
         transition. In the special case ``beta_0 = 0, beta_inf = 1, alpha = 2``
         the anisotropy variation reduces to the form by Osipkov & Merritt, but
         the extra parameters allow for much more realistic anisotropy profiles.
     epsrel: float, optional
         Relative error requested for the numerical quadrature
         (Default: ``epsrel=1e-2``)
+    logistic: bool, optional
+        When ``logistic=True``, JAM interprets the anisotropy parameter
+        ``beta`` as defining a 4-parameters logistic function.
+        See the documentation of the anisotropy keyword for details.
+        (Default ``logistic=False``)
 
     Output Parameters
     -----------------
 
     Returned as attributes of the ``jam_sph_intr`` class.
 
     .flux: array_like  with shape (p,)
@@ -167,30 +172,31 @@
         sig2th: array_like with shape (p,)
             Squared intrinsic dispersion in ``(km/s)^2`` along the th
             direction at each ``r`` location.
 
     """
 
     def __init__(self, dens_lum, sigma_lum, dens_pot, sigma_pot, mbh, rad,
-                 beta=None, epsrel=1e-2, quiet=False):
+                 beta=None, epsrel=1e-2, logistic=False, quiet=False):
 
         if beta is None:
             beta = np.zeros_like(dens_lum)
-        assert (dens_lum.size == sigma_lum.size) and ((len(beta) == 4)^(len(beta) == dens_lum.size)), \
+        assert (dens_lum.size == sigma_lum.size) and \
+               ((len(beta) == 4 and logistic) or (len(beta) == dens_lum.size)), \
             "The luminous MGE components and anisotropies do not match"
         assert len(dens_pot) == len(sigma_pot), 'surf_pot and sigma_pot must have the same length'
 
         t = clock()
 
         mass = dens_pot*(np.sqrt(2*np.pi)*sigma_pot)**3
         lim = np.log([1e-6*np.median(sigma_lum), 3*np.max(sigma_lum)])
         nu_sig2r, nu_sig2th = np.empty((2, rad.size))
 
         for j, rj in enumerate(rad):
-            args = [sigma_lum, sigma_pot, dens_lum, mass, mbh, rj, beta]
+            args = [sigma_lum, sigma_pot, dens_lum, mass, mbh, rj, beta, logistic]
             nu_sig2r[j], nu_sig2th[j] = \
                 [quad1d(integrand, lim, epsrel=epsrel, args=args+[txt]).integ
                  for txt in ['sig2r', 'sig2th']]
 
         self.rad = rad
         self.flux = (dens_lum*np.exp(-0.5*(rad[:, None]/sigma_lum)**2)).sum(1)
         self.model = nu_sig2r/self.flux, nu_sig2th/self.flux
```

### Comparing `jampy-7.0.10/jampy/jam_sph_proj.py` & `jampy-7.1.0/jampy/jam_sph_proj.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,23 +116,20 @@
     #    Eq.(8.17.20) of Olver et al. (2010) https://dlmf.nist.gov/8.17.E20
     #    After suggestion by Gary Mamon. MC, Oxford, 16/APR/2009
 
     a = a + 4.76123e-7  # Perturb to avoid singularities in gamma and betainc
     if np.all(a > 0):
         ib = special.betainc(a, b, x)
     else:
-        p = int(np.ceil(abs(np.min(a))))
-        tot = 0
-        gam1 = special.gamma(a + b)
-        gam2 = special.gamma(1 + a)
-        for j in range(p):
-            tot += gam1/gam2*x**(j + a)
-            gam1 *= j + b + a   # Gamma recurrence https://dlmf.nist.gov/5.5#E1
-            gam2 *= j + 1 + a
-        ib = tot*(1 - x)**b/special.gamma(b) + special.betainc(a + p, b, x)
+        p = np.ceil(abs(np.min(a)))
+        j = np.arange(p) + a
+        gam1 = special.gamma(j + b)
+        gam2 = special.gamma(j + 1)
+        tot = (gam1/gam2*x**j).sum(1)
+        ib = tot[:, None]*(1 - x)**b/special.gamma(b) + special.betainc(a + p, b, x)
 
     return ib*special.beta(a, b)
 
 ##############################################################################
 
 def integrand2d(s, t, sigma_lum, sigma_pot, dens_lum, mass, Mbh, rmin, beta, tensor):
     """
@@ -226,16 +223,17 @@
 
     integ = G*nuf*mass_r   # Vector of values computed at different radii
 
     return integ*drdt
 
 ##############################################################################
 
-def second_moment(R, sig_lum, sig_pot, dens_lum, mass, Mbh, beta, tensor, ra,
-                     sigmaPsf, normPsf, step, nrad, surf_lum, pixSize, epsrel):
+def second_moment(R, sig_lum, sig_pot, dens_lum, mass, Mbh, beta, logistic,
+                  tensor, ra, sigmaPsf, normPsf, step, nrad, surf_lum, pixSize,
+                  epsrel):
     """
     This routine gives the second V moment after convolution with a PSF.
     The convolution is done using interpolation of the model on a
     polar grid, as described in Appendix A of Cappellari (2008).
 
     """
     psfConvolution = (np.max(sigmaPsf) > 0) and (pixSize > 0)
@@ -258,15 +256,15 @@
 
         # The model Vrms computation is only performed on the radial grid
         # which is then used to interpolate the values at any other location
         #
         wm2Pol = np.empty_like(rr)
         for j, rj in enumerate(rr):     # Integration of equation (50)
             args = [sig_lum, sig_pot, dens_lum, mass, Mbh, rj, beta, tensor]
-            if len(beta) == 4 != dens_lum.size:
+            if logistic:
                 wm2Pol[j] = quad2d(integrand2d, lim, lim, epsrel=epsrel, args=args).integ
             else:
                 wm2Pol[j] = quad1d(integrand1d, lim, epsrel=epsrel, args=args+[ra]).integ
 
         nx = int(np.ceil(rmax/step))
         x1 = np.linspace(0.5 - nx, nx - 0.5, 2*nx)*step
         xCar, yCar = np.meshgrid(x1, x1)  # Cartesian grid for convolution
@@ -288,32 +286,32 @@
         dx = pixSize/2
         sp = np.sqrt(2)*sigmaPsf
         xg, yg = xgrid[..., None], ygrid[..., None]
         kernel = normPsf*(special.erf((dx - xg)/sp) + special.erf((dx + xg)/sp)) \
                         *(special.erf((dx - yg)/sp) + special.erf((dx + yg)/sp))
         kernel = np.sum(kernel, 2)   # Sum over PSF components
 
-        # Seeing and aperture convolution with equation (A3)
+        # Seeing and aperture convolution with equation (A3) of Cappellari (2008)
         #
-        muCar = np.sqrt(signal.fftconvolve(wm2Car, kernel, mode='same')
-                      / signal.fftconvolve(mgeCar, kernel, mode='same'))
+        m1, m2 = signal.fftconvolve([wm2Car, mgeCar], kernel[None, ...], mode='same')
+        muCar = np.sqrt(m1/m2)
 
         # Interpolate convolved image at observed apertures.
         # Aperture integration was already included in the kernel.
         #
         sigp = bilinear_interpolate(x1, x1, muCar, R/np.sqrt(2), R/np.sqrt(2))
 
     else: # No PSF convolution: just compute values
 
         assert np.all(R > 0), "One must avoid the singularity at `R = 0`"
 
         sigp = np.empty_like(R)
         for j, rj in enumerate(R):
             args = [sig_lum, sig_pot, dens_lum, mass, Mbh, rj, beta, tensor]
-            if len(beta) == 4 != dens_lum.size:
+            if logistic:
                 wm2Pol = quad2d(integrand2d, lim, lim, epsrel=epsrel, args=args).integ
             else:
                 wm2Pol = quad1d(integrand1d, lim, epsrel=epsrel, args=args+[ra]).integ
             mgePol = np.sum(surf_lum*np.exp(-0.5*(rj/sig_lum)**2))
             sigp[j] = np.sqrt(wm2Pol/mgePol)
 
     return sigp, psfConvolution
@@ -322,17 +320,19 @@
 
 class jam_sph_proj:
 
     """
     PURPOSE
     -------
 
-    This procedure calculates a prediction for any of the three components of the
+    This procedure calculates a prediction for any of the three components of
+    the
     the projected second velocity moments V_RMS = sqrt(V^2 + sigma^2), or for a
-    non-rotating galaxy V_RMS = sigma, for an anisotropic spherical galaxy model.
+    non-rotating galaxy V_RMS = sigma, for an anisotropic spherical galaxy
+    model.
     It implements the solution of the anisotropic Jeans equations
     presented in equation (50) of `Cappellari (2008, MNRAS, 390, 71).
     <https://ui.adsabs.harvard.edu/abs/2008MNRAS.390...71C>`_
     PSF convolution is done as described in the Appendix of Cappellari (2008).
     This procedure includes the proper motions calculation given in
     Appendix B3 of `Cappellari (2020, MNRAS, 494, 4819)
     <https://ui.adsabs.harvard.edu/abs/2020MNRAS.494.4819C>`_
@@ -400,15 +400,15 @@
 
     beta: array_like with shape (n,) or (4,)
         Radial anisotropy of the individual kinematic-tracer MGE Gaussians
         (Default: ``beta=np.zeros(n)``)::
 
             beta = 1 - (sigma_th/sigma_r)^2  # with align=`sph`
 
-        When ``len(beta) == 4`` the procedure assumes::
+        When ``logistic=True`` the procedure assumes::
 
             beta = [r_a, beta_0, beta_inf, alpha]
 
         and the anisotropy of the whole JAM model varies as a logistic
         function of the logarithmic spherical radius::
 
             beta(r) = beta_0 + (beta_inf - beta_0)/[1 + (r_a/r)^alpha]
@@ -421,25 +421,31 @@
         the extra parameters allow for much more realistic anisotropy profiles.
     data:
         Vector of length P with the input observed stellar
         V_RMS=sqrt(velBin^2 + sigBin^2) at the coordinates positions
         given by the vector RAD.
 
         If RMS is set and ML is negative or not set, then the model is fitted to
-        the data, otherwise the adopted ML is used and just the chi^2 is returned.
+        the data, otherwise the adopted ML is used and just the chi^2 is
+        returned.
     epsrel: float, optional
         Relative error requested for the numerical quadrature
         (Default: ``epsrel=1e-2``)
     errors:
         Vector of length P with the 1sigma errors associated to the RMS
         measurements. From the error propagation
         ERMS = sqrt((dVel*velBin)^2 + (dSig*sigBin)^2)/RMS,
         where velBin and sigBin are the velocity and dispersion in each bin
         and dVel and dSig are the corresponding errors
         (Default: constant errors=0.05*MEDIAN(data)).
+    logistic: bool, optional
+        When ``logistic=True``, JAM interprets the anisotropy parameter
+        ``beta`` as defining a 4-parameters logistic function.
+        See the documentation of the anisotropy keyword for details.
+        (Default ``logistic=False``)
     ml:
         Mass-to-light ratio to multiply the values given by SURF_POT.
         Setting this keyword is completely equivalent to multiplying the
         output RMSMODEL by SQRT(M/L) after the fit. This implies that the
         BH mass becomes MBH*(M/L).
 
         If this keyword is set to a negative number in input, the M/L is
@@ -493,47 +499,59 @@
         cases however, e.g. to accurately estimate the central Vrms in a very
         cuspy galaxy inside a large aperture, one may want to override the
         default value to force smaller spatial pixels using this keyword.
 
         Use this keyword to set the desired scale of the model when no PSF or
         pixel convolution is performed (SIGMAPSF=0 or PIXSIZE=0).
     tensor:
-        Specifies any of the three component of the projected velocity dispersion
-        tensor one wants to calculate. Possible options are (i) "los" (default) for
-        the line-of-sight component; (ii) "pmr" for tha radial component of the proper
-        motion second moment and (iii) "pmt" for the tangential component of the proper
-        motion second moment. All three components are computed in km/s at the adopted
+        Specifies any of the three component of the projected velocity
+        dispersion
+        tensor one wants to calculate. Possible options are (i) "los" (
+        default) for
+        the line-of-sight component; (ii) "pmr" for tha radial component of
+        the proper
+        motion second moment and (iii) "pmt" for the tangential component of
+        the proper
+        motion second moment. All three components are computed in km/s at
+        the adopted
         distance.
 
     OUTPUT PARAMETERS
     -----------------
 
     attributes of the ``jam_sph_proj`` class
 
-    model:
-        Vector of length P with the model predictions for the velocity
-        second moments (sigma in the spherical non-rotating case) of each bin.
-        The line-of-sigh component or either of the proper motion components can
-        be obtained in output using the ``tensor`` keyword.
-    ml:
+    .model: array_like with shape (p,)
+        Model predictions for the velocity second moments (sigma in the
+        spherical non-rotating case) of each bin. The line-of-sigh component
+        or either of the proper motion components can be obtained in output
+        using the ``tensor`` keyword.
+    .ml:
         best fitting M/L.
-    chi2:
+    .chi2:
         Reduced chi^2 describing the quality of the fit::
 
             chi^2 = total( ((rms-rmsModel)/erms)^2 ) / n_elements(rms)
+
+    .flux: array_like with shape (p,)
+        PSF-convolved MGE surface brightness of each bin in ``Lsun/pc^2``,
+        useful to plot the isophotes of the kinematic-tracer on the model
+        results.
     """
 
     def __init__(self, surf_lum, sigma_lum, surf_pot, sigma_pot, mbh, distance,
-                 rad, beta=None, data=None, epsrel=1e-2, errors=None, ml=None,
-                 normpsf=1, nrad=50, pixsize=0, plot=True, quiet=False,
-                 rani=None, sigmapsf=0, step=0, tensor='los'):
+                 rad, beta=None, data=None, epsrel=1e-2, errors=None,
+                 logistic=False, ml=None, normpsf=1, nrad=50, pixsize=0,
+                 plot=True, quiet=False, rani=None, sigmapsf=0, step=0,
+                 tensor='los'):
 
         if beta is None:
             beta = np.zeros_like(surf_lum)
-        assert (surf_lum.size == sigma_lum.size) and ((len(beta) == 4)^(len(beta) == surf_lum.size)), \
+        assert (surf_lum.size == sigma_lum.size) and \
+               ((len(beta) == 4 and logistic) or (len(beta) == surf_lum.size)), \
             "The luminous MGE components and anisotropies do not match"
         assert len(surf_pot) == len(sigma_pot), 'surf_pot and sigma_pot must have the same length'
         assert tensor in ["los", "pmr", "pmt"], 'tensor must be: los, pmr or pmt'
         if rani is not None:
             assert tensor == 'los', "Only tensor='los' implemented for Osipkov-Merritt"
         if (errors is None) and (data is not None):
             errors = np.full_like(data, np.median(data)*0.05)  # Constant ~5% errors
@@ -541,15 +559,15 @@
         sigmapsf = np.atleast_1d(sigmapsf)
         normpsf = np.atleast_1d(normpsf)
         assert sigmapsf.size == normpsf.size, "sigmaPSF and normPSF do not match"
         assert round(np.sum(normpsf), 2) == 1, "PSF not normalized"
 
         pc = distance*np.pi/0.648 # Constant factor to convert arcsec --> pc
 
-        sigmaPsf = sigmapsf*pc
+        sigmapsf_pc = sigmapsf*pc
         pixsize_pc = pixsize*pc
         step_pc = step*pc
 
         integ = 'quad1d'
         if len(beta) == 4 != surf_lum.size:  # Assumes beta = [r_a, beta_0, beta_inf, alpha]
             integ = 'quad2d'
             beta = beta.copy()
@@ -562,32 +580,41 @@
         dens_lum = surf_lum/(np.sqrt(2*np.pi)*sigma_lum_pc)
 
         sigma_pot_pc = sigma_pot*pc     # Convert from arcsec to pc
         mass = 2*np.pi*surf_pot*sigma_pot_pc**2
 
         t = clock()
         model, psfConvolution = second_moment(rad*pc, sigma_lum_pc,
-            sigma_pot_pc, dens_lum, mass, mbh, beta, tensor, rani, sigmaPsf,
-            normpsf, step_pc, nrad, surf_lum, pixsize_pc, epsrel)
+            sigma_pot_pc, dens_lum, mass, mbh, beta, logistic, tensor, rani,
+            sigmapsf_pc, normpsf, step_pc, nrad, surf_lum, pixsize_pc, epsrel)
 
         if not quiet:
             print(f'jam_sph_proj elapsed time sec: {clock() - t:.2f} ({integ})')
             if not psfConvolution:
                 txt = "No PSF convolution:"
                 if np.max(sigmapsf) == 0:
                     txt += " sigmapsf == 0;"
                 if pixsize == 0:
                     txt += " pixsize == 0;"
                 print(txt)
 
+        # Analytic convolution of the MGE model with an MGE circular PSF
+        # using Equations (4,5) of Cappellari (2002, MNRAS, 333, 400).
+        # Broadcast triple loop over (n_MGE, n_PSF, n_bins)
+        sigma2 = sigma_lum**2 + sigmapsf[:, None]**2
+        surf_conv = surf_lum*sigma_lum**2*normpsf[:, None]/np.sqrt(sigma2)
+        flux = surf_conv[..., None]*np.exp(-0.5*rad**2/sigma2[..., None])
+        flux = flux.sum((0, 1))  # PSF-convolved Lsun/pc^2
+
         self.pixsize = pixsize
         self.rad = rad
         self.data = data
         self.errors = errors
         self.model = model
+        self.flux = flux
 
         ####### Output and optional M/L fit
         # If `data`` keyword is not given all this section is skipped
 
         if data is not None:
 
             if (ml is None) or (ml <= 0):
```

### Comparing `jampy-7.0.10/jampy/mge_half_light_isophote.py` & `jampy-7.1.0/jampy/mge_half_light_isophote.py`

 * *Files identical despite different names*

### Comparing `jampy-7.0.10/jampy/mge_radial_density.py` & `jampy-7.1.0/jampy/mge_radial_density.py`

 * *Files identical despite different names*

### Comparing `jampy-7.0.10/jampy/mge_radial_mass.py` & `jampy-7.1.0/jampy/mge_radial_mass.py`

 * *Files identical despite different names*

### Comparing `jampy-7.0.10/jampy/mge_vcirc.py` & `jampy-7.1.0/jampy/mge_vcirc.py`

 * *Files identical despite different names*

### Comparing `jampy-7.0.10/jampy/quad1d.py` & `jampy-7.1.0/jampy/quad1d.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,15 +268,14 @@
             print('***Too many sub intervals.')
         OK = False
 
     if plot:
         plt.figure('quad1d')
         w = np.argsort(xall)
         plt.plot(xall[w], yall[w])
-        plt.pause(0.1)
 
     return Ifx, errbnd, OK, fcall, vfcall
 
 ################################################################################
 
 class quad1d:
     """
```

### Comparing `jampy-7.0.10/jampy/quad2d.py` & `jampy-7.1.0/jampy/quad2d.py`

 * *Files identical despite different names*

### Comparing `jampy-7.0.10/jampy.egg-info/PKG-INFO` & `jampy-7.1.0/jampy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jampy
-Version: 7.0.10
+Version: 7.1.0
 Summary: JamPy: Jeans Anisotropic Models for Galactic Dynamics
 Home-page: https://purl.org/cappellari/software
 Author: Michele Cappellari
 Author-email: michele.cappellari@physics.ox.ac.uk
 License: Other/Proprietary License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -133,22 +133,25 @@
   `Cappellari (2020) <https://ui.adsabs.harvard.edu/abs/2020MNRAS.494.4819C>`_
 
 Calling Sequence
 ----------------
 
 .. code-block:: python
 
+    from jampy.jam_axi_proj import jam_axi_proj
+
     jam = jam_axi_proj(
              surf_lum, sigma_lum, qobs_lum, surf_pot, sigma_pot, qobs_pot,
              inc, mbh, distance, xbin, ybin, align='cyl', analytic_los=True,
              beta=None, data=None, epsrel=1e-2, errors=None, flux_obs=None,
-             gamma=None, goodbins=None, interp=True, kappa=None, ml=None,
-             moment='zz', nang=10, nlos=1500, nodots=False, normpsf=1.,
-             nrad=20, pixang=0., pixsize=0., plot=True, quiet=False,
-             rbh=0.01, sigmapsf=0., step=0., vmax=None, vmin=None)
+             gamma=None, goodbins=None, interp=True, kappa=None,
+             logistic=False, ml=None, moment='zz', nang=10, nlos=1500,
+             nodots=False, normpsf=1., nrad=20, pixang=0., pixsize=0.,
+             plot=True, quiet=False, rbh=0.01, sigmapsf=0., step=0.,
+             vmax=None, vmin=None)
 
     vrms = jam.model  # with moment='zz' the output is the LOS Vrms
 
     jam.plot()   # Generate data/model comparison when data is given
 
 See more examples in the ``jampy/examples`` folder inside
 `site-packages <https://stackoverflow.com/a/46071447>`_.
@@ -251,15 +254,15 @@
 beta: array_like with shape (n,) or (4,)
     Radial anisotropy of the individual kinematic-tracer MGE Gaussians
     (Default: ``beta=np.zeros(n)``)::
 
         beta = 1 - (sigma_th/sigma_r)^2  # with align='sph'
         beta = 1 - (sigma_z/sigma_R)^2   # with align='cyl'
 
-    When ``len(beta) == 4`` the procedure assumes::
+    When ``logistic=True`` the procedure assumes::
 
         beta = [r_a, beta_0, beta_inf, alpha]
 
     and the anisotropy of the whole JAM model varies as a logistic
     function of the logarithmic spherical radius (with ``align='sph'``) or
     of the logarithmic distance from the equatorial plane (with ``align='cyl'``)::
 
@@ -268,14 +271,16 @@
 
     Here ``beta_0`` represents the anisotropy at ``r = 0``, ``beta_inf``
     is the anisotropy at ``r = inf`` and ``r_a`` is the anisotropy
     transition radius, with ``alpha`` controlling the sharpness of the
     transition. In the special case ``beta_0 = 0, beta_inf = 1, alpha = 2``
     the anisotropy variation reduces to the form by Osipkov & Merritt, but
     the extra parameters allow for much more realistic anisotropy profiles.
+    See an application in `Simon, Cappellari & Hartke (2023)
+    <https://ui.adsabs.harvard.edu/abs/2023arXiv230318229S>`_.
 data: array_like with shape (p,), optional
     observed first or second velocity moment used to fit the model.
 
     EXAMPLE: In the common case where one has only line-of-sight velocities
     the second moment is given by::
 
         Vrms = np.sqrt(velBin**2 + sigBin**2)
@@ -304,15 +309,15 @@
 gamma: array_like with shape (n,)
     tangential anisotropy of the individual kinematic-tracer MGE Gaussians
     (Default: ``gamma=np.zeros(n)``)::
 
         gamma = 1 - (sigma_phi/sigma_r)^2  # with align='sph'
         gamma = 1 - (sigma_phi/sigma_R)^2  # with align='cyl'
 
-    When ``len(gamma) == 4`` the procedure assumes::
+    When ``logistic=True`` the procedure assumes::
 
         gamma = [r_a, gamma_0, gamma_inf, alpha]
 
     and the anisotropy of the whole JAM model varies as a logistic
     function of the logarithmic spherical radius (with ``align='sph'``) or
     of the logarithmic distance from the equatorial plane (with ``align='cyl'``)::
 
@@ -346,14 +351,19 @@
     to compute all moments, including proper motions,  simultaneously.
 kappa: float, optional
     When ``kappa=None`` (default) the first velocity moments are scaled in
     such a way that the projected angular momentum of the data and model is
     the same [equation 52 of `Cappellari (2008)`_].
     When ``kappa=1`` the model first velocity moments are output without
     any scaling.
+logistic: bool, optional
+    When ``logistic=True``, JAM interprets the anisotropy parameters
+    ``beta`` and ``gamma`` as defining a 4-parameters logistic function.
+    See the documentation of the anisotropy keywords for details.
+    (Default ``logistic=False``)
 ml: float, optional
     Mass-to-light ratio (M/L) to multiply the values given by ``surf_pot``.
     Setting this keyword is completely equivalent to multiplying the
     output ``model`` by ``np.sqrt(M/L)`` after the fit. This implies that
     the BH mass is also scaled and becomes ``mbh*ml``.
 
     If ``ml=None`` (default) the M/L is fitted from the data and the
@@ -427,15 +437,17 @@
     PSF convolution is not performed.
 plot: bool
     When ``data is not None`` setting this keyword produces a plot with the
     data/model comparison at the end of the calculation.
 quiet: bool
     Set this keyword to avoid printing values on the console.
 rbh: float, optional
-    This scalar gives the sigma in arcsec of the Gaussian representing the
+    This keyword is ignored unless ``align='cyl'`` and `analytic_los=True`.
+    In all other cases JAM assume a point-like central black hole.
+    This scalar gives the sigma in arcsec of the Gaussian approximating the
     central black hole of mass MBH [See Section 3.1.2 of `Cappellari (2008)`_]
     The gravitational potential is indistinguishable from a point source
     for ``radii > 2*rbh``, so the default ``rbh=0.01`` arcsec is appropriate
     in most current situations.
 
     When using different units as input, e.g. pc instead of arcsec, one
     should check that ``rbh`` is not too many order of magnitude smaller
@@ -542,20 +554,22 @@
   `Cappellari (2020) <https://ui.adsabs.harvard.edu/abs/2020MNRAS.494.4819C>`_
 
 Calling Sequence
 ----------------
 
 .. code-block:: python
 
+    from jampy.jam_axi_intr import jam_axi_intr
+
     jam = jam_axi_intr(
              dens_lum, sigma_lum, qintr_lum, dens_pot, sigma_pot, qintr_pot,
-             mbh, Rbin, zbin, align='cyl', beta=None, data=None,
-             epsrel=1e-2, errors=None, gamma=None, goodbins=None,
-             interp=True, ml=None, nang=10, nodots=False, nrad=20,
-             plot=True, proj_cyl=False, quiet=False, rbh=1)
+             mbh, Rbin, zbin, align='cyl', beta=None, data=None, epsrel=1e-2,
+             errors=None, gamma=None, goodbins=None, interp=True,
+             logistic=False, ml=None, nang=10, nodots=False, nrad=20,
+             plot=True, proj_cyl=False, quiet=False)
 
     # The meaning of the output is different depending on `align`
     sig2R, sig2z, sig2phi, v2phi = jam.model  # with align='cyl'
     sig2r, sig2th, sig2phi, v2phi = jam.model  # with align='sph'
 
     jam.plot()   # Generate data/model comparison
 
@@ -611,15 +625,15 @@
 beta: array_like with shape (n,) or (4,)
     Vector with the axial anisotropy of the individual kinematic-tracer
     MGE Gaussians (Default: ``beta=np.zeros(n)``)::
 
         beta = 1 - (sigma_th/sigma_r)^2  # with align='sph'
         beta = 1 - (sigma_z/sigma_R)^2   # with align='cyl'
 
-    When ``len(beta) == 4`` the procedure assumes::
+    When ``logistic=True`` the procedure assumes::
 
         beta = [r_a, beta_0, beta_inf, alpha]
 
     and the anisotropy of the whole JAM model varies as a logistic
     function of the logarithmic spherical radius (with ``align='sph'``) or
     of the logarithmic distance from the equatorial plane (with ``align='cyl'``)::
 
@@ -628,14 +642,16 @@
 
     Here ``beta_0`` represents the anisotropy at ``r = 0``, ``beta_inf``
     is the anisotropy at ``r = inf`` and ``r_a`` is the anisotropy
     transition radius, with ``alpha`` controlling the sharpness of the
     transition. In the special case ``beta_0 = 0, beta_inf = 1, alpha = 2``
     the anisotropy variation reduces to the form by Osipkov & Merritt, but
     the extra parameters allow for much more realistic anisotropy profiles.
+    See an application in `Simon, Cappellari & Hartke (2023)
+    <https://ui.adsabs.harvard.edu/abs/2023arXiv230318229S>`_.
 data: array_like of shape (4, p), optional
     Four input vectors with the observed values of:
 
     - ``[sigR, sigz, sigphi, vrms_phi]`` in ``km/s``, when ``align='cyl'``
       (or ``align='sph'`` and ``proj_cyl=True``).
 
       ``vrms_phi`` is the square root of the velocity second moment in the
@@ -655,15 +671,15 @@
 gamma: array_like with shape (n,)
     Vector with the tangential anisotropy of the individual kinematic-tracer
     MGE Gaussians (Default: ``gamma=np.zeros(n)``)::
 
         gamma = 1 - (sigma_phi/sigma_r)^2  # with align='sph'
         gamma = 1 - (sigma_phi/sigma_R)^2  # with align='cyl'
 
-    When ``len(gamma) == 4`` the procedure assumes::
+    When ``logistic=True`` the procedure assumes::
 
         gamma = [r_a, gamma_0, gamma_inf, alpha]
 
     and the anisotropy of the whole JAM model varies as a logistic
     function of the logarithmic spherical radius (with ``align='sph'``) or
     of the logarithmic distance from the equatorial plane (with ``align='cyl'``)::
 
@@ -681,14 +697,19 @@
     for the bins which have to be included in the fit (if requested) and
     ``chi^2`` calculation (Default: fit all bins).
 interp: bool, optional
     If ``interp=False`` no interpolation is performed and the model is
     computed at every set of input (R, z) coordinates.
     If ``interp=True`` (default), the model is interpolated if the number
     of requested input (R, z) coordinates is larger than ``nang*nrad``.
+logistic: bool, optional
+    When ``logistic=True``, JAM interprets the anisotropy parameters
+    ``beta`` and ``gamma`` as defining a 4-parameters logistic function.
+    See the documentation of the anisotropy keywords for details.
+    (Default ``logistic=False``)
 ml: float, optional
     Mass-to-light ratio M/L. If ``ml=None`` (default) the M/L is fitted to
     the data and the best-fitting value is returned in output.
     The ``mbh`` is also scaled and becomes ``mbh*ml``.
     If ``ml=1`` no scaling is applied to the model.
 nang: int, optional
     The number of linearly-spaced intervals in the eccentric anomaly at
@@ -710,20 +731,14 @@
     ``[sig2R, sig2z, sig2phi, v2phi]`` components as in the case
     ``align='cyl'``. This is useful for a direct comparison of results with
     either the spherical or cylindrical alignment, as it allows one to fit
     the same data with both modelling assumptions.
 quiet: bool, optional
     If ``quiet=False`` (default), print the best-fitting M/L and chi2 at
     the end for the calculation.
-rbh: float, optional
-    This scalar gives the sigma in pc of the Gaussian representing the
-    central black hole of mass ``mbh`` [See Section 3.1.2 of
-    `Cappellari (2008)`_]. The gravitational potential is indistinguishable
-    from a point source for ``radii > 2*rbh``, so the default ``rbh=1`` pc
-    is appropriate for observations taken with current telescopes.
 
 Output Parameters
 -----------------
 
 Returned as attributes of the ``jam_axi_intr`` class.
 
 .chi2: float
@@ -784,14 +799,39 @@
 provided this copyright and disclaimer are included in all 
 copies of the software. All other rights are reserved.
 In particular, redistribution of the code is not allowed.
 
 Changelog
 =========
 
+V7.1.0: MC, Oxford, 1 June 2023
+    - Separated computation for the black hole kinematics for both the
+      cylindrically and spherically-aligned solutions. In both cases this
+      removed one numerical quadrature. This is useful in extreme situations,
+      when the minimum radius one wants to model around the black hole is orders
+      of magnitude smaller than the smallest MGE Gaussian. This change
+      eliminated the need for the ``rbh`` keyword in ``jam_axi_intr``, which I
+      removed. The only case where the black hole is still approximated with a
+      small Gaussian is in ``jam_axi_proj`` when both ``align='cyl'`` and
+      ``analytic_los=True``.
+    - Adopted consistent minimum radius, based on ``step``, for both the
+      intrinsic and projected interpolation grids.
+    - Simplified minimum-inclination test.
+    - Removed ``legacy`` folder with old redundant procedures.
+    - Moved the formalism for the LOS analytic integrand with ``align='cyl'``
+      into ``jam_axi_proj``.
+    - ``jam_axi_proj``, ``jam_axi_intr``, ``jam_sph_proj``, ``jam_sph_intr``:
+      New keyword ``logistic`` to specify when JAM should interpret the input
+      anisotropy parameters ``beta`` and ``gamma`` as defining a logistic
+      function anisotropy profile.
+    - ``jam_axi_intr``: Use DE quadrature from ``[z, inf]`` instead of
+      ``[0, 1]`` with ``align='cyl'`` as already done with ``align='sph'``.
+    - ``jam_hernquist_model_example``: New test against Osipkov-Merritt radial
+      variation of the anisotropy using ``logistic=True``. Revised plot.
+
 V7.0.10: MC, Oxford, 17 January 2023
     - Introduced an analytic radial variation of the anisotropy ``beta``
       and ``gamma`` using a flexible logistic function of logarithmic radius
       ``beta(r) = beta_0 + (beta_inf - beta_0)/[1 + (r_a/r)^alpha]``.
       This function specifies the inner/outer anisotropy ``beta_0`` and
       ``beta_inf``, the anisotropy radius ``r_a`` and the sharpness ``alpha``
       of the transition. This new function is an alternative to assigning
```

### Comparing `jampy-7.0.10/jampy.egg-info/SOURCES.txt` & `jampy-7.1.0/jampy.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -25,12 +25,8 @@
 jampy/examples/jam_axi_proj_example.py
 jampy/examples/jam_black_hole_bayes_example.py
 jampy/examples/jam_dark_halo_bayes_example.py
 jampy/examples/jam_hernquist_model_example.py
 jampy/examples/jam_mock_kinematics_black_hole.txt
 jampy/examples/jam_mock_kinematics_dark_halo.txt
 jampy/examples/jam_sph_proj_example.py
-jampy/examples/mge_vcirc_example.py
-jampy/legacy/__init__.py
-jampy/legacy/jam_axi_rms.py
-jampy/legacy/jam_axi_vel.py
-jampy/legacy/jam_sph_rms.py
+jampy/examples/mge_vcirc_example.py
```

### Comparing `jampy-7.0.10/setup.py` & `jampy-7.1.0/setup.py`

 * *Files identical despite different names*

