# Comparing `tmp/rds2py-0.2.2.tar.gz` & `tmp/rds2py-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rds2py-0.2.2.tar", last modified: Wed May  3 19:46:25 2023, max compression
+gzip compressed data, was "rds2py-0.2.3.tar", last modified: Mon Jun  5 17:43:04 2023, max compression
```

## Comparing `rds2py-0.2.2.tar` & `rds2py-0.2.3.tar`

### file list

```diff
@@ -1,322 +1,324 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.876153 rds2py-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-03 19:46:10.000000 rds2py-0.2.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.836153 rds2py-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.844153 rds2py-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-03 19:46:10.000000 rds2py-0.2.2/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-03 19:46:10.000000 rds2py-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-03 19:46:10.000000 rds2py-0.2.2/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-03 19:46:10.000000 rds2py-0.2.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-03 19:46:10.000000 rds2py-0.2.2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-03 19:46:10.000000 rds2py-0.2.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    13464 2023-05-03 19:46:10.000000 rds2py-0.2.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-03 19:46:10.000000 rds2py-0.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-03 19:46:10.000000 rds2py-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-03 19:46:25.876153 rds2py-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-03 19:46:10.000000 rds2py-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.848153 rds2py-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-03 19:46:10.000000 rds2py-0.2.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.848153 rds2py-0.2.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-03 19:46:10.000000 rds2py-0.2.2/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-03 19:46:10.000000 rds2py-0.2.2/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-03 19:46:10.000000 rds2py-0.2.2/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-05-03 19:46:10.000000 rds2py-0.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-03 19:46:10.000000 rds2py-0.2.2/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-03 19:46:10.000000 rds2py-0.2.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-03 19:46:10.000000 rds2py-0.2.2/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-03 19:46:10.000000 rds2py-0.2.2/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-03 19:46:10.000000 rds2py-0.2.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-03 19:46:10.000000 rds2py-0.2.2/docs/tutorial.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.836153 rds2py-0.2.2/extern/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.848153 rds2py-0.2.2/extern/rds2cpp/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/.git
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.836153 rds2py-0.2.2/extern/rds2cpp/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.848153 rds2py-0.2.2/extern/rds2cpp/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/.github/workflows/doxygenate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/.github/workflows/run-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    14096 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/CMakeCache.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.848153 rds2py-0.2.2/extern/rds2cpp/CMakeFiles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.848153 rds2py-0.2.2/extern/rds2cpp/CMakeFiles/3.26.3/
--rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/CMakeFiles/3.26.3/CMakeCXXCompiler.cmake
--rwxr-xr-x   0 runner    (1001) docker     (123)    15992 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/CMakeFiles/3.26.3/CMakeDetermineCompilerABI_CXX.bin
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/CMakeFiles/3.26.3/CMakeSystem.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.848153 rds2py-0.2.2/extern/rds2cpp/CMakeFiles/3.26.3/CompilerIdCXX/
--rw-r--r--   0 runner    (1001) docker     (123)    26276 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/CMakeFiles/3.26.3/CompilerIdCXX/CMakeCXXCompilerId.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)    16096 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/CMakeFiles/3.26.3/CompilerIdCXX/a.out
--rw-r--r--   0 runner    (1001) docker     (123)    27834 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/CMakeFiles/CMakeConfigureLog.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/CMakeFiles/CMakeDirectoryInformation.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/CMakeFiles/Makefile.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/CMakeFiles/Makefile2
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/CMakeFiles/TargetDirectories.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/CMakeFiles/cmake.check_cache
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/CMakeFiles/progress.marks
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     6583 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.840153 rds2py-0.2.2/extern/rds2cpp/_deps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.848153 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-build/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.848153 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-build/CMakeFiles/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-build/CMakeFiles/CMakeDirectoryInformation.cmake
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-build/CMakeFiles/progress.marks
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-build/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-build/cmake_install.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.848153 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.852153 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/HEAD
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/config
--rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/description
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.852153 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (123)      478 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      896 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/hooks/commit-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     4726 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/hooks/fsmonitor-watchman.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/hooks/post-update.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1643 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-commit.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      416 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-merge-commit.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1374 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-push.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     4898 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-rebase.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-receive.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1492 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     2783 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/hooks/push-to-checkout.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     3650 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/hooks/update.sample
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/index
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.852153 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/info/
--rwxr-xr-x   0 runner    (1001) docker     (123)      240 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/info/exclude
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.852153 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/logs/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/logs/HEAD
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.840153 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/logs/refs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.852153 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/logs/refs/heads/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/logs/refs/heads/master
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.840153 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/logs/refs/remotes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.852153 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/logs/refs/remotes/origin/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/logs/refs/remotes/origin/HEAD
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.840153 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/objects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.852153 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/objects/pack/
--r--r--r--   0 runner    (1001) docker     (123)    28232 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/objects/pack/pack-7240a34dedb6cbf1d892766b378b45d8ae1a08b4.idx
--r--r--r--   0 runner    (1001) docker     (123)  1112566 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/objects/pack/pack-7240a34dedb6cbf1d892766b378b45d8ae1a08b4.pack
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/packed-refs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.840153 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/refs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.852153 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/refs/heads/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/refs/heads/master
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.840153 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/refs/remotes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.852153 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/refs/remotes/origin/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/refs/remotes/origin/HEAD
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.840153 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.856153 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.github/workflows/doxygenate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.github/workflows/run-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.856153 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   108855 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/docs/Doxyfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.840153 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.856153 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/byteme/
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/byteme/GzipFileReader.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/byteme/GzipFileWriter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/byteme/IstreamReader.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/byteme/OstreamWriter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/byteme/PerByte.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/byteme/RawBufferReader.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/byteme/RawBufferWriter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/byteme/RawFileReader.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/byteme/RawFileWriter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/byteme/Reader.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/byteme/SelfClosingFILE.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/byteme/SelfClosingGzFile.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/byteme/SomeBufferReader.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/byteme/SomeFileReader.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/byteme/Writer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/byteme/ZlibBufferReader.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/byteme/ZlibBufferWriter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/byteme/magic_numbers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/byteme/temp_file_path.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.856153 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.856153 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/tests/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/tests/src/GzipFileReader.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/tests/src/GzipFileWriter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/tests/src/IstreamReader.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/tests/src/OstreamWriter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/tests/src/PerByte.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/tests/src/RawBufferReader.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/tests/src/RawBufferWriter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/tests/src/RawFileReader.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/tests/src/RawFileWriter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/tests/src/ZlibBufferReader.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/tests/src/ZlibBufferWriter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/tests/src/read_lines.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.860153 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/CMakeCache.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.860153 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.860153 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/3.26.3/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/3.26.3/CMakeSystem.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/CMakeConfigureLog.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/CMakeDirectoryInformation.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/CMakeRuleHashes.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/Makefile.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/Makefile2
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/TargetDirectories.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate-complete
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.860153 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/DependInfo.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/Labels.json
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/Labels.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11549 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/build.make
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/cmake_clean.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/compiler_depend.make
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/compiler_depend.ts
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/progress.make
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/cmake.check_cache
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/progress.marks
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.844153 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.844153 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.860153 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-build
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-configure
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-done
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-download
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-gitclone-lastrun.txt
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-gitinfo.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-install
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-mkdir
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-patch
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-test
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.860153 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/tmp/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/tmp/byteme-populate-cfgcmd.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/tmp/byteme-populate-gitclone.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    11364 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/tmp/byteme-populate-gitupdate.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/tmp/byteme-populate-mkdirs.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-03 19:46:11.000000 rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/cmake_install.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/cmake_install.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.860153 rds2py-0.2.2/extern/rds2cpp/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   109743 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/docs/Doxyfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.864153 rds2py-0.2.2/extern/rds2cpp/extern/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.864153 rds2py-0.2.2/extern/rds2cpp/extern/CMakeFiles/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/extern/CMakeFiles/CMakeDirectoryInformation.cmake
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/extern/CMakeFiles/progress.marks
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/extern/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/extern/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-03 19:46:12.000000 rds2py-0.2.2/extern/rds2cpp/extern/cmake_install.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.844153 rds2py-0.2.2/extern/rds2cpp/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.868153 rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/Environment.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/ExternalPointer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    13968 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/RObject.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/RdsFile.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/SEXPType.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/SharedParseInfo.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/SharedWriteInfo.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/StringEncoding.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/Symbol.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/parse_altrep.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/parse_atomic.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/parse_attributes.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/parse_builtin.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/parse_environment.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/parse_expression.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/parse_external_pointer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/parse_language.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/parse_list.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/parse_object.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/parse_pairlist.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/parse_rds.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/parse_s4.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/parse_single_string.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/parse_symbol.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/rds2cpp.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/utils_parse.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/utils_write.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/write_atomic.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/write_attributes.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/write_builtin.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/write_expression.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/write_language.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/write_list.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/write_object.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/write_pairlist.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/write_rds.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/write_s4.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/write_single_string.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.868153 rds2py-0.2.2/extern/rds2cpp/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/tests/DESCRIPTION
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/tests/NAMESPACE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.868153 rds2py-0.2.2/extern/rds2cpp/tests/R/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/tests/R/RcppExports.R
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/tests/R/inspect.R
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/tests/R/namespace.R
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.868153 rds2py-0.2.2/extern/rds2cpp/tests/src/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/tests/src/Makevars
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/tests/src/RcppExports.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/tests/src/parse.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11562 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/tests/src/write.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.868153 rds2py-0.2.2/extern/rds2cpp/tests/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.868153 rds2py-0.2.2/extern/rds2cpp/tests/tests/testthat/
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/tests/tests/testthat/test-altrep.R
--rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/tests/tests/testthat/test-atomic.R
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/tests/tests/testthat/test-builtin.R
--rw-r--r--   0 runner    (1001) docker     (123)    17174 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/tests/tests/testthat/test-environment.R
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/tests/tests/testthat/test-expression.R
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/tests/tests/testthat/test-external-pointer.R
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/tests/tests/testthat/test-language.R
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/tests/tests/testthat/test-list.R
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/tests/tests/testthat/test-pairlist.R
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/tests/tests/testthat/test-s4.R
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/tests/tests/testthat/test-symbol.R
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-03 19:46:10.000000 rds2py-0.2.2/extern/rds2cpp/tests/tests/testthat.R
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-03 19:46:10.000000 rds2py-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-03 19:46:25.876153 rds2py-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-03 19:46:10.000000 rds2py-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.844153 rds2py-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.868153 rds2py-0.2.2/src/rds2py/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-03 19:46:10.000000 rds2py-0.2.2/src/rds2py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-05-03 19:46:10.000000 rds2py-0.2.2/src/rds2py/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.872153 rds2py-0.2.2/src/rds2py/lib/
--rw-r--r--   0 runner    (1001) docker     (123)  1001629 2023-05-03 19:46:25.000000 rds2py-0.2.2/src/rds2py/lib/parser.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-03 19:46:10.000000 rds2py-0.2.2/src/rds2py/lib/parser.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-05-03 19:46:10.000000 rds2py-0.2.2/src/rds2py/lib/parser.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     9984 2023-05-03 19:46:10.000000 rds2py-0.2.2/src/rds2py/lib/rds_parser.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-03 19:46:10.000000 rds2py-0.2.2/src/rds2py/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-03 19:46:10.000000 rds2py-0.2.2/src/rds2py/pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.868153 rds2py-0.2.2/src/rds2py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-03 19:46:25.000000 rds2py-0.2.2/src/rds2py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12683 2023-05-03 19:46:25.000000 rds2py-0.2.2/src/rds2py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 19:46:25.000000 rds2py-0.2.2/src/rds2py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 19:46:25.000000 rds2py-0.2.2/src/rds2py.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-03 19:46:25.000000 rds2py-0.2.2/src/rds2py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 19:46:25.000000 rds2py-0.2.2/src/rds2py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-03 19:46:10.000000 rds2py-0.2.2/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.872153 rds2py-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-03 19:46:10.000000 rds2py-0.2.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:46:25.876153 rds2py-0.2.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    14190 2023-05-03 19:46:10.000000 rds2py-0.2.2/tests/data/.Rhistory
--rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-05-03 19:46:10.000000 rds2py-0.2.2/tests/data/atomic_attr.rds
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-03 19:46:10.000000 rds2py-0.2.2/tests/data/atomic_chars.rds
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-03 19:46:10.000000 rds2py-0.2.2/tests/data/atomic_chars_unicode.rds
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-03 19:46:10.000000 rds2py-0.2.2/tests/data/atomic_complex.rds
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-03 19:46:10.000000 rds2py-0.2.2/tests/data/atomic_double.rds
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-03 19:46:10.000000 rds2py-0.2.2/tests/data/atomic_ints.rds
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-03 19:46:10.000000 rds2py-0.2.2/tests/data/atomic_logical.rds
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-03 19:46:10.000000 rds2py-0.2.2/tests/data/atomic_logical_wNA.rds
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-03 19:46:10.000000 rds2py-0.2.2/tests/data/atomic_raw.rds
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-03 19:46:10.000000 rds2py-0.2.2/tests/data/generate_files.R
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-03 19:46:10.000000 rds2py-0.2.2/tests/data/lists.rds
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-03 19:46:10.000000 rds2py-0.2.2/tests/data/lists_df.rds
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-03 19:46:10.000000 rds2py-0.2.2/tests/data/lists_df_rownames.rds
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-03 19:46:10.000000 rds2py-0.2.2/tests/data/lists_nested.rds
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-03 19:46:10.000000 rds2py-0.2.2/tests/data/lists_nested_deep.rds
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-03 19:46:10.000000 rds2py-0.2.2/tests/data/s4_class.rds
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-03 19:46:10.000000 rds2py-0.2.2/tests/data/s4_dense_matrix.rds
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-03 19:46:10.000000 rds2py-0.2.2/tests/data/s4_matrix.rds
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-03 19:46:10.000000 rds2py-0.2.2/tests/test_atomic-attr.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-03 19:46:10.000000 rds2py-0.2.2/tests/test_atomic-bool.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-03 19:46:10.000000 rds2py-0.2.2/tests/test_atomic-double.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-03 19:46:10.000000 rds2py-0.2.2/tests/test_atomic-int.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-03 19:46:10.000000 rds2py-0.2.2/tests/test_atomic-str.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-03 19:46:10.000000 rds2py-0.2.2/tests/test_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-03 19:46:10.000000 rds2py-0.2.2/tests/test_s4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-03 19:46:10.000000 rds2py-0.2.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.573038 rds2py-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-05 17:42:45.000000 rds2py-0.2.3/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.533038 rds2py-0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.537037 rds2py-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-06-05 17:42:45.000000 rds2py-0.2.3/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-05 17:42:45.000000 rds2py-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-05 17:42:45.000000 rds2py-0.2.3/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-05 17:42:45.000000 rds2py-0.2.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-05 17:42:45.000000 rds2py-0.2.3/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-05 17:42:45.000000 rds2py-0.2.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13464 2023-06-05 17:42:45.000000 rds2py-0.2.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-05 17:42:45.000000 rds2py-0.2.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-05 17:42:45.000000 rds2py-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-06-05 17:43:04.573038 rds2py-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-06-05 17:42:45.000000 rds2py-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.541038 rds2py-0.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-05 17:42:45.000000 rds2py-0.2.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.541038 rds2py-0.2.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-05 17:42:45.000000 rds2py-0.2.3/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-05 17:42:45.000000 rds2py-0.2.3/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-05 17:42:45.000000 rds2py-0.2.3/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-06-05 17:42:45.000000 rds2py-0.2.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-05 17:42:45.000000 rds2py-0.2.3/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-05 17:42:45.000000 rds2py-0.2.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-05 17:42:45.000000 rds2py-0.2.3/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-05 17:42:45.000000 rds2py-0.2.3/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-05 17:42:45.000000 rds2py-0.2.3/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-06-05 17:42:45.000000 rds2py-0.2.3/docs/tutorial.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.533038 rds2py-0.2.3/extern/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.541038 rds2py-0.2.3/extern/rds2cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/.git
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.533038 rds2py-0.2.3/extern/rds2cpp/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.541038 rds2py-0.2.3/extern/rds2cpp/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/.github/workflows/doxygenate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/.github/workflows/run-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    14096 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/CMakeCache.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.541038 rds2py-0.2.3/extern/rds2cpp/CMakeFiles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.541038 rds2py-0.2.3/extern/rds2cpp/CMakeFiles/3.26.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/CMakeFiles/3.26.3/CMakeCXXCompiler.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15992 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/CMakeFiles/3.26.3/CMakeDetermineCompilerABI_CXX.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/CMakeFiles/3.26.3/CMakeSystem.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.541038 rds2py-0.2.3/extern/rds2cpp/CMakeFiles/3.26.3/CompilerIdCXX/
+-rw-r--r--   0 runner    (1001) docker     (123)    26276 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/CMakeFiles/3.26.3/CompilerIdCXX/CMakeCXXCompilerId.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16096 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/CMakeFiles/3.26.3/CompilerIdCXX/a.out
+-rw-r--r--   0 runner    (1001) docker     (123)    27834 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/CMakeFiles/CMakeConfigureLog.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/CMakeFiles/CMakeDirectoryInformation.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/CMakeFiles/Makefile.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/CMakeFiles/Makefile2
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/CMakeFiles/TargetDirectories.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/CMakeFiles/cmake.check_cache
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/CMakeFiles/progress.marks
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6583 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.533038 rds2py-0.2.3/extern/rds2cpp/_deps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.541038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-build/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.541038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-build/CMakeFiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-build/CMakeFiles/CMakeDirectoryInformation.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-build/CMakeFiles/progress.marks
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-build/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-build/cmake_install.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.545038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.545038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/config
+-rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/description
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.545038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      478 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      896 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4726 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/fsmonitor-watchman.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/post-update.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1643 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      416 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-merge-commit.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1374 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-push.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4898 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1492 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2783 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/push-to-checkout.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3650 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/update.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/index
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.545038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/info/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      240 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/info/exclude
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.545038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/logs/HEAD
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.533038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/logs/refs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.545038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/logs/refs/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/logs/refs/heads/master
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.533038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/logs/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.545038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/logs/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/logs/refs/remotes/origin/HEAD
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.533038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/objects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.545038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/objects/pack/
+-r--r--r--   0 runner    (1001) docker     (123)    28232 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/objects/pack/pack-7240a34dedb6cbf1d892766b378b45d8ae1a08b4.idx
+-r--r--r--   0 runner    (1001) docker     (123)  1112566 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/objects/pack/pack-7240a34dedb6cbf1d892766b378b45d8ae1a08b4.pack
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/packed-refs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.533038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/refs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.549038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/refs/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/refs/heads/master
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.533038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.549038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/refs/remotes/origin/HEAD
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.533038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.549038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.github/workflows/doxygenate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.github/workflows/run-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.549038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   108855 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/docs/Doxyfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.533038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.553038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/GzipFileReader.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/GzipFileWriter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/IstreamReader.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/OstreamWriter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/PerByte.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/RawBufferReader.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/RawBufferWriter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/RawFileReader.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/RawFileWriter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/Reader.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/SelfClosingFILE.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/SelfClosingGzFile.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/SomeBufferReader.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/SomeFileReader.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/Writer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/ZlibBufferReader.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/ZlibBufferWriter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/magic_numbers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/temp_file_path.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.553038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.553038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/GzipFileReader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/GzipFileWriter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/IstreamReader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/OstreamWriter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/PerByte.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/RawBufferReader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/RawBufferWriter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/RawFileReader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/RawFileWriter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/ZlibBufferReader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/ZlibBufferWriter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/read_lines.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.553038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeCache.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.553038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.553038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/3.26.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/3.26.3/CMakeSystem.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/CMakeConfigureLog.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/CMakeDirectoryInformation.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/CMakeRuleHashes.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/Makefile.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/Makefile2
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/TargetDirectories.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate-complete
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.557038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/DependInfo.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/Labels.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/Labels.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11549 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/build.make
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/cmake_clean.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/compiler_depend.make
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/compiler_depend.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/progress.make
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/cmake.check_cache
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/progress.marks
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.533038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.533038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.557038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-build
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-configure
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-done
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-download
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-gitclone-lastrun.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-gitinfo.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-install
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-mkdir
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-patch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-test
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.557038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/tmp/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/tmp/byteme-populate-cfgcmd.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/tmp/byteme-populate-gitclone.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    11364 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/tmp/byteme-populate-gitupdate.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/tmp/byteme-populate-mkdirs.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/cmake_install.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/cmake_install.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.557038 rds2py-0.2.3/extern/rds2cpp/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   109743 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/docs/Doxyfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.557038 rds2py-0.2.3/extern/rds2cpp/extern/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.557038 rds2py-0.2.3/extern/rds2cpp/extern/CMakeFiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/extern/CMakeFiles/CMakeDirectoryInformation.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/extern/CMakeFiles/progress.marks
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/extern/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/extern/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/extern/cmake_install.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.533038 rds2py-0.2.3/extern/rds2cpp/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.565038 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/Environment.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/ExternalPointer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13968 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/RObject.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/RdsFile.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/SEXPType.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/SharedParseInfo.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/SharedWriteInfo.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/StringEncoding.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/Symbol.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_altrep.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_atomic.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_attributes.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_builtin.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_environment.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_expression.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_external_pointer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_language.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_list.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_object.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_pairlist.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_rds.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_s4.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_single_string.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_symbol.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/rds2cpp.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/utils_parse.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/utils_write.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_atomic.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_attributes.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_builtin.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_expression.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_language.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_list.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_object.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_pairlist.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_rds.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_s4.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_single_string.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.565038 rds2py-0.2.3/extern/rds2cpp/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/DESCRIPTION
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/NAMESPACE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.565038 rds2py-0.2.3/extern/rds2cpp/tests/R/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/R/RcppExports.R
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/R/inspect.R
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/R/namespace.R
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.565038 rds2py-0.2.3/extern/rds2cpp/tests/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/src/Makevars
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/src/RcppExports.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/src/parse.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11562 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/src/write.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.565038 rds2py-0.2.3/extern/rds2cpp/tests/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.565038 rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-altrep.R
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-atomic.R
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-builtin.R
+-rw-r--r--   0 runner    (1001) docker     (123)    17174 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-environment.R
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-expression.R
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-external-pointer.R
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-language.R
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-list.R
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-pairlist.R
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-s4.R
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-symbol.R
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat.R
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-05 17:42:45.000000 rds2py-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-05 17:43:04.573038 rds2py-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-05 17:42:45.000000 rds2py-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.537037 rds2py-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.565038 rds2py-0.2.3/src/rds2py/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-05 17:42:45.000000 rds2py-0.2.3/src/rds2py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7647 2023-06-05 17:42:45.000000 rds2py-0.2.3/src/rds2py/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.569038 rds2py-0.2.3/src/rds2py/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)  1002507 2023-06-05 17:43:03.000000 rds2py-0.2.3/src/rds2py/lib/parser.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-05 17:42:45.000000 rds2py-0.2.3/src/rds2py/lib/parser.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-06-05 17:42:45.000000 rds2py-0.2.3/src/rds2py/lib/parser.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     9984 2023-06-05 17:42:45.000000 rds2py-0.2.3/src/rds2py/lib/rds_parser.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-05 17:42:45.000000 rds2py-0.2.3/src/rds2py/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-05 17:42:45.000000 rds2py-0.2.3/src/rds2py/pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.569038 rds2py-0.2.3/src/rds2py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-06-05 17:43:04.000000 rds2py-0.2.3/src/rds2py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-06-05 17:43:04.000000 rds2py-0.2.3/src/rds2py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:43:04.000000 rds2py-0.2.3/src/rds2py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:43:03.000000 rds2py-0.2.3/src/rds2py.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-05 17:43:04.000000 rds2py-0.2.3/src/rds2py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-05 17:43:04.000000 rds2py-0.2.3/src/rds2py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-05 17:42:45.000000 rds2py-0.2.3/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.569038 rds2py-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.573038 rds2py-0.2.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    14190 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/.Rhistory
+-rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/atomic_attr.rds
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/atomic_chars.rds
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/atomic_chars_unicode.rds
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/atomic_complex.rds
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/atomic_double.rds
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/atomic_ints.rds
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/atomic_logical.rds
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/atomic_logical_wNA.rds
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/atomic_raw.rds
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/generate_files.R
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/lists.rds
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/lists_df.rds
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/lists_df_rownames.rds
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/lists_nested.rds
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/lists_nested_deep.rds
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/s4_class.rds
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/s4_dense_matrix.rds
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/s4_matrix.rds
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/s4_matrix_dgt.rds
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/test_atomic-attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/test_atomic-bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/test_atomic-double.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/test_atomic-int.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/test_atomic-str.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/test_interface_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/test_s4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-06-05 17:42:45.000000 rds2py-0.2.3/tox.ini
```

### Comparing `rds2py-0.2.2/.coveragerc` & `rds2py-0.2.3/.coveragerc`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/.github/workflows/pypi-test.yml` & `rds2py-0.2.3/.github/workflows/pypi-test.yml`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/.gitignore` & `rds2py-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/CONTRIBUTING.md` & `rds2py-0.2.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/LICENSE.txt` & `rds2py-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/PKG-INFO` & `rds2py-0.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rds2py
-Version: 0.2.2
+Version: 0.2.3
 Summary: Parse and read RDS files as Python representations
 Home-page: https://github.com/biocpy/rds2py
 Author: jkanche
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://biocpy.github.io/rds2py/
 Project-URL: Source, https://github.com/biocpy/rds2py
