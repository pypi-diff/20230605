# Comparing `tmp/hhpy-0.3.0.tar.gz` & `tmp/hhpy-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, from Unix
+gzip compressed data, was "hhpy-0.3.1.tar", last modified: Mon Jun  5 12:50:07 2023, max compression
```

## Comparing `hhpy-0.3.0.tar` & `hhpy-0.3.1.tar`

### file list

```diff
@@ -1,185 +1,187 @@
-drwxrwxr-x   0 root         (0) root         (0)        0 2021-06-23 04:28:10.000000 hhpy-0.3.0/
--rw-rw-r--   0 root         (0) root         (0)      129 2021-06-23 04:28:10.000000 hhpy-0.3.0/.gitignore
-drwxrwxr-x   0 root         (0) root         (0)        0 2021-06-23 04:28:10.000000 hhpy-0.3.0/.idea/
--rw-rw-r--   0 root         (0) root         (0)       38 2021-06-23 04:28:10.000000 hhpy-0.3.0/.idea/.gitignore
-drwxrwxr-x   0 root         (0) root         (0)        0 2021-06-23 04:28:10.000000 hhpy-0.3.0/.idea/dictionaries/
--rw-rw-r--   0 root         (0) root         (0)     4875 2021-06-23 04:28:10.000000 hhpy-0.3.0/.idea/dictionaries/hanssen_henrik.xml
--rw-rw-r--   0 root         (0) root         (0)      547 2021-06-23 04:28:10.000000 hhpy-0.3.0/.idea/hhpy.iml
-drwxrwxr-x   0 root         (0) root         (0)        0 2021-06-23 04:28:10.000000 hhpy-0.3.0/.idea/inspectionProfiles/
--rw-rw-r--   0 root         (0) root         (0)      228 2021-06-23 04:28:10.000000 hhpy-0.3.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-rw-r--   0 root         (0) root         (0)      192 2021-06-23 04:28:10.000000 hhpy-0.3.0/.idea/misc.xml
--rw-rw-r--   0 root         (0) root         (0)      260 2021-06-23 04:28:10.000000 hhpy-0.3.0/.idea/modules.xml
--rw-rw-r--   0 root         (0) root         (0)      180 2021-06-23 04:28:10.000000 hhpy-0.3.0/.idea/vcs.xml
--rw-rw-r--   0 root         (0) root         (0)        6 2021-06-23 04:28:10.000000 hhpy-0.3.0/.python-version
--rwxrwxr-x   0 root         (0) root         (0)      551 2021-06-23 04:28:10.000000 hhpy-0.3.0/LICENSE.txt
--rwxrwxr-x   0 root         (0) root         (0)      266 2021-06-23 04:28:10.000000 hhpy-0.3.0/Pipfile
--rw-rw-r--   0 root         (0) root         (0)    25951 2021-06-23 04:28:10.000000 hhpy-0.3.0/Pipfile.lock
--rwxrwxr-x   0 root         (0) root         (0)      768 2021-06-23 04:28:10.000000 hhpy-0.3.0/README.md
--rw-rw-r--   0 root         (0) root         (0)       26 2021-06-23 04:28:10.000000 hhpy-0.3.0/_config.yml
-drwxrwxr-x   0 root         (0) root         (0)        0 2021-06-23 04:28:10.000000 hhpy-0.3.0/hhpy.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     1461 2021-06-23 04:28:10.000000 hhpy-0.3.0/hhpy.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      377 2021-06-23 04:28:10.000000 hhpy-0.3.0/hhpy.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2021-06-23 04:28:10.000000 hhpy-0.3.0/hhpy.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       49 2021-06-23 04:28:10.000000 hhpy-0.3.0/hhpy.egg-info/entry_points.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2021-06-23 04:28:10.000000 hhpy-0.3.0/hhpy.egg-info/not-zip-safe
--rw-rw-r--   0 root         (0) root         (0)      108 2021-06-23 04:28:10.000000 hhpy-0.3.0/hhpy.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)        5 2021-06-23 04:28:10.000000 hhpy-0.3.0/hhpy.egg-info/top_level.txt
-drwxrwxr-x   0 root         (0) root         (0)        0 2021-06-23 04:28:10.000000 hhpy-0.3.0/hhpy/
--rw-rw-r--   0 root         (0) root         (0)     6148 2021-06-23 04:28:10.000000 hhpy-0.3.0/hhpy/.DS_Store
--rwxrwxr-x   0 root         (0) root         (0)      330 2021-06-23 04:28:10.000000 hhpy-0.3.0/hhpy/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      287 2021-06-23 04:28:10.000000 hhpy-0.3.0/hhpy/__init__.pyc
--rwxrwxr-x   0 root         (0) root         (0)      434 2021-06-23 04:28:10.000000 hhpy-0.3.0/hhpy/__version__.py
--rw-rw-r--   0 root         (0) root         (0)   107663 2021-06-23 04:28:10.000000 hhpy-0.3.0/hhpy/ds.py
--rwxrwxr-x   0 root         (0) root         (0)     1534 2021-06-23 04:28:10.000000 hhpy-0.3.0/hhpy/entry_points.py
--rw-rw-r--   0 root         (0) root         (0)     5657 2021-06-23 04:28:10.000000 hhpy-0.3.0/hhpy/ipython.py
--rwxrwxr-x   0 root         (0) root         (0)    52008 2021-06-23 04:28:10.000000 hhpy-0.3.0/hhpy/main.py
--rw-rw-r--   0 root         (0) root         (0)    70504 2021-06-23 04:28:10.000000 hhpy-0.3.0/hhpy/modelling.py
--rw-rw-r--   0 root         (0) root         (0)   134008 2021-06-23 04:28:10.000000 hhpy-0.3.0/hhpy/plotting.py
--rw-rw-r--   0 root         (0) root         (0)     4018 2021-06-23 04:28:10.000000 hhpy-0.3.0/hhpy/regression.py
--rw-rw-r--   0 root         (0) root         (0)     3482 2021-06-23 04:28:10.000000 hhpy-0.3.0/release_notes.md
--rw-rw-r--   0 root         (0) root         (0)       61 2021-06-23 04:28:10.000000 hhpy-0.3.0/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)     1437 2021-06-23 04:28:10.000000 hhpy-0.3.0/setup.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/
--rw-rw-r--   0 root         (0) root         (0)     8196 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/.DS_Store
--rw-rw-r--   0 root         (0) root         (0)       12 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/.python-version
--rw-rw-r--   0 root         (0) root         (0)      634 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/Makefile
-drwxrwxr-x   0 root         (0) root         (0)        0 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/_static/
--rw-rw-r--   0 root         (0) root         (0)     6148 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/_static/.DS_Store
-drwxrwxr-x   0 root         (0) root         (0)        0 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/
--rw-rw-r--   0 root         (0) root         (0)    16388 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/.DS_Store
--rw-rw-r--   0 root         (0) root         (0)      589 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ds.DFMapping.rst
--rw-rw-r--   0 root         (0) root         (0)       59 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ds.acc.rst
--rw-rw-r--   0 root         (0) root         (0)      104 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ds.butter_pass_filter.rst
--rw-rw-r--   0 root         (0) root         (0)       83 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ds.change_span.rst
--rw-rw-r--   0 root         (0) root         (0)       56 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ds.cm.rst
--rw-rw-r--   0 root         (0) root         (0)       86 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ds.col_to_front.rst
--rw-rw-r--   0 root         (0) root         (0)       62 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ds.corr.rst
--rw-rw-r--   0 root         (0) root         (0)       74 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ds.df_count.rst
--rw-rw-r--   0 root         (0) root         (0)       62 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ds.df_p.rst
--rw-rw-r--   0 root         (0) root         (0)       71 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ds.df_rmsd.rst
--rw-rw-r--   0 root         (0) root         (0)       74 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ds.df_score.rst
--rw-rw-r--   0 root         (0) root         (0)       74 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ds.df_split.rst
--rw-rw-r--   0 root         (0) root         (0)      107 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ds.drop_duplicate_cols.rst
--rw-rw-r--   0 root         (0) root         (0)      116 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ds.drop_duplicate_indices.rst
--rw-rw-r--   0 root         (0) root         (0)       92 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ds.drop_zero_cols.rst
--rw-rw-r--   0 root         (0) root         (0)       65 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ds.f1_pr.rst
--rw-rw-r--   0 root         (0) root         (0)       71 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ds.f_score.rst
--rw-rw-r--   0 root         (0) root         (0)       83 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ds.get_df_corr.rst
--rw-rw-r--   0 root         (0) root         (0)      104 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ds.get_duplicate_cols.rst
--rw-rw-r--   0 root         (0) root         (0)      113 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ds.get_duplicate_indices.rst
--rw-rw-r--   0 root         (0) root         (0)       71 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ds.k_split.rst
--rw-rw-r--   0 root         (0) root         (0)       62 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ds.lfit.rst
--rw-rw-r--   0 root         (0) root         (0)       59 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ds.mae.rst
--rw-rw-r--   0 root         (0) root         (0)       83 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ds.mahalanobis.rst
--rw-rw-r--   0 root         (0) root         (0)       65 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ds.medae.rst
--rw-rw-r--   0 root         (0) root         (0)       83 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ds.optimize_pd.rst
--rw-rw-r--   0 root         (0) root         (0)       92 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ds.outlier_to_nan.rst
--rw-rw-r--   0 root         (0) root         (0)       89 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ds.pass_by_group.rst
--rw-rw-r--   0 root         (0) root         (0)       56 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ds.qf.rst
--rw-rw-r--   0 root         (0) root         (0)       92 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ds.quantile_split.rst
--rw-rw-r--   0 root         (0) root         (0)       56 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ds.r2.rst
--rw-rw-r--   0 root         (0) root         (0)       71 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ds.rel_acc.rst
--rw-rw-r--   0 root         (0) root         (0)      122 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ds.remove_unused_categories.rst
--rw-rw-r--   0 root         (0) root         (0)       62 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ds.rmsd.rst
--rw-rw-r--   0 root         (0) root         (0)       62 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ds.rmse.rst
--rw-rw-r--   0 root         (0) root         (0)       65 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ds.stdae.rst
--rw-rw-r--   0 root         (0) root         (0)       65 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ds.top_n.rst
--rw-rw-r--   0 root         (0) root         (0)       86 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ds.top_n_coding.rst
--rw-rw-r--   0 root         (0) root         (0)       85 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ipython.display_df.rst
--rw-rw-r--   0 root         (0) root         (0)       91 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ipython.display_full.rst
--rw-rw-r--   0 root         (0) root         (0)       82 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ipython.hide_code.rst
--rw-rw-r--   0 root         (0) root         (0)       94 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ipython.highlight_max.rst
--rw-rw-r--   0 root         (0) root         (0)      106 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ipython.highlight_max_min.rst
--rw-rw-r--   0 root         (0) root         (0)       94 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ipython.highlight_min.rst
--rw-rw-r--   0 root         (0) root         (0)       85 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ipython.pd_display.rst
--rw-rw-r--   0 root         (0) root         (0)       94 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.ipython.wide_notebook.rst
--rw-rw-r--   0 root         (0) root         (0)      553 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.main.BaseClass.rst
--rw-rw-r--   0 root         (0) root         (0)      109 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.main.append_to_dict_list.rst
--rw-rw-r--   0 root         (0) root         (0)       85 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.main.ceil_signif.rst
--rw-rw-r--   0 root         (0) root         (0)       70 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.main.cf_vec.rst
--rw-rw-r--   0 root         (0) root         (0)       85 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.main.concat_cols.rst
--rw-rw-r--   0 root         (0) root         (0)       76 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.main.dict_inv.rst
--rw-rw-r--   0 root         (0) root         (0)       79 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.main.dict_list.rst
--rw-rw-r--   0 root         (0) root         (0)       88 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.main.elapsed_time.rst
--rw-rw-r--   0 root         (0) root         (0)      103 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.main.elapsed_time_init.rst
--rw-rw-r--   0 root         (0) root         (0)       88 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.main.floor_signif.rst
--rw-rw-r--   0 root         (0) root         (0)       82 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.main.force_list.rst
--rw-rw-r--   0 root         (0) root         (0)       88 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.main.force_scalar.rst
--rw-rw-r--   0 root         (0) root         (0)       70 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.main.fprint.rst
--rw-rw-r--   0 root         (0) root         (0)       88 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.main.get_hdf_keys.rst
--rw-rw-r--   0 root         (0) root         (0)       88 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.main.is_list_like.rst
--rw-rw-r--   0 root         (0) root         (0)       79 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.main.is_scalar.rst
--rw-rw-r--   0 root         (0) root         (0)       88 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.main.list_exclude.rst
--rw-rw-r--   0 root         (0) root         (0)       88 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.main.list_flatten.rst
--rw-rw-r--   0 root         (0) root         (0)      103 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.main.list_intersection.rst
--rw-rw-r--   0 root         (0) root         (0)       82 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.main.list_merge.rst
--rw-rw-r--   0 root         (0) root         (0)       85 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.main.list_unique.rst
--rw-rw-r--   0 root         (0) root         (0)       79 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.main.mem_usage.rst
--rw-rw-r--   0 root         (0) root         (0)       85 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.main.progressbar.rst
--rw-rw-r--   0 root         (0) root         (0)       73 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.main.qformat.rst
--rw-rw-r--   0 root         (0) root         (0)       64 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.main.rand.rst
--rw-rw-r--   0 root         (0) root         (0)       76 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.main.read_hdf.rst
--rw-rw-r--   0 root         (0) root         (0)       97 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.main.reformat_string.rst
--rw-rw-r--   0 root         (0) root         (0)       94 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.main.remaining_time.rst
--rw-rw-r--   0 root         (0) root         (0)       88 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.main.round_signif.rst
--rw-rw-r--   0 root         (0) root         (0)       94 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.main.round_signif_i.rst
--rw-rw-r--   0 root         (0) root         (0)       79 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.main.rounddown.rst
--rw-rw-r--   0 root         (0) root         (0)       73 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.main.roundup.rst
--rw-rw-r--   0 root         (0) root         (0)       64 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.main.size.rst
--rw-rw-r--   0 root         (0) root         (0)       85 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.main.time_to_str.rst
--rw-rw-r--   0 root         (0) root         (0)       70 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.main.to_hdf.rst
--rw-rw-r--   0 root         (0) root         (0)       67 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.main.today.rst
--rw-rw-r--   0 root         (0) root         (0)       82 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.main.total_time.rst
--rw-rw-r--   0 root         (0) root         (0)       70 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.main.tprint.rst
--rw-rw-r--   0 root         (0) root         (0)      272 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.modelling.Model.rst
--rw-rw-r--   0 root         (0) root         (0)      530 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.modelling.Models.rst
--rw-rw-r--   0 root         (0) root         (0)       96 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.modelling.dict_to_model.rst
--rw-rw-r--   0 root         (0) root         (0)       90 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.modelling.force_model.rst
--rw-rw-r--   0 root         (0) root         (0)       84 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.modelling.get_coefs.rst
--rw-rw-r--   0 root         (0) root         (0)      123 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.modelling.get_feature_importance.rst
--rw-rw-r--   0 root         (0) root         (0)       80 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.plotting.animplot.rst
--rw-rw-r--   0 root         (0) root         (0)      104 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.plotting.annotate_barplot.rst
--rw-rw-r--   0 root         (0) root         (0)       89 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.plotting.ax_as_array.rst
--rw-rw-r--   0 root         (0) root         (0)       86 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.plotting.ax_as_list.rst
--rw-rw-r--   0 root         (0) root         (0)      110 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.plotting.ax_tick_linebreaks.rst
--rw-rw-r--   0 root         (0) root         (0)       89 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.plotting.barplot_err.rst
--rw-rw-r--   0 root         (0) root         (0)       80 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.plotting.corrplot.rst
--rw-rw-r--   0 root         (0) root         (0)       92 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.plotting.corrplot_bar.rst
--rw-rw-r--   0 root         (0) root         (0)       83 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.plotting.countplot.rst
--rw-rw-r--   0 root         (0) root         (0)       95 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.plotting.custom_legend.rst
--rw-rw-r--   0 root         (0) root         (0)       80 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.plotting.distplot.rst
--rw-rw-r--   0 root         (0) root         (0)       86 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.plotting.facet_wrap.rst
--rw-rw-r--   0 root         (0) root         (0)       83 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.plotting.get_axlim.rst
--rw-rw-r--   0 root         (0) root         (0)       89 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.plotting.get_legends.rst
--rw-rw-r--   0 root         (0) root         (0)       83 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.plotting.get_subax.rst
--rw-rw-r--   0 root         (0) root         (0)       80 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.plotting.get_twin.rst
--rw-rw-r--   0 root         (0) root         (0)       77 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.plotting.heatmap.rst
--rw-rw-r--   0 root         (0) root         (0)       77 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.plotting.hist_2d.rst
--rw-rw-r--   0 root         (0) root         (0)      104 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.plotting.insert_linebreak.rst
--rw-rw-r--   0 root         (0) root         (0)       98 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.plotting.legend_outside.rst
--rw-rw-r--   0 root         (0) root         (0)       83 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.plotting.levelplot.rst
--rw-rw-r--   0 root         (0) root         (0)       89 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.plotting.paired_plot.rst
--rw-rw-r--   0 root         (0) root         (0)      107 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.plotting.pairwise_corrplot.rst
--rw-rw-r--   0 root         (0) root         (0)       74 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.plotting.q_plim.rst
--rw-rw-r--   0 root         (0) root         (0)       95 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.plotting.quantile_plot.rst
--rw-rw-r--   0 root         (0) root         (0)       80 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.plotting.rmsdplot.rst
--rw-rw-r--   0 root         (0) root         (0)       86 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.plotting.set_ax_sym.rst
--rw-rw-r--   0 root         (0) root         (0)       83 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.plotting.set_axlim.rst
--rw-rw-r--   0 root         (0) root         (0)       92 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.plotting.share_legend.rst
--rw-rw-r--   0 root         (0) root         (0)       80 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.plotting.share_xy.rst
--rw-rw-r--   0 root         (0) root         (0)       80 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/api/hhpy.plotting.stemplot.rst
--rw-rw-r--   0 root         (0) root         (0)      127 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/build.sh
--rw-rw-r--   0 root         (0) root         (0)     2560 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/conf.py
--rw-rw-r--   0 root         (0) root         (0)      450 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/index.rst
--rw-rw-r--   0 root         (0) root         (0)      795 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/make.bat
--rw-rw-r--   0 root         (0) root         (0)      183 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/modules.rst
--rw-rw-r--   0 root         (0) root         (0)      583 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/quickstart.rst
--rw-rw-r--   0 root         (0) root         (0)      114 2021-06-23 04:28:10.000000 hhpy-0.3.0/sphinx/requires.txt
-drwxrwxr-x   0 root         (0) root         (0)        0 2021-06-23 04:28:10.000000 hhpy-0.3.0/tests/
--rwxrwxr-x   0 root         (0) root         (0)       67 2021-06-23 04:28:10.000000 hhpy-0.3.0/tests/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     1216 2021-06-23 04:28:10.000000 hhpy-0.3.0/tests/conftest.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2021-06-23 04:28:10.000000 hhpy-0.3.0/tests/files/
--rw-rw-r--   0 root         (0) root         (0)     8918 2021-06-23 04:28:10.000000 hhpy-0.3.0/tests/files/testdata_jp.xlsx
--rw-rw-r--   0 root         (0) root         (0)     5980 2021-06-23 04:28:10.000000 hhpy-0.3.0/tests/files/testdata_jp_dfmapping.xlsx
--rw-rw-r--   0 root         (0) root         (0)     1017 2021-06-23 04:28:10.000000 hhpy-0.3.0/tests/test_ds.py
--rw-rw-r--   0 root         (0) root         (0)       20 2021-06-23 04:28:10.000000 hhpy-0.3.0/to_pypi.sh
+drwxr-xr-x   0 henrik     (501) staff       (20)        0 2023-06-05 12:50:07.384657 hhpy-0.3.1/
+drwxr-xr-x   0 henrik     (501) staff       (20)        0 2023-06-05 12:50:07.168739 hhpy-0.3.1/.github/
+drwxr-xr-x   0 henrik     (501) staff       (20)        0 2023-06-05 12:50:07.183127 hhpy-0.3.1/.github/workflows/
+-rw-r--r--   0 henrik     (501) staff       (20)     1060 2021-12-09 14:17:17.000000 hhpy-0.3.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 henrik     (501) staff       (20)     2822 2023-06-05 08:18:51.000000 hhpy-0.3.1/.gitignore
+drwxr-xr-x   0 henrik     (501) staff       (20)        0 2023-06-05 12:50:07.189539 hhpy-0.3.1/.idea/
+-rw-r--r--   0 henrik     (501) staff       (20)       38 2021-12-09 14:17:17.000000 hhpy-0.3.1/.idea/.gitignore
+drwxr-xr-x   0 henrik     (501) staff       (20)        0 2023-06-05 12:50:07.190670 hhpy-0.3.1/.idea/dictionaries/
+-rw-r--r--   0 henrik     (501) staff       (20)     4875 2021-12-09 14:17:17.000000 hhpy-0.3.1/.idea/dictionaries/hanssen_henrik.xml
+-rw-r--r--   0 henrik     (501) staff       (20)      547 2023-06-05 07:52:34.000000 hhpy-0.3.1/.idea/hhpy.iml
+drwxr-xr-x   0 henrik     (501) staff       (20)        0 2023-06-05 12:50:07.192474 hhpy-0.3.1/.idea/inspectionProfiles/
+-rw-r--r--   0 henrik     (501) staff       (20)      228 2021-12-09 14:17:17.000000 hhpy-0.3.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 henrik     (501) staff       (20)      192 2023-06-05 07:52:34.000000 hhpy-0.3.1/.idea/misc.xml
+-rw-r--r--   0 henrik     (501) staff       (20)      260 2021-12-09 14:17:17.000000 hhpy-0.3.1/.idea/modules.xml
+-rw-r--r--   0 henrik     (501) staff       (20)      180 2021-12-09 14:17:17.000000 hhpy-0.3.1/.idea/vcs.xml
+-rwxr-xr-x   0 henrik     (501) staff       (20)      551 2021-12-09 14:17:17.000000 hhpy-0.3.1/LICENSE.txt
+-rw-r--r--   0 henrik     (501) staff       (20)     1313 2023-06-05 12:50:07.384903 hhpy-0.3.1/PKG-INFO
+-rwxr-xr-x   0 henrik     (501) staff       (20)      266 2021-12-09 14:17:17.000000 hhpy-0.3.1/Pipfile
+-rw-r--r--   0 henrik     (501) staff       (20)    33024 2023-06-05 08:18:51.000000 hhpy-0.3.1/Pipfile.lock
+-rwxr-xr-x   0 henrik     (501) staff       (20)      768 2021-12-09 14:17:17.000000 hhpy-0.3.1/README.md
+-rw-r--r--   0 henrik     (501) staff       (20)       26 2021-12-09 14:17:17.000000 hhpy-0.3.1/_config.yml
+drwxr-xr-x   0 henrik     (501) staff       (20)        0 2023-06-05 12:50:07.210995 hhpy-0.3.1/hhpy/
+-rw-r--r--   0 henrik     (501) staff       (20)     6148 2023-06-05 08:24:58.000000 hhpy-0.3.1/hhpy/.DS_Store
+-rwxr-xr-x   0 henrik     (501) staff       (20)      169 2023-06-05 08:00:47.000000 hhpy-0.3.1/hhpy/__init__.py
+-rw-r--r--   0 henrik     (501) staff       (20)      287 2021-12-09 14:17:17.000000 hhpy-0.3.1/hhpy/__init__.pyc
+-rwxr-xr-x   0 henrik     (501) staff       (20)      434 2023-06-05 07:53:36.000000 hhpy-0.3.1/hhpy/__version__.py
+-rw-r--r--   0 henrik     (501) staff       (20)   108757 2023-06-05 08:17:49.000000 hhpy-0.3.1/hhpy/ds.py
+-rwxr-xr-x   0 henrik     (501) staff       (20)     1534 2021-12-09 14:17:17.000000 hhpy-0.3.1/hhpy/entry_points.py
+-rw-r--r--   0 henrik     (501) staff       (20)     5682 2023-06-05 08:16:47.000000 hhpy-0.3.1/hhpy/ipython.py
+-rwxr-xr-x   0 henrik     (501) staff       (20)    52515 2023-06-05 08:15:57.000000 hhpy-0.3.1/hhpy/main.py
+-rw-r--r--   0 henrik     (501) staff       (20)    70940 2023-06-05 08:15:39.000000 hhpy-0.3.1/hhpy/modelling.py
+-rw-r--r--   0 henrik     (501) staff       (20)   134692 2023-06-05 08:15:07.000000 hhpy-0.3.1/hhpy/plotting.py
+-rw-r--r--   0 henrik     (501) staff       (20)     4073 2023-06-05 07:59:10.000000 hhpy-0.3.1/hhpy/regression.py
+drwxr-xr-x   0 henrik     (501) staff       (20)        0 2023-06-05 12:50:07.216538 hhpy-0.3.1/hhpy.egg-info/
+-rw-r--r--   0 henrik     (501) staff       (20)     1313 2023-06-05 12:50:07.000000 hhpy-0.3.1/hhpy.egg-info/PKG-INFO
+-rw-r--r--   0 henrik     (501) staff       (20)     5501 2023-06-05 12:50:07.000000 hhpy-0.3.1/hhpy.egg-info/SOURCES.txt
+-rw-r--r--   0 henrik     (501) staff       (20)        1 2023-06-05 12:50:07.000000 hhpy-0.3.1/hhpy.egg-info/dependency_links.txt
+-rw-r--r--   0 henrik     (501) staff       (20)       48 2023-06-05 12:50:07.000000 hhpy-0.3.1/hhpy.egg-info/entry_points.txt
+-rw-r--r--   0 henrik     (501) staff       (20)        1 2021-12-09 14:17:17.000000 hhpy-0.3.1/hhpy.egg-info/not-zip-safe
+-rw-r--r--   0 henrik     (501) staff       (20)      108 2023-06-05 12:50:07.000000 hhpy-0.3.1/hhpy.egg-info/requires.txt
+-rw-r--r--   0 henrik     (501) staff       (20)        5 2023-06-05 12:50:07.000000 hhpy-0.3.1/hhpy.egg-info/top_level.txt
+-rw-r--r--   0 henrik     (501) staff       (20)      498 2023-06-05 10:01:43.000000 hhpy-0.3.1/pyproject.toml
+-rw-r--r--   0 henrik     (501) staff       (20)     3482 2021-12-09 14:17:17.000000 hhpy-0.3.1/release_notes.md
+-rw-r--r--   0 henrik     (501) staff       (20)       79 2023-06-05 12:50:07.385913 hhpy-0.3.1/setup.cfg
+-rwxr-xr-x   0 henrik     (501) staff       (20)     1435 2023-06-05 07:53:03.000000 hhpy-0.3.1/setup.py
+drwxr-xr-x   0 henrik     (501) staff       (20)        0 2023-06-05 12:50:07.228277 hhpy-0.3.1/sphinx/
+-rw-r--r--   0 henrik     (501) staff       (20)     8196 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/.DS_Store
+-rw-r--r--   0 henrik     (501) staff       (20)      634 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/Makefile
+drwxr-xr-x   0 henrik     (501) staff       (20)        0 2023-06-05 12:50:07.229217 hhpy-0.3.1/sphinx/_static/
+-rw-r--r--   0 henrik     (501) staff       (20)     6148 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/_static/.DS_Store
+drwxr-xr-x   0 henrik     (501) staff       (20)        0 2023-06-05 12:50:07.379670 hhpy-0.3.1/sphinx/api/
+-rw-r--r--   0 henrik     (501) staff       (20)    16388 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/.DS_Store
+-rw-r--r--   0 henrik     (501) staff       (20)      589 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ds.DFMapping.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       59 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ds.acc.rst
+-rw-r--r--   0 henrik     (501) staff       (20)      104 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ds.butter_pass_filter.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       83 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ds.change_span.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       56 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ds.cm.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       86 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ds.col_to_front.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       62 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ds.corr.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       74 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ds.df_count.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       62 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ds.df_p.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       71 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ds.df_rmsd.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       74 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ds.df_score.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       74 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ds.df_split.rst
+-rw-r--r--   0 henrik     (501) staff       (20)      107 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ds.drop_duplicate_cols.rst
+-rw-r--r--   0 henrik     (501) staff       (20)      116 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ds.drop_duplicate_indices.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       92 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ds.drop_zero_cols.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       65 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ds.f1_pr.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       71 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ds.f_score.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       83 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ds.get_df_corr.rst
+-rw-r--r--   0 henrik     (501) staff       (20)      104 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ds.get_duplicate_cols.rst
+-rw-r--r--   0 henrik     (501) staff       (20)      113 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ds.get_duplicate_indices.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       71 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ds.k_split.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       62 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ds.lfit.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       59 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ds.mae.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       83 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ds.mahalanobis.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       65 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ds.medae.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       83 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ds.optimize_pd.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       92 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ds.outlier_to_nan.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       89 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ds.pass_by_group.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       56 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ds.qf.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       92 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ds.quantile_split.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       56 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ds.r2.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       71 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ds.rel_acc.rst
+-rw-r--r--   0 henrik     (501) staff       (20)      122 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ds.remove_unused_categories.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       62 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ds.rmsd.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       62 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ds.rmse.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       65 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ds.stdae.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       65 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ds.top_n.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       86 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ds.top_n_coding.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       85 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ipython.display_df.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       91 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ipython.display_full.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       82 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ipython.hide_code.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       94 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ipython.highlight_max.rst
+-rw-r--r--   0 henrik     (501) staff       (20)      106 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ipython.highlight_max_min.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       94 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ipython.highlight_min.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       85 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ipython.pd_display.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       94 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.ipython.wide_notebook.rst
+-rw-r--r--   0 henrik     (501) staff       (20)      553 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.main.BaseClass.rst
+-rw-r--r--   0 henrik     (501) staff       (20)      109 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.main.append_to_dict_list.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       85 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.main.ceil_signif.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       70 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.main.cf_vec.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       85 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.main.concat_cols.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       76 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.main.dict_inv.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       79 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.main.dict_list.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       88 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.main.elapsed_time.rst
+-rw-r--r--   0 henrik     (501) staff       (20)      103 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.main.elapsed_time_init.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       88 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.main.floor_signif.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       82 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.main.force_list.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       88 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.main.force_scalar.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       70 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.main.fprint.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       88 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.main.get_hdf_keys.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       88 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.main.is_list_like.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       79 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.main.is_scalar.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       88 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.main.list_exclude.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       88 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.main.list_flatten.rst
+-rw-r--r--   0 henrik     (501) staff       (20)      103 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.main.list_intersection.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       82 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.main.list_merge.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       85 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.main.list_unique.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       79 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.main.mem_usage.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       85 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.main.progressbar.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       73 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.main.qformat.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       64 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.main.rand.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       76 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.main.read_hdf.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       97 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.main.reformat_string.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       94 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.main.remaining_time.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       88 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.main.round_signif.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       94 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.main.round_signif_i.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       79 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.main.rounddown.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       73 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.main.roundup.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       64 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.main.size.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       85 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.main.time_to_str.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       70 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.main.to_hdf.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       67 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.main.today.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       82 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.main.total_time.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       70 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.main.tprint.rst
+-rw-r--r--   0 henrik     (501) staff       (20)      272 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.modelling.Model.rst
+-rw-r--r--   0 henrik     (501) staff       (20)      530 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.modelling.Models.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       96 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.modelling.dict_to_model.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       90 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.modelling.force_model.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       84 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.modelling.get_coefs.rst
+-rw-r--r--   0 henrik     (501) staff       (20)      123 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.modelling.get_feature_importance.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       80 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.plotting.animplot.rst
+-rw-r--r--   0 henrik     (501) staff       (20)      104 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.plotting.annotate_barplot.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       89 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.plotting.ax_as_array.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       86 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.plotting.ax_as_list.rst
+-rw-r--r--   0 henrik     (501) staff       (20)      110 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.plotting.ax_tick_linebreaks.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       89 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.plotting.barplot_err.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       80 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.plotting.corrplot.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       92 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.plotting.corrplot_bar.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       83 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.plotting.countplot.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       95 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.plotting.custom_legend.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       80 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.plotting.distplot.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       86 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.plotting.facet_wrap.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       83 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.plotting.get_axlim.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       89 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.plotting.get_legends.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       83 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.plotting.get_subax.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       80 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.plotting.get_twin.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       77 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.plotting.heatmap.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       77 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.plotting.hist_2d.rst
+-rw-r--r--   0 henrik     (501) staff       (20)      104 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.plotting.insert_linebreak.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       98 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.plotting.legend_outside.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       83 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.plotting.levelplot.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       89 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.plotting.paired_plot.rst
+-rw-r--r--   0 henrik     (501) staff       (20)      107 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.plotting.pairwise_corrplot.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       74 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.plotting.q_plim.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       95 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.plotting.quantile_plot.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       80 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.plotting.rmsdplot.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       86 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.plotting.set_ax_sym.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       83 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.plotting.set_axlim.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       92 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.plotting.share_legend.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       80 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.plotting.share_xy.rst
+-rw-r--r--   0 henrik     (501) staff       (20)       80 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/api/hhpy.plotting.stemplot.rst
+-rw-r--r--   0 henrik     (501) staff       (20)      127 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/build.sh
+-rw-r--r--   0 henrik     (501) staff       (20)     2560 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/conf.py
+-rw-r--r--   0 henrik     (501) staff       (20)      450 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/index.rst
+-rw-r--r--   0 henrik     (501) staff       (20)      795 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/make.bat
+-rw-r--r--   0 henrik     (501) staff       (20)      183 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/modules.rst
+-rw-r--r--   0 henrik     (501) staff       (20)      583 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/quickstart.rst
+-rw-r--r--   0 henrik     (501) staff       (20)      114 2021-12-09 14:17:17.000000 hhpy-0.3.1/sphinx/requires.txt
+drwxr-xr-x   0 henrik     (501) staff       (20)        0 2023-06-05 12:50:07.381430 hhpy-0.3.1/tests/
+-rwxr-xr-x   0 henrik     (501) staff       (20)       54 2023-06-05 08:08:57.000000 hhpy-0.3.1/tests/__init__.py
+drwxr-xr-x   0 henrik     (501) staff       (20)        0 2023-06-05 12:50:07.383778 hhpy-0.3.1/tests/files/
+-rw-r--r--   0 henrik     (501) staff       (20)     8918 2021-12-09 14:17:17.000000 hhpy-0.3.1/tests/files/testdata_jp.xlsx
+-rw-r--r--   0 henrik     (501) staff       (20)     5980 2021-12-09 14:17:17.000000 hhpy-0.3.1/tests/files/testdata_jp_dfmapping.xlsx
+-rw-r--r--   0 henrik     (501) staff       (20)      993 2023-06-05 08:08:25.000000 hhpy-0.3.1/tests/test_ds.py
+-rw-r--r--   0 henrik     (501) staff       (20)       79 2023-06-05 12:48:54.000000 hhpy-0.3.1/to_pypi.sh
```

### Comparing `hhpy-0.3.0/.idea/dictionaries/hanssen_henrik.xml` & `hhpy-0.3.1/.idea/dictionaries/hanssen_henrik.xml`

 * *Files identical despite different names*

### Comparing `hhpy-0.3.0/.idea/hhpy.iml` & `hhpy-0.3.1/.idea/hhpy.iml`

 * *Files 1% similar despite different names*

#### Comparing `hhpy-0.3.0/.idea/hhpy.iml` & `hhpy-0.3.1/.idea/hhpy.iml`

```diff
@@ -1,12 +1,12 @@
 <?xml version="1.0" encoding="utf-8"?>
 <module type="PYTHON_MODULE" version="4">
   <component name="NewModuleRootManager">
     <content url="file://$MODULE_DIR$"/>
