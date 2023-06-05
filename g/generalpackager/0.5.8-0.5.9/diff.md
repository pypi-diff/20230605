# Comparing `tmp/generalpackager-0.5.8.tar.gz` & `tmp/generalpackager-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generalpackager-0.5.8.tar", last modified: Fri Jun  2 21:27:54 2023, max compression
+gzip compressed data, was "generalpackager-0.5.9.tar", last modified: Mon Jun  5 09:31:23 2023, max compression
```

## Comparing `generalpackager-0.5.8.tar` & `generalpackager-0.5.9.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:54.916512 generalpackager-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-02 21:27:18.000000 generalpackager-0.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-02 21:27:18.000000 generalpackager-0.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    50789 2023-06-02 21:27:54.912512 generalpackager-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    49940 2023-06-02 21:27:26.000000 generalpackager-0.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:54.904512 generalpackager-0.5.8/generalpackager/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:54.908512 generalpackager-0.5.8/generalpackager/api/
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/localmodule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:54.904512 generalpackager-0.5.8/generalpackager/api/localrepo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:54.908512 generalpackager-0.5.8/generalpackager/api/localrepo/base/
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/localrepo/base/localrepo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/localrepo/base/localrepo_git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/localrepo/base/localrepo_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/localrepo/base/localrepo_target.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/localrepo/base/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:54.908512 generalpackager-0.5.8/generalpackager/api/localrepo/node/
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/localrepo/node/localrepo_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/localrepo/node/metadata_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:54.908512 generalpackager-0.5.8/generalpackager/api/localrepo/python/
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/localrepo/python/localrepo_python.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/localrepo/python/metadata_python.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:54.908512 generalpackager-0.5.8/generalpackager/api/localrepo/top/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/localrepo/top/target_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:54.908512 generalpackager-0.5.8/generalpackager/api/package_hosts/
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/package_hosts/github.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/package_hosts/npm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/package_hosts/pypi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:54.908512 generalpackager-0.5.8/generalpackager/api/shared/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/decos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:54.908512 generalpackager-0.5.8/generalpackager/api/shared/files/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:54.912512 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/commit_editmsg.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/exeproduct.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/exetarget.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/git_exclude.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/gitignore.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/index_js.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/init.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/license.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/npm_ignore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/org_readme.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/package_json.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/pre_commit_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/pre_push_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    12255 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/readme.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/test_js.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/test_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     9509 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/definitions/workflow_dev.py
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/file_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/files/shared_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/name.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/shared/target.py
--rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/venv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/api/venv_cruds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:54.912512 generalpackager-0.5.8/generalpackager/other/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/other/envvars.py
--rw-r--r--   0 runner    (1001) docker     (123)    12684 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/other/licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/packager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/packager_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/packager_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/packager_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/packager_github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/packager_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/packager_pypi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/packager_relations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/packager_workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:54.912512 generalpackager-0.5.8/generalpackager/test/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/test/test_generalpackager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/test/test_github.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/test/test_local_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/test/test_local_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/test/test_local_repo_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/test/test_local_repo_python.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/test/test_packager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/test/test_packager_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/test/test_packager_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/test/test_packager_github.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/test/test_packager_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/test/test_packager_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/test/test_packager_pypi.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/test/test_packager_relations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/test/test_pypi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/test/test_shared.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-02 21:25:05.000000 generalpackager-0.5.8/generalpackager/test/test_venv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:54.908512 generalpackager-0.5.8/generalpackager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    50789 2023-06-02 21:27:54.000000 generalpackager-0.5.8/generalpackager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-06-02 21:27:54.000000 generalpackager-0.5.8/generalpackager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 21:27:54.000000 generalpackager-0.5.8/generalpackager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-02 21:27:54.000000 generalpackager-0.5.8/generalpackager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-02 21:27:54.000000 generalpackager-0.5.8/generalpackager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-02 21:27:18.000000 generalpackager-0.5.8/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 21:27:54.916512 generalpackager-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-02 21:27:26.000000 generalpackager-0.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:31:23.978011 generalpackager-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 09:30:44.000000 generalpackager-0.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-05 09:30:44.000000 generalpackager-0.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    50789 2023-06-05 09:31:23.978011 generalpackager-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    49940 2023-06-05 09:30:53.000000 generalpackager-0.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:31:23.966010 generalpackager-0.5.9/generalpackager/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:31:23.970010 generalpackager-0.5.9/generalpackager/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/localmodule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:31:23.966010 generalpackager-0.5.9/generalpackager/api/localrepo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:31:23.970010 generalpackager-0.5.9/generalpackager/api/localrepo/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/localrepo/base/localrepo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/localrepo/base/localrepo_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/localrepo/base/localrepo_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/localrepo/base/localrepo_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/localrepo/base/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:31:23.970010 generalpackager-0.5.9/generalpackager/api/localrepo/node/
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/localrepo/node/localrepo_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/localrepo/node/metadata_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:31:23.970010 generalpackager-0.5.9/generalpackager/api/localrepo/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/localrepo/python/localrepo_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/localrepo/python/metadata_python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:31:23.970010 generalpackager-0.5.9/generalpackager/api/localrepo/top/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/localrepo/top/target_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:31:23.970010 generalpackager-0.5.9/generalpackager/api/package_hosts/
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/package_hosts/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/package_hosts/npm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/package_hosts/pypi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:31:23.970010 generalpackager-0.5.9/generalpackager/api/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/shared/decos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:31:23.970010 generalpackager-0.5.9/generalpackager/api/shared/files/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:31:23.974011 generalpackager-0.5.9/generalpackager/api/shared/files/definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/shared/files/definitions/commit_editmsg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/shared/files/definitions/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/shared/files/definitions/exeproduct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/shared/files/definitions/exetarget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/shared/files/definitions/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/shared/files/definitions/git_exclude.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/shared/files/definitions/gitignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/shared/files/definitions/index_js.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/shared/files/definitions/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/shared/files/definitions/license.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/shared/files/definitions/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/shared/files/definitions/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/shared/files/definitions/npm_ignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/shared/files/definitions/org_readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/shared/files/definitions/package_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/shared/files/definitions/pre_commit_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/shared/files/definitions/pre_push_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12255 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/shared/files/definitions/readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/shared/files/definitions/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/shared/files/definitions/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/shared/files/definitions/test_js.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/shared/files/definitions/test_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9509 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/shared/files/definitions/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/shared/files/definitions/workflow_dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/shared/files/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/shared/files/file_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/shared/files/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/shared/files/shared_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/shared/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/shared/owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/shared/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/shared/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/shared/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/venv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/api/venv_cruds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:31:23.974011 generalpackager-0.5.9/generalpackager/other/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/other/envvars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12684 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/other/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/packager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/packager_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/packager_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/packager_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/packager_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/packager_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/packager_pypi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/packager_relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/packager_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:31:23.978011 generalpackager-0.5.9/generalpackager/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/test/test_generalpackager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/test/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/test/test_local_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/test/test_local_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/test/test_local_repo_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/test/test_local_repo_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/test/test_packager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/test/test_packager_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/test/test_packager_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/test/test_packager_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/test/test_packager_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/test/test_packager_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/test/test_packager_pypi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/test/test_packager_relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/test/test_pypi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/test/test_shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-05 09:27:55.000000 generalpackager-0.5.9/generalpackager/test/test_venv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:31:23.966010 generalpackager-0.5.9/generalpackager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    50789 2023-06-05 09:31:23.000000 generalpackager-0.5.9/generalpackager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-06-05 09:31:23.000000 generalpackager-0.5.9/generalpackager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 09:31:23.000000 generalpackager-0.5.9/generalpackager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-05 09:31:23.000000 generalpackager-0.5.9/generalpackager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-05 09:31:23.000000 generalpackager-0.5.9/generalpackager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-05 09:30:44.000000 generalpackager-0.5.9/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 09:31:23.978011 generalpackager-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-05 09:30:53.000000 generalpackager-0.5.9/setup.py
```

### Comparing `generalpackager-0.5.8/LICENSE` & `generalpackager-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/PKG-INFO` & `generalpackager-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generalpackager
-Version: 0.5.8
+Version: 0.5.9
 Summary: Tools to interface GitHub, PyPI, NPM and local modules / repos. Used for generating files to keep projects dry and synced. Tailored for ManderaGeneral for now.
 Home-page: https://github.com/ManderaGeneral/generalpackager
 Author: Rickard "Mandera" Abraham
 Author-email: rickard.abraham@gmail.com
 License: mit
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3.8
@@ -38,21 +38,21 @@
 
 
 <details open>
 <summary><h2>Dependency Diagram for ManderaGeneral</h2></summary>
 
 ```mermaid
 flowchart LR
-2([library]) --> 5([packager])
 2([library]) --> 4([vector])
-3([file]) --> 5([packager])
-0([import]) --> 3([file])
 1([tool]) --> 2([library])
-0([import]) --> 2([library])
+3([file]) --> 5([packager])
 2([library]) --> 3([file])
+0([import]) --> 2([library])
+0([import]) --> 3([file])
+2([library]) --> 5([packager])
 click 0 "https://github.com/ManderaGeneral/generalimport"
 click 1 "https://github.com/ManderaGeneral/generaltool"
 click 2 "https://github.com/ManderaGeneral/generallibrary"
 click 3 "https://github.com/ManderaGeneral/generalfile"
 click 4 "https://github.com/ManderaGeneral/generalvector"
 click 5 "https://github.com/ManderaGeneral/generalpackager"
 style 5 fill:#482
@@ -77,15 +77,15 @@
 
 
 <details open>
 <summary><h2>Information</h2></summary>
 
 | Package                                                              | Ver                                                | Latest Release        | Python                                                                                                                                                                                                                                                 | Platform        | Cover   |
 |:---------------------------------------------------------------------|:---------------------------------------------------|:----------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------------|:--------|
-| [generalpackager](https://github.com/ManderaGeneral/generalpackager) | [0.5.8](https://pypi.org/project/generalpackager/) | 2023-06-02 23:27 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://www.python.org/downloads/release/python-3100/), [3.11](https://www.python.org/downloads/release/python-3110/) | Windows, Ubuntu | 67.8 %  |
+| [generalpackager](https://github.com/ManderaGeneral/generalpackager) | [0.5.9](https://pypi.org/project/generalpackager/) | 2023-06-05 11:30 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://www.python.org/downloads/release/python-3100/), [3.11](https://www.python.org/downloads/release/python-3110/) | Windows, Ubuntu | 67.8 %  |
 </details>
 
 
 
 <details>
 <summary><h2>Attributes</h2></summary>
 
@@ -359,26 +359,26 @@
 
 
 <details>
 <summary><h2>Todo</h2></summary>
 
 | Module                                                                                                                                                      | Message                                                                                                                                                                                                          |
 |:------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L1'>packager_files.py</a>                          | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L9'>Fix create_blank, it overwrites current projects pip install.</a>                                   |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L1'>packager_github.py</a>                        | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L44'>Setup env vars for project.</a>                                                                   |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L1'>target.py</a>                               | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L39'>Generate Python file in generalpackager containing general packages.</a>                        |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L1'>readme.py</a>             | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L166'>Sort todos by name to decrease automatic commit changes.</a>                 |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L1'>pypi.py</a>                            | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L13'>Move download to it's own package.</a>                                                     |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L1'>pypi.py</a>                            | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L78'>Find a faster fetch for latest PyPI version and datetime.</a>                              |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L1'>github.py</a>                        | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L15'>Get and Set GitHub repo private.</a>                                                     |
 | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L1'>localrepo_python.py</a> | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L77'>Make sure twine is installed when trying to upload to pypi.</a>             |
 | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L1'>localrepo_python.py</a> | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L78'>Look into private PyPI server where we could also do dry runs for test.</a> |
 | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L1'>localrepo.py</a>                 | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L22'>Search for imports to list dependencies.</a>                                         |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L1'>readme.py</a>             | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L166'>Sort todos by name to decrease automatic commit changes.</a>                 |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L1'>target.py</a>                               | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L39'>Generate Python file in generalpackager containing general packages.</a>                        |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L1'>github.py</a>                        | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L15'>Get and Set GitHub repo private.</a>                                                     |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L1'>pypi.py</a>                            | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L13'>Move download to it's own package.</a>                                                     |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L1'>pypi.py</a>                            | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L78'>Find a faster fetch for latest PyPI version and datetime.</a>                              |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L1'>packager_files.py</a>                          | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L9'>Fix create_blank, it overwrites current projects pip install.</a>                                   |
 | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L1'>packager_api.py</a>                              | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L43'>Check that every API has create an *_available method</a>                                            |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L1'>packager_github.py</a>                        | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L44'>Setup env vars for project.</a>                                                                   |
 </details>
 
 
 <sup>
-Generated 2023-06-02 23:27 CEST for commit <a href='https://github.com/ManderaGeneral/generalpackager/commit/master'>master</a>.
+Generated 2023-06-05 11:30 CEST for commit <a href='https://github.com/ManderaGeneral/generalpackager/commit/master'>master</a>.
 </sup>
 </details>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: generalpackager Version: 0.5.8 Summary: Tools to
+Metadata-Version: 2.1 Name: generalpackager Version: 0.5.9 Summary: Tools to
 interface GitHub, PyPI, NPM and local modules / repos. Used for generating
 files to keep projects dry and synced. Tailored for ManderaGeneral for now.
 Home-page: https://github.com/ManderaGeneral/generalpackager Author: Rickard
 "Mandera" Abraham Author-email: rickard.abraham@gmail.com License: mit
 Classifier: Topic :: Software Development :: Build Tools Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
@@ -20,17 +20,17 @@
 ââ Installation_showing_dependencies
 ââ Information
 ââ Attributes
 ââ Contributions
 ââ Todo
 
 ***** Dependency Diagram for ManderaGeneral *****
-```mermaid flowchart LR 2([library]) --> 5([packager]) 2([library]) --> 4(
-[vector]) 3([file]) --> 5([packager]) 0([import]) --> 3([file]) 1([tool]) --> 2
-([library]) 0([import]) --> 2([library]) 2([library]) --> 3([file]) click 0
+```mermaid flowchart LR 2([library]) --> 4([vector]) 1([tool]) --> 2([library])
+3([file]) --> 5([packager]) 2([library]) --> 3([file]) 0([import]) --> 2(
+[library]) 0([import]) --> 3([file]) 2([library]) --> 5([packager]) click 0
 "https://github.com/ManderaGeneral/generalimport" click 1 "https://github.com/
 ManderaGeneral/generaltool" click 2 "https://github.com/ManderaGeneral/
 generallibrary" click 3 "https://github.com/ManderaGeneral/generalfile" click 4
 "https://github.com/ManderaGeneral/generalvector" click 5 "https://github.com/
 ManderaGeneral/generalpackager" style 5 fill:#482 ```
 ***** Installation showing dependencies *****
 | `pip install` | `generalpackager` | |:---------------------------------------