@@ -54,15 +54,15 @@
 # to convert an robject to a sparse matrix
 sp_mat = as_sparse(rObj)
 
 # to convert an robject to SCE
 sce = as_SCE(rObj)
 ```
 
-For more use cases converting `data.frame`, `dgCMatrix`, `dgRMatrix` to Python, checkout the [documentation](https://biocpy.github.io/rds2py/).
+For more use cases converting `data.frame`, `dgCMatrix`, `dgRMatrix`, `dgTMatrix` to Python, checkout the [documentation](https://biocpy.github.io/rds2py/).
 
 ***If you want to add more representations, feel free to send a PR on this repository!***
 
 
 ## Developer Notes
 
 This project uses Cython to provide bindings from C++ to Python. It tries to use the same memory space (except for strings) instead of making copy of the data.
```

### Comparing `rds2py-0.2.2/README.md` & `rds2py-0.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 # to convert an robject to a sparse matrix
 sp_mat = as_sparse(rObj)
 
 # to convert an robject to SCE
 sce = as_SCE(rObj)
 ```
 
-For more use cases converting `data.frame`, `dgCMatrix`, `dgRMatrix` to Python, checkout the [documentation](https://biocpy.github.io/rds2py/).
+For more use cases converting `data.frame`, `dgCMatrix`, `dgRMatrix`, `dgTMatrix` to Python, checkout the [documentation](https://biocpy.github.io/rds2py/).
 
 ***If you want to add more representations, feel free to send a PR on this repository!***
 
 
 ## Developer Notes
 
 This project uses Cython to provide bindings from C++ to Python. It tries to use the same memory space (except for strings) instead of making copy of the data.
```