-    <orderEntry type="jdk" jdkName="Python 3.8 (hhpy)" jdkType="Python SDK"/>
+    <orderEntry type="jdk" jdkName="Python 3.9 (hhpy)" jdkType="Python SDK"/>
     <orderEntry type="sourceFolder" forTests="false"/>
   </component>
   <component name="PackageRequirementsSettings">
     <option name="requirementsPath" value=""/>
   </component>
   <component name="TestRunnerService">
     <option name="PROJECT_TEST_RUNNER" value="pytest"/>
```

### Comparing `hhpy-0.3.0/LICENSE.txt` & `hhpy-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hhpy-0.3.0/Pipfile.lock` & `hhpy-0.3.1/Pipfile.lock`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9031361082444674%*

 * *Differences: {"'default'": "{'bleach': {'hashes': "*

 * *              "['sha256:0900d8b37eba61a802ee40ac0061f8c2b5dee29c1927dd1d233e075ebf5a71da', "*

 * *              "'sha256:4d2651ab93271d1129ac9cbc679f524565cc8a1b791909c4a51eac4446a15994'], "*

 * *              '\'version\': \'==4.1.0\', \'markers\': "python_version >= \'3.6\'", delete: '*

 * *              "['index']}, 'certifi': {'hashes': "*

 * *              "['sha256:78884e7c1d4b00ce3cea67b44566851c4343c120abd683433ce934a68ea58872', "*

 * *              "'sha256:d62a0163eb4c2344ac042ab2bdf […]*

```diff
@@ -14,40 +14,41 @@
                 "verify_ssl": true
             }
         ]
     },
     "default": {
         "bleach": {
             "hashes": [
-                "sha256:cc8da25076a1fe56c3ac63671e2194458e0c4d9c7becfd52ca251650d517903c",
-                "sha256:e78e426105ac07026ba098f04de8abe9b6e3e98b5befbf89b51a5ef0a4292b03"
+                "sha256:0900d8b37eba61a802ee40ac0061f8c2b5dee29c1927dd1d233e075ebf5a71da",
+                "sha256:4d2651ab93271d1129ac9cbc679f524565cc8a1b791909c4a51eac4446a15994"
             ],
-            "index": "pypi",
-            "version": "==3.1.4"
+            "markers": "python_version >= '3.6'",
+            "version": "==4.1.0"
         },
         "certifi": {
             "hashes": [
-                "sha256:017c25db2a153ce562900032d5bc68e9f191e44e9a0f762f373977de9df1fbb3",
-                "sha256:25b64c7da4cd7479594d035c08c2d809eb4aab3a26e5a990ea98cc450c320f1f"
+                "sha256:78884e7c1d4b00ce3cea67b44566851c4343c120abd683433ce934a68ea58872",
+                "sha256:d62a0163eb4c2344ac042ab2bdf75399a71a2d8c7d47eac2e2ee91b9d6339569"
             ],
-            "version": "==2019.11.28"
+            "version": "==2021.10.8"
         },
         "chardet": {
             "hashes": [
                 "sha256:84ab92ed1c4d4f16916e05906b6b75a6c0fb5db821cc65e70cbd64a3e2a5eaae",
                 "sha256:fc323ffcaeaed0e0a02bf4d117757b98aed530d9ed4531e3e15460124c106691"
             ],
             "version": "==3.0.4"
         },
         "docutils": {
             "hashes": [
-                "sha256:0c5b78adfbf7762415433f5515cd5c9e762339e23369dbe8000d84a4bf4ab3af",
-                "sha256:c2de3a60e9e7d07be26b7f2b00ca0309c207e06c100f9cc2a94931fc75a478fc"
+                "sha256:23010f129180089fbcd3bc08cfefccb3b890b0050e1ca00c867036e9d161b98c",
+                "sha256:679987caf361a7539d76e584cbeddc311e3aee937877c87346f31debc63e9d06"
             ],
-            "version": "==0.16"
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
+            "version": "==0.18.1"
         },
         "idna": {
             "hashes": [
                 "sha256:156a6814fb5ac1fc6850fb002e0852d56c0c8d2531923a51032d1b70760e186e",
                 "sha256:684a38a6f903c1d71d6d5fac066b58d7768af4de2b832e426ec79c30daa94a16"
             ],
             "version": "==2.7"
@@ -82,34 +83,51 @@
                 "sha256:df04f4bad8a359daa2ff74f8108ea051670cafbca533bb2636c58b16e962989e",
                 "sha256:ecf81720934a0e18526177e645cbd6a8a21bb0ddc887ff9738de07a1df5c6b61",
                 "sha256:edfa6fba9157e0e3be0f40168eb142511012683ac3dc82420bee4a3f3981b30e"
             ],
             "index": "pypi",
             "version": "==1.15.4"
         },
+        "packaging": {
+            "hashes": [
+                "sha256:dd47c42927d89ab911e606518907cc2d3a1f38bbd026385970643f9c5b8ecfeb",
+                "sha256:ef103e05f519cdc783ae24ea4e2e0f508a9c99b2d4969652eed6a2e1ea5bd522"
+            ],
+            "markers": "python_version >= '3.6'",
+            "version": "==21.3"
+        },
         "pkginfo": {
             "hashes": [
-                "sha256:7424f2c8511c186cd5424bbf31045b77435b37a8d604990b79d4e70d741148bb",
-                "sha256:a6d9e40ca61ad3ebd0b72fbadd4fba16e4c0e4df0428c041e01e06eb6ee71f32"
+                "sha256:542e0d0b6750e2e21c20179803e40ab50598d8066d51097a0e382cba9eb02bff",
+                "sha256:c24c487c6a7f72c66e816ab1796b96ac6c3d14d49338293d2141664330b55ffc"
             ],
-            "version": "==1.5.0.1"
+            "version": "==1.8.2"
         },
         "pygments": {
             "hashes": [
-                "sha256:647344a061c249a3b74e230c739f434d7ea4d8b1d5f3721bc0f3558049b38f44",
-                "sha256:ff7a40b4860b727ab48fad6360eb351cc1b33cbf9b15a0f689ca5353e9463324"
+                "sha256:b8e67fe6af78f492b3c4b3e2970c0624cbf08beb1e493b2c99b9fa1b67a20380",
+                "sha256:f398865f7eb6874156579fdf36bc840a03cab64d1cde9e93d68f46a425ec52c6"
             ],
-            "version": "==2.6.1"
+            "markers": "python_version >= '3.5'",
+            "version": "==2.10.0"
+        },
+        "pyparsing": {
+            "hashes": [
+                "sha256:04ff808a5b90911829c55c4e26f75fa5ca8a2f5f36aa3a51f68e27033341d3e4",
+                "sha256:d9bdec0013ef1eb5a84ab39a3b3868911598afa494f5faa038647101504e2b81"
+            ],
+            "markers": "python_version >= '3.6'",
+            "version": "==3.0.6"
         },
         "readme-renderer": {
             "hashes": [
-                "sha256:1b6d8dd1673a0b293766b4106af766b6eff3654605f9c4f239e65de6076bc222",
-                "sha256:e67d64242f0174a63c3b727801a2fff4c1f38ebe5d71d95ff7ece081945a6cd4"
+                "sha256:3286806450d9961d6e3b5f8a59f77e61503799aca5155c8d8d40359b4e1e1adc",
+                "sha256:8299700d7a910c304072a7601eafada6712a5b011a20139417e1b1e9f04645d8"
             ],
-            "version": "==25.0"
+            "version": "==30.0"
         },
         "requests": {
             "hashes": [
                 "sha256:65b3a120e4329e33c9889db89c80976c5272f56ea92d3e74da8a463992e3ff54",
                 "sha256:ea881206e59f41dbd0bd445437d792e43906703fff75ca8ff43ccdb11f33f263"
             ],
             "index": "pypi",
@@ -118,41 +136,52 @@
         "requests-toolbelt": {
             "hashes": [
                 "sha256:380606e1d10dc85c3bd47bf5a6095f815ec007be7a8b69c878507068df059e6f",
                 "sha256:968089d4584ad4ad7c171454f0a5c6dac23971e9472521ea3b6d49d610aa6fc0"
             ],
             "version": "==0.9.1"
         },
+        "setuptools": {
+            "hashes": [
+                "sha256:6d10741ff20b89cd8c6a536ee9dc90d3002dec0226c78fb98605bfb9ef8a7adf",
+                "sha256:d144f85102f999444d06f9c0e8c737fd0194f10f2f7e5fdb77573f6e2fa4fad0"
+            ],
+            "markers": "python_version >= '3.6'",
+            "version": "==59.5.0"
+        },
         "six": {
             "hashes": [
-                "sha256:236bdbdce46e6e6a3d61a337c0f8b763ca1e8717c03b369e87a7ec7ce1319c0a",
-                "sha256:8f3cd2e254d8f793e7f3d6d9df77b92252b52637291d0f0da013c76ea2724b6c"
+                "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
+                "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
-            "version": "==1.14.0"
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
+            "version": "==1.16.0"
         },
         "tqdm": {
             "hashes": [
-                "sha256:03d2366c64d44c7f61e74c700d9b202d57e9efe355ea5c28814c52bfe7a50b8c",
-                "sha256:be5ddeec77d78ba781ea41eacb2358a77f74cc2407f54b82222d7ee7dc8c8ccf"
+                "sha256:8dd278a422499cd6b727e6ae4061c40b48fce8b76d1ccbf5d34fca9b7f925b0c",
+                "sha256:d359de7217506c9851b7869f3708d8ee53ed70a1b8edbba4dbcb47442592920d"
             ],
-            "version": "==4.44.1"
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
+            "version": "==4.62.3"
         },
         "twine": {
             "hashes": [
                 "sha256:7d89bc6acafb31d124e6e5b295ef26ac77030bf098960c2a4c4e058335827c5c",
                 "sha256:fad6f1251195f7ddd1460cb76d6ea106c93adb4e56c41e0da79658e56e547d2c"
             ],
             "index": "pypi",
             "version": "==1.12.1"
         },
         "urllib3": {
             "hashes": [
                 "sha256:2393a695cd12afedd0dcb26fe5d50d0cf248e5a66f75dbd89a3d4eb333a61af4",
                 "sha256:a637e5fae88995b256e3409dc4d52c2e2e0ba32c42a6365fee8bbd2238de3cfb"
             ],
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3' and python_version < '4'",
             "version": "==1.24.3"
         },
         "webencodings": {
             "hashes": [
                 "sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78",
                 "sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923"
             ],
@@ -165,67 +194,73 @@
                 "sha256:446438bdcca0e05bd45ea2de1668c1d9b032e1a9154c2c259092d77031ddd359",
                 "sha256:a661d72d58e6ea8a57f7a86e37d86716863ee5e92788398526d58b26a4e4dc02"
             ],
             "version": "==0.7.12"
         },
         "atomicwrites": {
             "hashes": [
-                "sha256:03472c30eb2c5d1ba9227e4c2ca66ab8287fbfbbda3888aa93dc2e28fc6811b4",
-                "sha256:75a9445bac02d8d058d5e1fe689654ba5a6556a1dfd8ce6ec55a0ed79866cfa6"
+                "sha256:6d1784dea7c0c8d4a5172b6c620f40b6e4cbfdf96d783691f2e1302a7b88e197",
+                "sha256:ae70396ad1a434f9c7046fd2dd196fc04b12f9e91ffb859164193be8b6168a7a"
             ],
-            "version": "==1.3.0"
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
+            "version": "==1.4.0"
         },
         "attrs": {
             "hashes": [
-                "sha256:08a96c641c3a74e44eb59afb61a24f2cb9f4d7188748e76ba4bb5edfa3cb7d1c",
-                "sha256:f7b7ce16570fe9965acd6d30101a28f62fb4a7f9e926b3bbc9b61f8b04247e72"
+                "sha256:149e90d6d8ac20db7a955ad60cf0e6881a3f20d37096140088356da6c716b0b1",
+                "sha256:ef6aaac3ca6cd92904cdd0d83f629a15f18053ec84e6432106f7a4d04ae4f5fb"
             ],
-            "version": "==19.3.0"
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
+            "version": "==21.2.0"
         },
         "babel": {
             "hashes": [
-                "sha256:1aac2ae2d0d8ea368fa90906567f5c08463d98ade155c0c4bfedd6a0f7160e38",
-                "sha256:d670ea0b10f8b723672d3a6abeb87b565b244da220d76b4dba1b66269ec152d4"
+                "sha256:ab49e12b91d937cd11f0b67cb259a57ab4ad2b59ac7a3b41d6c06c0ac5b0def9",
+                "sha256:bc0c176f9f6a994582230df350aa6e05ba2ebe4b3ac317eab29d9be5d2768da0"
             ],
-            "version": "==2.8.0"
+            "index": "pypi",
+            "version": "==2.9.1"
         },
         "backcall": {
             "hashes": [
-                "sha256:38ecd85be2c1e78f77fd91700c76e14667dc21e2713b63876c0eb901196e01e4",
-                "sha256:bbbf4b1e5cd2bdb08f915895b51081c041bac22394fdfcfdfbe9f14b77c08bf2"
+                "sha256:5cbdbf27be5e7cfadb448baf0aa95508f91f2bbc6c6437cd9cd06e2a4c215e1e",
+                "sha256:fbbce6a29f263178a1f7915c1940bde0ec2b2a967566fe1c65c1dfb7422bd255"
             ],
-            "version": "==0.1.0"
+            "version": "==0.2.0"
         },
         "certifi": {
             "hashes": [
-                "sha256:017c25db2a153ce562900032d5bc68e9f191e44e9a0f762f373977de9df1fbb3",
-                "sha256:25b64c7da4cd7479594d035c08c2d809eb4aab3a26e5a990ea98cc450c320f1f"
+                "sha256:78884e7c1d4b00ce3cea67b44566851c4343c120abd683433ce934a68ea58872",
+                "sha256:d62a0163eb4c2344ac042ab2bdf75399a71a2d8c7d47eac2e2ee91b9d6339569"
             ],
-            "version": "==2019.11.28"
+            "version": "==2021.10.8"
         },
-        "chardet": {
+        "charset-normalizer": {
             "hashes": [
-                "sha256:84ab92ed1c4d4f16916e05906b6b75a6c0fb5db821cc65e70cbd64a3e2a5eaae",
-                "sha256:fc323ffcaeaed0e0a02bf4d117757b98aed530d9ed4531e3e15460124c106691"
+                "sha256:1eecaa09422db5be9e29d7fc65664e6c33bd06f9ced7838578ba40d58bdf3721",
+                "sha256:b0b883e8e874edfdece9c28f314e3dd5badf067342e42fb162203335ae61aa2c"
             ],
-            "version": "==3.0.4"
+            "markers": "python_version >= '3'",
+            "version": "==2.0.9"
         },
         "decorator": {
             "hashes": [
-                "sha256:41fa54c2a0cc4ba648be4fd43cff00aedf5b9465c9bf18d64325bc225f08f760",
-                "sha256:e3a62f0520172440ca0dcc823749319382e377f37f140a0b99ef45fecb84bfe7"
+                "sha256:7b12e7c3c6ab203a29e157335e9122cb03de9ab7264b137594103fd4a683b374",
+                "sha256:e59913af105b9860aa2c8d3272d9de5a56a4e608db9a2f167a8480b323d529a7"
             ],
-            "version": "==4.4.2"
+            "markers": "python_version >= '3.5'",
+            "version": "==5.1.0"
         },
         "docutils": {
             "hashes": [
-                "sha256:0c5b78adfbf7762415433f5515cd5c9e762339e23369dbe8000d84a4bf4ab3af",
-                "sha256:c2de3a60e9e7d07be26b7f2b00ca0309c207e06c100f9cc2a94931fc75a478fc"
+                "sha256:23010f129180089fbcd3bc08cfefccb3b890b0050e1ca00c867036e9d161b98c",
+                "sha256:679987caf361a7539d76e584cbeddc311e3aee937877c87346f31debc63e9d06"
             ],
-            "version": "==0.16"
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
+            "version": "==0.18.1"
         },
         "flake8": {
             "hashes": [
                 "sha256:6a35f5b8761f45c5513e3405f110a86bea57982c3b75b766ce7b65217abe1670",
                 "sha256:c01f8a3963b3571a8e6bd7a4063359aff90749e160778e03817cd9b71c9e07d2"
             ],
             "index": "pypi",
@@ -236,107 +271,141 @@
                 "sha256:156a6814fb5ac1fc6850fb002e0852d56c0c8d2531923a51032d1b70760e186e",
                 "sha256:684a38a6f903c1d71d6d5fac066b58d7768af4de2b832e426ec79c30daa94a16"
             ],
             "version": "==2.7"
         },
         "imagesize": {
             "hashes": [
-                "sha256:6965f19a6a2039c7d48bca7dba2473069ff854c36ae6f19d2cde309d998228a1",
-                "sha256:b1f6b5a4eab1f73479a50fb79fcf729514a900c341d8503d62a62dbc4127a2b1"
+                "sha256:1db2f82529e53c3e929e8926a1fa9235aa82d0bd0c580359c67ec31b2fddaa8c",
+                "sha256:cd1750d452385ca327479d45b64d9c7729ecf0b3969a58148298c77092261f9d"
             ],
-            "version": "==1.2.0"
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
+            "version": "==1.3.0"
         },
         "importlib-metadata": {
             "hashes": [
-                "sha256:2a688cbaa90e0cc587f1df48bdc97a6eadccdcd9c35fb3f976a09e3b5016d90f",
-                "sha256:34513a8a0c4962bc66d35b359558fd8a5e10cd472d37aec5f66858addef32c1e"
+                "sha256:53ccfd5c134223e497627b9815d5030edf77d2ed573922f7a0b8f8bb81a1c100",
+                "sha256:75bdec14c397f528724c1bfd9709d660b33a4d2e77387a3358f20b848bb5e5fb"
             ],
             "markers": "python_version < '3.8'",
-            "version": "==1.6.0"
+            "version": "==4.8.2"
         },
         "ipython": {
             "hashes": [
                 "sha256:a5781d6934a3341a1f9acb4ea5acdc7ea0a0855e689dbe755d070ca51e995435",
                 "sha256:b10a7ddd03657c761fc503495bc36471c8158e3fc948573fb9fe82a7029d8efd"
             ],
             "index": "pypi",
             "version": "==7.1.1"
         },
-        "ipython-genutils": {
-            "hashes": [
-                "sha256:72dd37233799e619666c9f639a9da83c34013a73e8bbc79a7a6348d93c61fab8",
-                "sha256:eb2e116e75ecef9d4d228fdc66af54269afa26ab4463042e33785b887c628ba8"
-            ],
-            "version": "==0.2.0"
-        },
         "jedi": {
             "hashes": [
-                "sha256:b4f4052551025c6b0b0b193b29a6ff7bdb74c52450631206c262aef9f7159ad2",
-                "sha256:d5c871cb9360b414f981e7072c52c33258d598305280fef91c6cae34739d65d5"
+                "sha256:637c9635fcf47945ceb91cd7f320234a7be540ded6f3e99a50cb6febdfd1ba8d",
+                "sha256:74137626a64a99c8eb6ae5832d99b3bdd7d29a3850fe2aa80a4126b2a7d949ab"
             ],
-            "version": "==0.16.0"
+            "markers": "python_version >= '3.6'",
+            "version": "==0.18.1"
         },
         "jinja2": {
             "hashes": [
-                "sha256:93187ffbc7808079673ef52771baa950426fd664d3aad1d0fa3e95644360e250",
-                "sha256:b0eaf100007721b5c16c1fc1eecb87409464edc10469ddc9a22a27a99123be49"
+                "sha256:077ce6014f7b40d03b47d1f1ca4b0fc8328a692bd284016f806ed0eaca390ad8",
+                "sha256:611bb273cd68f3b993fabdc4064fc858c5b47a973cb5aa7999ec1ba405c87cd7"
             ],
-            "version": "==2.11.1"
+            "markers": "python_version >= '3.6'",
+            "version": "==3.0.3"
         },
         "markupsafe": {
             "hashes": [
-                "sha256:00bc623926325b26bb9605ae9eae8a215691f33cae5df11ca5424f06f2d1f473",
-                "sha256:09027a7803a62ca78792ad89403b1b7a73a01c8cb65909cd876f7fcebd79b161",
-                "sha256:09c4b7f37d6c648cb13f9230d847adf22f8171b1ccc4d5682398e77f40309235",
-                "sha256:1027c282dad077d0bae18be6794e6b6b8c91d58ed8a8d89a89d59693b9131db5",
-                "sha256:13d3144e1e340870b25e7b10b98d779608c02016d5184cfb9927a9f10c689f42",
-                "sha256:24982cc2533820871eba85ba648cd53d8623687ff11cbb805be4ff7b4c971aff",
-                "sha256:29872e92839765e546828bb7754a68c418d927cd064fd4708fab9fe9c8bb116b",
-                "sha256:43a55c2930bbc139570ac2452adf3d70cdbb3cfe5912c71cdce1c2c6bbd9c5d1",
-                "sha256:46c99d2de99945ec5cb54f23c8cd5689f6d7177305ebff350a58ce5f8de1669e",
-                "sha256:500d4957e52ddc3351cabf489e79c91c17f6e0899158447047588650b5e69183",
-                "sha256:535f6fc4d397c1563d08b88e485c3496cf5784e927af890fb3c3aac7f933ec66",
-                "sha256:596510de112c685489095da617b5bcbbac7dd6384aeebeda4df6025d0256a81b",
-                "sha256:62fe6c95e3ec8a7fad637b7f3d372c15ec1caa01ab47926cfdf7a75b40e0eac1",
-                "sha256:6788b695d50a51edb699cb55e35487e430fa21f1ed838122d722e0ff0ac5ba15",
-                "sha256:6dd73240d2af64df90aa7c4e7481e23825ea70af4b4922f8ede5b9e35f78a3b1",
-                "sha256:717ba8fe3ae9cc0006d7c451f0bb265ee07739daf76355d06366154ee68d221e",
-                "sha256:79855e1c5b8da654cf486b830bd42c06e8780cea587384cf6545b7d9ac013a0b",
-                "sha256:7c1699dfe0cf8ff607dbdcc1e9b9af1755371f92a68f706051cc8c37d447c905",
-                "sha256:88e5fcfb52ee7b911e8bb6d6aa2fd21fbecc674eadd44118a9cc3863f938e735",
-                "sha256:8defac2f2ccd6805ebf65f5eeb132adcf2ab57aa11fdf4c0dd5169a004710e7d",
-                "sha256:98c7086708b163d425c67c7a91bad6e466bb99d797aa64f965e9d25c12111a5e",
-                "sha256:9add70b36c5666a2ed02b43b335fe19002ee5235efd4b8a89bfcf9005bebac0d",
-                "sha256:9bf40443012702a1d2070043cb6291650a0841ece432556f784f004937f0f32c",
-                "sha256:ade5e387d2ad0d7ebf59146cc00c8044acbd863725f887353a10df825fc8ae21",
-                "sha256:b00c1de48212e4cc9603895652c5c410df699856a2853135b3967591e4beebc2",
-                "sha256:b1282f8c00509d99fef04d8ba936b156d419be841854fe901d8ae224c59f0be5",
-                "sha256:b2051432115498d3562c084a49bba65d97cf251f5a331c64a12ee7e04dacc51b",
-                "sha256:ba59edeaa2fc6114428f1637ffff42da1e311e29382d81b339c1817d37ec93c6",
-                "sha256:c8716a48d94b06bb3b2524c2b77e055fb313aeb4ea620c8dd03a105574ba704f",
-                "sha256:cd5df75523866410809ca100dc9681e301e3c27567cf498077e8551b6d20e42f",
-                "sha256:cdb132fc825c38e1aeec2c8aa9338310d29d337bebbd7baa06889d09a60a1fa2",
-                "sha256:e249096428b3ae81b08327a63a485ad0878de3fb939049038579ac0ef61e17e7",
-                "sha256:e8313f01ba26fbbe36c7be1966a7b7424942f670f38e666995b88d012765b9be"
+                "sha256:01a9b8ea66f1658938f65b93a85ebe8bc016e6769611be228d797c9d998dd298",
+                "sha256:023cb26ec21ece8dc3907c0e8320058b2e0cb3c55cf9564da612bc325bed5e64",
+                "sha256:0446679737af14f45767963a1a9ef7620189912317d095f2d9ffa183a4d25d2b",
+                "sha256:04635854b943835a6ea959e948d19dcd311762c5c0c6e1f0e16ee57022669194",
+                "sha256:0717a7390a68be14b8c793ba258e075c6f4ca819f15edfc2a3a027c823718567",
+                "sha256:0955295dd5eec6cb6cc2fe1698f4c6d84af2e92de33fbcac4111913cd100a6ff",
+                "sha256:0d4b31cc67ab36e3392bbf3862cfbadac3db12bdd8b02a2731f509ed5b829724",
+                "sha256:10f82115e21dc0dfec9ab5c0223652f7197feb168c940f3ef61563fc2d6beb74",
+                "sha256:168cd0a3642de83558a5153c8bd34f175a9a6e7f6dc6384b9655d2697312a646",
+                "sha256:1d609f577dc6e1aa17d746f8bd3c31aa4d258f4070d61b2aa5c4166c1539de35",
+                "sha256:1f2ade76b9903f39aa442b4aadd2177decb66525062db244b35d71d0ee8599b6",
+                "sha256:20dca64a3ef2d6e4d5d615a3fd418ad3bde77a47ec8a23d984a12b5b4c74491a",
+                "sha256:2a7d351cbd8cfeb19ca00de495e224dea7e7d919659c2841bbb7f420ad03e2d6",
+                "sha256:2d7d807855b419fc2ed3e631034685db6079889a1f01d5d9dac950f764da3dad",
+                "sha256:2ef54abee730b502252bcdf31b10dacb0a416229b72c18b19e24a4509f273d26",
+                "sha256:36bc903cbb393720fad60fc28c10de6acf10dc6cc883f3e24ee4012371399a38",
+                "sha256:37205cac2a79194e3750b0af2a5720d95f786a55ce7df90c3af697bfa100eaac",
+                "sha256:3c112550557578c26af18a1ccc9e090bfe03832ae994343cfdacd287db6a6ae7",
+                "sha256:3dd007d54ee88b46be476e293f48c85048603f5f516008bee124ddd891398ed6",
+                "sha256:4296f2b1ce8c86a6aea78613c34bb1a672ea0e3de9c6ba08a960efe0b0a09047",
+                "sha256:47ab1e7b91c098ab893b828deafa1203de86d0bc6ab587b160f78fe6c4011f75",
+                "sha256:49e3ceeabbfb9d66c3aef5af3a60cc43b85c33df25ce03d0031a608b0a8b2e3f",
+                "sha256:4dc8f9fb58f7364b63fd9f85013b780ef83c11857ae79f2feda41e270468dd9b",
+                "sha256:4efca8f86c54b22348a5467704e3fec767b2db12fc39c6d963168ab1d3fc9135",
+                "sha256:53edb4da6925ad13c07b6d26c2a852bd81e364f95301c66e930ab2aef5b5ddd8",
+                "sha256:5855f8438a7d1d458206a2466bf82b0f104a3724bf96a1c781ab731e4201731a",
+                "sha256:594c67807fb16238b30c44bdf74f36c02cdf22d1c8cda91ef8a0ed8dabf5620a",
+                "sha256:5b6d930f030f8ed98e3e6c98ffa0652bdb82601e7a016ec2ab5d7ff23baa78d1",
+                "sha256:5bb28c636d87e840583ee3adeb78172efc47c8b26127267f54a9c0ec251d41a9",
+                "sha256:60bf42e36abfaf9aff1f50f52644b336d4f0a3fd6d8a60ca0d054ac9f713a864",
+                "sha256:611d1ad9a4288cf3e3c16014564df047fe08410e628f89805e475368bd304914",
+                "sha256:6300b8454aa6930a24b9618fbb54b5a68135092bc666f7b06901f897fa5c2fee",
+                "sha256:63f3268ba69ace99cab4e3e3b5840b03340efed0948ab8f78d2fd87ee5442a4f",
+                "sha256:6557b31b5e2c9ddf0de32a691f2312a32f77cd7681d8af66c2692efdbef84c18",
+                "sha256:693ce3f9e70a6cf7d2fb9e6c9d8b204b6b39897a2c4a1aa65728d5ac97dcc1d8",
+                "sha256:6a7fae0dd14cf60ad5ff42baa2e95727c3d81ded453457771d02b7d2b3f9c0c2",
+                "sha256:6c4ca60fa24e85fe25b912b01e62cb969d69a23a5d5867682dd3e80b5b02581d",
+                "sha256:6fcf051089389abe060c9cd7caa212c707e58153afa2c649f00346ce6d260f1b",
+                "sha256:7d91275b0245b1da4d4cfa07e0faedd5b0812efc15b702576d103293e252af1b",
+                "sha256:89c687013cb1cd489a0f0ac24febe8c7a666e6e221b783e53ac50ebf68e45d86",
+                "sha256:8d206346619592c6200148b01a2142798c989edcb9c896f9ac9722a99d4e77e6",
+                "sha256:905fec760bd2fa1388bb5b489ee8ee5f7291d692638ea5f67982d968366bef9f",
+                "sha256:97383d78eb34da7e1fa37dd273c20ad4320929af65d156e35a5e2d89566d9dfb",
+                "sha256:984d76483eb32f1bcb536dc27e4ad56bba4baa70be32fa87152832cdd9db0833",
+                "sha256:99df47edb6bda1249d3e80fdabb1dab8c08ef3975f69aed437cb69d0a5de1e28",
+                "sha256:9f02365d4e99430a12647f09b6cc8bab61a6564363f313126f775eb4f6ef798e",
+                "sha256:a30e67a65b53ea0a5e62fe23682cfe22712e01f453b95233b25502f7c61cb415",
+                "sha256:ab3ef638ace319fa26553db0624c4699e31a28bb2a835c5faca8f8acf6a5a902",
+                "sha256:aca6377c0cb8a8253e493c6b451565ac77e98c2951c45f913e0b52facdcff83f",
+                "sha256:add36cb2dbb8b736611303cd3bfcee00afd96471b09cda130da3581cbdc56a6d",
+                "sha256:b2f4bf27480f5e5e8ce285a8c8fd176c0b03e93dcc6646477d4630e83440c6a9",
+                "sha256:b7f2d075102dc8c794cbde1947378051c4e5180d52d276987b8d28a3bd58c17d",
+                "sha256:baa1a4e8f868845af802979fcdbf0bb11f94f1cb7ced4c4b8a351bb60d108145",
+                "sha256:be98f628055368795d818ebf93da628541e10b75b41c559fdf36d104c5787066",
+                "sha256:bf5d821ffabf0ef3533c39c518f3357b171a1651c1ff6827325e4489b0e46c3c",
+                "sha256:c47adbc92fc1bb2b3274c4b3a43ae0e4573d9fbff4f54cd484555edbf030baf1",
+                "sha256:cdfba22ea2f0029c9261a4bd07e830a8da012291fbe44dc794e488b6c9bb353a",
+                "sha256:d6c7ebd4e944c85e2c3421e612a7057a2f48d478d79e61800d81468a8d842207",
+                "sha256:d7f9850398e85aba693bb640262d3611788b1f29a79f0c93c565694658f4071f",
+                "sha256:d8446c54dc28c01e5a2dbac5a25f071f6653e6e40f3a8818e8b45d790fe6ef53",
+                "sha256:deb993cacb280823246a026e3b2d81c493c53de6acfd5e6bfe31ab3402bb37dd",
+                "sha256:e0f138900af21926a02425cf736db95be9f4af72ba1bb21453432a07f6082134",
+                "sha256:e9936f0b261d4df76ad22f8fee3ae83b60d7c3e871292cd42f40b81b70afae85",
+                "sha256:f0567c4dc99f264f49fe27da5f735f414c4e7e7dd850cfd8e69f0862d7c74ea9",
+                "sha256:f5653a225f31e113b152e56f154ccbe59eeb1c7487b39b9d9f9cdb58e6c79dc5",
+                "sha256:f826e31d18b516f653fe296d967d700fddad5901ae07c622bb3705955e1faa94",
+                "sha256:f8ba0e8349a38d3001fae7eadded3f6606f0da5d748ee53cc1dab1d6527b9509",
+                "sha256:f9081981fe268bd86831e5c75f7de206ef275defcb82bc70740ae6dc507aee51",
+                "sha256:fa130dd50c57d53368c9d59395cb5526eda596d3ffe36666cd81a44d56e48872"
             ],
-            "version": "==1.1.1"
+            "markers": "python_version >= '3.6'",
+            "version": "==2.0.1"
         },
         "mccabe": {
             "hashes": [
                 "sha256:ab8a6258860da4b6677da4bd2fe5dc2c659cff31b3ee4f7f5d64e79735b80d42",
                 "sha256:dd8d182285a0fe56bace7f45b5e7d1a6ebcbf524e8f3bd87eb0f125271b8831f"
             ],
             "version": "==0.6.1"
         },
         "more-itertools": {
             "hashes": [
-                "sha256:5dd8bcf33e5f9513ffa06d5ad33d78f31e1931ac9a18f33d37e77a180d393a7c",
-                "sha256:b1ddb932186d8a6ac451e1d95844b382f55e12686d51ca0c68b6f61f2ab7a507"
+                "sha256:43e6dd9942dffd72661a2c4ef383ad7da1e6a3e968a927ad7a6083ab410a688b",
+                "sha256:7dc6ad46f05f545f900dd59e8dfb4e84a4827b97b3cfecb175ea0c7d247f6064"
             ],
-            "version": "==8.2.0"
+            "markers": "python_version >= '3.5'",
+            "version": "==8.12.0"
         },
         "mypy": {
             "hashes": [
                 "sha256:8e071ec32cc226e948a34bbb3d196eb0fd96f3ac69b6843a5aff9bd4efa14455",
                 "sha256:fb90c804b84cfd8133d3ddfbd630252694d11ccc1eb0166a1b2efb5da37ecab2"
             ],
             "index": "pypi",
@@ -347,25 +416,27 @@
                 "sha256:090fedd75945a69ae91ce1303b5824f428daf5a028d2f6ab8a299250a846f15d",
                 "sha256:2d82818f5bb3e369420cb3c4060a7970edba416647068eb4c5343488a6c604a8"
             ],
             "version": "==0.4.3"
         },
         "packaging": {
             "hashes": [
-                "sha256:3c292b474fda1671ec57d46d739d072bfd495a4f51ad01a055121d81e952b7a3",
-                "sha256:82f77b9bee21c1bafbf35a84905d604d5d1223801d639cf3ed140bd651c08752"
+                "sha256:dd47c42927d89ab911e606518907cc2d3a1f38bbd026385970643f9c5b8ecfeb",
+                "sha256:ef103e05f519cdc783ae24ea4e2e0f508a9c99b2d4969652eed6a2e1ea5bd522"
             ],
-            "version": "==20.3"
+            "markers": "python_version >= '3.6'",
+            "version": "==21.3"
         },
         "parso": {
             "hashes": [
-                "sha256:0c5659e0c6eba20636f99a04f469798dca8da279645ce5c387315b2c23912157",
-                "sha256:8515fc12cfca6ee3aa59138741fc5624d62340c97e401c74875769948d4f2995"
+                "sha256:8c07be290bb59f03588915921e29e8a50002acaf2cdc5fa0e0114f91709fafa0",
+                "sha256:c001d4636cd3aecdaf33cbb40aebb59b094be2a74c556778ef5576c175e19e75"
             ],
-            "version": "==0.6.2"
+            "markers": "python_version >= '3.6'",
+            "version": "==0.8.3"
         },
         "pexpect": {
             "hashes": [
                 "sha256:0b48a55dcb3c05f3329815901ea4fc1537514d6ba867a152b581d69ae3710937",
                 "sha256:fc65a43959d153d0114afe13997d439c22823a27cefceb5ff35c2178c6784c0c"
             ],
             "markers": "sys_platform != 'win32'",
@@ -376,105 +447,119 @@
                 "sha256:87683d47965c1da65cdacaf31c8441d12b8044cdec9aca500cd78fc2c683afca",
                 "sha256:9649af414d74d4df115d5d718f82acb59c9d418196b7b4290ed47a12ce62df56"
             ],
             "version": "==0.7.5"
         },
         "pluggy": {
             "hashes": [
-                "sha256:15b2acde666561e1298d71b523007ed7364de07029219b604cf808bfa1c765b0",
-                "sha256:966c145cd83c96502c3c3868f50408687b38434af77734af1e9ca461a4081d2d"
+                "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
+                "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
-            "version": "==0.13.1"
+            "markers": "python_version >= '3.6'",
+            "version": "==1.0.0"
         },
         "prompt-toolkit": {
             "hashes": [
                 "sha256:46642344ce457641f28fc9d1c9ca939b63dadf8df128b86f1b9860e59c73a5e4",
                 "sha256:e7f8af9e3d70f514373bf41aa51bc33af12a6db3f71461ea47fea985defb2c31",
                 "sha256:f15af68f66e664eaa559d4ac8a928111eebd5feda0c11738b5998045224829db"
             ],
             "version": "==2.0.10"
         },
         "ptyprocess": {
             "hashes": [
-                "sha256:923f299cc5ad920c68f2bc0bc98b75b9f838b93b599941a6b63ddbc2476394c0",
-                "sha256:d7cc528d76e76342423ca640335bd3633420dc1366f258cb31d05e865ef5ca1f"
+                "sha256:4b41f3967fce3af57cc7e94b888626c18bf37a083e3651ca8feeb66d492fef35",
+                "sha256:5c5d0a3b48ceee0b48485e0c26037c0acd7d29765ca3fbb5cb3831d347423220"
             ],
-            "version": "==0.6.0"
+            "version": "==0.7.0"
         },
         "py": {
             "hashes": [
-                "sha256:5e27081401262157467ad6e7f851b7aa402c5852dbcb3dae06768434de5752aa",
-                "sha256:c20fdd83a5dbc0af9efd622bee9a5564e278f6380fffcacc43ba6f43db2813b0"
+                "sha256:51c75c4126074b472f746a24399ad32f6053d1b34b68d2fa41e558e6f4a98719",
+                "sha256:607c53218732647dff4acdfcd50cb62615cedf612e72d1724fb1a0cc6405b378"
             ],
-            "version": "==1.8.1"
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
+            "version": "==1.11.0"
         },
         "pycodestyle": {
             "hashes": [
+                "sha256:74abc4e221d393ea5ce1f129ea6903209940c1ecd29e002e8c6933c2b21026e0",
                 "sha256:cbc619d09254895b0d12c2c691e237b2e91e9b2ecf5e84c26b35400f93dcfb83",
                 "sha256:cbfca99bd594a10f674d0cd97a3d802a1fdef635d4361e1a2658de47ed261e3a"
             ],
             "version": "==2.4.0"
         },
         "pyflakes": {
             "hashes": [
                 "sha256:9a7662ec724d0120012f6e29d6248ae3727d821bba522a0e6b356eff19126a49",
                 "sha256:f661252913bc1dbe7fcfcbf0af0db3f42ab65aabd1a6ca68fe5d466bace94dae"
             ],
             "version": "==2.0.0"
         },
         "pygments": {
             "hashes": [
-                "sha256:647344a061c249a3b74e230c739f434d7ea4d8b1d5f3721bc0f3558049b38f44",
-                "sha256:ff7a40b4860b727ab48fad6360eb351cc1b33cbf9b15a0f689ca5353e9463324"
+                "sha256:b8e67fe6af78f492b3c4b3e2970c0624cbf08beb1e493b2c99b9fa1b67a20380",
+                "sha256:f398865f7eb6874156579fdf36bc840a03cab64d1cde9e93d68f46a425ec52c6"
             ],
-            "version": "==2.6.1"
+            "markers": "python_version >= '3.5'",
+            "version": "==2.10.0"
         },
         "pyparsing": {
             "hashes": [
-                "sha256:4c830582a84fb022400b85429791bc551f1f4871c33f23e44f353119e92f969f",
-                "sha256:c342dccb5250c08d45fd6f8b4a559613ca603b57498511740e65cd11a2e7dcec"
+                "sha256:04ff808a5b90911829c55c4e26f75fa5ca8a2f5f36aa3a51f68e27033341d3e4",
+                "sha256:d9bdec0013ef1eb5a84ab39a3b3868911598afa494f5faa038647101504e2b81"
             ],
-            "version": "==2.4.6"
+            "markers": "python_version >= '3.6'",
+            "version": "==3.0.6"
         },
         "pytest": {
             "hashes": [
                 "sha256:630ff1dbe04f469ee78faa5660f712e58b953da7df22ea5d828c9012e134da43",
                 "sha256:a2b5232735dd0b736cbea9c0f09e5070d78fcaba2823a4f6f09d9a81bd19415c"
             ],
             "index": "pypi",
             "version": "==3.10.0"
         },
         "pytz": {
             "hashes": [
-                "sha256:1c557d7d0e871de1f5ccd5833f60fb2550652da6be2693c1e02300743d21500d",
-                "sha256:b02c06db6cf09c12dd25137e563b31700d3b80fcc4ad23abb7a315f2789819be"
+                "sha256:3672058bc3453457b622aab7a1c3bfd5ab0bdae451512f6cf25f64ed37f5b87c",
+                "sha256:acad2d8b20a1af07d4e4c9d2e9285c5ed9104354062f275f3fcd88dcef4f1326"
             ],
-            "version": "==2019.3"
+            "version": "==2021.3"
         },
         "requests": {
             "hashes": [
                 "sha256:65b3a120e4329e33c9889db89c80976c5272f56ea92d3e74da8a463992e3ff54",
                 "sha256:ea881206e59f41dbd0bd445437d792e43906703fff75ca8ff43ccdb11f33f263"
             ],
             "index": "pypi",
             "version": "==2.20.1"
         },
+        "setuptools": {
+            "hashes": [
+                "sha256:6d10741ff20b89cd8c6a536ee9dc90d3002dec0226c78fb98605bfb9ef8a7adf",
+                "sha256:d144f85102f999444d06f9c0e8c737fd0194f10f2f7e5fdb77573f6e2fa4fad0"
+            ],
+            "markers": "python_version >= '3.6'",
+            "version": "==59.5.0"
+        },
         "six": {
             "hashes": [
-                "sha256:236bdbdce46e6e6a3d61a337c0f8b763ca1e8717c03b369e87a7ec7ce1319c0a",
-                "sha256:8f3cd2e254d8f793e7f3d6d9df77b92252b52637291d0f0da013c76ea2724b6c"
+                "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
+                "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
-            "version": "==1.14.0"
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
+            "version": "==1.16.0"
         },
         "snowballstemmer": {
             "hashes": [
-                "sha256:209f257d7533fdb3cb73bdbd24f436239ca3b2fa67d56f6ff88e86be08cc5ef0",
-                "sha256:df3bac3df4c2c01363f3dd2cfa78cce2840a79b9f1c2d2de9ce8d31683992f52"
+                "sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1",
+                "sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a"
             ],
-            "version": "==2.0.0"
+            "version": "==2.2.0"
         },
         "sphinx": {
             "hashes": [
                 "sha256:652eb8c566f18823a022bb4b6dbc868d366df332a11a0226b5bc3a798a479f17",
                 "sha256:d222626d8356de702431e813a05c68a35967e3d66c6cd1c2c89539bb179a7464"
             ],
             "index": "pypi",
@@ -484,27 +569,37 @@
             "hashes": [
                 "sha256:02f02a676d6baabb758a20c7a479d58648e0f64f13e07d1b388e9bb2afe86a09",
                 "sha256:d0f6bc70f98961145c5b0e26a992829363a197321ba571b31b24ea91879e0c96"
             ],
             "index": "pypi",
             "version": "==0.4.2"
         },
+        "sphinxcontrib-serializinghtml": {
+            "hashes": [
+                "sha256:352a9a00ae864471d3a7ead8d7d79f5fc0b57e8b3f95e9867eb9eb28999b92fd",
+                "sha256:aa5f6de5dfdf809ef505c4895e51ef5c9eac17d0f287933eb49ec495280b6952"
+            ],
+            "markers": "python_version >= '3.5'",
+            "version": "==1.1.5"
+        },
         "sphinxcontrib-websupport": {
             "hashes": [
-                "sha256:545f5da4bd7757e82b8a23ce3af9500c6ffeedbcb13429fca436ad1e80bd10cf",
-                "sha256:69364896eae5d1145d82b6ee09f66d597099ef8069615e2888921ec48005470f"
+                "sha256:4edf0223a0685a7c485ae5a156b6f529ba1ee481a1417817935b20bde1956232",
+                "sha256:6fc9287dfc823fe9aa432463edd6cea47fa9ebbf488d7f289b322ffcfca075c7"
             ],
-            "version": "==1.2.1"
+            "markers": "python_version >= '3.5'",
+            "version": "==1.2.4"
         },
         "traitlets": {
             "hashes": [
-                "sha256:70b4c6a1d9019d7b4f6846832288f86998aa3b9207c6821f3578a6a6a467fe44",
-                "sha256:d023ee369ddd2763310e4c3eae1ff649689440d4ae59d7485eb4cfbbe3e359f7"
+                "sha256:059f456c5a7c1c82b98c2e8c799f39c9b8128f6d0d46941ee118daace9eb70c7",
+                "sha256:2d313cc50a42cd6c277e7d7dc8d4d7fedd06a2c215f78766ae7b1a66277e0033"
             ],
-            "version": "==4.3.3"
+            "markers": "python_version >= '3.7'",
+            "version": "==5.1.1"
         },
         "typed-ast": {
             "hashes": [
                 "sha256:0cf0c406af2a6472a02254fe1ced40cb81a7c1215b7ceba88a3bb9c3a864f851",
                 "sha256:1b784cd3c6778cd7b99afb41ddcaa1eb5b35a399210db7fcf24ed082670e0070",
                 "sha256:2d7a322c1df6cccff2381c0475c1ebf82d3e9a331e48ed4ea89bbc72a8dedca6",
                 "sha256:4304399ff89452871348f6fb7a7112454cd508fbe3eb49b5ed711cce9b99fe9e",
@@ -524,30 +619,40 @@
                 "sha256:cb1c7e5b3195103f5a784db7969fc55463cfae9b354e3b97cc219d32293d5e65",
                 "sha256:d2d2cce74165cae2663167c921e331fb0eecfff2e93254dfdb16beb99716e519",
                 "sha256:d6fc3b9fbf67d556223aa5493501022e1d585b9a1892fa87ba1257627763c461",
                 "sha256:fa4eafaa57074958f065c2a6222d8f11162739f8c9db125472a1f04794a0b91d"
             ],
             "version": "==1.1.2"
         },
+        "typing-extensions": {
+            "hashes": [
+                "sha256:4ca091dea149f945ec56afb48dae714f21e8692ef22a395223bcd328961b6a0e",
+                "sha256:7f001e5ac290a0c0401508864c7ec868be4e701886d5b573a9528ed3973d9d3b"
+            ],
+            "markers": "python_version < '3.8'",
+            "version": "==4.0.1"
+        },
         "urllib3": {
             "hashes": [
                 "sha256:2393a695cd12afedd0dcb26fe5d50d0cf248e5a66f75dbd89a3d4eb333a61af4",
                 "sha256:a637e5fae88995b256e3409dc4d52c2e2e0ba32c42a6365fee8bbd2238de3cfb"
             ],
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3' and python_version < '4'",
             "version": "==1.24.3"
         },
         "wcwidth": {
             "hashes": [
-                "sha256:cafe2186b3c009a04067022ce1dcd79cb38d8d65ee4f4791b8888d6599d1bbe1",
-                "sha256:ee73862862a156bf77ff92b09034fc4825dd3af9cf81bc5b360668d425f3c5f1"
+                "sha256:beb4802a9cebb9144e99086eff703a642a13d6a0052920003a230f3294bbe784",
+                "sha256:c4d647b99872929fdb7bdcaa4fbe7f01413ed3d98077df798530e5b04f116c83"
             ],
-            "version": "==0.1.9"
+            "version": "==0.2.5"
         },
         "zipp": {
             "hashes": [
-                "sha256:aa36550ff0c0b7ef7fa639055d797116ee891440eac1a56f378e2d3179e0320b",
-                "sha256:c599e4d75c98f6798c509911d08a22e6c021d074469042177c8c86fb92eefd96"
+                "sha256:71c644c5369f4a6e07636f0aa966270449561fcea2e3d6747b8d23efaa9d7832",
+                "sha256:9fe5ea21568a0a70e50f273397638d39b03353731e6cbbb3fd8502a33fec40bc"
             ],
-            "version": "==3.1.0"
+            "markers": "python_version >= '3.6'",
+            "version": "==3.6.0"
         }
     }
 }