@@ -42,16 +42,16 @@
 | Package | Ver | Latest Release | Python | Platform | Cover | |:--------------
 -------------------------------------------------------|:----------------------
 -----------------------------|:----------------------|:------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -----------------------------------------------------------------|:------------
 ----|:--------| | [generalpackager](https://github.com/ManderaGeneral/
-generalpackager) | [0.5.8](https://pypi.org/project/generalpackager/) | 2023-
-06-02 23:27 CEST | [3.8](https://www.python.org/downloads/release/python-380/),
+generalpackager) | [0.5.9](https://pypi.org/project/generalpackager/) | 2023-
+06-05 11:30 CEST | [3.8](https://www.python.org/downloads/release/python-380/),
 [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://
 www.python.org/downloads/release/python-3100/), [3.11](https://www.python.org/
 downloads/release/python-3110/) | Windows, Ubuntu | 67.8 % |
 ***** Attributes *****
 Module:_generalpackager
 ââ Class:_GitHub
 â  ââ Class:_GitHub
@@ -314,18 +314,18 @@
 Issue-creation, discussions and pull requests are most welcome!
 ***** Todo *****
 | Module | Message | |:--------------------------------------------------------
 -------------------------------------------------------------------------------
 ---------------------|:--------------------------------------------------------
 -------------------------------------------------------------------------------
 --------------------------------------------------------------------------| |
-packager_files.py | Fix_create_blank,_it_overwrites_current_projects_pip
-install. | | packager_github.py | Setup_env_vars_for_project. | | target.py |
-Generate_Python_file_in_generalpackager_containing_general_packages. | |
-readme.py | Sort_todos_by_name_to_decrease_automatic_commit_changes. | |
-pypi.py | Move_download_to_it's_own_package. | | pypi.py | Find_a_faster_fetch
-for_latest_PyPI_version_and_datetime. | | github.py | Get_and_Set_GitHub_repo
-private. | | localrepo_python.py | Make_sure_twine_is_installed_when_trying_to
-upload_to_pypi. | | localrepo_python.py | Look_into_private_PyPI_server_where
-we_could_also_do_dry_runs_for_test. | | localrepo.py | Search_for_imports_to
-list_dependencies. | | packager_api.py | Check_that_every_API_has_create_an
-*_available_method |  Generated 2023-06-02 23:27 CEST for commit master.
+localrepo_python.py | Make_sure_twine_is_installed_when_trying_to_upload_to
+pypi. | | localrepo_python.py | Look_into_private_PyPI_server_where_we_could
+also_do_dry_runs_for_test. | | localrepo.py | Search_for_imports_to_list
+dependencies. | | readme.py | Sort_todos_by_name_to_decrease_automatic_commit
+changes. | | target.py | Generate_Python_file_in_generalpackager_containing
+general_packages. | | github.py | Get_and_Set_GitHub_repo_private. | | pypi.py
+| Move_download_to_it's_own_package. | | pypi.py | Find_a_faster_fetch_for
+latest_PyPI_version_and_datetime. | | packager_files.py | Fix_create_blank,_it
+overwrites_current_projects_pip_install. | | packager_api.py | Check_that_every
+API_has_create_an_*_available_method | | packager_github.py | Setup_env_vars
+for_project. |  Generated 2023-06-05 11:30 CEST for commit master.
```

### Comparing `generalpackager-0.5.8/README.md` & `generalpackager-0.5.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -19,21 +19,21 @@
 
 
 <details open>
 <summary><h2>Dependency Diagram for ManderaGeneral</h2></summary>
 
 ```mermaid
 flowchart LR
-2([library]) --> 5([packager])
 2([library]) --> 4([vector])
-3([file]) --> 5([packager])
-0([import]) --> 3([file])
 1([tool]) --> 2([library])
-0([import]) --> 2([library])
+3([file]) --> 5([packager])
 2([library]) --> 3([file])
+0([import]) --> 2([library])
+0([import]) --> 3([file])
+2([library]) --> 5([packager])
 click 0 "https://github.com/ManderaGeneral/generalimport"
 click 1 "https://github.com/ManderaGeneral/generaltool"
 click 2 "https://github.com/ManderaGeneral/generallibrary"
 click 3 "https://github.com/ManderaGeneral/generalfile"
 click 4 "https://github.com/ManderaGeneral/generalvector"
 click 5 "https://github.com/ManderaGeneral/generalpackager"
 style 5 fill:#482
@@ -58,15 +58,15 @@
 
 
 <details open>
 <summary><h2>Information</h2></summary>
 
 | Package                                                              | Ver                                                | Latest Release        | Python                                                                                                                                                                                                                                                 | Platform        | Cover   |
 |:---------------------------------------------------------------------|:---------------------------------------------------|:----------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------------|:--------|
-| [generalpackager](https://github.com/ManderaGeneral/generalpackager) | [0.5.8](https://pypi.org/project/generalpackager/) | 2023-06-02 23:27 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://www.python.org/downloads/release/python-3100/), [3.11](https://www.python.org/downloads/release/python-3110/) | Windows, Ubuntu | 67.8 %  |
+| [generalpackager](https://github.com/ManderaGeneral/generalpackager) | [0.5.9](https://pypi.org/project/generalpackager/) | 2023-06-05 11:30 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://www.python.org/downloads/release/python-3100/), [3.11](https://www.python.org/downloads/release/python-3110/) | Windows, Ubuntu | 67.8 %  |
 </details>
 
 
 
 <details>
 <summary><h2>Attributes</h2></summary>
 
@@ -340,26 +340,26 @@
 
 
 <details>
 <summary><h2>Todo</h2></summary>
 
 | Module                                                                                                                                                      | Message                                                                                                                                                                                                          |
 |:------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L1'>packager_files.py</a>                          | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L9'>Fix create_blank, it overwrites current projects pip install.</a>                                   |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L1'>packager_github.py</a>                        | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L44'>Setup env vars for project.</a>                                                                   |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L1'>target.py</a>                               | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L39'>Generate Python file in generalpackager containing general packages.</a>                        |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L1'>readme.py</a>             | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L166'>Sort todos by name to decrease automatic commit changes.</a>                 |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L1'>pypi.py</a>                            | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L13'>Move download to it's own package.</a>                                                     |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L1'>pypi.py</a>                            | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L78'>Find a faster fetch for latest PyPI version and datetime.</a>                              |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L1'>github.py</a>                        | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L15'>Get and Set GitHub repo private.</a>                                                     |
 | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L1'>localrepo_python.py</a> | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L77'>Make sure twine is installed when trying to upload to pypi.</a>             |
 | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L1'>localrepo_python.py</a> | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L78'>Look into private PyPI server where we could also do dry runs for test.</a> |
 | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L1'>localrepo.py</a>                 | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L22'>Search for imports to list dependencies.</a>                                         |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L1'>readme.py</a>             | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L166'>Sort todos by name to decrease automatic commit changes.</a>                 |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L1'>target.py</a>                               | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L39'>Generate Python file in generalpackager containing general packages.</a>                        |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L1'>github.py</a>                        | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L15'>Get and Set GitHub repo private.</a>                                                     |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L1'>pypi.py</a>                            | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L13'>Move download to it's own package.</a>                                                     |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L1'>pypi.py</a>                            | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L78'>Find a faster fetch for latest PyPI version and datetime.</a>                              |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L1'>packager_files.py</a>                          | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L9'>Fix create_blank, it overwrites current projects pip install.</a>                                   |
 | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L1'>packager_api.py</a>                              | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L43'>Check that every API has create an *_available method</a>                                            |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L1'>packager_github.py</a>                        | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L44'>Setup env vars for project.</a>                                                                   |
 </details>
 
 
 <sup>
-Generated 2023-06-02 23:27 CEST for commit <a href='https://github.com/ManderaGeneral/generalpackager/commit/master'>master</a>.
+Generated 2023-06-05 11:30 CEST for commit <a href='https://github.com/ManderaGeneral/generalpackager/commit/master'>master</a>.
 </sup>
 </details>
```

#### html2text {}

```diff
@@ -8,17 +8,17 @@
 ââ Installation_showing_dependencies
 ââ Information
 ââ Attributes
 ââ Contributions
 ââ Todo
 
 ***** Dependency Diagram for ManderaGeneral *****
-```mermaid flowchart LR 2([library]) --> 5([packager]) 2([library]) --> 4(
-[vector]) 3([file]) --> 5([packager]) 0([import]) --> 3([file]) 1([tool]) --> 2
-([library]) 0([import]) --> 2([library]) 2([library]) --> 3([file]) click 0
+```mermaid flowchart LR 2([library]) --> 4([vector]) 1([tool]) --> 2([library])
+3([file]) --> 5([packager]) 2([library]) --> 3([file]) 0([import]) --> 2(
+[library]) 0([import]) --> 3([file]) 2([library]) --> 5([packager]) click 0
 "https://github.com/ManderaGeneral/generalimport" click 1 "https://github.com/
 ManderaGeneral/generaltool" click 2 "https://github.com/ManderaGeneral/
 generallibrary" click 3 "https://github.com/ManderaGeneral/generalfile" click 4
 "https://github.com/ManderaGeneral/generalvector" click 5 "https://github.com/
 ManderaGeneral/generalpackager" style 5 fill:#482 ```
 ***** Installation showing dependencies *****
 | `pip install` | `generalpackager` | |:---------------------------------------
@@ -30,16 +30,16 @@
 | Package | Ver | Latest Release | Python | Platform | Cover | |:--------------
 -------------------------------------------------------|:----------------------
 -----------------------------|:----------------------|:------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -----------------------------------------------------------------|:------------
 ----|:--------| | [generalpackager](https://github.com/ManderaGeneral/
-generalpackager) | [0.5.8](https://pypi.org/project/generalpackager/) | 2023-
-06-02 23:27 CEST | [3.8](https://www.python.org/downloads/release/python-380/),
+generalpackager) | [0.5.9](https://pypi.org/project/generalpackager/) | 2023-
+06-05 11:30 CEST | [3.8](https://www.python.org/downloads/release/python-380/),
 [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://
 www.python.org/downloads/release/python-3100/), [3.11](https://www.python.org/
 downloads/release/python-3110/) | Windows, Ubuntu | 67.8 % |
 ***** Attributes *****
 Module:_generalpackager
 ââ Class:_GitHub
 â  ââ Class:_GitHub
@@ -302,18 +302,18 @@
 Issue-creation, discussions and pull requests are most welcome!
 ***** Todo *****
 | Module | Message | |:--------------------------------------------------------
 -------------------------------------------------------------------------------
 ---------------------|:--------------------------------------------------------
 -------------------------------------------------------------------------------
 --------------------------------------------------------------------------| |
-packager_files.py | Fix_create_blank,_it_overwrites_current_projects_pip
-install. | | packager_github.py | Setup_env_vars_for_project. | | target.py |
-Generate_Python_file_in_generalpackager_containing_general_packages. | |
-readme.py | Sort_todos_by_name_to_decrease_automatic_commit_changes. | |
-pypi.py | Move_download_to_it's_own_package. | | pypi.py | Find_a_faster_fetch
-for_latest_PyPI_version_and_datetime. | | github.py | Get_and_Set_GitHub_repo
-private. | | localrepo_python.py | Make_sure_twine_is_installed_when_trying_to
-upload_to_pypi. | | localrepo_python.py | Look_into_private_PyPI_server_where
-we_could_also_do_dry_runs_for_test. | | localrepo.py | Search_for_imports_to
-list_dependencies. | | packager_api.py | Check_that_every_API_has_create_an
-*_available_method |  Generated 2023-06-02 23:27 CEST for commit master.
+localrepo_python.py | Make_sure_twine_is_installed_when_trying_to_upload_to
+pypi. | | localrepo_python.py | Look_into_private_PyPI_server_where_we_could
+also_do_dry_runs_for_test. | | localrepo.py | Search_for_imports_to_list
+dependencies. | | readme.py | Sort_todos_by_name_to_decrease_automatic_commit
+changes. | | target.py | Generate_Python_file_in_generalpackager_containing
+general_packages. | | github.py | Get_and_Set_GitHub_repo_private. | | pypi.py
+| Move_download_to_it's_own_package. | | pypi.py | Find_a_faster_fetch_for
+latest_PyPI_version_and_datetime. | | packager_files.py | Fix_create_blank,_it
+overwrites_current_projects_pip_install. | | packager_api.py | Check_that_every
+API_has_create_an_*_available_method | | packager_github.py | Setup_env_vars
+for_project. |  Generated 2023-06-05 11:30 CEST for commit master.
```

### Comparing `generalpackager-0.5.8/generalpackager/__init__.py` & `generalpackager-0.5.9/generalpackager/__init__.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/api/localmodule.py` & `generalpackager-0.5.9/generalpackager/api/localmodule.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/api/localrepo/base/localrepo.py` & `generalpackager-0.5.9/generalpackager/api/localrepo/base/localrepo.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/api/localrepo/base/localrepo_git.py` & `generalpackager-0.5.9/generalpackager/api/localrepo/base/localrepo_git.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/api/localrepo/base/localrepo_paths.py` & `generalpackager-0.5.9/generalpackager/api/localrepo/base/localrepo_paths.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/api/localrepo/base/localrepo_target.py` & `generalpackager-0.5.9/generalpackager/api/localrepo/base/localrepo_target.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/api/localrepo/base/metadata.py` & `generalpackager-0.5.9/generalpackager/api/localrepo/base/metadata.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/api/localrepo/node/localrepo_node.py` & `generalpackager-0.5.9/generalpackager/api/localrepo/node/localrepo_node.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/api/localrepo/python/localrepo_python.py` & `generalpackager-0.5.9/generalpackager/api/localrepo/python/localrepo_python.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/api/localrepo/python/metadata_python.py` & `generalpackager-0.5.9/generalpackager/api/localrepo/python/metadata_python.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/api/package_hosts/github.py` & `generalpackager-0.5.9/generalpackager/api/package_hosts/github.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/api/package_hosts/npm.py` & `generalpackager-0.5.9/generalpackager/api/package_hosts/npm.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/api/package_hosts/pypi.py` & `generalpackager-0.5.9/generalpackager/api/package_hosts/pypi.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/api/shared/files/definitions/generate.py` & `generalpackager-0.5.9/generalpackager/api/shared/files/definitions/generate.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/api/shared/files/definitions/org_readme.py` & `generalpackager-0.5.9/generalpackager/api/shared/files/definitions/org_readme.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/api/shared/files/definitions/package_json.py` & `generalpackager-0.5.9/generalpackager/api/shared/files/definitions/package_json.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/api/shared/files/definitions/pre_push_hook.py` & `generalpackager-0.5.9/generalpackager/api/shared/files/definitions/pre_push_hook.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/api/shared/files/definitions/readme.py` & `generalpackager-0.5.9/generalpackager/api/shared/files/definitions/readme.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/api/shared/files/definitions/setup.py` & `generalpackager-0.5.9/generalpackager/api/shared/files/definitions/setup.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/api/shared/files/definitions/test_js.py` & `generalpackager-0.5.9/generalpackager/api/shared/files/definitions/test_js.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/api/shared/files/definitions/test_template.py` & `generalpackager-0.5.9/generalpackager/api/shared/files/definitions/test_template.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/api/shared/files/definitions/workflow.py` & `generalpackager-0.5.9/generalpackager/api/shared/files/definitions/workflow.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/api/shared/files/definitions/workflow_dev.py` & `generalpackager-0.5.9/generalpackager/api/shared/files/definitions/workflow_dev.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/api/shared/files/file.py` & `generalpackager-0.5.9/generalpackager/api/shared/files/file.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/api/shared/files/file_fetcher.py` & `generalpackager-0.5.9/generalpackager/api/shared/files/file_fetcher.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/api/shared/files/helpers.py` & `generalpackager-0.5.9/generalpackager/api/shared/files/helpers.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/api/shared/files/shared_files.py` & `generalpackager-0.5.9/generalpackager/api/shared/files/shared_files.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/api/shared/name.py` & `generalpackager-0.5.9/generalpackager/api/shared/name.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/api/shared/owner.py` & `generalpackager-0.5.9/generalpackager/api/shared/owner.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/api/shared/path.py` & `generalpackager-0.5.9/generalpackager/api/shared/path.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/api/shared/protocols.py` & `generalpackager-0.5.9/generalpackager/api/shared/protocols.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/api/shared/target.py` & `generalpackager-0.5.9/generalpackager/api/shared/target.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/api/venv.py` & `generalpackager-0.5.9/generalpackager/api/venv.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/api/venv_cruds.py` & `generalpackager-0.5.9/generalpackager/api/venv_cruds.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/other/licenses.py` & `generalpackager-0.5.9/generalpackager/other/licenses.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/packager.py` & `generalpackager-0.5.9/generalpackager/packager.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/packager_api.py` & `generalpackager-0.5.9/generalpackager/packager_api.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/packager_environment.py` & `generalpackager-0.5.9/generalpackager/packager_environment.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/packager_files.py` & `generalpackager-0.5.9/generalpackager/packager_files.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/packager_github.py` & `generalpackager-0.5.9/generalpackager/packager_github.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/packager_metadata.py` & `generalpackager-0.5.9/generalpackager/packager_metadata.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/packager_pypi.py` & `generalpackager-0.5.9/generalpackager/packager_pypi.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/packager_relations.py` & `generalpackager-0.5.9/generalpackager/packager_relations.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/packager_workflow.py` & `generalpackager-0.5.9/generalpackager/packager_workflow.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/test/test_github.py` & `generalpackager-0.5.9/generalpackager/test/test_github.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/test/test_local_module.py` & `generalpackager-0.5.9/generalpackager/test/test_local_module.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/test/test_local_repo.py` & `generalpackager-0.5.9/generalpackager/test/test_local_repo.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/test/test_packager.py` & `generalpackager-0.5.9/generalpackager/test/test_packager.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/test/test_packager_api.py` & `generalpackager-0.5.9/generalpackager/test/test_packager_api.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/test/test_packager_files.py` & `generalpackager-0.5.9/generalpackager/test/test_packager_files.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/test/test_packager_metadata.py` & `generalpackager-0.5.9/generalpackager/test/test_packager_metadata.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/test/test_packager_node.py` & `generalpackager-0.5.9/generalpackager/test/test_packager_node.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/test/test_packager_relations.py` & `generalpackager-0.5.9/generalpackager/test/test_packager_relations.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/test/test_pypi.py` & `generalpackager-0.5.9/generalpackager/test/test_pypi.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/test/test_shared.py` & `generalpackager-0.5.9/generalpackager/test/test_shared.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager/test/test_venv.py` & `generalpackager-0.5.9/generalpackager/test/test_venv.py`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/generalpackager.egg-info/PKG-INFO` & `generalpackager-0.5.9/generalpackager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generalpackager
-Version: 0.5.8
+Version: 0.5.9
 Summary: Tools to interface GitHub, PyPI, NPM and local modules / repos. Used for generating files to keep projects dry and synced. Tailored for ManderaGeneral for now.
 Home-page: https://github.com/ManderaGeneral/generalpackager
 Author: Rickard "Mandera" Abraham
 Author-email: rickard.abraham@gmail.com
 License: mit
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3.8
@@ -38,21 +38,21 @@
 
 
 <details open>
 <summary><h2>Dependency Diagram for ManderaGeneral</h2></summary>
 
 ```mermaid
 flowchart LR
-2([library]) --> 5([packager])
 2([library]) --> 4([vector])
-3([file]) --> 5([packager])
-0([import]) --> 3([file])
 1([tool]) --> 2([library])
-0([import]) --> 2([library])
+3([file]) --> 5([packager])
 2([library]) --> 3([file])
+0([import]) --> 2([library])
+0([import]) --> 3([file])
+2([library]) --> 5([packager])
 click 0 "https://github.com/ManderaGeneral/generalimport"
 click 1 "https://github.com/ManderaGeneral/generaltool"
 click 2 "https://github.com/ManderaGeneral/generallibrary"
 click 3 "https://github.com/ManderaGeneral/generalfile"
 click 4 "https://github.com/ManderaGeneral/generalvector"
 click 5 "https://github.com/ManderaGeneral/generalpackager"
 style 5 fill:#482
@@ -77,15 +77,15 @@
 
 
 <details open>
 <summary><h2>Information</h2></summary>
 
 | Package                                                              | Ver                                                | Latest Release        | Python                                                                                                                                                                                                                                                 | Platform        | Cover   |
 |:---------------------------------------------------------------------|:---------------------------------------------------|:----------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------------|:--------|
-| [generalpackager](https://github.com/ManderaGeneral/generalpackager) | [0.5.8](https://pypi.org/project/generalpackager/) | 2023-06-02 23:27 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://www.python.org/downloads/release/python-3100/), [3.11](https://www.python.org/downloads/release/python-3110/) | Windows, Ubuntu | 67.8 %  |
+| [generalpackager](https://github.com/ManderaGeneral/generalpackager) | [0.5.9](https://pypi.org/project/generalpackager/) | 2023-06-05 11:30 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://www.python.org/downloads/release/python-3100/), [3.11](https://www.python.org/downloads/release/python-3110/) | Windows, Ubuntu | 67.8 %  |
 </details>
 
 
 
 <details>
 <summary><h2>Attributes</h2></summary>
 
@@ -359,26 +359,26 @@
 
 
 <details>
 <summary><h2>Todo</h2></summary>
 
 | Module                                                                                                                                                      | Message                                                                                                                                                                                                          |
 |:------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L1'>packager_files.py</a>                          | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L9'>Fix create_blank, it overwrites current projects pip install.</a>                                   |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L1'>packager_github.py</a>                        | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L44'>Setup env vars for project.</a>                                                                   |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L1'>target.py</a>                               | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L39'>Generate Python file in generalpackager containing general packages.</a>                        |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L1'>readme.py</a>             | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L166'>Sort todos by name to decrease automatic commit changes.</a>                 |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L1'>pypi.py</a>                            | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L13'>Move download to it's own package.</a>                                                     |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L1'>pypi.py</a>                            | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L78'>Find a faster fetch for latest PyPI version and datetime.</a>                              |
-| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L1'>github.py</a>                        | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L15'>Get and Set GitHub repo private.</a>                                                     |
 | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L1'>localrepo_python.py</a> | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L77'>Make sure twine is installed when trying to upload to pypi.</a>             |
 | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L1'>localrepo_python.py</a> | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/python/localrepo_python.py#L78'>Look into private PyPI server where we could also do dry runs for test.</a> |
 | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L1'>localrepo.py</a>                 | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/localrepo/base/localrepo.py#L22'>Search for imports to list dependencies.</a>                                         |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L1'>readme.py</a>             | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/files/definitions/readme.py#L166'>Sort todos by name to decrease automatic commit changes.</a>                 |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L1'>target.py</a>                               | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/shared/target.py#L39'>Generate Python file in generalpackager containing general packages.</a>                        |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L1'>github.py</a>                        | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/github.py#L15'>Get and Set GitHub repo private.</a>                                                     |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L1'>pypi.py</a>                            | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L13'>Move download to it's own package.</a>                                                     |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L1'>pypi.py</a>                            | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/api/package_hosts/pypi.py#L78'>Find a faster fetch for latest PyPI version and datetime.</a>                              |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L1'>packager_files.py</a>                          | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_files.py#L9'>Fix create_blank, it overwrites current projects pip install.</a>                                   |
 | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L1'>packager_api.py</a>                              | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_api.py#L43'>Check that every API has create an *_available method</a>                                            |
+| <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L1'>packager_github.py</a>                        | <a href='https://github.com/ManderaGeneral/generalpackager/blob/master/generalpackager/packager_github.py#L44'>Setup env vars for project.</a>                                                                   |
 </details>
 
 
 <sup>
-Generated 2023-06-02 23:27 CEST for commit <a href='https://github.com/ManderaGeneral/generalpackager/commit/master'>master</a>.
+Generated 2023-06-05 11:30 CEST for commit <a href='https://github.com/ManderaGeneral/generalpackager/commit/master'>master</a>.
 </sup>
 </details>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: generalpackager Version: 0.5.8 Summary: Tools to
+Metadata-Version: 2.1 Name: generalpackager Version: 0.5.9 Summary: Tools to
 interface GitHub, PyPI, NPM and local modules / repos. Used for generating
 files to keep projects dry and synced. Tailored for ManderaGeneral for now.
 Home-page: https://github.com/ManderaGeneral/generalpackager Author: Rickard
 "Mandera" Abraham Author-email: rickard.abraham@gmail.com License: mit
 Classifier: Topic :: Software Development :: Build Tools Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
@@ -20,17 +20,17 @@
 ââ Installation_showing_dependencies
 ââ Information
 ââ Attributes
 ââ Contributions
 ââ Todo
 
 ***** Dependency Diagram for ManderaGeneral *****
-```mermaid flowchart LR 2([library]) --> 5([packager]) 2([library]) --> 4(
-[vector]) 3([file]) --> 5([packager]) 0([import]) --> 3([file]) 1([tool]) --> 2
-([library]) 0([import]) --> 2([library]) 2([library]) --> 3([file]) click 0
+```mermaid flowchart LR 2([library]) --> 4([vector]) 1([tool]) --> 2([library])
+3([file]) --> 5([packager]) 2([library]) --> 3([file]) 0([import]) --> 2(
+[library]) 0([import]) --> 3([file]) 2([library]) --> 5([packager]) click 0
 "https://github.com/ManderaGeneral/generalimport" click 1 "https://github.com/
 ManderaGeneral/generaltool" click 2 "https://github.com/ManderaGeneral/
 generallibrary" click 3 "https://github.com/ManderaGeneral/generalfile" click 4
 "https://github.com/ManderaGeneral/generalvector" click 5 "https://github.com/
 ManderaGeneral/generalpackager" style 5 fill:#482 ```
 ***** Installation showing dependencies *****
 | `pip install` | `generalpackager` | |:---------------------------------------
@@ -42,16 +42,16 @@
 | Package | Ver | Latest Release | Python | Platform | Cover | |:--------------
 -------------------------------------------------------|:----------------------
 -----------------------------|:----------------------|:------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -----------------------------------------------------------------|:------------
 ----|:--------| | [generalpackager](https://github.com/ManderaGeneral/
-generalpackager) | [0.5.8](https://pypi.org/project/generalpackager/) | 2023-
-06-02 23:27 CEST | [3.8](https://www.python.org/downloads/release/python-380/),
+generalpackager) | [0.5.9](https://pypi.org/project/generalpackager/) | 2023-
+06-05 11:30 CEST | [3.8](https://www.python.org/downloads/release/python-380/),
 [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://
 www.python.org/downloads/release/python-3100/), [3.11](https://www.python.org/
 downloads/release/python-3110/) | Windows, Ubuntu | 67.8 % |
 ***** Attributes *****
 Module:_generalpackager
 ââ Class:_GitHub
 â  ââ Class:_GitHub
@@ -314,18 +314,18 @@
 Issue-creation, discussions and pull requests are most welcome!
 ***** Todo *****
 | Module | Message | |:--------------------------------------------------------
 -------------------------------------------------------------------------------
 ---------------------|:--------------------------------------------------------
 -------------------------------------------------------------------------------
 --------------------------------------------------------------------------| |
-packager_files.py | Fix_create_blank,_it_overwrites_current_projects_pip
-install. | | packager_github.py | Setup_env_vars_for_project. | | target.py |
-Generate_Python_file_in_generalpackager_containing_general_packages. | |
-readme.py | Sort_todos_by_name_to_decrease_automatic_commit_changes. | |
-pypi.py | Move_download_to_it's_own_package. | | pypi.py | Find_a_faster_fetch
-for_latest_PyPI_version_and_datetime. | | github.py | Get_and_Set_GitHub_repo
-private. | | localrepo_python.py | Make_sure_twine_is_installed_when_trying_to
-upload_to_pypi. | | localrepo_python.py | Look_into_private_PyPI_server_where
-we_could_also_do_dry_runs_for_test. | | localrepo.py | Search_for_imports_to
-list_dependencies. | | packager_api.py | Check_that_every_API_has_create_an
-*_available_method |  Generated 2023-06-02 23:27 CEST for commit master.
+localrepo_python.py | Make_sure_twine_is_installed_when_trying_to_upload_to
+pypi. | | localrepo_python.py | Look_into_private_PyPI_server_where_we_could
+also_do_dry_runs_for_test. | | localrepo.py | Search_for_imports_to_list
+dependencies. | | readme.py | Sort_todos_by_name_to_decrease_automatic_commit
+changes. | | target.py | Generate_Python_file_in_generalpackager_containing
+general_packages. | | github.py | Get_and_Set_GitHub_repo_private. | | pypi.py
+| Move_download_to_it's_own_package. | | pypi.py | Find_a_faster_fetch_for
+latest_PyPI_version_and_datetime. | | packager_files.py | Fix_create_blank,_it
+overwrites_current_projects_pip_install. | | packager_api.py | Check_that_every
+API_has_create_an_*_available_method | | packager_github.py | Setup_env_vars
+for_project. |  Generated 2023-06-05 11:30 CEST for commit master.
```

### Comparing `generalpackager-0.5.8/generalpackager.egg-info/SOURCES.txt` & `generalpackager-0.5.9/generalpackager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `generalpackager-0.5.8/metadata.json` & `generalpackager-0.5.9/metadata.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'version'": "'0.5.9'"}*

```diff
@@ -18,9 +18,9 @@
     ],
     "name": "generalpackager",
     "private": false,
     "target": "python",
     "topics": [
         "tool"
     ],
-    "version": "0.5.8"
+    "version": "0.5.9"
 }
```

### Comparing `generalpackager-0.5.8/setup.py` & `generalpackager-0.5.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 except FileNotFoundError:
     long_description = 'Readme missing'
 
 setup(
     name="generalpackager",
     author='Rickard "Mandera" Abraham',
     author_email="rickard.abraham@gmail.com",
-    version="0.5.8",
+    version="0.5.9",
     description="Tools to interface GitHub, PyPI, NPM and local modules / repos. Used for generating files to keep projects dry and synced. Tailored for ManderaGeneral for now.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         'generallibrary[table]',
         'generalfile',
         'requests',
```