### Comparing `rds2py-0.2.2/docs/Makefile` & `rds2py-0.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/docs/conf.py` & `rds2py-0.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/docs/index.md` & `rds2py-0.2.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/docs/tutorial.md` & `rds2py-0.2.3/docs/tutorial.md`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 The package provides friendly functions to convert some R representations to useful Python representations.
 
 ## Step 2: Python representations
 
 ### Matrices
 
-Use these methods if the RDS file contains either a sparse matrix (`dgCMatrix` or `dgRMatrix`) or a dense matrix.
+Use these methods if the RDS file contains either a sparse matrix (`dgCMatrix`, `dgRMatrix`, or `dgTMatrix`) or a dense matrix.
 
 
 ***Note: If an R object contains `dims` in the `attributes`, we consider this as a matrix.***
 
 ```python
 from rds2py import as_spase_matrix, as_dense_matrix
```

### Comparing `rds2py-0.2.2/extern/rds2cpp/.github/workflows/doxygenate.yaml` & `rds2py-0.2.3/extern/rds2cpp/.github/workflows/doxygenate.yaml`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/.github/workflows/run-tests.yaml` & `rds2py-0.2.3/extern/rds2cpp/.github/workflows/run-tests.yaml`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/CMakeCache.txt` & `rds2py-0.2.3/extern/rds2cpp/CMakeCache.txt`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/CMakeFiles/3.26.3/CMakeCXXCompiler.cmake` & `rds2py-0.2.3/extern/rds2cpp/CMakeFiles/3.26.3/CMakeCXXCompiler.cmake`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/CMakeFiles/3.26.3/CMakeDetermineCompilerABI_CXX.bin` & `rds2py-0.2.3/extern/rds2cpp/CMakeFiles/3.26.3/CMakeDetermineCompilerABI_CXX.bin`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/CMakeFiles/3.26.3/CompilerIdCXX/CMakeCXXCompilerId.cpp` & `rds2py-0.2.3/extern/rds2cpp/CMakeFiles/3.26.3/CompilerIdCXX/CMakeCXXCompilerId.cpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/CMakeFiles/3.26.3/CompilerIdCXX/a.out` & `rds2py-0.2.3/extern/rds2cpp/CMakeFiles/3.26.3/CompilerIdCXX/a.out`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/CMakeFiles/CMakeConfigureLog.yaml` & `rds2py-0.2.3/extern/rds2cpp/CMakeFiles/CMakeConfigureLog.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 events:
   -
     kind: "message-v1"
     backtrace:
       - "/usr/local/share/cmake-3.26/Modules/CMakeDetermineSystem.cmake:204 (message)"
       - "CMakeLists.txt:3 (project)"
     message: |
-      The system is: Linux - 5.15.0-1036-azure - x86_64
+      The system is: Linux - 5.15.0-1038-azure - x86_64
   -
     kind: "message-v1"
     backtrace:
       - "/usr/local/share/cmake-3.26/Modules/CMakeDetermineCompilerId.cmake:17 (message)"
       - "/usr/local/share/cmake-3.26/Modules/CMakeDetermineCompilerId.cmake:64 (__determine_compiler_id_test)"
       - "/usr/local/share/cmake-3.26/Modules/CMakeDetermineCXXCompiler.cmake:126 (CMAKE_DETERMINE_COMPILER_ID)"
       - "CMakeLists.txt:3 (project)"
@@ -35,41 +35,41 @@
     backtrace:
       - "/usr/local/share/cmake-3.26/Modules/CMakeDetermineCompilerABI.cmake:57 (try_compile)"
       - "/usr/local/share/cmake-3.26/Modules/CMakeTestCXXCompiler.cmake:26 (CMAKE_DETERMINE_COMPILER_ABI)"
       - "CMakeLists.txt:3 (project)"
     checks:
       - "Detecting CXX compiler ABI info"
     directories:
-      source: "/home/runner/work/rds2py/rds2py/extern/rds2cpp/CMakeFiles/CMakeScratch/TryCompile-Aj4Lo0"
-      binary: "/home/runner/work/rds2py/rds2py/extern/rds2cpp/CMakeFiles/CMakeScratch/TryCompile-Aj4Lo0"
+      source: "/home/runner/work/rds2py/rds2py/extern/rds2cpp/CMakeFiles/CMakeScratch/TryCompile-a24SWL"
+      binary: "/home/runner/work/rds2py/rds2py/extern/rds2cpp/CMakeFiles/CMakeScratch/TryCompile-a24SWL"
     cmakeVariables:
       CMAKE_CXX_FLAGS: ""
       CMAKE_CXX_FLAGS_DEBUG: "-g"
       CMAKE_EXE_LINKER_FLAGS: ""
     buildResult:
       variable: "CMAKE_CXX_ABI_COMPILED"
       cached: true
       stdout: |
-        Change Dir: /home/runner/work/rds2py/rds2py/extern/rds2cpp/CMakeFiles/CMakeScratch/TryCompile-Aj4Lo0
+        Change Dir: /home/runner/work/rds2py/rds2py/extern/rds2cpp/CMakeFiles/CMakeScratch/TryCompile-a24SWL
         
-        Run Build Command(s):/usr/local/bin/cmake -E env VERBOSE=1 /usr/bin/gmake -f Makefile cmTC_bbff4/fast && /usr/bin/gmake  -f CMakeFiles/cmTC_bbff4.dir/build.make CMakeFiles/cmTC_bbff4.dir/build
-        gmake[1]: Entering directory '/home/runner/work/rds2py/rds2py/extern/rds2cpp/CMakeFiles/CMakeScratch/TryCompile-Aj4Lo0'
-        Building CXX object CMakeFiles/cmTC_bbff4.dir/CMakeCXXCompilerABI.cpp.o
-        /usr/bin/c++   -v -o CMakeFiles/cmTC_bbff4.dir/CMakeCXXCompilerABI.cpp.o -c /usr/local/share/cmake-3.26/Modules/CMakeCXXCompilerABI.cpp
+        Run Build Command(s):/usr/local/bin/cmake -E env VERBOSE=1 /usr/bin/gmake -f Makefile cmTC_95e5c/fast && /usr/bin/gmake  -f CMakeFiles/cmTC_95e5c.dir/build.make CMakeFiles/cmTC_95e5c.dir/build
+        gmake[1]: Entering directory '/home/runner/work/rds2py/rds2py/extern/rds2cpp/CMakeFiles/CMakeScratch/TryCompile-a24SWL'
+        Building CXX object CMakeFiles/cmTC_95e5c.dir/CMakeCXXCompilerABI.cpp.o
+        /usr/bin/c++   -v -o CMakeFiles/cmTC_95e5c.dir/CMakeCXXCompilerABI.cpp.o -c /usr/local/share/cmake-3.26/Modules/CMakeCXXCompilerABI.cpp
         Using built-in specs.
         COLLECT_GCC=/usr/bin/c++
         OFFLOAD_TARGET_NAMES=nvptx-none:amdgcn-amdhsa
         OFFLOAD_TARGET_DEFAULT=1
         Target: x86_64-linux-gnu
         Configured with: ../src/configure -v --with-pkgversion='Ubuntu 11.3.0-1ubuntu1~22.04' --with-bugurl=file:///usr/share/doc/gcc-11/README.Bugs --enable-languages=c,ada,c++,go,brig,d,fortran,objc,obj-c++,m2 --prefix=/usr --with-gcc-major-version-only --program-suffix=-11 --program-prefix=x86_64-linux-gnu- --enable-shared --enable-linker-build-id --libexecdir=/usr/lib --without-included-gettext --enable-threads=posix --libdir=/usr/lib --enable-nls --enable-bootstrap --enable-clocale=gnu --enable-libstdcxx-debug --enable-libstdcxx-time=yes --with-default-libstdcxx-abi=new --enable-gnu-unique-object --disable-vtable-verify --enable-plugin --enable-default-pie --with-system-zlib --enable-libphobos-checking=release --with-target-system-zlib=auto --enable-objc-gc=auto --enable-multiarch --disable-werror --enable-cet --with-arch-32=i686 --with-abi=m64 --with-multilib-list=m32,m64,mx32 --enable-multilib --with-tune=generic --enable-offload-targets=nvptx-none=/build/gcc-11-xKiWfi/gcc-11-11.3.0/debian/tmp-nvptx/usr,amdgcn-amdhsa=/build/gcc-11-xKiWfi/gcc-11-11.3.0/debian/tmp-gcn/usr --without-cuda-driver --enable-checking=release --build=x86_64-linux-gnu --host=x86_64-linux-gnu --target=x86_64-linux-gnu --with-build-config=bootstrap-lto-lean --enable-link-serialization=2
         Thread model: posix
         Supported LTO compression algorithms: zlib zstd
         gcc version 11.3.0 (Ubuntu 11.3.0-1ubuntu1~22.04) 