```

### Comparing `hhpy-0.3.0/README.md` & `hhpy-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `hhpy-0.3.0/hhpy.egg-info/PKG-INFO` & `hhpy-0.3.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 Metadata-Version: 2.1
 Name: hhpy
-Version: 0.3.0
-Summary: hhpy - convenient data science
+Version: 0.3.1
+Summary: Convenient Data Science
 Home-page: https://github.com/rhedak/hhpy
 Author: Henrik Hanssen
-Author-email: henrik.hanssen@gmail.com
+Author-email: Henrik Hanssen <rhedak00@yahoo.de>
 License: Apache 2.0
-Description: # hhpy - Data Science convenience project
-        
-        
-        Built with [Python Package Template Project](https://github.com/AlexIoannides/py-package-template/). 
-        
-        My attempt at creating a convenient way to use different data science and machine learning operations and frameworks using one unified way.
-        The main idea is to store data in pandas DataFrames and start from there.
-        
-        Also provides several extensions on pandas, matplotlib and seaborn for convenience.
-        
-        ## Installing
-        
-        Install and update using [pip](https://pypi.org/project/hhpy/):
-        
-        ```bash
-        pip install hhpy
-        ```
-        
-        Or get the latest dev version from github
-        
-        ```bash
-        pip install git+https://github.com/rhedak/hhpy
-        ```
-        
-        ## Documentation
-        
-        Documentation is available at [https://hhpy.readthedocs.io/](https://hhpy.readthedocs.io/)
+Project-URL: Homepage, https://github.com/rhedak/hhpy
 Keywords: package development template
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.6.*
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# hhpy - Data Science convenience project
+
+
+Built with [Python Package Template Project](https://github.com/AlexIoannides/py-package-template/). 
+
+My attempt at creating a convenient way to use different data science and machine learning operations and frameworks using one unified way.
+The main idea is to store data in pandas DataFrames and start from there.
+
+Also provides several extensions on pandas, matplotlib and seaborn for convenience.
+
+## Installing
+
+Install and update using [pip](https://pypi.org/project/hhpy/):
+
+```bash
+pip install hhpy
+```
+
+Or get the latest dev version from github
+
+```bash
+pip install git+https://github.com/rhedak/hhpy
+```
+
+## Documentation
+
+Documentation is available at [https://hhpy.readthedocs.io/](https://hhpy.readthedocs.io/)
```

### Comparing `hhpy-0.3.0/hhpy/.DS_Store` & `hhpy-0.3.1/hhpy/.DS_Store`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
-00000010: 0000 1000 0000 040a 0000 0000 0000 0000  ................
+00000010: 0000 1000 0000 0209 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 000a  ................
+00000040: 0000 0000 0000 0002 0000 0000 0000 0009  ................
 00000050: 0000 0001 0000 1000 0069 0074 005f 005f  .........i.t._._
 00000060: 002e 0070 0000 0000 0000 0000 0000 0000  ...p............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -26,81 +26,81 @@
 00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000260: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000003a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000003c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000003d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000003e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000200: 0000 0000 0000 0000 0000 0009 0000 000b  ................