-        COLLECT_GCC_OPTIONS='-v' '-o' 'CMakeFiles/cmTC_bbff4.dir/CMakeCXXCompilerABI.cpp.o' '-c' '-shared-libgcc' '-mtune=generic' '-march=x86-64' '-dumpdir' 'CMakeFiles/cmTC_bbff4.dir/'
-         /usr/lib/gcc/x86_64-linux-gnu/11/cc1plus -quiet -v -imultiarch x86_64-linux-gnu -D_GNU_SOURCE /usr/local/share/cmake-3.26/Modules/CMakeCXXCompilerABI.cpp -quiet -dumpdir CMakeFiles/cmTC_bbff4.dir/ -dumpbase CMakeCXXCompilerABI.cpp.cpp -dumpbase-ext .cpp -mtune=generic -march=x86-64 -version -fasynchronous-unwind-tables -fstack-protector-strong -Wformat -Wformat-security -fstack-clash-protection -fcf-protection -o /tmp/cc94vv4s.s
+        COLLECT_GCC_OPTIONS='-v' '-o' 'CMakeFiles/cmTC_95e5c.dir/CMakeCXXCompilerABI.cpp.o' '-c' '-shared-libgcc' '-mtune=generic' '-march=x86-64' '-dumpdir' 'CMakeFiles/cmTC_95e5c.dir/'
+         /usr/lib/gcc/x86_64-linux-gnu/11/cc1plus -quiet -v -imultiarch x86_64-linux-gnu -D_GNU_SOURCE /usr/local/share/cmake-3.26/Modules/CMakeCXXCompilerABI.cpp -quiet -dumpdir CMakeFiles/cmTC_95e5c.dir/ -dumpbase CMakeCXXCompilerABI.cpp.cpp -dumpbase-ext .cpp -mtune=generic -march=x86-64 -version -fasynchronous-unwind-tables -fstack-protector-strong -Wformat -Wformat-security -fstack-clash-protection -fcf-protection -o /tmp/cctDHyu2.s
         GNU C++17 (Ubuntu 11.3.0-1ubuntu1~22.04) version 11.3.0 (x86_64-linux-gnu)
         	compiled by GNU C version 11.3.0, GMP version 6.2.1, MPFR version 4.1.0, MPC version 1.2.1, isl version isl-0.24-GMP
         
         GGC heuristics: --param ggc-min-expand=100 --param ggc-min-heapsize=131072
         ignoring duplicate directory "/usr/include/x86_64-linux-gnu/c++/11"
         ignoring nonexistent directory "/usr/local/include/x86_64-linux-gnu"
         ignoring nonexistent directory "/usr/lib/gcc/x86_64-linux-gnu/11/include-fixed"
@@ -85,39 +85,39 @@
          /usr/include
         End of search list.
         GNU C++17 (Ubuntu 11.3.0-1ubuntu1~22.04) version 11.3.0 (x86_64-linux-gnu)
         	compiled by GNU C version 11.3.0, GMP version 6.2.1, MPFR version 4.1.0, MPC version 1.2.1, isl version isl-0.24-GMP
         
         GGC heuristics: --param ggc-min-expand=100 --param ggc-min-heapsize=131072
         Compiler executable checksum: 449548cbb29044828dc7ea158b577b98
-        COLLECT_GCC_OPTIONS='-v' '-o' 'CMakeFiles/cmTC_bbff4.dir/CMakeCXXCompilerABI.cpp.o' '-c' '-shared-libgcc' '-mtune=generic' '-march=x86-64' '-dumpdir' 'CMakeFiles/cmTC_bbff4.dir/'
-         as -v --64 -o CMakeFiles/cmTC_bbff4.dir/CMakeCXXCompilerABI.cpp.o /tmp/cc94vv4s.s
+        COLLECT_GCC_OPTIONS='-v' '-o' 'CMakeFiles/cmTC_95e5c.dir/CMakeCXXCompilerABI.cpp.o' '-c' '-shared-libgcc' '-mtune=generic' '-march=x86-64' '-dumpdir' 'CMakeFiles/cmTC_95e5c.dir/'
+         as -v --64 -o CMakeFiles/cmTC_95e5c.dir/CMakeCXXCompilerABI.cpp.o /tmp/cctDHyu2.s
         GNU assembler version 2.38 (x86_64-linux-gnu) using BFD version (GNU Binutils for Ubuntu) 2.38
         COMPILER_PATH=/usr/lib/gcc/x86_64-linux-gnu/11/:/usr/lib/gcc/x86_64-linux-gnu/11/:/usr/lib/gcc/x86_64-linux-gnu/:/usr/lib/gcc/x86_64-linux-gnu/11/:/usr/lib/gcc/x86_64-linux-gnu/
         LIBRARY_PATH=/usr/lib/gcc/x86_64-linux-gnu/11/:/usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/:/usr/lib/gcc/x86_64-linux-gnu/11/../../../../lib/:/lib/x86_64-linux-gnu/:/lib/../lib/:/usr/lib/x86_64-linux-gnu/:/usr/lib/../lib/:/usr/lib/gcc/x86_64-linux-gnu/11/../../../:/lib/:/usr/lib/
-        COLLECT_GCC_OPTIONS='-v' '-o' 'CMakeFiles/cmTC_bbff4.dir/CMakeCXXCompilerABI.cpp.o' '-c' '-shared-libgcc' '-mtune=generic' '-march=x86-64' '-dumpdir' 'CMakeFiles/cmTC_bbff4.dir/CMakeCXXCompilerABI.cpp.'
-        Linking CXX executable cmTC_bbff4
-        /usr/local/bin/cmake -E cmake_link_script CMakeFiles/cmTC_bbff4.dir/link.txt --verbose=1
-        /usr/bin/c++  -v CMakeFiles/cmTC_bbff4.dir/CMakeCXXCompilerABI.cpp.o -o cmTC_bbff4 
+        COLLECT_GCC_OPTIONS='-v' '-o' 'CMakeFiles/cmTC_95e5c.dir/CMakeCXXCompilerABI.cpp.o' '-c' '-shared-libgcc' '-mtune=generic' '-march=x86-64' '-dumpdir' 'CMakeFiles/cmTC_95e5c.dir/CMakeCXXCompilerABI.cpp.'
+        Linking CXX executable cmTC_95e5c
+        /usr/local/bin/cmake -E cmake_link_script CMakeFiles/cmTC_95e5c.dir/link.txt --verbose=1
+        /usr/bin/c++  -v CMakeFiles/cmTC_95e5c.dir/CMakeCXXCompilerABI.cpp.o -o cmTC_95e5c 
         Using built-in specs.
         COLLECT_GCC=/usr/bin/c++
         COLLECT_LTO_WRAPPER=/usr/lib/gcc/x86_64-linux-gnu/11/lto-wrapper
         OFFLOAD_TARGET_NAMES=nvptx-none:amdgcn-amdhsa
         OFFLOAD_TARGET_DEFAULT=1
         Target: x86_64-linux-gnu
         Configured with: ../src/configure -v --with-pkgversion='Ubuntu 11.3.0-1ubuntu1~22.04' --with-bugurl=file:///usr/share/doc/gcc-11/README.Bugs --enable-languages=c,ada,c++,go,brig,d,fortran,objc,obj-c++,m2 --prefix=/usr --with-gcc-major-version-only --program-suffix=-11 --program-prefix=x86_64-linux-gnu- --enable-shared --enable-linker-build-id --libexecdir=/usr/lib --without-included-gettext --enable-threads=posix --libdir=/usr/lib --enable-nls --enable-bootstrap --enable-clocale=gnu --enable-libstdcxx-debug --enable-libstdcxx-time=yes --with-default-libstdcxx-abi=new --enable-gnu-unique-object --disable-vtable-verify --enable-plugin --enable-default-pie --with-system-zlib --enable-libphobos-checking=release --with-target-system-zlib=auto --enable-objc-gc=auto --enable-multiarch --disable-werror --enable-cet --with-arch-32=i686 --with-abi=m64 --with-multilib-list=m32,m64,mx32 --enable-multilib --with-tune=generic --enable-offload-targets=nvptx-none=/build/gcc-11-xKiWfi/gcc-11-11.3.0/debian/tmp-nvptx/usr,amdgcn-amdhsa=/build/gcc-11-xKiWfi/gcc-11-11.3.0/debian/tmp-gcn/usr --without-cuda-driver --enable-checking=release --build=x86_64-linux-gnu --host=x86_64-linux-gnu --target=x86_64-linux-gnu --with-build-config=bootstrap-lto-lean --enable-link-serialization=2
         Thread model: posix
         Supported LTO compression algorithms: zlib zstd
         gcc version 11.3.0 (Ubuntu 11.3.0-1ubuntu1~22.04) 
         COMPILER_PATH=/usr/lib/gcc/x86_64-linux-gnu/11/:/usr/lib/gcc/x86_64-linux-gnu/11/:/usr/lib/gcc/x86_64-linux-gnu/:/usr/lib/gcc/x86_64-linux-gnu/11/:/usr/lib/gcc/x86_64-linux-gnu/
         LIBRARY_PATH=/usr/lib/gcc/x86_64-linux-gnu/11/:/usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/:/usr/lib/gcc/x86_64-linux-gnu/11/../../../../lib/:/lib/x86_64-linux-gnu/:/lib/../lib/:/usr/lib/x86_64-linux-gnu/:/usr/lib/../lib/:/usr/lib/gcc/x86_64-linux-gnu/11/../../../:/lib/:/usr/lib/
-        COLLECT_GCC_OPTIONS='-v' '-o' 'cmTC_bbff4' '-shared-libgcc' '-mtune=generic' '-march=x86-64' '-dumpdir' 'cmTC_bbff4.'
-         /usr/lib/gcc/x86_64-linux-gnu/11/collect2 -plugin /usr/lib/gcc/x86_64-linux-gnu/11/liblto_plugin.so -plugin-opt=/usr/lib/gcc/x86_64-linux-gnu/11/lto-wrapper -plugin-opt=-fresolution=/tmp/ccF9KXaf.res -plugin-opt=-pass-through=-lgcc_s -plugin-opt=-pass-through=-lgcc -plugin-opt=-pass-through=-lc -plugin-opt=-pass-through=-lgcc_s -plugin-opt=-pass-through=-lgcc --build-id --eh-frame-hdr -m elf_x86_64 --hash-style=gnu --as-needed -dynamic-linker /lib64/ld-linux-x86-64.so.2 -pie -z now -z relro -o cmTC_bbff4 /usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/Scrt1.o /usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/crti.o /usr/lib/gcc/x86_64-linux-gnu/11/crtbeginS.o -L/usr/lib/gcc/x86_64-linux-gnu/11 -L/usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu -L/usr/lib/gcc/x86_64-linux-gnu/11/../../../../lib -L/lib/x86_64-linux-gnu -L/lib/../lib -L/usr/lib/x86_64-linux-gnu -L/usr/lib/../lib -L/usr/lib/gcc/x86_64-linux-gnu/11/../../.. CMakeFiles/cmTC_bbff4.dir/CMakeCXXCompilerABI.cpp.o -lstdc++ -lm -lgcc_s -lgcc -lc -lgcc_s -lgcc /usr/lib/gcc/x86_64-linux-gnu/11/crtendS.o /usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/crtn.o
-        COLLECT_GCC_OPTIONS='-v' '-o' 'cmTC_bbff4' '-shared-libgcc' '-mtune=generic' '-march=x86-64' '-dumpdir' 'cmTC_bbff4.'
-        gmake[1]: Leaving directory '/home/runner/work/rds2py/rds2py/extern/rds2cpp/CMakeFiles/CMakeScratch/TryCompile-Aj4Lo0'
+        COLLECT_GCC_OPTIONS='-v' '-o' 'cmTC_95e5c' '-shared-libgcc' '-mtune=generic' '-march=x86-64' '-dumpdir' 'cmTC_95e5c.'
+         /usr/lib/gcc/x86_64-linux-gnu/11/collect2 -plugin /usr/lib/gcc/x86_64-linux-gnu/11/liblto_plugin.so -plugin-opt=/usr/lib/gcc/x86_64-linux-gnu/11/lto-wrapper -plugin-opt=-fresolution=/tmp/ccCHBvP6.res -plugin-opt=-pass-through=-lgcc_s -plugin-opt=-pass-through=-lgcc -plugin-opt=-pass-through=-lc -plugin-opt=-pass-through=-lgcc_s -plugin-opt=-pass-through=-lgcc --build-id --eh-frame-hdr -m elf_x86_64 --hash-style=gnu --as-needed -dynamic-linker /lib64/ld-linux-x86-64.so.2 -pie -z now -z relro -o cmTC_95e5c /usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/Scrt1.o /usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/crti.o /usr/lib/gcc/x86_64-linux-gnu/11/crtbeginS.o -L/usr/lib/gcc/x86_64-linux-gnu/11 -L/usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu -L/usr/lib/gcc/x86_64-linux-gnu/11/../../../../lib -L/lib/x86_64-linux-gnu -L/lib/../lib -L/usr/lib/x86_64-linux-gnu -L/usr/lib/../lib -L/usr/lib/gcc/x86_64-linux-gnu/11/../../.. CMakeFiles/cmTC_95e5c.dir/CMakeCXXCompilerABI.cpp.o -lstdc++ -lm -lgcc_s -lgcc -lc -lgcc_s -lgcc /usr/lib/gcc/x86_64-linux-gnu/11/crtendS.o /usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/crtn.o
+        COLLECT_GCC_OPTIONS='-v' '-o' 'cmTC_95e5c' '-shared-libgcc' '-mtune=generic' '-march=x86-64' '-dumpdir' 'cmTC_95e5c.'
+        gmake[1]: Leaving directory '/home/runner/work/rds2py/rds2py/extern/rds2cpp/CMakeFiles/CMakeScratch/TryCompile-a24SWL'
         
       exitCode: 0
   -
     kind: "message-v1"
     backtrace:
       - "/usr/local/share/cmake-3.26/Modules/CMakeDetermineCompilerABI.cmake:127 (message)"
       - "/usr/local/share/cmake-3.26/Modules/CMakeTestCXXCompiler.cmake:26 (CMAKE_DETERMINE_COMPILER_ABI)"
@@ -149,31 +149,31 @@
     backtrace:
       - "/usr/local/share/cmake-3.26/Modules/CMakeDetermineCompilerABI.cmake:152 (message)"
       - "/usr/local/share/cmake-3.26/Modules/CMakeTestCXXCompiler.cmake:26 (CMAKE_DETERMINE_COMPILER_ABI)"
       - "CMakeLists.txt:3 (project)"
     message: |
       Parsed CXX implicit link information:
         link line regex: [^( *|.*[/\\])(ld|CMAKE_LINK_STARTFILE-NOTFOUND|([^/\\]+-)?ld|collect2)[^/\\]*( |$)]
-        ignore line: [Change Dir: /home/runner/work/rds2py/rds2py/extern/rds2cpp/CMakeFiles/CMakeScratch/TryCompile-Aj4Lo0]
+        ignore line: [Change Dir: /home/runner/work/rds2py/rds2py/extern/rds2cpp/CMakeFiles/CMakeScratch/TryCompile-a24SWL]
         ignore line: []