+00000210: 005f 005f 0069 006e 0069 0074 005f 005f  ._._.i.n.i.t._._
+00000220: 002e 0070 0079 496c 6f63 626c 6f62 0000  ...p.yIlocblob..
+00000230: 0010 0000 003b 0000 0028 ffff ffff ffff  .....;...(......
+00000240: 0000 0000 000c 005f 005f 0069 006e 0069  ......._._.i.n.i
+00000250: 0074 005f 005f 002e 0070 0079 0063 496c  .t._._...p.y.cIl
+00000260: 6f63 626c 6f62 0000 0010 0000 00a9 0000  ocblob..........
+00000270: 0028 ffff ffff ffff 0000 0000 000e 005f  .(............._
+00000280: 005f 0076 0065 0072 0073 0069 006f 006e  ._.v.e.r.s.i.o.n
+00000290: 005f 005f 002e 0070 0079 496c 6f63 626c  ._._...p.yIlocbl
+000002a0: 6f62 0000 0010 0000 0185 0000 0028 ffff  ob...........(..
+000002b0: ffff ffff 0000 0000 0005 0064 0073 002e  ...........d.s..
+000002c0: 0070 0079 496c 6f63 626c 6f62 0000 0010  .p.yIlocblob....
+000002d0: 0000 003b 0000 0098 ffff ffff ffff 0000  ...;............
+000002e0: 0000 000f 0065 006e 0074 0072 0079 005f  .....e.n.t.r.y._
+000002f0: 0070 006f 0069 006e 0074 0073 002e 0070  .p.o.i.n.t.s...p
+00000300: 0079 496c 6f63 626c 6f62 0000 0010 0000  .yIlocblob......
+00000310: 00a9 0000 0098 ffff ffff ffff 0000 0000  ................
+00000320: 000a 0069 0070 0079 0074 0068 006f 006e  ...i.p.y.t.h.o.n
+00000330: 002e 0070 0079 496c 6f63 626c 6f62 0000  ...p.yIlocblob..
+00000340: 0010 0000 0117 0000 0098 ffff ffff ffff  ................
+00000350: 0000 0000 0007 006d 0061 0069 006e 002e  .......m.a.i.n..
+00000360: 0070 0079 496c 6f63 626c 6f62 0000 0010  .p.yIlocblob....
+00000370: 0000 0185 0000 0098 ffff ffff ffff 0000  ................
+00000380: 0000 000c 006d 006f 0064 0065 006c 006c  .....m.o.d.e.l.l
+00000390: 0069 006e 0067 002e 0070 0079 496c 6f63  .i.n.g...p.yIloc
+000003a0: 626c 6f62 0000 0010 0000 003b 0000 0108  blob.......;....
+000003b0: ffff ffff ffff 0000 0000 000b 0070 006c  .............p.l
+000003c0: 006f 0074 0074 0069 006e 0067 002e 0070  .o.t.t.i.n.g...p
+000003d0: 0079 496c 6f63 626c 6f62 0000 0010 0000  .yIlocblob......
+000003e0: 00a9 0000 0108 ffff ffff ffff 0000 0000  ................
 000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000400: 0000 0000 0000 0000 0000 000a 0000 000b  ................
-00000410: 005f 005f 0069 006e 0069 0074 005f 005f  ._._.i.n.i.t._._
-00000420: 002e 0070 0079 496c 6f63 626c 6f62 0000  ...p.yIlocblob..
-00000430: 0010 0000 003b 0000 0028 ffff ffff ffff  .....;...(......
-00000440: 0000 0000 000c 005f 005f 0069 006e 0069  ......._._.i.n.i
-00000450: 0074 005f 005f 002e 0070 0079 0063 496c  .t._._...p.y.cIl
-00000460: 6f63 626c 6f62 0000 0010 0000 00a9 0000  ocblob..........
-00000470: 0028 ffff ffff ffff 0000 0000 000b 005f  .(............._
-00000480: 005f 0070 0079 0063 0061 0063 0068 0065  ._.p.y.c.a.c.h.e
-00000490: 005f 005f 496c 6f63 626c 6f62 0000 0010  ._._Ilocblob....
-000004a0: 0000 0117 0000 0028 ffff ffff ffff 0000  .......(........
-000004b0: 0000 000e 005f 005f 0076 0065 0072 0073  ....._._.v.e.r.s
-000004c0: 0069 006f 006e 005f 005f 002e 0070 0079  .i.o.n._._...p.y
-000004d0: 496c 6f63 626c 6f62 0000 0010 0000 0185  Ilocblob........
-000004e0: 0000 0028 ffff ffff ffff 0000 0000 0005  ...(............
-000004f0: 0064 0073 002e 0070 0079 496c 6f63 626c  .d.s...p.yIlocbl
-00000500: 6f62 0000 0010 0000 003b 0000 0098 ffff  ob.......;......
-00000510: ffff ffff 0000 0000 000f 0065 006e 0074  ...........e.n.t
-00000520: 0072 0079 005f 0070 006f 0069 006e 0074  .r.y._.p.o.i.n.t
-00000530: 0073 002e 0070 0079 496c 6f63 626c 6f62  .s...p.yIlocblob
-00000540: 0000 0010 0000 00a9 0000 0098 ffff ffff  ................
-00000550: ffff 0000 0000 000a 0069 0070 0079 0074  .........i.p.y.t
-00000560: 0068 006f 006e 002e 0070 0079 496c 6f63  .h.o.n...p.yIloc
-00000570: 626c 6f62 0000 0010 0000 0117 0000 0098  blob............
-00000580: ffff ffff ffff 0000 0000 0007 006d 0061  .............m.a
-00000590: 0069 006e 002e 0070 0079 496c 6f63 626c  .i.n...p.yIlocbl
-000005a0: 6f62 0000 0010 0000 0185 0000 0098 ffff  ob..............
-000005b0: ffff ffff 0000 0000 000c 006d 006f 0064  ...........m.o.d
-000005c0: 0065 006c 006c 0069 006e 0067 002e 0070  .e.l.l.i.n.g...p
-000005d0: 0079 496c 6f63 626c 6f62 0000 0010 0000  .yIlocblob......
-000005e0: 003b 0000 0108 ffff ffff ffff 0000 0000  .;..............
-000005f0: 000b 0070 006c 006f 0074 0074 0069 006e  ...p.l.o.t.t.i.n
-00000600: 0067 002e 0070 0079 496c 6f63 626c 6f62  .g...p.yIlocblob
-00000610: 0000 0010 0000 00a9 0000 0108 ffff ffff  ................
-00000620: ffff 0000 0000 0000 0000 0000 0000 0000  ................
+00000400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000410: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000430: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000440: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000450: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000460: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000470: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000480: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000490: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000004a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000004b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000004c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000004d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000004e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000004f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000500: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000510: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000520: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000530: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000540: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000550: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000560: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000570: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000580: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000590: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000005a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000005b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000005c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000005d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000005e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000005f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000600: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000610: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000620: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000630: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000640: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000650: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000660: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000670: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000680: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000690: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -251,15 +251,15 @@
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0003 0000 0000 0000 100b  ................
-00001010: 0000 0045 0000 040a 0000 0000 0000 0000  ...E............
+00001010: 0000 0045 0000 0209 0000 0000 0000 0000  ...E............
 00001020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -319,15 +319,15 @@
 000013e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001400: 0000 0000 0000 0000 0000 0000 0000 0001  ................
 00001410: 0444 5344 4200 0000 0100 0000 0000 0000  .DSDB...........
 00001420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001430: 0200 0000 2000 0000 6000 0000 0000 0000  .... ...`.......
 00001440: 0100 0000 8000 0000 0100 0001 0000 0000  ................
-00001450: 0100 0002 0000 0000 0000 0000 0200 0008  ................
+00001450: 0000 0000 0100 0004 0000 0000 0200 0008  ................
 00001460: 0000 0018 0000 0000 0000 0000 0100 0020  ............... 
 00001470: 0000 0000 0100 0040 0000 0000 0100 0080  .......@........
 00001480: 0000 0000 0100 0100 0000 0000 0100 0200  ................
 00001490: 0000 0000 0100 0400 0000 0000 0100 0800  ................
 000014a0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
 000014b0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
 000014c0: 0000 0000 0101 0000 0000 0000 0102 0000  ................
```

### Comparing `hhpy-0.3.0/hhpy/ds.py` & `hhpy-0.3.1/hhpy/ds.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,18 +17,19 @@
 from scipy import stats, signal
 from scipy.spatial import distance
 from sklearn.metrics import r2_score, mean_squared_error, mean_absolute_error, median_absolute_error
 from sklearn.preprocessing import StandardScaler
 from typing import Mapping, Sequence, Callable, Union, List, Optional, Tuple, Any
 from io import StringIO
 from datetime import datetime
+from docrep import DocstringProcessor
 
 # --- local imports
 from hhpy.main import export, BaseClass, assert_list, tprint, progressbar, qformat, list_intersection, round_signif, \
-    is_list_like, dict_list, append_to_dict_list, concat_cols, DocstringProcessor, reformat_string, dict_inv, \
+    is_list_like, dict_list, append_to_dict_list, concat_cols, reformat_string, dict_inv, \
     list_exclude, docstr as docstr_main, SequenceOfScalars, SequenceOrScalar, STRING_NAN, is_scalar, GROUPBY_DUMMY, \
     assert_scalar, list_merge
 
 # ---- variables
 # --- constants
 ROW_DUMMY = '__row__'
 # --- validations
@@ -79,15 +80,15 @@
 
 
 # ---- classes
 @export
 class DFMapping(BaseClass):
     """
         Mapping object bound to a pandas DataFrame that standardizes column names and values according to the chosen
-        conventions. Also implements google translation. Can be used like an sklearn scalar object.
+        conventions. Also implements google translation. Can be used like a sklearn scalar object.
         The mapping can be saved and later used to restore the original shape of the DataFrame.
         Note that the index is exempt.
 
         :param name: name of the object [Optional]
         :param df: a DataFrame to init on or path to a saved DFMapping object [Optional]
         :param kwargs: other arguments passed to the respective init function
     """
@@ -99,15 +100,15 @@
     # --- functions
     def __init__(self, df: Union[pd.DataFrame, dict, str] = None, **kwargs) -> None:
 
         self.col_mapping = {}
         self.value_mapping = {}
 
         # -- defaults
-        # - if the function is called with only one argument attempt to parse it's type and act accordingly
+        # - if the function is called with only one argument attempt to parse its type and act accordingly
         # DataFrame is passed: init from it
         if isinstance(df, pd.DataFrame):
             self.from_df(df, **kwargs)
         # Dict is passed: init from it
         elif isinstance(df, dict):
             self.from_dict(df)
         # path to excel or pickle file is passed: init from it
@@ -127,15 +128,15 @@
         :param df: %(df)s
         :param col_names: %(DFMapping__col_names)s
         :param values:  %(DFMapping__values)s
         :param columns: %(DFMapping__columns)s
         :param return_type: if 'self': writes to self, 'tuple' returns (col_mapping, value_mapping) [optional]
         :param printf: %(printf)s
         :param duplicate_limit: allowed number of reformated duplicates per column, each duplicate is suffixed with '_'
-            but if you have too many you likely have a column of non allowed character strings and the mapping
+            but if you have too many you likely have a column of non-allowed character strings and the mapping
             would take a very long time. The duplicate handling therefore stops and a warning is triggered
             since the transformation is no longer invertible. Consider excluding the column or using cat codes
             [optional]
         :param warn: %(warn)s
         :param kwargs: Other keyword arguments passed to :func:`~hhpy.main.reformat_string` [optional]
         :return: see return_type
         """
@@ -143,15 +144,16 @@
         # -- assert
         df = assert_df(df)
 
         # -- init
         # assert
         if return_type not in validations['DFMapping__from_df__return_type']:
             if warn:
-                warnings.warn(f'Unknown return_type {return_type}, falling back to self')
+                warnings.warn(
+                    f'Unknown return_type {return_type}, falling back to self')
             return_type = 'self'
 
         # -- main
         # extract columns
         if columns:
             _columns = columns
         else:
@@ -162,27 +164,29 @@
         _value_mapping = {}
         _str_columns = df.select_dtypes(['object', 'category']).columns
 
         # loop columns
         for _it, _column in enumerate(_columns):
             # progressbar
             if printf:
-                progressbar(_it, len(_columns), printf=printf, print_prefix=f'{_column}: ')
+                progressbar(_it, len(_columns), printf=printf,
+                            print_prefix=f'{_column}: ')
             # map col name
             if col_names:
                 _reformated_column = reformat_string(_column, **kwargs)
                 # careful: it is possible that the reformated string is a duplicate, in this case we append '_' to the
                 # string until it is no longer a duplicate
                 _it_ = 0
                 while _reformated_column in _col_mapping.values():
                     _reformated_column += '_'
                     _it_ += 1
                     if _it_ == duplicate_limit:
                         if warn:
-                            warnings.warn(f'too many reformated duplicates in column names')
+                            warnings.warn(
+                                'too many reformated duplicates in column names')
                         break
                 # assign to dict
                 _col_mapping[_column] = _reformated_column
             # check if column is string like
             if _column in _str_columns:
                 # get unique values
                 _uniques = df[_column].drop_duplicates().values
@@ -201,15 +205,16 @@
                         # append '_' to the string until it is no longer a duplicate
                         _it_ = 0
                         while _reformated_unique in _value_mapping[_column].values():
                             _reformated_unique += '_'
                             _it_ += 1
                             if _it_ == duplicate_limit:
                                 if warn:
-                                    warnings.warn(f'too many reformated duplicates in column {_column}')
+                                    warnings.warn(
+                                        f'too many reformated duplicates in column {_column}')
                                 break
                         # assign to dict
                         _value_mapping[_column][_unique] = _reformated_unique
         # progressbar 100%
         if printf:
             progressbar(printf=printf)
 
@@ -317,15 +322,16 @@
         :param columns: %(DFMapping__columns)s
         :param kwargs: passed to transform
         :param kwargs_fit: passed to fit
         :return: see transform
         """
         if kwargs_fit is None:
             kwargs_fit = {}
-        self.fit(df=df, col_names=col_names, values=values, columns=columns, **kwargs_fit)
+        self.fit(df=df, col_names=col_names, values=values,
+                 columns=columns, **kwargs_fit)
         return self.transform(df=df, col_names=col_names, values=values, columns=columns, **kwargs)
 
     def to_excel(self, path: str, if_exists: str = 'error') -> None:
         """
         Save the DFMapping object as an excel file. Useful if you want to edit the results of the automatically
         generated object to fit your specific needs.
 
@@ -344,30 +350,33 @@
                 _df_mapping = pd.read_excel(path, sheet_name, index_col=0).append(_df_mapping)\
                     .pipe(drop_duplicate_indices)
             # write excel
             _df_mapping.to_excel(writer, sheet_name=sheet_name)
         # -- init
         # - assert
         if if_exists not in validations['DFMapping__to_excel__if_exists']:
-            raise ValueError(f"if_exists must be one of {validations['DFMapping__to_excel__if_exists']}")
+            raise ValueError(
+                f"if_exists must be one of {validations['DFMapping__to_excel__if_exists']}")
         # - handle if_exists
         _sheet_names = []
         if os.path.exists(path):
             if if_exists == 'error':
-                raise FileExistsError(f"file already exists, please specify if_exists as one of ")
+                raise FileExistsError('file already exists, please specify if_exists as one of')
             elif if_exists == 'append':
                 _sheet_names = pd.ExcelFile(path).sheet_names
         # -- main
         # pandas ExcelWriter object (saves on close)
         with pd.ExcelWriter(path) as _writer:
             # col mapping
-            _write_excel_sheet(writer=_writer, mapping=self.col_mapping, sheet_name='__columns__')
+            _write_excel_sheet(
+                writer=_writer, mapping=self.col_mapping, sheet_name='__columns__')
             # value mappings
             for _key, _mapping in self.value_mapping.items():
-                _write_excel_sheet(writer=_writer, mapping=_mapping, sheet_name=_key)
+                _write_excel_sheet(
+                    writer=_writer, mapping=_mapping, sheet_name=_key)
 
     def from_excel(self, path: str) -> None:
         """
         Init the DFMapping object from an excel file. For example you could auto generate a DFMapping using googletrans
         and then adjust the translations you feel are inappropriate in the excel file. Then regenerate the object
         from the edited excel file.
 
@@ -379,15 +388,16 @@
             return pd.read_excel(xls, sheet_name, index_col=0).T.to_dict(orient='records')[0]
 
         # open ExcelFile
         with pd.ExcelFile(path) as _xls:
             self.col_mapping = _read_excel(xls=_xls, sheet_name='__columns__')
             self.value_mapping = {}
             for _sheet_name in list_exclude(_xls.sheet_names, '__columns__'):
-                self.value_mapping[_sheet_name] = _read_excel(xls=_xls, sheet_name=_sheet_name)
+                self.value_mapping[_sheet_name] = _read_excel(
+                    xls=_xls, sheet_name=_sheet_name)
 
 
 # ---- functions
 # --- export
 @export
 def assert_df(df: Any, groupby: Union[SequenceOrScalar, bool] = False, name: str = 'df',
               ) -> Union[pd.DataFrame, Tuple[pd.DataFrame, List]]:
@@ -400,15 +410,16 @@
     :return: pandas DataFrame
     """
 
     try:
         df = pd.DataFrame(df).copy()
     except Exception as _e:
         print(f"{_e.__class__.__name__}: {_e}")
-        raise ValueError(f"{name} must be a DataFrame or castable to DataFrame")
+        raise ValueError(
+            f"{name} must be a DataFrame or castable to DataFrame")
 
     if isinstance(groupby, bool) and not groupby:
         return df
     elif groupby is None or groupby in [[], GROUPBY_DUMMY, [GROUPBY_DUMMY]]:
         groupby = [GROUPBY_DUMMY]
         df[GROUPBY_DUMMY] = 1
     else:
@@ -493,15 +504,16 @@
             elif (df[_col] > 0).all():
                 _downcast = 'unsigned'
             else:
                 _downcast = 'signed'
             df = _do_downcast(df=df, cols=_col, downcast=_downcast)
 
     if c_float:
-        df = _do_downcast(df=df, cols=df.select_dtypes(include=['float']).columns, downcast='float')
+        df = _do_downcast(df=df, cols=df.select_dtypes(
+            include=['float']).columns, downcast='float')
 
     if c_cat:
         _include = ['object']
         if _pandas_version_1_plus:
             _include += ['string']
         for _col in df.select_dtypes(include=_include).columns:
             # if there are less than 1 - cat_frac unique elements: cast to category
@@ -546,20 +558,23 @@
 
     # -- main
     # init df as list of dfs
     _df_corr = []
     # loop groups
     for _index, _df_i in df.groupby(groupby):
         # get corr
-        _df_corr_i = _df_i.corr().reset_index().rename({'index': 'col_0'}, axis=1)
+        _df_corr_i = _df_i.corr().reset_index().rename(
+            {'index': 'col_0'}, axis=1)
         # set upper right half to nan
         for _i, _col in enumerate(columns):
-            _df_corr_i[_col] = np.where(_df_corr_i[_col].index <= _i, np.nan, _df_corr_i[_col])
+            _df_corr_i[_col] = np.where(
+                _df_corr_i[_col].index <= _i, np.nan, _df_corr_i[_col])
         # gather / melt
-        _df_corr_i = pd.melt(_df_corr_i, id_vars=['col_0'], var_name='col_1', value_name='corr').dropna()
+        _df_corr_i = pd.melt(_df_corr_i, id_vars=[
+                             'col_0'], var_name='col_1', value_name='corr').dropna()
         # drop self correlation
         _df_corr_i = _df_corr_i[_df_corr_i['col_0'] != _df_corr_i['col_1']]
         # get identifier
         for _groupby in groupby:
             _df_corr_i[_groupby] = _df_i[_groupby].iloc[0]
         # append to list of dfs
         _df_corr.append(_df_corr_i)
@@ -573,23 +588,26 @@
         # move groupby columns to front
         _df_corr = col_to_front(_df_corr, groupby)
 
     # reorder and keep only columns involving the target (if applicable)
     if target is not None:
         # if the target is col_1: switch it to col_0
         _target_is_col_1 = (_df_corr['col_1'] == target)
-        _df_corr['col_1'] = np.where(_target_is_col_1, _df_corr['col_0'], _df_corr['col_1'])
-        _df_corr['col_0'] = np.where(_target_is_col_1, target, _df_corr['col_0'])
+        _df_corr['col_1'] = np.where(
+            _target_is_col_1, _df_corr['col_0'], _df_corr['col_1'])
+        _df_corr['col_0'] = np.where(
+            _target_is_col_1, target, _df_corr['col_0'])
         # keep only target in col_0
         _df_corr = _df_corr[_df_corr['col_0'] == target]
 
     # get absolute correlation
     _df_corr['corr_abs'] = np.abs(_df_corr['corr'])
     # sort descending
-    _df_corr = _df_corr.sort_values(['corr_abs'], ascending=False).reset_index(drop=True)
+    _df_corr = _df_corr.sort_values(
+        ['corr_abs'], ascending=False).reset_index(drop=True)
 
     return _df_corr
 
 
 @export
 def drop_zero_cols(df: pd.DataFrame) -> pd.DataFrame:
     """
@@ -694,19 +712,20 @@
         _df_grouped = df.groupby(groupby)
 
         # use interpolation to treat missing values
         df[col] = _df_grouped[col].transform(pd.DataFrame.interpolate)
 
         # calculate delta (mean of diff to previous and next value)
         _delta = .5 * (
-                (df[col] - _df_grouped[col].shift(1).bfill()).abs() +
-                (df[col] - _df_grouped[col].shift(-1).ffill()).abs()
+            (df[col] - _df_grouped[col].shift(1).bfill()).abs() +
+            (df[col] - _df_grouped[col].shift(-1).ffill()).abs()
         )
 
-        df[col] = df[col].where((_delta - _df_grouped[col].mean()).abs() <= (std_cutoff * _df_grouped[col].std()))
+        df[col] = df[col].where(
+            (_delta - _df_grouped[col].mean()).abs() <= (std_cutoff * _df_grouped[col].std()))
 
     if GROUPBY_DUMMY in df.columns:
         df = df.drop(GROUPBY_DUMMY, axis=1)
 
     return df[col]
 
 
@@ -725,28 +744,30 @@
     :return: 1d numpy array containing the filtered data
     """
 
     def _f_butter_pass(_f_cutoff, _f_fs, _f_order, _f_btype):
         _nyq = 0.5 * _f_fs
         _normal_cutoff = _f_cutoff / _nyq
         # noinspection PyTupleAssignmentBalance
-        __b, __a = signal.butter(_f_order, _normal_cutoff, btype=_f_btype, analog=False, output='ba')
+        __b, __a = signal.butter(
+            _f_order, _normal_cutoff, btype=_f_btype, analog=False, output='ba')
 
         return __b, __a
 
     _data = np.array(data)
 
     if shift:
         _shift = pd.Series(data).iloc[0]
     else:
         _shift = 0
 
     _data -= _shift
 
-    _b, _a = _f_butter_pass(_f_cutoff=cutoff, _f_fs=fs, _f_order=order, _f_btype=btype)
+    _b, _a = _f_butter_pass(_f_cutoff=cutoff, _f_fs=fs,
+                            _f_order=order, _f_btype=btype)
 
     _y = signal.lfilter(_b, _a, _data)
 
     _y = _y + _shift
 
     return _y
 
@@ -858,20 +879,22 @@
         if _w is not None:
             _w_idx = _w[_idx]
         else:
             _w_idx = None
 
         if catch_error:
             try:
-                _fit = np.poly1d(np.polyfit(x=_x[_idx], y=_y[_idx], deg=1, w=_w_idx))
+                _fit = np.poly1d(np.polyfit(
+                    x=_x[_idx], y=_y[_idx], deg=1, w=_w_idx))
             except Exception as _exc:
                 warnings.warn('handled exception: {}'.format(_exc))
                 _fit = None
         else:
-            _fit = np.poly1d(np.polyfit(x=_x[_idx], y=_y[_idx], deg=1, w=_w_idx))
+            _fit = np.poly1d(np.polyfit(
+                x=_x[_idx], y=_y[_idx], deg=1, w=_w_idx))
 
         _x_diff = _x.diff().mean()
         _x = list(_x)
         _y = list(_y)
 
         if _fit is None:
             _y_fit = _y
@@ -996,15 +1019,16 @@
     _filter_iloc = _filter_df.iloc[0]
 
     # create a dummy boolean of all trues with len of df
     _filter_condition = (_df.index == _df.index)
 
     # logical and filter for all columns in filter df
     for _col in _filter_df.columns:
-        _filter_condition = _filter_condition & (_df[_col] == _filter_iloc[_col])
+        _filter_condition = _filter_condition & (
+            _df[_col] == _filter_iloc[_col])
 
     # create filtered df
     _df = _df[_filter_condition]
 
     # remove_unused_categories
     if rem_unused_categories:
         _df = remove_unused_categories(_df)
@@ -1065,15 +1089,16 @@
         else:
             __q_max_adj = __q_max
             _right_equal_sign = '<'
 
         _q_name = 'q{}: {}<=_{}{}'.format(_i, round_signif(__q_min, signif), _right_equal_sign,
                                           round_signif(__q_max, signif))
 
-        _s_out = np.where((_s >= __q_min) & (_s < __q_max_adj), _q_name, _s_out)
+        _s_out = np.where((_s >= __q_min) & (
+            _s < __q_max_adj), _q_name, _s_out)
 
     # get back the old properties of the series (or you'll screw the index)
     _s_out = pd.Series(_s_out)
     _s_out.name = s.name
     _s_out.index = s.index
 
     # convert to cat
@@ -1186,24 +1211,23 @@
         .pivot_table(index=y_true, columns=y_pred, values='_count')
     _cm = _cm.fillna(0).astype(int)
 
     return _cm
 
 
 @export
-def f1_pr(y_true: Union[pd.Series, str], y_pred: Union[pd.Series, str], df: pd.DataFrame = None, target: str = None,
-          factor: int = 100) -> pd.DataFrame:
+def f1_pr(y_true: Union[pd.Series, str], y_pred: Union[pd.Series, str], df: pd.DataFrame = None, target: str = None
+          ) -> pd.DataFrame:
     """
     get f1 score, true positive, true negative, missed positive and missed negative rate
 
     :param y_true: true values as name of df or vector data
     :param y_pred: predicted values as name of df or vector data
     :param df: pandas DataFrame containing true and predicted values [optional]
     :param target: level for which to return the rates, by default all levels are returned [optional]
-    :param factor: factor by which to scale results, default 100 [optional]
     :return: pandas DataFrame containing f1 score, true positive, true negative, missed positive
         and missed negative rate
     """
     if df is None:
 
         _y_true = deepcopy(y_true)
         _y_pred = deepcopy(y_pred)
@@ -1244,21 +1268,14 @@
         if _target in _cm.index:
             _count_true = _cm.loc[_target].sum()
         else:
             _count_true = 0
 
         _count_true_sum += _count_true
 
-        if _target in _cm.columns:
-            _count_pred = _cm[_target].sum()
-        else:
-            _count_pred = 0
-
-        _perc_pred = _count_pred / _count_true * factor
-
         # true positive: out of predicted as target how many are actually target
         try:
             _tp_i = _cm[_target][_target]
             _tp_sum += _tp_i
         except ValueError:
             _tp_i = np.nan
         # false positive: out of predicted as not target how many are actually not target
@@ -1292,15 +1309,16 @@
             _recall = _tp_i / (_tp_i + _mp_i) * 100
         except ValueError:
             _recall = np.nan
 
         if np.isnan(_precision) or np.isnan(_recall):
             _f1 = np.nan
         else:
-            _f1 = 200 * (_precision / 100. * _recall / 100.) / (_precision / 100. + _recall / 100.)
+            _f1 = 200 * (_precision / 100. * _recall / 100.) / \
+                (_precision / 100. + _recall / 100.)
 
         # to df
         _cm_target = pd.DataFrame({
             y_true: [_target], 'count': [_count_true], 'F1': [_f1], 'precision': [_precision], 'recall': [_recall]
         }).copy()
 
         _f1_pr.append(_cm_target)
@@ -1339,15 +1357,16 @@
         _y_true = assert_scalar(y_true)
         _y_pred = assert_scalar(y_pred)
 
         _df = df.copy()
         del df
 
     if dropna:
-        _df = _df.replace(np.inf, np.nan).replace(-np.inf, np.nan).dropna(subset=[_y_true, _y_pred])
+        _df = _df.replace(np.inf, np.nan).replace(-np.inf,
+                                                  np.nan).dropna(subset=[_y_true, _y_pred])
         if groupby is not None:
             _df = _df.dropna(subset=groupby)
     if _df.shape[0] == 0:
         return np.nan
 
     if groupby is None:
 
@@ -1493,29 +1512,31 @@
         # return
         return _score
     # return f_score
     return f_score(*args, f=_mpae, **kwargs)
 
 
 def pae(*args, **kwargs):
-    warnings.warn('pae is deprecated, please use mpae instead', DeprecationWarning)
+    warnings.warn('pae is deprecated, please use mpae instead',
+                  DeprecationWarning)
     return mpae(*args, **kwargs)
 
 
 @export
 def corr(*args, **kwargs) -> Union[pd.DataFrame, float]:
     """
     wrapper for f_score using pandas.Series.corr
 
     :param args: passed to f_score
     :param kwargs: passed to f_score
     :return: if groupby is supplied: pandas DataFrame, else: scalar value
     """
 
-    def _f_corr(x, y): return pd.Series(x).corr(other=pd.Series(y))
+    def _f_corr(x, y):
+        return pd.Series(x).corr(other=pd.Series(y))
 
     return f_score(*args, f=_f_corr, **kwargs)
 
 
 @export
 def df_score(df: pd.DataFrame, y_true: SequenceOrScalar, y_pred: SequenceOrScalar = None, pred_suffix: list = None,
              scores: List[Callable] = None, pivot: bool = True, scale: Union[dict, list, int] = None,
@@ -1559,15 +1580,16 @@
         scores = assert_list(scores)
         # str to function
         for _score in scores:
             if isinstance(_score, str):
                 if _score in _score_dict.keys():
                     _score = _score_dict[_score]
                 else:
-                    raise ValueError(f"Unknown score label: '{_score}', please pass a function instead")
+                    raise ValueError(
+                        f"Unknown score label: '{_score}', please pass a function instead")
     df = assert_df(df)
 
     if groupby:
         groupby = assert_list(groupby)
     else:
         groupby = [GROUPBY_DUMMY]
         df[GROUPBY_DUMMY] = 1
@@ -1587,15 +1609,16 @@
     else:
         y_pred = assert_list(y_pred)
         # check if y_pred is longer than y_true
         if len(y_pred) > len(y_true):
             warnings.warn('y_pred is longer than y_true, trailing entries will be dropped. If one y_true belongs'
                           'to multiple y_pred please specify it multiple times')
         elif len(y_true) > len(y_pred):
-            warnings.warn('y_true is longer than y_pred, trailing entries will be dropped.')
+            warnings.warn(
+                'y_true is longer than y_pred, trailing entries will be dropped.')
 
     # -- init
     if dropna:
         df = df.dropna(subset=list_merge(y_true, y_pred))
     for _groupby in groupby:
         if df[_groupby].dtype.name == 'category':
             df[_groupby] = df[_groupby].cat.remove_unused_categories()
@@ -1603,26 +1626,26 @@
     if isinstance(scale, Mapping):
         for _y_true, _scale in scale.items():
             df[_y_true] *= _scale
             _index = y_true.index(_y_true)
             _y_pred = y_pred[_index]
             df[_y_pred] *= _scale
     elif is_list_like(scale):
-        _i = -1
         for _scale, _y_true, _y_pred in zip(scale, y_true, y_pred):
             df[_y_true] *= _scale
             df[_y_pred] *= _scale
     elif scale is not None:
         for _y_true in y_true:
             df[_y_true] *= scale
         for _y_pred in y_pred:
             df[_y_pred] *= scale
 
     # -- main
-    _df_score = dict_list(groupby + ['y_true', 'y_pred', 'y_ref', 'model', 'score', 'value'])
+    _df_score = dict_list(
+        groupby + ['y_true', 'y_pred', 'y_ref', 'model', 'score', 'value'])
 
     for _y_true, _y_pred in zip(y_true, y_pred):
 
         if _y_pred not in df.columns:
             raise KeyError(f"{_y_pred} not in columns")
 
         for _score in scores:
@@ -1642,15 +1665,16 @@
 
                 for _groupby_i in groupby:
                     _append_dict[_groupby_i] = _df_i[_groupby_i].iloc[0]
 
                 append_to_dict_list(_df_score, _append_dict)
 
     _df_score = pd.DataFrame(_df_score)
-    _df_score[['y_true', 'y_pred', 'score']] = _df_score[['y_true', 'y_pred', 'score']].astype(str)
+    _df_score[['y_true', 'y_pred', 'score']] = _df_score[[
+        'y_true', 'y_pred', 'score']].astype(str)
     _df_score['value'] = _df_score['value'].astype(float)
 
     if _df_score.shape[0] == 0:
         raise ValueError("df_score is empty")
 
     _pivot_index = ['y_true', 'y_pred']
 
@@ -1659,15 +1683,16 @@
         _df_score[groupby] = _df_score[groupby].astype(str)
     else:
         _df_score = _df_score.drop([GROUPBY_DUMMY], axis=1)
 
     if pivot:
         _columns = _pivot_index + ['score', 'value']
         _df_score = _df_score[_columns]
-        _df_score = pd.pivot_table(_df_score, index=_pivot_index, columns='score', values='value')
+        _df_score = pd.pivot_table(
+            _df_score, index=_pivot_index, columns='score', values='value')
 
     return _df_score
 
 
 @export
 def rmsd(x: str, df: pd.DataFrame, group: str, return_df_paired: bool = False, agg_func: str = 'median',
          standardize: bool = False, to_abs: bool = False) -> Union[float, pd.DataFrame]:
@@ -1701,16 +1726,18 @@
     _df = _df.groupby([group]).agg({x: ['count', agg_func]}).reset_index()
     _df.columns = ['group', 'count', _agg_by_group]
     _df['dummy'] = 1
 
     _df_paired = pd.merge(_df, _df, on='dummy')
     _df_paired = _df_paired[_df_paired['group_x'] != _df_paired['group_y']]
     _df_paired['weight'] = _df_paired['count_x'] * _df_paired['count_y']
-    _df_paired['difference'] = _df_paired[_agg_by_group + '_x'] - _df_paired[_agg_by_group + '_y']
-    _df_paired['weighted_squared_difference'] = _df_paired['weight'] * _df_paired['difference'] ** 2
+    _df_paired['difference'] = _df_paired[_agg_by_group + '_x'] - \
+        _df_paired[_agg_by_group + '_y']
+    _df_paired['weighted_squared_difference'] = _df_paired['weight'] * \
+        _df_paired['difference'] ** 2
 
     if return_df_paired:
         return _df_paired
     else:
         return np.sqrt(_df_paired['weighted_squared_difference'].sum() / _df_paired['weight'].sum())
 
 
@@ -1797,25 +1824,28 @@
 
                 if include_rmsd:
                     _rmsd = rmsd(x=_x, df=_df_hue, group='_group', **kwargs)
                 else:
                     _rmsd = np.nan
 
                 _count = len(_df_hue['_group'])
-                _maxcount = _df_hue['_group'].value_counts().reset_index()['_group'].iloc[0]
+                _maxcount = _df_hue['_group'].value_counts().reset_index()[
+                    '_group'].iloc[0]
                 _maxperc = _maxcount / _count
-                _maxlevel = _df_hue['_group'].value_counts().reset_index()['index'].iloc[0]
+                _maxlevel = _df_hue['_group'].value_counts().reset_index()[
+                    'index'].iloc[0]
 
                 _df_rmsd_hue = pd.DataFrame(
                     {'x': _x, 'group': _group, 'rmsd': _rmsd, 'maxperc': _maxperc, 'maxlevel': _maxlevel,
                      'maxcount': _maxcount, 'count': _count}, index=[0])
                 if hue is not None:
                     _df_rmsd_hue[hue] = _hue
 
-                _df_rmsd = _df_rmsd.append(_df_rmsd_hue, ignore_index=True, sort=False)
+                _df_rmsd = _df_rmsd.append(
+                    _df_rmsd_hue, ignore_index=True, sort=False)
 
     # postprocessing, sorting etc.
     if hue is not None:
 
         _df_rmsd[hue] = _df_rmsd[hue].astype('category')
 
         if hue_order is not None:
@@ -1824,19 +1854,22 @@
             _hues = _df_rmsd[hue].cat.categories
 
         _df_order = _df_rmsd[_df_rmsd[hue] == _hues[0]].sort_values(by=['rmsd'], ascending=False).reset_index(
             drop=True).reset_index().rename({'index': '_order'}, axis=1)[['group', '_order']]
         _df_rmsd = pd.merge(_df_rmsd, _df_order)
 
         if sort_by_hue:
-            _df_rmsd = _df_rmsd.sort_values(by=[hue, '_order']).reset_index(drop=True).drop(['_order'], axis=1)
+            _df_rmsd = _df_rmsd.sort_values(by=[hue, '_order']).reset_index(
+                drop=True).drop(['_order'], axis=1)
         else:
-            _df_rmsd = _df_rmsd.sort_values(by=['_order', hue]).reset_index(drop=True).drop(['_order'], axis=1)
+            _df_rmsd = _df_rmsd.sort_values(by=['_order', hue]).reset_index(
+                drop=True).drop(['_order'], axis=1)
     else:
-        _df_rmsd = _df_rmsd.sort_values(by=['rmsd'], ascending=False).reset_index(drop=True)
+        _df_rmsd = _df_rmsd.sort_values(
+            by=['rmsd'], ascending=False).reset_index(drop=True)
 
     return _df_rmsd
 
 
 @export
 def df_p(x: str, group: str, df: pd.DataFrame, hue: str = None, agg_func: str = 'mean', agg: bool = False,
          n_quantiles: int = 10):
@@ -1890,15 +1923,16 @@
                 else:
 
                     _df_dict[group] = _level_1
                     _df_dict[group + '_2'] = _level_2
 
                 _df_dict['p'] = _p
 
-                _df_p = _df_p.append(pd.DataFrame(_df_dict, index=[0]), ignore_index=True, sort=False)
+                _df_p = _df_p.append(pd.DataFrame(
+                    _df_dict, index=[0]), ignore_index=True, sort=False)
 
     if agg:
         _df_p = _df_p.groupby(_groupby).agg({'p': 'mean'}).reset_index()
 
     return _df_p
 
 
@@ -1917,24 +1951,27 @@
 
     if hue is not None:
         _hue = '_hue'
     else:
         _hue = None
 
     # get agg
-    _df_agg = _df.groupby(_groupby).agg({'_dummy': 'count', x: agg}).reset_index()
+    _df_agg = _df.groupby(_groupby).agg(
+        {'_dummy': 'count', x: agg}).reset_index()
     _df_agg.columns = _groupby + ['count'] + agg
     if sort_by_count:
         _df_agg = _df_agg.sort_values(by=['count'], ascending=False)
 
     if p:
-        _df_p = df_p(x=x, group='_group', hue=_hue, df=_df, agg_func=p_test, agg=True)
+        _df_p = df_p(x=x, group='_group', hue=_hue,
+                     df=_df, agg_func=p_test, agg=True)
         _df_agg = pd.merge(_df_agg, _df_p, on=_groupby)
 
-    _df_agg.columns = _groupby_names + [_col for _col in _df_agg.columns if _col not in _groupby]
+    _df_agg.columns = _groupby_names + \
+        [_col for _col in _df_agg.columns if _col not in _groupby]
 
     return _df_agg
 
 
 # quick function to adjust group and hue to be categorical
 def df_group_hue(df, group, hue=None, x=None, n_quantiles=10, na_to_med=False, keep=True):
     _df = df.copy()
@@ -1973,28 +2010,32 @@
     _df[_group] = _df[group].copy()
     if hue is not None:
         _df[_hue] = _df[hue].copy()
 
     # - numeric to quantile
     # group
     if _group in list(_df.select_dtypes(include=np.number)):
-        _df[_group] = quantile_split(_df[group], n_quantiles, na_to_med=na_to_med)
+        _df[_group] = quantile_split(
+            _df[group], n_quantiles, na_to_med=na_to_med)
     _df[_group] = _df[_group].astype('category').cat.remove_unused_categories()
 
     # hue
     if hue is not None:
         if _hue in list(_df.select_dtypes(include=np.number)):
-            _df[_hue] = quantile_split(_df[hue], n_quantiles, na_to_med=na_to_med)
+            _df[_hue] = quantile_split(
+                _df[hue], n_quantiles, na_to_med=na_to_med)
         _df[_hue] = _df[_hue].astype('category').cat.remove_unused_categories()
         _df['_label'] = concat_cols(_df, [_group, _hue]).astype('category')
-        _df_levels = _df[[_group, _hue, '_label']].drop_duplicates().reset_index(drop=True)
+        _df_levels = _df[[_group, _hue, '_label']
+                         ].drop_duplicates().reset_index(drop=True)
         _levels = _df_levels['_label']
     else:
         _df['_label'] = _df[_group]
-        _df_levels = _df[[_group, '_label']].drop_duplicates().reset_index(drop=True)
+        _df_levels = _df[[_group, '_label']
+                         ].drop_duplicates().reset_index(drop=True)
         _levels = _df_levels['_label']
 
     return _df, _groupby, _groupby_names, _vars, _df_levels, _levels
 
 
 def order_cols(df, cols):
     return df[cols + [_col for _col in df.columns if _col not in cols]]
@@ -2002,15 +2043,14 @@
 
 def df_precision_filter(df, col, precision):
     return df[(np.abs(df[col] - df[col].round(precision)) < (1 / (2 * 10 ** (precision + 1))))]
 
 
 # grouped iterpolate method (avoids .apply failing if one sub group fails)
 def grouped_interpolate(df, col, groupby, method=None):
-    _df = df.copy()
 
     _dfs_i = []
 
     for _index_i, _df_i in df.groupby(groupby):
 
         try:
             _df_i[col] = _df_i[col].interpolate(method=method)
@@ -2124,22 +2164,24 @@
 
         # calculate y fit
         _df_t[_y_fit] = _y_int_i + _df_t[_t_i] * _y_slope_i
 
         _df_phases[_y_slope][_i] = _y_slope_i
         _df_phases[_y_int][_i] = _y_int_i
         _df_phases[_y_r2][_i] = r2_score(_df_t[y], _df_t[_y_fit])
-        _df_phases[_y_rmse][_i] = np.sqrt(mean_squared_error(_df_t[y], _df_t[_y_fit]))
+        _df_phases[_y_rmse][_i] = np.sqrt(
+            mean_squared_error(_df_t[y], _df_t[_y_fit]))
 
         _dfs.append(_df_t)
 
     _df_fit = pd.concat(_dfs)
 
     # postprocessing
-    _df_phases = _df_phases[_df_phases['_keep']].reset_index(drop=True).drop(['_keep'], axis=1)
+    _df_phases = _df_phases[_df_phases['_keep']].reset_index(
+        drop=True).drop(['_keep'], axis=1)
 
     if return_df_fit:
         return _df_fit
     else:
         return _df_phases
 
 
@@ -2275,15 +2317,16 @@
         _dfs = {}
 
     for _i, _df in df.groupby(_split_by):
 
         if return_type == 'list':
             _dfs.append(_df)
         else:
-            _key = qformat(pd.DataFrame(_df[_split_by]).head(1), print_key=print_key, sep=sep, key_sep=key_sep)
+            _key = qformat(pd.DataFrame(_df[_split_by]).head(
+                1), print_key=print_key, sep=sep, key_sep=key_sep)
             _dfs[_key] = _df
 
     return _dfs
 
 
 # concats a df, wrapper for pandas.concat
 def concat(obj, ignore_index=True, sort=False, **kwargs):
@@ -2320,15 +2363,16 @@
     # -- main
     # save row
     df[ROW_DUMMY] = range(df.shape[0])
     # handle ascending
     if sortby_ascending is None:
         _ascending = rank_ascending
     else:
-        _ascending = assert_list(rank_ascending) + [True for _ in groupby] + assert_list(sortby_ascending)
+        _ascending = assert_list(
+            rank_ascending) + [True for _ in groupby] + assert_list(sortby_ascending)
     # sort
     _by = rankby + groupby + sortby
     df = df.sort_values(by=_by, ascending=_ascending).assign(rank=1)
     # rank
     df['__rank__'] = df.groupby(groupby)['rank'].cumsum()
     # sort back to original row order
     df = df.sort_values(by=ROW_DUMMY)
@@ -2341,15 +2385,16 @@
     if df is not None:
 
         _df = df.copy()
         del df
 
         if x in ['value', 'perc', 'diff', 'sign', 'ex', 'ex_max', 'ex_min', 'mean', 'std', 'range',
                  'value_min', 'value_max', 'range_min', 'range_max']:
-            raise ValueError('x cannot be named {}, please rename your variable'.format(x))
+            raise ValueError(
+                'x cannot be named {}, please rename your variable'.format(x))
     else:
         _df = None
 
     # std cutoff = norm(0,1).pdf(1)/norm(0,1).pdf(0)
     # 1/e cutoff: range_cutoff = 1-1/e = .63
     # full width at half maximum: range_cutoff = .5
     if range_cutoff is None or range_cutoff in ['sigma', 'std']:
@@ -2370,16 +2415,14 @@
             _x_name = x.name
         else:
             _x_name = 'x'
 
     assert (len(_x) > 0), 'Series {} has zero length'.format(_x_name)
     _x = pd.Series(_x).reset_index(drop=True)
 
-    _x_name_max = f"{_x_name }_max"
-
     if x_range is None:
         x_range = np.linspace(np.nanmin(_x), np.nanmax(_x), x_steps)
 
     # -- fit kde
     _kde = stats.gaussian_kde(_x)
 
     # -- to df
@@ -2390,32 +2433,35 @@
     _df_kde['diff'] = _df_kde['value'].diff()
     _df_kde['sign'] = np.sign(_df_kde['diff'])
     _df_kde['ex_max'] = _df_kde['sign'].diff(-1).fillna(0) > 0
     _df_kde['ex_min'] = _df_kde['sign'].diff(-1).fillna(0) < 0
     _df_kde['phase'] = _df_kde['ex_min'].astype(int).cumsum()
 
     if perc_cutoff:
-        _df_kde['ex_max'] = _df_kde['ex_max'].where(_df_kde['perc'] > perc_cutoff, False)
+        _df_kde['ex_max'] = _df_kde['ex_max'].where(
+            _df_kde['perc'] > perc_cutoff, False)
 
     # -- get std
     # we get the extrema and do a full merge to find the closest one to each point
-    _df_kde_ex = _df_kde.query('ex_max')[[_x_name, 'value', 'phase']].reset_index()
+    _df_kde_ex = _df_kde.query(
+        'ex_max')[[_x_name, 'value', 'phase']].reset_index()
     _df_kde_ex['mean'] = np.nan
     _df_kde_ex['std'] = np.nan
     _df_kde_ex['range'] = np.nan
     _df_kde_ex['range_min'] = np.nan
     _df_kde_ex['range_max'] = np.nan
     _df_kde_ex['value_min'] = np.nan
     _df_kde_ex['value_max'] = np.nan
 
     for _index, _row in _df_kde_ex.iterrows():
         _df_kde_i = _df_kde[_df_kde['phase'] == _row['phase']]
 
         # Width of Peak range
-        _df_kde_i = _df_kde_i[_df_kde_i['value'] >= _row['value'] * _range_cutoff]
+        _df_kde_i = _df_kde_i[_df_kde_i['value']
+                              >= _row['value'] * _range_cutoff]
 
         _x_min = _df_kde_i[_x_name].iloc[0]
         _x_max = _df_kde_i[_x_name].iloc[-1]
 
         _x_i = np.extract((_x > _x_min) & (_x < _x_max), _x)
 
         _mean, _std = stats.norm.fit(_x_i)
@@ -2436,15 +2482,16 @@
 def qagg(df: pd.DataFrame, groupby, columns=None, agg=None, reset_index=True):
     if agg is None:
         agg = ['mean', 'std']
     if columns is None:
         columns = df.select_dtypes(include=np.number).columns
 
     _df_agg = df.groupby(groupby).agg({_: agg for _ in columns})
-    _df_agg = _df_agg.set_axis(flatten([[_ + '_mean', _ + '_std'] for _ in columns]), axis=1, inplace=False)
+    _df_agg = _df_agg.set_axis(
+        flatten([[_ + '_mean', _ + '_std'] for _ in columns]), axis=1, inplace=False)
     if reset_index:
         _df_agg = _df_agg.reset_index()
     return _df_agg
 
 
 @export
 def mahalanobis(point: Union[pd.DataFrame, pd.Series, np.ndarray], df: pd.DataFrame = None, params: List[str] = None,
@@ -2508,19 +2555,23 @@
 
     _df = df.copy()
     del df
 
     _df_out = []
 
     for _col in cols:
-        _value_vars = ['{}{}{}'.format(_col, sep, _suffix) for _suffix in suffixes]
+        _value_vars = ['{}{}{}'.format(_col, sep, _suffix)
+                       for _suffix in suffixes]
 
-        _df_out_i = _df.melt(id_vars=id_vars, value_vars=_value_vars, value_name=_col, var_name=var_name, **kwargs)
-        _df_out_i[var_name] = _df_out_i[var_name].str.slice(len(_col) + len(sep))
-        _df_out_i = _df_out_i.sort_values(by=assert_list(id_vars) + [var_name]).reset_index(drop=True)
+        _df_out_i = _df.melt(id_vars=id_vars, value_vars=_value_vars,
+                             value_name=_col, var_name=var_name, **kwargs)
+        _df_out_i[var_name] = _df_out_i[var_name].str.slice(
+            len(_col) + len(sep))
+        _df_out_i = _df_out_i.sort_values(by=assert_list(
+            id_vars) + [var_name]).reset_index(drop=True)
         _df_out.append(_df_out_i)
 
     _df_out = pd.concat(_df_out, axis=1).pipe(drop_duplicate_cols)
 
     return _df_out
 
 
@@ -2557,15 +2608,16 @@
         _df = _df.sum()
     else:
         _df = _df.agg({_: agg for _ in _columns})
         if adj_column_names:
             _adj_column_names = True
 
     # back to int
-    _df.index = ((_df.index - pd.to_datetime('1970-01-01')).total_seconds() / factor)
+    _df.index = ((_df.index - pd.to_datetime('1970-01-01')
+                  ).total_seconds() / factor)
     if _adj_column_names:
         _column_names = []
         for _col in _columns:
             for _agg in assert_list(agg):
                 _column_names += ['{}_{}'.format(_col, _agg)]
         _df.columns = _column_names
 
@@ -2631,16 +2683,18 @@
         if x_max is None:
             x_max = df[x].max()
         _df_xs = pd.DataFrame({x: range(x_min, x_max, x_base)})
         _xs_on = [x]
 
         # init hues
         if hue is not None:
-            _df_hues = df[[hue]].drop_duplicates().reset_index().assign(_dummy=1)
-            _df_xs = pd.merge(_df_xs.assign(_dummy=1), _df_hues, on='_dummy').drop(['_dummy'], axis=1)
+            _df_hues = df[[hue]].drop_duplicates(
+            ).reset_index().assign(_dummy=1)
+            _df_xs = pd.merge(_df_xs.assign(_dummy=1), _df_hues,
+                              on='_dummy').drop(['_dummy'], axis=1)
             _xs_on = _xs_on + [hue]
 
     else:
         # apply x limits (ignored if not numeric)
         if x in df.select_dtypes(np.number):
             if x_min:
                 df[x] = df[x].where(lambda _: _ >= x_min, x_min)
@@ -2650,25 +2704,28 @@
     # to string
     df[x] = df[x].astype(str)
     if hue is not None:
         df[hue] = df[hue].astype(str)
 
     # if applicable: apply top_n_coding (both x and hue)
     if top_nr:
-        df[x] = top_n_coding(s=df[x], n=top_nr, other_name=other_name, other_to_na=other_to_na)
+        df[x] = top_n_coding(
+            s=df[x], n=top_nr, other_name=other_name, other_to_na=other_to_na)
         if hue is not None:
-            df[hue] = top_n_coding(s=df[hue], n=top_nr, other_name=other_name, other_to_na=other_to_na)
+            df[hue] = top_n_coding(
+                s=df[hue], n=top_nr, other_name=other_name, other_to_na=other_to_na)
 
     # init groupby
     _groupby = [x]
     if hue is not None:
         _groupby = _groupby + [hue]
 
     # we use a dummy column called count and sum over it by group to retain the original x column values
-    _df_count = df.assign(count=1).groupby(_groupby).agg({'count': 'sum'}).reset_index()
+    _df_count = df.assign(count=1).groupby(
+        _groupby).agg({'count': 'sum'}).reset_index()
 
     # if applicable: append 0 entries for numerical x inside x_range
     if x_base:
         # was already called with same if before
         # noinspection PyUnboundLocalVariable
         _df_count = pd.merge(_df_count, _df_xs, on=_xs_on, how='outer')
         _df_count['count'] = _df_count['count'].fillna(0)
@@ -2677,24 +2734,29 @@
     _count_x = 'count_{}'.format(x)
     _count_hue = 'count_{}'.format(hue)
 
     if hue is None:
         _df_count[_count_hue] = _df_count['count'].sum()
         _df_count[_count_x] = _df_count['count']
     else:
-        _df_count[_count_x] = _df_count.groupby(x)['count'].transform(pd.Series.sum)
-        _df_count[_count_hue] = _df_count.groupby(hue)['count'].transform(pd.Series.sum)
+        _df_count[_count_x] = _df_count.groupby(
+            x)['count'].transform(pd.Series.sum)
+        _df_count[_count_hue] = _df_count.groupby(
+            hue)['count'].transform(pd.Series.sum)
 
     # sort
     if sort_by_count:
-        _df_count = _df_count.sort_values([_count_x], ascending=False).reset_index(drop=True)
+        _df_count = _df_count.sort_values(
+            [_count_x], ascending=False).reset_index(drop=True)
 
     # add perc columns
-    _df_count[f"perc_{x}"] = np.round(_df_count['count'] / _df_count[_count_x] * 100, 2)
-    _df_count[f"perc_{hue}"] = np.round(_df_count['count'] / _df_count[_count_hue] * 100, 2)
+    _df_count[f"perc_{x}"] = np.round(
+        _df_count['count'] / _df_count[_count_x] * 100, 2)
+    _df_count[f"perc_{hue}"] = np.round(
+        _df_count['count'] / _df_count[_count_hue] * 100, 2)
 
     return _df_count
 
 
 # return prediction accuracy in percent
 def get_accuracy(class_true, class_pred):
     return np.where(class_true.astype(str) == class_pred.astype(str), 1, 0).sum() / len(class_true)
@@ -2706,15 +2768,17 @@
     outer_limit = int(outer_limit)
 
     # make a copy to avoid inplace effects
     _series = pd.Series(deepcopy(pd_series))
 
     # use standard scaler to center around mean with std +- 1
     if use_standard_scaler:
-        _series = StandardScaler().fit(_series.values.reshape(-1, 1)).transform(_series.values.reshape(-1, 1)).flatten()
+        # noinspection PyUnresolvedReferences
+        _series = StandardScaler().fit(_series.values.reshape(-1, 1)
+                                       ).transform(_series.values.reshape(-1, 1)).flatten()
 
     # if step is none: use 1 as step
     if step is None:
         step = 1
     if suffix is None:
         if use_standard_scaler:
             suffix = 'std'
@@ -2728,29 +2792,27 @@
     if use_abs:
         _series = np.abs(_series)
     else:
         # gather the +0 and -0 group to 0
         _series = np.where(np.abs(_series) < step, 0, _series)
 
     # group
-
-    # get sign
-    _series_sign = np.sign(_series)
-
     # divide by step, floor and integer
-    _series = (np.floor(np.abs(_series) / step)).astype(int) * np.sign(_series).astype(int)
+    _series = (np.floor(np.abs(_series) / step)).astype(int) * \
+        np.sign(_series).astype(int)
 
     # apply outer limit
     if outer_limit is not None:
         _series = np.where(_series > outer_limit, outer_limit, _series)
         _series = np.where(_series < -outer_limit, -outer_limit, _series)
 
     # make a pretty string
     # noinspection PyTypeChecker
-    _series = pd.Series(_series).apply(lambda x: '{0:n}'.format(x)).astype('str') + suffix
+    _series = pd.Series(_series).apply(
+        lambda x: '{0:n}'.format(x)).astype('str') + suffix
 
     # to cat
     _series = _series.astype('category')
 
     return _series
 
 
@@ -2773,28 +2835,30 @@
     if isinstance(n, int) or str(n).isnumeric():
         n = int(n)
         if w is None:
             _df_count = pd.Series(s).value_counts().reset_index()
             return list(_df_count.sort_values(by=[_df_count.columns[1], 'index'], ascending=[False, True])['index'][:n])
         else:
             return pd.DataFrame({'s': s, 'w': w}).groupby('s').agg({'w': 'sum'}) \
-                       .sort_values(by='w', ascending=False).index.tolist()[:n]
+                .sort_values(by='w', ascending=False).index.tolist()[:n]
     # -- case str (percent)
     elif isinstance(n, str):
         if '%' not in n:
-            raise ValueError(f"Please specify n as integer or percent with percentage sign %")
+            raise ValueError(
+                "Please specify n as integer or percent with percentage sign %")
         n = float(n.split('%')[0]) / 100.
         _df = pd.DataFrame({'s': s})
         # get weights
         if w is None:
             _df['w'] = 1
         else:
             _df['w'] = w
         # sum weights
-        _df = _df.groupby('s').agg({'w': 'sum'}).reset_index().sort_values(by=['w', 's'], ascending=[False, True])
+        _df = _df.groupby('s').agg({'w': 'sum'}).reset_index(
+        ).sort_values(by=['w', 's'], ascending=[False, True])
         # calculate cutoff
         _df['c'] = _df['w'].cumsum() / _df['w'].sum()
         _df = _df[_df['c'].shift(1).fillna(0) <= n]
         _n_list = _df['s'].tolist()
         if n_max is not None and len(_n_list) > n_max:
             _n_list = _n_list[:n_max]
 
@@ -2872,20 +2936,21 @@
         # if k is list like then assume it is a lift of values to split at
         # check for sortby
         if sortby is None:
             raise ValueError(f"k={k} (string, datetime) requires sortby")
         # prepare output df
         _df_out = df.copy()
         # init k index on first k value
-        _df_out['_k_index'] = np.where(_df_out[sortby] < k[0], len(k)+1, len(k))
+        _df_out['_k_index'] = np.where(
+            _df_out[sortby] < k[0], len(k) + 1, len(k))
         # compare with the others
         for _k_index in range(1, len(k), 1):
             # the value has to be between the previous and this value
             _df_out['_k_index'] = np.where((_df_out[sortby] < k[_k_index]) & (_df_out[sortby] >= k[_k_index - 1]),
-                                           _k_index+1, _df_out['_k_index'])
+                                           _k_index + 1, _df_out['_k_index'])
     elif isinstance(k, (str, datetime)):
         # check for sortby
 
         if sortby is None:
             raise ValueError(f"k={k} (string, datetime) requires sortby")
         _df_out = df.copy()
         _df_out['_k_index'] = np.where(_df_out[sortby] < k, 1, 0)
@@ -2919,16 +2984,18 @@
         if GROUPBY_DUMMY in _df_out.columns:
             _df_out = _df_out.drop(GROUPBY_DUMMY, axis=1)
     # tprint
     if do_print:
         tprint('k_split done')
     # -- return
     if return_type in range(k):
-        _df_train = _df_out[_df_out['_k_index'] != return_type].drop('_k_index', axis=1)
-        _df_test = _df_out[_df_out['_k_index'] == return_type].drop('_k_index', axis=1)
+        _df_train = _df_out[_df_out['_k_index'] !=
+                            return_type].drop('_k_index', axis=1)
+        _df_test = _df_out[_df_out['_k_index'] ==
+                           return_type].drop('_k_index', axis=1)
         return _df_train, _df_test
     else:
         return _df_out['_k_index']
 
 
 @docstr
 @export
@@ -2976,14 +3043,15 @@
     with open(path.encode('utf-8'), 'r', encoding=encoding, errors=errors, **kws_open) as _f:
         if nrows:
             _csv = StringIO('\n'.join([next(_f) for _ in range(nrows + 1)]))
         else:
             _csv = StringIO(_f.read())
 
     # -- return
+    # noinspection PyTypeChecker
     return pd.read_csv(deepcopy(_csv), nrows=nrows, **kwargs)
 
 
 @docstr
 @export
 def get_columns(df: pd.DataFrame, dtype: Union[SequenceOrScalar, np.number] = None,
                 to_list: bool = False) -> Union[list, pd.Index]:
```

### Comparing `hhpy-0.3.0/hhpy/entry_points.py` & `hhpy-0.3.1/hhpy/entry_points.py`

 * *Files identical despite different names*

### Comparing `hhpy-0.3.0/hhpy/ipython.py` & `hhpy-0.3.1/hhpy/ipython.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,16 @@
      based on https://stackoverflow.com/questions/21971449/how-do-i-increase-the-cell-width-of-the-jupyter-
      ipython-notebook-in-my-browser
 
     :param: width in percent, default 90 [optional]
     :return: None
     """
     # noinspection PyTypeChecker
-    display(HTML('<style>.container { width:{}% !important; }</style>'.format(width)))
+    display(
+        HTML(f"<style>.container { width:{width}% !important; }</style>"))
 
 
 @export
 def hide_code():
     """
     hides the code and introduces a toggle button
      based on https://stackoverflow.com/questions/27934885/how-to-hide-code-from-cells-in-ipython-notebook-visualized
@@ -39,23 +40,23 @@
 
     :return: None
     """
 
     # noinspection PyTypeChecker
     display(HTML('''
         <script>
-        code_show=true; 
+        code_show=true;
         function code_toggle() {
          if (code_show){
          $('div.input').hide();
          } else {
          $('div.input').show();
          }
          code_show = !code_show
-        } 
+        }
         $( document ).ready(code_toggle);
         </script>
         The raw code for this IPython notebook is by default hidden for easier reading.
         To toggle on/off the raw code, click <a href="javascript:code_toggle()">here</a>.
     '''))
 
 
@@ -116,17 +117,19 @@
     # avoid inplace
     df = pd.DataFrame(df).copy()
 
     _cols_int = list_exclude(df.select_dtypes(int).columns, exclude)
     _cols_float = list_exclude(df.select_dtypes(float).columns, exclude)
 
     for _col in _cols_int:
-        df[_col] = df[_col].apply(lambda _: format(_, int_format) if not pd.isna(_) else '<NaN>')
+        df[_col] = df[_col].apply(lambda _: format(
+            _, int_format) if not pd.isna(_) else '<NaN>')
     for _col in _cols_float:
-        df[_col] = df[_col].apply(lambda _: format(_, float_format) if not pd.isna(_) else '<NaN>')
+        df[_col] = df[_col].apply(lambda _: format(
+            _, float_format) if not pd.isna(_) else '<NaN>')
 
     if full:
         display_full(df, **kwargs)
     else:
         display(df, **kwargs)
```

### Comparing `hhpy-0.3.0/hhpy/main.py` & `hhpy-0.3.1/hhpy/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,16 @@
         Converts self to a dictionary
 
         :recursive: Whether to recursively propagate to_dict to children
         :return: Dictionary
         """
 
         if len(self.__attributes__) == 0:
-            warnings.warn('self.__attributes__ has length zero, did you declare it?')
+            warnings.warn(
+                'self.__attributes__ has length zero, did you declare it?')
 
         _dict = {}
         for _attr_name in list_merge('__name__', self.__attributes__):
             _attr = self.__getattribute__(_attr_name)
 
             # - call to children's to_dict
             if recursive:
@@ -182,19 +183,21 @@
                     _kws['classes'] = _classes
                 # call sub-function
                 _attr_evaluated.from_dict(attr_value, **_kws)
 
             return _attr_evaluated
 
         # -- init
-        _classes = assert_list(self.__dependent_classes__, default=[]) + assert_list(classes, default=[])
+        _classes = assert_list(self.__dependent_classes__, default=[
+        ]) + assert_list(classes, default=[])
 
         # -- main
         if len(self.__attributes__) == 0:
-            warnings.warn('self.__attributes__ has length zero, did you declare it?')
+            warnings.warn(
+                'self.__attributes__ has length zero, did you declare it?')
 
         for _attr_name in list_merge('__name__', self.__attributes__):
             if _attr_name not in dct.keys():
                 continue
             _attr = dct[_attr_name]
 
             # - call to children's from_dict
@@ -202,20 +205,22 @@
                 if is_list_like(_attr):
                     if isinstance(_attr, Dict):  # Dict
                         if '__name__' in _attr.keys():
                             _attr = _f_eval(_attr['__name__'], _attr)  # eval
                         else:
                             for _attr_key, _attr_value in _attr.items():
                                 if isinstance(_attr_value, Dict) and '__name__' in _attr_value.keys():
-                                    _attr[_attr_key] = _f_eval(_attr_value['__name__'], _attr_value)  # eval
+                                    _attr[_attr_key] = _f_eval(
+                                        _attr_value['__name__'], _attr_value)  # eval
                     else:  # List
                         for _i in range(len(_attr)):
                             _attr_value = _attr[_i]
                             if isinstance(_attr_value, Mapping) and '__name__' in _attr_value.keys():
-                                _attr[_i] = _f_eval(_attr_value['__name__'], _attr_value)  # eval
+                                _attr[_i] = _f_eval(
+                                    _attr_value['__name__'], _attr_value)  # eval
 
             self.__setattr__(_attr_name, _attr)
         # -- return
         return self
 
     def to_pickle(self, filename: str):
         """
@@ -266,15 +271,16 @@
         # eval custom rules
         if rules is not None:
             for _type, _callable in rules.items():
                 if isinstance(value, _type) or (value == _type):
                     try:
                         __repr_i = _callable(value)
                     except Exception as _e:
-                        print(f"{_e.__class__.__name__}: {_e} handled for {value}")
+                        print(
+                            f"{_e.__class__.__name__}: {_e} handled for {value}")
 
         return __repr_i
 
     # -- assert
 
     # check if self.__name__ is still the same as Base (i.e. unset)
     # - name
@@ -288,18 +294,20 @@
     # - attributes
     if hasattr(obj, '__attributes__'):
         _attributes = obj.__attributes__
         # exclude attributes to be hidden in repr
         if hasattr(obj, '__attributes_no_repr__'):
             _attributes = list_exclude(_attributes, obj.__attributes_no_repr__)
     else:
-        warnings.warn('Object has no __attributes__ attribute, did you declare it?')
+        warnings.warn(
+            'Object has no __attributes__ attribute, did you declare it?')
         _attributes = []
     if len(obj.__attributes__) == 0:
-        warnings.warn('self.__attributes__ has length zero, did you declare it?')
+        warnings.warn(
+            'self.__attributes__ has length zero, did you declare it?')
     # - rules
     if rules is not None and not isinstance(rules, Mapping):
         raise ValueError('rules should be a dictionary of types and callables')
 
     # -- init
     _repr = f"{_name}("
     # iterator for separator handling
@@ -326,20 +334,21 @@
             _it += 1
             # add separator
             if _it > 0:
                 _repr += ', '
             # add to repr string
             _repr += f"{_attribute}={_repr_i}"
         else:
-            warnings.warn(f"{_attribute} is specified in self.__attributes__ but does not exist. Skipping...")
+            warnings.warn(
+                f"{_attribute} is specified in self.__attributes__ but does not exist. Skipping...")
             continue
     # close brace
     _repr += ')'
     # remove all \
-    _reprs = _repr.replace('\\', '').replace('\'', '')
+    _repr = _repr.replace('\\', '').replace('\'', '')
     # -- return
     return _repr
 
 
 # --- exported functions
 @export
 def today(date_format: str = '%Y_%m_%d') -> str:
@@ -440,15 +449,16 @@
 
     """
     global global_tprint_len
 
     _allowed_r_locs = ['front', 'end']
 
     if r_loc not in _allowed_r_locs:
-        warnings.warn(f'r_loc not in {_allowed_r_locs}, defaulting to {rcParams["tprint.r_loc"]}')
+        warnings.warn(
+            f'r_loc not in {_allowed_r_locs}, defaulting to {rcParams["tprint.r_loc"]}')
         r_loc = rcParams['tprint.r_loc']
 
     _string = ''
     _arg_len = 0
 
     for _arg in args:
 
@@ -644,32 +654,34 @@
     :param printf: Using tprint by default. Use fprint to write to file instead.
     :param persist: Whether to persist the progressbar after reaching 100 percent.
     :param kwargs: Passed to print function
     :return:
     """
     # -- assert
     if mode not in validations['progressbar__mode']:
-        raise ValueError(f"mode must be one of {validations['progressbar__mode']}")
+        raise ValueError(
+            f"mode must be one of {validations['progressbar__mode']}")
     # -- init
     _perc_f = i / i_max * 100
     _perc = int(np.floor(_perc_f))
-    _rem = 100 - _perc
     if len(print_prefix) > 0 and (print_prefix[-2:] != ': ') and (print_prefix[-1:] not in [':', '\n']):
         print_prefix += ": "
 
     # -- main
     if _perc <= 50:
 
         _right = empty_symbol * (50 // p_step)
-        _left = symbol * int(np.ceil(_perc / p_step)) + empty_symbol * ((50 - _perc) // p_step)
+        _left = symbol * int(np.ceil(_perc / p_step)) + \
+            empty_symbol * ((50 - _perc) // p_step)
 
     else:
 
         _left = symbol * (50 // p_step)
-        _right = symbol * int(np.ceil(((50 - (100 - _perc)) / p_step))) + empty_symbol * ((100 - _perc) // p_step)
+        _right = symbol * int(np.ceil(((50 - (100 - _perc)) / p_step))
+                              ) + empty_symbol * ((100 - _perc) // p_step)
 
     if mid is not None:
         _mid = mid
     elif mode in ['remaining', 'elapsed']:
 
         # if i == 0: init elapse time
         if i == 0:
@@ -686,15 +698,16 @@
             _remaining_time = _total_time - _elapsed_time
 
             if i < i_max:
 
                 if mode == 'remaining':
                     _mid = '-{}'.format(str(_remaining_time)[:-5])
                 else:
-                    _mid = '{} / {}'.format(str(_elapsed_time)[:-5], str(_total_time)[:-5])
+                    _mid = '{} / {}'.format(str(_elapsed_time)
+                                            [:-5], str(_total_time)[:-5])
 
             else:
                 _mid = '{}'.format(str(_elapsed_time)[:-5])
 
     elif mode == 'perc':
         _mid = '{:6.2f}%'.format(_perc_f)
     else:
@@ -1053,15 +1066,16 @@
 
         if is_list_like(append):
             _append = list(append)
         else:
             _append = [append]
 
         if len(_append) > len(dct):
-            warnings.warn('list is longer than dict, trailing entries will be lost')
+            warnings.warn(
+                'list is longer than dict, trailing entries will be lost')
         _append = dict(zip(dct.keys(), _append))
 
     else:
         _append = append
 
     for _key in _append.keys():
         dct[_key].append(_append[_key])
@@ -1186,15 +1200,16 @@
     :return: List
     """
 
     return tuple(assert_list(*args, **kwargs))
 
 
 def force_list(*args, **kwargs):
-    warnings.warn('force_list is deprecated, please use assert_list instead', DeprecationWarning)
+    warnings.warn(
+        'force_list is deprecated, please use assert_list instead', DeprecationWarning)
     return assert_list(*args, **kwargs)
 
 
 @export
 def assert_scalar(obj: Any, warn: bool = True, default: Scalar = None) -> Scalar:
     """
     Takes any python object and turns it into a scalar object.
@@ -1209,21 +1224,23 @@
 
     _lst = assert_list(obj)
     _len = len(_lst)
     if _len == 0:
         warnings.warn("empty list cannot be cast to scalar, returning None")
         return None
     if warn and _len > 1:
-        warnings.warn(f"assert_scalar: object {obj} has length {_len}, retaining only first entry")
+        warnings.warn(
+            f"assert_scalar: object {obj} has length {_len}, retaining only first entry")
 
     return _lst[0]
 
 
 def force_scalar(*args, **kwargs):
-    warnings.warn('force_scalar is deprecated, please use assert_list instead', DeprecationWarning)
+    warnings.warn(
+        'force_scalar is deprecated, please use assert_list instead', DeprecationWarning)
     return assert_scalar(*args, **kwargs)
 
 
 @export
 def qformat(value: Any, int_format: str = ',', float_format: str = ',.2f', datetime_format: str = '%Y-%m-%d',
             sep: str = ' - ', key_sep: str = ': ', print_key: bool = True) -> str:
     """
@@ -1305,15 +1322,16 @@
     :param replace: Whether to replace or append to existing files. Defaults to append [optional]
     :param format: Table format to use, passed to pandas.DataFrame.to_hdf. Defaults to 'table' while pandas defaults
         to 'fixed' [optional]
     :param do_print: Whether to print intermediate steps to console [optional]
     :param kwargs: Other keyword arguments passed to pandas.DataFrame.to_hdf [optional]
     :return: None
     """
-    assert (groupby is not None) or (key is not None), "You must supply either groupby or key"
+    assert (groupby is not None) or (
+        key is not None), "You must supply either groupby or key"
 
     # -- init
     # - no inplace
     df = pd.DataFrame(df).copy()
     # - defaults
     # groupby
     if groupby is None:
@@ -1334,15 +1352,16 @@
 
         if key is None:
             _key = qformat(_index, int_format='', float_format='.2f')
         else:
             _key = str(key)
 
         if do_print:
-            progressbar(_it, _i_max, print_prefix=f"writing key {_key:<30}: ", p_step=2)
+            progressbar(
+                _it, _i_max, print_prefix=f"writing key {_key:<30}: ", p_step=2)
 
         if write_groupby:
             if GROUPBY_DUMMY in _df_i.columns:
                 _df_i = _df_i.drop(GROUPBY_DUMMY, axis=1)
         else:
             _df_i = _df_i.drop(groupby, axis=1)
 
@@ -1383,15 +1402,15 @@
     :param key_to_col: Whether to save the key value to a column, if a string then used as column name [optional]
     :param do_print: Whether to print intermediate steps [optional]
     :param catch_error: Whether to catch errors when reading [optional]
     :param kwargs: Other keyword arguments passed to pandas.read_hdf [optional]
     :return: pandas DataFrame
     """
 
-    if not os.path.exists(file): 
+    if not os.path.exists(file):
         raise ValueError('{} does not exist'.format(file))
 
     # if key was not specified: read all keys
     if key is None:
         _keys = get_hdf_keys(file)
         _read_keys = 'all'
         if sample is not None:
@@ -1406,15 +1425,16 @@
         _read_keys = ','.join(_keys)
 
     _df = []
 
     for _it, _key in enumerate(_keys):
 
         if do_print:
-            tprint('reading {} - key {} / {} : {}...'.format(file, _it+1, len(_keys), _key))
+            tprint('reading {} - key {} / {} : {}...'.format(file,
+                   _it + 1, len(_keys), _key))
         if catch_error:
             try:
                 _df_i = pd.read_hdf(file, key=_key, **kwargs)
             except KeyboardInterrupt:
                 raise KeyboardInterrupt
             except Exception as _e:
                 tprint('')
@@ -1514,28 +1534,31 @@
     string = str(string)
 
     # -- demojize: (needs to come before trans)
     if demojize:
         if emoji:
             string = emoji.demojize(string)
         else:
-            warnings.warn('Missing optional dependency emoji, skipping demojize')
+            warnings.warn(
+                'Missing optional dependency emoji, skipping demojize')
 
     # -- trans: (needs to come after demojize but before the rest)
     if trans:
         if Translator is None:
-            raise ModuleNotFoundError('Missing optional dependency googletrans, please install it to use trans=True')
+            raise ModuleNotFoundError(
+                'Missing optional dependency googletrans, please install it to use trans=True')
 
         _translator = Translator()
         try:
             # avoid rate limits
             if trans_sleep:
                 sleep(trans_sleep)
             # translate
-            string = _translator.translate(string, dest=trans_dest, src=trans_src).text
+            string = _translator.translate(
+                string, dest=trans_dest, src=trans_src).text
         except JSONDecodeError:
             if warn:
                 warnings.warn(f'handled JSONDecodeError at {string}, this probably means that you exceeded the '
                               f'googletrans rate limit and need to wait 24 hours.')
         except Exception as _exc:
             if warn:
                 warnings.warn(f'handled exception " {type(_exc).__name__,}: {_exc}" when translating {string}, '
@@ -1575,29 +1598,32 @@
     :param key_as_str: Whether all keys of the inverted dictionary should be forced to string
     :param duplicates: Whether to 'adjust' or 'drop' duplicates. In case of 'adjust' duplicates are suffixed with '_'
     :return: Inverted dictionary
     """
 
     # -- assert
     if duplicates not in validations['dict_inv__duplicates']:
-        raise ValueError(f"duplicates must be one of {validations['dict_inv__duplicates']}")
+        raise ValueError(
+            f"duplicates must be one of {validations['dict_inv__duplicates']}")
     # -- init
     _dct_inv = {}
     # -- main
     for _key, _value in dct.items():
         # assert scalar
         if not is_scalar(_value):
-            raise ValueError(f'A non-scalar dictionary value is not invertible, found at key {_key}')
+            raise ValueError(
+                f'A non-scalar dictionary value is not invertible, found at key {_key}')
         # assert non-duplicate value
         if duplicates == 'adjust':
             _warn = True
             while _value in _dct_inv.keys():
                 if _warn:
                     _warn = False
-                    warnings.warn(f'duplicate value found at "{_key}: {_value}", appending _')
+                    warnings.warn(
+                        f'duplicate value found at "{_key}: {_value}", appending _')
                 _value = str(_value) + '_'
         elif (duplicates == 'drop') and (_value in _dct_inv.keys()):
             continue
         # if applicable: convert value to string
         if key_as_str:
             _value = str(_value)
         # assign
@@ -1611,15 +1637,16 @@
     """
     return a copy of a function, based on this StackOverflow answer
     https://stackoverflow.com/questions/13503079/how-to-create-a-copy-of-a-python-function
 
     :param f: a function
     :return: copy of function
     """
-    _f = FunctionType(f.__code__, f.__globals__, name=f.__name__, argdefs=f.__defaults__, closure=f.__closure__)
+    _f = FunctionType(f.__code__, f.__globals__, name=f.__name__,
+                      argdefs=f.__defaults__, closure=f.__closure__)
     _f = functools.update_wrapper(_f, f)
     _f.__kwdefaults__ = f.__kwdefaults__
     return _f
 
 
 @export
 def get_else_key(dct: Mapping, key: Any, exclude: SequenceOrScalar = None) -> Any:
```

### Comparing `hhpy-0.3.0/hhpy/modelling.py` & `hhpy-0.3.1/hhpy/modelling.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
     @docstr
     def fit(self, X: Union[DFOrArray, SequenceOrScalar] = None, y: Union[DFOrArray, SequenceOrScalar] = None,
             df: pd.DataFrame = None, dropna: bool = True, X_test: Union[DFOrArray, SequenceOrScalar] = None,
             y_test: Union[DFOrArray, SequenceOrScalar] = None, df_test: pd.DataFrame = None,
             groupby: SequenceOrScalar = None, split_groupby: bool = None, k: int = 0, **kwargs) -> None:
         """
         generalized fit method extending on model.fit
-        
+
         :param X: %(X)s
         :param y: %(y)s
         :param df: %(df_train)s
         :param dropna: %(dropna)s
         :param X_test: %(X_test)s
         :param y_test: %(y_test)s
         :param df_test: %(df_test)s
@@ -178,28 +178,30 @@
         if split_groupby is None:
             split_groupby = self.split_groupby
         else:
             self.split_groupby = split_groupby
         # - k
         k = assert_list(k)
         if split_groupby and k != [0]:
-            raise ValueError(f"k split is not supported for split_groupby==True")
+            raise ValueError(
+                "k split is not supported for split_groupby==True")
         # - check for groupby in kwargs
 
         # if X and y are passed separately: concat them to a DataFrame
         if df is None:
 
             _df_X = assert_df(X)
             _df_y = assert_df(y)
             # if both X and y are DataFrames we can use their column names
             if isinstance(X, pd.DataFrame) and isinstance(y, (pd.DataFrame, pd.Series)):
                 df = pd.concat([_df_X, _df_y], axis=1)
             # if not then we override the default column names when concatting to avoid duplicates
             else:
-                df = pd.concat([_df_X, _df_y], ignore_index=True, sort=False, axis=1)
+                df = pd.concat(
+                    [_df_X, _df_y], ignore_index=True, sort=False, axis=1)
             # save column names to self
             self.X_ref = _df_X.columns
             self.y_ref = _df_y.columns
             # in this case groupby is not supported
             groupby = []
         # get X_ref and y_ref
         else:
@@ -210,15 +212,16 @@
 
         df = assert_df(df)
         if df_test is not None:
             df_test = assert_df(df_test)
 
         # handle dropna
         if dropna:
-            _dropna_cols = list_intersection(df.columns, list_merge(self.X_ref, self.y_ref, groupby))
+            _dropna_cols = list_intersection(
+                df.columns, list_merge(self.X_ref, self.y_ref, groupby))
             df = df.dropna(subset=_dropna_cols)
             if df_test is not None:
                 df_test = df_test.dropna(subset=_dropna_cols)
 
         # -- init
         if split_groupby:
             df['_groupby'] = concat_cols(df, groupby)
@@ -280,26 +283,27 @@
                 _kwargs['y_test'] = _y_test
 
             _model.fit(X=_X, y=_y, **kwargs)
             self.model[_index] = _model
             del _model
 
         # noinspection PyTypeChecker
-        warnings.simplefilter('default', (FutureWarning, DataConversionWarning))
+        warnings.simplefilter(
+            'default', (FutureWarning, DataConversionWarning))
         self.is_fit = True
 
     @docstr
     def predict(self, X: Union[DFOrArray, SequenceOrScalar] = None, y: Union[DFOrArray, SequenceOrScalar] = None,
                 df: pd.DataFrame = None, return_type: str = 'y', k_index: pd.Series = None,
                 groupby: SequenceOrScalar = None, split_groupby: bool = None,
                 handle_na: bool = True, multi: SequenceOrScalar = None, **kwargs
                 ) -> Union[pd.Series, pd.DataFrame]:
         """
         Generalized predict method based on model.predict
-        
+
         :param X: %(X)s
         :param y: %(y)s
         :param df: %(df)s
         :param return_type: one of %(Model__predict__return_type)s, if 'y' returns a pandas Series / DataFrame
             with only the predictions, if one of 'df','DataFrame' returns the full DataFrame with predictions added
         :param k_index: If specified and model is k_cross split: return only the predictions for each test subset
         :param groupby: %(groupby)s
@@ -312,15 +316,16 @@
 
         # -- assert
         # - model is fit
         if not self.is_fit:
             raise ValueError('Model is not fit yet')
         # - valid return type
         if return_type not in validations['Model__predict__return_type']:
-            raise ValueError(f"return type must be one of {validations['Model__predict__return_type']}")
+            raise ValueError(
+                f"return type must be one of {validations['Model__predict__return_type']}")
         # - df
         if df is not None:
             df = assert_df(df)
         else:
             df = pd.concat([assert_df(X), assert_df(y)], axis=1)
         # - groupby
         if groupby in [None, []]:
@@ -334,15 +339,14 @@
         # backwards compatibility
         _ = k_index
         _ = multi
 
         _y_ref_pred = [f"{_}_{self.name}" for _ in self.y_ref]
 
         # - predict using sklearn api
-        _ks = len(self.model)
         _df_out = []
 
         # loop model dictionary
         for _k, (_key, _model) in enumerate(self.model.items()):
 
             # init
             _kwargs = kwargs.copy()
@@ -364,15 +368,16 @@
                 _X = _df[self.X_ref]
             # noinspection PyUnresolvedReferences
             _na_indices = _X[_X.isna().any(axis=1)].index.tolist()
             # y
             if 'y' not in _kwargs.keys() and 'y' in _varnames:
                 _y = _df[self.y_ref]
                 # noinspection PyUnresolvedReferences
-                _na_indices = list_merge(_na_indices, _X[_X.isna().any(axis=1)].index.tolist())
+                _na_indices = list_merge(
+                    _na_indices, _X[_X.isna().any(axis=1)].index.tolist())
                 if handle_na:  # drop na
                     _y = _y.drop(_na_indices)
                 _kwargs['y'] = _y
             if handle_na:  # drop na (has to be here so y na indices have been handled)
                 _X = _X.drop(_na_indices)
             # - predict
             try:
@@ -381,15 +386,16 @@
                 # sometimes the model accepts y as keyword argument but cannot actually handle it
                 # I'm looking at you sklearn.multioutput
                 kwargs.pop('y')
                 _y_pred = _model.predict(_X, **_kwargs)
 
             # cast to pandas
             if len(_y_pred) != len(_X):
-                raise ValueError(f"The lengths of y_pred ({len(_y_pred)}) and X ({len(_X)}) do not match")
+                raise ValueError(
+                    f"The lengths of y_pred ({len(_y_pred)}) and X ({len(_X)}) do not match")
             _y_pred = pd.DataFrame(_y_pred, index=_X.index)
             _y_pred.columns = _y_ref_pred
             # bring back dropped nans
             if handle_na:
                 _y_pred = pd.concat([_y_pred, pd.DataFrame(np.nan, index=_na_indices, columns=_y_pred.columns)])\
                     .sort_index()
 
@@ -455,15 +461,16 @@
         :param target: One of %(setattr__target)s, for 'self' sets only on self, for 'children' sets for children and
             for 'all' tries to set on both
         :return: None
         """
 
         # -- assert
         if target not in validations['setattr__target']:
-            raise ValueError(f"target must be one of {validations['setattr__target']}")
+            raise ValueError(
+                f"target must be one of {validations['setattr__target']}")
 
         # -- main
         # - self
         if target in ['all', 'a', 'self', 's'] and hasattr(self, key):
             setattr(self, key, value)
 
         # - children
@@ -476,15 +483,15 @@
 # noinspection PyPep8Naming
 @docstr
 @export
 class Models(BaseClass):
     """
     Collection of Models that allow for fitting and predicting with multiple Models at once,
     comparing accuracy and creating Ensembles
-        
+
     :param args: multiple Model objects that will form a Models Collection
     :param name: name of the collection
     :param df: %(df)s
     :param X_ref: %(X_ref)s
     :param y_ref: %(y_ref)s
     :param groupby: %(groupby)s
     :param split_groupby: %(split_groupby)s
@@ -606,15 +613,15 @@
         for _y_pred in list_intersection(self.y_pred, assert_list(self.df.columns)):
             self.df = self.df.drop(_y_pred, axis=1)
 
     @docstr
     def k_split(self, **kwargs):
         """
         apply hhpy.ds.k_split to self to create train-test or k-cross ready data
-        
+
         :param kwargs: keyword arguments passed to :func:`~hhpy.ds.k_split`
         :return: None
         """
 
         # -- init
         if self.df is None:
             raise ValueError('You must specify a df')
@@ -638,40 +645,42 @@
                 if not is_list_like(name):
                     return _model
                 else:
                     _models.append(_model)
         return _models
 
     @docstr
-    def fit(self, fit_type: str = 'train_test',  k_test: Optional[int] = 0, groupby: SequenceOrScalar = None,
+    def fit(self, fit_type: str = 'train_test', k_test: Optional[int] = 0, groupby: SequenceOrScalar = None,
             do_print: bool = True, **kwargs):
         """
         fit all Model objects in collection
-        
+
         :param fit_type: one of %(fit__fit_type)s
         :param k_test: which k_index to use as test data
         :param groupby: %(groupby)s
         :param do_print: %(do_print)s
         :param kwargs: Other keyword arguments passed to :func:`~Model.fit`
         :return: None
         """
 
         # -- assert
         if fit_type not in validations['fit__fit_type']:
-            raise ValueError(f"fit type must be one of {validations['fit__fit_type']}")
+            raise ValueError(
+                f"fit type must be one of {validations['fit__fit_type']}")
 
         # -- init
         if groupby is None:
             groupby = self.groupby
         # get df
         _df = self.df.copy()
         # groupby and k index
         # -- apply scaler to X and y separately
         warnings.simplefilter('ignore', DataConversionWarning)
-        if self.scaler_X is not None and _df[self.X_ref].shape[1] > 0:  # 0 column features cannot be scaled
+        # 0 column features cannot be scaled
+        if self.scaler_X is not None and _df[self.X_ref].shape[1] > 0:
             self.scaler_X = self.scaler_X.fit(_df[self.X_ref])
             _df[self.X_ref] = self.scaler_X.transform(_df[self.X_ref])
         else:
             self.scaler_X = None
         if self.scaler_y is not None:
             self.scaler_y = self.scaler_y.fit(_df[self.y_ref])
             _df[self.y_ref] = self.scaler_y.transform(_df[self.y_ref])
@@ -705,15 +714,15 @@
     def predict(
             self, X: Union[DFOrArray, SequenceOrScalar] = None, y: Union[DFOrArray, SequenceOrScalar] = None,
             df: pd.DataFrame = None, return_type: str = 'self', ensemble: bool = False, k_predict_type: str = 'test',
             groupby: SequenceOrScalar = None, multi: SequenceOrScalar = None, do_print: bool = True, **kwargs
     ) -> Optional[Union[pd.Series, pd.DataFrame]]:
         """
         predict with all models in collection
-        
+
         :param X: %(X_predict)s
         :param y: %(y_predict)s
         :param df: %(df_predict)s
         :param return_type: one of %(Models__predict__return_type)s
         :param ensemble: %(ensemble)s
         :param k_predict_type: 'test' or 'all'
         :param groupby: %(groupby)s
@@ -724,15 +733,16 @@
         """
 
         # -- assert
         # backwards compatibility
         _ = multi
         # return_type
         _valid_return_types = ['self', 'df', 'df_full', 'DataFrame']
-        assert(return_type in _valid_return_types), f"return_type must be one of {_valid_return_types}"
+        assert (
+            return_type in _valid_return_types), f"return_type must be one of {_valid_return_types}"
         # fit_type
         if not self.fit_type:
             raise ValueError('Model is not fit yet')
         # X / y
         if df is None:
             if isinstance(X, pd.DataFrame):
                 if isinstance(y, pd.DataFrame):
@@ -770,15 +780,16 @@
                 # k_cross_type all: return all predictions
                 else:
                     for _k in range(len(_model.model)):
                         _y_ref_preds += [f"{_}_{_model.name}_{_k}" for _ in _model.y_ref]
             else:
                 _y_ref_preds += [f"{_}_{_model.name}" for _ in _model.y_ref]
 
-            _y_pred_scaled = _model.predict(df=df, groupby=groupby, k_index=_k_index, **kwargs)
+            _y_pred_scaled = _model.predict(
+                df=df, groupby=groupby, k_index=_k_index, **kwargs)
 
             # - handle scaler inverse transformation
             if self.scaler_y is None:
                 _y_pred = silentcopy(_y_pred_scaled)
             else:
                 _df_y_pred_scaled = pd.DataFrame(_y_pred_scaled)
                 _df_y_pred_scaled.columns = _model.y_ref
@@ -818,15 +829,16 @@
 
         # adjust column names
         _df.columns = _y_ref_preds
 
         # adjust index
         _df.index = df.index
 
-        if ensemble:  # supports up to 3 model ensembles (does not support multi regression)
+        # supports up to 3 model ensembles (does not support multi regression)
+        if ensemble:
             # drop duplicates
             _model_names = list(set(_model_names))
             # get all combinations
             for _comb in list(itertools.combinations(_model_names, 2)) + list(itertools.combinations(_model_names, 3)):
                 for _y_ref in self.y_ref:
                     _comb_name = '_'.join(_comb)
                     _y_comb_name = '{}_{}'.format(_y_ref, _comb_name)
@@ -848,15 +860,15 @@
             for _col in list_intersection(df.columns, _df.columns):
                 df = df.drop(_col, axis=1)
             return pd.concat([df, _df], axis=1)
 
     @docstr
     def score(
             self, return_type: str = 'self', pivot: bool = False, groupby: SequenceOrScalar = None,
-            do_print: bool = True,  display_score: bool = True, display_format: str = ',.3f', **kwargs
+            do_print: bool = True, display_score: bool = True, display_format: str = ',.3f', **kwargs
     ) -> Optional[pd.DataFrame]:
         """
         calculate score of the Model predictions
 
         :param return_type: one of %(Models__score__return_type)s
         :param pivot: whether to pivot the DataFrame for easier readability [optional]
         :param do_print: %(do_print)s
@@ -865,15 +877,15 @@
         :param groupby: %(groupby)s
         :param kwargs: other keyword arguments passed to :func:`~hhpy.ds.df_score`
         :return: if return_type is 'self': None, else: pandas DataFrame containing the scores
         """
 
         # -- assert
         _valid_return_types = ['self', 'df', 'df_full', 'DataFrame']
-        assert(return_type in _valid_return_types),\
+        assert (return_type in _valid_return_types),\
             f"return_type must be one of {_valid_return_types}"
         groupby = assert_list(groupby)
         _df = self.df.copy()
 
         # -- init
         if do_print:
             self.printf('scoring...')
@@ -888,15 +900,16 @@
         _df_score = df_score(df=_df, y_true=self.y_ref, pred_suffix=self.model_names, pivot=pivot, groupby=groupby,
                              multi=self.multi, **kwargs)
 
         if display_score:
             if pivot:
                 _display_score = _df_score
             else:
-                _display_score = _df_score.pivot_table(index=['y_true', 'y_pred'], columns='score', values='value')
+                _display_score = _df_score.pivot_table(
+                    index=['y_true', 'y_pred'], columns='score', values='value')
             display_df(_display_score, float_format=display_format)
 
         if return_type == 'self':
             self.df_score = _df_score
         else:
             return _df_score
 
@@ -943,21 +956,25 @@
         if kws_pred is None:
             kws_pred = {}
         if kws_score is None:
             kws_score = {}
 
         # -- main
         if do_split:
-            self.k_split(k=k, groupby=groupby, sortby=sortby, random_state=random_state, do_print=do_print)
+            self.k_split(k=k, groupby=groupby, sortby=sortby,
+                         random_state=random_state, do_print=do_print)
         if do_fit:
-            self.fit(fit_type=fit_type, k_test=k_test, do_print=do_print, groupby=groupby, **kws_fit)
+            self.fit(fit_type=fit_type, k_test=k_test,
+                     do_print=do_print, groupby=groupby, **kws_fit)
         if do_predict:
-            self.predict(ensemble=ensemble, do_print=do_print, groupby=groupby, multi=multi, **kws_pred)
+            self.predict(ensemble=ensemble, do_print=do_print,
+                         groupby=groupby, multi=multi, **kws_pred)
         if do_score:
-            self.score(scores=scores, scale=scale, do_print=do_print, display_score=display_score, **kws_score)
+            self.score(scores=scores, scale=scale, do_print=do_print,
+                       display_score=display_score, **kws_score)
         if do_print:
             self.printf('training done')
 
     @docstr_hpt
     def scoreplot(
             self, x='y_ref', y='value', hue='model', hue_order=None, row='score', row_order=None,
             palette=None, width=16, height=9 / 2, scale=None, query=None, return_fig_ax=False,
@@ -987,18 +1004,20 @@
             row_order = ['r2', 'rmse', 'mae', 'stdae', 'medae', 'pae']
         if hue_order is None:
             hue_order = self.model_names
         if palette is None:
             palette = hpt_rcParams['palette']
         _row_order = assert_list(row_order)
 
-        fig, ax = plt.subplots(nrows=len(_row_order), figsize=(width, height * len(_row_order)))
+        fig, ax = plt.subplots(nrows=len(_row_order), figsize=(
+            width, height * len(_row_order)))
         _ax_list = ax_as_list(ax)
 
-        _df_score = self.score(return_type='df', scale=scale, do_print=False, display_score=False)
+        _df_score = self.score(return_type='df', scale=scale,
+                               do_print=False, display_score=False)
         if query is not None:
             _df_score = _df_score.query(query)
 
         _row = -1
         for _row_value in _row_order:
             _row += 1
             _ax = _ax_list[_row]
@@ -1028,15 +1047,16 @@
             for 'all' tries to set on both
         :param child_target: Same as target but passed to :func:`~Model.setattr`
         :return: None
         """
 
         # -- assert
         if target not in validations['setattr__target']:
-            raise ValueError(f"target must be one of {validations['setattr__target']}")
+            raise ValueError(
+                f"target must be one of {validations['setattr__target']}")
 
         # -- main
         # - self
         if target in ['all', 'a', 'self', 's'] and hasattr(self, key):
             setattr(self, key, value)
 
         # - children
@@ -1114,15 +1134,16 @@
     else:
         raise KeyError('no element named __name__')
 
     return _model
 
 
 def force_model(*args, **kwargs):
-    warnings.warn('force_model is deprecated, please use assert_model instead', DeprecationWarning)
+    warnings.warn(
+        'force_model is deprecated, please use assert_model instead', DeprecationWarning)
     return assert_model(*args, **kwargs)
 
 
 @export
 def get_coefs(model: Any, y: SequenceOrScalar):
     """
     get coefficients of a linear regression in a sorted data frame
@@ -1133,15 +1154,16 @@
     """
 
     if isinstance(model, Model):
         _model = model.model
     else:
         _model = model
 
-    assert(hasattr(_model, 'coef_')), 'Attribute coef_ not available, did you specify a linear model?'
+    assert (hasattr(_model, 'coef_')
+            ), 'Attribute coef_ not available, did you specify a linear model?'
 
     _coef = _model.coef_.tolist()
     _coef.append(model.intercept_)
 
     _df = pd.DataFrame()
     _df['feature'] = assert_list(y) + ['intercept']
     _df['coef'] = _coef
@@ -1170,18 +1192,20 @@
             'feature': __predictors,
             'importance': __model.feature_importances_
         })
 
         # if applicable: sum features
         if __features_to_sum is not None:
             for _key in list(__features_to_sum.keys()):
-                ___df['feature'] = np.where(___df['feature'].isin(__features_to_sum[_key]), _key, ___df['feature'])
+                ___df['feature'] = np.where(___df['feature'].isin(
+                    __features_to_sum[_key]), _key, ___df['feature'])
                 ___df = ___df.groupby('feature').sum().reset_index()
 
-        ___df = ___df.sort_values(['importance'], ascending=False).reset_index(drop=True)
+        ___df = ___df.sort_values(
+            ['importance'], ascending=False).reset_index(drop=True)
         ___df['importance'] = np.round(___df['importance'], 5)
 
         return ___df
 
     # get feature importance of a decision tree like model in a sorted data frame
     def _get_feature_importance_xgb(_f_model, _f_predictors, _f_features_to_sum=None):
         # get f_score
@@ -1192,27 +1216,31 @@
 
         # get predictor code
         __df['feature_code'] = list(_f_score.keys())
         __df['feature_code'] = __df['feature_code'].str[1:].astype(int)
 
         # code importance
         __df['importance_abs'] = list(_f_score.values())
-        __df['importance'] = __df['importance_abs'] / __df['importance_abs'].sum()
+        __df['importance'] = __df['importance_abs'] / \
+            __df['importance_abs'].sum()
 
         __df = __df.sort_values(['feature_code']).reset_index(drop=True)
 
-        __df['feature'] = [_f_predictors[x] for x in range(len(_f_predictors)) if x in __df['feature_code']]
+        __df['feature'] = [_f_predictors[x]
+                           for x in range(len(_f_predictors)) if x in __df['feature_code']]
 
         if _f_features_to_sum is not None:
 
             for _key in list(_f_features_to_sum.keys()):
-                __df['feature'] = np.where(__df['feature'].isin(_f_features_to_sum[_key]), _key, __df['feature'])
+                __df['feature'] = np.where(__df['feature'].isin(
+                    _f_features_to_sum[_key]), _key, __df['feature'])
                 __df = __df.groupby('feature').sum().reset_index()
 
-        __df = __df.sort_values(['importance'], ascending=False).reset_index(drop=True)
+        __df = __df.sort_values(
+            ['importance'], ascending=False).reset_index(drop=True)
 
         __df['importance'] = np.round(__df['importance'], 5)
 
         __df = __df[['feature', 'importance']]
 
         return __df
 
@@ -1285,15 +1313,15 @@
     _y = []
 
     # - groupby loop
     for _index, _df_i in _df.groupby(groupby):
         # shift loop
         for _step in range(window):
             # shift by _step+1 since shifting by 0 would mean using the target (label) value as predictor (feature)
-            _x_shift_i = _df_i[_x_cols].shift(_step+1)
+            _x_shift_i = _df_i[_x_cols].shift(_step + 1)
             if dropna:
                 # drop the first window elements (since they are na in at least 1 cast)
                 _x_shift_i = _x_shift_i.iloc[window:]
             _x[_step].append(_x_shift_i)
         # drop the first window elements of y
         if y is not None:
             _y_i = _df_i[_y_cols]
```

### Comparing `hhpy-0.3.0/hhpy/plotting.py` & `hhpy-0.3.1/hhpy/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,28 +92,28 @@
     t='Name of the t variable in data or vector data',
     x_novec='Name of the x variable in data',
     y_novec='Name of the y variable in data',
     t_novec='Name of the t variable in data',
     data='Pandas DataFrame containing named data, optional if vector data is used',
     data_novec='Pandas DataFrame containing named data',
     hue='Further split the plot by the levels of this variable [optional]',
-    order='Either a string describing how the (hue) levels or to be ordered or an explicit list of levels to be ' 
+    order='Either a string describing how the (hue) levels or to be ordered or an explicit list of levels to be '
     'used for plotting. Accepted strings are: '
     '''
-    
+
         * ``sorted``: following python standard sorting conventions (alphabetical for string, ascending for value)
-        
+
         * ``inv``: following python standard sorting conventions but in inverse order
-        
+
         * ``count``: sorted by value counts
-        
+
         * ``mean``, ``mean_ascending``, ``mean_descending``: sorted by mean value, defaults to descending
-        
+
         * ``median``, ``mean_ascending``, ``median_descending``: sorted by median value, defaults to descending
-        
+
     ''',
     color='Color used for plotting, must be known to matplotlib.pyplot [optional]',
     palette='Collection of colors to be used for plotting. Can be a dictionary for with names for each level or '
             'a list of colors or an individual color name. Must be valid colors known to pyplot [optional]',
     cmap='Color map to use [optional]',
     annotations='Whether to display annotations [optional]',
     number_format='The format string used for annotations [optional]',
@@ -180,25 +180,28 @@
     :return: list of ordered levels
     """
     if order is None or order == 'sorted':
         _hues = data[level].drop_duplicates().sort_values().tolist()
     elif order == 'inv':
         _hues = data[level].drop_duplicates().sort_values().tolist()[::-1]
     elif order == 'count':
-        _hues = data[level].value_counts().reset_index().sort_values(by=[level, 'index'])['index'].tolist()
+        _hues = data[level].value_counts().reset_index().sort_values(
+            by=[level, 'index'])['index'].tolist()
     elif order in ['mean', 'mean_descending']:
         _hues = data.groupby(level)[x].mean().reset_index().sort_values(by=[x, level], ascending=[False, True]
                                                                         )[level].tolist()
     elif order == 'mean_ascending':
-        _hues = data.groupby(level)[x].mean().reset_index().sort_values(by=[x, level])[level].tolist()
+        _hues = data.groupby(level)[x].mean().reset_index(
+        ).sort_values(by=[x, level])[level].tolist()
     elif order in ['median', 'median_descending']:
         _hues = data.groupby(level)[x].median().reset_index().sort_values(by=[x, level], ascending=[False, True]
                                                                           )[level].tolist()
     elif order == 'median_ascending':
-        _hues = data.groupby(level)[x].median().reset_index().sort_values(by=[x, level])[level].tolist()
+        _hues = data.groupby(level)[x].median().reset_index(
+        ).sort_values(by=[x, level])[level].tolist()
     else:
         _hues = order
 
     return _hues
 
 
 @docstr
@@ -259,15 +262,16 @@
     _colormap = sns.diverging_palette(220, 10, as_cmap=True)
 
     # mask
     _mask = np.zeros_like(_corr)
     _mask[np.triu_indices_from(_mask)] = True
 
     # Generate Heat Map, allow annotations and place floats in map
-    sns.heatmap(_corr, cmap=_colormap, annot=annotations, fmt=number_format, mask=_mask, ax=ax)
+    sns.heatmap(_corr, cmap=_colormap, annot=annotations,
+                fmt=number_format, mask=_mask, ax=ax)
 
     # Adjust tick labels
     ax.set_xticks(ax.get_xticks()[:-1])
     _yticklabels = ax.get_yticklabels()[1:]
     ax.set_yticks(ax.get_yticks()[1:])
     ax.set_yticklabels(_yticklabels)
 
@@ -292,24 +296,26 @@
     :param ax: %(ax_in)s
     :return: %(ax_out)s
     """
     _df_corr = get_df_corr(data, target=target)
     _df_corr = _df_corr[_df_corr['corr_abs'] >= corr_cutoff]
 
     if target is None:
-        _df_corr['label'] = concat_cols(_df_corr, ['col_0', 'col_1'], sep=' X ')
+        _df_corr['label'] = concat_cols(
+            _df_corr, ['col_0', 'col_1'], sep=' X ')
     else:
         _df_corr['label'] = _df_corr['col_1']
 
     # filter columns (if applicable)
     if columns is not None:
         _columns = columns + []
         if target is not None and target not in _columns:
             _columns.append(target)
-        _df_corr = _df_corr[(_df_corr['col_0'].isin(_columns)) & (_df_corr['col_1'].isin(_columns))]
+        _df_corr = _df_corr[(_df_corr['col_0'].isin(_columns))
+                            & (_df_corr['col_1'].isin(_columns))]
 
     # get colors
     _rgba_colors = np.zeros((len(_df_corr), 4))
 
     # for red the first column needs to be one
     _rgba_colors[:, 0] = np.where(_df_corr['corr'] > 0., 0., 1.)
     # for blue the third column needs to be one
@@ -321,15 +327,15 @@
         _rgba_colors[:, 3] = 1
 
     if ax is None:
         ax = plt.gca()
 
     _rgba_colors = np.round(_rgba_colors, 2)
 
-    _plot = ax.barh(_df_corr['label'], _df_corr['corr'], color=_rgba_colors)
+    ax.barh(_df_corr['label'], _df_corr['corr'], color=_rgba_colors)
     ax.invert_yaxis()
 
     if xlim:
         # noinspection PyTypeChecker
         ax.set_xlim(xlim)
 
     if target is not None:
@@ -386,18 +392,20 @@
                 if sample_warn:
                     warnings.warn(
                         'Limiting Scatter Plot to {:,} randomly selected points. '
                         'Turn this off with max_n=None or suppress this warning with sample_warn=False.'.format(
                             max_n))
                 _data = _data.sample(max_n, random_state=random_state)
 
-        _f_ax.scatter(_f_x, _f_y, data=_data, alpha=alpha, color=_f_color, label=_f_label)
+        _f_ax.scatter(_f_x, _f_y, data=_data, alpha=alpha,
+                      color=_f_color, label=_f_label)
 
         if trendline:
-            _f_ax.plot(_f_data[_f_x], lfit(_f_data[_f_x], _f_data[_f_y]), color=_f_color_trendline, linestyle=':')
+            _f_ax.plot(_f_data[_f_x], lfit(
+                _f_data[_f_x], _f_data[_f_y]), color=_f_color_trendline, linestyle=':')
 
         return _f_ax
 
     # avoid inplace operations
     _df = data.copy()
     _df_hues = pd.DataFrame()
     _df_corrs = pd.DataFrame()
@@ -419,43 +427,46 @@
     _df_corr = get_df_corr(_df, target=target)
 
     if corr_cutoff is not None:
         _df_corr = _df_corr[_df_corr['corr_abs'] >= corr_cutoff]
 
     # warning for empty df
     if len(_df_corr) == 0:
-        warnings.warn('Correlation DataFrame is Empty. Do you need a lower corr_cutoff?')
+        warnings.warn(
+            'Correlation DataFrame is Empty. Do you need a lower corr_cutoff?')
         return None
 
     # edge case for less plots than ncols
     if len(_df_corr) < col_wrap:
         _ncols = len(_df_corr)
     else:
         _ncols = col_wrap
 
     # calculate nrows
     _nrows = int(np.ceil(len(_df_corr) / _ncols))
 
     _figsize = (width * col_wrap, height * _nrows)
 
     if ax is None:
-        fig, ax = plt.subplots(nrows=_nrows, ncols=_ncols, figsize=_figsize, **kwargs)
+        fig, ax = plt.subplots(nrows=_nrows, ncols=_ncols,
+                               figsize=_figsize, **kwargs)
     else:
         fig = plt.gcf()
 
     _row = None
     _col = None
 
     for _it in range(len(_df_corr)):
 
         _col = _it % _ncols
         _row = _it // _ncols
 
         _x = _df_corr.iloc[_it]['col_1']
-        _y = _df_corr.iloc[_it]['col_0']  # so that target (if available) becomes y
+        # so that target (if available) becomes y
+        _y = _df_corr.iloc[_it]['col_0']
         _corr = _df_corr.iloc[_it]['corr']
 
         if _ncols == 1:
             _rows_prio = True
         else:
             _rows_prio = False
 
@@ -465,15 +476,16 @@
         _ax.set_ylabel(_y)
         _ax.set_title('corr = {:.3f}'.format(_corr))
 
         # hue if
         if hue is None:
 
             # actual plot
-            _f_plot(_f_x=_x, _f_y=_y, _f_data=_df, _f_color=None, _f_color_trendline='k', _f_label=None, _f_ax=_ax)
+            _f_plot(_f_x=_x, _f_y=_y, _f_data=_df, _f_color=None,
+                    _f_color_trendline='k', _f_label=None, _f_ax=_ax)
 
         else:
 
             for _hue_it, _hue in enumerate(_hues):
 
                 if isinstance(palette, Mapping):
                     _color = palette[_hue]
@@ -570,15 +582,16 @@
     :param x_offset_perc: the amount whitespace to display next to x_min and x_max in percent of x_range [optional]
     :param ax: %(ax_in)s
     :param kwargs: additional keyword arguments passed to pyplot.plot
     :return: %(ax_out)s
     """
     # -- asserts
     if distfit not in validations['distplot__distfit']:
-        raise ValueError(f"distfit must be one of {validations['distplot__distfit']}")
+        raise ValueError(
+            f"distfit must be one of {validations['distplot__distfit']}")
     # -- defaults
     if palette is None:
         palette = rcParams['palette']
     if not top_nr:
         top_nr = None
 
     # case: vector data
@@ -658,15 +671,15 @@
 
                 __x_min = _mu - _f_std_cutoff * _sigma
                 __x_max = _mu + _f_std_cutoff * _sigma
 
             _df_i = _df_i[
                 (_df_i[_f_x] >= __x_min) &
                 (_df_i[_f_x] <= __x_max)
-                ]
+            ]
 
         # for plot trimming
         _x_mins.append(_df_i[x].min())
         _x_maxs.append(_df_i[x].max())
 
         # handle label
         try:
@@ -681,29 +694,29 @@
 
         if agg_func == 'mean':
             _mu_symbol = r'\ \mu'
         else:
             _mu_symbol = r'\ \nu'
 
         if label_style == 'mu_sigma':
-            _label = r'{}: $ {}={},\ \sigma={}$'.format(_f_x_label, _mu_symbol, _mu_label, _sigma_label)
+            _label = r'{}: $ {}={},\ \sigma={}$'.format(
+                _f_x_label, _mu_symbol, _mu_label, _sigma_label)
         else:
             _label = _f_x_label
 
         # plot histogram
         if hist:
             _hist_n, _hist_bins = _f_ax.hist(_df_i[_f_x], _f_bins, density=perc, facecolor=_f_facecolor,
                                              edgecolor=edgecolor,
                                              alpha=alpha, label=_label)[:2]
             _label_2 = '__nolegend___'
             if _f_distfit_line is None:
                 _f_distfit_line = '--'
         else:
             _hist_n = None
-            _hist_bins = None
             _label_2 = _label + ''
             if _f_distfit_line is None:
                 _f_distfit_line = '-'
 
         # plot distfit
         if distfit:
 
@@ -742,15 +755,16 @@
             _y_max = np.max(_hist_n) / np.sum(_hist_n) * 100
             _y_ticklabels = list(_f_ax.get_yticks())
             _y_ticklabels = [float(_) for _ in _y_ticklabels]
 
             _factor = _y_max / np.nanmax(_y_ticklabels)
             if np.isnan(_factor):
                 _factor = 1
-            _y_ticklabels = [format(int(_ * _factor), ',') for _ in _y_ticklabels]
+            _y_ticklabels = [format(int(_ * _factor), ',')
+                             for _ in _y_ticklabels]
             _f_ax.set_yticklabels(_y_ticklabels)
             _f_ax.set_ylabel('%')
 
         elif hist:
 
             _f_ax.set_ylabel('count')
 
@@ -830,16 +844,18 @@
                               _f_bins=_bins, _f_std_cutoff=std_cutoff,
                               _f_xlim=xlim, _f_distfit_line=linestyle, _f_ax=ax, _f_ax2=ax2, _f_fill=fill)
 
     else:  # no hue
 
         # group values outside of top_n to other_name
         if top_nr is not None:
-            _hues = _df[hue].value_counts().reset_index().sort_values(by=[hue, 'index'])['index'].tolist()
-            if (top_nr + 1) < len(_hues):  # the plus 1 is there to avoid the other group having exactly 1 entry
+            _hues = _df[hue].value_counts().reset_index().sort_values(
+                by=[hue, 'index'])['index'].tolist()
+            # the plus 1 is there to avoid the other group having exactly 1 entry
+            if (top_nr + 1) < len(_hues):
                 _hues = pd.Series(_hues)[0:top_nr]
                 _df[hue] = np.where(_df[hue].isin(_hues), _df[hue], other_name)
                 _df[hue] = _df[hue].astype('str')
                 _hues = list(_hues) + [other_name]
         # parse hue order
         else:
             _hues = _get_ordered_levels(_df, hue, hue_order, x)
@@ -904,16 +920,18 @@
                                   _f_std_cutoff=_std_cutoff_hues,
                                   _f_xlim=xlim, _f_distfit_line=_linestyle, _f_ax=ax, _f_ax2=ax2, _f_fill=fill)
 
     # -- postprocessing
     # handle legend
     if legend:
         if legend_loc in ['bottom', 'right']:
-            legend_outside(ax, loc=legend_loc, legend_space=legend_space, ncol=legend_ncol)
-            legend_outside(ax2, loc=legend_loc, legend_space=legend_space, ncol=legend_ncol)
+            legend_outside(ax, loc=legend_loc,
+                           legend_space=legend_space, ncol=legend_ncol)
+            legend_outside(ax2, loc=legend_loc,
+                           legend_space=legend_space, ncol=legend_ncol)
         else:
             _, _labels = ax.get_legend_handles_labels()
             if len(_labels) > 0:
                 ax.legend(loc=legend_loc, ncol=legend_ncol)
 
             _, _labels = ax2.get_legend_handles_labels()
             if len(_labels) > 0:
@@ -1032,28 +1050,30 @@
         # Calculate the value
         _coef = np.corrcoef(_f_x, _f_y)[0][1]
         # Make the label
         _label = r'$\rho$ = ' + str(round(_coef, 2))
 
         # Add the label to the plot
         _ax = plt.gca()
-        _ax.annotate(_label, xy=(0.2, 0.95 - (_f_s - 10.) / 10.), size=20, xycoords=_ax.transAxes, **_f_kwargs)
+        _ax.annotate(_label, xy=(0.2, 0.95 - (_f_s - 10.) / 10.),
+                     size=20, xycoords=_ax.transAxes, **_f_kwargs)
 
     # Create an instance of the PairGrid class.
     _grid = sns.PairGrid(data=data,
                          vars=cols,
                          **kwargs)
 
     # Map a scatter plot to the upper triangle
     _grid = _grid.map_upper(plt.scatter, alpha=alpha, color=color)
     # Map a corr coef
     _grid = _grid.map_upper(_f_corr)
 
     # density = True might not be supported in older versions of seaborn / matplotlib
-    _grid = _grid.map_diag(plt.hist, bins=30, color=color, alpha=alpha, edgecolor='k', density=True)
+    _grid = _grid.map_diag(plt.hist, bins=30, color=color,
+                           alpha=alpha, edgecolor='k', density=True)
 
     # Map a density plot to the lower triangle
     _grid = _grid.map_lower(sns.kdeplot, cmap=cmap, alpha=alpha)
 
     # add legend
     _grid.add_legend()
 
@@ -1143,52 +1163,55 @@
 
     if cols is None:
         cols = data.select_dtypes(include=np.number)
 
     _levels = _get_ordered_levels(data=data, level=level, order=order)
 
     if hue is not None:
-        _hues = _get_ordered_levels(data=data, level=hue, order=hue_order)
         _hue_str = ' by {}'.format(hue)
     else:
         _hue_str = ''
 
     _nrows = len(cols)
     _ncols = len(_levels) + 1
 
     _it_max = _nrows * _ncols
 
-    fig, ax = plt.subplots(nrows=_nrows, ncols=_ncols, figsize=(_ncols * width, _nrows * height))
+    fig, ax = plt.subplots(nrows=_nrows, ncols=_ncols,
+                           figsize=(_ncols * width, _nrows * height))
 
     _it = -1
 
     for _col_i, _col in enumerate(cols):
 
-        _ax_summary = get_subax(ax, _col_i, 0, rows_prio=False)  # always plot to col 0 of current row
+        # always plot to col 0 of current row
+        _ax_summary = get_subax(ax, _col_i, 0, rows_prio=False)
         # summary plot
         func(_col, data=data, hue=level, ax=_ax_summary, **kwargs_summary)
         if summary_title:
             _ax_summary.set_title('{} by {}'.format(_col, level))
 
         for _level_i, _level in enumerate(_levels):
 
             _it += 1
 
             if do_print:
-                progressbar(_it, _it_max, print_prefix='{}_{}'.format(_col, _level))
+                progressbar(
+                    _it, _it_max, print_prefix='{}_{}'.format(_col, _level))
 
             _df_level = data[data[level] == _level]
 
             _ax = get_subax(ax, _col_i, _level_i + 1)
 
             # level plot
             func(_col, data=_df_level, hue=hue, ax=_ax, **kwargs)
 
             if level_title:
-                _ax.set_title('{}{} - {}={}'.format(_col, _hue_str, level, _level))
+                _ax.set_title('{}{} - {}={}'.format(_col,
+                              _hue_str, level, _level))
 
     if kwargs_subplots_adjust is not None:
         plt.subplots_adjust(**kwargs_subplots_adjust)
 
     if do_print:
         progressbar()
 
@@ -1217,15 +1240,16 @@
     # you can pass the hues to use or if none are given the default ones (std,plus/minus) are used
     # you can pass xlim and ylim or assume default (4 std)
 
     # four components, ie 2 x 2
     if return_fig_ax is None:
         return_fig_ax = rcParams['return_fig_ax']
     if lim is None:
-        lim = {'x_1': 'default', 'x_2': 'default', 'y_1': 'default', 'y_2': 'default'}
+        lim = {'x_1': 'default', 'x_2': 'default',
+               'y_1': 'default', 'y_2': 'default'}
     _nrows = 2
     _ncols = 2
 
     # init plot
     fig, ax = plt.subplots(ncols=_ncols, nrows=_nrows)
 
     # make a copy yo avoid inplace operations
@@ -1246,18 +1270,22 @@
                                    _df_plot['std'])
         _df_plot['std'] = _df_plot['std'].astype('category')
 
         hue_1 = 'std'
 
     # type 2: split by plus minus
     if hue_2 is None:
-        _df_plot['plus_minus'] = np.where((_df_plot[x_1] <= 0) & (_df_plot[y_1] <= 0), '- -', 'Null')
-        _df_plot['plus_minus'] = np.where((_df_plot[x_1] <= 0) & (_df_plot[y_1] > 0), '- +', _df_plot['plus_minus'])
-        _df_plot['plus_minus'] = np.where((_df_plot[x_1] > 0) & (_df_plot[y_1] <= 0), '+ -', _df_plot['plus_minus'])
-        _df_plot['plus_minus'] = np.where((_df_plot[x_1] > 0) & (_df_plot[y_1] > 0), '+ +', _df_plot['plus_minus'])
+        _df_plot['plus_minus'] = np.where(
+            (_df_plot[x_1] <= 0) & (_df_plot[y_1] <= 0), '- -', 'Null')
+        _df_plot['plus_minus'] = np.where((_df_plot[x_1] <= 0) & (
+            _df_plot[y_1] > 0), '- +', _df_plot['plus_minus'])
+        _df_plot['plus_minus'] = np.where((_df_plot[x_1] > 0) & (
+            _df_plot[y_1] <= 0), '+ -', _df_plot['plus_minus'])
+        _df_plot['plus_minus'] = np.where((_df_plot[x_1] > 0) & (
+            _df_plot[y_1] > 0), '+ +', _df_plot['plus_minus'])
         _df_plot['plus_minus'] = _df_plot['plus_minus'].astype('category')
 
         hue_2 = 'plus_minus'
 
     _xs = [x_1, x_2]
     _ys = [y_1, y_2]
     _hues = [hue_1, hue_2]
@@ -1276,15 +1304,16 @@
             _y_name = _ys[_col]
             _hue = _hues[_row]
 
             _x = _df_plot[_x_name]
             _y = _df_plot[_y_name]
 
             # scatterplot
-            _ax = sns.scatterplot(data=_df_plot, x=_x_name, y=_y_name, hue=_hue, marker='.', ax=_ax, **kwargs)
+            _ax = sns.scatterplot(
+                data=_df_plot, x=_x_name, y=_y_name, hue=_hue, marker='.', ax=_ax, **kwargs)
 
             # grid 0 line
             _ax.axvline(0, color='k', alpha=.5, linestyle=':')
             _ax.axhline(0, color='k', alpha=.5, linestyle=':')
 
             # title
             _ax.set_title('%s vs %s, hue: %s' % (_x_name, _y_name, _hue))
@@ -1402,15 +1431,16 @@
     if len(_facets) > col_wrap:
         _ncols = col_wrap
         _nrows = int(np.ceil(len(_facets) / _ncols))
     else:
         _ncols = len(_facets)
         _nrows = 1
 
-    fig, ax = plt.subplots(ncols=_ncols, nrows=_nrows, figsize=(width * _ncols, height * _nrows), **subplots_kws)
+    fig, ax = plt.subplots(ncols=_ncols, nrows=_nrows, figsize=(
+        width * _ncols, height * _nrows), **subplots_kws)
     _ax_list = ax_as_list(ax)
 
     # loop facets
     for _it, _facet in enumerate(_facets):
 
         _col = _it % _ncols
         _row = _it // _ncols
@@ -1550,15 +1580,16 @@
         palette = rcParams['palette']
     if text_kws is None:
         text_kws = {}
     if ax is None:
         ax = plt.gca()
 
     _df = data.copy()
-    _df = _df[~((_df[x].isnull()) | (_df[y].isnull()) | (_df[s].isnull()))].reset_index(drop=True)
+    _df = _df[~((_df[x].isnull()) | (_df[y].isnull()) |
+                (_df[s].isnull()))].reset_index(drop=True)
 
     if hue_order is not None:
         _df['_sort'] = _df[hue].apply(lambda _: hue_order.index(_))
         _df = _df.sort_values(by=['_sort'])
 
     _df = _df.reset_index(drop=True)
 
@@ -1612,15 +1643,16 @@
             if _y_max is None:
                 _y_max = _y_max_i
             elif _y_max_i > _y_max:
                 _y_max = _y_max_i
 
     else:
         # scatter for bubbles
-        ax.scatter(x=_x, y=_y, s=_s, label='__nolegend__', facecolor=_df['_color'], edgecolor='black', alpha=.75)
+        ax.scatter(x=_x, y=_y, s=_s, label='__nolegend__',
+                   facecolor=_df['_color'], edgecolor='black', alpha=.75)
 
         _x_range = _x.max() - _x.min()
         _x_min = _x.min() - _x_range / x_range_factor
         _x_max = _x.max() + _x_range / x_range_factor
 
         _y_range = _y.max() - _y.min()
         _y_min = _y.min() - _y_range / y_range_factor
@@ -1689,37 +1721,41 @@
 
     # handle na
     _df[x] = _df[x].fillna(_df[x].dropna().agg(agg_function))
     _df[y] = _df[y].fillna(_df[y].dropna().agg(agg_function))
 
     # build agg dict
     _df['_count'] = 1
-    _df = _df.groupby([hue]).agg({x: [agg_function, 'std'], y: [agg_function, 'std'], '_count': 'count'}).reset_index()
+    _df = _df.groupby([hue]).agg({x: [agg_function, 'std'], y: [
+        agg_function, 'std'], '_count': 'count'}).reset_index()
     if x != y:
         _columns = [hue, x, x + '_std', y, y + '_std', '_count']
     else:
         _columns = [hue, x, x + '_std', '_count']
     _df.columns = _columns
     _df['_perc'] = _df['_count'] / _df['_count'].sum() * 100
-    _df['_count_text'] = _df.apply(lambda _: "{:,}".format(_['_count']), axis=1)
+    _df['_count_text'] = _df.apply(
+        lambda _: "{:,}".format(_['_count']), axis=1)
     _df['_perc_text'] = np.round(_df['_perc'], 2)
     _df['_perc_text'] = _df['_perc_text'].astype(str) + '%'
 
     if show_std:
         _df['_text'] = _df[hue].astype(str) + '(' + _df['_count_text'] + ')' + '\n' \
-                       + 'x:' + _df[x].apply(lambda _: format(_, float_format)) + r'$\pm$' + _df[x + '_std'].apply(
+            + 'x:' + _df[x].apply(lambda _: format(_, float_format)) + r'$\pm$' + _df[x + '_std'].apply(
             lambda _: format(_, float_format)) + '\n' \
-                       + 'y:' + _df[y].apply(lambda _: format(_, float_format)) + r'$\pm$' + _df[y + '_std'].apply(
+            + 'y:' + _df[y].apply(lambda _: format(_, float_format)) + r'$\pm$' + _df[y + '_std'].apply(
             lambda _: format(_, float_format))
     else:
-        _df['_text'] = _df[hue].astype(str) + '\n' + _df['_count_text'] + '\n' + _df['_perc_text']
+        _df['_text'] = _df[hue].astype(
+            str) + '\n' + _df['_count_text'] + '\n' + _df['_perc_text']
 
     _df['_text'] += text_end
 
-    bubbleplot(x=x, y=y, hue=hue, s='_perc', text='_text', data=_df, show_std=show_std, **kwargs)
+    bubbleplot(x=x, y=y, hue=hue, s='_perc', text='_text',
+               data=_df, show_std=show_std, **kwargs)
 
 
 @docstr
 @export
 def rmsdplot(x: str, data: pd.DataFrame, groups: Union[Sequence, str] = None, hue: str = None,
              hue_order: Union[Sequence, str] = None, cutoff: float = 0, ax: plt.Axes = None,
              color_as_balance: bool = False, balance_cutoff: float = None, rmsd_as_alpha: bool = False,
@@ -1755,65 +1791,76 @@
         barh_kws = {}
     _data = data.copy()
     del data
 
     if hue is not None and hue_order is not None:
         _data = _data.query('{} in @hue_order'.format(hue))
 
-    _df_rmsd = df_rmsd(x=x, df=_data, groups=groups, hue=hue, sort_by_hue=sort_by_hue, **kwargs)
+    _df_rmsd = df_rmsd(x=x, df=_data, groups=groups, hue=hue,
+                       sort_by_hue=sort_by_hue, **kwargs)
     _df_rmsd = _df_rmsd[_df_rmsd['rmsd'] >= cutoff]
 
     if hue is not None:
-        _df_rmsd_no_hue = df_rmsd(x=x, df=_data, groups=groups, include_rmsd=False, **kwargs)
+        _df_rmsd_no_hue = df_rmsd(
+            x=x, df=_data, groups=groups, include_rmsd=False, **kwargs)
     else:
         _df_rmsd_no_hue = pd.DataFrame()
 
     if isinstance(x, list):
         if hue is None:
-            _df_rmsd['label'] = concat_cols(_df_rmsd, ['x', 'group'], sep=' X ')
+            _df_rmsd['label'] = concat_cols(
+                _df_rmsd, ['x', 'group'], sep=' X ')
         else:
-            _df_rmsd['label'] = concat_cols(_df_rmsd, ['x', 'group', hue], sep=' X ')
+            _df_rmsd['label'] = concat_cols(
+                _df_rmsd, ['x', 'group', hue], sep=' X ')
     else:
         if hue is None:
             _df_rmsd['label'] = _df_rmsd['group']
         else:
-            _df_rmsd['label'] = concat_cols(_df_rmsd, ['group', hue], sep=' X ')
+            _df_rmsd['label'] = concat_cols(
+                _df_rmsd, ['group', hue], sep=' X ')
 
     _df_rmsd['rmsd_scaled'] = _df_rmsd['rmsd'] / _df_rmsd['rmsd'].max()
 
     # get colors
     _rgba_colors = np.zeros((len(_df_rmsd), 4))
     _hues = []
 
     if hue is not None:
 
-        _hues = _get_ordered_levels(data=_df_rmsd, level=hue, order=hue_order, x=x)
+        _hues = _get_ordered_levels(
+            data=_df_rmsd, level=hue, order=hue_order, x=x)
 
         if isinstance(palette, Mapping):
             _df_rmsd['_color'] = _df_rmsd[hue].apply(lambda _: palette[_])
         elif is_list_like(palette):
-            _df_rmsd['_color'] = _df_rmsd[hue].apply(lambda _: palette[list(_hues).index(_)])
+            _df_rmsd['_color'] = _df_rmsd[hue].apply(
+                lambda _: palette[list(_hues).index(_)])
         else:
             _df_rmsd['_color'] = palette
 
         _rgba_colors[:, 0] = _df_rmsd['_color'].apply(lambda _: Color(_).red)
         _rgba_colors[:, 1] = _df_rmsd['_color'].apply(lambda _: Color(_).green)
         _rgba_colors[:, 2] = _df_rmsd['_color'].apply(lambda _: Color(_).blue)
 
     elif color_as_balance:
 
         if balance_cutoff is None:
 
-            _rgba_colors[:, 0] = _df_rmsd['maxperc']  # for red the first column needs to be one
-            _rgba_colors[:, 2] = 1 - _df_rmsd['maxperc']  # for blue the third column needs to be one
+            # for red the first column needs to be one
+            _rgba_colors[:, 0] = _df_rmsd['maxperc']
+            # for blue the third column needs to be one
+            _rgba_colors[:, 2] = 1 - _df_rmsd['maxperc']
 
         else:
 
-            _rgba_colors[:, 0] = np.where(_df_rmsd['maxperc'] >= balance_cutoff, 1, 0)
-            _rgba_colors[:, 2] = np.where(_df_rmsd['maxperc'] < balance_cutoff, 1, 0)
+            _rgba_colors[:, 0] = np.where(
+                _df_rmsd['maxperc'] >= balance_cutoff, 1, 0)
+            _rgba_colors[:, 2] = np.where(
+                _df_rmsd['maxperc'] < balance_cutoff, 1, 0)
 
     else:
         _rgba_colors[:, 2] = 1  # for blue the third column needs to be one
 
     # the fourth column needs to be alphas
     if rmsd_as_alpha:
         _rgba_colors[:, 3] = _df_rmsd['rmsd_scaled']
@@ -1835,30 +1882,33 @@
     if (hue is not None) and (not sort_by_hue):
         # iterate over rows and add to pos if label changes
         for _row in range(1, len(_df_rmsd)):
             if _df_rmsd['group'].iloc[_row] != _df_rmsd['group'].iloc[_row - 1]:
                 _df_rmsd['pos'][_row:] = _df_rmsd['pos'][_row:] + _pos_factor
 
         # make a df of the average positions for each group
-        _df_ticks = _df_rmsd.groupby('group').agg({'pos': 'mean'}).reset_index()  # 'maxperc':'max'
-        _df_ticks = pd.merge(_df_ticks, _df_rmsd_no_hue[['group', 'maxperc']])  # get maxperc from global value
+        _df_ticks = _df_rmsd.groupby('group').agg(
+            {'pos': 'mean'}).reset_index()  # 'maxperc':'max'
+        # get maxperc from global value
+        _df_ticks = pd.merge(_df_ticks, _df_rmsd_no_hue[['group', 'maxperc']])
     else:
         _df_ticks = pd.DataFrame()
 
     ax.barh(_df_rmsd['pos'], _df_rmsd['rmsd'], color=_rgba_colors, **barh_kws)
 
     _y_colors = None
 
     if (hue is not None) and (not sort_by_hue):
 
         _y_pos = _df_ticks['pos']
         _y_lab = _df_ticks['group']
         # color
         if balance_cutoff is not None:
-            _y_colors = np.where(_df_ticks['maxperc'] > balance_cutoff, sns.xkcd_rgb['red'], 'k')
+            _y_colors = np.where(
+                _df_ticks['maxperc'] > balance_cutoff, sns.xkcd_rgb['red'], 'k')
 
     else:
 
         _y_pos = _df_rmsd['pos']
 
         if not is_list_like(x):
             _y_lab = _df_rmsd['group']
@@ -1884,15 +1934,16 @@
     ax.invert_yaxis()
 
     # create legend for hues
     if hue is not None:
 
         _patches = []
         for _hue, _color, _count in _df_rmsd[[hue, '_color', 'count']].drop_duplicates().values:
-            _patches.append(patches.Patch(color=_color, label='{} (n={:,})'.format(_hue, _count)))
+            _patches.append(patches.Patch(
+                color=_color, label='{} (n={:,})'.format(_hue, _count)))
         ax.legend(handles=_patches)
 
     # check if standardized
     _x_label_suffix = ''
 
     if 'standardize' in kwargs.keys():
         if kwargs['standardize']:
@@ -1933,15 +1984,16 @@
 
     _x = x
     _group = group
 
     # EITHER x OR group can be a list (hue cannot be a lists)
     if is_list_like(x) and is_list_like(group):
 
-        warnings.warn('both x and group cannot be a list, setting group = {}'.format(group[0]))
+        warnings.warn(
+            'both x and group cannot be a list, setting group = {}'.format(group[0]))
         _x_is_list = True
         _group_is_list = False
         _group = group[0]
         _ncols = len(x)
         _nrows = _len
 
     elif isinstance(x, list):
@@ -1962,41 +2014,46 @@
     else:
 
         _x_is_list = False
         _group_is_list = False
         _ncols = int(np.floor(_len / 2))
         _nrows = int(np.ceil(_len / 2))
 
-    fig, ax = plt.subplots(figsize=(width * _ncols, height * _nrows), nrows=_nrows, ncols=_ncols, **subplots_kws)
+    fig, ax = plt.subplots(figsize=(
+        width * _ncols, height * _nrows), nrows=_nrows, ncols=_ncols, **subplots_kws)
 
     _it = -1
 
     for _col in range(_ncols):
 
         if _x_is_list:
             _x = x[_col]
         if _group_is_list:
             _group = group[_col]
 
-        _df_agg = df_agg(x=_x, group=_group, hue=hue, df=data, agg=agg, p=p, **aggkws)
+        _df_agg = df_agg(x=_x, group=_group, hue=hue,
+                         df=data, agg=agg, p=p, **aggkws)
 
         if hue is not None:
             if sort_by_hue:
                 _sort_by = [hue, _group]
             else:
                 _sort_by = [_group, hue]
             _df_agg = _df_agg.sort_values(by=_sort_by).reset_index(drop=True)
             _label = '_label'
-            _df_agg[_label] = concat_cols(_df_agg, [_group, hue], sep='_').astype('category')
-            _hues = _get_ordered_levels(data=data, level=hue, order=hue_order, x=x)
+            _df_agg[_label] = concat_cols(
+                _df_agg, [_group, hue], sep='_').astype('category')
+            _hues = _get_ordered_levels(
+                data=data, level=hue, order=hue_order, x=x)
 
             if isinstance(palette, Mapping):
                 _df_agg['_color'] = _df_agg[hue].apply(lambda _: palette[_])
             elif is_list_like(palette):
-                _df_agg['_color'] = _df_agg[hue].apply(lambda _: palette[list(_hues).index(_)])
+                _df_agg['_color'] = _df_agg[hue].apply(
+                    lambda _: palette[list(_hues).index(_)])
             else:
                 _df_agg['_color'] = palette
 
         else:
             _label = _group
 
         for _row in range(_nrows):
@@ -2028,22 +2085,25 @@
 
             _df_agg['pos'] = _df_agg.index
 
             if (hue is not None) and (not sort_by_hue):
                 # iterate over rows and add to pos if label changes
                 for _row_2 in range(1, len(_df_agg)):
                     if _df_agg[_group].iloc[_row_2] != _df_agg[_group].iloc[_row_2 - 1]:
-                        _df_agg['pos'][_row_2:] = _df_agg['pos'][_row_2:] + _pos_factor
+                        _df_agg['pos'][_row_2:] = _df_agg['pos'][_row_2:] + \
+                            _pos_factor
 
                 # make a df of the average positions for each group
-                _df_ticks = _df_agg.groupby(_group).agg({'pos': 'mean'}).reset_index()
+                _df_ticks = _df_agg.groupby(_group).agg(
+                    {'pos': 'mean'}).reset_index()
             else:
                 _df_ticks = pd.DataFrame()
 
-            _ax.barh('pos', _agg, color='_color', label=_agg, data=_df_agg, **kwargs)
+            _ax.barh('pos', _agg, color='_color',
+                     label=_agg, data=_df_agg, **kwargs)
 
             if (hue is not None) and (not sort_by_hue):
                 _ax.set_yticks(_df_ticks['pos'])
                 _ax.set_yticklabels(_df_ticks[_group])
             else:
                 _ax.set_yticks(_df_agg['pos'])
                 _ax.set_yticklabels(_df_agg[_group])
@@ -2108,21 +2168,23 @@
     if x_int is not None:
         data[x] = np.round(data[x] / x_int) * x_int
     if time_int is not None:
         data[x] = data[x].astype('<M8[{}]'.format(time_int))
 
     # agg
 
-    data = data.groupby([x]).agg({y: [aggfunc, 'std']}).set_axis([_y_agg, _y_std], axis=1, inplace=False).reset_index()
+    data = data.groupby([x]).agg({y: [aggfunc, 'std']}).set_axis(
+        [_y_agg, _y_std], axis=1, inplace=False).reset_index()
 
     if ax is None:
         ax = plt.gca()
 
     ax.plot(data[x], data[_y_agg], color=color, label=_y_agg)
-    ax.fill_between(data[x], data[_y_agg] + data[_y_std], data[_y_agg] - data[_y_std], color='xkcd:cyan', label=_y_std)
+    ax.fill_between(data[x], data[_y_agg] + data[_y_std],
+                    data[_y_agg] - data[_y_std], color='xkcd:cyan', label=_y_std)
     ax.set_xlabel(x)
     ax.set_ylabel(y)
     ax.legend()
 
     return ax
 
 
@@ -2182,17 +2244,19 @@
     :param kwargs: other keyword arguments passed to insert_linebreaks
     :return: None
     """
     if ax is None:
         ax = plt.gca()
 
     if x:
-        ax.set_xticklabels([insert_linebreak(_item.get_text(), **kwargs) for _item in ax.get_xticklabels()])
+        ax.set_xticklabels([insert_linebreak(_item.get_text(), **kwargs)
+                           for _item in ax.get_xticklabels()])
     if y:
-        ax.set_yticklabels([insert_linebreak(_item.get_text(), **kwargs) for _item in ax.get_yticklabels()])
+        ax.set_yticklabels([insert_linebreak(_item.get_text(), **kwargs)
+                           for _item in ax.get_yticklabels()])
 
 
 @docstr
 @export
 def annotate_barplot(ax: plt.Axes = None, x: Sequence = None, y: Sequence = None, ci: bool = True,
                      ci_newline: bool = True, adj_ylim: float = .05, nr_format: str = None,
                      ha: str = 'center', va: str = 'center', offset: int = None,
@@ -2272,15 +2336,16 @@
                 _line = ax.lines[_it]
 
                 _line_y = _line.get_xydata()[:, 1]
                 _ci = (_line_y[1] - _line_y[0]) / 2
 
                 if not np.isnan(_ci):
                     _ci_text = format(_ci, nr_format)
-                    _annotate = r'${}$'.format(_val_text) + _ci_sep + r'$\pm{}$'.format(_ci_text)
+                    _annotate = r'${}$'.format(
+                        _val_text) + _ci_sep + r'$\pm{}$'.format(_ci_text)
 
             ax.annotate(_annotate, (_x, _y), ha=ha, va=va, xytext=(0, np.sign(_val) * _offset),
                         textcoords='offset points', **kwargs)
 
         except Exception as exc:
             print(exc)
 
@@ -2483,16 +2548,18 @@
                     _line['label'] = y
 
                 # update keys
                 _keys = list(_line.keys())
 
             # get kws
             _line_kws = {}
-            _line_kw_keys = [_ for _ in _keys if _ not in ['ax', 'line', 'ts', 'data', 'x', 'y', 't']]
-            _kw_keys = [_ for _ in list(kwargs.keys()) if _ not in _line_kw_keys]
+            _line_kw_keys = [_ for _ in _keys if _ not in [
+                'ax', 'line', 'ts', 'data', 'x', 'y', 't']]
+            _kw_keys = [_ for _ in list(
+                kwargs.keys()) if _ not in _line_kw_keys]
 
             for _key in _line_kw_keys:
                 _line_kws[_key] = _line[_key]
             for _kw_key in _kw_keys:
                 _line_kws[_kw_key] = kwargs[_kw_key]
 
             if 'ax' not in _keys:
@@ -2502,17 +2569,19 @@
             if is_list_like(_line['line']):
                 _line['line'] = _line['line'][0]
 
             for _arg in list(_args.keys()):
                 if _arg not in _keys:
                     _line[_arg] = _args[_arg]
 
-            _line['ts'] = _line['data'][_line['t']].drop_duplicates().sort_values().reset_index(drop=True)
+            _line['ts'] = _line['data'][_line['t']].drop_duplicates(
+            ).sort_values().reset_index(drop=True)
 
-            _ts = _ts.append(_line['ts']).drop_duplicates().sort_values().reset_index(drop=True)
+            _ts = _ts.append(_line['ts']).drop_duplicates(
+            ).sort_values().reset_index(drop=True)
 
     # get max interval
     if max_interval is not None:
         if max_interval < _ts.shape[0]:
             _max_interval = max_interval
         else:
             _max_interval = _ts.shape[0]
@@ -2573,15 +2642,16 @@
                     # -- vlines --
                     if 'vline' in __line.keys():
                         _vline_i = __line['vline']
                         if _vline_i is not None:
                             if not is_list_like(_vline_i):
                                 _vline_i = [_vline_i]
                             for _vline_j in _vline_i:
-                                __ax.axvline(_vline_j, color='k', linestyle=':')
+                                __ax.axvline(
+                                    _vline_j, color='k', linestyle=':')
 
             # -- lims --
             if xlim is not None:
                 if xlim:
                     __ax.set_xlim(xlim)
             else:
                 __ax.set_xlim([_x_min, _x_max])
@@ -2617,20 +2687,14 @@
 
             _data = _line_i['data'].copy()
             _data = _data[_data[_line_i['t']] == _t]
 
             if hue:
                 __hue = hue_order[__it]
                 _data = _data[_data[hue] == __hue]
-                if isinstance(palette, Mapping):
-                    __color = palette[__hue]
-                elif is_list_like(palette):
-                    __color = palette[__it]
-                else:
-                    __color = palette
                 _line_i['line'].set_markerfacecolor(_color)
             _line_i['line'].set_data(_data[_line_i['x']], _data[_line_i['y']])
 
             # -- title --
             _title = title
             _title_prefix = title_prefix
 
@@ -2662,15 +2726,16 @@
     for _line in lines:
         if 'ax' in list(_line.keys()):
             _ax = _line['ax']
         else:
             _ax = plt.gca()
 
     # - create main FuncAnimation object
-    _anim = FuncAnimation(fig, animate, init_func=init, frames=_max_interval, interval=time_per_frame, blit=True)
+    _anim = FuncAnimation(fig, animate, init_func=init,
+                          frames=_max_interval, interval=time_per_frame, blit=True)
     # - close plots
     plt.close('all')
 
     # -- return
     # -handle return mode
     if mode == 'html':
         return HTML(_anim.to_html5_video())
@@ -2703,22 +2768,24 @@
     if legend_space is None:
         legend_space = rcParams['legend_outside.legend_space']
     if ax is None:
         ax = plt.gca()
     # - check if loc is legend_outside specific, if not treat as inside loc and call regular ax.legend
     if loc not in ['bottom', 'right']:
         if loc_warn:
-            warnings.warn('legend_outside: legend loc not recognized, defaulting to plt.legend')
+            warnings.warn(
+                'legend_outside: legend loc not recognized, defaulting to plt.legend')
         ax.legend(loc=loc, **kwargs)
         return None
 
     # -- main
     # - get loc and bbox
     _loc = {'bottom': 'upper center', 'right': 'center left'}[loc]
-    _bbox_to_anchor = {'bottom': (0.5 + offset_x, - .15 + offset_y), 'right': (1, 0.5)}[loc]
+    _bbox_to_anchor = {'bottom': (
+        0.5 + offset_x, - .15 + offset_y), 'right': (1, 0.5)}[loc]
     # - loop axes
     for _ax in ax_as_list(ax):
 
         # -- shrink box
         _box = _ax.get_position()
         _pos = {
             'bottom': [_box.x0, _box.y0, _box.width, _box.height * (1 - legend_space)],
@@ -2799,15 +2866,16 @@
         _label_test = labels
 
     if ax is None:
         ax = plt.gca()
 
     ax.plot(train, color='xkcd:blue', label=_label_train)
     ax.plot(test, color='xkcd:red', label=_label_test)
-    ax.plot(lfit(test), color='xkcd:red', ls='--', alpha=.75, label=_label_test + '_lfit')
+    ax.plot(lfit(test), color='xkcd:red', ls='--',
+            alpha=.75, label=_label_test + '_lfit')
     ax.axhline(np.min(test), color='xkcd:red', ls=':', alpha=.5)
     ax.axvline(np.argmin(test), color='xkcd:red', ls=':', alpha=.5)
 
     if legend:
         if isinstance(legend, str):
             _loc = legend
         else:
@@ -2873,15 +2941,16 @@
         ax = plt.gca()
 
     # baseline
     ax.axhline(baseline, color='k', ls='--', alpha=.5)
 
     # iterate over data so you can draw the lines
     for _it, _row in _data.iterrows():
-        ax.plot([_row[_x], _row[_x]], [baseline, _row[_y]], color=color, label='__nolegend__', **kwline)
+        ax.plot([_row[_x], _row[_x]], [baseline, _row[_y]],
+                color=color, label='__nolegend__', **kwline)
 
     # scatterplot for markers
     ax.scatter(x=_x, y=_y, data=_data, facecolor=color, **kwargs)
 
     return ax
 
 
@@ -2912,15 +2981,16 @@
         if isinstance(palette, Mapping):
             _color = palette[_name]
         elif is_list_like(palette):
             _color = palette[_labels.index(_name) % len(palette)]
         else:
             _color = palette
 
-        ax.fill_betweenx([y_from, y_to], _row[x_from], _row[x_to], label=_label, color=_color, **kwargs)
+        ax.fill_betweenx([y_from, y_to], _row[x_from],
+                         _row[x_to], label=_label, color=_color, **kwargs)
 
     if legend and label:
         ax.legend(loc=legend_loc)
 
     return ax
 
 
@@ -3215,16 +3285,14 @@
 
     if hue is None:
         hue = '_dummy'
         _df[hue] = 1
     if hue_order is None:
         hue_order = sorted(_df[hue].unique())
 
-    _x = _df[_x_name]
-
     if facecolor is None:
         if show_area:
             facecolor = 'None'
         else:
             facecolor = 'xkcd:cyan'
 
     if show_kde and show_area:
@@ -3265,20 +3333,16 @@
             _df_kde['value'] = _df_kde['value'] / _df_kde['value'].max()
             _df_kde_ex['value'] = _df_kde_ex['value'] / _df_kde['value'].max()
 
         if adj_x_range:
             _x_min = _df_kde_ex['range_min'].min()
             _x_max = _df_kde_ex['range_max'].max()
 
-            _x_step = (_x_max - _x_min) / bins
-            _x_range_min = _x_min - _x_step * adj_x_range * bins
-            _x_range_max = _x_max + _x_step * adj_x_range * bins
-
-            _df_hue = _df_hue.query('{}>=@_x_range_min & {}<=@_x_range_max'.format(_x_name, _x_name))
-            _df_kde = _df_kde.query('{}>=@_x_range_min & {}<=@_x_range_max'.format(_x_name, _x_name))
+            _df_hue = _df_hue[lambda _: (_x_min >= _['_x_range_min']) & (_x_max <= _['_x_range_min'])]
+            _df_kde = _df_kde[lambda _: (_x_min >= _['_x_range_min']) & (_x_max <= _['_x_range_min'])]
 
         # -- plot
 
         if ax is None:
             ax = plt.gca()
 
         # hist
@@ -3290,35 +3354,33 @@
             _twinx = False
 
         if _twinx and (ax2 is None):
             ax2 = ax.twinx()
         else:
             ax2 = ax
 
-        _kde_label = '{} ; '.format(_x_name) + r'${:,.2f}\pm{:,.2f}$'.format(_df[_x_name].mean(), _df[_x_name].std())
+        _kde_label = '{} ; '.format(
+            _x_name) + r'${:,.2f}\pm{:,.2f}$'.format(_df[_x_name].mean(), _df[_x_name].std())
 
         # kde
-        ax2.plot(_df_kde[_x_name], _df_kde['value'], ls='--', label=_kde_label, color=_kde_color, **kwargs)
+        ax2.plot(_df_kde[_x_name], _df_kde['value'], ls='--',
+                 label=_kde_label, color=_kde_color, **kwargs)
 
         _ylim = list(ax2.get_ylim())
         _ylim[0] = 0
         _ylim[1] = _ylim[1] * (100 + text_offset) / 100.
         ax2.set_ylim(_ylim)
 
         # area
         if show_area:
 
             # get max
             if area_center == 'max':
-                _area_center = _df_kde[_df_kde['value'] == _df_kde['value'].max()].index[0]
-            else:
-                if area_center == 'mean':
-                    _ref = _df_hue[_x_name].mean()
-                else:
-                    _ref = area_center
+                _area_center = _df_kde[_df_kde['value']
+                                       == _df_kde['value'].max()].index[0]
 
                 _df_area = _df_kde.copy()
                 _df_area['diff'] = (_df_area[_x_name] - area_center).abs()
                 _df_area = _df_area.sort_values(by='diff', ascending=True)
                 _area_center = _df_area.index[0]
 
             _sigma = None
@@ -3335,29 +3397,31 @@
                 if (_perc_data >= .9544) and (_2_sigma is None):
                     _2_sigma = _it + 0
                     break
                 if _it == _df_kde.shape[0] - 1:
                     _2_sigma = _it + 0
 
             _df_sigma = _df_kde.loc[
-                        np.max([0, _area_center - _sigma]):np.min([_df_kde.shape[0], _area_center + _sigma])]
+                np.max([0, _area_center - _sigma]):np.min([_df_kde.shape[0], _area_center + _sigma])]
             _df_2_sigma_left = _df_kde.loc[
-                               np.max([0, _area_center - _2_sigma]):np.min([_df_kde.shape[0], _area_center - _sigma])]
+                np.max([0, _area_center - _2_sigma]):np.min([_df_kde.shape[0], _area_center - _sigma])]
             _df_2_sigma_right = _df_kde.loc[
-                                np.max([0, _area_center + _sigma]):np.min([_df_kde.shape[0], _area_center + _2_sigma])]
+                np.max([0, _area_center + _sigma]):np.min([_df_kde.shape[0], _area_center + _2_sigma])]
 
             _2_sigma_min = _df_2_sigma_left[_x_name].min()
             _2_sigma_max = _df_2_sigma_right[_x_name].max()
             if np.isnan(_2_sigma_min):
                 _2_sigma_min = _df[_x_name].min()
             if np.isnan(_2_sigma_max):
                 _2_sigma_max = _df[_x_name].max()
 
-            _sigma_range = ': {:,.2f} to {:,.2f}'.format(_df_sigma[_x_name].min(), _df_sigma[_x_name].max())
-            _2_sigma_range = ': {:,.2f} to {:,.2f}'.format(_2_sigma_min, _2_sigma_max)
+            _sigma_range = ': {:,.2f} to {:,.2f}'.format(
+                _df_sigma[_x_name].min(), _df_sigma[_x_name].max())
+            _2_sigma_range = ': {:,.2f} to {:,.2f}'.format(
+                _2_sigma_min, _2_sigma_max)
 
             ax2.fill_between(_x_name, 'value', data=_df_sigma, color=sigma_color,
                              label=r'$1\sigma(68\%)$' + _sigma_range, alpha=alpha)
             ax2.fill_between(_x_name, 'value', data=_df_2_sigma_left, color=sigma_2_color,
                              label=r'$2\sigma(95\%)$' + _2_sigma_range, alpha=alpha)
             ax2.fill_between(_x_name, 'value', data=_df_2_sigma_right, color=sigma_2_color, label='__nolegend__',
                              alpha=alpha)
@@ -3368,22 +3432,24 @@
 
             for _it, _row in _df_kde_ex.iterrows():
 
                 _mu = _row[_x_name]
                 _value_std = np.min([_row['value_min'], _row['value_max']])
 
                 # stem (max)
-                ax2.plot([_mu, _mu], [baseline, _row['value']], color=kde_color, label='__nolegend__', ls=':', **kwline)
+                ax2.plot([_mu, _mu], [baseline, _row['value']],
+                         color=kde_color, label='__nolegend__', ls=':', **kwline)
                 # std
                 if highlight_peaks != 'max':
                     ax2.plot([_row['range_min'], _row['range_max']], [_value_std, _value_std],
                              color=kde_color, label='__nolegend__', ls=':', **kwline)
 
                 # scatterplot for markers
-                ax2.scatter(x=_mu, y=_row['value'], facecolor=kde_color, **kwargs)
+                ax2.scatter(x=_mu, y=_row['value'],
+                            facecolor=kde_color, **kwargs)
 
                 _mean_str = format(_mu, nr_format)
                 _std_str = format(_row['range'] / 2., nr_format)
 
                 _annotate = r'${}$'.format(_mean_str)
                 if highlight_peaks != 'max':
                     _annotate += '\n' + r'$\pm{}$'.format(_std_str)
@@ -3421,15 +3487,16 @@
     :param kwargs: other keyword arguments passed to `seaborn barplot
         <https://seaborn.pydata.org/generated/seaborn.barplot.html>`_
     :return: %(ax_out)s
     """
     _data = []
     for _it in data.index:
 
-        _data_i = pd.concat([data.loc[_it:_it]] * 3, ignore_index=True, sort=False)
+        _data_i = pd.concat([data.loc[_it:_it]] * 3,
+                            ignore_index=True, sort=False)
         _row = data.loc[_it]
 
         if xerr is not None:
             _data_i[x] = [_row[x] - _row[xerr], _row[x], _row[x] + _row[xerr]]
         if yerr is not None:
             _data_i[y] = [_row[y] - _row[yerr], _row[y], _row[y] + _row[yerr]]
         _data.append(_data_i)
@@ -3483,15 +3550,16 @@
         _x = 'x'
 
     _xs = _df_plot[_x]
 
     # if applicable: filter data
     if use_q_xlim:
         _x_lim = q_plim(_xs)
-        _df_plot = _df_plot[(_df_plot[_x] >= _x_lim[0]) & (_df_plot[_x] <= _x_lim[1])]
+        _df_plot = _df_plot[(_df_plot[_x] >= _x_lim[0]) &
+                            (_df_plot[_x] <= _x_lim[1])]
         _xs = _df_plot[_x]
 
     # create bins
     if not isinstance(bins, list):
         bins = np.linspace(_xs.min(), _xs.max(), bins)
 
     # if an axis has not been passed initialize one
@@ -3571,15 +3639,14 @@
             data = x.copy().assign(_dummy=1)
         else:
             # assume passed object is a Sequence and create dummy df
             data = pd.DataFrame({'_dummy': x})
         x = '_dummy'
 
     _count_x = 'count_{}'.format(x)
-    _count_hue = 'count_{}'.format(hue)
 
     # if an axis has not been passed initialize one
     if ax is None:
         ax = plt.gca()
 
     if normalize_x:
         _y = 'perc_{}'.format(x)
@@ -3587,23 +3654,21 @@
         _y = 'perc_{}'.format(hue)
     else:
         _y = 'count'
 
     _df_count = df_count(x=x, df=data, hue=hue, **kwargs)
 
     if order is None or order == 'count':
-        _order = _df_count[[x, _count_x]].drop_duplicates().sort_values(by=[_count_x], ascending=False)[x].tolist()
+        _order = _df_count[[x, _count_x]].drop_duplicates().sort_values(
+            by=[_count_x], ascending=False)[x].tolist()
     elif order == 'sorted':
         _order = _df_count[x].drop_duplicates().sort_values().tolist()
     else:
         _order = order
 
-    if hue is not None:
-        _hues = _get_ordered_levels(data=data, level=hue, order=hue_order, x=x)
-
     if palette is None:
         palette = rcParams['palette'] * 5
 
     sns.barplot(data=_df_count, x=x, y=_y, hue=hue, order=_order, hue_order=hue_order, palette=palette, ax=ax,
                 **barplot_kws)
     ax.set_xlabel('')
 
@@ -3641,15 +3706,16 @@
         _count_twinx_kws_keys = list(count_twinx_kws.keys())
         if 'marker' not in _count_twinx_kws_keys:
             count_twinx_kws['marker'] = '_'
         if 'color' not in _count_twinx_kws_keys:
             count_twinx_kws['color'] = 'k'
         if 'alpha' not in _count_twinx_kws_keys:
             count_twinx_kws['alpha'] = .5
-        _ax.scatter(x, _count_x, data=_df_count[[x, _count_x]].drop_duplicates(), **count_twinx_kws)
+        _ax.scatter(x, _count_x, data=_df_count[[
+                    x, _count_x]].drop_duplicates(), **count_twinx_kws)
         _ax.set_ylabel('count')
 
     return ax
 
 
 @docstr
 @export
@@ -3761,15 +3827,16 @@
     :param kws_dropdown: Other keyword arguments passed to the dropdown updatemenu [optional]
     :param kws_fig: other keyword arguments passed to plotly.graph_objects.Figure [optional]
     :param kwargs: other keyword arguments passed to plotly.graph_objects.scatter [optional]
     :return: plotly Figure with the plot on it
     """
     # -- assert
     if (y_min is not None and y_max is None) or (y_min is None and y_max is not None):
-        raise ValueError('If you supply y_min or y_max you must also supply the other')
+        raise ValueError(
+            'If you supply y_min or y_max you must also supply the other')
 
     # -- functions
     def _get_xy(fltr: tuple = None, hue_i: Scalar = None) -> tuple:
         _df = data.copy()
         if hue != '__dummy__':
             _df = _df[_df[hue] == hue_i]
         if fltr is not None:
@@ -3822,15 +3889,16 @@
     # - scatter
     for _hue in _hues:
         _x, _y = _get_xy(hue_i=_hue)
         fig.add_trace(go.Scatter(x=_x, y=_y, mode=mode, name=_hue, **kwargs))
     # - concat groupbys
     _groupby_dict = {}
     for _groupby in groupby:
-        _groupby_dict[_groupby] = ['<ALL>'] + data[_groupby].drop_duplicates().sort_values().tolist()
+        _groupby_dict[_groupby] = ['<ALL>'] + \
+            data[_groupby].drop_duplicates().sort_values().tolist()
     _groupby_values = list(itertools.product(*list(_groupby_dict.values())))
     _len_groupby_values = len(_groupby_values)
     # - updatemenus
     _updatemenus = []
     _buttons = []
     for _it_group, _category in enumerate(_groupby_values):
         # show progressbar
@@ -3874,15 +3942,16 @@
     # # - annotation (not properly aligned, therefore dropped for now)
     # _annotation = sep.join([str(_) for _ in force_list(groupby)])
     # _fig.update_layout(annotations=[
     #     go.layout.Annotation(text=_annotation, showarrow=False, x=dropdown_x, y=dropdown_y+.1, xref="paper",
     #                          yref="paper", align="left")
     # ])
     # - title / axis titles
-    fig.update_layout(title=title, xaxis_title=xaxis_title, yaxis_title=yaxis_title)
+    fig.update_layout(title=title, xaxis_title=xaxis_title,
+                      yaxis_title=yaxis_title)
     # - y_min / y_max
     if y_min is not None:
         fig.update_yaxes(range=[y_min, y_max])
     # - final progressbar
     if do_print:
         progressbar()
 
@@ -3914,15 +3983,16 @@
         return _color
 
     # -- assert
     # - no inplace
     s = pd.Series(s).copy()
     # - out_type
     if out_type not in validations['cat_to_color__out_type']:
-        raise ValueError(f"out_type must be one of {validations['cat_to_color__out_type']}")
+        raise ValueError(
+            f"out_type must be one of {validations['cat_to_color__out_type']}")
 
     # -- init
     # - defaults
     if palette is None:
         palette = rcParams['palette']
     palette = assert_list(palette)
```

### Comparing `hhpy-0.3.0/hhpy/regression.py` & `hhpy-0.3.1/hhpy/regression.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,24 +74,26 @@
         self.output_size = y.shape[1]
 
         # -- init model
         _model = keras.Sequential()
         # -- add double conv 1d layer
         _model.add(keras.layers.Conv1D(filters=self.filters, kernel_size=self.kernel_size, activation=self.activation,
                                        input_shape=(self.window, self.input_size)))
-        _model.add(keras.layers.Conv1D(filters=self.filters, kernel_size=self.kernel_size, activation=self.activation))
+        _model.add(keras.layers.Conv1D(filters=self.filters,
+                   kernel_size=self.kernel_size, activation=self.activation))
         # -- add dropout layer
         if self.dropout:
             _model.add(keras.layers.Dropout(self.dropout))
         # -- add pool layer
         if self.pool_size:
             _model.add(keras.layers.MaxPooling1D(pool_size=self.pool_size))
         # -- flatten and dense to get to output shape
         _model.add(keras.layers.Flatten())
-        _model.add(keras.layers.Dense(self.output_size, activation=self.activation))
+        _model.add(keras.layers.Dense(
+            self.output_size, activation=self.activation))
         # -- compile
         _model.compile(loss=self.loss, optimizer=self.optimizer)
         # -- return
         return _model
 
     def reset(self):
 
@@ -114,15 +116,16 @@
         # - reset
         if reset or self.model is None:
             self.model = self._init_model(X=X, y=y)
             self.epochs_trained = 0
 
         # -- main
         # - call member model fit
-        self.model.fit(x=X, y=y, epochs=epochs, batch_size=self.batch_size, verbose=verbose)
+        self.model.fit(x=X, y=y, epochs=epochs,
+                       batch_size=self.batch_size, verbose=verbose)
         self.epochs_trained += epochs
 
     def predict(self, X, groupby: SequenceOrScalar = None):
 
         # -- assert
         _X = to_keras_3d(X, window=self.window, dropna=False, groupby=groupby)
```

### Comparing `hhpy-0.3.0/release_notes.md` & `hhpy-0.3.1/release_notes.md`

 * *Files identical despite different names*

### Comparing `hhpy-0.3.0/setup.py` & `hhpy-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_description_content_type='text/markdown',
     version=about['__version__'],
     author=about['__author__'],
     author_email=about['__author_email__'],
     url=about['__url__'],
     packages=['hhpy'],
     include_package_data=True,
-    python_requires=">=3.6.*",
+    python_requires=">=3.8",
     install_requires=['numpy', 'pandas', 'scipy', 'matplotlib', 'scikit-learn', 'seaborn', 'colour', 'pytest',
                       'requests', 'IPython', 'docrep', 'h5py', 'openpyxl', 'xlrd'],
     license=about['__license__'],
     zip_safe=False,
     entry_points={
         'console_scripts': ['main=hhpy.entry_points:main'],
     },
```

### Comparing `hhpy-0.3.0/sphinx/.DS_Store` & `hhpy-0.3.1/sphinx/.DS_Store`

 * *Files identical despite different names*

### Comparing `hhpy-0.3.0/sphinx/Makefile` & `hhpy-0.3.1/sphinx/Makefile`

 * *Files identical despite different names*

### Comparing `hhpy-0.3.0/sphinx/_static/.DS_Store` & `hhpy-0.3.1/sphinx/_static/.DS_Store`

 * *Files identical despite different names*

### Comparing `hhpy-0.3.0/sphinx/api/.DS_Store` & `hhpy-0.3.1/sphinx/api/.DS_Store`

 * *Files identical despite different names*

### Comparing `hhpy-0.3.0/sphinx/api/hhpy.ds.DFMapping.rst` & `hhpy-0.3.1/sphinx/api/hhpy.ds.DFMapping.rst`

 * *Files identical despite different names*

### Comparing `hhpy-0.3.0/sphinx/api/hhpy.main.BaseClass.rst` & `hhpy-0.3.1/sphinx/api/hhpy.main.BaseClass.rst`

 * *Files identical despite different names*

### Comparing `hhpy-0.3.0/sphinx/api/hhpy.modelling.Models.rst` & `hhpy-0.3.1/sphinx/api/hhpy.modelling.Models.rst`

 * *Files identical despite different names*

### Comparing `hhpy-0.3.0/sphinx/conf.py` & `hhpy-0.3.1/sphinx/conf.py`

 * *Files identical despite different names*

### Comparing `hhpy-0.3.0/sphinx/make.bat` & `hhpy-0.3.1/sphinx/make.bat`

 * *Files identical despite different names*

### Comparing `hhpy-0.3.0/sphinx/quickstart.rst` & `hhpy-0.3.1/sphinx/quickstart.rst`

 * *Files identical despite different names*

### Comparing `hhpy-0.3.0/tests/files/testdata_jp.xlsx` & `hhpy-0.3.1/tests/files/testdata_jp.xlsx`

 * *Files identical despite different names*

### Comparing `hhpy-0.3.0/tests/files/testdata_jp_dfmapping.xlsx` & `hhpy-0.3.1/tests/files/testdata_jp_dfmapping.xlsx`

 * *Files identical despite different names*

### Comparing `hhpy-0.3.0/tests/test_ds.py` & `hhpy-0.3.1/tests/test_ds.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 tests for hhpy.ds
 """
 
 import pytest
-import hhpy.main as hmn
 import hhpy.ds as hds
 import pandas as pd
 import os
 
 
 # --- fixtures
 @pytest.fixture
```