-        ignore line: [Run Build Command(s):/usr/local/bin/cmake -E env VERBOSE=1 /usr/bin/gmake -f Makefile cmTC_bbff4/fast && /usr/bin/gmake  -f CMakeFiles/cmTC_bbff4.dir/build.make CMakeFiles/cmTC_bbff4.dir/build]
-        ignore line: [gmake[1]: Entering directory '/home/runner/work/rds2py/rds2py/extern/rds2cpp/CMakeFiles/CMakeScratch/TryCompile-Aj4Lo0']
-        ignore line: [Building CXX object CMakeFiles/cmTC_bbff4.dir/CMakeCXXCompilerABI.cpp.o]
-        ignore line: [/usr/bin/c++   -v -o CMakeFiles/cmTC_bbff4.dir/CMakeCXXCompilerABI.cpp.o -c /usr/local/share/cmake-3.26/Modules/CMakeCXXCompilerABI.cpp]
+        ignore line: [Run Build Command(s):/usr/local/bin/cmake -E env VERBOSE=1 /usr/bin/gmake -f Makefile cmTC_95e5c/fast && /usr/bin/gmake  -f CMakeFiles/cmTC_95e5c.dir/build.make CMakeFiles/cmTC_95e5c.dir/build]
+        ignore line: [gmake[1]: Entering directory '/home/runner/work/rds2py/rds2py/extern/rds2cpp/CMakeFiles/CMakeScratch/TryCompile-a24SWL']
+        ignore line: [Building CXX object CMakeFiles/cmTC_95e5c.dir/CMakeCXXCompilerABI.cpp.o]
+        ignore line: [/usr/bin/c++   -v -o CMakeFiles/cmTC_95e5c.dir/CMakeCXXCompilerABI.cpp.o -c /usr/local/share/cmake-3.26/Modules/CMakeCXXCompilerABI.cpp]
         ignore line: [Using built-in specs.]
         ignore line: [COLLECT_GCC=/usr/bin/c++]
         ignore line: [OFFLOAD_TARGET_NAMES=nvptx-none:amdgcn-amdhsa]
         ignore line: [OFFLOAD_TARGET_DEFAULT=1]
         ignore line: [Target: x86_64-linux-gnu]
         ignore line: [Configured with: ../src/configure -v --with-pkgversion='Ubuntu 11.3.0-1ubuntu1~22.04' --with-bugurl=file:///usr/share/doc/gcc-11/README.Bugs --enable-languages=c ada c++ go brig d fortran objc obj-c++ m2 --prefix=/usr --with-gcc-major-version-only --program-suffix=-11 --program-prefix=x86_64-linux-gnu- --enable-shared --enable-linker-build-id --libexecdir=/usr/lib --without-included-gettext --enable-threads=posix --libdir=/usr/lib --enable-nls --enable-bootstrap --enable-clocale=gnu --enable-libstdcxx-debug --enable-libstdcxx-time=yes --with-default-libstdcxx-abi=new --enable-gnu-unique-object --disable-vtable-verify --enable-plugin --enable-default-pie --with-system-zlib --enable-libphobos-checking=release --with-target-system-zlib=auto --enable-objc-gc=auto --enable-multiarch --disable-werror --enable-cet --with-arch-32=i686 --with-abi=m64 --with-multilib-list=m32 m64 mx32 --enable-multilib --with-tune=generic --enable-offload-targets=nvptx-none=/build/gcc-11-xKiWfi/gcc-11-11.3.0/debian/tmp-nvptx/usr amdgcn-amdhsa=/build/gcc-11-xKiWfi/gcc-11-11.3.0/debian/tmp-gcn/usr --without-cuda-driver --enable-checking=release --build=x86_64-linux-gnu --host=x86_64-linux-gnu --target=x86_64-linux-gnu --with-build-config=bootstrap-lto-lean --enable-link-serialization=2]
         ignore line: [Thread model: posix]
         ignore line: [Supported LTO compression algorithms: zlib zstd]
         ignore line: [gcc version 11.3.0 (Ubuntu 11.3.0-1ubuntu1~22.04) ]
-        ignore line: [COLLECT_GCC_OPTIONS='-v' '-o' 'CMakeFiles/cmTC_bbff4.dir/CMakeCXXCompilerABI.cpp.o' '-c' '-shared-libgcc' '-mtune=generic' '-march=x86-64' '-dumpdir' 'CMakeFiles/cmTC_bbff4.dir/']
-        ignore line: [ /usr/lib/gcc/x86_64-linux-gnu/11/cc1plus -quiet -v -imultiarch x86_64-linux-gnu -D_GNU_SOURCE /usr/local/share/cmake-3.26/Modules/CMakeCXXCompilerABI.cpp -quiet -dumpdir CMakeFiles/cmTC_bbff4.dir/ -dumpbase CMakeCXXCompilerABI.cpp.cpp -dumpbase-ext .cpp -mtune=generic -march=x86-64 -version -fasynchronous-unwind-tables -fstack-protector-strong -Wformat -Wformat-security -fstack-clash-protection -fcf-protection -o /tmp/cc94vv4s.s]
+        ignore line: [COLLECT_GCC_OPTIONS='-v' '-o' 'CMakeFiles/cmTC_95e5c.dir/CMakeCXXCompilerABI.cpp.o' '-c' '-shared-libgcc' '-mtune=generic' '-march=x86-64' '-dumpdir' 'CMakeFiles/cmTC_95e5c.dir/']
+        ignore line: [ /usr/lib/gcc/x86_64-linux-gnu/11/cc1plus -quiet -v -imultiarch x86_64-linux-gnu -D_GNU_SOURCE /usr/local/share/cmake-3.26/Modules/CMakeCXXCompilerABI.cpp -quiet -dumpdir CMakeFiles/cmTC_95e5c.dir/ -dumpbase CMakeCXXCompilerABI.cpp.cpp -dumpbase-ext .cpp -mtune=generic -march=x86-64 -version -fasynchronous-unwind-tables -fstack-protector-strong -Wformat -Wformat-security -fstack-clash-protection -fcf-protection -o /tmp/cctDHyu2.s]
         ignore line: [GNU C++17 (Ubuntu 11.3.0-1ubuntu1~22.04) version 11.3.0 (x86_64-linux-gnu)]
         ignore line: [	compiled by GNU C version 11.3.0  GMP version 6.2.1  MPFR version 4.1.0  MPC version 1.2.1  isl version isl-0.24-GMP]
         ignore line: []
         ignore line: [GGC heuristics: --param ggc-min-expand=100 --param ggc-min-heapsize=131072]
         ignore line: [ignoring duplicate directory "/usr/include/x86_64-linux-gnu/c++/11"]
         ignore line: [ignoring nonexistent directory "/usr/local/include/x86_64-linux-gnu"]
         ignore line: [ignoring nonexistent directory "/usr/lib/gcc/x86_64-linux-gnu/11/include-fixed"]
@@ -189,42 +189,42 @@
         ignore line: [ /usr/include]
         ignore line: [End of search list.]
         ignore line: [GNU C++17 (Ubuntu 11.3.0-1ubuntu1~22.04) version 11.3.0 (x86_64-linux-gnu)]
         ignore line: [	compiled by GNU C version 11.3.0  GMP version 6.2.1  MPFR version 4.1.0  MPC version 1.2.1  isl version isl-0.24-GMP]
         ignore line: []
         ignore line: [GGC heuristics: --param ggc-min-expand=100 --param ggc-min-heapsize=131072]
         ignore line: [Compiler executable checksum: 449548cbb29044828dc7ea158b577b98]
-        ignore line: [COLLECT_GCC_OPTIONS='-v' '-o' 'CMakeFiles/cmTC_bbff4.dir/CMakeCXXCompilerABI.cpp.o' '-c' '-shared-libgcc' '-mtune=generic' '-march=x86-64' '-dumpdir' 'CMakeFiles/cmTC_bbff4.dir/']
-        ignore line: [ as -v --64 -o CMakeFiles/cmTC_bbff4.dir/CMakeCXXCompilerABI.cpp.o /tmp/cc94vv4s.s]
+        ignore line: [COLLECT_GCC_OPTIONS='-v' '-o' 'CMakeFiles/cmTC_95e5c.dir/CMakeCXXCompilerABI.cpp.o' '-c' '-shared-libgcc' '-mtune=generic' '-march=x86-64' '-dumpdir' 'CMakeFiles/cmTC_95e5c.dir/']
+        ignore line: [ as -v --64 -o CMakeFiles/cmTC_95e5c.dir/CMakeCXXCompilerABI.cpp.o /tmp/cctDHyu2.s]
         ignore line: [GNU assembler version 2.38 (x86_64-linux-gnu) using BFD version (GNU Binutils for Ubuntu) 2.38]
         ignore line: [COMPILER_PATH=/usr/lib/gcc/x86_64-linux-gnu/11/:/usr/lib/gcc/x86_64-linux-gnu/11/:/usr/lib/gcc/x86_64-linux-gnu/:/usr/lib/gcc/x86_64-linux-gnu/11/:/usr/lib/gcc/x86_64-linux-gnu/]
         ignore line: [LIBRARY_PATH=/usr/lib/gcc/x86_64-linux-gnu/11/:/usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/:/usr/lib/gcc/x86_64-linux-gnu/11/../../../../lib/:/lib/x86_64-linux-gnu/:/lib/../lib/:/usr/lib/x86_64-linux-gnu/:/usr/lib/../lib/:/usr/lib/gcc/x86_64-linux-gnu/11/../../../:/lib/:/usr/lib/]
-        ignore line: [COLLECT_GCC_OPTIONS='-v' '-o' 'CMakeFiles/cmTC_bbff4.dir/CMakeCXXCompilerABI.cpp.o' '-c' '-shared-libgcc' '-mtune=generic' '-march=x86-64' '-dumpdir' 'CMakeFiles/cmTC_bbff4.dir/CMakeCXXCompilerABI.cpp.']
-        ignore line: [Linking CXX executable cmTC_bbff4]
-        ignore line: [/usr/local/bin/cmake -E cmake_link_script CMakeFiles/cmTC_bbff4.dir/link.txt --verbose=1]
-        ignore line: [/usr/bin/c++  -v CMakeFiles/cmTC_bbff4.dir/CMakeCXXCompilerABI.cpp.o -o cmTC_bbff4 ]
+        ignore line: [COLLECT_GCC_OPTIONS='-v' '-o' 'CMakeFiles/cmTC_95e5c.dir/CMakeCXXCompilerABI.cpp.o' '-c' '-shared-libgcc' '-mtune=generic' '-march=x86-64' '-dumpdir' 'CMakeFiles/cmTC_95e5c.dir/CMakeCXXCompilerABI.cpp.']
+        ignore line: [Linking CXX executable cmTC_95e5c]
+        ignore line: [/usr/local/bin/cmake -E cmake_link_script CMakeFiles/cmTC_95e5c.dir/link.txt --verbose=1]
+        ignore line: [/usr/bin/c++  -v CMakeFiles/cmTC_95e5c.dir/CMakeCXXCompilerABI.cpp.o -o cmTC_95e5c ]
         ignore line: [Using built-in specs.]
         ignore line: [COLLECT_GCC=/usr/bin/c++]
         ignore line: [COLLECT_LTO_WRAPPER=/usr/lib/gcc/x86_64-linux-gnu/11/lto-wrapper]
         ignore line: [OFFLOAD_TARGET_NAMES=nvptx-none:amdgcn-amdhsa]
         ignore line: [OFFLOAD_TARGET_DEFAULT=1]
         ignore line: [Target: x86_64-linux-gnu]
         ignore line: [Configured with: ../src/configure -v --with-pkgversion='Ubuntu 11.3.0-1ubuntu1~22.04' --with-bugurl=file:///usr/share/doc/gcc-11/README.Bugs --enable-languages=c ada c++ go brig d fortran objc obj-c++ m2 --prefix=/usr --with-gcc-major-version-only --program-suffix=-11 --program-prefix=x86_64-linux-gnu- --enable-shared --enable-linker-build-id --libexecdir=/usr/lib --without-included-gettext --enable-threads=posix --libdir=/usr/lib --enable-nls --enable-bootstrap --enable-clocale=gnu --enable-libstdcxx-debug --enable-libstdcxx-time=yes --with-default-libstdcxx-abi=new --enable-gnu-unique-object --disable-vtable-verify --enable-plugin --enable-default-pie --with-system-zlib --enable-libphobos-checking=release --with-target-system-zlib=auto --enable-objc-gc=auto --enable-multiarch --disable-werror --enable-cet --with-arch-32=i686 --with-abi=m64 --with-multilib-list=m32 m64 mx32 --enable-multilib --with-tune=generic --enable-offload-targets=nvptx-none=/build/gcc-11-xKiWfi/gcc-11-11.3.0/debian/tmp-nvptx/usr amdgcn-amdhsa=/build/gcc-11-xKiWfi/gcc-11-11.3.0/debian/tmp-gcn/usr --without-cuda-driver --enable-checking=release --build=x86_64-linux-gnu --host=x86_64-linux-gnu --target=x86_64-linux-gnu --with-build-config=bootstrap-lto-lean --enable-link-serialization=2]
         ignore line: [Thread model: posix]
         ignore line: [Supported LTO compression algorithms: zlib zstd]
         ignore line: [gcc version 11.3.0 (Ubuntu 11.3.0-1ubuntu1~22.04) ]
         ignore line: [COMPILER_PATH=/usr/lib/gcc/x86_64-linux-gnu/11/:/usr/lib/gcc/x86_64-linux-gnu/11/:/usr/lib/gcc/x86_64-linux-gnu/:/usr/lib/gcc/x86_64-linux-gnu/11/:/usr/lib/gcc/x86_64-linux-gnu/]
         ignore line: [LIBRARY_PATH=/usr/lib/gcc/x86_64-linux-gnu/11/:/usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/:/usr/lib/gcc/x86_64-linux-gnu/11/../../../../lib/:/lib/x86_64-linux-gnu/:/lib/../lib/:/usr/lib/x86_64-linux-gnu/:/usr/lib/../lib/:/usr/lib/gcc/x86_64-linux-gnu/11/../../../:/lib/:/usr/lib/]
-        ignore line: [COLLECT_GCC_OPTIONS='-v' '-o' 'cmTC_bbff4' '-shared-libgcc' '-mtune=generic' '-march=x86-64' '-dumpdir' 'cmTC_bbff4.']
-        link line: [ /usr/lib/gcc/x86_64-linux-gnu/11/collect2 -plugin /usr/lib/gcc/x86_64-linux-gnu/11/liblto_plugin.so -plugin-opt=/usr/lib/gcc/x86_64-linux-gnu/11/lto-wrapper -plugin-opt=-fresolution=/tmp/ccF9KXaf.res -plugin-opt=-pass-through=-lgcc_s -plugin-opt=-pass-through=-lgcc -plugin-opt=-pass-through=-lc -plugin-opt=-pass-through=-lgcc_s -plugin-opt=-pass-through=-lgcc --build-id --eh-frame-hdr -m elf_x86_64 --hash-style=gnu --as-needed -dynamic-linker /lib64/ld-linux-x86-64.so.2 -pie -z now -z relro -o cmTC_bbff4 /usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/Scrt1.o /usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/crti.o /usr/lib/gcc/x86_64-linux-gnu/11/crtbeginS.o -L/usr/lib/gcc/x86_64-linux-gnu/11 -L/usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu -L/usr/lib/gcc/x86_64-linux-gnu/11/../../../../lib -L/lib/x86_64-linux-gnu -L/lib/../lib -L/usr/lib/x86_64-linux-gnu -L/usr/lib/../lib -L/usr/lib/gcc/x86_64-linux-gnu/11/../../.. CMakeFiles/cmTC_bbff4.dir/CMakeCXXCompilerABI.cpp.o -lstdc++ -lm -lgcc_s -lgcc -lc -lgcc_s -lgcc /usr/lib/gcc/x86_64-linux-gnu/11/crtendS.o /usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/crtn.o]
+        ignore line: [COLLECT_GCC_OPTIONS='-v' '-o' 'cmTC_95e5c' '-shared-libgcc' '-mtune=generic' '-march=x86-64' '-dumpdir' 'cmTC_95e5c.']
+        link line: [ /usr/lib/gcc/x86_64-linux-gnu/11/collect2 -plugin /usr/lib/gcc/x86_64-linux-gnu/11/liblto_plugin.so -plugin-opt=/usr/lib/gcc/x86_64-linux-gnu/11/lto-wrapper -plugin-opt=-fresolution=/tmp/ccCHBvP6.res -plugin-opt=-pass-through=-lgcc_s -plugin-opt=-pass-through=-lgcc -plugin-opt=-pass-through=-lc -plugin-opt=-pass-through=-lgcc_s -plugin-opt=-pass-through=-lgcc --build-id --eh-frame-hdr -m elf_x86_64 --hash-style=gnu --as-needed -dynamic-linker /lib64/ld-linux-x86-64.so.2 -pie -z now -z relro -o cmTC_95e5c /usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/Scrt1.o /usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/crti.o /usr/lib/gcc/x86_64-linux-gnu/11/crtbeginS.o -L/usr/lib/gcc/x86_64-linux-gnu/11 -L/usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu -L/usr/lib/gcc/x86_64-linux-gnu/11/../../../../lib -L/lib/x86_64-linux-gnu -L/lib/../lib -L/usr/lib/x86_64-linux-gnu -L/usr/lib/../lib -L/usr/lib/gcc/x86_64-linux-gnu/11/../../.. CMakeFiles/cmTC_95e5c.dir/CMakeCXXCompilerABI.cpp.o -lstdc++ -lm -lgcc_s -lgcc -lc -lgcc_s -lgcc /usr/lib/gcc/x86_64-linux-gnu/11/crtendS.o /usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/crtn.o]
           arg [/usr/lib/gcc/x86_64-linux-gnu/11/collect2] ==> ignore
           arg [-plugin] ==> ignore
           arg [/usr/lib/gcc/x86_64-linux-gnu/11/liblto_plugin.so] ==> ignore
           arg [-plugin-opt=/usr/lib/gcc/x86_64-linux-gnu/11/lto-wrapper] ==> ignore
-          arg [-plugin-opt=-fresolution=/tmp/ccF9KXaf.res] ==> ignore
+          arg [-plugin-opt=-fresolution=/tmp/ccCHBvP6.res] ==> ignore
           arg [-plugin-opt=-pass-through=-lgcc_s] ==> ignore
           arg [-plugin-opt=-pass-through=-lgcc] ==> ignore
           arg [-plugin-opt=-pass-through=-lc] ==> ignore
           arg [-plugin-opt=-pass-through=-lgcc_s] ==> ignore
           arg [-plugin-opt=-pass-through=-lgcc] ==> ignore
           arg [--build-id] ==> ignore
           arg [--eh-frame-hdr] ==> ignore
@@ -234,27 +234,27 @@
           arg [--as-needed] ==> ignore
           arg [-dynamic-linker] ==> ignore
           arg [/lib64/ld-linux-x86-64.so.2] ==> ignore
           arg [-pie] ==> ignore
           arg [-znow] ==> ignore
           arg [-zrelro] ==> ignore
           arg [-o] ==> ignore
-          arg [cmTC_bbff4] ==> ignore
+          arg [cmTC_95e5c] ==> ignore
           arg [/usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/Scrt1.o] ==> obj [/usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/Scrt1.o]
           arg [/usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/crti.o] ==> obj [/usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/crti.o]
           arg [/usr/lib/gcc/x86_64-linux-gnu/11/crtbeginS.o] ==> obj [/usr/lib/gcc/x86_64-linux-gnu/11/crtbeginS.o]
           arg [-L/usr/lib/gcc/x86_64-linux-gnu/11] ==> dir [/usr/lib/gcc/x86_64-linux-gnu/11]
           arg [-L/usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu] ==> dir [/usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu]
           arg [-L/usr/lib/gcc/x86_64-linux-gnu/11/../../../../lib] ==> dir [/usr/lib/gcc/x86_64-linux-gnu/11/../../../../lib]
           arg [-L/lib/x86_64-linux-gnu] ==> dir [/lib/x86_64-linux-gnu]
           arg [-L/lib/../lib] ==> dir [/lib/../lib]
           arg [-L/usr/lib/x86_64-linux-gnu] ==> dir [/usr/lib/x86_64-linux-gnu]
           arg [-L/usr/lib/../lib] ==> dir [/usr/lib/../lib]
           arg [-L/usr/lib/gcc/x86_64-linux-gnu/11/../../..] ==> dir [/usr/lib/gcc/x86_64-linux-gnu/11/../../..]
-          arg [CMakeFiles/cmTC_bbff4.dir/CMakeCXXCompilerABI.cpp.o] ==> ignore
+          arg [CMakeFiles/cmTC_95e5c.dir/CMakeCXXCompilerABI.cpp.o] ==> ignore
           arg [-lstdc++] ==> lib [stdc++]
           arg [-lm] ==> lib [m]
           arg [-lgcc_s] ==> lib [gcc_s]
           arg [-lgcc] ==> lib [gcc]
           arg [-lc] ==> lib [c]
           arg [-lgcc_s] ==> lib [gcc_s]
           arg [-lgcc] ==> lib [gcc]
```

### Comparing `rds2py-0.2.2/extern/rds2cpp/CMakeFiles/CMakeDirectoryInformation.cmake` & `rds2py-0.2.3/extern/rds2cpp/CMakeFiles/CMakeDirectoryInformation.cmake`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/CMakeFiles/Makefile.cmake` & `rds2py-0.2.3/extern/rds2cpp/CMakeFiles/Makefile.cmake`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/CMakeFiles/Makefile2` & `rds2py-0.2.3/extern/rds2cpp/CMakeFiles/Makefile2`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/LICENSE` & `rds2py-0.2.3/extern/rds2cpp/LICENSE`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/Makefile` & `rds2py-0.2.3/extern/rds2cpp/Makefile`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/README.md` & `rds2py-0.2.3/extern/rds2cpp/README.md`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-build/CMakeFiles/CMakeDirectoryInformation.cmake` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-build/CMakeFiles/CMakeDirectoryInformation.cmake`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-build/Makefile` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-build/Makefile`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-build/cmake_install.cmake` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-build/cmake_install.cmake`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/hooks/commit-msg.sample` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/commit-msg.sample`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/hooks/fsmonitor-watchman.sample` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/fsmonitor-watchman.sample`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-commit.sample` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-commit.sample`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-push.sample` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-push.sample`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-rebase.sample` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-rebase.sample`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-receive.sample` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-receive.sample`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/hooks/prepare-commit-msg.sample` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/prepare-commit-msg.sample`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/hooks/push-to-checkout.sample` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/push-to-checkout.sample`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/hooks/update.sample` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/update.sample`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/objects/pack/pack-7240a34dedb6cbf1d892766b378b45d8ae1a08b4.idx` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/objects/pack/pack-7240a34dedb6cbf1d892766b378b45d8ae1a08b4.idx`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.git/objects/pack/pack-7240a34dedb6cbf1d892766b378b45d8ae1a08b4.pack` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/objects/pack/pack-7240a34dedb6cbf1d892766b378b45d8ae1a08b4.pack`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.github/workflows/doxygenate.yaml` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.github/workflows/doxygenate.yaml`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/.github/workflows/run-tests.yaml` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.github/workflows/run-tests.yaml`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/LICENSE` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/LICENSE`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/README.md` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/README.md`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/docs/Doxyfile` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/byteme/GzipFileReader.hpp` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/GzipFileReader.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/byteme/GzipFileWriter.hpp` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/GzipFileWriter.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/byteme/IstreamReader.hpp` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/IstreamReader.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/byteme/OstreamWriter.hpp` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/OstreamWriter.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/byteme/PerByte.hpp` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/PerByte.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/byteme/RawBufferReader.hpp` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/RawBufferReader.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/byteme/RawBufferWriter.hpp` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/RawBufferWriter.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/byteme/RawFileReader.hpp` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/RawFileReader.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/byteme/RawFileWriter.hpp` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/RawFileWriter.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/byteme/Reader.hpp` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/Reader.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/byteme/SelfClosingFILE.hpp` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/SelfClosingFILE.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/byteme/SelfClosingGzFile.hpp` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/SelfClosingGzFile.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/byteme/SomeBufferReader.hpp` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/SomeBufferReader.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/byteme/SomeFileReader.hpp` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/SomeFileReader.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/byteme/Writer.hpp` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/Writer.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/byteme/ZlibBufferReader.hpp` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/ZlibBufferReader.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/byteme/ZlibBufferWriter.hpp` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/ZlibBufferWriter.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/byteme/magic_numbers.hpp` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/magic_numbers.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/include/byteme/temp_file_path.hpp` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/temp_file_path.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/tests/CMakeLists.txt` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/tests/src/GzipFileReader.cpp` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/GzipFileReader.cpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/tests/src/GzipFileWriter.cpp` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/GzipFileWriter.cpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/tests/src/IstreamReader.cpp` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/IstreamReader.cpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/tests/src/OstreamWriter.cpp` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/OstreamWriter.cpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/tests/src/PerByte.cpp` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/PerByte.cpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/tests/src/RawBufferReader.cpp` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/RawBufferReader.cpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/tests/src/RawBufferWriter.cpp` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/RawBufferWriter.cpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/tests/src/RawFileReader.cpp` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/RawFileReader.cpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/tests/src/RawFileWriter.cpp` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/RawFileWriter.cpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/tests/src/ZlibBufferReader.cpp` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/ZlibBufferReader.cpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/tests/src/ZlibBufferWriter.cpp` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/ZlibBufferWriter.cpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-src/tests/src/read_lines.h` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/read_lines.h`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/CMakeCache.txt` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeCache.txt`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/CMakeDirectoryInformation.cmake` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/CMakeDirectoryInformation.cmake`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/CMakeRuleHashes.txt` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/CMakeRuleHashes.txt`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/Makefile.cmake` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/Makefile.cmake`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/Makefile2` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/Makefile2`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/Labels.json` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/Labels.json`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/Labels.txt` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/Labels.txt`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/build.make` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/build.make`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/cmake_clean.cmake` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/cmake_clean.cmake`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/CMakeLists.txt` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/Makefile` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/Makefile`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-gitclone-lastrun.txt` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-gitclone-lastrun.txt`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-gitinfo.txt` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-gitinfo.txt`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/tmp/byteme-populate-gitclone.cmake` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/tmp/byteme-populate-gitclone.cmake`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/tmp/byteme-populate-gitupdate.cmake` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/tmp/byteme-populate-gitupdate.cmake`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/tmp/byteme-populate-mkdirs.cmake` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/tmp/byteme-populate-mkdirs.cmake`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/_deps/byteme-subbuild/cmake_install.cmake` & `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/cmake_install.cmake`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/cmake_install.cmake` & `rds2py-0.2.3/extern/rds2cpp/cmake_install.cmake`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/docs/Doxyfile` & `rds2py-0.2.3/extern/rds2cpp/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/extern/CMakeFiles/CMakeDirectoryInformation.cmake` & `rds2py-0.2.3/extern/rds2cpp/extern/CMakeFiles/CMakeDirectoryInformation.cmake`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/extern/Makefile` & `rds2py-0.2.3/extern/rds2cpp/extern/Makefile`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/extern/cmake_install.cmake` & `rds2py-0.2.3/extern/rds2cpp/extern/cmake_install.cmake`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/Environment.hpp` & `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/Environment.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/ExternalPointer.hpp` & `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/ExternalPointer.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/RObject.hpp` & `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/RObject.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/RdsFile.hpp` & `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/RdsFile.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/SEXPType.hpp` & `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/SEXPType.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/SharedParseInfo.hpp` & `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/SharedParseInfo.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/SharedWriteInfo.hpp` & `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/SharedWriteInfo.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/parse_altrep.hpp` & `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_altrep.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/parse_atomic.hpp` & `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_atomic.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/parse_attributes.hpp` & `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_attributes.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/parse_builtin.hpp` & `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_builtin.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/parse_environment.hpp` & `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_environment.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/parse_expression.hpp` & `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_expression.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/parse_external_pointer.hpp` & `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_external_pointer.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/parse_language.hpp` & `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_language.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/parse_list.hpp` & `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_list.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/parse_object.hpp` & `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_object.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/parse_pairlist.hpp` & `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_pairlist.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/parse_rds.hpp` & `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_rds.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/parse_s4.hpp` & `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_s4.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/parse_single_string.hpp` & `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_single_string.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/parse_symbol.hpp` & `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_symbol.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/utils_parse.hpp` & `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/utils_parse.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/utils_write.hpp` & `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/utils_write.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/write_atomic.hpp` & `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_atomic.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/write_attributes.hpp` & `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_attributes.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/write_builtin.hpp` & `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_builtin.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/write_expression.hpp` & `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_expression.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/write_language.hpp` & `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_language.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/write_list.hpp` & `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_list.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/write_object.hpp` & `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_object.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/write_pairlist.hpp` & `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_pairlist.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/write_rds.hpp` & `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_rds.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/write_s4.hpp` & `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_s4.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/include/rds2cpp/write_single_string.hpp` & `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_single_string.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/tests/src/RcppExports.cpp` & `rds2py-0.2.3/extern/rds2cpp/tests/src/RcppExports.cpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/tests/src/parse.cpp` & `rds2py-0.2.3/extern/rds2cpp/tests/src/parse.cpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/tests/src/write.cpp` & `rds2py-0.2.3/extern/rds2cpp/tests/src/write.cpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/tests/tests/testthat/test-altrep.R` & `rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-altrep.R`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/tests/tests/testthat/test-atomic.R` & `rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-atomic.R`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/tests/tests/testthat/test-builtin.R` & `rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-builtin.R`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/tests/tests/testthat/test-environment.R` & `rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-environment.R`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/tests/tests/testthat/test-expression.R` & `rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-expression.R`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/tests/tests/testthat/test-external-pointer.R` & `rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-external-pointer.R`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/tests/tests/testthat/test-language.R` & `rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-language.R`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/tests/tests/testthat/test-list.R` & `rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-list.R`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/tests/tests/testthat/test-pairlist.R` & `rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-pairlist.R`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/tests/tests/testthat/test-s4.R` & `rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-s4.R`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/extern/rds2cpp/tests/tests/testthat/test-symbol.R` & `rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-symbol.R`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/setup.cfg` & `rds2py-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/setup.py` & `rds2py-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/src/rds2py/__init__.py` & `rds2py-0.2.3/src/rds2py/__init__.py`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/src/rds2py/interface.py` & `rds2py-0.2.3/src/rds2py/interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,17 +48,17 @@
         TypeError: not a supported class
 
     Returns:
         sp.spmatrix: a sparse matrix of the R object
     """
     cls = get_class(robj)
 
-    if cls not in ["dgCMatrix", "dgRMatrix"]:
+    if cls not in ["dgCMatrix", "dgRMatrix", "dgTMatrix"]:
         raise TypeError(
-            f"obj is not a supported sparse matrix format (`dgCMatrix`, `dgRMatrix`) but is `{cls}`"
+            f"obj is not a supported sparse matrix format (`dgCMatrix`, `dgRMatrix`, `dgTMatrix`) but is `{cls}`"
         )
 
     if cls == "dgCMatrix":
         return sp.csc_matrix(
             (
                 robj["attributes"]["x"]["data"],
                 robj["attributes"]["i"]["data"],
@@ -73,14 +73,26 @@
                 robj["attributes"]["x"]["data"],
                 robj["attributes"]["i"]["data"],
                 robj["attributes"]["p"]["data"],
             ),
             shape=tuple(robj["attributes"]["Dim"]["data"].tolist()),
         )
 
+    if cls == "dgTMatrix":
+        return sp.csr_matrix(
+            (
+                robj["attributes"]["x"]["data"],
+                (
+                    robj["attributes"]["i"]["data"],
+                    robj["attributes"]["j"]["data"],
+                ),
+            ),
+            shape=tuple(robj["attributes"]["Dim"]["data"].tolist()),
+        )
+
 
 def as_dense_matrix(robj: MutableMapping, order: str = "F") -> np.ndarray:
     """Convert a realized R object to a dense matrix representation
 
     Args:
         robj (MutableMapping): object parsed from the Rds file
         order (str): Row-major (C-style) or column-major (Fortran-style) order. Defaults to "F".
@@ -133,15 +145,15 @@
     for idx in range(len(asy_names)):
         idx_asy = robj["attributes"]["assays"]["attributes"]["data"]["attributes"][
             "listData"
         ]["data"][idx]
 
         asy_cls = get_class(idx_asy)
 
-        if asy_cls in ["dgCMatrix", "dgRMatrix"]:
+        if asy_cls in ["dgCMatrix", "dgRMatrix", "dgTMatrix"]:
             robj_asys[asy_names[idx]] = as_sparse_matrix(idx_asy)
             if assay_dims is None:
                 assay_dims = robj_asys[asy_names[idx]].shape
         elif asy_cls == "densematrix":
             robj_asys[asy_names[idx]] = as_dense_matrix(idx_asy)
             if assay_dims is None:
                 assay_dims = robj_asys[asy_names[idx]].shape
```

### Comparing `rds2py-0.2.2/src/rds2py/lib/parser.cpp` & `rds2py-0.2.3/src/rds2py/lib/parser.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "src/rds2py/lib/rds_parser.cpp"
         ],
         "extra_compile_args": [
             "-std=c++17"
         ],
         "extra_link_args": [
             "-lz"
         ],
         "include_dirs": [
             "src/rds2py/lib",
             "extern/rds2cpp/include",
             "extern/rds2cpp/_deps/byteme-src/include",
-            "/tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/core/include"
         ],
         "language": "c++",
         "name": "rds2py.core",
         "sources": [
             "src/rds2py/lib/parser.pyx",
             "src/rds2py/lib/rds_parser.cpp"
         ]
@@ -39,16 +39,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -108,16 +108,20 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -1160,195 +1164,195 @@
   Py_ssize_t shape[8];
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":717
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":724
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1381,42 +1385,42 @@
 struct __pyx_obj_6rds2py_4core_PyParsedObject;
 struct __pyx_obj_6rds2py_4core_PyRObject;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":728
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":732
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2086,30 +2090,30 @@
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* SetVTable.proto */
 static int __Pyx_SetVtable(PyObject *dict, void *vtable);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
+#define __PYX_HAVE_RT_ImportType_proto_0_29_35
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+enum __Pyx_ImportType_CheckSize_0_29_35 {
+   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
 #endif
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
@@ -6174,15 +6178,15 @@
   __Pyx_AddTraceback("rds2py.core.PyRObject.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":734
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -6191,29 +6195,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -6224,15 +6228,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":737
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -6241,29 +6245,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -6274,15 +6278,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":740
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -6291,29 +6295,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -6324,15 +6328,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":743
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -6341,29 +6345,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -6374,15 +6378,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":746
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -6391,29 +6395,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -6424,212 +6428,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":749
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":928
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":932
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":940
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -6645,15 +6649,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -6661,53 +6665,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 942, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 944, __pyx_L5_except_error)
@@ -6715,30 +6719,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -6753,15 +6757,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":946
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6777,15 +6781,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -6793,53 +6797,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 948, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 950, __pyx_L5_except_error)
@@ -6847,30 +6851,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6885,15 +6889,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":952
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6909,15 +6913,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -6925,53 +6929,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 954, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 956, __pyx_L5_except_error)
@@ -6979,30 +6983,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7017,176 +7021,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":966
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":981
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":996
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -20773,15 +20777,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_6rds2py_4core_PyRObject(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_6rds2py_4core_PyRObject *p;
   PyObject *o;
@@ -20897,15 +20901,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_array __pyx_vtable_array;
 
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_array_obj *p;
@@ -21089,15 +21093,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_MemviewEnum_obj *p;
   PyObject *o;
@@ -21211,15 +21215,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_memoryview __pyx_vtable_memoryview;
 
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryview_obj *p;
@@ -21475,15 +21479,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct__memoryviewslice __pyx_vtable__memoryviewslice;
 
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryviewslice_obj *p;
@@ -21624,15 +21628,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -21888,26 +21892,26 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(2, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
-  /* "../../../../../tmp/build-env-yu6af2f7/lib/python3.10/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(2, 950, __pyx_L1_error)
@@ -22322,70 +22326,39 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 826, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 770, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 772, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 774, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 776, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 778, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 780, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 782, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 784, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 786, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 788, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -24674,18 +24647,18 @@
     return 0;
 bad:
     Py_XDECREF(ob);
     return -1;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_35
+#define __PYX_HAVE_RT_ImportType_0_29_35
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -24731,22 +24704,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -25663,15 +25636,15 @@
                         } else if (8 * sizeof(size_t) >= 4 * PyLong_SHIFT) {
                             return (size_t) (((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -25935,15 +25908,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -26131,15 +26104,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -26327,15 +26300,15 @@
                         } else if (8 * sizeof(char) >= 4 * PyLong_SHIFT) {
                             return (char) (((((((((char)digits[3]) << PyLong_SHIFT) | (char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `rds2py-0.2.2/src/rds2py/lib/parser.pxd` & `rds2py-0.2.3/src/rds2py/lib/parser.pxd`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/src/rds2py/lib/parser.pyx` & `rds2py-0.2.3/src/rds2py/lib/parser.pyx`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/src/rds2py/lib/rds_parser.cpp` & `rds2py-0.2.3/src/rds2py/lib/rds_parser.cpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/src/rds2py/parser.py` & `rds2py-0.2.3/src/rds2py/parser.py`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/src/rds2py/pdf.py` & `rds2py-0.2.3/src/rds2py/pdf.py`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/src/rds2py.egg-info/PKG-INFO` & `rds2py-0.2.3/src/rds2py.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rds2py
-Version: 0.2.2
+Version: 0.2.3
 Summary: Parse and read RDS files as Python representations
 Home-page: https://github.com/biocpy/rds2py
 Author: jkanche
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://biocpy.github.io/rds2py/
 Project-URL: Source, https://github.com/biocpy/rds2py
@@ -54,15 +54,15 @@
 # to convert an robject to a sparse matrix
 sp_mat = as_sparse(rObj)
 
 # to convert an robject to SCE
 sce = as_SCE(rObj)
 ```
 
-For more use cases converting `data.frame`, `dgCMatrix`, `dgRMatrix` to Python, checkout the [documentation](https://biocpy.github.io/rds2py/).
+For more use cases converting `data.frame`, `dgCMatrix`, `dgRMatrix`, `dgTMatrix` to Python, checkout the [documentation](https://biocpy.github.io/rds2py/).
 
 ***If you want to add more representations, feel free to send a PR on this repository!***
 
 
 ## Developer Notes
 
 This project uses Cython to provide bindings from C++ to Python. It tries to use the same memory space (except for strings) instead of making copy of the data.
```

### Comparing `rds2py-0.2.2/src/rds2py.egg-info/SOURCES.txt` & `rds2py-0.2.3/src/rds2py.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -233,14 +233,15 @@
 src/rds2py/lib/rds_parser.cpp
 tests/conftest.py
 tests/test_atomic-attr.py
 tests/test_atomic-bool.py
 tests/test_atomic-double.py
 tests/test_atomic-int.py
 tests/test_atomic-str.py
+tests/test_interface_matrix.py
 tests/test_list.py
 tests/test_s4.py
 tests/data/.Rhistory
 tests/data/atomic_attr.rds
 tests/data/atomic_chars.rds
 tests/data/atomic_chars_unicode.rds
 tests/data/atomic_complex.rds
@@ -253,8 +254,9 @@
 tests/data/lists.rds
 tests/data/lists_df.rds
 tests/data/lists_df_rownames.rds
 tests/data/lists_nested.rds
 tests/data/lists_nested_deep.rds
 tests/data/s4_class.rds
 tests/data/s4_dense_matrix.rds
-tests/data/s4_matrix.rds
+tests/data/s4_matrix.rds
+tests/data/s4_matrix_dgt.rds
```

### Comparing `rds2py-0.2.2/test.py` & `rds2py-0.2.3/test.py`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/tests/data/.Rhistory` & `rds2py-0.2.3/tests/data/.Rhistory`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/tests/data/atomic_attr.rds` & `rds2py-0.2.3/tests/data/atomic_attr.rds`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/tests/data/atomic_complex.rds` & `rds2py-0.2.3/tests/data/atomic_complex.rds`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/tests/data/atomic_double.rds` & `rds2py-0.2.3/tests/data/atomic_double.rds`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/tests/data/generate_files.R` & `rds2py-0.2.3/tests/data/generate_files.R`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/tests/data/s4_matrix.rds` & `rds2py-0.2.3/tests/data/s4_matrix.rds`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/tests/test_atomic-attr.py` & `rds2py-0.2.3/tests/test_atomic-attr.py`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/tests/test_atomic-bool.py` & `rds2py-0.2.3/tests/test_atomic-bool.py`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/tests/test_atomic-str.py` & `rds2py-0.2.3/tests/test_atomic-str.py`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.2/tests/test_list.py` & `rds2py-0.2.3/tests/test_list.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,14 +34,14 @@
     parsed_obj = PyParsedObject("tests/data/lists_df.rds")
     robject_obj = parsed_obj.get_robject()
     array = robject_obj.realize_value()
 
     assert array is not None
     assert len(array) > 0
 
-def test_read_atomic_lists_nested_deep():
+def test_read_atomic_lists_nested_deep_rownames():
     parsed_obj = PyParsedObject("tests/data/lists_df_rownames.rds")
     robject_obj = parsed_obj.get_robject()
     array = robject_obj.realize_value()
 
     assert array is not None
     assert len(array) > 0
```

### Comparing `rds2py-0.2.2/tests/test_s4.py` & `rds2py-0.2.3/tests/test_s4.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,8 +15,15 @@
     assert array is not None
 
 def test_read_s4_matrix():
     parsed_obj = PyParsedObject("tests/data/s4_matrix.rds")
     robject_obj = parsed_obj.get_robject()
     array = robject_obj.realize_value()
 
+    assert array is not None
+
+def test_read_s4_matrix_dgt():
+    parsed_obj = PyParsedObject("tests/data/s4_matrix_dgt.rds")
+    robject_obj = parsed_obj.get_robject()
+    array = robject_obj.realize_value()
+
     assert array is not None
```

### Comparing `rds2py-0.2.2/tox.ini` & `rds2py-0.2.3/tox.ini`

 * *Files identical despite different names*

