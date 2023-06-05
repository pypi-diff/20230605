# Comparing `tmp/nester-struct-0.5.1.tar.gz` & `tmp/nester-struct-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nester-struct-0.5.1.tar", last modified: Thu Jun  1 20:28:17 2023, max compression
+gzip compressed data, was "nester-struct-0.5.2.tar", last modified: Mon Jun  5 14:51:36 2023, max compression
```

## Comparing `nester-struct-0.5.1.tar` & `nester-struct-0.5.2.tar`

### file list

```diff
@@ -1,163 +1,171 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.239712 nester-struct-0.5.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.227712 nester-struct-0.5.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.227712 nester-struct-0.5.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-01 20:27:59.000000 nester-struct-0.5.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-01 20:27:59.000000 nester-struct-0.5.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-01 20:27:59.000000 nester-struct-0.5.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-01 20:27:59.000000 nester-struct-0.5.1/.github/labeler.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.227712 nester-struct-0.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-01 20:27:59.000000 nester-struct-0.5.1/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-01 20:27:59.000000 nester-struct-0.5.1/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-01 20:27:59.000000 nester-struct-0.5.1/.github/workflows/increase_version.yml
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-01 20:27:59.000000 nester-struct-0.5.1/.github/workflows/label.yml
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-01 20:27:59.000000 nester-struct-0.5.1/.github/workflows/newsfragment_checker.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-01 20:27:59.000000 nester-struct-0.5.1/.github/workflows/packaging.yml
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-01 20:27:59.000000 nester-struct-0.5.1/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-01 20:27:59.000000 nester-struct-0.5.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-01 20:27:59.000000 nester-struct-0.5.1/.github/workflows/towncrier.yml
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-01 20:27:59.000000 nester-struct-0.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-01 20:27:59.000000 nester-struct-0.5.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-01 20:27:59.000000 nester-struct-0.5.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-01 20:27:59.000000 nester-struct-0.5.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-01 20:27:59.000000 nester-struct-0.5.1/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-06-01 20:27:59.000000 nester-struct-0.5.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-06-01 20:27:59.000000 nester-struct-0.5.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-01 20:27:59.000000 nester-struct-0.5.1/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-01 20:27:59.000000 nester-struct-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-06-01 20:28:17.239712 nester-struct-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-06-01 20:27:59.000000 nester-struct-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-01 20:27:59.000000 nester-struct-0.5.1/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.227712 nester-struct-0.5.1/changelog/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:27:59.000000 nester-struct-0.5.1/changelog/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.227712 nester-struct-0.5.1/changelog.d/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-01 20:27:59.000000 nester-struct-0.5.1/changelog.d/30.added
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-01 20:27:59.000000 nester-struct-0.5.1/changelog.d/34.added
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-01 20:27:59.000000 nester-struct-0.5.1/changelog.d/changelog_template.jinja
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.227712 nester-struct-0.5.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.223713 nester-struct-0.5.1/docs/_build/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.227712 nester-struct-0.5.1/docs/_build/html/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/.buildinfo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.231712 nester-struct-0.5.1/docs/_build/html/.doctrees/
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/.doctrees/dev_docs.doctree
--rw-r--r--   0 runner    (1001) docker     (123)   116870 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/.doctrees/environment.pickle
--rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/.doctrees/index.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    10229 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/.doctrees/installation_guide.doctree
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.231712 nester-struct-0.5.1/docs/_build/html/.doctrees/source/
--rw-r--r--   0 runner    (1001) docker     (123)    28309 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/.doctrees/source/utils.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/.doctrees/supported_languages.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    23168 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/.doctrees/usage_guide.doctree
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.231712 nester-struct-0.5.1/docs/_build/html/_sources/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/_sources/dev_docs.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/_sources/installation_guide.rst.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.231712 nester-struct-0.5.1/docs/_build/html/_sources/source/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/_sources/source/utils.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/_sources/supported_languages.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/_sources/usage_guide.rst.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.231712 nester-struct-0.5.1/docs/_build/html/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/_static/basic.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.231712 nester-struct-0.5.1/docs/_build/html/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/_static/css/badge_only.css
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.235712 nester-struct-0.5.1/docs/_build/html/_static/css/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    87624 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    67312 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    86288 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    66444 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   165742 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)   444379 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)   165548 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    98024 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)    77160 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   323344 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)   193308 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   309728 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)   184912 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   328412 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)   195704 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   309192 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0 runner    (1001) docker     (123)   182708 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   135235 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/css/theme.css
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/doctools.js
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/file.png
--rw-r--r--   0 runner    (1001) docker     (123)    86196 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/index_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.239712 nester-struct-0.5.1/docs/_build/html/_static/js/
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/js/badge_only.js
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/js/html5shiv.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/js/theme.js
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/language_data.js
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (123)    18215 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/searchtools.js
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/sphinx_highlight.js
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/dev_docs.html
--rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/genindex.html
--rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/installation_guide.html
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/objects.inv
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/py-modindex.html
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/search.html
--rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/searchindex.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.239712 nester-struct-0.5.1/docs/_build/html/source/
--rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/source/utils.html
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/supported_languages.html
--rw-r--r--   0 runner    (1001) docker     (123)    11300 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/usage_guide.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.239712 nester-struct-0.5.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.239712 nester-struct-0.5.1/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)    86196 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_static/index_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/dev_docs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/installation_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.239712 nester-struct-0.5.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/source/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/supported_languages.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/usage_guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.239712 nester-struct-0.5.1/img/
--rw-r--r--   0 runner    (1001) docker     (123)    70052 2023-06-01 20:28:00.000000 nester-struct-0.5.1/img/logo_social_preview.png
--rw-r--r--   0 runner    (1001) docker     (123)    62005 2023-06-01 20:28:00.000000 nester-struct-0.5.1/img/logo_thumbnail.png
--rw-r--r--   0 runner    (1001) docker     (123)    86196 2023-06-01 20:28:00.000000 nester-struct-0.5.1/index_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-01 20:28:00.000000 nester-struct-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-01 20:28:17.243713 nester-struct-0.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.223713 nester-struct-0.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.239712 nester-struct-0.5.1/src/nester/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-01 20:28:00.000000 nester-struct-0.5.1/src/nester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-06-01 20:28:00.000000 nester-struct-0.5.1/src/nester/nester_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-06-01 20:28:00.000000 nester-struct-0.5.1/src/nester/nester_log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.223713 nester-struct-0.5.1/src/nester/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.239712 nester-struct-0.5.1/src/nester/templates/c/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-01 20:28:00.000000 nester-struct-0.5.1/src/nester/templates/c/c_layout.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.239712 nester-struct-0.5.1/src/nester/templates/cpp/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-01 20:28:00.000000 nester-struct-0.5.1/src/nester/templates/cpp/cpp_layout.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.239712 nester-struct-0.5.1/src/nester/templates/cs/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-01 20:28:00.000000 nester-struct-0.5.1/src/nester/templates/cs/cs_layout.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.239712 nester-struct-0.5.1/src/nester/templates/java/
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-01 20:28:00.000000 nester-struct-0.5.1/src/nester/templates/java/java_layout.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.239712 nester-struct-0.5.1/src/nester/templates/py/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-01 20:28:00.000000 nester-struct-0.5.1/src/nester/templates/py/py_layout.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.239712 nester-struct-0.5.1/src/nester/templates/rb/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-01 20:28:00.000000 nester-struct-0.5.1/src/nester/templates/rb/rb_layout.json
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-06-01 20:28:00.000000 nester-struct-0.5.1/src/nester/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.239712 nester-struct-0.5.1/src/nester_struct.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-06-01 20:28:17.000000 nester-struct-0.5.1/src/nester_struct.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-06-01 20:28:17.000000 nester-struct-0.5.1/src/nester_struct.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 20:28:17.000000 nester-struct-0.5.1/src/nester_struct.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-01 20:28:17.000000 nester-struct-0.5.1/src/nester_struct.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-01 20:28:17.000000 nester-struct-0.5.1/src/nester_struct.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 20:28:17.000000 nester-struct-0.5.1/src/nester_struct.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 20:28:16.000000 nester-struct-0.5.1/src/nester_struct.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.239712 nester-struct-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:00.000000 nester-struct-0.5.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.239712 nester-struct-0.5.1/tests/interation_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:00.000000 nester-struct-0.5.1/tests/interation_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-01 20:28:00.000000 nester-struct-0.5.1/tests/interation_tests/test_util_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.239712 nester-struct-0.5.1/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:00.000000 nester-struct-0.5.1/tests/unit_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-06-01 20:28:00.000000 nester-struct-0.5.1/tests/unit_tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-01 20:28:00.000000 nester-struct-0.5.1/tests/unit_tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:51:36.038596 nester-struct-0.5.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:51:36.022596 nester-struct-0.5.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:51:36.022596 nester-struct-0.5.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-05 14:51:20.000000 nester-struct-0.5.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-05 14:51:20.000000 nester-struct-0.5.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-05 14:51:20.000000 nester-struct-0.5.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-05 14:51:20.000000 nester-struct-0.5.2/.github/labeler.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:51:36.022596 nester-struct-0.5.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-05 14:51:20.000000 nester-struct-0.5.2/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-05 14:51:20.000000 nester-struct-0.5.2/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-05 14:51:20.000000 nester-struct-0.5.2/.github/workflows/increase_version.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-05 14:51:20.000000 nester-struct-0.5.2/.github/workflows/label.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-05 14:51:20.000000 nester-struct-0.5.2/.github/workflows/newsfragment_checker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-05 14:51:20.000000 nester-struct-0.5.2/.github/workflows/packaging.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-05 14:51:20.000000 nester-struct-0.5.2/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-05 14:51:20.000000 nester-struct-0.5.2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-05 14:51:20.000000 nester-struct-0.5.2/.github/workflows/towncrier.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-05 14:51:20.000000 nester-struct-0.5.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-05 14:51:20.000000 nester-struct-0.5.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-05 14:51:20.000000 nester-struct-0.5.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-05 14:51:20.000000 nester-struct-0.5.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-05 14:51:20.000000 nester-struct-0.5.2/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-06-05 14:51:20.000000 nester-struct-0.5.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7628 2023-06-05 14:51:20.000000 nester-struct-0.5.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-05 14:51:20.000000 nester-struct-0.5.2/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-05 14:51:20.000000 nester-struct-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-06-05 14:51:36.038596 nester-struct-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-06-05 14:51:20.000000 nester-struct-0.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-05 14:51:20.000000 nester-struct-0.5.2/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:51:36.022596 nester-struct-0.5.2/changelog/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:51:20.000000 nester-struct-0.5.2/changelog/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:51:36.022596 nester-struct-0.5.2/changelog.d/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-05 14:51:20.000000 nester-struct-0.5.2/changelog.d/30.added
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-05 14:51:20.000000 nester-struct-0.5.2/changelog.d/34.added
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-05 14:51:20.000000 nester-struct-0.5.2/changelog.d/changelog_template.jinja
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:51:36.022596 nester-struct-0.5.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:51:36.018596 nester-struct-0.5.2/docs/_build/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:51:36.026596 nester-struct-0.5.2/docs/_build/html/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/.buildinfo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:51:36.026596 nester-struct-0.5.2/docs/_build/html/.doctrees/
+-rw-r--r--   0 runner    (1001) docker     (123)    28333 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/.doctrees/contributing.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/.doctrees/dev_docs.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)   199576 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/.doctrees/environment.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/.doctrees/index.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    14326 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/.doctrees/installation_guide.doctree
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:51:36.026596 nester-struct-0.5.2/docs/_build/html/.doctrees/source/
+-rw-r--r--   0 runner    (1001) docker     (123)    26270 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/.doctrees/source/logging.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    28309 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/.doctrees/source/utils.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/.doctrees/supported_languages.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    23063 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/.doctrees/usage_guide.doctree
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:51:36.026596 nester-struct-0.5.2/docs/_build/html/_sources/
+-rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_sources/contributing.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_sources/dev_docs.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_sources/installation_guide.rst.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:51:36.026596 nester-struct-0.5.2/docs/_build/html/_sources/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_sources/source/logging.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_sources/source/utils.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_sources/supported_languages.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_sources/usage_guide.rst.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:51:36.026596 nester-struct-0.5.2/docs/_build/html/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_static/basic.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:51:36.030596 nester-struct-0.5.2/docs/_build/html/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_static/css/badge_only.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:51:36.034596 nester-struct-0.5.2/docs/_build/html/_static/css/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    87624 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    67312 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    86288 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    66444 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   165742 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   444379 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   165548 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    98024 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    77160 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   323344 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   193308 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   309728 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   184912 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   328412 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   195704 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   309192 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   182708 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   135235 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_static/css/theme.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_static/doctools.js
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_static/file.png
+-rw-r--r--   0 runner    (1001) docker     (123)    86196 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_static/index_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:51:36.034596 nester-struct-0.5.2/docs/_build/html/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_static/js/badge_only.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_static/js/theme.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_static/language_data.js
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_static/plus.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (123)    18215 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14748 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/contributing.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9305 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/dev_docs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8501 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/installation_guide.html
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/objects.inv
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/py-modindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/searchindex.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:51:36.034596 nester-struct-0.5.2/docs/_build/html/source/
+-rw-r--r--   0 runner    (1001) docker     (123)    14922 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/source/logging.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13585 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/source/utils.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/supported_languages.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11057 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_build/html/usage_guide.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:51:36.034596 nester-struct-0.5.2/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:51:36.034596 nester-struct-0.5.2/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)    86196 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/_static/index_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/dev_docs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/installation_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:51:36.034596 nester-struct-0.5.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/source/logging.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/source/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/supported_languages.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-05 14:51:20.000000 nester-struct-0.5.2/docs/usage_guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:51:36.034596 nester-struct-0.5.2/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    70052 2023-06-05 14:51:20.000000 nester-struct-0.5.2/img/logo_social_preview.png
+-rw-r--r--   0 runner    (1001) docker     (123)    62005 2023-06-05 14:51:20.000000 nester-struct-0.5.2/img/logo_thumbnail.png
+-rw-r--r--   0 runner    (1001) docker     (123)    86196 2023-06-05 14:51:20.000000 nester-struct-0.5.2/index_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-05 14:51:20.000000 nester-struct-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-05 14:51:36.038596 nester-struct-0.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:51:36.018596 nester-struct-0.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:51:36.034596 nester-struct-0.5.2/src/nester/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-05 14:51:20.000000 nester-struct-0.5.2/src/nester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-06-05 14:51:20.000000 nester-struct-0.5.2/src/nester/nester_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-06-05 14:51:20.000000 nester-struct-0.5.2/src/nester/nester_log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:51:36.018596 nester-struct-0.5.2/src/nester/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:51:36.038596 nester-struct-0.5.2/src/nester/templates/c/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-05 14:51:20.000000 nester-struct-0.5.2/src/nester/templates/c/c_layout.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:51:36.038596 nester-struct-0.5.2/src/nester/templates/cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-05 14:51:20.000000 nester-struct-0.5.2/src/nester/templates/cpp/cpp_layout.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:51:36.038596 nester-struct-0.5.2/src/nester/templates/cs/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-05 14:51:20.000000 nester-struct-0.5.2/src/nester/templates/cs/cs_layout.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:51:36.038596 nester-struct-0.5.2/src/nester/templates/java/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-05 14:51:20.000000 nester-struct-0.5.2/src/nester/templates/java/java_layout.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:51:36.038596 nester-struct-0.5.2/src/nester/templates/py/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-05 14:51:20.000000 nester-struct-0.5.2/src/nester/templates/py/py_layout.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:51:36.038596 nester-struct-0.5.2/src/nester/templates/rb/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-05 14:51:20.000000 nester-struct-0.5.2/src/nester/templates/rb/rb_layout.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-06-05 14:51:20.000000 nester-struct-0.5.2/src/nester/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:51:36.038596 nester-struct-0.5.2/src/nester_struct.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-06-05 14:51:35.000000 nester-struct-0.5.2/src/nester_struct.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-06-05 14:51:36.000000 nester-struct-0.5.2/src/nester_struct.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 14:51:35.000000 nester-struct-0.5.2/src/nester_struct.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-05 14:51:35.000000 nester-struct-0.5.2/src/nester_struct.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-05 14:51:35.000000 nester-struct-0.5.2/src/nester_struct.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-05 14:51:35.000000 nester-struct-0.5.2/src/nester_struct.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 14:51:35.000000 nester-struct-0.5.2/src/nester_struct.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:51:36.038596 nester-struct-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:51:20.000000 nester-struct-0.5.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:51:36.038596 nester-struct-0.5.2/tests/interation_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:51:20.000000 nester-struct-0.5.2/tests/interation_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-05 14:51:20.000000 nester-struct-0.5.2/tests/interation_tests/test_util_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:51:36.038596 nester-struct-0.5.2/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:51:20.000000 nester-struct-0.5.2/tests/unit_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-06-05 14:51:20.000000 nester-struct-0.5.2/tests/unit_tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-05 14:51:20.000000 nester-struct-0.5.2/tests/unit_tests/test_utils.py
```

### Comparing `nester-struct-0.5.1/.github/ISSUE_TEMPLATE/bug_report.md` & `nester-struct-0.5.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/.github/ISSUE_TEMPLATE/feature_request.md` & `nester-struct-0.5.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/.github/PULL_REQUEST_TEMPLATE.md` & `nester-struct-0.5.2/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/.github/workflows/codeql.yml` & `nester-struct-0.5.2/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/.github/workflows/increase_version.yml` & `nester-struct-0.5.2/.github/workflows/increase_version.yml`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/.github/workflows/label.yml` & `nester-struct-0.5.2/.github/workflows/label.yml`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/.github/workflows/newsfragment_checker.yml` & `nester-struct-0.5.2/.github/workflows/newsfragment_checker.yml`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/.github/workflows/packaging.yml` & `nester-struct-0.5.2/.github/workflows/packaging.yml`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/.github/workflows/pylint.yml` & `nester-struct-0.5.2/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/.github/workflows/towncrier.yml` & `nester-struct-0.5.2/.github/workflows/towncrier.yml`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/.pre-commit-config.yaml` & `nester-struct-0.5.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/CODE_OF_CONDUCT.md` & `nester-struct-0.5.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/CONTRIBUTING.md` & `nester-struct-0.5.2/CONTRIBUTING.md`

 * *Files 8% similar despite different names*

```diff
@@ -24,29 +24,31 @@
 git clone git@github.com:yourusername/nester.git
 ```
 
 Now you have a local copy of the Nester repository on your machine.
 
 ## Install Requirements
 
-Nester uses `setuptools` as its build tool and `pyproject.toml` and `setup.cfg` as configuration files. To install the requirements for Nester, you can use `pip` as follows:
+Nester uses `setuptools` as its build tool and `pyproject.toml` and `setup.cfg` as configuration files. **We strongly recommend you use a `virtualenv` to isolate your development environment from the rest of your system.** To install the requirements for Nester, you can use `pip` as follows:
 
 1. Change to the Nester directory:
 
 ```shell
 cd nester
 ```
 
 2. Install the dependencies listed in `setup.cfg` using `pip`:
 
 ```shell
 pip install -e .
 ```
 
-This should install all necessary requirements for nester aswell as nester itself.
+This should install all necessary requirements for nester aswell as nester itself.<br>
+Using the `-e` flag will also install Nester as `editable`. Which means that your installation of Nester within your virtual environment will update itself when you make changes to the code.<br>
+*Note*: Sometimes it is still required to uninstall your Nester installation and reinstall it. Run `pip uninstall nester-struct` to uninstall it.
 
 >Note: If you encounter any issues with dependencies or installation, please refer to the troubleshooting section or reach out for help in the issues section or via email.
 
 ## Use Pull Request and Issue Templates
 
 As a project owner, I encourage you to use the provided Pull Request and Issue templates when contributing to Nester. These templates provide guidelines and instructions for creating effective Pull Requests (PRs) and Issues. Please follow the template and provide as much information as possible to help us understand your contribution or question.
```

### Comparing `nester-struct-0.5.1/INSTALL.md` & `nester-struct-0.5.2/INSTALL.md`

 * *Files 22% similar despite different names*

```diff
@@ -10,35 +10,60 @@
 </p>
 <h2 align="center" style="text-decoration:underline">Building the nest for you</h2>
 
 <h1>Install Nester</h1>
 
 <h2> Notice</h2>
 
-:heavy_exclamation_mark: **Please note that Nester is not yet released.**
-
-While we plan on releasing the first version of Nester soon, we are still working out the last kinks in our testing and release process.
+Nester is currently released to `PyPi`, the Python Packaging Index.
 
 ---
 <h2>Index</h2>
 
 - [Install via `pip`](#install-via-pip)
 - [Install as `rpm`](#install-as-rpm)
 - [Build from source](#build-from-source)
 
 ---
 ## Install via `pip`
 
-We plan to publish Nester to [pypi](pypi.org) first. COMING SOON.
+To install Nester from `PyPi`, make sure you have `pip` aswell as at least `python 3.10.10` installed.
+
+Open a Terminal and run:
+```bash
+pip install nester-struct
+```
+
+Note: The package name `nester` was already occupied by the time we released Nester to PyPi. Although we could not find a package with that name.<br>
+We are currently investigating if we can get the name assigned to us.
 
 ---
 
 ## Install as `rpm`
 
-We plan to build a Nester `rpm` package.
+We can now offer a `.rpm` package!
+
+To do so follow these steps (on openSUSE):
+
+1. Add the repository
+```bash
+sudo zypper addrepo https://download.opensuse.org/repositories/home:kodymo/openSUSE_Tumbleweed/home:kodymo.repo
+```
+2. Refresh your repositories
+```bash
+sudo zypper ref
+```
+3. Install Nester
+```bash
+sudo zypper install python3-nester
+```
+Note: The repository contains three builds for nester for Python 3.9, 3.10 and 3.11. `zypper` will automatically decide which version to use when running the command above.
+
+You can visit the repository on the [package maintainer's OBS account](https://build.opensuse.org/package/show/home:kodymo/python-nester).
+
 
 ---
 
 ## Build from source
 
 Nester uses `setuptools` as its build tool and `pyproject.toml` and `setup.cfg` as configuration files. To install the requirements for Nester, you can use `pip` as follows:
```

### Comparing `nester-struct-0.5.1/LICENSE` & `nester-struct-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/PKG-INFO` & `nester-struct-0.5.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: nester-struct
-Version: 0.5.1
-Summary: Automated creation of project structure
-Home-page: https://github.com/ByteOtter/nester
-Author: Christopher Hock
-Author-email: christopher-hock@protonmail.com
-License: GPLv3.0
-Keywords: automation,project_structure,python
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: tests
-Provides-Extra: docs
-License-File: LICENSE
-
 <p align="center">
 <img
     style="display: block;
            margin-left: auto;
            margin-right: auto;
            width:60%"
     src="./index_logo.png"
@@ -43,15 +25,15 @@
 A small command line tool to set up the basic structure for your Python, C#, C++, Java or Ruby project.
 
 **Index**
 - [Introduction](#introduction)
 - [Our Goal](#our-goal)
 - [Installation](#installation)
   - [Get it on PyPi!](#get-it-on-pypi)
-  - [Get it as an `.rpm` package](#get-it-as-an-rpm-package)
+  - [Get it as an `.rpm` package (wip)](#get-it-as-an-rpm-package-wip)
   - [Build it from source](#build-it-from-source)
 - [Usage](#usage)
   - [CLI Mode](#cli-mode)
   - [Interactive / GUI - Mode (coming soon)](#interactive--gui---mode-coming-soon)
   - [Supported Languages](#supported-languages)
 - [Documentation](#documentation)
     - [Read the Docs (wip)](#read-the-docs-wip)
@@ -76,28 +58,44 @@
 
 Nester, by default, also logs all projects you create with it which allows you to easily view and clean up your projects and avoid creating duplicate projects. Never loose your overview over your projects again!
 
 ## Installation
 
 ### Get it on PyPi!
 
-`Nester` is finally released on [PyPi](https://pypi.org)!<br>
+`Nester` is released on [PyPi](https://pypi.org)!<br>
 To do so, make sure you have at least `Python 3.10` and `pip` installed.<br>
 To get `Nester` simply run:
 
 ```bash
 pip install nester-struct
 ```
 Your done! Have fun with `Nester`!
 
-### Get it as an `.rpm` package
+### Get it as an `.rpm` package (wip)
+
+We can now offer a `.rpm` package!
+
+To do so follow these steps (on openSUSE):
 
-We plan to release Nester to pypi first and as an `.rpm` package in the future.
+1. Add the repository
+```bash
+sudo zypper addrepo https://download.opensuse.org/repositories/home:kodymo/openSUSE_Tumbleweed/home:kodymo.repo
+```
+2. Refresh your repositories
+```bash
+sudo zypper ref
+```
+3. Install Nester
+```bash
+sudo zypper install python3-nester
+```
+Note: The repository contains three builds for nester for Python 3.9, 3.10 and 3.11. `zypper` will automatically decide which version to use when running the command above.
 
-TBA
+You can visit the repository on the [package maintainer's OBS account](https://build.opensuse.org/package/show/home:kodymo/python-nester).
 
 ### Build it from source
 
 If you want to contribute to `Nester` or just prefer building it yoursef, refer to the [Contributing Guide](docs/CONTRIBUTING.md) to find out how.
 
 
 ## Usage
@@ -113,15 +111,15 @@
 nester <OPERATION> <OPTIONAL -git FLAG> <LANGUAGE> <PROJECT_NAME>
 ```
 The following operations will be available:
 |`Operation`|Flags|Argument|Argument|Effect|
 |-|-|-|-|-|
 |`create`|`-g/--git`, `--no-log`|`Language`|`Projectname`|Creates the project structure for the selected lanugage in *the current directory*. IF `-git` is set it will also call `git init` in this directory. `--no-log` Will prevent Nester from creating a log entry for this project. You can find the log in your home directory at `~/nester.log`|
 |`validate`|n/A|`Language`|`Projectname`|Checks the current directory and its sub-directories if it corresponds to the schema provided for the language|
-|`log`|n/A|n/A|n/A|Prints out all *logged* projects that have been created previously|
+|`log`|`--clean`|n/A|n/A|Prints out all *logged* projects that have been created previously<br>If the `--clean` flag is set, orphaned log entries (projects which had their directory deleted) will be purged from the log|
 |`clean`|`-y/--yes`|`Projectname`|n/A|Deletes the content of the specified project|
 
 ### Interactive / GUI - Mode (coming soon)
 
 This is considered to be the fallback mode. If **Nester** is called without any arguments you will be asked to enter all parameters manually.
 
 The parameters themselves will stay the same though.
@@ -149,15 +147,15 @@
 
 ## Documentation
 
 Good documentation is very important to us, even with such a small project like Nester. To this end we have two methods in place to build documentation for us:
 
 #### Read the Docs (wip)
 
-On our [Read the Docs](https://nester.readthedocs.io/en/latest/index.html#) we build the general documentation for the project. You can find the installation and usage guides there, aswell as an overview over the languages we support or want to support.
+On our [Read the Docs](https://nester.readthedocs.io/en/latest/index.html#) we build the documentation for the project. You can find the installation and usage guides there, aswell as an overview over the languages we support or want to support.
 
 Also there is the automatically build documentation of functions and modules that make Nester go.
 
 #### Towncrier (wip)
 
 Towncrier is used to build changelogs for us. It is required that Pull Requests, which change Nesters behaviour, include a changelog file.
```

### Comparing `nester-struct-0.5.1/README.md` & `nester-struct-0.5.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: nester-struct
+Version: 0.5.2
+Summary: Automated creation of project structure
+Home-page: https://github.com/ByteOtter/nester
+Author: Christopher Hock
+Author-email: christopher-hock@protonmail.com
+License: GPLv3.0
+Keywords: automation,project_structure,python
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: tests
+Provides-Extra: docs
+License-File: LICENSE
+
 <p align="center">
 <img
     style="display: block;
            margin-left: auto;
            margin-right: auto;
            width:60%"
     src="./index_logo.png"
@@ -25,15 +43,15 @@
 A small command line tool to set up the basic structure for your Python, C#, C++, Java or Ruby project.
 
 **Index**
 - [Introduction](#introduction)
 - [Our Goal](#our-goal)
 - [Installation](#installation)
   - [Get it on PyPi!](#get-it-on-pypi)
-  - [Get it as an `.rpm` package](#get-it-as-an-rpm-package)
+  - [Get it as an `.rpm` package (wip)](#get-it-as-an-rpm-package-wip)
   - [Build it from source](#build-it-from-source)
 - [Usage](#usage)
   - [CLI Mode](#cli-mode)
   - [Interactive / GUI - Mode (coming soon)](#interactive--gui---mode-coming-soon)
   - [Supported Languages](#supported-languages)
 - [Documentation](#documentation)
     - [Read the Docs (wip)](#read-the-docs-wip)
@@ -58,28 +76,44 @@
 
 Nester, by default, also logs all projects you create with it which allows you to easily view and clean up your projects and avoid creating duplicate projects. Never loose your overview over your projects again!
 
 ## Installation
 
 ### Get it on PyPi!
 
-`Nester` is finally released on [PyPi](https://pypi.org)!<br>
+`Nester` is released on [PyPi](https://pypi.org)!<br>
 To do so, make sure you have at least `Python 3.10` and `pip` installed.<br>
 To get `Nester` simply run:
 
 ```bash
 pip install nester-struct
 ```
 Your done! Have fun with `Nester`!
 
-### Get it as an `.rpm` package
+### Get it as an `.rpm` package (wip)
+
+We can now offer a `.rpm` package!
+
+To do so follow these steps (on openSUSE):
 
-We plan to release Nester to pypi first and as an `.rpm` package in the future.
+1. Add the repository
+```bash
+sudo zypper addrepo https://download.opensuse.org/repositories/home:kodymo/openSUSE_Tumbleweed/home:kodymo.repo
+```
+2. Refresh your repositories
+```bash
+sudo zypper ref
+```
+3. Install Nester
+```bash
+sudo zypper install python3-nester
+```
+Note: The repository contains three builds for nester for Python 3.9, 3.10 and 3.11. `zypper` will automatically decide which version to use when running the command above.
 
-TBA
+You can visit the repository on the [package maintainer's OBS account](https://build.opensuse.org/package/show/home:kodymo/python-nester).
 
 ### Build it from source
 
 If you want to contribute to `Nester` or just prefer building it yoursef, refer to the [Contributing Guide](docs/CONTRIBUTING.md) to find out how.
 
 
 ## Usage
@@ -95,15 +129,15 @@
 nester <OPERATION> <OPTIONAL -git FLAG> <LANGUAGE> <PROJECT_NAME>
 ```
 The following operations will be available:
 |`Operation`|Flags|Argument|Argument|Effect|
 |-|-|-|-|-|
 |`create`|`-g/--git`, `--no-log`|`Language`|`Projectname`|Creates the project structure for the selected lanugage in *the current directory*. IF `-git` is set it will also call `git init` in this directory. `--no-log` Will prevent Nester from creating a log entry for this project. You can find the log in your home directory at `~/nester.log`|
 |`validate`|n/A|`Language`|`Projectname`|Checks the current directory and its sub-directories if it corresponds to the schema provided for the language|
-|`log`|n/A|n/A|n/A|Prints out all *logged* projects that have been created previously|
+|`log`|`--clean`|n/A|n/A|Prints out all *logged* projects that have been created previously<br>If the `--clean` flag is set, orphaned log entries (projects which had their directory deleted) will be purged from the log|
 |`clean`|`-y/--yes`|`Projectname`|n/A|Deletes the content of the specified project|
 
 ### Interactive / GUI - Mode (coming soon)
 
 This is considered to be the fallback mode. If **Nester** is called without any arguments you will be asked to enter all parameters manually.
 
 The parameters themselves will stay the same though.
@@ -131,15 +165,15 @@
 
 ## Documentation
 
 Good documentation is very important to us, even with such a small project like Nester. To this end we have two methods in place to build documentation for us:
 
 #### Read the Docs (wip)
 
-On our [Read the Docs](https://nester.readthedocs.io/en/latest/index.html#) we build the general documentation for the project. You can find the installation and usage guides there, aswell as an overview over the languages we support or want to support.
+On our [Read the Docs](https://nester.readthedocs.io/en/latest/index.html#) we build the documentation for the project. You can find the installation and usage guides there, aswell as an overview over the languages we support or want to support.
 
 Also there is the automatically build documentation of functions and modules that make Nester go.
 
 #### Towncrier (wip)
 
 Towncrier is used to build changelogs for us. It is required that Pull Requests, which change Nesters behaviour, include a changelog file.
```

### Comparing `nester-struct-0.5.1/docs/Makefile` & `nester-struct-0.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/docs/_build/html/.doctrees/dev_docs.doctree` & `nester-struct-0.5.2/docs/_build/html/.doctrees/dev_docs.doctree`

 * *Files 26% similar despite different names*

```diff
@@ -1,149 +1,201 @@
-00000000: 8005 9544 0900 0000 0000 008c 0f73 7068  ...D.........sph
+00000000: 8005 9576 0c00 0000 0000 008c 0f73 7068  ...v.........sph
 00000010: 696e 782e 6164 646e 6f64 6573 948c 0864  inx.addnodes...d
 00000020: 6f63 756d 656e 7494 9394 2981 947d 9428  ocument...)..}.(
 00000030: 8c09 7261 7773 6f75 7263 6594 8c00 948c  ..rawsource.....
 00000040: 0863 6869 6c64 7265 6e94 5d94 8c0e 646f  .children.]...do
 00000050: 6375 7469 6c73 2e6e 6f64 6573 948c 0773  cutils.nodes...s
 00000060: 6563 7469 6f6e 9493 9429 8194 7d94 2868  ection...)..}.(h
-00000070: 0568 0668 075d 9468 098c 0574 6974 6c65  .h.h.].h...title
-00000080: 9493 9429 8194 7d94 2868 058c 0e44 6576  ...)..}.(h...Dev
-00000090: 656c 6f70 6572 2044 6f63 7394 6807 5d94  eloper Docs.h.].
-000000a0: 6809 8c04 5465 7874 9493 948c 0e44 6576  h...Text.....Dev
-000000b0: 656c 6f70 6572 2044 6f63 7394 8594 8194  eloper Docs.....
-000000c0: 7d94 288c 0670 6172 656e 7494 6811 8c09  }.(..parent.h...
-000000d0: 5f64 6f63 756d 656e 7494 6803 8c06 736f  _document.h...so
-000000e0: 7572 6365 944e 8c04 6c69 6e65 944e 7562  urce.N..line.Nub
-000000f0: 618c 0a61 7474 7269 6275 7465 7394 7d94  a..attributes.}.
-00000100: 288c 0369 6473 945d 948c 0763 6c61 7373  (..ids.]...class
-00000110: 6573 945d 948c 056e 616d 6573 945d 948c  es.]...names.]..
-00000120: 0864 7570 6e61 6d65 7394 5d94 8c08 6261  .dupnames.]...ba
-00000130: 636b 7265 6673 945d 9475 8c07 7461 676e  ckrefs.].u..tagn
-00000140: 616d 6594 680f 681b 680c 681c 6803 681d  ame.h.h.h.h.h.h.
-00000150: 8c38 2f68 6f6d 652f 6368 7269 732f 4465  .8/home/chris/De
-00000160: 762f 5072 6976 6174 6550 726f 6a65 6374  v/PrivateProject
-00000170: 732f 6e65 7374 6572 2f64 6f63 732f 6465  s/nester/docs/de
-00000180: 765f 646f 6373 2e72 7374 9468 1e4b 0275  v_docs.rst.h.K.u
-00000190: 6261 681f 7d94 2868 215d 948c 0e64 6576  bah.}.(h!]...dev
-000001a0: 656c 6f70 6572 2d64 6f63 7394 6168 235d  eloper-docs.ah#]
-000001b0: 9468 255d 948c 0e64 6576 656c 6f70 6572  .h%]...developer
-000001c0: 2064 6f63 7394 6168 275d 9468 295d 9475   docs.ah'].h)].u
-000001d0: 682b 680a 681b 6803 681c 6803 681d 682c  h+h.h.h.h.h.h.h,
-000001e0: 681e 4b02 7562 6168 1f7d 9428 6821 5d94  h.K.ubah.}.(h!].
-000001f0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-00000200: 8c06 736f 7572 6365 9468 2c75 682b 6801  ..source.h,uh+h.
-00000210: 8c0e 6375 7272 656e 745f 736f 7572 6365  ..current_source
-00000220: 944e 8c0c 6375 7272 656e 745f 6c69 6e65  .N..current_line
-00000230: 944e 8c08 7365 7474 696e 6773 948c 1164  .N..settings...d
-00000240: 6f63 7574 696c 732e 6672 6f6e 7465 6e64  ocutils.frontend
-00000250: 948c 0656 616c 7565 7394 9394 2981 947d  ...Values...)..}
-00000260: 9428 680f 4e8c 0967 656e 6572 6174 6f72  .(h.N..generator
-00000270: 944e 8c09 6461 7465 7374 616d 7094 4e8c  .N..datestamp.N.
-00000280: 0b73 6f75 7263 655f 6c69 6e6b 944e 8c0a  .source_link.N..
-00000290: 736f 7572 6365 5f75 726c 944e 8c0d 746f  source_url.N..to
-000002a0: 635f 6261 636b 6c69 6e6b 7394 8c05 656e  c_backlinks...en
-000002b0: 7472 7994 8c12 666f 6f74 6e6f 7465 5f62  try...footnote_b
-000002c0: 6163 6b6c 696e 6b73 944b 018c 0d73 6563  acklinks.K...sec
-000002d0: 746e 756d 5f78 666f 726d 944b 018c 0e73  tnum_xform.K...s
-000002e0: 7472 6970 5f63 6f6d 6d65 6e74 7394 4e8c  trip_comments.N.
-000002f0: 1b73 7472 6970 5f65 6c65 6d65 6e74 735f  .strip_elements_
-00000300: 7769 7468 5f63 6c61 7373 6573 944e 8c0d  with_classes.N..
-00000310: 7374 7269 705f 636c 6173 7365 7394 4e8c  strip_classes.N.
-00000320: 0c72 6570 6f72 745f 6c65 7665 6c94 4b02  .report_level.K.
-00000330: 8c0a 6861 6c74 5f6c 6576 656c 944b 058c  ..halt_level.K..
-00000340: 1165 7869 745f 7374 6174 7573 5f6c 6576  .exit_status_lev
-00000350: 656c 944b 058c 0564 6562 7567 944e 8c0e  el.K...debug.N..
-00000360: 7761 726e 696e 675f 7374 7265 616d 944e  warning_stream.N
-00000370: 8c09 7472 6163 6562 6163 6b94 888c 0e69  ..traceback....i
-00000380: 6e70 7574 5f65 6e63 6f64 696e 6794 8c09  nput_encoding...
-00000390: 7574 662d 382d 7369 6794 8c1c 696e 7075  utf-8-sig...inpu
-000003a0: 745f 656e 636f 6469 6e67 5f65 7272 6f72  t_encoding_error
-000003b0: 5f68 616e 646c 6572 948c 0673 7472 6963  _handler...stric
-000003c0: 7494 8c0f 6f75 7470 7574 5f65 6e63 6f64  t...output_encod
-000003d0: 696e 6794 8c05 7574 662d 3894 8c1d 6f75  ing...utf-8...ou
-000003e0: 7470 7574 5f65 6e63 6f64 696e 675f 6572  tput_encoding_er
-000003f0: 726f 725f 6861 6e64 6c65 7294 6858 8c0e  ror_handler.hX..
-00000400: 6572 726f 725f 656e 636f 6469 6e67 948c  error_encoding..
-00000410: 0575 7466 2d38 948c 1c65 7272 6f72 5f65  .utf-8...error_e
-00000420: 6e63 6f64 696e 675f 6572 726f 725f 6861  ncoding_error_ha
-00000430: 6e64 6c65 7294 8c10 6261 636b 736c 6173  ndler...backslas
-00000440: 6872 6570 6c61 6365 948c 0d6c 616e 6775  hreplace...langu
-00000450: 6167 655f 636f 6465 948c 0265 6e94 8c13  age_code...en...
-00000460: 7265 636f 7264 5f64 6570 656e 6465 6e63  record_dependenc
-00000470: 6965 7394 4e8c 0663 6f6e 6669 6794 4e8c  ies.N..config.N.
-00000480: 0969 645f 7072 6566 6978 9468 068c 0e61  .id_prefix.h...a
-00000490: 7574 6f5f 6964 5f70 7265 6669 7894 8c02  uto_id_prefix...
-000004a0: 6964 948c 0d64 756d 705f 7365 7474 696e  id...dump_settin
-000004b0: 6773 944e 8c0e 6475 6d70 5f69 6e74 6572  gs.N..dump_inter
-000004c0: 6e61 6c73 944e 8c0f 6475 6d70 5f74 7261  nals.N..dump_tra
-000004d0: 6e73 666f 726d 7394 4e8c 0f64 756d 705f  nsforms.N..dump_
-000004e0: 7073 6575 646f 5f78 6d6c 944e 8c10 6578  pseudo_xml.N..ex
-000004f0: 706f 7365 5f69 6e74 6572 6e61 6c73 944e  pose_internals.N
-00000500: 8c0e 7374 7269 6374 5f76 6973 6974 6f72  ..strict_visitor
-00000510: 944e 8c0f 5f64 6973 6162 6c65 5f63 6f6e  .N.._disable_con
-00000520: 6669 6794 4e8c 075f 736f 7572 6365 9468  fig.N.._source.h
-00000530: 2c8c 0c5f 6465 7374 696e 6174 696f 6e94  ,.._destination.
-00000540: 4e8c 0d5f 636f 6e66 6967 5f66 696c 6573  N.._config_files
-00000550: 945d 948c 1666 696c 655f 696e 7365 7274  .]...file_insert
-00000560: 696f 6e5f 656e 6162 6c65 6494 888c 0b72  ion_enabled....r
-00000570: 6177 5f65 6e61 626c 6564 944b 018c 116c  aw_enabled.K...l
-00000580: 696e 655f 6c65 6e67 7468 5f6c 696d 6974  ine_length_limit
-00000590: 944d 1027 8c0e 7065 705f 7265 6665 7265  .M.'..pep_refere
-000005a0: 6e63 6573 944e 8c0c 7065 705f 6261 7365  nces.N..pep_base
-000005b0: 5f75 726c 948c 1868 7474 7073 3a2f 2f70  _url...https://p
-000005c0: 6570 732e 7079 7468 6f6e 2e6f 7267 2f94  eps.python.org/.
-000005d0: 8c15 7065 705f 6669 6c65 5f75 726c 5f74  ..pep_file_url_t
-000005e0: 656d 706c 6174 6594 8c08 7065 702d 2530  emplate...pep-%0
-000005f0: 3464 948c 0e72 6663 5f72 6566 6572 656e  4d...rfc_referen
-00000600: 6365 7394 4e8c 0c72 6663 5f62 6173 655f  ces.N..rfc_base_
-00000610: 7572 6c94 8c26 6874 7470 733a 2f2f 6461  url..&https://da
-00000620: 7461 7472 6163 6b65 722e 6965 7466 2e6f  tatracker.ietf.o
-00000630: 7267 2f64 6f63 2f68 746d 6c2f 948c 0974  rg/doc/html/...t
-00000640: 6162 5f77 6964 7468 944b 088c 1d74 7269  ab_width.K...tri
-00000650: 6d5f 666f 6f74 6e6f 7465 5f72 6566 6572  m_footnote_refer
-00000660: 656e 6365 5f73 7061 6365 9489 8c10 7379  ence_space....sy
-00000670: 6e74 6178 5f68 6967 686c 6967 6874 948c  ntax_highlight..
-00000680: 046c 6f6e 6794 8c0c 736d 6172 745f 7175  .long...smart_qu
-00000690: 6f74 6573 9488 8c13 736d 6172 7471 756f  otes....smartquo
-000006a0: 7465 735f 6c6f 6361 6c65 7394 5d94 8c1d  tes_locales.]...
-000006b0: 6368 6172 6163 7465 725f 6c65 7665 6c5f  character_level_
-000006c0: 696e 6c69 6e65 5f6d 6172 6b75 7094 898c  inline_markup...
-000006d0: 0e64 6f63 7469 746c 655f 7866 6f72 6d94  .doctitle_xform.
-000006e0: 898c 0d64 6f63 696e 666f 5f78 666f 726d  ...docinfo_xform
-000006f0: 944b 018c 1273 6563 7473 7562 7469 746c  .K...sectsubtitl
-00000700: 655f 7866 6f72 6d94 898c 0d69 6d61 6765  e_xform....image
-00000710: 5f6c 6f61 6469 6e67 948c 046c 696e 6b94  _loading...link.
-00000720: 8c10 656d 6265 645f 7374 796c 6573 6865  ..embed_styleshe
-00000730: 6574 9489 8c15 636c 6f61 6b5f 656d 6169  et....cloak_emai
-00000740: 6c5f 6164 6472 6573 7365 7394 888c 1173  l_addresses....s
-00000750: 6563 7469 6f6e 5f73 656c 665f 6c69 6e6b  ection_self_link
-00000760: 9489 8c03 656e 7694 4e75 628c 0872 6570  ....env.Nub..rep
-00000770: 6f72 7465 7294 4e8c 1069 6e64 6972 6563  orter.N..indirec
-00000780: 745f 7461 7267 6574 7394 5d94 8c11 7375  t_targets.]...su
-00000790: 6273 7469 7475 7469 6f6e 5f64 6566 7394  bstitution_defs.
-000007a0: 7d94 8c12 7375 6273 7469 7475 7469 6f6e  }...substitution
-000007b0: 5f6e 616d 6573 947d 948c 0872 6566 6e61  _names.}...refna
-000007c0: 6d65 7394 7d94 8c06 7265 6669 6473 947d  mes.}...refids.}
-000007d0: 948c 076e 616d 6569 6473 947d 9468 3268  ...nameids.}.h2h
-000007e0: 2f73 8c09 6e61 6d65 7479 7065 7394 7d94  /s..nametypes.}.
-000007f0: 6832 8973 6821 7d94 682f 680c 738c 0d66  h2.sh!}.h/h.s..f
-00000800: 6f6f 746e 6f74 655f 7265 6673 947d 948c  ootnote_refs.}..
-00000810: 0d63 6974 6174 696f 6e5f 7265 6673 947d  .citation_refs.}
-00000820: 948c 0d61 7574 6f66 6f6f 746e 6f74 6573  ...autofootnotes
-00000830: 945d 948c 1161 7574 6f66 6f6f 746e 6f74  .]...autofootnot
-00000840: 655f 7265 6673 945d 948c 1073 796d 626f  e_refs.]...symbo
-00000850: 6c5f 666f 6f74 6e6f 7465 7394 5d94 8c14  l_footnotes.]...
-00000860: 7379 6d62 6f6c 5f66 6f6f 746e 6f74 655f  symbol_footnote_
-00000870: 7265 6673 945d 948c 0966 6f6f 746e 6f74  refs.]...footnot
-00000880: 6573 945d 948c 0963 6974 6174 696f 6e73  es.]...citations
-00000890: 945d 948c 1261 7574 6f66 6f6f 746e 6f74  .]...autofootnot
-000008a0: 655f 7374 6172 7494 4b01 8c15 7379 6d62  e_start.K...symb
-000008b0: 6f6c 5f66 6f6f 746e 6f74 655f 7374 6172  ol_footnote_star
-000008c0: 7494 4b00 8c0a 6964 5f63 6f75 6e74 6572  t.K...id_counter
-000008d0: 948c 0b63 6f6c 6c65 6374 696f 6e73 948c  ...collections..
-000008e0: 0743 6f75 6e74 6572 9493 947d 9485 9452  .Counter...}...R
-000008f0: 948c 0e70 6172 7365 5f6d 6573 7361 6765  ...parse_message
-00000900: 7394 5d94 8c12 7472 616e 7366 6f72 6d5f  s.]...transform_
-00000910: 6d65 7373 6167 6573 945d 948c 0b74 7261  messages.]...tra
-00000920: 6e73 666f 726d 6572 944e 8c0b 696e 636c  nsformer.N..incl
-00000930: 7564 655f 6c6f 6794 5d94 8c0a 6465 636f  ude_log.]...deco
-00000940: 7261 7469 6f6e 944e 681c 6803 7562 2e    ration.Nh.h.ub.
+00000070: 0568 0668 075d 9428 6809 8c05 7469 746c  .h.h.].(h...titl
+00000080: 6594 9394 2981 947d 9428 6805 8c0e 4465  e...)..}.(h...De
+00000090: 7665 6c6f 7065 7220 446f 6373 9468 075d  veloper Docs.h.]
+000000a0: 9468 098c 0454 6578 7494 9394 8c0e 4465  .h...Text.....De
+000000b0: 7665 6c6f 7065 7220 446f 6373 9485 9481  veloper Docs....
+000000c0: 947d 9428 8c06 7061 7265 6e74 9468 118c  .}.(..parent.h..
+000000d0: 095f 646f 6375 6d65 6e74 9468 038c 0673  ._document.h...s
+000000e0: 6f75 7263 6594 4e8c 046c 696e 6594 4e75  ource.N..line.Nu
+000000f0: 6261 8c0a 6174 7472 6962 7574 6573 947d  ba..attributes.}
+00000100: 9428 8c03 6964 7394 5d94 8c07 636c 6173  .(..ids.]...clas
+00000110: 7365 7394 5d94 8c05 6e61 6d65 7394 5d94  ses.]...names.].
+00000120: 8c08 6475 706e 616d 6573 945d 948c 0862  ..dupnames.]...b
+00000130: 6163 6b72 6566 7394 5d94 758c 0774 6167  ackrefs.].u..tag
+00000140: 6e61 6d65 9468 0f68 1b68 0c68 1c68 0368  name.h.h.h.h.h.h
+00000150: 1d8c 382f 686f 6d65 2f63 6872 6973 2f44  ..8/home/chris/D
+00000160: 6576 2f50 7269 7661 7465 5072 6f6a 6563  ev/PrivateProjec
+00000170: 7473 2f6e 6573 7465 722f 646f 6373 2f64  ts/nester/docs/d
+00000180: 6576 5f64 6f63 732e 7273 7494 681e 4b02  ev_docs.rst.h.K.
+00000190: 7562 6809 8c09 7061 7261 6772 6170 6894  ubh...paragraph.
+000001a0: 9394 2981 947d 9428 6805 8c72 5468 6573  ..)..}.(h..rThes
+000001b0: 6520 646f 6373 2061 7265 2061 2063 6f6d  e docs are a com
+000001c0: 7069 6c61 7469 6f6e 206f 6620 616c 6c20  pilation of all 
+000001d0: 6f66 204e 6573 7465 7227 7320 636f 6d70  of Nester's comp
+000001e0: 6f6e 656e 7473 2061 7377 656c 6c20 6173  onents aswell as
+000001f0: 2069 6e66 6f72 6d61 7469 6f6e 2079 6f75   information you
+00000200: 206e 6565 6420 746f 2063 6f6e 7472 6962   need to contrib
+00000210: 7574 6520 746f 204e 6573 7465 722e 9468  ute to Nester..h
+00000220: 075d 9468 168c 7454 6865 7365 2064 6f63  .].h..tThese doc
+00000230: 7320 6172 6520 6120 636f 6d70 696c 6174  s are a compilat
+00000240: 696f 6e20 6f66 2061 6c6c 206f 6620 4e65  ion of all of Ne
+00000250: 7374 6572 e280 9973 2063 6f6d 706f 6e65  ster...s compone
+00000260: 6e74 7320 6173 7765 6c6c 2061 7320 696e  nts aswell as in
+00000270: 666f 726d 6174 696f 6e20 796f 7520 6e65  formation you ne
+00000280: 6564 2074 6f20 636f 6e74 7269 6275 7465  ed to contribute
+00000290: 2074 6f20 4e65 7374 6572 2e94 8594 8194   to Nester......
+000002a0: 7d94 2868 1b68 2f68 1c68 0368 1d4e 681e  }.(h.h/h.h.h.Nh.
+000002b0: 4e75 6261 681f 7d94 2868 215d 9468 235d  Nubah.}.(h!].h#]
+000002c0: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
+000002d0: 682d 681d 682c 681e 4b04 681b 680c 681c  h-h.h,h.K.h.h.h.
+000002e0: 6803 7562 6809 8c08 636f 6d70 6f75 6e64  h.ubh...compound
+000002f0: 9493 9429 8194 7d94 2868 0568 0668 075d  ...)..}.(h.h.h.]
+00000300: 9468 008c 0774 6f63 7472 6565 9493 9429  .h...toctree...)
+00000310: 8194 7d94 2868 0568 0668 075d 9468 1f7d  ..}.(h.h.h.].h.}
+00000320: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
+00000330: 5d94 6829 5d94 681b 8c08 6465 765f 646f  ].h)].h...dev_do
+00000340: 6373 948c 0765 6e74 7269 6573 945d 9428  cs...entries.].(
+00000350: 8c13 2043 6f6e 7472 6962 7574 696e 6720  .. Contributing 
+00000360: 4775 6964 6594 8c0c 636f 6e74 7269 6275  Guide...contribu
+00000370: 7469 6e67 9486 948c 1320 5468 6520 6075  ting..... The `u
+00000380: 7469 6c73 6020 6d6f 6475 6c65 948c 0c73  tils` module...s
+00000390: 6f75 7263 652f 7574 696c 7394 8694 8c18  ource/utils.....
+000003a0: 2054 6865 2060 6e65 7374 6572 5f6c 6f67   The `nester_log
+000003b0: 6020 6d6f 6475 6c65 948c 0e73 6f75 7263  ` module...sourc
+000003c0: 652f 6c6f 6767 696e 6794 8694 658c 0c69  e/logging...e..i
+000003d0: 6e63 6c75 6465 6669 6c65 7394 5d94 2868  ncludefiles.].(h
+000003e0: 5168 5468 5765 8c08 6d61 7864 6570 7468  QhThWe..maxdepth
+000003f0: 944b 028c 0763 6170 7469 6f6e 948c 0943  .K...caption...C
+00000400: 6f6e 7465 6e74 733a 948c 0467 6c6f 6294  ontents:...glob.
+00000410: 898c 0668 6964 6465 6e94 898c 0d69 6e63  ...hidden....inc
+00000420: 6c75 6465 6869 6464 656e 9489 8c08 6e75  ludehidden....nu
+00000430: 6d62 6572 6564 944b 008c 0a74 6974 6c65  mbered.K...title
+00000440: 736f 6e6c 7994 898c 0a72 6177 656e 7472  sonly....rawentr
+00000450: 6965 7394 5d94 2868 5068 5368 5665 8c0a  ies.].(hPhShVe..
+00000460: 7261 7763 6170 7469 6f6e 9468 5d75 682b  rawcaption.h]uh+
+00000470: 6842 681d 682c 681e 4b06 681b 683f 7562  hBh.h,h.K.h.h?ub
+00000480: 6168 1f7d 9428 6821 5d94 6823 5d94 8c0f  ah.}.(h!].h#]...
+00000490: 746f 6374 7265 652d 7772 6170 7065 7294  toctree-wrapper.
+000004a0: 6168 255d 9468 275d 9468 295d 9475 682b  ah%].h'].h)].uh+
+000004b0: 683d 681b 680c 681c 6803 681d 682c 681e  h=h.h.h.h.h.h,h.
+000004c0: 4e75 6265 681f 7d94 2868 215d 948c 0e64  Nubeh.}.(h!]...d
+000004d0: 6576 656c 6f70 6572 2d64 6f63 7394 6168  eveloper-docs.ah
+000004e0: 235d 9468 255d 948c 0e64 6576 656c 6f70  #].h%]...develop
+000004f0: 6572 2064 6f63 7394 6168 275d 9468 295d  er docs.ah'].h)]
+00000500: 9475 682b 680a 681b 6803 681c 6803 681d  .uh+h.h.h.h.h.h.
+00000510: 682c 681e 4b02 7562 6168 1f7d 9428 6821  h,h.K.ubah.}.(h!
+00000520: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+00000530: 5d94 8c06 736f 7572 6365 9468 2c75 682b  ]...source.h,uh+
+00000540: 6801 8c0e 6375 7272 656e 745f 736f 7572  h...current_sour
+00000550: 6365 944e 8c0c 6375 7272 656e 745f 6c69  ce.N..current_li
+00000560: 6e65 944e 8c08 7365 7474 696e 6773 948c  ne.N..settings..
+00000570: 1164 6f63 7574 696c 732e 6672 6f6e 7465  .docutils.fronte
+00000580: 6e64 948c 0656 616c 7565 7394 9394 2981  nd...Values...).
+00000590: 947d 9428 680f 4e8c 0967 656e 6572 6174  .}.(h.N..generat
+000005a0: 6f72 944e 8c09 6461 7465 7374 616d 7094  or.N..datestamp.
+000005b0: 4e8c 0b73 6f75 7263 655f 6c69 6e6b 944e  N..source_link.N
+000005c0: 8c0a 736f 7572 6365 5f75 726c 944e 8c0d  ..source_url.N..
+000005d0: 746f 635f 6261 636b 6c69 6e6b 7394 8c05  toc_backlinks...
+000005e0: 656e 7472 7994 8c12 666f 6f74 6e6f 7465  entry...footnote
+000005f0: 5f62 6163 6b6c 696e 6b73 944b 018c 0d73  _backlinks.K...s
+00000600: 6563 746e 756d 5f78 666f 726d 944b 018c  ectnum_xform.K..
+00000610: 0e73 7472 6970 5f63 6f6d 6d65 6e74 7394  .strip_comments.
+00000620: 4e8c 1b73 7472 6970 5f65 6c65 6d65 6e74  N..strip_element
+00000630: 735f 7769 7468 5f63 6c61 7373 6573 944e  s_with_classes.N
+00000640: 8c0d 7374 7269 705f 636c 6173 7365 7394  ..strip_classes.
+00000650: 4e8c 0c72 6570 6f72 745f 6c65 7665 6c94  N..report_level.
+00000660: 4b02 8c0a 6861 6c74 5f6c 6576 656c 944b  K...halt_level.K
+00000670: 058c 1165 7869 745f 7374 6174 7573 5f6c  ...exit_status_l
+00000680: 6576 656c 944b 058c 0564 6562 7567 944e  evel.K...debug.N
+00000690: 8c0e 7761 726e 696e 675f 7374 7265 616d  ..warning_stream
+000006a0: 944e 8c09 7472 6163 6562 6163 6b94 888c  .N..traceback...
+000006b0: 0e69 6e70 7574 5f65 6e63 6f64 696e 6794  .input_encoding.
+000006c0: 8c09 7574 662d 382d 7369 6794 8c1c 696e  ..utf-8-sig...in
+000006d0: 7075 745f 656e 636f 6469 6e67 5f65 7272  put_encoding_err
+000006e0: 6f72 5f68 616e 646c 6572 948c 0673 7472  or_handler...str
+000006f0: 6963 7494 8c0f 6f75 7470 7574 5f65 6e63  ict...output_enc
+00000700: 6f64 696e 6794 8c05 7574 662d 3894 8c1d  oding...utf-8...
+00000710: 6f75 7470 7574 5f65 6e63 6f64 696e 675f  output_encoding_
+00000720: 6572 726f 725f 6861 6e64 6c65 7294 6898  error_handler.h.
+00000730: 8c0e 6572 726f 725f 656e 636f 6469 6e67  ..error_encoding
+00000740: 948c 0575 7466 2d38 948c 1c65 7272 6f72  ...utf-8...error
+00000750: 5f65 6e63 6f64 696e 675f 6572 726f 725f  _encoding_error_
+00000760: 6861 6e64 6c65 7294 8c10 6261 636b 736c  handler...backsl
+00000770: 6173 6872 6570 6c61 6365 948c 0d6c 616e  ashreplace...lan
+00000780: 6775 6167 655f 636f 6465 948c 0265 6e94  guage_code...en.
+00000790: 8c13 7265 636f 7264 5f64 6570 656e 6465  ..record_depende
+000007a0: 6e63 6965 7394 4e8c 0663 6f6e 6669 6794  ncies.N..config.
+000007b0: 4e8c 0969 645f 7072 6566 6978 9468 068c  N..id_prefix.h..
+000007c0: 0e61 7574 6f5f 6964 5f70 7265 6669 7894  .auto_id_prefix.
+000007d0: 8c02 6964 948c 0d64 756d 705f 7365 7474  ..id...dump_sett
+000007e0: 696e 6773 944e 8c0e 6475 6d70 5f69 6e74  ings.N..dump_int
+000007f0: 6572 6e61 6c73 944e 8c0f 6475 6d70 5f74  ernals.N..dump_t
+00000800: 7261 6e73 666f 726d 7394 4e8c 0f64 756d  ransforms.N..dum
+00000810: 705f 7073 6575 646f 5f78 6d6c 944e 8c10  p_pseudo_xml.N..
+00000820: 6578 706f 7365 5f69 6e74 6572 6e61 6c73  expose_internals
+00000830: 944e 8c0e 7374 7269 6374 5f76 6973 6974  .N..strict_visit
+00000840: 6f72 944e 8c0f 5f64 6973 6162 6c65 5f63  or.N.._disable_c
+00000850: 6f6e 6669 6794 4e8c 075f 736f 7572 6365  onfig.N.._source
+00000860: 9468 2c8c 0c5f 6465 7374 696e 6174 696f  .h,.._destinatio
+00000870: 6e94 4e8c 0d5f 636f 6e66 6967 5f66 696c  n.N.._config_fil
+00000880: 6573 945d 948c 1666 696c 655f 696e 7365  es.]...file_inse
+00000890: 7274 696f 6e5f 656e 6162 6c65 6494 888c  rtion_enabled...
+000008a0: 0b72 6177 5f65 6e61 626c 6564 944b 018c  .raw_enabled.K..
+000008b0: 116c 696e 655f 6c65 6e67 7468 5f6c 696d  .line_length_lim
+000008c0: 6974 944d 1027 8c0e 7065 705f 7265 6665  it.M.'..pep_refe
+000008d0: 7265 6e63 6573 944e 8c0c 7065 705f 6261  rences.N..pep_ba
+000008e0: 7365 5f75 726c 948c 1868 7474 7073 3a2f  se_url...https:/
+000008f0: 2f70 6570 732e 7079 7468 6f6e 2e6f 7267  /peps.python.org
+00000900: 2f94 8c15 7065 705f 6669 6c65 5f75 726c  /...pep_file_url
+00000910: 5f74 656d 706c 6174 6594 8c08 7065 702d  _template...pep-
+00000920: 2530 3464 948c 0e72 6663 5f72 6566 6572  %04d...rfc_refer
+00000930: 656e 6365 7394 4e8c 0c72 6663 5f62 6173  ences.N..rfc_bas
+00000940: 655f 7572 6c94 8c26 6874 7470 733a 2f2f  e_url..&https://
+00000950: 6461 7461 7472 6163 6b65 722e 6965 7466  datatracker.ietf
+00000960: 2e6f 7267 2f64 6f63 2f68 746d 6c2f 948c  .org/doc/html/..
+00000970: 0974 6162 5f77 6964 7468 944b 088c 1d74  .tab_width.K...t
+00000980: 7269 6d5f 666f 6f74 6e6f 7465 5f72 6566  rim_footnote_ref
+00000990: 6572 656e 6365 5f73 7061 6365 9489 8c10  erence_space....
+000009a0: 7379 6e74 6178 5f68 6967 686c 6967 6874  syntax_highlight
+000009b0: 948c 046c 6f6e 6794 8c0c 736d 6172 745f  ...long...smart_
+000009c0: 7175 6f74 6573 9488 8c13 736d 6172 7471  quotes....smartq
+000009d0: 756f 7465 735f 6c6f 6361 6c65 7394 5d94  uotes_locales.].
+000009e0: 8c1d 6368 6172 6163 7465 725f 6c65 7665  ..character_leve
+000009f0: 6c5f 696e 6c69 6e65 5f6d 6172 6b75 7094  l_inline_markup.
+00000a00: 898c 0e64 6f63 7469 746c 655f 7866 6f72  ...doctitle_xfor
+00000a10: 6d94 898c 0d64 6f63 696e 666f 5f78 666f  m....docinfo_xfo
+00000a20: 726d 944b 018c 1273 6563 7473 7562 7469  rm.K...sectsubti
+00000a30: 746c 655f 7866 6f72 6d94 898c 0d69 6d61  tle_xform....ima
+00000a40: 6765 5f6c 6f61 6469 6e67 948c 046c 696e  ge_loading...lin
+00000a50: 6b94 8c10 656d 6265 645f 7374 796c 6573  k...embed_styles
+00000a60: 6865 6574 9489 8c15 636c 6f61 6b5f 656d  heet....cloak_em
+00000a70: 6169 6c5f 6164 6472 6573 7365 7394 888c  ail_addresses...
+00000a80: 1173 6563 7469 6f6e 5f73 656c 665f 6c69  .section_self_li
+00000a90: 6e6b 9489 8c03 656e 7694 4e75 628c 0872  nk....env.Nub..r
+00000aa0: 6570 6f72 7465 7294 4e8c 1069 6e64 6972  eporter.N..indir
+00000ab0: 6563 745f 7461 7267 6574 7394 5d94 8c11  ect_targets.]...
+00000ac0: 7375 6273 7469 7475 7469 6f6e 5f64 6566  substitution_def
+00000ad0: 7394 7d94 8c12 7375 6273 7469 7475 7469  s.}...substituti
+00000ae0: 6f6e 5f6e 616d 6573 947d 948c 0872 6566  on_names.}...ref
+00000af0: 6e61 6d65 7394 7d94 8c06 7265 6669 6473  names.}...refids
+00000b00: 947d 948c 076e 616d 6569 6473 947d 9468  .}...nameids.}.h
+00000b10: 7268 6f73 8c09 6e61 6d65 7479 7065 7394  rhos..nametypes.
+00000b20: 7d94 6872 8973 6821 7d94 686f 680c 738c  }.hr.sh!}.hoh.s.
+00000b30: 0d66 6f6f 746e 6f74 655f 7265 6673 947d  .footnote_refs.}
+00000b40: 948c 0d63 6974 6174 696f 6e5f 7265 6673  ...citation_refs
+00000b50: 947d 948c 0d61 7574 6f66 6f6f 746e 6f74  .}...autofootnot
+00000b60: 6573 945d 948c 1161 7574 6f66 6f6f 746e  es.]...autofootn
+00000b70: 6f74 655f 7265 6673 945d 948c 1073 796d  ote_refs.]...sym
+00000b80: 626f 6c5f 666f 6f74 6e6f 7465 7394 5d94  bol_footnotes.].
+00000b90: 8c14 7379 6d62 6f6c 5f66 6f6f 746e 6f74  ..symbol_footnot
+00000ba0: 655f 7265 6673 945d 948c 0966 6f6f 746e  e_refs.]...footn
+00000bb0: 6f74 6573 945d 948c 0963 6974 6174 696f  otes.]...citatio
+00000bc0: 6e73 945d 948c 1261 7574 6f66 6f6f 746e  ns.]...autofootn
+00000bd0: 6f74 655f 7374 6172 7494 4b01 8c15 7379  ote_start.K...sy
+00000be0: 6d62 6f6c 5f66 6f6f 746e 6f74 655f 7374  mbol_footnote_st
+00000bf0: 6172 7494 4b00 8c0a 6964 5f63 6f75 6e74  art.K...id_count
+00000c00: 6572 948c 0b63 6f6c 6c65 6374 696f 6e73  er...collections
+00000c10: 948c 0743 6f75 6e74 6572 9493 947d 9485  ...Counter...}..
+00000c20: 9452 948c 0e70 6172 7365 5f6d 6573 7361  .R...parse_messa
+00000c30: 6765 7394 5d94 8c12 7472 616e 7366 6f72  ges.]...transfor
+00000c40: 6d5f 6d65 7373 6167 6573 945d 948c 0b74  m_messages.]...t
+00000c50: 7261 6e73 666f 726d 6572 944e 8c0b 696e  ransformer.N..in
+00000c60: 636c 7564 655f 6c6f 6794 5d94 8c0a 6465  clude_log.]...de
+00000c70: 636f 7261 7469 6f6e 944e 681c 6803 7562  coration.Nh.h.ub
+00000c80: 2e                                       .
```

### Comparing `nester-struct-0.5.1/docs/_build/html/.doctrees/index.doctree` & `nester-struct-0.5.2/docs/_build/html/.doctrees/index.doctree`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8005 9533 1500 0000 0000 008c 0f73 7068  ...3.........sph
+00000000: 8005 9567 1500 0000 0000 008c 0f73 7068  ...g.........sph
 00000010: 696e 782e 6164 646e 6f64 6573 948c 0864  inx.addnodes...d
 00000020: 6f63 756d 656e 7494 9394 2981 947d 9428  ocument...)..}.(
 00000030: 8c09 7261 7773 6f75 7263 6594 8c00 948c  ..rawsource.....
 00000040: 0863 6869 6c64 7265 6e94 5d94 288c 0e64  .children.].(..d
 00000050: 6f63 7574 696c 732e 6e6f 6465 7394 8c07  ocutils.nodes...
 00000060: 636f 6d6d 656e 7494 9394 2981 947d 9428  comment...)..}.(
 00000070: 6805 8ccb 4e65 7374 6572 2064 6f63 756d  h...Nester docum
@@ -88,253 +88,257 @@
 00000570: 616c 6c61 7469 6f6e 5f67 7569 6465 9486  allation_guide..
 00000580: 948c 0555 7361 6765 948c 0b75 7361 6765  ...Usage...usage
 00000590: 5f67 7569 6465 9486 948c 0e44 6576 656c  _guide.....Devel
 000005a0: 6f70 6572 2044 6f63 7394 8c08 6465 765f  oper Docs...dev_
 000005b0: 646f 6373 9486 948c 1520 2020 5468 6520  docs.....   The 
 000005c0: 6075 7469 6c73 6020 6d6f 6475 6c65 948c  `utils` module..
 000005d0: 0c73 6f75 7263 652f 7574 696c 7394 8694  .source/utils...
-000005e0: 8c13 5375 7070 6f72 7465 6420 4c61 6e67  ..Supported Lang
-000005f0: 7561 6765 7394 8c13 7375 7070 6f72 7465  uages...supporte
-00000600: 645f 6c61 6e67 7561 6765 7394 8694 658c  d_languages...e.
-00000610: 0c69 6e63 6c75 6465 6669 6c65 7394 5d94  .includefiles.].
-00000620: 2868 6368 6668 6968 6c68 6f65 8c08 6d61  (hchfhihlhoe..ma
-00000630: 7864 6570 7468 944b 028c 0763 6170 7469  xdepth.K...capti
-00000640: 6f6e 948c 0943 6f6e 7465 6e74 733a 948c  on...Contents:..
-00000650: 0467 6c6f 6294 898c 0668 6964 6465 6e94  .glob....hidden.
-00000660: 898c 0d69 6e63 6c75 6465 6869 6464 656e  ...includehidden
-00000670: 9489 8c08 6e75 6d62 6572 6564 944b 008c  ....numbered.K..
-00000680: 0a74 6974 6c65 736f 6e6c 7994 898c 0a72  .titlesonly....r
-00000690: 6177 656e 7472 6965 7394 5d94 2868 6268  awentries.].(hbh
-000006a0: 6568 6868 6b68 6e65 8c0a 7261 7763 6170  ehhhkhne..rawcap
-000006b0: 7469 6f6e 9468 7575 6825 6854 6827 6828  tion.huuh%hTh'h(
-000006c0: 6829 4b0b 6816 6851 7562 6168 177d 9428  h)K.h.hQubah.}.(
-000006d0: 6819 5d94 681b 5d94 8c0f 746f 6374 7265  h.].h.]...toctre
-000006e0: 652d 7772 6170 7065 7294 6168 1d5d 9468  e-wrapper.ah.].h
-000006f0: 1f5d 9468 215d 9475 6825 684f 6816 682c  .].h!].uh%hOh.h,
-00000700: 6826 6803 6827 6828 6829 4e75 6265 6817  h&h.h'h(h)Nubeh.
-00000710: 7d94 2868 195d 948c 2177 656c 636f 6d65  }.(h.]..!welcome
-00000720: 2d74 6f2d 6e65 7374 6572 2d73 2d64 6f63  -to-nester-s-doc
-00000730: 756d 656e 7461 7469 6f6e 9461 681b 5d94  umentation.ah.].
-00000740: 681d 5d94 8c22 7765 6c63 6f6d 6520 746f  h.].."welcome to
-00000750: 206e 6573 7465 7227 7320 646f 6375 6d65   nester's docume
-00000760: 6e74 6174 696f 6e21 9461 681f 5d94 6821  ntation!.ah.].h!
-00000770: 5d94 7568 2568 2a68 1668 0368 2668 0368  ].uh%h*h.h.h&h.h
-00000780: 2768 2868 294b 0775 6268 2b29 8194 7d94  'h(h)K.ubh+)..}.
-00000790: 2868 0568 0668 075d 9428 6830 2981 947d  (h.h.h.].(h0)..}
-000007a0: 9428 6805 8c12 496e 6469 6365 7320 616e  .(h...Indices an
-000007b0: 6420 7461 626c 6573 9468 075d 9468 118c  d tables.h.].h..
-000007c0: 1249 6e64 6963 6573 2061 6e64 2074 6162  .Indices and tab
-000007d0: 6c65 7394 8594 8194 7d94 2868 1668 9068  les.....}.(h.h.h
-000007e0: 2668 0368 274e 6829 4e75 6261 6817 7d94  &h.h'Nh)Nubah.}.
-000007f0: 2868 195d 9468 1b5d 9468 1d5d 9468 1f5d  (h.].h.].h.].h.]
-00000800: 9468 215d 9475 6825 682f 6816 688d 6826  .h!].uh%h/h.h.h&
-00000810: 6803 6827 6828 6829 4b18 7562 6809 8c0b  h.h'h(h)K.ubh...
-00000820: 6275 6c6c 6574 5f6c 6973 7494 9394 2981  bullet_list...).
-00000830: 947d 9428 6805 6806 6807 5d94 2868 098c  .}.(h.h.h.].(h..
-00000840: 096c 6973 745f 6974 656d 9493 9429 8194  .list_item...)..
-00000850: 7d94 2868 058c 0f3a 7265 663a 6067 656e  }.(h...:ref:`gen
-00000860: 696e 6465 7860 9468 075d 9468 4029 8194  index`.h.].h@)..
-00000870: 7d94 2868 0568 a768 075d 9468 008c 0c70  }.(h.h.h.].h...p
-00000880: 656e 6469 6e67 5f78 7265 6694 9394 2981  ending_xref...).
-00000890: 947d 9428 6805 68a7 6807 5d94 6809 8c06  .}.(h.h.h.].h...
-000008a0: 696e 6c69 6e65 9493 9429 8194 7d94 2868  inline...)..}.(h
-000008b0: 0568 a768 075d 9468 118c 0867 656e 696e  .h.h.].h...genin
-000008c0: 6465 7894 8594 8194 7d94 2868 1668 b368  dex.....}.(h.h.h
-000008d0: 2668 0368 274e 6829 4e75 6261 6817 7d94  &h.h'Nh)Nubah.}.
-000008e0: 2868 195d 9468 1b5d 9428 8c04 7872 6566  (h.].h.].(..xref
-000008f0: 948c 0373 7464 948c 0773 7464 2d72 6566  ...std...std-ref
-00000900: 9465 681d 5d94 681f 5d94 6821 5d94 7568  .eh.].h.].h!].uh
-00000910: 2568 b168 1668 ae75 6261 6817 7d94 2868  %h.h.h.ubah.}.(h
-00000920: 195d 9468 1b5d 9468 1d5d 9468 1f5d 9468  .].h.].h.].h.].h
-00000930: 215d 948c 0672 6566 646f 6394 685f 8c09  !]...refdoc.h_..
-00000940: 7265 6664 6f6d 6169 6e94 68be 8c07 7265  refdomain.h...re
-00000950: 6674 7970 6594 8c03 7265 6694 8c0b 7265  ftype...ref...re
-00000960: 6665 7870 6c69 6369 7494 898c 0772 6566  fexplicit....ref
-00000970: 7761 726e 9488 8c09 7265 6674 6172 6765  warn....reftarge
-00000980: 7494 8c08 6765 6e69 6e64 6578 9475 6825  t...genindex.uh%
-00000990: 68ac 6827 6828 6829 4b1a 6816 68a9 7562  h.h'h(h)K.h.h.ub
-000009a0: 6168 177d 9428 6819 5d94 681b 5d94 681d  ah.}.(h.].h.].h.
-000009b0: 5d94 681f 5d94 6821 5d94 7568 2568 3f68  ].h.].h!].uh%h?h
-000009c0: 2768 2868 294b 1a68 1668 a575 6261 6817  'h(h)K.h.h.ubah.
-000009d0: 7d94 2868 195d 9468 1b5d 9468 1d5d 9468  }.(h.].h.].h.].h
-000009e0: 1f5d 9468 215d 9475 6825 68a3 6816 68a0  .].h!].uh%h.h.h.
-000009f0: 6826 6803 6827 6828 6829 4e75 6268 a429  h&h.h'h(h)Nubh.)
-00000a00: 8194 7d94 2868 058c 0f3a 7265 663a 606d  ..}.(h...:ref:`m
-00000a10: 6f64 696e 6465 7860 9468 075d 9468 4029  odindex`.h.].h@)
-00000a20: 8194 7d94 2868 0568 df68 075d 9468 ad29  ..}.(h.h.h.].h.)
-00000a30: 8194 7d94 2868 0568 df68 075d 9468 b229  ..}.(h.h.h.].h.)
-00000a40: 8194 7d94 2868 0568 df68 075d 9468 118c  ..}.(h.h.h.].h..
-00000a50: 086d 6f64 696e 6465 7894 8594 8194 7d94  .modindex.....}.
-00000a60: 2868 1668 e768 2668 0368 274e 6829 4e75  (h.h.h&h.h'Nh)Nu
-00000a70: 6261 6817 7d94 2868 195d 9468 1b5d 9428  bah.}.(h.].h.].(
-00000a80: 68bd 8c03 7374 6494 8c07 7374 642d 7265  h...std...std-re
-00000a90: 6694 6568 1d5d 9468 1f5d 9468 215d 9475  f.eh.].h.].h!].u
-00000aa0: 6825 68b1 6816 68e4 7562 6168 177d 9428  h%h.h.h.ubah.}.(
-00000ab0: 6819 5d94 681b 5d94 681d 5d94 681f 5d94  h.].h.].h.].h.].
-00000ac0: 6821 5d94 8c06 7265 6664 6f63 9468 5f8c  h!]...refdoc.h_.
-00000ad0: 0972 6566 646f 6d61 696e 9468 f18c 0772  .refdomain.h...r
-00000ae0: 6566 7479 7065 948c 0372 6566 948c 0b72  eftype...ref...r
-00000af0: 6566 6578 706c 6963 6974 9489 8c07 7265  efexplicit....re
-00000b00: 6677 6172 6e94 8868 cf8c 086d 6f64 696e  fwarn..h...modin
-00000b10: 6465 7894 7568 2568 ac68 2768 2868 294b  dex.uh%h.h'h(h)K
-00000b20: 1b68 1668 e175 6261 6817 7d94 2868 195d  .h.h.ubah.}.(h.]
-00000b30: 9468 1b5d 9468 1d5d 9468 1f5d 9468 215d  .h.].h.].h.].h!]
-00000b40: 9475 6825 683f 6827 6828 6829 4b1b 6816  .uh%h?h'h(h)K.h.
-00000b50: 68dd 7562 6168 177d 9428 6819 5d94 681b  h.ubah.}.(h.].h.
-00000b60: 5d94 681d 5d94 681f 5d94 6821 5d94 7568  ].h.].h.].h!].uh
-00000b70: 2568 a368 1668 a068 2668 0368 2768 2868  %h.h.h.h&h.h'h(h
-00000b80: 294e 7562 68a4 2981 947d 9428 6805 8c0d  )Nubh.)..}.(h...
-00000b90: 3a72 6566 3a60 7365 6172 6368 6094 6807  :ref:`search`.h.
-00000ba0: 5d94 6840 2981 947d 9428 6805 6a11 0100  ].h@)..}.(h.j...
-00000bb0: 0068 075d 9468 ad29 8194 7d94 2868 056a  .h.].h.)..}.(h.j
-00000bc0: 1101 0000 6807 5d94 68b2 2981 947d 9428  ....h.].h.)..}.(
-00000bd0: 6805 6a11 0100 0068 075d 9468 118c 0673  h.j....h.].h...s
-00000be0: 6561 7263 6894 8594 8194 7d94 2868 166a  earch.....}.(h.j
-00000bf0: 1901 0000 6826 6803 6827 4e68 294e 7562  ....h&h.h'Nh)Nub
-00000c00: 6168 177d 9428 6819 5d94 681b 5d94 2868  ah.}.(h.].h.].(h
-00000c10: bd8c 0373 7464 948c 0773 7464 2d72 6566  ...std...std-ref
-00000c20: 9465 681d 5d94 681f 5d94 6821 5d94 7568  .eh.].h.].h!].uh
-00000c30: 2568 b168 166a 1601 0000 7562 6168 177d  %h.h.j....ubah.}
-00000c40: 9428 6819 5d94 681b 5d94 681d 5d94 681f  .(h.].h.].h.].h.
-00000c50: 5d94 6821 5d94 8c06 7265 6664 6f63 9468  ].h!]...refdoc.h
-00000c60: 5f8c 0972 6566 646f 6d61 696e 946a 2301  _..refdomain.j#.
-00000c70: 0000 8c07 7265 6674 7970 6594 8c03 7265  ....reftype...re
-00000c80: 6694 8c0b 7265 6665 7870 6c69 6369 7494  f...refexplicit.
-00000c90: 898c 0772 6566 7761 726e 9488 68cf 8c06  ...refwarn..h...
-00000ca0: 7365 6172 6368 9475 6825 68ac 6827 6828  search.uh%h.h'h(
-00000cb0: 6829 4b1c 6816 6a13 0100 0075 6261 6817  h)K.h.j....ubah.
-00000cc0: 7d94 2868 195d 9468 1b5d 9468 1d5d 9468  }.(h.].h.].h.].h
-00000cd0: 1f5d 9468 215d 9475 6825 683f 6827 6828  .].h!].uh%h?h'h(
-00000ce0: 6829 4b1c 6816 6a0f 0100 0075 6261 6817  h)K.h.j....ubah.
-00000cf0: 7d94 2868 195d 9468 1b5d 9468 1d5d 9468  }.(h.].h.].h.].h
-00000d00: 1f5d 9468 215d 9475 6825 68a3 6816 68a0  .].h!].uh%h.h.h.
-00000d10: 6826 6803 6827 6828 6829 4e75 6265 6817  h&h.h'h(h)Nubeh.
-00000d20: 7d94 2868 195d 9468 1b5d 9468 1d5d 9468  }.(h.].h.].h.].h
-00000d30: 1f5d 9468 215d 948c 0662 756c 6c65 7494  .].h!]...bullet.
-00000d40: 8c01 2a94 7568 2568 9e68 2768 2868 294b  ..*.uh%h.h'h(h)K
-00000d50: 1a68 1668 8d68 2668 0375 6265 6817 7d94  .h.h.h&h.ubeh.}.
-00000d60: 2868 195d 948c 1269 6e64 6963 6573 2d61  (h.]...indices-a
-00000d70: 6e64 2d74 6162 6c65 7394 6168 1b5d 9468  nd-tables.ah.].h
-00000d80: 1d5d 948c 1269 6e64 6963 6573 2061 6e64  .]...indices and
-00000d90: 2074 6162 6c65 7394 6168 1f5d 9468 215d   tables.ah.].h!]
-00000da0: 9475 6825 682a 6816 6803 6826 6803 6827  .uh%h*h.h.h&h.h'
-00000db0: 6828 6829 4b18 7562 6568 177d 9428 6819  h(h)K.ubeh.}.(h.
-00000dc0: 5d94 681b 5d94 681d 5d94 681f 5d94 6821  ].h.].h.].h.].h!
-00000dd0: 5d94 8c06 736f 7572 6365 9468 2875 6825  ]...source.h(uh%
-00000de0: 6801 8c0e 6375 7272 656e 745f 736f 7572  h...current_sour
-00000df0: 6365 944e 8c0c 6375 7272 656e 745f 6c69  ce.N..current_li
-00000e00: 6e65 944e 8c08 7365 7474 696e 6773 948c  ne.N..settings..
-00000e10: 1164 6f63 7574 696c 732e 6672 6f6e 7465  .docutils.fronte
-00000e20: 6e64 948c 0656 616c 7565 7394 9394 2981  nd...Values...).
-00000e30: 947d 9428 682f 4e8c 0967 656e 6572 6174  .}.(h/N..generat
-00000e40: 6f72 944e 8c09 6461 7465 7374 616d 7094  or.N..datestamp.
-00000e50: 4e8c 0b73 6f75 7263 655f 6c69 6e6b 944e  N..source_link.N
-00000e60: 8c0a 736f 7572 6365 5f75 726c 944e 8c0d  ..source_url.N..
-00000e70: 746f 635f 6261 636b 6c69 6e6b 7394 8c05  toc_backlinks...
-00000e80: 656e 7472 7994 8c12 666f 6f74 6e6f 7465  entry...footnote
-00000e90: 5f62 6163 6b6c 696e 6b73 944b 018c 0d73  _backlinks.K...s
-00000ea0: 6563 746e 756d 5f78 666f 726d 944b 018c  ectnum_xform.K..
-00000eb0: 0e73 7472 6970 5f63 6f6d 6d65 6e74 7394  .strip_comments.
-00000ec0: 4e8c 1b73 7472 6970 5f65 6c65 6d65 6e74  N..strip_element
-00000ed0: 735f 7769 7468 5f63 6c61 7373 6573 944e  s_with_classes.N
-00000ee0: 8c0d 7374 7269 705f 636c 6173 7365 7394  ..strip_classes.
-00000ef0: 4e8c 0c72 6570 6f72 745f 6c65 7665 6c94  N..report_level.
-00000f00: 4b02 8c0a 6861 6c74 5f6c 6576 656c 944b  K...halt_level.K
-00000f10: 058c 1165 7869 745f 7374 6174 7573 5f6c  ...exit_status_l
-00000f20: 6576 656c 944b 058c 0564 6562 7567 944e  evel.K...debug.N
-00000f30: 8c0e 7761 726e 696e 675f 7374 7265 616d  ..warning_stream
-00000f40: 944e 8c09 7472 6163 6562 6163 6b94 888c  .N..traceback...
-00000f50: 0e69 6e70 7574 5f65 6e63 6f64 696e 6794  .input_encoding.
-00000f60: 8c09 7574 662d 382d 7369 6794 8c1c 696e  ..utf-8-sig...in
-00000f70: 7075 745f 656e 636f 6469 6e67 5f65 7272  put_encoding_err
-00000f80: 6f72 5f68 616e 646c 6572 948c 0673 7472  or_handler...str
-00000f90: 6963 7494 8c0f 6f75 7470 7574 5f65 6e63  ict...output_enc
-00000fa0: 6f64 696e 6794 8c05 7574 662d 3894 8c1d  oding...utf-8...
-00000fb0: 6f75 7470 7574 5f65 6e63 6f64 696e 675f  output_encoding_
-00000fc0: 6572 726f 725f 6861 6e64 6c65 7294 6a74  error_handler.jt
-00000fd0: 0100 008c 0e65 7272 6f72 5f65 6e63 6f64  .....error_encod
-00000fe0: 696e 6794 8c05 7574 662d 3894 8c1c 6572  ing...utf-8...er
-00000ff0: 726f 725f 656e 636f 6469 6e67 5f65 7272  ror_encoding_err
-00001000: 6f72 5f68 616e 646c 6572 948c 1062 6163  or_handler...bac
-00001010: 6b73 6c61 7368 7265 706c 6163 6594 8c0d  kslashreplace...
-00001020: 6c61 6e67 7561 6765 5f63 6f64 6594 8c02  language_code...
-00001030: 656e 948c 1372 6563 6f72 645f 6465 7065  en...record_depe
-00001040: 6e64 656e 6369 6573 944e 8c06 636f 6e66  ndencies.N..conf
-00001050: 6967 944e 8c09 6964 5f70 7265 6669 7894  ig.N..id_prefix.
-00001060: 6806 8c0e 6175 746f 5f69 645f 7072 6566  h...auto_id_pref
-00001070: 6978 948c 0269 6494 8c0d 6475 6d70 5f73  ix...id...dump_s
-00001080: 6574 7469 6e67 7394 4e8c 0e64 756d 705f  ettings.N..dump_
-00001090: 696e 7465 726e 616c 7394 4e8c 0f64 756d  internals.N..dum
-000010a0: 705f 7472 616e 7366 6f72 6d73 944e 8c0f  p_transforms.N..
-000010b0: 6475 6d70 5f70 7365 7564 6f5f 786d 6c94  dump_pseudo_xml.
-000010c0: 4e8c 1065 7870 6f73 655f 696e 7465 726e  N..expose_intern
-000010d0: 616c 7394 4e8c 0e73 7472 6963 745f 7669  als.N..strict_vi
-000010e0: 7369 746f 7294 4e8c 0f5f 6469 7361 626c  sitor.N.._disabl
-000010f0: 655f 636f 6e66 6967 944e 8c07 5f73 6f75  e_config.N.._sou
-00001100: 7263 6594 6828 8c0c 5f64 6573 7469 6e61  rce.h(.._destina
-00001110: 7469 6f6e 944e 8c0d 5f63 6f6e 6669 675f  tion.N.._config_
-00001120: 6669 6c65 7394 5d94 8c16 6669 6c65 5f69  files.]...file_i
-00001130: 6e73 6572 7469 6f6e 5f65 6e61 626c 6564  nsertion_enabled
-00001140: 9488 8c0b 7261 775f 656e 6162 6c65 6494  ....raw_enabled.
-00001150: 4b01 8c11 6c69 6e65 5f6c 656e 6774 685f  K...line_length_
-00001160: 6c69 6d69 7494 4d10 278c 0e70 6570 5f72  limit.M.'..pep_r
-00001170: 6566 6572 656e 6365 7394 4e8c 0c70 6570  eferences.N..pep
-00001180: 5f62 6173 655f 7572 6c94 8c18 6874 7470  _base_url...http
-00001190: 733a 2f2f 7065 7073 2e70 7974 686f 6e2e  s://peps.python.
-000011a0: 6f72 672f 948c 1570 6570 5f66 696c 655f  org/...pep_file_
-000011b0: 7572 6c5f 7465 6d70 6c61 7465 948c 0870  url_template...p
-000011c0: 6570 2d25 3034 6494 8c0e 7266 635f 7265  ep-%04d...rfc_re
-000011d0: 6665 7265 6e63 6573 944e 8c0c 7266 635f  ferences.N..rfc_
-000011e0: 6261 7365 5f75 726c 948c 2668 7474 7073  base_url..&https
-000011f0: 3a2f 2f64 6174 6174 7261 636b 6572 2e69  ://datatracker.i
-00001200: 6574 662e 6f72 672f 646f 632f 6874 6d6c  etf.org/doc/html
-00001210: 2f94 8c09 7461 625f 7769 6474 6894 4b08  /...tab_width.K.
-00001220: 8c1d 7472 696d 5f66 6f6f 746e 6f74 655f  ..trim_footnote_
-00001230: 7265 6665 7265 6e63 655f 7370 6163 6594  reference_space.
-00001240: 898c 1073 796e 7461 785f 6869 6768 6c69  ...syntax_highli
-00001250: 6768 7494 8c04 6c6f 6e67 948c 0c73 6d61  ght...long...sma
-00001260: 7274 5f71 756f 7465 7394 888c 1373 6d61  rt_quotes....sma
-00001270: 7274 7175 6f74 6573 5f6c 6f63 616c 6573  rtquotes_locales
-00001280: 945d 948c 1d63 6861 7261 6374 6572 5f6c  .]...character_l
-00001290: 6576 656c 5f69 6e6c 696e 655f 6d61 726b  evel_inline_mark
-000012a0: 7570 9489 8c0e 646f 6374 6974 6c65 5f78  up....doctitle_x
-000012b0: 666f 726d 9489 8c0d 646f 6369 6e66 6f5f  form....docinfo_
-000012c0: 7866 6f72 6d94 4b01 8c12 7365 6374 7375  xform.K...sectsu
-000012d0: 6274 6974 6c65 5f78 666f 726d 9489 8c0d  btitle_xform....
-000012e0: 696d 6167 655f 6c6f 6164 696e 6794 8c04  image_loading...
-000012f0: 6c69 6e6b 948c 1065 6d62 6564 5f73 7479  link...embed_sty
-00001300: 6c65 7368 6565 7494 898c 1563 6c6f 616b  lesheet....cloak
-00001310: 5f65 6d61 696c 5f61 6464 7265 7373 6573  _email_addresses
-00001320: 9488 8c11 7365 6374 696f 6e5f 7365 6c66  ....section_self
-00001330: 5f6c 696e 6b94 898c 0365 6e76 944e 7562  _link....env.Nub
-00001340: 8c08 7265 706f 7274 6572 944e 8c10 696e  ..reporter.N..in
-00001350: 6469 7265 6374 5f74 6172 6765 7473 945d  direct_targets.]
-00001360: 948c 1173 7562 7374 6974 7574 696f 6e5f  ...substitution_
-00001370: 6465 6673 947d 948c 1273 7562 7374 6974  defs.}...substit
-00001380: 7574 696f 6e5f 6e61 6d65 7394 7d94 8c08  ution_names.}...
-00001390: 7265 666e 616d 6573 947d 948c 0672 6566  refnames.}...ref
-000013a0: 6964 7394 7d94 8c07 6e61 6d65 6964 7394  ids.}...nameids.
-000013b0: 7d94 2868 8a68 876a 4e01 0000 6a4b 0100  }.(h.h.jN...jK..
-000013c0: 0075 8c09 6e61 6d65 7479 7065 7394 7d94  .u..nametypes.}.
-000013d0: 2868 8a89 6a4e 0100 0089 7568 197d 9428  (h..jN....uh.}.(
-000013e0: 6887 682c 6a4b 0100 0068 8d75 8c0d 666f  h.h,jK...h.u..fo
-000013f0: 6f74 6e6f 7465 5f72 6566 7394 7d94 8c0d  otnote_refs.}...
-00001400: 6369 7461 7469 6f6e 5f72 6566 7394 7d94  citation_refs.}.
-00001410: 8c0d 6175 746f 666f 6f74 6e6f 7465 7394  ..autofootnotes.
-00001420: 5d94 8c11 6175 746f 666f 6f74 6e6f 7465  ]...autofootnote
-00001430: 5f72 6566 7394 5d94 8c10 7379 6d62 6f6c  _refs.]...symbol
-00001440: 5f66 6f6f 746e 6f74 6573 945d 948c 1473  _footnotes.]...s
-00001450: 796d 626f 6c5f 666f 6f74 6e6f 7465 5f72  ymbol_footnote_r
-00001460: 6566 7394 5d94 8c09 666f 6f74 6e6f 7465  efs.]...footnote
-00001470: 7394 5d94 8c09 6369 7461 7469 6f6e 7394  s.]...citations.
-00001480: 5d94 8c12 6175 746f 666f 6f74 6e6f 7465  ]...autofootnote
-00001490: 5f73 7461 7274 944b 018c 1573 796d 626f  _start.K...symbo
-000014a0: 6c5f 666f 6f74 6e6f 7465 5f73 7461 7274  l_footnote_start
-000014b0: 944b 008c 0a69 645f 636f 756e 7465 7294  .K...id_counter.
-000014c0: 8c0b 636f 6c6c 6563 7469 6f6e 7394 8c07  ..collections...
-000014d0: 436f 756e 7465 7294 9394 7d94 8594 5294  Counter...}...R.
-000014e0: 8c0e 7061 7273 655f 6d65 7373 6167 6573  ..parse_messages
-000014f0: 945d 948c 1274 7261 6e73 666f 726d 5f6d  .]...transform_m
-00001500: 6573 7361 6765 7394 5d94 8c0b 7472 616e  essages.]...tran
-00001510: 7366 6f72 6d65 7294 4e8c 0b69 6e63 6c75  sformer.N..inclu
-00001520: 6465 5f6c 6f67 945d 948c 0a64 6563 6f72  de_log.]...decor
-00001530: 6174 696f 6e94 4e68 2668 0375 622e       ation.Nh&h.ub.
+000005e0: 8c1a 2020 2054 6865 2060 6e65 7374 6572  ..   The `nester
+000005f0: 5f6c 6f67 6020 6d6f 6475 6c65 948c 0e73  _log` module...s
+00000600: 6f75 7263 652f 6c6f 6767 696e 6794 8694  ource/logging...
+00000610: 8c13 5375 7070 6f72 7465 6420 4c61 6e67  ..Supported Lang
+00000620: 7561 6765 7394 8c13 7375 7070 6f72 7465  uages...supporte
+00000630: 645f 6c61 6e67 7561 6765 7394 8694 658c  d_languages...e.
+00000640: 0c69 6e63 6c75 6465 6669 6c65 7394 5d94  .includefiles.].
+00000650: 2868 6368 6668 6968 6c68 6f68 7265 8c08  (hchfhihlhohre..
+00000660: 6d61 7864 6570 7468 944b 028c 0763 6170  maxdepth.K...cap
+00000670: 7469 6f6e 948c 0943 6f6e 7465 6e74 733a  tion...Contents:
+00000680: 948c 0467 6c6f 6294 898c 0668 6964 6465  ...glob....hidde
+00000690: 6e94 898c 0d69 6e63 6c75 6465 6869 6464  n....includehidd
+000006a0: 656e 9489 8c08 6e75 6d62 6572 6564 944b  en....numbered.K
+000006b0: 008c 0a74 6974 6c65 736f 6e6c 7994 898c  ...titlesonly...
+000006c0: 0a72 6177 656e 7472 6965 7394 5d94 2868  .rawentries.].(h
+000006d0: 6268 6568 6868 6b68 6e68 7165 8c0a 7261  bhehhhkhnhqe..ra
+000006e0: 7763 6170 7469 6f6e 9468 7875 6825 6854  wcaption.hxuh%hT
+000006f0: 6827 6828 6829 4b0b 6816 6851 7562 6168  h'h(h)K.h.hQubah
+00000700: 177d 9428 6819 5d94 681b 5d94 8c0f 746f  .}.(h.].h.]...to
+00000710: 6374 7265 652d 7772 6170 7065 7294 6168  ctree-wrapper.ah
+00000720: 1d5d 9468 1f5d 9468 215d 9475 6825 684f  .].h.].h!].uh%hO
+00000730: 6816 682c 6826 6803 6827 6828 6829 4e75  h.h,h&h.h'h(h)Nu
+00000740: 6265 6817 7d94 2868 195d 948c 2177 656c  beh.}.(h.]..!wel
+00000750: 636f 6d65 2d74 6f2d 6e65 7374 6572 2d73  come-to-nester-s
+00000760: 2d64 6f63 756d 656e 7461 7469 6f6e 9461  -documentation.a
+00000770: 681b 5d94 681d 5d94 8c22 7765 6c63 6f6d  h.].h.].."welcom
+00000780: 6520 746f 206e 6573 7465 7227 7320 646f  e to nester's do
+00000790: 6375 6d65 6e74 6174 696f 6e21 9461 681f  cumentation!.ah.
+000007a0: 5d94 6821 5d94 7568 2568 2a68 1668 0368  ].h!].uh%h*h.h.h
+000007b0: 2668 0368 2768 2868 294b 0775 6268 2b29  &h.h'h(h)K.ubh+)
+000007c0: 8194 7d94 2868 0568 0668 075d 9428 6830  ..}.(h.h.h.].(h0
+000007d0: 2981 947d 9428 6805 8c12 496e 6469 6365  )..}.(h...Indice
+000007e0: 7320 616e 6420 7461 626c 6573 9468 075d  s and tables.h.]
+000007f0: 9468 118c 1249 6e64 6963 6573 2061 6e64  .h...Indices and
+00000800: 2074 6162 6c65 7394 8594 8194 7d94 2868   tables.....}.(h
+00000810: 1668 9368 2668 0368 274e 6829 4e75 6261  .h.h&h.h'Nh)Nuba
+00000820: 6817 7d94 2868 195d 9468 1b5d 9468 1d5d  h.}.(h.].h.].h.]
+00000830: 9468 1f5d 9468 215d 9475 6825 682f 6816  .h.].h!].uh%h/h.
+00000840: 6890 6826 6803 6827 6828 6829 4b19 7562  h.h&h.h'h(h)K.ub
+00000850: 6809 8c0b 6275 6c6c 6574 5f6c 6973 7494  h...bullet_list.
+00000860: 9394 2981 947d 9428 6805 6806 6807 5d94  ..)..}.(h.h.h.].
+00000870: 2868 098c 096c 6973 745f 6974 656d 9493  (h...list_item..
+00000880: 9429 8194 7d94 2868 058c 0f3a 7265 663a  .)..}.(h...:ref:
+00000890: 6067 656e 696e 6465 7860 9468 075d 9468  `genindex`.h.].h
+000008a0: 4029 8194 7d94 2868 0568 aa68 075d 9468  @)..}.(h.h.h.].h
+000008b0: 008c 0c70 656e 6469 6e67 5f78 7265 6694  ...pending_xref.
+000008c0: 9394 2981 947d 9428 6805 68aa 6807 5d94  ..)..}.(h.h.h.].
+000008d0: 6809 8c06 696e 6c69 6e65 9493 9429 8194  h...inline...)..
+000008e0: 7d94 2868 0568 aa68 075d 9468 118c 0867  }.(h.h.h.].h...g
+000008f0: 656e 696e 6465 7894 8594 8194 7d94 2868  enindex.....}.(h
+00000900: 1668 b668 2668 0368 274e 6829 4e75 6261  .h.h&h.h'Nh)Nuba
+00000910: 6817 7d94 2868 195d 9468 1b5d 9428 8c04  h.}.(h.].h.].(..
+00000920: 7872 6566 948c 0373 7464 948c 0773 7464  xref...std...std
+00000930: 2d72 6566 9465 681d 5d94 681f 5d94 6821  -ref.eh.].h.].h!
+00000940: 5d94 7568 2568 b468 1668 b175 6261 6817  ].uh%h.h.h.ubah.
+00000950: 7d94 2868 195d 9468 1b5d 9468 1d5d 9468  }.(h.].h.].h.].h
+00000960: 1f5d 9468 215d 948c 0672 6566 646f 6394  .].h!]...refdoc.
+00000970: 685f 8c09 7265 6664 6f6d 6169 6e94 68c1  h_..refdomain.h.
+00000980: 8c07 7265 6674 7970 6594 8c03 7265 6694  ..reftype...ref.
+00000990: 8c0b 7265 6665 7870 6c69 6369 7494 898c  ..refexplicit...
+000009a0: 0772 6566 7761 726e 9488 8c09 7265 6674  .refwarn....reft
+000009b0: 6172 6765 7494 8c08 6765 6e69 6e64 6578  arget...genindex
+000009c0: 9475 6825 68af 6827 6828 6829 4b1b 6816  .uh%h.h'h(h)K.h.
+000009d0: 68ac 7562 6168 177d 9428 6819 5d94 681b  h.ubah.}.(h.].h.
+000009e0: 5d94 681d 5d94 681f 5d94 6821 5d94 7568  ].h.].h.].h!].uh
+000009f0: 2568 3f68 2768 2868 294b 1b68 1668 a875  %h?h'h(h)K.h.h.u
+00000a00: 6261 6817 7d94 2868 195d 9468 1b5d 9468  bah.}.(h.].h.].h
+00000a10: 1d5d 9468 1f5d 9468 215d 9475 6825 68a6  .].h.].h!].uh%h.
+00000a20: 6816 68a3 6826 6803 6827 6828 6829 4e75  h.h.h&h.h'h(h)Nu
+00000a30: 6268 a729 8194 7d94 2868 058c 0f3a 7265  bh.)..}.(h...:re
+00000a40: 663a 606d 6f64 696e 6465 7860 9468 075d  f:`modindex`.h.]
+00000a50: 9468 4029 8194 7d94 2868 0568 e268 075d  .h@)..}.(h.h.h.]
+00000a60: 9468 b029 8194 7d94 2868 0568 e268 075d  .h.)..}.(h.h.h.]
+00000a70: 9468 b529 8194 7d94 2868 0568 e268 075d  .h.)..}.(h.h.h.]
+00000a80: 9468 118c 086d 6f64 696e 6465 7894 8594  .h...modindex...
+00000a90: 8194 7d94 2868 1668 ea68 2668 0368 274e  ..}.(h.h.h&h.h'N
+00000aa0: 6829 4e75 6261 6817 7d94 2868 195d 9468  h)Nubah.}.(h.].h
+00000ab0: 1b5d 9428 68c0 8c03 7374 6494 8c07 7374  .].(h...std...st
+00000ac0: 642d 7265 6694 6568 1d5d 9468 1f5d 9468  d-ref.eh.].h.].h
+00000ad0: 215d 9475 6825 68b4 6816 68e7 7562 6168  !].uh%h.h.h.ubah
+00000ae0: 177d 9428 6819 5d94 681b 5d94 681d 5d94  .}.(h.].h.].h.].
+00000af0: 681f 5d94 6821 5d94 8c06 7265 6664 6f63  h.].h!]...refdoc
+00000b00: 9468 5f8c 0972 6566 646f 6d61 696e 9468  .h_..refdomain.h
+00000b10: f48c 0772 6566 7479 7065 948c 0372 6566  ...reftype...ref
+00000b20: 948c 0b72 6566 6578 706c 6963 6974 9489  ...refexplicit..
+00000b30: 8c07 7265 6677 6172 6e94 8868 d28c 086d  ..refwarn..h...m
+00000b40: 6f64 696e 6465 7894 7568 2568 af68 2768  odindex.uh%h.h'h
+00000b50: 2868 294b 1c68 1668 e475 6261 6817 7d94  (h)K.h.h.ubah.}.
+00000b60: 2868 195d 9468 1b5d 9468 1d5d 9468 1f5d  (h.].h.].h.].h.]
+00000b70: 9468 215d 9475 6825 683f 6827 6828 6829  .h!].uh%h?h'h(h)
+00000b80: 4b1c 6816 68e0 7562 6168 177d 9428 6819  K.h.h.ubah.}.(h.
+00000b90: 5d94 681b 5d94 681d 5d94 681f 5d94 6821  ].h.].h.].h.].h!
+00000ba0: 5d94 7568 2568 a668 1668 a368 2668 0368  ].uh%h.h.h.h&h.h
+00000bb0: 2768 2868 294e 7562 68a7 2981 947d 9428  'h(h)Nubh.)..}.(
+00000bc0: 6805 8c0d 3a72 6566 3a60 7365 6172 6368  h...:ref:`search
+00000bd0: 6094 6807 5d94 6840 2981 947d 9428 6805  `.h.].h@)..}.(h.
+00000be0: 6a14 0100 0068 075d 9468 b029 8194 7d94  j....h.].h.)..}.
+00000bf0: 2868 056a 1401 0000 6807 5d94 68b5 2981  (h.j....h.].h.).
+00000c00: 947d 9428 6805 6a14 0100 0068 075d 9468  .}.(h.j....h.].h
+00000c10: 118c 0673 6561 7263 6894 8594 8194 7d94  ...search.....}.
+00000c20: 2868 166a 1c01 0000 6826 6803 6827 4e68  (h.j....h&h.h'Nh
+00000c30: 294e 7562 6168 177d 9428 6819 5d94 681b  )Nubah.}.(h.].h.
+00000c40: 5d94 2868 c08c 0373 7464 948c 0773 7464  ].(h...std...std
+00000c50: 2d72 6566 9465 681d 5d94 681f 5d94 6821  -ref.eh.].h.].h!
+00000c60: 5d94 7568 2568 b468 166a 1901 0000 7562  ].uh%h.h.j....ub
+00000c70: 6168 177d 9428 6819 5d94 681b 5d94 681d  ah.}.(h.].h.].h.
+00000c80: 5d94 681f 5d94 6821 5d94 8c06 7265 6664  ].h.].h!]...refd
+00000c90: 6f63 9468 5f8c 0972 6566 646f 6d61 696e  oc.h_..refdomain
+00000ca0: 946a 2601 0000 8c07 7265 6674 7970 6594  .j&.....reftype.
+00000cb0: 8c03 7265 6694 8c0b 7265 6665 7870 6c69  ..ref...refexpli
+00000cc0: 6369 7494 898c 0772 6566 7761 726e 9488  cit....refwarn..
+00000cd0: 68d2 8c06 7365 6172 6368 9475 6825 68af  h...search.uh%h.
+00000ce0: 6827 6828 6829 4b1d 6816 6a16 0100 0075  h'h(h)K.h.j....u
+00000cf0: 6261 6817 7d94 2868 195d 9468 1b5d 9468  bah.}.(h.].h.].h
+00000d00: 1d5d 9468 1f5d 9468 215d 9475 6825 683f  .].h.].h!].uh%h?
+00000d10: 6827 6828 6829 4b1d 6816 6a12 0100 0075  h'h(h)K.h.j....u
+00000d20: 6261 6817 7d94 2868 195d 9468 1b5d 9468  bah.}.(h.].h.].h
+00000d30: 1d5d 9468 1f5d 9468 215d 9475 6825 68a6  .].h.].h!].uh%h.
+00000d40: 6816 68a3 6826 6803 6827 6828 6829 4e75  h.h.h&h.h'h(h)Nu
+00000d50: 6265 6817 7d94 2868 195d 9468 1b5d 9468  beh.}.(h.].h.].h
+00000d60: 1d5d 9468 1f5d 9468 215d 948c 0662 756c  .].h.].h!]...bul
+00000d70: 6c65 7494 8c01 2a94 7568 2568 a168 2768  let...*.uh%h.h'h
+00000d80: 2868 294b 1b68 1668 9068 2668 0375 6265  (h)K.h.h.h&h.ube
+00000d90: 6817 7d94 2868 195d 948c 1269 6e64 6963  h.}.(h.]...indic
+00000da0: 6573 2d61 6e64 2d74 6162 6c65 7394 6168  es-and-tables.ah
+00000db0: 1b5d 9468 1d5d 948c 1269 6e64 6963 6573  .].h.]...indices
+00000dc0: 2061 6e64 2074 6162 6c65 7394 6168 1f5d   and tables.ah.]
+00000dd0: 9468 215d 9475 6825 682a 6816 6803 6826  .h!].uh%h*h.h.h&
+00000de0: 6803 6827 6828 6829 4b19 7562 6568 177d  h.h'h(h)K.ubeh.}
+00000df0: 9428 6819 5d94 681b 5d94 681d 5d94 681f  .(h.].h.].h.].h.
+00000e00: 5d94 6821 5d94 8c06 736f 7572 6365 9468  ].h!]...source.h
+00000e10: 2875 6825 6801 8c0e 6375 7272 656e 745f  (uh%h...current_
+00000e20: 736f 7572 6365 944e 8c0c 6375 7272 656e  source.N..curren
+00000e30: 745f 6c69 6e65 944e 8c08 7365 7474 696e  t_line.N..settin
+00000e40: 6773 948c 1164 6f63 7574 696c 732e 6672  gs...docutils.fr
+00000e50: 6f6e 7465 6e64 948c 0656 616c 7565 7394  ontend...Values.
+00000e60: 9394 2981 947d 9428 682f 4e8c 0967 656e  ..)..}.(h/N..gen
+00000e70: 6572 6174 6f72 944e 8c09 6461 7465 7374  erator.N..datest
+00000e80: 616d 7094 4e8c 0b73 6f75 7263 655f 6c69  amp.N..source_li
+00000e90: 6e6b 944e 8c0a 736f 7572 6365 5f75 726c  nk.N..source_url
+00000ea0: 944e 8c0d 746f 635f 6261 636b 6c69 6e6b  .N..toc_backlink
+00000eb0: 7394 8c05 656e 7472 7994 8c12 666f 6f74  s...entry...foot
+00000ec0: 6e6f 7465 5f62 6163 6b6c 696e 6b73 944b  note_backlinks.K
+00000ed0: 018c 0d73 6563 746e 756d 5f78 666f 726d  ...sectnum_xform
+00000ee0: 944b 018c 0e73 7472 6970 5f63 6f6d 6d65  .K...strip_comme
+00000ef0: 6e74 7394 4e8c 1b73 7472 6970 5f65 6c65  nts.N..strip_ele
+00000f00: 6d65 6e74 735f 7769 7468 5f63 6c61 7373  ments_with_class
+00000f10: 6573 944e 8c0d 7374 7269 705f 636c 6173  es.N..strip_clas
+00000f20: 7365 7394 4e8c 0c72 6570 6f72 745f 6c65  ses.N..report_le
+00000f30: 7665 6c94 4b02 8c0a 6861 6c74 5f6c 6576  vel.K...halt_lev
+00000f40: 656c 944b 058c 1165 7869 745f 7374 6174  el.K...exit_stat
+00000f50: 7573 5f6c 6576 656c 944b 058c 0564 6562  us_level.K...deb
+00000f60: 7567 944e 8c0e 7761 726e 696e 675f 7374  ug.N..warning_st
+00000f70: 7265 616d 944e 8c09 7472 6163 6562 6163  ream.N..tracebac
+00000f80: 6b94 888c 0e69 6e70 7574 5f65 6e63 6f64  k....input_encod
+00000f90: 696e 6794 8c09 7574 662d 382d 7369 6794  ing...utf-8-sig.
+00000fa0: 8c1c 696e 7075 745f 656e 636f 6469 6e67  ..input_encoding
+00000fb0: 5f65 7272 6f72 5f68 616e 646c 6572 948c  _error_handler..
+00000fc0: 0673 7472 6963 7494 8c0f 6f75 7470 7574  .strict...output
+00000fd0: 5f65 6e63 6f64 696e 6794 8c05 7574 662d  _encoding...utf-
+00000fe0: 3894 8c1d 6f75 7470 7574 5f65 6e63 6f64  8...output_encod
+00000ff0: 696e 675f 6572 726f 725f 6861 6e64 6c65  ing_error_handle
+00001000: 7294 6a77 0100 008c 0e65 7272 6f72 5f65  r.jw.....error_e
+00001010: 6e63 6f64 696e 6794 8c05 7574 662d 3894  ncoding...utf-8.
+00001020: 8c1c 6572 726f 725f 656e 636f 6469 6e67  ..error_encoding
+00001030: 5f65 7272 6f72 5f68 616e 646c 6572 948c  _error_handler..
+00001040: 1062 6163 6b73 6c61 7368 7265 706c 6163  .backslashreplac
+00001050: 6594 8c0d 6c61 6e67 7561 6765 5f63 6f64  e...language_cod
+00001060: 6594 8c02 656e 948c 1372 6563 6f72 645f  e...en...record_
+00001070: 6465 7065 6e64 656e 6369 6573 944e 8c06  dependencies.N..
+00001080: 636f 6e66 6967 944e 8c09 6964 5f70 7265  config.N..id_pre
+00001090: 6669 7894 6806 8c0e 6175 746f 5f69 645f  fix.h...auto_id_
+000010a0: 7072 6566 6978 948c 0269 6494 8c0d 6475  prefix...id...du
+000010b0: 6d70 5f73 6574 7469 6e67 7394 4e8c 0e64  mp_settings.N..d
+000010c0: 756d 705f 696e 7465 726e 616c 7394 4e8c  ump_internals.N.
+000010d0: 0f64 756d 705f 7472 616e 7366 6f72 6d73  .dump_transforms
+000010e0: 944e 8c0f 6475 6d70 5f70 7365 7564 6f5f  .N..dump_pseudo_
+000010f0: 786d 6c94 4e8c 1065 7870 6f73 655f 696e  xml.N..expose_in
+00001100: 7465 726e 616c 7394 4e8c 0e73 7472 6963  ternals.N..stric
+00001110: 745f 7669 7369 746f 7294 4e8c 0f5f 6469  t_visitor.N.._di
+00001120: 7361 626c 655f 636f 6e66 6967 944e 8c07  sable_config.N..
+00001130: 5f73 6f75 7263 6594 6828 8c0c 5f64 6573  _source.h(.._des
+00001140: 7469 6e61 7469 6f6e 944e 8c0d 5f63 6f6e  tination.N.._con
+00001150: 6669 675f 6669 6c65 7394 5d94 8c16 6669  fig_files.]...fi
+00001160: 6c65 5f69 6e73 6572 7469 6f6e 5f65 6e61  le_insertion_ena
+00001170: 626c 6564 9488 8c0b 7261 775f 656e 6162  bled....raw_enab
+00001180: 6c65 6494 4b01 8c11 6c69 6e65 5f6c 656e  led.K...line_len
+00001190: 6774 685f 6c69 6d69 7494 4d10 278c 0e70  gth_limit.M.'..p
+000011a0: 6570 5f72 6566 6572 656e 6365 7394 4e8c  ep_references.N.
+000011b0: 0c70 6570 5f62 6173 655f 7572 6c94 8c18  .pep_base_url...
+000011c0: 6874 7470 733a 2f2f 7065 7073 2e70 7974  https://peps.pyt
+000011d0: 686f 6e2e 6f72 672f 948c 1570 6570 5f66  hon.org/...pep_f
+000011e0: 696c 655f 7572 6c5f 7465 6d70 6c61 7465  ile_url_template
+000011f0: 948c 0870 6570 2d25 3034 6494 8c0e 7266  ...pep-%04d...rf
+00001200: 635f 7265 6665 7265 6e63 6573 944e 8c0c  c_references.N..
+00001210: 7266 635f 6261 7365 5f75 726c 948c 2668  rfc_base_url..&h
+00001220: 7474 7073 3a2f 2f64 6174 6174 7261 636b  ttps://datatrack
+00001230: 6572 2e69 6574 662e 6f72 672f 646f 632f  er.ietf.org/doc/
+00001240: 6874 6d6c 2f94 8c09 7461 625f 7769 6474  html/...tab_widt
+00001250: 6894 4b08 8c1d 7472 696d 5f66 6f6f 746e  h.K...trim_footn
+00001260: 6f74 655f 7265 6665 7265 6e63 655f 7370  ote_reference_sp
+00001270: 6163 6594 898c 1073 796e 7461 785f 6869  ace....syntax_hi
+00001280: 6768 6c69 6768 7494 8c04 6c6f 6e67 948c  ghlight...long..
+00001290: 0c73 6d61 7274 5f71 756f 7465 7394 888c  .smart_quotes...
+000012a0: 1373 6d61 7274 7175 6f74 6573 5f6c 6f63  .smartquotes_loc
+000012b0: 616c 6573 945d 948c 1d63 6861 7261 6374  ales.]...charact
+000012c0: 6572 5f6c 6576 656c 5f69 6e6c 696e 655f  er_level_inline_
+000012d0: 6d61 726b 7570 9489 8c0e 646f 6374 6974  markup....doctit
+000012e0: 6c65 5f78 666f 726d 9489 8c0d 646f 6369  le_xform....doci
+000012f0: 6e66 6f5f 7866 6f72 6d94 4b01 8c12 7365  nfo_xform.K...se
+00001300: 6374 7375 6274 6974 6c65 5f78 666f 726d  ctsubtitle_xform
+00001310: 9489 8c0d 696d 6167 655f 6c6f 6164 696e  ....image_loadin
+00001320: 6794 8c04 6c69 6e6b 948c 1065 6d62 6564  g...link...embed
+00001330: 5f73 7479 6c65 7368 6565 7494 898c 1563  _stylesheet....c
+00001340: 6c6f 616b 5f65 6d61 696c 5f61 6464 7265  loak_email_addre
+00001350: 7373 6573 9488 8c11 7365 6374 696f 6e5f  sses....section_
+00001360: 7365 6c66 5f6c 696e 6b94 898c 0365 6e76  self_link....env
+00001370: 944e 7562 8c08 7265 706f 7274 6572 944e  .Nub..reporter.N
+00001380: 8c10 696e 6469 7265 6374 5f74 6172 6765  ..indirect_targe
+00001390: 7473 945d 948c 1173 7562 7374 6974 7574  ts.]...substitut
+000013a0: 696f 6e5f 6465 6673 947d 948c 1273 7562  ion_defs.}...sub
+000013b0: 7374 6974 7574 696f 6e5f 6e61 6d65 7394  stitution_names.
+000013c0: 7d94 8c08 7265 666e 616d 6573 947d 948c  }...refnames.}..
+000013d0: 0672 6566 6964 7394 7d94 8c07 6e61 6d65  .refids.}...name
+000013e0: 6964 7394 7d94 2868 8d68 8a6a 5101 0000  ids.}.(h.h.jQ...
+000013f0: 6a4e 0100 0075 8c09 6e61 6d65 7479 7065  jN...u..nametype
+00001400: 7394 7d94 2868 8d89 6a51 0100 0089 7568  s.}.(h..jQ....uh
+00001410: 197d 9428 688a 682c 6a4e 0100 0068 9075  .}.(h.h,jN...h.u
+00001420: 8c0d 666f 6f74 6e6f 7465 5f72 6566 7394  ..footnote_refs.
+00001430: 7d94 8c0d 6369 7461 7469 6f6e 5f72 6566  }...citation_ref
+00001440: 7394 7d94 8c0d 6175 746f 666f 6f74 6e6f  s.}...autofootno
+00001450: 7465 7394 5d94 8c11 6175 746f 666f 6f74  tes.]...autofoot
+00001460: 6e6f 7465 5f72 6566 7394 5d94 8c10 7379  note_refs.]...sy
+00001470: 6d62 6f6c 5f66 6f6f 746e 6f74 6573 945d  mbol_footnotes.]
+00001480: 948c 1473 796d 626f 6c5f 666f 6f74 6e6f  ...symbol_footno
+00001490: 7465 5f72 6566 7394 5d94 8c09 666f 6f74  te_refs.]...foot
+000014a0: 6e6f 7465 7394 5d94 8c09 6369 7461 7469  notes.]...citati
+000014b0: 6f6e 7394 5d94 8c12 6175 746f 666f 6f74  ons.]...autofoot
+000014c0: 6e6f 7465 5f73 7461 7274 944b 018c 1573  note_start.K...s
+000014d0: 796d 626f 6c5f 666f 6f74 6e6f 7465 5f73  ymbol_footnote_s
+000014e0: 7461 7274 944b 008c 0a69 645f 636f 756e  tart.K...id_coun
+000014f0: 7465 7294 8c0b 636f 6c6c 6563 7469 6f6e  ter...collection
+00001500: 7394 8c07 436f 756e 7465 7294 9394 7d94  s...Counter...}.
+00001510: 8594 5294 8c0e 7061 7273 655f 6d65 7373  ..R...parse_mess
+00001520: 6167 6573 945d 948c 1274 7261 6e73 666f  ages.]...transfo
+00001530: 726d 5f6d 6573 7361 6765 7394 5d94 8c0b  rm_messages.]...
+00001540: 7472 616e 7366 6f72 6d65 7294 4e8c 0b69  transformer.N..i
+00001550: 6e63 6c75 6465 5f6c 6f67 945d 948c 0a64  nclude_log.]...d
+00001560: 6563 6f72 6174 696f 6e94 4e68 2668 0375  ecoration.Nh&h.u
+00001570: 622e                                     b.
```

### Comparing `nester-struct-0.5.1/docs/_build/html/.doctrees/installation_guide.doctree` & `nester-struct-0.5.2/docs/_build/html/.doctrees/installation_guide.doctree`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8005 95ea 2700 0000 0000 008c 0f73 7068  ....'........sph
+00000000: 8005 95eb 3700 0000 0000 008c 0f73 7068  ....7........sph
 00000010: 696e 782e 6164 646e 6f64 6573 948c 0864  inx.addnodes...d
 00000020: 6f63 756d 656e 7494 9394 2981 947d 9428  ocument...)..}.(
 00000030: 8c09 7261 7773 6f75 7263 6594 8c00 948c  ..rawsource.....
 00000040: 0863 6869 6c64 7265 6e94 5d94 8c0e 646f  .children.]...do
 00000050: 6375 7469 6c73 2e6e 6f64 6573 948c 0773  cutils.nodes...s
 00000060: 6563 7469 6f6e 9493 9429 8194 7d94 2868  ection...)..}.(h
 00000070: 0568 0668 075d 9428 6809 8c05 7469 746c  .h.h.].(h...titl
@@ -321,320 +321,576 @@
 00001400: 7320 6973 2077 6861 7420 7765 2077 696c  s is what we wil
 00001410: 6c20 6f66 6665 7220 6669 7273 742e 9485  l offer first...
 00001420: 9481 947d 9428 681b 6ad9 0100 0068 1c68  ...}.(h.j....h.h
 00001430: 0368 1d4e 681e 4e75 6265 681f 7d94 2868  .h.Nh.Nubeh.}.(h
 00001440: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
 00001450: 295d 9475 682b 682d 681d 682c 681e 4b20  )].uh+h-h.h,h.K 
 00001460: 681b 6a64 0100 0068 1c68 0375 6268 2e29  h.jd...h.h.ubh.)
-00001470: 8194 7d94 2868 058c 4e4e 6f74 653a 2054  ..}.(h..NNote: T
-00001480: 6869 7320 6973 2061 2066 6561 7475 7265  his is a feature
-00001490: 2077 6520 7769 6c6c 206f 6666 6572 2061   we will offer a
-000014a0: 7420 736f 6d65 2070 6f69 6e74 2e20 4e6f  t some point. No
-000014b0: 2064 6174 6573 2061 7265 2070 6c61 6e6e   dates are plann
-000014c0: 6564 2079 6574 2194 6807 5d94 6816 8c4e  ed yet!.h.].h..N
-000014d0: 4e6f 7465 3a20 5468 6973 2069 7320 6120  Note: This is a 
-000014e0: 6665 6174 7572 6520 7765 2077 696c 6c20  feature we will 
-000014f0: 6f66 6665 7220 6174 2073 6f6d 6520 706f  offer at some po
-00001500: 696e 742e 204e 6f20 6461 7465 7320 6172  int. No dates ar
-00001510: 6520 706c 616e 6e65 6420 7965 7421 9485  e planned yet!..
-00001520: 9481 947d 9428 681b 6af9 0100 0068 1c68  ...}.(h.j....h.h
-00001530: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
-00001540: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-00001550: 295d 9475 682b 682d 681d 682c 681e 4b22  )].uh+h-h.h,h.K"
-00001560: 681b 6a64 0100 0068 1c68 0375 6268 2e29  h.jd...h.h.ubh.)
-00001570: 8194 7d94 2868 058c 1154 6f20 696e 7374  ..}.(h...To inst
-00001580: 616c 6c20 6974 2072 756e 9468 075d 9468  all it run.h.].h
-00001590: 168c 1154 6f20 696e 7374 616c 6c20 6974  ...To install it
-000015a0: 2072 756e 9485 9481 947d 9428 681b 6a07   run.....}.(h.j.
-000015b0: 0200 0068 1c68 0368 1d4e 681e 4e75 6261  ...h.h.h.Nh.Nuba
-000015c0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-000015d0: 9468 275d 9468 295d 9475 682b 682d 681d  .h'].h)].uh+h-h.
-000015e0: 682c 681e 4b24 681b 6a64 0100 0068 1c68  h,h.K$h.jd...h.h
-000015f0: 0375 626a 2a01 0000 2981 947d 9428 6805  .ubj*...)..}.(h.
-00001600: 8c15 7375 646f 207a 7970 7065 7220 696e  ..sudo zypper in
-00001610: 206e 6573 7465 7294 6807 5d94 6816 8c15   nester.h.].h...
-00001620: 7375 646f 207a 7970 7065 7220 696e 206e  sudo zypper in n
-00001630: 6573 7465 7294 8594 8194 7d94 681b 6a15  ester.....}.h.j.
-00001640: 0200 0073 6261 681f 7d94 2868 215d 9468  ...sbah.}.(h!].h
-00001650: 235d 9468 255d 9468 275d 9468 295d 946a  #].h%].h'].h)].j
-00001660: 3901 0000 6a3a 0100 006a 3b01 0000 896a  9...j:...j;....j
-00001670: 3c01 0000 8c05 7368 656c 6c94 6a3e 0100  <.....shell.j>..
-00001680: 007d 9475 682b 6a29 0100 0068 1d68 2c68  .}.uh+j)...h.h,h
-00001690: 1e4b 2668 1b6a 6401 0000 681c 6803 7562  .K&h.jd...h.h.ub
-000016a0: 682e 2981 947d 9428 6805 8c20 5468 6973  h.)..}.(h.. This
-000016b0: 2073 686f 756c 6420 696e 7374 616c 6c20   should install 
-000016c0: 7468 6520 7061 636b 6167 652e 9468 075d  the package..h.]
-000016d0: 9468 168c 2054 6869 7320 7368 6f75 6c64  .h.. This should
-000016e0: 2069 6e73 7461 6c6c 2074 6865 2070 6163   install the pac
-000016f0: 6b61 6765 2e94 8594 8194 7d94 2868 1b6a  kage......}.(h.j
-00001700: 2502 0000 681c 6803 681d 4e68 1e4e 7562  %...h.h.h.Nh.Nub
-00001710: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
-00001720: 5d94 6827 5d94 6829 5d94 7568 2b68 2d68  ].h'].h)].uh+h-h
-00001730: 1d68 2c68 1e4b 2a68 1b6a 6401 0000 681c  .h,h.K*h.jd...h.
-00001740: 6803 7562 6568 1f7d 9428 6821 5d94 8c1b  h.ubeh.}.(h!]...
-00001750: 696e 7374 616c 6c61 7469 6f6e 2d61 732d  installation-as-
-00001760: 7270 6d2d 7061 636b 6167 6594 6168 235d  rpm-package.ah#]
-00001770: 9468 255d 948c 1b69 6e73 7461 6c6c 6174  .h%]...installat
-00001780: 696f 6e20 6173 2072 706d 2070 6163 6b61  ion as rpm packa
-00001790: 6765 9461 6827 5d94 6829 5d94 7568 2b68  ge.ah'].h)].uh+h
-000017a0: 0a68 1b68 0c68 1c68 0368 1d68 2c68 1e4b  .h.h.h.h.h.h,h.K
-000017b0: 1975 6268 0b29 8194 7d94 2868 0568 0668  .ubh.)..}.(h.h.h
-000017c0: 075d 9428 6810 2981 947d 9428 6805 8c14  .].(h.)..}.(h...
-000017d0: 4275 696c 6469 6e67 2066 726f 6d20 736f  Building from so
-000017e0: 7572 6365 9468 075d 9468 168c 1442 7569  urce.h.].h...Bui
-000017f0: 6c64 696e 6720 6672 6f6d 2073 6f75 7263  lding from sourc
-00001800: 6594 8594 8194 7d94 2868 1b6a 3e02 0000  e.....}.(h.j>...
-00001810: 681c 6803 681d 4e68 1e4e 7562 6168 1f7d  h.h.h.Nh.Nubah.}
-00001820: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-00001830: 5d94 6829 5d94 7568 2b68 0f68 1b6a 3b02  ].h)].uh+h.h.j;.
-00001840: 0000 681c 6803 681d 682c 681e 4b2d 7562  ..h.h.h.h,h.K-ub
-00001850: 682e 2981 947d 9428 6805 8c6e 536f 6d65  h.)..}.(h..nSome
-00001860: 7469 6d65 7320 696e 7374 616c 6c69 6e67  times installing
-00001870: 2066 726f 6d20 7368 6164 7920 736f 7572   from shady sour
-00001880: 6365 7320 6d61 7920 6e6f 7420 6265 2079  ces may not be y
-00001890: 6f75 7220 7468 696e 672e 2046 6561 7220  our thing. Fear 
-000018a0: 6e6f 7567 6874 210a 596f 7520 6361 6e20  nought!.You can 
-000018b0: 616c 736f 2062 7569 6c64 2069 7420 6672  also build it fr
-000018c0: 6f6d 2073 6f75 7263 652e 9468 075d 9468  om source..h.].h
-000018d0: 168c 6e53 6f6d 6574 696d 6573 2069 6e73  ..nSometimes ins
-000018e0: 7461 6c6c 696e 6720 6672 6f6d 2073 6861  talling from sha
-000018f0: 6479 2073 6f75 7263 6573 206d 6179 206e  dy sources may n
-00001900: 6f74 2062 6520 796f 7572 2074 6869 6e67  ot be your thing
-00001910: 2e20 4665 6172 206e 6f75 6768 7421 0a59  . Fear nought!.Y
-00001920: 6f75 2063 616e 2061 6c73 6f20 6275 696c  ou can also buil
-00001930: 6420 6974 2066 726f 6d20 736f 7572 6365  d it from source
-00001940: 2e94 8594 8194 7d94 2868 1b6a 4c02 0000  ......}.(h.jL...
-00001950: 681c 6803 681d 4e68 1e4e 7562 6168 1f7d  h.h.h.Nh.Nubah.}
-00001960: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-00001970: 5d94 6829 5d94 7568 2b68 2d68 1d68 2c68  ].h)].uh+h-h.h,h
-00001980: 1e4b 2f68 1b6a 3b02 0000 681c 6803 7562  .K/h.j;...h.h.ub
-00001990: 682e 2981 947d 9428 6805 8cb0 546f 2064  h.)..}.(h...To d
-000019a0: 6f20 7468 6174 2073 696d 706c 7920 636c  o that simply cl
-000019b0: 6f6e 6520 6f72 2064 6f77 6e6c 6f61 6420  one or download 
-000019c0: 604e 6573 7465 7227 7320 4769 7448 7562  `Nester's GitHub
-000019d0: 2072 6570 6f73 6974 6f72 7920 3c68 7474   repository <htt
-000019e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000019f0: 4279 7465 4f74 7465 722f 6e65 7374 6572  ByteOtter/nester
-00001a00: 3e60 5f20 656e 7465 7220 7468 6520 606e  >`_ enter the `n
-00001a10: 6573 7465 722f 6020 6469 7265 6374 6f72  ester/` director
-00001a20: 7920 616e 6420 7275 6e20 6070 6970 2069  y and run `pip i
-00001a30: 6e73 7461 6c6c 202e 6020 746f 2069 6e73  nstall .` to ins
-00001a40: 7461 6c6c 204e 6573 7465 722e 9468 075d  tall Nester..h.]
-00001a50: 9428 6816 8c24 546f 2064 6f20 7468 6174  .(h..$To do that
-00001a60: 2073 696d 706c 7920 636c 6f6e 6520 6f72   simply clone or
-00001a70: 2064 6f77 6e6c 6f61 6420 9485 9481 947d   download .....}
-00001a80: 9428 681b 6a5a 0200 0068 1c68 0368 1d4e  .(h.jZ...h.h.h.N
-00001a90: 681e 4e75 6268 ee29 8194 7d94 2868 058c  h.Nubh.)..}.(h..
-00001aa0: 4360 4e65 7374 6572 2773 2047 6974 4875  C`Nester's GitHu
-00001ab0: 6220 7265 706f 7369 746f 7279 203c 6874  b repository <ht
-00001ac0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001ad0: 2f42 7974 654f 7474 6572 2f6e 6573 7465  /ByteOtter/neste
-00001ae0: 723e 605f 9468 075d 9468 168c 1c4e 6573  r>`_.h.].h...Nes
-00001af0: 7465 72e2 8099 7320 4769 7448 7562 2072  ter...s GitHub r
-00001b00: 6570 6f73 6974 6f72 7994 8594 8194 7d94  epository.....}.
-00001b10: 2868 1b6a 6202 0000 681c 6803 681d 4e68  (h.jb...h.h.h.Nh
-00001b20: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
-00001b30: 5d94 6825 5d94 6827 5d94 6829 5d94 8c04  ].h%].h'].h)]...
-00001b40: 6e61 6d65 948c 1a4e 6573 7465 7227 7320  name...Nester's 
-00001b50: 4769 7448 7562 2072 6570 6f73 6974 6f72  GitHub repositor
-00001b60: 7994 68ff 8c23 6874 7470 733a 2f2f 6769  y.h..#https://gi
-00001b70: 7468 7562 2e63 6f6d 2f42 7974 654f 7474  thub.com/ByteOtt
-00001b80: 6572 2f6e 6573 7465 7294 7568 2b68 ed68  er/nester.uh+h.h
-00001b90: 1b6a 5a02 0000 7562 6a02 0100 0029 8194  .jZ...ubj....)..
-00001ba0: 7d94 2868 058c 2620 3c68 7474 7073 3a2f  }.(h..& <https:/
-00001bb0: 2f67 6974 6875 622e 636f 6d2f 4279 7465  /github.com/Byte
-00001bc0: 4f74 7465 722f 6e65 7374 6572 3e94 6807  Otter/nester>.h.
-00001bd0: 5d94 681f 7d94 2868 215d 948c 1a6e 6573  ].h.}.(h!]...nes
-00001be0: 7465 722d 732d 6769 7468 7562 2d72 6570  ter-s-github-rep
-00001bf0: 6f73 6974 6f72 7994 6168 235d 9468 255d  ository.ah#].h%]
-00001c00: 948c 1a6e 6573 7465 7227 7320 6769 7468  ...nester's gith
-00001c10: 7562 2072 6570 6f73 6974 6f72 7994 6168  ub repository.ah
-00001c20: 275d 9468 295d 948c 0672 6566 7572 6994  '].h)]...refuri.
-00001c30: 6a72 0200 0075 682b 6a01 0100 006a 1001  jr...uh+j....j..
-00001c40: 0000 4b01 681b 6a5a 0200 0075 6268 168c  ..K.h.jZ...ubh..
-00001c50: 0b20 656e 7465 7220 7468 6520 9485 9481  . enter the ....
-00001c60: 947d 9428 681b 6a5a 0200 0068 1c68 0368  .}.(h.jZ...h.h.h
-00001c70: 1d4e 681e 4e75 6268 5029 8194 7d94 2868  .Nh.NubhP)..}.(h
-00001c80: 058c 0960 6e65 7374 6572 2f60 9468 075d  ...`nester/`.h.]
-00001c90: 9468 168c 076e 6573 7465 722f 9485 9481  .h...nester/....
-00001ca0: 947d 9428 681b 6a84 0200 0068 1c68 0368  .}.(h.j....h.h.h
-00001cb0: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
-00001cc0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-00001cd0: 9475 682b 684f 681b 6a5a 0200 0075 6268  .uh+hOh.jZ...ubh
-00001ce0: 168c 1320 6469 7265 6374 6f72 7920 616e  ... directory an
-00001cf0: 6420 7275 6e20 9485 9481 947d 9428 681b  d run .....}.(h.
-00001d00: 6a5a 0200 0068 1c68 0368 1d4e 681e 4e75  jZ...h.h.h.Nh.Nu
-00001d10: 6268 5029 8194 7d94 2868 058c 0f60 7069  bhP)..}.(h...`pi
-00001d20: 7020 696e 7374 616c 6c20 2e60 9468 075d  p install .`.h.]
-00001d30: 9468 168c 0d70 6970 2069 6e73 7461 6c6c  .h...pip install
-00001d40: 202e 9485 9481 947d 9428 681b 6a96 0200   ......}.(h.j...
-00001d50: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
-00001d60: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-00001d70: 275d 9468 295d 9475 682b 684f 681b 6a5a  '].h)].uh+hOh.jZ
-00001d80: 0200 0075 6268 168c 1320 746f 2069 6e73  ...ubh... to ins
-00001d90: 7461 6c6c 204e 6573 7465 722e 9485 9481  tall Nester.....
-00001da0: 947d 9428 681b 6a5a 0200 0068 1c68 0368  .}.(h.jZ...h.h.h
-00001db0: 1d4e 681e 4e75 6265 681f 7d94 2868 215d  .Nh.Nubeh.}.(h!]
-00001dc0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-00001dd0: 9475 682b 682d 681d 682c 681e 4b32 681b  .uh+h-h.h,h.K2h.
-00001de0: 6a3b 0200 0068 1c68 0375 6268 2e29 8194  j;...h.h.ubh.)..
-00001df0: 7d94 2868 058c 0544 6f6e 6521 9468 075d  }.(h...Done!.h.]
-00001e00: 9468 168c 0544 6f6e 6521 9485 9481 947d  .h...Done!.....}
-00001e10: 9428 681b 6aae 0200 0068 1c68 0368 1d4e  .(h.j....h.h.h.N
-00001e20: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
-00001e30: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
-00001e40: 682b 682d 681d 682c 681e 4b34 681b 6a3b  h+h-h.h,h.K4h.j;
-00001e50: 0200 0068 1c68 0375 6268 2e29 8194 7d94  ...h.h.ubh.)..}.
-00001e60: 2868 058c 4157 6520 686f 7065 2079 6f75  (h..AWe hope you
-00001e70: 2068 6176 6520 6173 206d 7563 6820 6675   have as much fu
-00001e80: 6e20 7573 696e 6720 4e65 7374 6572 2061  n using Nester a
-00001e90: 7320 7765 2068 6176 6520 6275 696c 6469  s we have buildi
-00001ea0: 6e67 2069 7421 9468 075d 9468 168c 4157  ng it!.h.].h..AW
-00001eb0: 6520 686f 7065 2079 6f75 2068 6176 6520  e hope you have 
-00001ec0: 6173 206d 7563 6820 6675 6e20 7573 696e  as much fun usin
-00001ed0: 6720 4e65 7374 6572 2061 7320 7765 2068  g Nester as we h
-00001ee0: 6176 6520 6275 696c 6469 6e67 2069 7421  ave building it!
-00001ef0: 9485 9481 947d 9428 681b 6abc 0200 0068  .....}.(h.j....h
-00001f00: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
-00001f10: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
-00001f20: 9468 295d 9475 682b 682d 681d 682c 681e  .h)].uh+h-h.h,h.
-00001f30: 4b36 681b 6a3b 0200 0068 1c68 0375 6265  K6h.j;...h.h.ube
-00001f40: 681f 7d94 2868 215d 948c 1462 7569 6c64  h.}.(h!]...build
-00001f50: 696e 672d 6672 6f6d 2d73 6f75 7263 6594  ing-from-source.
-00001f60: 6168 235d 9468 255d 948c 1462 7569 6c64  ah#].h%]...build
-00001f70: 696e 6720 6672 6f6d 2073 6f75 7263 6594  ing from source.
-00001f80: 6168 275d 9468 295d 9475 682b 680a 681b  ah'].h)].uh+h.h.
-00001f90: 680c 681c 6803 681d 682c 681e 4b2d 7562  h.h.h.h.h,h.K-ub
-00001fa0: 6568 1f7d 9428 6821 5d94 8c11 696e 7374  eh.}.(h!]...inst
-00001fb0: 616c 6c69 6e67 2d6e 6573 7465 7294 6168  alling-nester.ah
-00001fc0: 235d 9468 255d 948c 1169 6e73 7461 6c6c  #].h%]...install
-00001fd0: 696e 6720 6e65 7374 6572 9461 6827 5d94  ing nester.ah'].
-00001fe0: 6829 5d94 7568 2b68 0a68 1b68 0368 1c68  h)].uh+h.h.h.h.h
-00001ff0: 0368 1d68 2c68 1e4b 0275 6261 681f 7d94  .h.h,h.K.ubah.}.
-00002000: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
-00002010: 9468 295d 948c 0673 6f75 7263 6594 682c  .h)]...source.h,
-00002020: 7568 2b68 018c 0e63 7572 7265 6e74 5f73  uh+h...current_s
-00002030: 6f75 7263 6594 4e8c 0c63 7572 7265 6e74  ource.N..current
-00002040: 5f6c 696e 6594 4e8c 0873 6574 7469 6e67  _line.N..setting
-00002050: 7394 8c11 646f 6375 7469 6c73 2e66 726f  s...docutils.fro
-00002060: 6e74 656e 6494 8c06 5661 6c75 6573 9493  ntend...Values..
-00002070: 9429 8194 7d94 2868 0f4e 8c09 6765 6e65  .)..}.(h.N..gene
-00002080: 7261 746f 7294 4e8c 0964 6174 6573 7461  rator.N..datesta
-00002090: 6d70 944e 8c0b 736f 7572 6365 5f6c 696e  mp.N..source_lin
-000020a0: 6b94 4e8c 0a73 6f75 7263 655f 7572 6c94  k.N..source_url.
-000020b0: 4e8c 0d74 6f63 5f62 6163 6b6c 696e 6b73  N..toc_backlinks
-000020c0: 948c 0565 6e74 7279 948c 1266 6f6f 746e  ...entry...footn
-000020d0: 6f74 655f 6261 636b 6c69 6e6b 7394 4b01  ote_backlinks.K.
-000020e0: 8c0d 7365 6374 6e75 6d5f 7866 6f72 6d94  ..sectnum_xform.
-000020f0: 4b01 8c0e 7374 7269 705f 636f 6d6d 656e  K...strip_commen
-00002100: 7473 944e 8c1b 7374 7269 705f 656c 656d  ts.N..strip_elem
-00002110: 656e 7473 5f77 6974 685f 636c 6173 7365  ents_with_classe
-00002120: 7394 4e8c 0d73 7472 6970 5f63 6c61 7373  s.N..strip_class
-00002130: 6573 944e 8c0c 7265 706f 7274 5f6c 6576  es.N..report_lev
-00002140: 656c 944b 028c 0a68 616c 745f 6c65 7665  el.K...halt_leve
-00002150: 6c94 4b05 8c11 6578 6974 5f73 7461 7475  l.K...exit_statu
-00002160: 735f 6c65 7665 6c94 4b05 8c05 6465 6275  s_level.K...debu
-00002170: 6794 4e8c 0e77 6172 6e69 6e67 5f73 7472  g.N..warning_str
-00002180: 6561 6d94 4e8c 0974 7261 6365 6261 636b  eam.N..traceback
-00002190: 9488 8c0e 696e 7075 745f 656e 636f 6469  ....input_encodi
-000021a0: 6e67 948c 0975 7466 2d38 2d73 6967 948c  ng...utf-8-sig..
-000021b0: 1c69 6e70 7574 5f65 6e63 6f64 696e 675f  .input_encoding_
-000021c0: 6572 726f 725f 6861 6e64 6c65 7294 8c06  error_handler...
-000021d0: 7374 7269 6374 948c 0f6f 7574 7075 745f  strict...output_
-000021e0: 656e 636f 6469 6e67 948c 0575 7466 2d38  encoding...utf-8
-000021f0: 948c 1d6f 7574 7075 745f 656e 636f 6469  ...output_encodi
-00002200: 6e67 5f65 7272 6f72 5f68 616e 646c 6572  ng_error_handler
-00002210: 946a fd02 0000 8c0e 6572 726f 725f 656e  .j......error_en
-00002220: 636f 6469 6e67 948c 0575 7466 2d38 948c  coding...utf-8..
-00002230: 1c65 7272 6f72 5f65 6e63 6f64 696e 675f  .error_encoding_
-00002240: 6572 726f 725f 6861 6e64 6c65 7294 8c10  error_handler...
-00002250: 6261 636b 736c 6173 6872 6570 6c61 6365  backslashreplace
-00002260: 948c 0d6c 616e 6775 6167 655f 636f 6465  ...language_code
-00002270: 948c 0265 6e94 8c13 7265 636f 7264 5f64  ...en...record_d
-00002280: 6570 656e 6465 6e63 6965 7394 4e8c 0663  ependencies.N..c
-00002290: 6f6e 6669 6794 4e8c 0969 645f 7072 6566  onfig.N..id_pref
-000022a0: 6978 9468 068c 0e61 7574 6f5f 6964 5f70  ix.h...auto_id_p
-000022b0: 7265 6669 7894 8c02 6964 948c 0d64 756d  refix...id...dum
-000022c0: 705f 7365 7474 696e 6773 944e 8c0e 6475  p_settings.N..du
-000022d0: 6d70 5f69 6e74 6572 6e61 6c73 944e 8c0f  mp_internals.N..
-000022e0: 6475 6d70 5f74 7261 6e73 666f 726d 7394  dump_transforms.
-000022f0: 4e8c 0f64 756d 705f 7073 6575 646f 5f78  N..dump_pseudo_x
-00002300: 6d6c 944e 8c10 6578 706f 7365 5f69 6e74  ml.N..expose_int
-00002310: 6572 6e61 6c73 944e 8c0e 7374 7269 6374  ernals.N..strict
-00002320: 5f76 6973 6974 6f72 944e 8c0f 5f64 6973  _visitor.N.._dis
-00002330: 6162 6c65 5f63 6f6e 6669 6794 4e8c 075f  able_config.N.._
-00002340: 736f 7572 6365 9468 2c8c 0c5f 6465 7374  source.h,.._dest
-00002350: 696e 6174 696f 6e94 4e8c 0d5f 636f 6e66  ination.N.._conf
-00002360: 6967 5f66 696c 6573 945d 948c 1666 696c  ig_files.]...fil
-00002370: 655f 696e 7365 7274 696f 6e5f 656e 6162  e_insertion_enab
-00002380: 6c65 6494 888c 0b72 6177 5f65 6e61 626c  led....raw_enabl
-00002390: 6564 944b 018c 116c 696e 655f 6c65 6e67  ed.K...line_leng
-000023a0: 7468 5f6c 696d 6974 944d 1027 8c0e 7065  th_limit.M.'..pe
-000023b0: 705f 7265 6665 7265 6e63 6573 944e 8c0c  p_references.N..
-000023c0: 7065 705f 6261 7365 5f75 726c 948c 1868  pep_base_url...h
-000023d0: 7474 7073 3a2f 2f70 6570 732e 7079 7468  ttps://peps.pyth
-000023e0: 6f6e 2e6f 7267 2f94 8c15 7065 705f 6669  on.org/...pep_fi
-000023f0: 6c65 5f75 726c 5f74 656d 706c 6174 6594  le_url_template.
-00002400: 8c08 7065 702d 2530 3464 948c 0e72 6663  ..pep-%04d...rfc
-00002410: 5f72 6566 6572 656e 6365 7394 4e8c 0c72  _references.N..r
-00002420: 6663 5f62 6173 655f 7572 6c94 8c26 6874  fc_base_url..&ht
-00002430: 7470 733a 2f2f 6461 7461 7472 6163 6b65  tps://datatracke
-00002440: 722e 6965 7466 2e6f 7267 2f64 6f63 2f68  r.ietf.org/doc/h
-00002450: 746d 6c2f 948c 0974 6162 5f77 6964 7468  tml/...tab_width
-00002460: 944b 088c 1d74 7269 6d5f 666f 6f74 6e6f  .K...trim_footno
-00002470: 7465 5f72 6566 6572 656e 6365 5f73 7061  te_reference_spa
-00002480: 6365 9489 8c10 7379 6e74 6178 5f68 6967  ce....syntax_hig
-00002490: 686c 6967 6874 948c 046c 6f6e 6794 8c0c  hlight...long...
-000024a0: 736d 6172 745f 7175 6f74 6573 9488 8c13  smart_quotes....
-000024b0: 736d 6172 7471 756f 7465 735f 6c6f 6361  smartquotes_loca
-000024c0: 6c65 7394 5d94 8c1d 6368 6172 6163 7465  les.]...characte
-000024d0: 725f 6c65 7665 6c5f 696e 6c69 6e65 5f6d  r_level_inline_m
-000024e0: 6172 6b75 7094 898c 0e64 6f63 7469 746c  arkup....doctitl
-000024f0: 655f 7866 6f72 6d94 898c 0d64 6f63 696e  e_xform....docin
-00002500: 666f 5f78 666f 726d 944b 018c 1273 6563  fo_xform.K...sec
-00002510: 7473 7562 7469 746c 655f 7866 6f72 6d94  tsubtitle_xform.
-00002520: 898c 0d69 6d61 6765 5f6c 6f61 6469 6e67  ...image_loading
-00002530: 948c 046c 696e 6b94 8c10 656d 6265 645f  ...link...embed_
-00002540: 7374 796c 6573 6865 6574 9489 8c15 636c  stylesheet....cl
-00002550: 6f61 6b5f 656d 6169 6c5f 6164 6472 6573  oak_email_addres
-00002560: 7365 7394 888c 1173 6563 7469 6f6e 5f73  ses....section_s
-00002570: 656c 665f 6c69 6e6b 9489 8c03 656e 7694  elf_link....env.
-00002580: 4e75 628c 0872 6570 6f72 7465 7294 4e8c  Nub..reporter.N.
-00002590: 1069 6e64 6972 6563 745f 7461 7267 6574  .indirect_target
-000025a0: 7394 5d94 8c11 7375 6273 7469 7475 7469  s.]...substituti
-000025b0: 6f6e 5f64 6566 7394 7d94 8c12 7375 6273  on_defs.}...subs
-000025c0: 7469 7475 7469 6f6e 5f6e 616d 6573 947d  titution_names.}
-000025d0: 948c 0872 6566 6e61 6d65 7394 7d94 8c06  ...refnames.}...
-000025e0: 7265 6669 6473 947d 948c 076e 616d 6569  refids.}...namei
-000025f0: 6473 947d 9428 6ad7 0200 006a d402 0000  ds.}.(j....j....
-00002600: 6a61 0100 006a 5e01 0000 6a0c 0100 006a  ja...j^...j....j
-00002610: 0901 0000 6a38 0200 006a 3502 0000 6acf  ....j8...j5...j.
-00002620: 0200 006a cc02 0000 6a7c 0200 006a 7902  ...j....j|...jy.
-00002630: 0000 758c 096e 616d 6574 7970 6573 947d  ..u..nametypes.}
-00002640: 9428 6ad7 0200 0089 6a61 0100 0089 6a0c  .(j.....ja....j.
-00002650: 0100 0088 6a38 0200 0089 6acf 0200 0089  ....j8....j.....
-00002660: 6a7c 0200 0088 7568 217d 9428 6ad4 0200  j|....uh!}.(j...
-00002670: 0068 0c6a 5e01 0000 68b8 6a09 0100 006a  .h.j^...h.j....j
-00002680: 0301 0000 6a35 0200 006a 6401 0000 6acc  ....j5...jd...j.
-00002690: 0200 006a 3b02 0000 6a79 0200 006a 7302  ...j;...jy...js.
-000026a0: 0000 758c 0d66 6f6f 746e 6f74 655f 7265  ..u..footnote_re
-000026b0: 6673 947d 948c 0d63 6974 6174 696f 6e5f  fs.}...citation_
-000026c0: 7265 6673 947d 948c 0d61 7574 6f66 6f6f  refs.}...autofoo
-000026d0: 746e 6f74 6573 945d 948c 1161 7574 6f66  tnotes.]...autof
-000026e0: 6f6f 746e 6f74 655f 7265 6673 945d 948c  ootnote_refs.]..
-000026f0: 1073 796d 626f 6c5f 666f 6f74 6e6f 7465  .symbol_footnote
-00002700: 7394 5d94 8c14 7379 6d62 6f6c 5f66 6f6f  s.]...symbol_foo
-00002710: 746e 6f74 655f 7265 6673 945d 948c 0966  tnote_refs.]...f
-00002720: 6f6f 746e 6f74 6573 945d 948c 0963 6974  ootnotes.]...cit
-00002730: 6174 696f 6e73 945d 948c 1261 7574 6f66  ations.]...autof
-00002740: 6f6f 746e 6f74 655f 7374 6172 7494 4b01  ootnote_start.K.
-00002750: 8c15 7379 6d62 6f6c 5f66 6f6f 746e 6f74  ..symbol_footnot
-00002760: 655f 7374 6172 7494 4b00 8c0a 6964 5f63  e_start.K...id_c
-00002770: 6f75 6e74 6572 948c 0b63 6f6c 6c65 6374  ounter...collect
-00002780: 696f 6e73 948c 0743 6f75 6e74 6572 9493  ions...Counter..
-00002790: 947d 9485 9452 948c 0e70 6172 7365 5f6d  .}...R...parse_m
-000027a0: 6573 7361 6765 7394 5d94 8c12 7472 616e  essages.]...tran
-000027b0: 7366 6f72 6d5f 6d65 7373 6167 6573 945d  sform_messages.]
-000027c0: 948c 0b74 7261 6e73 666f 726d 6572 944e  ...transformer.N
-000027d0: 8c0b 696e 636c 7564 655f 6c6f 6794 5d94  ..include_log.].
-000027e0: 8c0a 6465 636f 7261 7469 6f6e 944e 681c  ..decoration.Nh.
-000027f0: 6803 7562 2e                             h.ub.
+00001470: 8194 7d94 2868 058c 2257 6520 6361 6e20  ..}.(h.."We can 
+00001480: 6e6f 7720 6f66 6665 7220 6120 602e 7270  now offer a `.rp
+00001490: 6d60 2070 6163 6b61 6765 2194 6807 5d94  m` package!.h.].
+000014a0: 2868 168c 1357 6520 6361 6e20 6e6f 7720  (h...We can now 
+000014b0: 6f66 6665 7220 6120 9485 9481 947d 9428  offer a .....}.(
+000014c0: 681b 6af9 0100 0068 1c68 0368 1d4e 681e  h.j....h.h.h.Nh.
+000014d0: 4e75 6268 5029 8194 7d94 2868 058c 0660  NubhP)..}.(h...`
+000014e0: 2e72 706d 6094 6807 5d94 6816 8c04 2e72  .rpm`.h.].h....r
+000014f0: 706d 9485 9481 947d 9428 681b 6a01 0200  pm.....}.(h.j...
+00001500: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
+00001510: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+00001520: 275d 9468 295d 9475 682b 684f 681b 6af9  '].h)].uh+hOh.j.
+00001530: 0100 0075 6268 168c 0920 7061 636b 6167  ...ubh... packag
+00001540: 6521 9485 9481 947d 9428 681b 6af9 0100  e!.....}.(h.j...
+00001550: 0068 1c68 0368 1d4e 681e 4e75 6265 681f  .h.h.h.Nh.Nubeh.
+00001560: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+00001570: 275d 9468 295d 9475 682b 682d 681d 682c  '].h)].uh+h-h.h,
+00001580: 681e 4b22 681b 6a64 0100 0068 1c68 0375  h.K"h.jd...h.h.u
+00001590: 6268 2e29 8194 7d94 2868 058c 2a54 6f20  bh.)..}.(h..*To 
+000015a0: 646f 2073 6f20 666f 6c6c 6f77 2074 6865  do so follow the
+000015b0: 7365 2073 7465 7073 2028 6f6e 206f 7065  se steps (on ope
+000015c0: 6e53 5553 4529 3a94 6807 5d94 6816 8c2a  nSUSE):.h.].h..*
+000015d0: 546f 2064 6f20 736f 2066 6f6c 6c6f 7720  To do so follow 
+000015e0: 7468 6573 6520 7374 6570 7320 286f 6e20  these steps (on 
+000015f0: 6f70 656e 5355 5345 293a 9485 9481 947d  openSUSE):.....}
+00001600: 9428 681b 6a19 0200 0068 1c68 0368 1d4e  .(h.j....h.h.h.N
+00001610: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
+00001620: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
+00001630: 682b 682d 681d 682c 681e 4b24 681b 6a64  h+h-h.h,h.K$h.jd
+00001640: 0100 0068 1c68 0375 6268 098c 0f65 6e75  ...h.h.ubh...enu
+00001650: 6d65 7261 7465 645f 6c69 7374 9493 9429  merated_list...)
+00001660: 8194 7d94 2868 0568 0668 075d 9468 4329  ..}.(h.h.h.].hC)
+00001670: 8194 7d94 2868 058c 1341 6464 2074 6865  ..}.(h...Add the
+00001680: 2072 6570 6f73 6974 6f72 790a 9468 075d   repository..h.]
+00001690: 9468 2e29 8194 7d94 2868 058c 1241 6464  .h.)..}.(h...Add
+000016a0: 2074 6865 2072 6570 6f73 6974 6f72 7994   the repository.
+000016b0: 6807 5d94 6816 8c12 4164 6420 7468 6520  h.].h...Add the 
+000016c0: 7265 706f 7369 746f 7279 9485 9481 947d  repository.....}
+000016d0: 9428 681b 6a30 0200 0068 1c68 0368 1d4e  .(h.j0...h.h.h.N
+000016e0: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
+000016f0: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
+00001700: 682b 682d 681d 682c 681e 4b26 681b 6a2c  h+h-h.h,h.K&h.j,
+00001710: 0200 0075 6261 681f 7d94 2868 215d 9468  ...ubah.}.(h!].h
+00001720: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
+00001730: 682b 6842 681b 6a29 0200 0068 1c68 0368  h+hBh.j)...h.h.h
+00001740: 1d68 2c68 1e4e 7562 6168 1f7d 9428 6821  .h,h.Nubah.}.(h!
+00001750: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+00001760: 5d94 8c08 656e 756d 7479 7065 948c 0661  ]...enumtype...a
+00001770: 7261 6269 6394 8c06 7072 6566 6978 9468  rabic...prefix.h
+00001780: 068c 0673 7566 6669 7894 8c01 2e94 7568  ...suffix.....uh
+00001790: 2b6a 2702 0000 681b 6a64 0100 0068 1c68  +j'...h.jd...h.h
+000017a0: 0368 1d68 2c68 1e4b 2675 626a 2a01 0000  .h.h,h.K&ubj*...
+000017b0: 2981 947d 9428 6805 8c72 7375 646f 207a  )..}.(h..rsudo z
+000017c0: 7970 7065 7220 6164 6472 6570 6f20 6068  ypper addrepo `h
+000017d0: 7474 7073 3a2f 2f64 6f77 6e6c 6f61 642e  ttps://download.
+000017e0: 6f70 656e 7375 7365 2e6f 7267 2f72 6570  opensuse.org/rep
+000017f0: 6f73 6974 6f72 6965 732f 686f 6d65 3a6b  ositories/home:k
+00001800: 6f64 796d 6f2f 6f70 656e 5355 5345 5f54  odymo/openSUSE_T
+00001810: 756d 626c 6577 6565 642f 686f 6d65 3a6b  umbleweed/home:k
+00001820: 6f64 796d 6f2e 7265 706f 605f 9468 075d  odymo.repo`_.h.]
+00001830: 9468 168c 7273 7564 6f20 7a79 7070 6572  .h..rsudo zypper
+00001840: 2061 6464 7265 706f 2060 6874 7470 733a   addrepo `https:
+00001850: 2f2f 646f 776e 6c6f 6164 2e6f 7065 6e73  //download.opens
+00001860: 7573 652e 6f72 672f 7265 706f 7369 746f  use.org/reposito
+00001870: 7269 6573 2f68 6f6d 653a 6b6f 6479 6d6f  ries/home:kodymo
+00001880: 2f6f 7065 6e53 5553 455f 5475 6d62 6c65  /openSUSE_Tumble
+00001890: 7765 6564 2f68 6f6d 653a 6b6f 6479 6d6f  weed/home:kodymo
+000018a0: 2e72 6570 6f60 5f94 8594 8194 7d94 681b  .repo`_.....}.h.
+000018b0: 6a4f 0200 0073 6261 681f 7d94 2868 215d  jO...sbah.}.(h!]
+000018c0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+000018d0: 946a 3901 0000 6a3a 0100 006a 3b01 0000  .j9...j:...j;...
+000018e0: 896a 3c01 0000 8c05 7368 656c 6c94 6a3e  .j<.....shell.j>
+000018f0: 0100 007d 9475 682b 6a29 0100 0068 1d68  ...}.uh+j)...h.h
+00001900: 2c68 1e4b 2868 1b6a 6401 0000 681c 6803  ,h.K(h.jd...h.h.
+00001910: 7562 6a02 0100 0029 8194 7d94 2868 058c  ubj....)..}.(h..
+00001920: 622e 2e20 5f60 6874 7470 733a 2f2f 646f  b.. _`https://do
+00001930: 776e 6c6f 6164 2e6f 7065 6e73 7573 652e  wnload.opensuse.
+00001940: 6f72 672f 7265 706f 7369 746f 7269 6573  org/repositories
+00001950: 2f68 6f6d 653a 6b6f 6479 6d6f 2f6f 7065  /home:kodymo/ope
+00001960: 6e53 5553 455f 5475 6d62 6c65 7765 6564  nSUSE_Tumbleweed
+00001970: 2f68 6f6d 653a 6b6f 6479 6d6f 2e72 6570  /home:kodymo.rep
+00001980: 6f60 3a94 6807 5d94 681f 7d94 2868 215d  o`:.h.].h.}.(h!]
+00001990: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+000019a0: 948c 0572 6566 6964 948c 5968 7474 7073  ...refid..Yhttps
+000019b0: 2d64 6f77 6e6c 6f61 642d 6f70 656e 7375  -download-opensu
+000019c0: 7365 2d6f 7267 2d72 6570 6f73 6974 6f72  se-org-repositor
+000019d0: 6965 732d 686f 6d65 2d6b 6f64 796d 6f2d  ies-home-kodymo-
+000019e0: 6f70 656e 7375 7365 2d74 756d 626c 6577  opensuse-tumblew
+000019f0: 6565 642d 686f 6d65 2d6b 6f64 796d 6f2d  eed-home-kodymo-
+00001a00: 7265 706f 9475 682b 6a01 0100 0068 1e4b  repo.uh+j....h.K
+00001a10: 2c68 1b6a 6401 0000 681c 6803 681d 682c  ,h.jd...h.h.h.h,
+00001a20: 7562 6a28 0200 0029 8194 7d94 2868 0568  ubj(...)..}.(h.h
+00001a30: 0668 075d 9468 4329 8194 7d94 2868 058c  .h.].hC)..}.(h..
+00001a40: 1a52 6566 7265 7368 2079 6f75 7220 7265  .Refresh your re
+00001a50: 706f 7369 746f 7269 6573 0a94 6807 5d94  positories..h.].
+00001a60: 682e 2981 947d 9428 6805 8c19 5265 6672  h.)..}.(h...Refr
+00001a70: 6573 6820 796f 7572 2072 6570 6f73 6974  esh your reposit
+00001a80: 6f72 6965 7394 6807 5d94 6816 8c19 5265  ories.h.].h...Re
+00001a90: 6672 6573 6820 796f 7572 2072 6570 6f73  fresh your repos
+00001aa0: 6974 6f72 6965 7394 8594 8194 7d94 2868  itories.....}.(h
+00001ab0: 1b6a 7202 0000 681c 6803 681d 4e68 1e4e  .jr...h.h.h.Nh.N
+00001ac0: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+00001ad0: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
+00001ae0: 2d68 1d68 2c68 1e4b 2f68 1b6a 6e02 0000  -h.h,h.K/h.jn...
+00001af0: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+00001b00: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
+00001b10: 4268 1b6a 6b02 0000 681c 6803 681d 682c  Bh.jk...h.h.h.h,
+00001b20: 681e 4e75 6261 681f 7d94 2868 215d 946a  h.Nubah.}.(h!].j
+00001b30: 6a02 0000 6168 235d 9468 255d 948c 5b68  j...ah#].h%]..[h
+00001b40: 7474 7073 3a2f 2f64 6f77 6e6c 6f61 642e  ttps://download.
+00001b50: 6f70 656e 7375 7365 2e6f 7267 2f72 6570  opensuse.org/rep
+00001b60: 6f73 6974 6f72 6965 732f 686f 6d65 3a6b  ositories/home:k
+00001b70: 6f64 796d 6f2f 6f70 656e 7375 7365 5f74  odymo/opensuse_t
+00001b80: 756d 626c 6577 6565 642f 686f 6d65 3a6b  umbleweed/home:k
+00001b90: 6f64 796d 6f2e 7265 706f 9461 6827 5d94  odymo.repo.ah'].
+00001ba0: 6829 5d94 6a4a 0200 006a 4b02 0000 6a4c  h)].jJ...jK...jL
+00001bb0: 0200 0068 066a 4d02 0000 6a4e 0200 008c  ...h.jM...jN....
+00001bc0: 0573 7461 7274 944b 0275 682b 6a27 0200  .start.K.uh+j'..
+00001bd0: 0068 1b6a 6401 0000 681c 6803 681d 682c  .h.jd...h.h.h.h,
+00001be0: 681e 4b2f 8c19 6578 7065 6374 5f72 6566  h.K/..expect_ref
+00001bf0: 6572 656e 6365 645f 6279 5f6e 616d 6594  erenced_by_name.
+00001c00: 7d94 6a8a 0200 006a 5f02 0000 738c 1765  }.j....j_...s..e
+00001c10: 7870 6563 745f 7265 6665 7265 6e63 6564  xpect_referenced
+00001c20: 5f62 795f 6964 947d 946a 6a02 0000 6a5f  _by_id.}.jj...j_
+00001c30: 0200 0073 7562 6a2a 0100 0029 8194 7d94  ...subj*...)..}.
+00001c40: 2868 058c 0f73 7564 6f20 7a79 7070 6572  (h...sudo zypper
+00001c50: 2072 6566 9468 075d 9468 168c 0f73 7564   ref.h.].h...sud
+00001c60: 6f20 7a79 7070 6572 2072 6566 9485 9481  o zypper ref....
+00001c70: 947d 9468 1b6a 9202 0000 7362 6168 1f7d  .}.h.j....sbah.}
+00001c80: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
+00001c90: 5d94 6829 5d94 6a39 0100 006a 3a01 0000  ].h)].j9...j:...
+00001ca0: 6a3b 0100 0089 6a3c 0100 008c 0573 6865  j;....j<.....she
+00001cb0: 6c6c 946a 3e01 0000 7d94 7568 2b6a 2901  ll.j>...}.uh+j).
+00001cc0: 0000 681d 682c 681e 4b31 681b 6a64 0100  ..h.h,h.K1h.jd..
+00001cd0: 0068 1c68 0375 626a 2802 0000 2981 947d  .h.h.ubj(...)..}
+00001ce0: 9428 6805 6806 6807 5d94 6843 2981 947d  .(h.h.h.].hC)..}
+00001cf0: 9428 6805 8c0f 496e 7374 616c 6c20 4e65  .(h...Install Ne
+00001d00: 7374 6572 0a94 6807 5d94 682e 2981 947d  ster..h.].h.)..}
+00001d10: 9428 6805 8c0e 496e 7374 616c 6c20 4e65  .(h...Install Ne
+00001d20: 7374 6572 9468 075d 9468 168c 0e49 6e73  ster.h.].h...Ins
+00001d30: 7461 6c6c 204e 6573 7465 7294 8594 8194  tall Nester.....
+00001d40: 7d94 2868 1b6a a902 0000 681c 6803 681d  }.(h.j....h.h.h.
+00001d50: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
+00001d60: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+00001d70: 7568 2b68 2d68 1d68 2c68 1e4b 3668 1b6a  uh+h-h.h,h.K6h.j
+00001d80: a502 0000 7562 6168 1f7d 9428 6821 5d94  ....ubah.}.(h!].
+00001d90: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+00001da0: 7568 2b68 4268 1b6a a202 0000 681c 6803  uh+hBh.j....h.h.
+00001db0: 681d 682c 681e 4e75 6261 681f 7d94 2868  h.h,h.Nubah.}.(h
+00001dc0: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+00001dd0: 295d 946a 4a02 0000 6a4b 0200 006a 4c02  )].jJ...jK...jL.
+00001de0: 0000 6806 6a4d 0200 006a 4e02 0000 6a8d  ..h.jM...jN...j.
+00001df0: 0200 004b 0375 682b 6a27 0200 0068 1b6a  ...K.uh+j'...h.j
+00001e00: 6401 0000 681c 6803 681d 682c 681e 4b36  d...h.h.h.h,h.K6
+00001e10: 7562 6a2a 0100 0029 8194 7d94 2868 058c  ubj*...)..}.(h..
+00001e20: 2273 7564 6f20 7a79 7070 6572 2069 6e73  "sudo zypper ins
+00001e30: 7461 6c6c 2070 7974 686f 6e33 2d6e 6573  tall python3-nes
+00001e40: 7465 7294 6807 5d94 6816 8c22 7375 646f  ter.h.].h.."sudo
+00001e50: 207a 7970 7065 7220 696e 7374 616c 6c20   zypper install 
+00001e60: 7079 7468 6f6e 332d 6e65 7374 6572 9485  python3-nester..
+00001e70: 9481 947d 9468 1b6a c302 0000 7362 6168  ...}.h.j....sbah
+00001e80: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+00001e90: 6827 5d94 6829 5d94 6a39 0100 006a 3a01  h'].h)].j9...j:.
+00001ea0: 0000 6a3b 0100 0089 6a3c 0100 008c 0573  ..j;....j<.....s
+00001eb0: 6865 6c6c 946a 3e01 0000 7d94 7568 2b6a  hell.j>...}.uh+j
+00001ec0: 2901 0000 681d 682c 681e 4b38 681b 6a64  )...h.h,h.K8h.jd
+00001ed0: 0100 0068 1c68 0375 6268 2e29 8194 7d94  ...h.h.ubh.)..}.
+00001ee0: 2868 058c ac4e 6f74 653a 2054 6865 2072  (h...Note: The r
+00001ef0: 6570 6f73 6974 6f72 7920 636f 6e74 6169  epository contai
+00001f00: 6e73 2074 6872 6565 2062 7569 6c64 7320  ns three builds 
+00001f10: 666f 7220 6e65 7374 6572 2066 6f72 2050  for nester for P
+00001f20: 7974 686f 6e20 332e 392c 2033 2e31 3020  ython 3.9, 3.10 
+00001f30: 616e 6420 332e 3131 2e20 607a 7970 7065  and 3.11. `zyppe
+00001f40: 7260 2077 696c 6c20 6175 746f 6d61 7469  r` will automati
+00001f50: 6361 6c6c 7920 6465 6369 6465 2077 6869  cally decide whi
+00001f60: 6368 2076 6572 7369 6f6e 2074 6f20 7573  ch version to us
+00001f70: 6520 7768 656e 2072 756e 6e69 6e67 2074  e when running t
+00001f80: 6865 2063 6f6d 6d61 6e64 2061 626f 7665  he command above
+00001f90: 2e94 6807 5d94 2868 168c 554e 6f74 653a  ..h.].(h..UNote:
+00001fa0: 2054 6865 2072 6570 6f73 6974 6f72 7920   The repository 
+00001fb0: 636f 6e74 6169 6e73 2074 6872 6565 2062  contains three b
+00001fc0: 7569 6c64 7320 666f 7220 6e65 7374 6572  uilds for nester
+00001fd0: 2066 6f72 2050 7974 686f 6e20 332e 392c   for Python 3.9,
+00001fe0: 2033 2e31 3020 616e 6420 332e 3131 2e20   3.10 and 3.11. 
+00001ff0: 9485 9481 947d 9428 681b 6ad3 0200 0068  .....}.(h.j....h
+00002000: 1c68 0368 1d4e 681e 4e75 6268 5029 8194  .h.h.Nh.NubhP)..
+00002010: 7d94 2868 058c 0860 7a79 7070 6572 6094  }.(h...`zypper`.
+00002020: 6807 5d94 6816 8c06 7a79 7070 6572 9485  h.].h...zypper..
+00002030: 9481 947d 9428 681b 6adb 0200 0068 1c68  ...}.(h.j....h.h
+00002040: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
+00002050: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+00002060: 295d 9475 682b 684f 681b 6ad3 0200 0075  )].uh+hOh.j....u
+00002070: 6268 168c 4f20 7769 6c6c 2061 7574 6f6d  bh..O will autom
+00002080: 6174 6963 616c 6c79 2064 6563 6964 6520  atically decide 
+00002090: 7768 6963 6820 7665 7273 696f 6e20 746f  which version to
+000020a0: 2075 7365 2077 6865 6e20 7275 6e6e 696e   use when runnin
+000020b0: 6720 7468 6520 636f 6d6d 616e 6420 6162  g the command ab
+000020c0: 6f76 652e 9485 9481 947d 9428 681b 6ad3  ove......}.(h.j.
+000020d0: 0200 0068 1c68 0368 1d4e 681e 4e75 6265  ...h.h.h.Nh.Nube
+000020e0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+000020f0: 9468 275d 9468 295d 9475 682b 682d 681d  .h'].h)].uh+h-h.
+00002100: 682c 681e 4b3d 681b 6a64 0100 0068 1c68  h,h.K=h.jd...h.h
+00002110: 0375 6268 2e29 8194 7d94 2868 058c 8a59  .ubh.)..}.(h...Y
+00002120: 6f75 2063 616e 2076 6973 6974 2074 6865  ou can visit the
+00002130: 2072 6570 6f73 6974 6f72 7920 6f6e 2074   repository on t
+00002140: 6865 205b 7061 636b 6167 6520 6d61 696e  he [package main
+00002150: 7461 696e 6572 2773 204f 4253 2061 6363  tainer's OBS acc
+00002160: 6f75 6e74 5d28 6874 7470 733a 2f2f 6275  ount](https://bu
+00002170: 696c 642e 6f70 656e 7375 7365 2e6f 7267  ild.opensuse.org
+00002180: 2f70 6163 6b61 6765 2f73 686f 772f 686f  /package/show/ho
+00002190: 6d65 3a6b 6f64 796d 6f2f 7079 7468 6f6e  me:kodymo/python
+000021a0: 2d6e 6573 7465 7229 2e94 6807 5d94 2868  -nester)..h.].(h
+000021b0: 168c 4959 6f75 2063 616e 2076 6973 6974  ..IYou can visit
+000021c0: 2074 6865 2072 6570 6f73 6974 6f72 7920   the repository 
+000021d0: 6f6e 2074 6865 205b 7061 636b 6167 6520  on the [package 
+000021e0: 6d61 696e 7461 696e 6572 e280 9973 204f  maintainer...s O
+000021f0: 4253 2061 6363 6f75 6e74 5d28 9485 9481  BS account](....
+00002200: 947d 9428 681b 6af3 0200 0068 1c68 0368  .}.(h.j....h.h.h
+00002210: 1d4e 681e 4e75 6268 ee29 8194 7d94 2868  .Nh.Nubh.)..}.(h
+00002220: 058c 4168 7474 7073 3a2f 2f62 7569 6c64  ..Ahttps://build
+00002230: 2e6f 7065 6e73 7573 652e 6f72 672f 7061  .opensuse.org/pa
+00002240: 636b 6167 652f 7368 6f77 2f68 6f6d 653a  ckage/show/home:
+00002250: 6b6f 6479 6d6f 2f70 7974 686f 6e2d 6e65  kodymo/python-ne
+00002260: 7374 6572 9468 075d 9468 168c 4168 7474  ster.h.].h..Ahtt
+00002270: 7073 3a2f 2f62 7569 6c64 2e6f 7065 6e73  ps://build.opens
+00002280: 7573 652e 6f72 672f 7061 636b 6167 652f  use.org/package/
+00002290: 7368 6f77 2f68 6f6d 653a 6b6f 6479 6d6f  show/home:kodymo
+000022a0: 2f70 7974 686f 6e2d 6e65 7374 6572 9485  /python-nester..
+000022b0: 9481 947d 9428 681b 6afb 0200 0068 1c68  ...}.(h.j....h.h
+000022c0: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
+000022d0: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+000022e0: 295d 948c 0672 6566 7572 6994 6afd 0200  )]...refuri.j...
+000022f0: 0075 682b 68ed 681b 6af3 0200 0075 6268  .uh+h.h.j....ubh
+00002300: 168c 0229 2e94 8594 8194 7d94 2868 1b6a  ...)......}.(h.j
+00002310: f302 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
+00002320: 6568 1f7d 9428 6821 5d94 6823 5d94 6825  eh.}.(h!].h#].h%
+00002330: 5d94 6827 5d94 6829 5d94 7568 2b68 2d68  ].h'].h)].uh+h-h
+00002340: 1d68 2c68 1e4b 3f68 1b6a 6401 0000 681c  .h,h.K?h.jd...h.
+00002350: 6803 7562 6568 1f7d 9428 6821 5d94 8c1b  h.ubeh.}.(h!]...
+00002360: 696e 7374 616c 6c61 7469 6f6e 2d61 732d  installation-as-
+00002370: 7270 6d2d 7061 636b 6167 6594 6168 235d  rpm-package.ah#]
+00002380: 9468 255d 948c 1b69 6e73 7461 6c6c 6174  .h%]...installat
+00002390: 696f 6e20 6173 2072 706d 2070 6163 6b61  ion as rpm packa
+000023a0: 6765 9461 6827 5d94 6829 5d94 7568 2b68  ge.ah'].h)].uh+h
+000023b0: 0a68 1b68 0c68 1c68 0368 1d68 2c68 1e4b  .h.h.h.h.h.h,h.K
+000023c0: 1975 6268 0b29 8194 7d94 2868 0568 0668  .ubh.)..}.(h.h.h
+000023d0: 075d 9428 6810 2981 947d 9428 6805 8c14  .].(h.)..}.(h...
+000023e0: 4275 696c 6469 6e67 2066 726f 6d20 736f  Building from so
+000023f0: 7572 6365 9468 075d 9468 168c 1442 7569  urce.h.].h...Bui
+00002400: 6c64 696e 6720 6672 6f6d 2073 6f75 7263  lding from sourc
+00002410: 6594 8594 8194 7d94 2868 1b6a 1f03 0000  e.....}.(h.j....
+00002420: 681c 6803 681d 4e68 1e4e 7562 6168 1f7d  h.h.h.Nh.Nubah.}
+00002430: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
+00002440: 5d94 6829 5d94 7568 2b68 0f68 1b6a 1c03  ].h)].uh+h.h.j..
+00002450: 0000 681c 6803 681d 682c 681e 4b42 7562  ..h.h.h.h,h.KBub
+00002460: 682e 2981 947d 9428 6805 8c6e 536f 6d65  h.)..}.(h..nSome
+00002470: 7469 6d65 7320 696e 7374 616c 6c69 6e67  times installing
+00002480: 2066 726f 6d20 7368 6164 7920 736f 7572   from shady sour
+00002490: 6365 7320 6d61 7920 6e6f 7420 6265 2079  ces may not be y
+000024a0: 6f75 7220 7468 696e 672e 2046 6561 7220  our thing. Fear 
+000024b0: 6e6f 7567 6874 210a 596f 7520 6361 6e20  nought!.You can 
+000024c0: 616c 736f 2062 7569 6c64 2069 7420 6672  also build it fr
+000024d0: 6f6d 2073 6f75 7263 652e 9468 075d 9468  om source..h.].h
+000024e0: 168c 6e53 6f6d 6574 696d 6573 2069 6e73  ..nSometimes ins
+000024f0: 7461 6c6c 696e 6720 6672 6f6d 2073 6861  talling from sha
+00002500: 6479 2073 6f75 7263 6573 206d 6179 206e  dy sources may n
+00002510: 6f74 2062 6520 796f 7572 2074 6869 6e67  ot be your thing
+00002520: 2e20 4665 6172 206e 6f75 6768 7421 0a59  . Fear nought!.Y
+00002530: 6f75 2063 616e 2061 6c73 6f20 6275 696c  ou can also buil
+00002540: 6420 6974 2066 726f 6d20 736f 7572 6365  d it from source
+00002550: 2e94 8594 8194 7d94 2868 1b6a 2d03 0000  ......}.(h.j-...
+00002560: 681c 6803 681d 4e68 1e4e 7562 6168 1f7d  h.h.h.Nh.Nubah.}
+00002570: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
+00002580: 5d94 6829 5d94 7568 2b68 2d68 1d68 2c68  ].h)].uh+h-h.h,h
+00002590: 1e4b 4468 1b6a 1c03 0000 681c 6803 7562  .KDh.j....h.h.ub
+000025a0: 682e 2981 947d 9428 6805 8cb0 546f 2064  h.)..}.(h...To d
+000025b0: 6f20 7468 6174 2073 696d 706c 7920 636c  o that simply cl
+000025c0: 6f6e 6520 6f72 2064 6f77 6e6c 6f61 6420  one or download 
+000025d0: 604e 6573 7465 7227 7320 4769 7448 7562  `Nester's GitHub
+000025e0: 2072 6570 6f73 6974 6f72 7920 3c68 7474   repository <htt
+000025f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00002600: 4279 7465 4f74 7465 722f 6e65 7374 6572  ByteOtter/nester
+00002610: 3e60 5f20 656e 7465 7220 7468 6520 606e  >`_ enter the `n
+00002620: 6573 7465 722f 6020 6469 7265 6374 6f72  ester/` director
+00002630: 7920 616e 6420 7275 6e20 6070 6970 2069  y and run `pip i
+00002640: 6e73 7461 6c6c 202e 6020 746f 2069 6e73  nstall .` to ins
+00002650: 7461 6c6c 204e 6573 7465 722e 9468 075d  tall Nester..h.]
+00002660: 9428 6816 8c24 546f 2064 6f20 7468 6174  .(h..$To do that
+00002670: 2073 696d 706c 7920 636c 6f6e 6520 6f72   simply clone or
+00002680: 2064 6f77 6e6c 6f61 6420 9485 9481 947d   download .....}
+00002690: 9428 681b 6a3b 0300 0068 1c68 0368 1d4e  .(h.j;...h.h.h.N
+000026a0: 681e 4e75 6268 ee29 8194 7d94 2868 058c  h.Nubh.)..}.(h..
+000026b0: 4360 4e65 7374 6572 2773 2047 6974 4875  C`Nester's GitHu
+000026c0: 6220 7265 706f 7369 746f 7279 203c 6874  b repository <ht
+000026d0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000026e0: 2f42 7974 654f 7474 6572 2f6e 6573 7465  /ByteOtter/neste
+000026f0: 723e 605f 9468 075d 9468 168c 1c4e 6573  r>`_.h.].h...Nes
+00002700: 7465 72e2 8099 7320 4769 7448 7562 2072  ter...s GitHub r
+00002710: 6570 6f73 6974 6f72 7994 8594 8194 7d94  epository.....}.
+00002720: 2868 1b6a 4303 0000 681c 6803 681d 4e68  (h.jC...h.h.h.Nh
+00002730: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
+00002740: 5d94 6825 5d94 6827 5d94 6829 5d94 8c04  ].h%].h'].h)]...
+00002750: 6e61 6d65 948c 1a4e 6573 7465 7227 7320  name...Nester's 
+00002760: 4769 7448 7562 2072 6570 6f73 6974 6f72  GitHub repositor
+00002770: 7994 68ff 8c23 6874 7470 733a 2f2f 6769  y.h..#https://gi
+00002780: 7468 7562 2e63 6f6d 2f42 7974 654f 7474  thub.com/ByteOtt
+00002790: 6572 2f6e 6573 7465 7294 7568 2b68 ed68  er/nester.uh+h.h
+000027a0: 1b6a 3b03 0000 7562 6a02 0100 0029 8194  .j;...ubj....)..
+000027b0: 7d94 2868 058c 2620 3c68 7474 7073 3a2f  }.(h..& <https:/
+000027c0: 2f67 6974 6875 622e 636f 6d2f 4279 7465  /github.com/Byte
+000027d0: 4f74 7465 722f 6e65 7374 6572 3e94 6807  Otter/nester>.h.
+000027e0: 5d94 681f 7d94 2868 215d 948c 1a6e 6573  ].h.}.(h!]...nes
+000027f0: 7465 722d 732d 6769 7468 7562 2d72 6570  ter-s-github-rep
+00002800: 6f73 6974 6f72 7994 6168 235d 9468 255d  ository.ah#].h%]
+00002810: 948c 1a6e 6573 7465 7227 7320 6769 7468  ...nester's gith
+00002820: 7562 2072 6570 6f73 6974 6f72 7994 6168  ub repository.ah
+00002830: 275d 9468 295d 948c 0672 6566 7572 6994  '].h)]...refuri.
+00002840: 6a53 0300 0075 682b 6a01 0100 006a 1001  jS...uh+j....j..
+00002850: 0000 4b01 681b 6a3b 0300 0075 6268 168c  ..K.h.j;...ubh..
+00002860: 0b20 656e 7465 7220 7468 6520 9485 9481  . enter the ....
+00002870: 947d 9428 681b 6a3b 0300 0068 1c68 0368  .}.(h.j;...h.h.h
+00002880: 1d4e 681e 4e75 6268 5029 8194 7d94 2868  .Nh.NubhP)..}.(h
+00002890: 058c 0960 6e65 7374 6572 2f60 9468 075d  ...`nester/`.h.]
+000028a0: 9468 168c 076e 6573 7465 722f 9485 9481  .h...nester/....
+000028b0: 947d 9428 681b 6a65 0300 0068 1c68 0368  .}.(h.je...h.h.h
+000028c0: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
+000028d0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+000028e0: 9475 682b 684f 681b 6a3b 0300 0075 6268  .uh+hOh.j;...ubh
+000028f0: 168c 1320 6469 7265 6374 6f72 7920 616e  ... directory an
+00002900: 6420 7275 6e20 9485 9481 947d 9428 681b  d run .....}.(h.
+00002910: 6a3b 0300 0068 1c68 0368 1d4e 681e 4e75  j;...h.h.h.Nh.Nu
+00002920: 6268 5029 8194 7d94 2868 058c 0f60 7069  bhP)..}.(h...`pi
+00002930: 7020 696e 7374 616c 6c20 2e60 9468 075d  p install .`.h.]
+00002940: 9468 168c 0d70 6970 2069 6e73 7461 6c6c  .h...pip install
+00002950: 202e 9485 9481 947d 9428 681b 6a77 0300   ......}.(h.jw..
+00002960: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
+00002970: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+00002980: 275d 9468 295d 9475 682b 684f 681b 6a3b  '].h)].uh+hOh.j;
+00002990: 0300 0075 6268 168c 1320 746f 2069 6e73  ...ubh... to ins
+000029a0: 7461 6c6c 204e 6573 7465 722e 9485 9481  tall Nester.....
+000029b0: 947d 9428 681b 6a3b 0300 0068 1c68 0368  .}.(h.j;...h.h.h
+000029c0: 1d4e 681e 4e75 6265 681f 7d94 2868 215d  .Nh.Nubeh.}.(h!]
+000029d0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+000029e0: 9475 682b 682d 681d 682c 681e 4b47 681b  .uh+h-h.h,h.KGh.
+000029f0: 6a1c 0300 0068 1c68 0375 6268 2e29 8194  j....h.h.ubh.)..
+00002a00: 7d94 2868 058c 0544 6f6e 6521 9468 075d  }.(h...Done!.h.]
+00002a10: 9468 168c 0544 6f6e 6521 9485 9481 947d  .h...Done!.....}
+00002a20: 9428 681b 6a8f 0300 0068 1c68 0368 1d4e  .(h.j....h.h.h.N
+00002a30: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
+00002a40: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
+00002a50: 682b 682d 681d 682c 681e 4b49 681b 6a1c  h+h-h.h,h.KIh.j.
+00002a60: 0300 0068 1c68 0375 6268 2e29 8194 7d94  ...h.h.ubh.)..}.
+00002a70: 2868 058c 4157 6520 686f 7065 2079 6f75  (h..AWe hope you
+00002a80: 2068 6176 6520 6173 206d 7563 6820 6675   have as much fu
+00002a90: 6e20 7573 696e 6720 4e65 7374 6572 2061  n using Nester a
+00002aa0: 7320 7765 2068 6176 6520 6275 696c 6469  s we have buildi
+00002ab0: 6e67 2069 7421 9468 075d 9468 168c 4157  ng it!.h.].h..AW
+00002ac0: 6520 686f 7065 2079 6f75 2068 6176 6520  e hope you have 
+00002ad0: 6173 206d 7563 6820 6675 6e20 7573 696e  as much fun usin
+00002ae0: 6720 4e65 7374 6572 2061 7320 7765 2068  g Nester as we h
+00002af0: 6176 6520 6275 696c 6469 6e67 2069 7421  ave building it!
+00002b00: 9485 9481 947d 9428 681b 6a9d 0300 0068  .....}.(h.j....h
+00002b10: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
+00002b20: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+00002b30: 9468 295d 9475 682b 682d 681d 682c 681e  .h)].uh+h-h.h,h.
+00002b40: 4b4b 681b 6a1c 0300 0068 1c68 0375 6265  KKh.j....h.h.ube
+00002b50: 681f 7d94 2868 215d 948c 1462 7569 6c64  h.}.(h!]...build
+00002b60: 696e 672d 6672 6f6d 2d73 6f75 7263 6594  ing-from-source.
+00002b70: 6168 235d 9468 255d 948c 1462 7569 6c64  ah#].h%]...build
+00002b80: 696e 6720 6672 6f6d 2073 6f75 7263 6594  ing from source.
+00002b90: 6168 275d 9468 295d 9475 682b 680a 681b  ah'].h)].uh+h.h.
+00002ba0: 680c 681c 6803 681d 682c 681e 4b42 7562  h.h.h.h.h,h.KBub
+00002bb0: 6568 1f7d 9428 6821 5d94 8c11 696e 7374  eh.}.(h!]...inst
+00002bc0: 616c 6c69 6e67 2d6e 6573 7465 7294 6168  alling-nester.ah
+00002bd0: 235d 9468 255d 948c 1169 6e73 7461 6c6c  #].h%]...install
+00002be0: 696e 6720 6e65 7374 6572 9461 6827 5d94  ing nester.ah'].
+00002bf0: 6829 5d94 7568 2b68 0a68 1b68 0368 1c68  h)].uh+h.h.h.h.h
+00002c00: 0368 1d68 2c68 1e4b 0275 6261 681f 7d94  .h.h,h.K.ubah.}.
+00002c10: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+00002c20: 9468 295d 948c 0673 6f75 7263 6594 682c  .h)]...source.h,
+00002c30: 7568 2b68 018c 0e63 7572 7265 6e74 5f73  uh+h...current_s
+00002c40: 6f75 7263 6594 4e8c 0c63 7572 7265 6e74  ource.N..current
+00002c50: 5f6c 696e 6594 4e8c 0873 6574 7469 6e67  _line.N..setting
+00002c60: 7394 8c11 646f 6375 7469 6c73 2e66 726f  s...docutils.fro
+00002c70: 6e74 656e 6494 8c06 5661 6c75 6573 9493  ntend...Values..
+00002c80: 9429 8194 7d94 2868 0f4e 8c09 6765 6e65  .)..}.(h.N..gene
+00002c90: 7261 746f 7294 4e8c 0964 6174 6573 7461  rator.N..datesta
+00002ca0: 6d70 944e 8c0b 736f 7572 6365 5f6c 696e  mp.N..source_lin
+00002cb0: 6b94 4e8c 0a73 6f75 7263 655f 7572 6c94  k.N..source_url.
+00002cc0: 4e8c 0d74 6f63 5f62 6163 6b6c 696e 6b73  N..toc_backlinks
+00002cd0: 948c 0565 6e74 7279 948c 1266 6f6f 746e  ...entry...footn
+00002ce0: 6f74 655f 6261 636b 6c69 6e6b 7394 4b01  ote_backlinks.K.
+00002cf0: 8c0d 7365 6374 6e75 6d5f 7866 6f72 6d94  ..sectnum_xform.
+00002d00: 4b01 8c0e 7374 7269 705f 636f 6d6d 656e  K...strip_commen
+00002d10: 7473 944e 8c1b 7374 7269 705f 656c 656d  ts.N..strip_elem
+00002d20: 656e 7473 5f77 6974 685f 636c 6173 7365  ents_with_classe
+00002d30: 7394 4e8c 0d73 7472 6970 5f63 6c61 7373  s.N..strip_class
+00002d40: 6573 944e 8c0c 7265 706f 7274 5f6c 6576  es.N..report_lev
+00002d50: 656c 944b 028c 0a68 616c 745f 6c65 7665  el.K...halt_leve
+00002d60: 6c94 4b05 8c11 6578 6974 5f73 7461 7475  l.K...exit_statu
+00002d70: 735f 6c65 7665 6c94 4b05 8c05 6465 6275  s_level.K...debu
+00002d80: 6794 4e8c 0e77 6172 6e69 6e67 5f73 7472  g.N..warning_str
+00002d90: 6561 6d94 4e8c 0974 7261 6365 6261 636b  eam.N..traceback
+00002da0: 9488 8c0e 696e 7075 745f 656e 636f 6469  ....input_encodi
+00002db0: 6e67 948c 0975 7466 2d38 2d73 6967 948c  ng...utf-8-sig..
+00002dc0: 1c69 6e70 7574 5f65 6e63 6f64 696e 675f  .input_encoding_
+00002dd0: 6572 726f 725f 6861 6e64 6c65 7294 8c06  error_handler...
+00002de0: 7374 7269 6374 948c 0f6f 7574 7075 745f  strict...output_
+00002df0: 656e 636f 6469 6e67 948c 0575 7466 2d38  encoding...utf-8
+00002e00: 948c 1d6f 7574 7075 745f 656e 636f 6469  ...output_encodi
+00002e10: 6e67 5f65 7272 6f72 5f68 616e 646c 6572  ng_error_handler
+00002e20: 946a de03 0000 8c0e 6572 726f 725f 656e  .j......error_en
+00002e30: 636f 6469 6e67 948c 0575 7466 2d38 948c  coding...utf-8..
+00002e40: 1c65 7272 6f72 5f65 6e63 6f64 696e 675f  .error_encoding_
+00002e50: 6572 726f 725f 6861 6e64 6c65 7294 8c10  error_handler...
+00002e60: 6261 636b 736c 6173 6872 6570 6c61 6365  backslashreplace
+00002e70: 948c 0d6c 616e 6775 6167 655f 636f 6465  ...language_code
+00002e80: 948c 0265 6e94 8c13 7265 636f 7264 5f64  ...en...record_d
+00002e90: 6570 656e 6465 6e63 6965 7394 4e8c 0663  ependencies.N..c
+00002ea0: 6f6e 6669 6794 4e8c 0969 645f 7072 6566  onfig.N..id_pref
+00002eb0: 6978 9468 068c 0e61 7574 6f5f 6964 5f70  ix.h...auto_id_p
+00002ec0: 7265 6669 7894 8c02 6964 948c 0d64 756d  refix...id...dum
+00002ed0: 705f 7365 7474 696e 6773 944e 8c0e 6475  p_settings.N..du
+00002ee0: 6d70 5f69 6e74 6572 6e61 6c73 944e 8c0f  mp_internals.N..
+00002ef0: 6475 6d70 5f74 7261 6e73 666f 726d 7394  dump_transforms.
+00002f00: 4e8c 0f64 756d 705f 7073 6575 646f 5f78  N..dump_pseudo_x
+00002f10: 6d6c 944e 8c10 6578 706f 7365 5f69 6e74  ml.N..expose_int
+00002f20: 6572 6e61 6c73 944e 8c0e 7374 7269 6374  ernals.N..strict
+00002f30: 5f76 6973 6974 6f72 944e 8c0f 5f64 6973  _visitor.N.._dis
+00002f40: 6162 6c65 5f63 6f6e 6669 6794 4e8c 075f  able_config.N.._
+00002f50: 736f 7572 6365 9468 2c8c 0c5f 6465 7374  source.h,.._dest
+00002f60: 696e 6174 696f 6e94 4e8c 0d5f 636f 6e66  ination.N.._conf
+00002f70: 6967 5f66 696c 6573 945d 948c 1666 696c  ig_files.]...fil
+00002f80: 655f 696e 7365 7274 696f 6e5f 656e 6162  e_insertion_enab
+00002f90: 6c65 6494 888c 0b72 6177 5f65 6e61 626c  led....raw_enabl
+00002fa0: 6564 944b 018c 116c 696e 655f 6c65 6e67  ed.K...line_leng
+00002fb0: 7468 5f6c 696d 6974 944d 1027 8c0e 7065  th_limit.M.'..pe
+00002fc0: 705f 7265 6665 7265 6e63 6573 944e 8c0c  p_references.N..
+00002fd0: 7065 705f 6261 7365 5f75 726c 948c 1868  pep_base_url...h
+00002fe0: 7474 7073 3a2f 2f70 6570 732e 7079 7468  ttps://peps.pyth
+00002ff0: 6f6e 2e6f 7267 2f94 8c15 7065 705f 6669  on.org/...pep_fi
+00003000: 6c65 5f75 726c 5f74 656d 706c 6174 6594  le_url_template.
+00003010: 8c08 7065 702d 2530 3464 948c 0e72 6663  ..pep-%04d...rfc
+00003020: 5f72 6566 6572 656e 6365 7394 4e8c 0c72  _references.N..r
+00003030: 6663 5f62 6173 655f 7572 6c94 8c26 6874  fc_base_url..&ht
+00003040: 7470 733a 2f2f 6461 7461 7472 6163 6b65  tps://datatracke
+00003050: 722e 6965 7466 2e6f 7267 2f64 6f63 2f68  r.ietf.org/doc/h
+00003060: 746d 6c2f 948c 0974 6162 5f77 6964 7468  tml/...tab_width
+00003070: 944b 088c 1d74 7269 6d5f 666f 6f74 6e6f  .K...trim_footno
+00003080: 7465 5f72 6566 6572 656e 6365 5f73 7061  te_reference_spa
+00003090: 6365 9489 8c10 7379 6e74 6178 5f68 6967  ce....syntax_hig
+000030a0: 686c 6967 6874 948c 046c 6f6e 6794 8c0c  hlight...long...
+000030b0: 736d 6172 745f 7175 6f74 6573 9488 8c13  smart_quotes....
+000030c0: 736d 6172 7471 756f 7465 735f 6c6f 6361  smartquotes_loca
+000030d0: 6c65 7394 5d94 8c1d 6368 6172 6163 7465  les.]...characte
+000030e0: 725f 6c65 7665 6c5f 696e 6c69 6e65 5f6d  r_level_inline_m
+000030f0: 6172 6b75 7094 898c 0e64 6f63 7469 746c  arkup....doctitl
+00003100: 655f 7866 6f72 6d94 898c 0d64 6f63 696e  e_xform....docin
+00003110: 666f 5f78 666f 726d 944b 018c 1273 6563  fo_xform.K...sec
+00003120: 7473 7562 7469 746c 655f 7866 6f72 6d94  tsubtitle_xform.
+00003130: 898c 0d69 6d61 6765 5f6c 6f61 6469 6e67  ...image_loading
+00003140: 948c 046c 696e 6b94 8c10 656d 6265 645f  ...link...embed_
+00003150: 7374 796c 6573 6865 6574 9489 8c15 636c  stylesheet....cl
+00003160: 6f61 6b5f 656d 6169 6c5f 6164 6472 6573  oak_email_addres
+00003170: 7365 7394 888c 1173 6563 7469 6f6e 5f73  ses....section_s
+00003180: 656c 665f 6c69 6e6b 9489 8c03 656e 7694  elf_link....env.
+00003190: 4e75 628c 0872 6570 6f72 7465 7294 4e8c  Nub..reporter.N.
+000031a0: 1069 6e64 6972 6563 745f 7461 7267 6574  .indirect_target
+000031b0: 7394 5d94 8c11 7375 6273 7469 7475 7469  s.]...substituti
+000031c0: 6f6e 5f64 6566 7394 7d94 8c12 7375 6273  on_defs.}...subs
+000031d0: 7469 7475 7469 6f6e 5f6e 616d 6573 947d  titution_names.}
+000031e0: 948c 0872 6566 6e61 6d65 7394 7d94 8c06  ...refnames.}...
+000031f0: 7265 6669 6473 947d 946a 6a02 0000 5d94  refids.}.jj...].
+00003200: 6a5f 0200 0061 738c 076e 616d 6569 6473  j_...as..nameids
+00003210: 947d 9428 6ab8 0300 006a b503 0000 6a61  .}.(j....j....ja
+00003220: 0100 006a 5e01 0000 6a0c 0100 006a 0901  ...j^...j....j..
+00003230: 0000 6a19 0300 006a 1603 0000 6a8a 0200  ..j....j....j...
+00003240: 006a 6a02 0000 6ab0 0300 006a ad03 0000  .jj...j....j....
+00003250: 6a5d 0300 006a 5a03 0000 758c 096e 616d  j]...jZ...u..nam
+00003260: 6574 7970 6573 947d 9428 6ab8 0300 0089  etypes.}.(j.....
+00003270: 6a61 0100 0089 6a0c 0100 0088 6a19 0300  ja....j.....j...
+00003280: 0089 6a8a 0200 0088 6ab0 0300 0089 6a5d  ..j.....j.....j]
+00003290: 0300 0088 7568 217d 9428 6ab5 0300 0068  ....uh!}.(j....h
+000032a0: 0c6a 5e01 0000 68b8 6a09 0100 006a 0301  .j^...h.j....j..
+000032b0: 0000 6a16 0300 006a 6401 0000 6a6a 0200  ..j....jd...jj..
+000032c0: 006a 6b02 0000 6aad 0300 006a 1c03 0000  .jk...j....j....
+000032d0: 6a5a 0300 006a 5403 0000 758c 0d66 6f6f  jZ...jT...u..foo
+000032e0: 746e 6f74 655f 7265 6673 947d 948c 0d63  tnote_refs.}...c
+000032f0: 6974 6174 696f 6e5f 7265 6673 947d 948c  itation_refs.}..
+00003300: 0d61 7574 6f66 6f6f 746e 6f74 6573 945d  .autofootnotes.]
+00003310: 948c 1161 7574 6f66 6f6f 746e 6f74 655f  ...autofootnote_
+00003320: 7265 6673 945d 948c 1073 796d 626f 6c5f  refs.]...symbol_
+00003330: 666f 6f74 6e6f 7465 7394 5d94 8c14 7379  footnotes.]...sy
+00003340: 6d62 6f6c 5f66 6f6f 746e 6f74 655f 7265  mbol_footnote_re
+00003350: 6673 945d 948c 0966 6f6f 746e 6f74 6573  fs.]...footnotes
+00003360: 945d 948c 0963 6974 6174 696f 6e73 945d  .]...citations.]
+00003370: 948c 1261 7574 6f66 6f6f 746e 6f74 655f  ...autofootnote_
+00003380: 7374 6172 7494 4b01 8c15 7379 6d62 6f6c  start.K...symbol
+00003390: 5f66 6f6f 746e 6f74 655f 7374 6172 7494  _footnote_start.
+000033a0: 4b00 8c0a 6964 5f63 6f75 6e74 6572 948c  K...id_counter..
+000033b0: 0b63 6f6c 6c65 6374 696f 6e73 948c 0743  .collections...C
+000033c0: 6f75 6e74 6572 9493 947d 9485 9452 948c  ounter...}...R..
+000033d0: 0e70 6172 7365 5f6d 6573 7361 6765 7394  .parse_messages.
+000033e0: 5d94 2868 098c 0e73 7973 7465 6d5f 6d65  ].(h...system_me
+000033f0: 7373 6167 6594 9394 2981 947d 9428 6805  ssage...)..}.(h.
+00003400: 6806 6807 5d94 682e 2981 947d 9428 6805  h.h.].h.)..}.(h.
+00003410: 8c3a 456e 756d 6572 6174 6564 206c 6973  .:Enumerated lis
+00003420: 7420 7374 6172 7420 7661 6c75 6520 6e6f  t start value no
+00003430: 7420 6f72 6469 6e61 6c2d 313a 2022 3222  t ordinal-1: "2"
+00003440: 2028 6f72 6469 6e61 6c20 3229 9468 075d   (ordinal 2).h.]
+00003450: 9468 168c 3e45 6e75 6d65 7261 7465 6420  .h..>Enumerated 
+00003460: 6c69 7374 2073 7461 7274 2076 616c 7565  list start value
+00003470: 206e 6f74 206f 7264 696e 616c 2d31 3a20   not ordinal-1: 
+00003480: e280 9c32 e280 9d20 286f 7264 696e 616c  ...2... (ordinal
+00003490: 2032 2994 8594 8194 7d94 2868 1b6a 4504   2).....}.(h.jE.
+000034a0: 0000 681c 6803 681d 4e68 1e4e 7562 6168  ..h.h.h.Nh.Nubah
+000034b0: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+000034c0: 6827 5d94 6829 5d94 7568 2b68 2d68 1b6a  h'].h)].uh+h-h.j
+000034d0: 4204 0000 7562 6168 1f7d 9428 6821 5d94  B...ubah.}.(h!].
+000034e0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+000034f0: 8c05 6c65 7665 6c94 4b01 8c04 7479 7065  ..level.K...type
+00003500: 948c 0449 4e46 4f94 8c06 736f 7572 6365  ...INFO...source
+00003510: 9468 2c8c 046c 696e 6594 4b02 7568 2b6a  .h,..line.K.uh+j
+00003520: 4004 0000 681b 6a64 0100 0068 1c68 0368  @...h.jd...h.h.h
+00003530: 1d68 2c68 1e4b 2f75 626a 4104 0000 2981  .h,h.K/ubjA...).
+00003540: 947d 9428 6805 6806 6807 5d94 682e 2981  .}.(h.h.h.].h.).
+00003550: 947d 9428 6805 8c3a 456e 756d 6572 6174  .}.(h..:Enumerat
+00003560: 6564 206c 6973 7420 7374 6172 7420 7661  ed list start va
+00003570: 6c75 6520 6e6f 7420 6f72 6469 6e61 6c2d  lue not ordinal-
+00003580: 313a 2022 3322 2028 6f72 6469 6e61 6c20  1: "3" (ordinal 
+00003590: 3329 9468 075d 9468 168c 3e45 6e75 6d65  3).h.].h..>Enume
+000035a0: 7261 7465 6420 6c69 7374 2073 7461 7274  rated list start
+000035b0: 2076 616c 7565 206e 6f74 206f 7264 696e   value not ordin
+000035c0: 616c 2d31 3a20 e280 9c33 e280 9d20 286f  al-1: ...3... (o
+000035d0: 7264 696e 616c 2033 2994 8594 8194 7d94  rdinal 3).....}.
+000035e0: 2868 1b6a 6104 0000 681c 6803 681d 4e68  (h.ja...h.h.h.Nh
+000035f0: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
+00003600: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
+00003610: 2b68 2d68 1b6a 5e04 0000 7562 6168 1f7d  +h-h.j^...ubah.}
+00003620: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
+00003630: 5d94 6829 5d94 8c05 6c65 7665 6c94 4b01  ].h)]...level.K.
+00003640: 8c04 7479 7065 946a 5b04 0000 8c06 736f  ..type.j[.....so
+00003650: 7572 6365 9468 2c8c 046c 696e 6594 4b02  urce.h,..line.K.
+00003660: 7568 2b6a 4004 0000 681b 6a64 0100 0068  uh+j@...h.jd...h
+00003670: 1c68 0368 1d68 2c68 1e4b 3675 6265 8c12  .h.h.h,h.K6ube..
+00003680: 7472 616e 7366 6f72 6d5f 6d65 7373 6167  transform_messag
+00003690: 6573 945d 946a 4104 0000 2981 947d 9428  es.].jA...)..}.(
+000036a0: 6805 6806 6807 5d94 682e 2981 947d 9428  h.h.h.].h.)..}.(
+000036b0: 6805 6806 6807 5d94 6816 8c7f 4879 7065  h.h.h.].h...Hype
+000036c0: 726c 696e 6b20 7461 7267 6574 2022 6874  rlink target "ht
+000036d0: 7470 732d 646f 776e 6c6f 6164 2d6f 7065  tps-download-ope
+000036e0: 6e73 7573 652d 6f72 672d 7265 706f 7369  nsuse-org-reposi
+000036f0: 746f 7269 6573 2d68 6f6d 652d 6b6f 6479  tories-home-kody
+00003700: 6d6f 2d6f 7065 6e73 7573 652d 7475 6d62  mo-opensuse-tumb
+00003710: 6c65 7765 6564 2d68 6f6d 652d 6b6f 6479  leweed-home-kody
+00003720: 6d6f 2d72 6570 6f22 2069 7320 6e6f 7420  mo-repo" is not 
+00003730: 7265 6665 7265 6e63 6564 2e94 8594 8194  referenced......
+00003740: 7d94 681b 6a7e 0400 0073 6261 681f 7d94  }.h.j~...sbah.}.
+00003750: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+00003760: 9468 295d 9475 682b 682d 681b 6a7b 0400  .h)].uh+h-h.j{..
+00003770: 0075 6261 681f 7d94 2868 215d 9468 235d  .ubah.}.(h!].h#]
+00003780: 9468 255d 9468 275d 9468 295d 948c 056c  .h%].h'].h)]...l
+00003790: 6576 656c 944b 018c 0474 7970 6594 6a5b  evel.K...type.j[
+000037a0: 0400 008c 0673 6f75 7263 6594 682c 8c04  .....source.h,..
+000037b0: 6c69 6e65 944b 2c75 682b 6a40 0400 0075  line.K,uh+j@...u
+000037c0: 6261 8c0b 7472 616e 7366 6f72 6d65 7294  ba..transformer.
+000037d0: 4e8c 0b69 6e63 6c75 6465 5f6c 6f67 945d  N..include_log.]
+000037e0: 948c 0a64 6563 6f72 6174 696f 6e94 4e68  ...decoration.Nh
+000037f0: 1c68 0375 622e                           .h.ub.
```

### Comparing `nester-struct-0.5.1/docs/_build/html/.doctrees/source/utils.doctree` & `nester-struct-0.5.2/docs/_build/html/.doctrees/source/utils.doctree`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/docs/_build/html/.doctrees/supported_languages.doctree` & `nester-struct-0.5.2/docs/_build/html/.doctrees/supported_languages.doctree`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/docs/_build/html/.doctrees/usage_guide.doctree` & `nester-struct-0.5.2/docs/_build/html/.doctrees/usage_guide.doctree`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8005 9575 5a00 0000 0000 008c 0f73 7068  ...uZ........sph
+00000000: 8005 950c 5a00 0000 0000 008c 0f73 7068  ....Z........sph
 00000010: 696e 782e 6164 646e 6f64 6573 948c 0864  inx.addnodes...d
 00000020: 6f63 756d 656e 7494 9394 2981 947d 9428  ocument...)..}.(
 00000030: 8c09 7261 7773 6f75 7263 6594 8c00 948c  ..rawsource.....
 00000040: 0863 6869 6c64 7265 6e94 5d94 8c0e 646f  .children.]...do
 00000050: 6375 7469 6c73 2e6e 6f64 6573 948c 0773  cutils.nodes...s
 00000060: 6563 7469 6f6e 9493 9429 8194 7d94 2868  ection...)..}.(h
 00000070: 0568 0668 075d 9428 6809 8c05 7469 746c  .h.h.].(h...titl
@@ -134,1315 +134,1309 @@
 00000850: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
 00000860: 5d94 6829 5d94 7568 2b68 6f68 1b68 6c68  ].h)].uh+hoh.hlh
 00000870: 1c68 0368 1d68 2c68 1e4e 7562 6568 1f7d  .h.h.h,h.Nubeh.}
 00000880: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
 00000890: 5d94 6829 5d94 8c06 6275 6c6c 6574 948c  ].h)]...bullet..
 000008a0: 012d 9475 682b 686a 681d 682c 681e 4b0f  .-.uh+hjh.h,h.K.
 000008b0: 681b 684b 681c 6803 7562 682e 2981 947d  h.hKh.h.ubh.)..}
-000008c0: 9428 6805 8c2d 4c65 7420 7573 206c 6f6f  .(h..-Let us loo
-000008d0: 6b20 696e 746f 2065 6163 6820 7468 7265  k into each thre
-000008e0: 6520 696e 206d 6f72 6520 6465 7461 696c  e in more detail
-000008f0: 2e2e 2e94 6807 5d94 6816 8c2d 4c65 7420  ....h.].h..-Let 
-00000900: 7573 206c 6f6f 6b20 696e 746f 2065 6163  us look into eac
-00000910: 6820 7468 7265 6520 696e 206d 6f72 6520  h three in more 
-00000920: 6465 7461 696c e280 a694 8594 8194 7d94  detail........}.
-00000930: 2868 1b68 fc68 1c68 0368 1d4e 681e 4e75  (h.h.h.h.h.Nh.Nu
-00000940: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-00000950: 255d 9468 275d 9468 295d 9475 682b 682d  %].h'].h)].uh+h-
-00000960: 681d 682c 681e 4b14 681b 684b 681c 6803  h.h,h.K.h.hKh.h.
-00000970: 7562 680b 2981 947d 9428 6805 6806 6807  ubh.)..}.(h.h.h.
-00000980: 5d94 2868 1029 8194 7d94 2868 058c 0d4e  ].(h.)..}.(h...N
-00000990: 6573 7465 7220 6372 6561 7465 9468 075d  ester create.h.]
-000009a0: 9468 168c 0d4e 6573 7465 7220 6372 6561  .h...Nester crea
-000009b0: 7465 9485 9481 947d 9428 681b 6a0d 0100  te.....}.(h.j...
-000009c0: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
-000009d0: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-000009e0: 275d 9468 295d 9475 682b 680f 681b 6a0a  '].h)].uh+h.h.j.
-000009f0: 0100 0068 1c68 0368 1d68 2c68 1e4b 1775  ...h.h.h.h,h.K.u
-00000a00: 6268 008c 0569 6e64 6578 9493 9429 8194  bh...index...)..
-00000a10: 7d94 2868 0568 0668 075d 9468 1f7d 9428  }.(h.h.h.].h.}.(
-00000a20: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-00000a30: 6829 5d94 8c07 656e 7472 6965 7394 5d94  h)]...entries.].
-00000a40: 7568 2b6a 1b01 0000 681b 6a0a 0100 0068  uh+j....h.j....h
-00000a50: 1c68 0368 1d4e 681e 4e75 6268 008c 0464  .h.h.Nh.Nubh...d
-00000a60: 6573 6394 9394 2981 947d 9428 6805 6806  esc...)..}.(h.h.
-00000a70: 6807 5d94 2868 008c 0e64 6573 635f 7369  h.].(h...desc_si
-00000a80: 676e 6174 7572 6594 9394 2981 947d 9428  gnature...)..}.(
-00000a90: 6805 8c30 6e65 7374 6572 2063 7265 6174  h..0nester creat
-00000aa0: 6528 6c61 6e67 7561 6765 2c20 7072 6f6a  e(language, proj
-00000ab0: 6563 746e 616d 652c 205b 2d67 7c2d 2d67  ectname, [-g|--g
-00000ac0: 6974 5d29 9468 075d 9468 008c 0964 6573  it]).h.].h...des
-00000ad0: 635f 6e61 6d65 9493 9429 8194 7d94 2868  c_name...)..}.(h
-00000ae0: 056a 3101 0000 6807 5d94 6816 8c30 6e65  .j1...h.].h..0ne
-00000af0: 7374 6572 2063 7265 6174 6528 6c61 6e67  ster create(lang
-00000b00: 7561 6765 2c20 7072 6f6a 6563 746e 616d  uage, projectnam
-00000b10: 652c 205b 2d67 7c2d 2d67 6974 5d29 9485  e, [-g|--git])..
-00000b20: 9481 947d 9428 681b 6a35 0100 0068 1c68  ...}.(h.j5...h.h
-00000b30: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
-00000b40: 215d 9468 235d 9428 8c08 7369 672d 6e61  !].h#].(..sig-na
-00000b50: 6d65 948c 0864 6573 636e 616d 6594 6568  me...descname.eh
-00000b60: 255d 9468 275d 9468 295d 948c 0978 6d6c  %].h'].h)]...xml
-00000b70: 3a73 7061 6365 948c 0870 7265 7365 7276  :space...preserv
-00000b80: 6594 7568 2b6a 3301 0000 681b 6a2f 0100  e.uh+j3...h.j/..
-00000b90: 0068 1c68 0368 1d68 2c68 1e4b 1975 6261  .h.h.h.h,h.K.uba
-00000ba0: 681f 7d94 2868 215d 9468 235d 9428 8c03  h.}.(h!].h#].(..
-00000bb0: 7369 6794 8c0a 7369 672d 6f62 6a65 6374  sig...sig-object
-00000bc0: 9465 6825 5d94 6827 5d94 6829 5d94 8c0a  .eh%].h'].h)]...
-00000bd0: 5f74 6f63 5f70 6172 7473 9429 8c09 5f74  _toc_parts.).._t
-00000be0: 6f63 5f6e 616d 6594 6806 7568 2b6a 2d01  oc_name.h.uh+j-.
-00000bf0: 0000 681d 682c 681e 4b19 681b 6a2a 0100  ..h.h,h.K.h.j*..
-00000c00: 0068 1c68 0375 6268 008c 0c64 6573 635f  .h.h.ubh...desc_
-00000c10: 636f 6e74 656e 7494 9394 2981 947d 9428  content...)..}.(
-00000c20: 6805 6806 6807 5d94 2868 2e29 8194 7d94  h.h.h.].(h.)..}.
-00000c30: 2868 0558 0501 0000 4372 6561 7465 7320  (h.X....Creates 
-00000c40: 7468 6520 7072 6f6a 6563 7420 7374 7275  the project stru
-00000c50: 6374 7572 6520 666f 7220 7468 6520 6769  cture for the gi
-00000c60: 7665 6e20 7072 6f6a 6563 742e 0a49 6620  ven project..If 
-00000c70: 796f 7520 6172 6520 616c 7265 6164 7920  you are already 
-00000c80: 696e 2061 2064 6972 6563 746f 7279 2077  in a directory w
-00000c90: 6869 6368 206d 6174 6368 6573 2074 6865  hich matches the
-00000ca0: 206e 616d 6520 6f66 2074 6865 2067 6976   name of the giv
-00000cb0: 656e 2070 726f 6a65 6374 2c20 7468 6520  en project, the 
-00000cc0: 736f 7572 6365 2066 696c 6573 2077 696c  source files wil
-00000cd0: 6c20 6265 2063 7265 6174 6564 2069 6e20  l be created in 
-00000ce0: 796f 7572 2063 7572 7265 6e74 2064 6972  your current dir
-00000cf0: 6563 746f 7279 2e0a 4966 206e 6f74 204e  ectory..If not N
-00000d00: 6573 7465 7220 7769 6c6c 2061 7574 6f6d  ester will autom
-00000d10: 6174 6963 616c 6c79 2063 7265 6174 6520  atically create 
-00000d20: 6120 6469 7265 6374 6f72 7920 666f 7220  a directory for 
-00000d30: 796f 7572 2070 726f 6a65 6374 2e94 6807  your project..h.
-00000d40: 5d94 6816 5805 0100 0043 7265 6174 6573  ].h.X....Creates
-00000d50: 2074 6865 2070 726f 6a65 6374 2073 7472   the project str
-00000d60: 7563 7475 7265 2066 6f72 2074 6865 2067  ucture for the g
-00000d70: 6976 656e 2070 726f 6a65 6374 2e0a 4966  iven project..If
-00000d80: 2079 6f75 2061 7265 2061 6c72 6561 6479   you are already
-00000d90: 2069 6e20 6120 6469 7265 6374 6f72 7920   in a directory 
-00000da0: 7768 6963 6820 6d61 7463 6865 7320 7468  which matches th
-00000db0: 6520 6e61 6d65 206f 6620 7468 6520 6769  e name of the gi
-00000dc0: 7665 6e20 7072 6f6a 6563 742c 2074 6865  ven project, the
-00000dd0: 2073 6f75 7263 6520 6669 6c65 7320 7769   source files wi
-00000de0: 6c6c 2062 6520 6372 6561 7465 6420 696e  ll be created in
-00000df0: 2079 6f75 7220 6375 7272 656e 7420 6469   your current di
-00000e00: 7265 6374 6f72 792e 0a49 6620 6e6f 7420  rectory..If not 
-00000e10: 4e65 7374 6572 2077 696c 6c20 6175 746f  Nester will auto
-00000e20: 6d61 7469 6361 6c6c 7920 6372 6561 7465  matically create
-00000e30: 2061 2064 6972 6563 746f 7279 2066 6f72   a directory for
-00000e40: 2079 6f75 7220 7072 6f6a 6563 742e 9485   your project...
-00000e50: 9481 947d 9428 681b 6a55 0100 0068 1c68  ...}.(h.jU...h.h
-00000e60: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
-00000e70: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-00000e80: 295d 9475 682b 682d 681d 682c 681e 4b1b  )].uh+h-h.h,h.K.
-00000e90: 681b 6a52 0100 0068 1c68 0375 6268 098c  h.jR...h.h.ubh..
-00000ea0: 0a66 6965 6c64 5f6c 6973 7494 9394 2981  .field_list...).
-00000eb0: 947d 9428 6805 6806 6807 5d94 2868 098c  .}.(h.h.h.].(h..
-00000ec0: 0566 6965 6c64 9493 9429 8194 7d94 2868  .field...)..}.(h
-00000ed0: 0568 0668 075d 9428 6809 8c0a 6669 656c  .h.h.].(h...fiel
-00000ee0: 645f 6e61 6d65 9493 9429 8194 7d94 2868  d_name...)..}.(h
-00000ef0: 058c 0a50 6172 616d 6574 6572 7394 6807  ...Parameters.h.
-00000f00: 5d94 6816 8c0a 5061 7261 6d65 7465 7273  ].h...Parameters
-00000f10: 9485 9481 947d 9428 681b 6a6f 0100 0068  .....}.(h.jo...h
-00000f20: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
-00000f30: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
-00000f40: 9468 295d 9475 682b 6a6d 0100 0068 1b6a  .h)].uh+jm...h.j
-00000f50: 6a01 0000 681d 682c 681e 4b00 7562 6809  j...h.h,h.K.ubh.
-00000f60: 8c0a 6669 656c 645f 626f 6479 9493 9429  ..field_body...)
-00000f70: 8194 7d94 2868 0568 0668 075d 9468 6b29  ..}.(h.h.h.].hk)
-00000f80: 8194 7d94 2868 0568 0668 075d 9428 6870  ..}.(h.h.h.].(hp
-00000f90: 2981 947d 9428 6805 6806 6807 5d94 682e  )..}.(h.h.h.].h.
-00000fa0: 2981 947d 9428 6805 8c8a 6c61 6e67 7561  )..}.(h...langua
-00000fb0: 6765 2028 7374 7229 202d 2d20 5468 6520  ge (str) -- The 
-00000fc0: 7368 6f72 7466 6f72 6d20 6f66 2061 2073  shortform of a s
-00000fd0: 7570 706f 7274 6564 2070 726f 6772 616d  upported program
-00000fe0: 6d69 6e67 206c 616e 6775 6167 652e 2052  ming language. R
-00000ff0: 6566 6572 2074 6f20 7468 6520 3a64 6f63  efer to the :doc
-00001000: 3a20 6c69 7374 206f 6620 7375 7070 6f72  : list of suppor
-00001010: 7465 6420 6c61 6e67 7561 6765 7320 3c73  ted languages <s
-00001020: 7570 706f 7274 6564 5f6c 616e 6775 6167  upported_languag
-00001030: 6573 3e2e 9468 075d 9428 6800 8c0e 6c69  es>..h.].(h...li
-00001040: 7465 7261 6c5f 7374 726f 6e67 9493 9429  teral_strong...)
-00001050: 8194 7d94 2868 058c 086c 616e 6775 6167  ..}.(h...languag
-00001060: 6594 6807 5d94 6816 8c08 6c61 6e67 7561  e.h.].h...langua
-00001070: 6765 9485 9481 947d 9428 681b 6a8e 0100  ge.....}.(h.j...
-00001080: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
-00001090: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-000010a0: 275d 9468 295d 9475 682b 6a8c 0100 0068  '].h)].uh+j....h
-000010b0: 1b6a 8801 0000 7562 6816 8c02 2028 9485  .j....ubh... (..
-000010c0: 9481 947d 9428 681b 6a88 0100 0068 1c68  ...}.(h.j....h.h
-000010d0: 0368 1d4e 681e 4e75 6268 008c 0c70 656e  .h.Nh.Nubh...pen
-000010e0: 6469 6e67 5f78 7265 6694 9394 2981 947d  ding_xref...)..}
-000010f0: 9428 6805 6806 6807 5d94 6800 8c10 6c69  .(h.h.h.].h...li
-00001100: 7465 7261 6c5f 656d 7068 6173 6973 9493  teral_emphasis..
-00001110: 9429 8194 7d94 2868 058c 0373 7472 9468  .)..}.(h...str.h
-00001120: 075d 9468 168c 0373 7472 9485 9481 947d  .].h...str.....}
-00001130: 9428 681b 6aa7 0100 0068 1c68 0368 1d4e  .(h.j....h.h.h.N
-00001140: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
-00001150: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
-00001160: 682b 6aa5 0100 0068 1b6a a201 0000 7562  h+j....h.j....ub
-00001170: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
-00001180: 5d94 6827 5d94 6829 5d94 8c09 7265 6664  ].h'].h)]...refd
-00001190: 6f6d 6169 6e94 8c02 7079 948c 0b72 6566  omain...py...ref
-000011a0: 6578 706c 6963 6974 9489 8c07 7265 6674  explicit....reft
-000011b0: 7970 6594 8c05 636c 6173 7394 8c09 7265  ype...class...re
-000011c0: 6674 6172 6765 7494 6aa9 0100 008c 0b72  ftarget.j......r
-000011d0: 6566 7370 6563 6966 6963 9488 8c09 7079  efspecific....py
-000011e0: 3a6d 6f64 756c 6594 4e8c 0870 793a 636c  :module.N..py:cl
-000011f0: 6173 7394 4e75 682b 6aa0 0100 0068 1b6a  ass.Nuh+j....h.j
-00001200: 8801 0000 7562 6816 8c01 2994 8594 8194  ....ubh...).....
-00001210: 7d94 2868 1b6a 8801 0000 681c 6803 681d  }.(h.j....h.h.h.
-00001220: 4e68 1e4e 7562 6816 8c05 20e2 8093 2094  Nh.Nubh... ... .
-00001230: 8594 8194 7d94 2868 1b6a 8801 0000 681c  ....}.(h.j....h.
-00001240: 6803 681d 4e68 1e4e 7562 6816 8c46 5468  h.h.Nh.Nubh..FTh
-00001250: 6520 7368 6f72 7466 6f72 6d20 6f66 2061  e shortform of a
-00001260: 2073 7570 706f 7274 6564 2070 726f 6772   supported progr
-00001270: 616d 6d69 6e67 206c 616e 6775 6167 652e  amming language.
-00001280: 2052 6566 6572 2074 6f20 7468 6520 3a64   Refer to the :d
-00001290: 6f63 3a20 9485 9481 947d 9428 681b 6a88  oc: .....}.(h.j.
-000012a0: 0100 0068 1c68 0368 1d4e 681e 4e75 6268  ...h.h.h.Nh.Nubh
-000012b0: 7929 8194 7d94 2868 058c 3360 6c69 7374  y)..}.(h..3`list
-000012c0: 206f 6620 7375 7070 6f72 7465 6420 6c61   of supported la
-000012d0: 6e67 7561 6765 7320 3c73 7570 706f 7274  nguages <support
-000012e0: 6564 5f6c 616e 6775 6167 6573 3e60 9468  ed_languages>`.h
-000012f0: 075d 9468 168c 316c 6973 7420 6f66 2073  .].h..1list of s
-00001300: 7570 706f 7274 6564 206c 616e 6775 6167  upported languag
-00001310: 6573 203c 7375 7070 6f72 7465 645f 6c61  es <supported_la
-00001320: 6e67 7561 6765 733e 9485 9481 947d 9428  nguages>.....}.(
-00001330: 681b 6ad0 0100 0068 1c68 0368 1d4e 681e  h.j....h.h.h.Nh.
-00001340: 4e75 6261 681f 7d94 2868 215d 9468 235d  Nubah.}.(h!].h#]
-00001350: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
-00001360: 6878 681b 6a88 0100 0068 1c68 0368 1d4e  hxh.j....h.h.h.N
-00001370: 681e 4e75 6268 168c 012e 9485 9481 947d  h.Nubh.........}
-00001380: 9428 681b 6a88 0100 0068 1c68 0368 1d4e  .(h.j....h.h.h.N
-00001390: 681e 4e75 6265 681f 7d94 2868 215d 9468  h.Nubeh.}.(h!].h
-000013a0: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
-000013b0: 682b 682d 681b 6a85 0100 0075 6261 681f  h+h-h.j....ubah.
-000013c0: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-000013d0: 275d 9468 295d 9475 682b 686f 681b 6a82  '].h)].uh+hoh.j.
-000013e0: 0100 0075 6268 7029 8194 7d94 2868 0568  ...ubhp)..}.(h.h
-000013f0: 0668 075d 9468 2e29 8194 7d94 2868 058c  .h.].h.)..}.(h..
-00001400: 4a70 726f 6a65 6374 6e61 6d65 2028 7374  Jprojectname (st
-00001410: 7229 202d 2d20 5468 6520 6e61 6d65 206f  r) -- The name o
-00001420: 6620 7468 6520 7072 6f6a 6563 7420 7061  f the project pa
-00001430: 636b 6167 6520 7468 6174 2077 696c 6c20  ckage that will 
-00001440: 6265 2063 7265 6174 6564 2e94 6807 5d94  be created..h.].
-00001450: 286a 8d01 0000 2981 947d 9428 6805 8c0b  (j....)..}.(h...
-00001460: 7072 6f6a 6563 746e 616d 6594 6807 5d94  projectname.h.].
-00001470: 6816 8c0b 7072 6f6a 6563 746e 616d 6594  h...projectname.
-00001480: 8594 8194 7d94 2868 1b6a f501 0000 681c  ....}.(h.j....h.
-00001490: 6803 681d 4e68 1e4e 7562 6168 1f7d 9428  h.h.Nh.Nubah.}.(
-000014a0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-000014b0: 6829 5d94 7568 2b6a 8c01 0000 681b 6af1  h)].uh+j....h.j.
-000014c0: 0100 0075 6268 168c 0220 2894 8594 8194  ...ubh... (.....
-000014d0: 7d94 2868 1b6a f101 0000 681c 6803 681d  }.(h.j....h.h.h.
-000014e0: 4e68 1e4e 7562 6aa1 0100 0029 8194 7d94  Nh.Nubj....)..}.
-000014f0: 2868 0568 0668 075d 946a a601 0000 2981  (h.h.h.].j....).
-00001500: 947d 9428 6805 8c03 7374 7294 6807 5d94  .}.(h...str.h.].
-00001510: 6816 8c03 7374 7294 8594 8194 7d94 2868  h...str.....}.(h
-00001520: 1b6a 0a02 0000 681c 6803 681d 4e68 1e4e  .j....h.h.h.Nh.N
-00001530: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
-00001540: 6825 5d94 6827 5d94 6829 5d94 7568 2b6a  h%].h'].h)].uh+j
-00001550: a501 0000 681b 6a07 0200 0075 6261 681f  ....h.j....ubah.
-00001560: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-00001570: 275d 9468 295d 948c 0972 6566 646f 6d61  '].h)]...refdoma
-00001580: 696e 946a bc01 0000 8c0b 7265 6665 7870  in.j......refexp
-00001590: 6c69 6369 7494 898c 0772 6566 7479 7065  licit....reftype
-000015a0: 946a bf01 0000 8c09 7265 6674 6172 6765  .j......reftarge
-000015b0: 7494 6a0c 0200 006a c101 0000 886a c201  t.j....j.....j..
-000015c0: 0000 4e6a c301 0000 4e75 682b 6aa0 0100  ..Nj....Nuh+j...
-000015d0: 0068 1b6a f101 0000 7562 6816 8c01 2994  .h.j....ubh...).
-000015e0: 8594 8194 7d94 2868 1b6a f101 0000 681c  ....}.(h.j....h.
-000015f0: 6803 681d 4e68 1e4e 7562 6816 8c05 20e2  h.h.Nh.Nubh... .
-00001600: 8093 2094 8594 8194 7d94 2868 1b6a f101  .. .....}.(h.j..
-00001610: 0000 681c 6803 681d 4e68 1e4e 7562 6816  ..h.h.h.Nh.Nubh.
-00001620: 8c35 5468 6520 6e61 6d65 206f 6620 7468  .5The name of th
-00001630: 6520 7072 6f6a 6563 7420 7061 636b 6167  e project packag
-00001640: 6520 7468 6174 2077 696c 6c20 6265 2063  e that will be c
-00001650: 7265 6174 6564 2e94 8594 8194 7d94 2868  reated......}.(h
-00001660: 1b6a f101 0000 681c 6803 681d 4e68 1e4e  .j....h.h.h.Nh.N
-00001670: 7562 6568 1f7d 9428 6821 5d94 6823 5d94  ubeh.}.(h!].h#].
-00001680: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
-00001690: 2d68 1b6a ee01 0000 7562 6168 1f7d 9428  -h.j....ubah.}.(
-000016a0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-000016b0: 6829 5d94 7568 2b68 6f68 1b6a 8201 0000  h)].uh+hoh.j....
-000016c0: 7562 6870 2981 947d 9428 6805 6806 6807  ubhp)..}.(h.h.h.
-000016d0: 5d94 682e 2981 947d 9428 6805 8cb6 2d67  ].h.)..}.(h...-g
-000016e0: 7c2d 2d67 6974 2028 666c 6167 2920 2d2d  |--git (flag) --
-000016f0: 2041 6e20 6f70 7469 6f6e 616c 2066 6c61   An optional fla
-00001700: 6720 746f 2069 6e69 7469 616c 697a 6520  g to initialize 
-00001710: 6120 4769 7420 7265 706f 7369 746f 7279  a Git repository
-00001720: 2069 6e20 7468 6520 7072 6f6a 6563 7420   in the project 
-00001730: 6469 7265 6374 6f72 792e 2049 6620 7370  directory. If sp
-00001740: 6563 6966 6965 642c 2061 2047 6974 2072  ecified, a Git r
-00001750: 6570 6f73 6974 6f72 7920 7769 6c6c 2062  epository will b
-00001760: 6520 6372 6561 7465 6420 7369 6d75 6c74  e created simult
-00001770: 616e 656f 7573 6c79 2077 6974 6820 7468  aneously with th
-00001780: 6520 7072 6f6a 6563 7420 7374 7275 6374  e project struct
-00001790: 7572 652e 9468 075d 9428 6a8d 0100 0029  ure..h.].(j....)
-000017a0: 8194 7d94 2868 058c 022d 6794 6807 5d94  ..}.(h...-g.h.].
-000017b0: 6816 8c02 2d67 9485 9481 947d 9428 681b  h...-g.....}.(h.
-000017c0: 6a41 0200 0068 1c68 0368 1d4e 681e 4e75  jA...h.h.h.Nh.Nu
-000017d0: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-000017e0: 255d 9468 275d 9468 295d 9475 682b 6a8c  %].h'].h)].uh+j.
-000017f0: 0100 0068 1b6a 3d02 0000 7562 6a8d 0100  ...h.j=...ubj...
-00001800: 0029 8194 7d94 2868 058c 017c 9468 075d  .)..}.(h...|.h.]
-00001810: 9468 168c 017c 9485 9481 947d 9428 681b  .h...|.....}.(h.
-00001820: 6a4f 0200 0068 1c68 0368 1d4e 681e 4e75  jO...h.h.h.Nh.Nu
-00001830: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-00001840: 255d 9468 275d 9468 295d 9475 682b 6a8c  %].h'].h)].uh+j.
-00001850: 0100 0068 1b6a 3d02 0000 7562 6a8d 0100  ...h.j=...ubj...
-00001860: 0029 8194 7d94 2868 058c 052d 2d67 6974  .)..}.(h...--git
-00001870: 9468 075d 9468 168c 052d 2d67 6974 9485  .h.].h...--git..
-00001880: 9481 947d 9428 681b 6a5d 0200 0068 1c68  ...}.(h.j]...h.h
-00001890: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
-000018a0: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-000018b0: 295d 9475 682b 6a8c 0100 0068 1b6a 3d02  )].uh+j....h.j=.
-000018c0: 0000 7562 6816 8c02 2028 9485 9481 947d  ..ubh... (.....}
-000018d0: 9428 681b 6a3d 0200 0068 1c68 0368 1d4e  .(h.j=...h.h.h.N
-000018e0: 681e 4e75 626a a101 0000 2981 947d 9428  h.Nubj....)..}.(
-000018f0: 6805 6806 6807 5d94 6aa6 0100 0029 8194  h.h.h.].j....)..
-00001900: 7d94 2868 058c 0466 6c61 6794 6807 5d94  }.(h...flag.h.].
-00001910: 6816 8c04 666c 6167 9485 9481 947d 9428  h...flag.....}.(
-00001920: 681b 6a72 0200 0068 1c68 0368 1d4e 681e  h.jr...h.h.h.Nh.
-00001930: 4e75 6261 681f 7d94 2868 215d 9468 235d  Nubah.}.(h!].h#]
-00001940: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
-00001950: 6aa5 0100 0068 1b6a 6f02 0000 7562 6168  j....h.jo...ubah
-00001960: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
-00001970: 6827 5d94 6829 5d94 8c09 7265 6664 6f6d  h'].h)]...refdom
-00001980: 6169 6e94 6abc 0100 008c 0b72 6566 6578  ain.j......refex
-00001990: 706c 6963 6974 9489 8c07 7265 6674 7970  plicit....reftyp
-000019a0: 6594 6abf 0100 008c 0972 6566 7461 7267  e.j......reftarg
-000019b0: 6574 946a 7402 0000 6ac1 0100 0088 6ac2  et.jt...j.....j.
-000019c0: 0100 004e 6ac3 0100 004e 7568 2b6a a001  ...Nj....Nuh+j..
-000019d0: 0000 681b 6a3d 0200 0075 6268 168c 0129  ..h.j=...ubh...)
-000019e0: 9485 9481 947d 9428 681b 6a3d 0200 0068  .....}.(h.j=...h
-000019f0: 1c68 0368 1d4e 681e 4e75 6268 168c 0520  .h.h.Nh.Nubh... 
-00001a00: e280 9320 9485 9481 947d 9428 681b 6a3d  ... .....}.(h.j=
-00001a10: 0200 0068 1c68 0368 1d4e 681e 4e75 6268  ...h.h.h.Nh.Nubh
-00001a20: 168c a341 6e20 6f70 7469 6f6e 616c 2066  ...An optional f
-00001a30: 6c61 6720 746f 2069 6e69 7469 616c 697a  lag to initializ
-00001a40: 6520 6120 4769 7420 7265 706f 7369 746f  e a Git reposito
-00001a50: 7279 2069 6e20 7468 6520 7072 6f6a 6563  ry in the projec
-00001a60: 7420 6469 7265 6374 6f72 792e 2049 6620  t directory. If 
-00001a70: 7370 6563 6966 6965 642c 2061 2047 6974  specified, a Git
-00001a80: 2072 6570 6f73 6974 6f72 7920 7769 6c6c   repository will
-00001a90: 2062 6520 6372 6561 7465 6420 7369 6d75   be created simu
-00001aa0: 6c74 616e 656f 7573 6c79 2077 6974 6820  ltaneously with 
-00001ab0: 7468 6520 7072 6f6a 6563 7420 7374 7275  the project stru
-00001ac0: 6374 7572 652e 9485 9481 947d 9428 681b  cture......}.(h.
-00001ad0: 6a3d 0200 0068 1c68 0368 1d4e 681e 4e75  j=...h.h.h.Nh.Nu
-00001ae0: 6265 681f 7d94 2868 215d 9468 235d 9468  beh.}.(h!].h#].h
-00001af0: 255d 9468 275d 9468 295d 9475 682b 682d  %].h'].h)].uh+h-
-00001b00: 681b 6a3a 0200 0075 6261 681f 7d94 2868  h.j:...ubah.}.(h
-00001b10: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-00001b20: 295d 9475 682b 686f 681b 6a82 0100 0075  )].uh+hoh.j....u
-00001b30: 6268 7029 8194 7d94 2868 0568 0668 075d  bhp)..}.(h.h.h.]
-00001b40: 9468 2e29 8194 7d94 2868 058c 572d 2d6e  .h.)..}.(h..W--n
-00001b50: 6f2d 6c6f 6720 2866 6c61 6729 202d 2d20  o-log (flag) -- 
-00001b60: 416e 206f 7074 696f 6e61 6c20 666c 6167  An optional flag
-00001b70: 2074 6f20 6469 7361 626c 6520 7072 6f6a   to disable proj
-00001b80: 6563 7420 6c6f 6767 696e 6720 666f 7220  ect logging for 
-00001b90: 7468 6520 6375 7272 656e 7420 7072 6f6a  the current proj
-00001ba0: 6563 742e 9468 075d 9428 6a8d 0100 0029  ect..h.].(j....)
-00001bb0: 8194 7d94 2868 058c 082d 2d6e 6f2d 6c6f  ..}.(h...--no-lo
-00001bc0: 6794 6807 5d94 6816 8c08 2d2d 6e6f 2d6c  g.h.].h...--no-l
-00001bd0: 6f67 9485 9481 947d 9428 681b 6aa9 0200  og.....}.(h.j...
-00001be0: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
-00001bf0: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-00001c00: 275d 9468 295d 9475 682b 6a8c 0100 0068  '].h)].uh+j....h
-00001c10: 1b6a a502 0000 7562 6816 8c02 2028 9485  .j....ubh... (..
-00001c20: 9481 947d 9428 681b 6aa5 0200 0068 1c68  ...}.(h.j....h.h
-00001c30: 0368 1d4e 681e 4e75 626a a101 0000 2981  .h.Nh.Nubj....).
-00001c40: 947d 9428 6805 6806 6807 5d94 6aa6 0100  .}.(h.h.h.].j...
-00001c50: 0029 8194 7d94 2868 058c 0466 6c61 6794  .)..}.(h...flag.
-00001c60: 6807 5d94 6816 8c04 666c 6167 9485 9481  h.].h...flag....
-00001c70: 947d 9428 681b 6abe 0200 0068 1c68 0368  .}.(h.j....h.h.h
-00001c80: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
-00001c90: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-00001ca0: 9475 682b 6aa5 0100 0068 1b6a bb02 0000  .uh+j....h.j....
-00001cb0: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
-00001cc0: 6825 5d94 6827 5d94 6829 5d94 8c09 7265  h%].h'].h)]...re
-00001cd0: 6664 6f6d 6169 6e94 6abc 0100 008c 0b72  fdomain.j......r
-00001ce0: 6566 6578 706c 6963 6974 9489 8c07 7265  efexplicit....re
-00001cf0: 6674 7970 6594 6abf 0100 008c 0972 6566  ftype.j......ref
-00001d00: 7461 7267 6574 946a c002 0000 6ac1 0100  target.j....j...
-00001d10: 0088 6ac2 0100 004e 6ac3 0100 004e 7568  ..j....Nj....Nuh
-00001d20: 2b6a a001 0000 681b 6aa5 0200 0075 6268  +j....h.j....ubh
-00001d30: 168c 0129 9485 9481 947d 9428 681b 6aa5  ...).....}.(h.j.
-00001d40: 0200 0068 1c68 0368 1d4e 681e 4e75 6268  ...h.h.h.Nh.Nubh
-00001d50: 168c 0520 e280 9320 9485 9481 947d 9428  ... ... .....}.(
-00001d60: 681b 6aa5 0200 0068 1c68 0368 1d4e 681e  h.j....h.h.h.Nh.
-00001d70: 4e75 6268 168c 4441 6e20 6f70 7469 6f6e  Nubh..DAn option
-00001d80: 616c 2066 6c61 6720 746f 2064 6973 6162  al flag to disab
-00001d90: 6c65 2070 726f 6a65 6374 206c 6f67 6769  le project loggi
-00001da0: 6e67 2066 6f72 2074 6865 2063 7572 7265  ng for the curre
-00001db0: 6e74 2070 726f 6a65 6374 2e94 8594 8194  nt project......
-00001dc0: 7d94 2868 1b6a a502 0000 681c 6803 681d  }.(h.j....h.h.h.
-00001dd0: 4e68 1e4e 7562 6568 1f7d 9428 6821 5d94  Nh.Nubeh.}.(h!].
-00001de0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-00001df0: 7568 2b68 2d68 1b6a a202 0000 7562 6168  uh+h-h.j....ubah
-00001e00: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
-00001e10: 6827 5d94 6829 5d94 7568 2b68 6f68 1b6a  h'].h)].uh+hoh.j
-00001e20: 8201 0000 7562 6568 1f7d 9428 6821 5d94  ....ubeh.}.(h!].
-00001e30: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-00001e40: 7568 2b68 6a68 1b6a 7f01 0000 7562 6168  uh+hjh.j....ubah
-00001e50: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
-00001e60: 6827 5d94 6829 5d94 7568 2b6a 7d01 0000  h'].h)].uh+j}...
-00001e70: 681b 6a6a 0100 0075 6265 681f 7d94 2868  h.jj...ubeh.}.(h
-00001e80: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-00001e90: 295d 9475 682b 6a68 0100 0068 1b6a 6501  )].uh+jh...h.je.
-00001ea0: 0000 7562 6a69 0100 0029 8194 7d94 2868  ..ubji...)..}.(h
-00001eb0: 0568 0668 075d 9428 6a6e 0100 0029 8194  .h.h.].(jn...)..
-00001ec0: 7d94 2868 058c 0752 6574 7572 6e73 9468  }.(h...Returns.h
-00001ed0: 075d 9468 168c 0752 6574 7572 6e73 9485  .].h...Returns..
-00001ee0: 9481 947d 9428 681b 6a03 0300 0068 1c68  ...}.(h.j....h.h
-00001ef0: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
-00001f00: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-00001f10: 295d 9475 682b 6a6d 0100 0068 1b6a 0003  )].uh+jm...h.j..
-00001f20: 0000 681d 682c 681e 4b00 7562 6a7e 0100  ..h.h,h.K.ubj~..
-00001f30: 0029 8194 7d94 2868 0568 0668 075d 9468  .)..}.(h.h.h.].h
-00001f40: 2e29 8194 7d94 2868 058c 044e 6f6e 6594  .)..}.(h...None.
-00001f50: 6807 5d94 6816 8c04 4e6f 6e65 9485 9481  h.].h...None....
-00001f60: 947d 9428 681b 6a14 0300 0068 1c68 0368  .}.(h.j....h.h.h
-00001f70: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
-00001f80: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-00001f90: 9475 682b 682d 681b 6a11 0300 0075 6261  .uh+h-h.j....uba
-00001fa0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-00001fb0: 9468 275d 9468 295d 9475 682b 6a7d 0100  .h'].h)].uh+j}..
-00001fc0: 0068 1b6a 0003 0000 7562 6568 1f7d 9428  .h.j....ubeh.}.(
-00001fd0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-00001fe0: 6829 5d94 7568 2b6a 6801 0000 681b 6a65  h)].uh+jh...h.je
-00001ff0: 0100 0075 626a 6901 0000 2981 947d 9428  ...ubji...)..}.(
-00002000: 6805 6806 6807 5d94 286a 6e01 0000 2981  h.h.h.].(jn...).
-00002010: 947d 9428 6805 8c0b 5265 7475 726e 2074  .}.(h...Return t
-00002020: 7970 6594 6807 5d94 6816 8c0b 5265 7475  ype.h.].h...Retu
-00002030: 726e 2074 7970 6594 8594 8194 7d94 2868  rn type.....}.(h
-00002040: 1b6a 3103 0000 681c 6803 681d 4e68 1e4e  .j1...h.h.h.Nh.N
-00002050: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
-00002060: 6825 5d94 6827 5d94 6829 5d94 7568 2b6a  h%].h'].h)].uh+j
-00002070: 6d01 0000 681b 6a2e 0300 0068 1d68 2c68  m...h.j....h.h,h
-00002080: 1e4b 0075 626a 7e01 0000 2981 947d 9428  .K.ubj~...)..}.(
-00002090: 6805 6806 6807 5d94 682e 2981 947d 9428  h.h.h.].h.)..}.(
-000020a0: 6805 8c04 4e6f 6e65 9468 075d 946a a101  h...None.h.].j..
-000020b0: 0000 2981 947d 9428 6805 6806 6807 5d94  ..)..}.(h.h.h.].
-000020c0: 6816 8c04 4e6f 6e65 9485 9481 947d 9428  h...None.....}.(
-000020d0: 681b 6a46 0300 0068 1c68 0368 1d4e 681e  h.jF...h.h.h.Nh.
-000020e0: 4e75 6261 681f 7d94 2868 215d 9468 235d  Nubah.}.(h!].h#]
-000020f0: 9468 255d 9468 275d 9468 295d 948c 0972  .h%].h'].h)]...r
-00002100: 6566 646f 6d61 696e 946a bc01 0000 8c0b  efdomain.j......
-00002110: 7265 6665 7870 6c69 6369 7494 898c 0772  refexplicit....r
-00002120: 6566 7479 7065 946a bf01 0000 8c09 7265  eftype.j......re
-00002130: 6674 6172 6765 7494 8c04 4e6f 6e65 946a  ftarget...None.j
-00002140: c101 0000 886a c201 0000 4e6a c301 0000  .....j....Nj....
-00002150: 4e75 682b 6aa0 0100 0068 1b6a 4203 0000  Nuh+j....h.jB...
-00002160: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
-00002170: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
-00002180: 2d68 1b6a 3f03 0000 7562 6168 1f7d 9428  -h.j?...ubah.}.(
-00002190: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-000021a0: 6829 5d94 7568 2b6a 7d01 0000 681b 6a2e  h)].uh+j}...h.j.
-000021b0: 0300 0075 6265 681f 7d94 2868 215d 9468  ...ubeh.}.(h!].h
-000021c0: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
-000021d0: 682b 6a68 0100 0068 1b6a 6501 0000 7562  h+jh...h.je...ub
-000021e0: 6568 1f7d 9428 6821 5d94 6823 5d94 6825  eh.}.(h!].h#].h%
-000021f0: 5d94 6827 5d94 6829 5d94 7568 2b6a 6301  ].h'].h)].uh+jc.
-00002200: 0000 681b 6a52 0100 0068 1c68 0368 1d4e  ..h.jR...h.h.h.N
-00002210: 681e 4e75 6265 681f 7d94 2868 215d 9468  h.Nubeh.}.(h!].h
-00002220: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
-00002230: 682b 6a50 0100 0068 1b6a 2a01 0000 681c  h+jP...h.j*...h.
-00002240: 6803 681d 682c 681e 4b19 7562 6568 1f7d  h.h.h,h.K.ubeh.}
-00002250: 9428 6821 5d94 6823 5d94 286a bc01 0000  .(h!].h#].(j....
-00002260: 8c08 6675 6e63 7469 6f6e 9465 6825 5d94  ..function.eh%].
-00002270: 6827 5d94 6829 5d94 8c06 646f 6d61 696e  h'].h)]...domain
-00002280: 946a bc01 0000 8c07 6f62 6a74 7970 6594  .j......objtype.
-00002290: 6a79 0300 008c 0864 6573 6374 7970 6594  jy.....desctype.
-000022a0: 6a79 0300 008c 076e 6f69 6e64 6578 9489  jy.....noindex..
-000022b0: 8c0c 6e6f 696e 6465 7865 6e74 7279 9489  ..noindexentry..
-000022c0: 8c0f 6e6f 636f 6e74 656e 7473 656e 7472  ..nocontentsentr
-000022d0: 7994 8975 682b 6a28 0100 0068 1c68 0368  y..uh+j(...h.h.h
-000022e0: 1b6a 0a01 0000 681d 4e68 1e4e 7562 6568  .j....h.Nh.Nubeh
-000022f0: 1f7d 9428 6821 5d94 8c0d 6e65 7374 6572  .}.(h!]...nester
-00002300: 2d63 7265 6174 6594 6168 235d 9468 255d  -create.ah#].h%]
-00002310: 948c 0d6e 6573 7465 7220 6372 6561 7465  ...nester create
-00002320: 9461 6827 5d94 6829 5d94 7568 2b68 0a68  .ah'].h)].uh+h.h
-00002330: 1b68 4b68 1c68 0368 1d68 2c68 1e4b 1775  .hKh.h.h.h,h.K.u
-00002340: 6268 0b29 8194 7d94 2868 0568 0668 075d  bh.)..}.(h.h.h.]
-00002350: 9428 6810 2981 947d 9428 6805 8c0f 4e65  .(h.)..}.(h...Ne
-00002360: 7374 6572 2076 616c 6964 6174 6594 6807  ster validate.h.
-00002370: 5d94 6816 8c0f 4e65 7374 6572 2076 616c  ].h...Nester val
-00002380: 6964 6174 6594 8594 8194 7d94 2868 1b6a  idate.....}.(h.j
-00002390: 8e03 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
-000023a0: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
-000023b0: 5d94 6827 5d94 6829 5d94 7568 2b68 0f68  ].h'].h)].uh+h.h
-000023c0: 1b6a 8b03 0000 681c 6803 681d 682c 681e  .j....h.h.h.h,h.
-000023d0: 4b2b 7562 6a1c 0100 0029 8194 7d94 2868  K+ubj....)..}.(h
-000023e0: 0568 0668 075d 9468 1f7d 9428 6821 5d94  .h.h.].h.}.(h!].
-000023f0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-00002400: 8c07 656e 7472 6965 7394 5d94 7568 2b6a  ..entries.].uh+j
-00002410: 1b01 0000 681b 6a8b 0300 0068 1c68 0368  ....h.j....h.h.h
-00002420: 1d4e 681e 4e75 626a 2901 0000 2981 947d  .Nh.Nubj)...)..}
-00002430: 9428 6805 6806 6807 5d94 286a 2e01 0000  .(h.h.h.].(j....
-00002440: 2981 947d 9428 6805 8c26 6e65 7374 6572  )..}.(h..&nester
-00002450: 2076 616c 6964 6174 6528 6c61 6e67 7561   validate(langua
-00002460: 6765 2c20 7072 6f6a 6563 746e 616d 6529  ge, projectname)
-00002470: 9468 075d 946a 3401 0000 2981 947d 9428  .h.].j4...)..}.(
-00002480: 6805 6aac 0300 0068 075d 9468 168c 266e  h.j....h.].h..&n
-00002490: 6573 7465 7220 7661 6c69 6461 7465 286c  ester validate(l
-000024a0: 616e 6775 6167 652c 2070 726f 6a65 6374  anguage, project
-000024b0: 6e61 6d65 2994 8594 8194 7d94 2868 1b6a  name).....}.(h.j
-000024c0: ae03 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
-000024d0: 6168 1f7d 9428 6821 5d94 6823 5d94 286a  ah.}.(h!].h#].(j
-000024e0: 3f01 0000 6a40 0100 0065 6825 5d94 6827  ?...j@...eh%].h'
-000024f0: 5d94 6829 5d94 6a44 0100 006a 4501 0000  ].h)].jD...jE...
-00002500: 7568 2b6a 3301 0000 681b 6aaa 0300 0068  uh+j3...h.j....h
-00002510: 1c68 0368 1d68 2c68 1e4b 2d75 6261 681f  .h.h.h,h.K-ubah.
-00002520: 7d94 2868 215d 9468 235d 9428 6a49 0100  }.(h!].h#].(jI..
-00002530: 006a 4a01 0000 6568 255d 9468 275d 9468  .jJ...eh%].h'].h
-00002540: 295d 946a 4e01 0000 296a 4f01 0000 6806  )].jN...)jO...h.
-00002550: 7568 2b6a 2d01 0000 681d 682c 681e 4b2d  uh+j-...h.h,h.K-
-00002560: 681b 6aa7 0300 0068 1c68 0375 626a 5101  h.j....h.h.ubjQ.
-00002570: 0000 2981 947d 9428 6805 6806 6807 5d94  ..)..}.(h.h.h.].
-00002580: 2868 2e29 8194 7d94 2868 058c e056 616c  (h.)..}.(h...Val
-00002590: 6964 6174 6573 2074 6865 2066 696c 6520  idates the file 
-000025a0: 7374 7275 6374 7572 6520 6f66 2074 6865  structure of the
-000025b0: 2067 6976 656e 2070 726f 6a65 6374 2061   given project a
-000025c0: 6761 696e 7374 206f 7572 204a 534f 4e20  gainst our JSON 
-000025d0: 7363 686d 656d 6173 2e0a 4669 6c65 7320  schmemas..Files 
-000025e0: 796f 7520 6372 6561 7465 642c 2077 6869  you created, whi
-000025f0: 6368 2061 7265 2074 6865 7265 666f 7265  ch are therefore
-00002600: 206e 6f74 2070 6172 7420 6f66 206f 7572   not part of our
-00002610: 2073 6368 656d 612c 206f 7220 7375 6368   schema, or such
-00002620: 2077 6869 6368 2068 6176 6520 6265 656e   which have been
-00002630: 2063 7265 6174 6564 2062 7920 6f74 6865   created by othe
-00002640: 7220 7574 696c 6974 6573 2028 652e 672e  r utilites (e.g.
-00002650: 2060 6769 7420 696e 6974 6029 2077 696c   `git init`) wil
-00002660: 6c20 6265 2069 676e 6f72 6564 2e94 6807  l be ignored..h.
-00002670: 5d94 2868 168c c456 616c 6964 6174 6573  ].(h...Validates
-00002680: 2074 6865 2066 696c 6520 7374 7275 6374   the file struct
-00002690: 7572 6520 6f66 2074 6865 2067 6976 656e  ure of the given
-000026a0: 2070 726f 6a65 6374 2061 6761 696e 7374   project against
-000026b0: 206f 7572 204a 534f 4e20 7363 686d 656d   our JSON schmem
-000026c0: 6173 2e0a 4669 6c65 7320 796f 7520 6372  as..Files you cr
-000026d0: 6561 7465 642c 2077 6869 6368 2061 7265  eated, which are
-000026e0: 2074 6865 7265 666f 7265 206e 6f74 2070   therefore not p
-000026f0: 6172 7420 6f66 206f 7572 2073 6368 656d  art of our schem
-00002700: 612c 206f 7220 7375 6368 2077 6869 6368  a, or such which
-00002710: 2068 6176 6520 6265 656e 2063 7265 6174   have been creat
-00002720: 6564 2062 7920 6f74 6865 7220 7574 696c  ed by other util
-00002730: 6974 6573 2028 652e 672e 2094 8594 8194  ites (e.g. .....
-00002740: 7d94 2868 1b6a c403 0000 681c 6803 681d  }.(h.j....h.h.h.
-00002750: 4e68 1e4e 7562 6879 2981 947d 9428 6805  Nh.Nubhy)..}.(h.
-00002760: 8c0a 6067 6974 2069 6e69 7460 9468 075d  ..`git init`.h.]
-00002770: 9468 168c 0867 6974 2069 6e69 7494 8594  .h...git init...
-00002780: 8194 7d94 2868 1b6a cc03 0000 681c 6803  ..}.(h.j....h.h.
-00002790: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
-000027a0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-000027b0: 5d94 7568 2b68 7868 1b6a c403 0000 7562  ].uh+hxh.j....ub
-000027c0: 6816 8c12 2920 7769 6c6c 2062 6520 6967  h...) will be ig
-000027d0: 6e6f 7265 642e 9485 9481 947d 9428 681b  nored......}.(h.
-000027e0: 6ac4 0300 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
-000027f0: 6265 681f 7d94 2868 215d 9468 235d 9468  beh.}.(h!].h#].h
-00002800: 255d 9468 275d 9468 295d 9475 682b 682d  %].h'].h)].uh+h-
-00002810: 681d 682c 681e 4b2f 681b 6ac1 0300 0068  h.h,h.K/h.j....h
-00002820: 1c68 0375 626a 6401 0000 2981 947d 9428  .h.ubjd...)..}.(
-00002830: 6805 6806 6807 5d94 286a 6901 0000 2981  h.h.h.].(ji...).
-00002840: 947d 9428 6805 6806 6807 5d94 286a 6e01  .}.(h.h.h.].(jn.
-00002850: 0000 2981 947d 9428 6805 8c0a 5061 7261  ..)..}.(h...Para
-00002860: 6d65 7465 7273 9468 075d 9468 168c 0a50  meters.h.].h...P
-00002870: 6172 616d 6574 6572 7394 8594 8194 7d94  arameters.....}.
-00002880: 2868 1b6a ea03 0000 681c 6803 681d 4e68  (h.j....h.h.h.Nh
-00002890: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
-000028a0: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
-000028b0: 2b6a 6d01 0000 681b 6ae7 0300 0068 1d68  +jm...h.j....h.h
-000028c0: 2c68 1e4b 0075 626a 7e01 0000 2981 947d  ,h.K.ubj~...)..}
-000028d0: 9428 6805 6806 6807 5d94 686b 2981 947d  .(h.h.h.].hk)..}
-000028e0: 9428 6805 6806 6807 5d94 2868 7029 8194  .(h.h.h.].(hp)..
-000028f0: 7d94 2868 0568 0668 075d 9468 2e29 8194  }.(h.h.h.].h.)..
-00002900: 7d94 2868 058c 8a6c 616e 6775 6167 6520  }.(h...language 
-00002910: 2873 7472 2920 2d2d 2054 6865 2073 686f  (str) -- The sho
-00002920: 7274 666f 726d 206f 6620 6120 7375 7070  rtform of a supp
-00002930: 6f72 7465 6420 7072 6f67 7261 6d6d 696e  orted programmin
-00002940: 6720 6c61 6e67 7561 6765 2e20 5265 6665  g language. Refe
-00002950: 7220 746f 2074 6865 203a 646f 633a 206c  r to the :doc: l
-00002960: 6973 7420 6f66 2073 7570 706f 7274 6564  ist of supported
-00002970: 206c 616e 6775 6167 6573 203c 7375 7070   languages <supp
-00002980: 6f72 7465 645f 6c61 6e67 7561 6765 733e  orted_languages>
-00002990: 2e94 6807 5d94 286a 8d01 0000 2981 947d  ..h.].(j....)..}
-000029a0: 9428 6805 8c08 6c61 6e67 7561 6765 9468  .(h...language.h
-000029b0: 075d 9468 168c 086c 616e 6775 6167 6594  .].h...language.
-000029c0: 8594 8194 7d94 2868 1b6a 0504 0000 681c  ....}.(h.j....h.
-000029d0: 6803 681d 4e68 1e4e 7562 6168 1f7d 9428  h.h.Nh.Nubah.}.(
-000029e0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-000029f0: 6829 5d94 7568 2b6a 8c01 0000 681b 6a01  h)].uh+j....h.j.
-00002a00: 0400 0075 6268 168c 0220 2894 8594 8194  ...ubh... (.....
-00002a10: 7d94 2868 1b6a 0104 0000 681c 6803 681d  }.(h.j....h.h.h.
-00002a20: 4e68 1e4e 7562 6aa1 0100 0029 8194 7d94  Nh.Nubj....)..}.
-00002a30: 2868 0568 0668 075d 946a a601 0000 2981  (h.h.h.].j....).
-00002a40: 947d 9428 6805 8c03 7374 7294 6807 5d94  .}.(h...str.h.].
-00002a50: 6816 8c03 7374 7294 8594 8194 7d94 2868  h...str.....}.(h
-00002a60: 1b6a 1a04 0000 681c 6803 681d 4e68 1e4e  .j....h.h.h.Nh.N
-00002a70: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
-00002a80: 6825 5d94 6827 5d94 6829 5d94 7568 2b6a  h%].h'].h)].uh+j
-00002a90: a501 0000 681b 6a17 0400 0075 6261 681f  ....h.j....ubah.
-00002aa0: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-00002ab0: 275d 9468 295d 948c 0972 6566 646f 6d61  '].h)]...refdoma
-00002ac0: 696e 948c 0270 7994 8c0b 7265 6665 7870  in...py...refexp
-00002ad0: 6c69 6369 7494 898c 0772 6566 7479 7065  licit....reftype
-00002ae0: 946a bf01 0000 8c09 7265 6674 6172 6765  .j......reftarge
-00002af0: 7494 6a1c 0400 006a c101 0000 886a c201  t.j....j.....j..
-00002b00: 0000 4e6a c301 0000 4e75 682b 6aa0 0100  ..Nj....Nuh+j...
-00002b10: 0068 1b6a 0104 0000 7562 6816 8c01 2994  .h.j....ubh...).
-00002b20: 8594 8194 7d94 2868 1b6a 0104 0000 681c  ....}.(h.j....h.
-00002b30: 6803 681d 4e68 1e4e 7562 6816 8c05 20e2  h.h.Nh.Nubh... .
-00002b40: 8093 2094 8594 8194 7d94 2868 1b6a 0104  .. .....}.(h.j..
-00002b50: 0000 681c 6803 681d 4e68 1e4e 7562 6816  ..h.h.h.Nh.Nubh.
-00002b60: 8c46 5468 6520 7368 6f72 7466 6f72 6d20  .FThe shortform 
-00002b70: 6f66 2061 2073 7570 706f 7274 6564 2070  of a supported p
-00002b80: 726f 6772 616d 6d69 6e67 206c 616e 6775  rogramming langu
-00002b90: 6167 652e 2052 6566 6572 2074 6f20 7468  age. Refer to th
-00002ba0: 6520 3a64 6f63 3a20 9485 9481 947d 9428  e :doc: .....}.(
-00002bb0: 681b 6a01 0400 0068 1c68 0368 1d4e 681e  h.j....h.h.h.Nh.
-00002bc0: 4e75 6268 7929 8194 7d94 2868 058c 3360  Nubhy)..}.(h..3`
-00002bd0: 6c69 7374 206f 6620 7375 7070 6f72 7465  list of supporte
-00002be0: 6420 6c61 6e67 7561 6765 7320 3c73 7570  d languages <sup
-00002bf0: 706f 7274 6564 5f6c 616e 6775 6167 6573  ported_languages
-00002c00: 3e60 9468 075d 9468 168c 316c 6973 7420  >`.h.].h..1list 
-00002c10: 6f66 2073 7570 706f 7274 6564 206c 616e  of supported lan
-00002c20: 6775 6167 6573 203c 7375 7070 6f72 7465  guages <supporte
-00002c30: 645f 6c61 6e67 7561 6765 733e 9485 9481  d_languages>....
-00002c40: 947d 9428 681b 6a3f 0400 0068 1c68 0368  .}.(h.j?...h.h.h
-00002c50: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
-00002c60: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-00002c70: 9475 682b 6878 681b 6a01 0400 0068 1c68  .uh+hxh.j....h.h
-00002c80: 0368 1d4e 681e 4e75 6268 168c 012e 9485  .h.Nh.Nubh......
-00002c90: 9481 947d 9428 681b 6a01 0400 0068 1c68  ...}.(h.j....h.h
-00002ca0: 0368 1d4e 681e 4e75 6265 681f 7d94 2868  .h.Nh.Nubeh.}.(h
-00002cb0: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-00002cc0: 295d 9475 682b 682d 681b 6afe 0300 0075  )].uh+h-h.j....u
-00002cd0: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-00002ce0: 255d 9468 275d 9468 295d 9475 682b 686f  %].h'].h)].uh+ho
-00002cf0: 681b 6afb 0300 0075 6268 7029 8194 7d94  h.j....ubhp)..}.
-00002d00: 2868 0568 0668 075d 9468 2e29 8194 7d94  (h.h.h.].h.)..}.
-00002d10: 2868 058c 4c70 726f 6a65 6374 6e61 6d65  (h..Lprojectname
-00002d20: 2028 7374 7229 202d 2d20 5468 6520 6e61   (str) -- The na
-00002d30: 6d65 206f 6620 7468 6520 7072 6f6a 6563  me of the projec
-00002d40: 7420 6f72 2070 6163 6b61 6765 2079 6f75  t or package you
-00002d50: 2077 616e 7420 746f 2076 616c 6964 6174   want to validat
-00002d60: 6594 6807 5d94 286a 8d01 0000 2981 947d  e.h.].(j....)..}
-00002d70: 9428 6805 8c0b 7072 6f6a 6563 746e 616d  .(h...projectnam
-00002d80: 6594 6807 5d94 6816 8c0b 7072 6f6a 6563  e.h.].h...projec
-00002d90: 746e 616d 6594 8594 8194 7d94 2868 1b6a  tname.....}.(h.j
-00002da0: 6404 0000 681c 6803 681d 4e68 1e4e 7562  d...h.h.h.Nh.Nub
-00002db0: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
-00002dc0: 5d94 6827 5d94 6829 5d94 7568 2b6a 8c01  ].h'].h)].uh+j..
-00002dd0: 0000 681b 6a60 0400 0075 6268 168c 0220  ..h.j`...ubh... 
-00002de0: 2894 8594 8194 7d94 2868 1b6a 6004 0000  (.....}.(h.j`...
-00002df0: 681c 6803 681d 4e68 1e4e 7562 6aa1 0100  h.h.h.Nh.Nubj...
-00002e00: 0029 8194 7d94 2868 0568 0668 075d 946a  .)..}.(h.h.h.].j
-00002e10: a601 0000 2981 947d 9428 6805 8c03 7374  ....)..}.(h...st
-00002e20: 7294 6807 5d94 6816 8c03 7374 7294 8594  r.h.].h...str...
-00002e30: 8194 7d94 2868 1b6a 7904 0000 681c 6803  ..}.(h.jy...h.h.
-00002e40: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
-00002e50: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-00002e60: 5d94 7568 2b6a a501 0000 681b 6a76 0400  ].uh+j....h.jv..
-00002e70: 0075 6261 681f 7d94 2868 215d 9468 235d  .ubah.}.(h!].h#]
-00002e80: 9468 255d 9468 275d 9468 295d 948c 0972  .h%].h'].h)]...r
-00002e90: 6566 646f 6d61 696e 946a 2f04 0000 8c0b  efdomain.j/.....
-00002ea0: 7265 6665 7870 6c69 6369 7494 898c 0772  refexplicit....r
-00002eb0: 6566 7479 7065 946a bf01 0000 8c09 7265  eftype.j......re
-00002ec0: 6674 6172 6765 7494 6a7b 0400 006a c101  ftarget.j{...j..
-00002ed0: 0000 886a c201 0000 4e6a c301 0000 4e75  ...j....Nj....Nu
-00002ee0: 682b 6aa0 0100 0068 1b6a 6004 0000 7562  h+j....h.j`...ub
-00002ef0: 6816 8c01 2994 8594 8194 7d94 2868 1b6a  h...).....}.(h.j
-00002f00: 6004 0000 681c 6803 681d 4e68 1e4e 7562  `...h.h.h.Nh.Nub
-00002f10: 6816 8c05 20e2 8093 2094 8594 8194 7d94  h... ... .....}.
-00002f20: 2868 1b6a 6004 0000 681c 6803 681d 4e68  (h.j`...h.h.h.Nh
-00002f30: 1e4e 7562 6816 8c37 5468 6520 6e61 6d65  .Nubh..7The name
-00002f40: 206f 6620 7468 6520 7072 6f6a 6563 7420   of the project 
-00002f50: 6f72 2070 6163 6b61 6765 2079 6f75 2077  or package you w
-00002f60: 616e 7420 746f 2076 616c 6964 6174 6594  ant to validate.
-00002f70: 8594 8194 7d94 2868 1b6a 6004 0000 681c  ....}.(h.j`...h.
-00002f80: 6803 681d 4e68 1e4e 7562 6568 1f7d 9428  h.h.Nh.Nubeh.}.(
-00002f90: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-00002fa0: 6829 5d94 7568 2b68 2d68 1b6a 5d04 0000  h)].uh+h-h.j]...
-00002fb0: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
-00002fc0: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
-00002fd0: 6f68 1b6a fb03 0000 7562 6568 1f7d 9428  oh.j....ubeh.}.(
-00002fe0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-00002ff0: 6829 5d94 7568 2b68 6a68 1b6a f803 0000  h)].uh+hjh.j....
-00003000: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
-00003010: 6825 5d94 6827 5d94 6829 5d94 7568 2b6a  h%].h'].h)].uh+j
-00003020: 7d01 0000 681b 6ae7 0300 0075 6265 681f  }...h.j....ubeh.
-00003030: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-00003040: 275d 9468 295d 9475 682b 6a68 0100 0068  '].h)].uh+jh...h
-00003050: 1b6a e403 0000 7562 6a69 0100 0029 8194  .j....ubji...)..
-00003060: 7d94 2868 0568 0668 075d 9428 6a6e 0100  }.(h.h.h.].(jn..
-00003070: 0029 8194 7d94 2868 058c 0752 6574 7572  .)..}.(h...Retur
-00003080: 6e73 9468 075d 9468 168c 0752 6574 7572  ns.h.].h...Retur
-00003090: 6e73 9485 9481 947d 9428 681b 6abe 0400  ns.....}.(h.j...
-000030a0: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
-000030b0: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-000030c0: 275d 9468 295d 9475 682b 6a6d 0100 0068  '].h)].uh+jm...h
-000030d0: 1b6a bb04 0000 681d 682c 681e 4b00 7562  .j....h.h,h.K.ub
-000030e0: 6a7e 0100 0029 8194 7d94 2868 0568 0668  j~...)..}.(h.h.h
-000030f0: 075d 9468 2e29 8194 7d94 2868 058c 3d54  .].h.)..}.(h..=T
-00003100: 656c 6c73 2079 6f75 2076 6961 2054 6572  ells you via Ter
-00003110: 6d69 6e61 6c20 7765 7468 6572 2079 6f75  minal wether you
-00003120: 7220 7374 7275 6374 7572 6520 6c69 6e65  r structure line
-00003130: 7320 7570 206f 7220 6e6f 742e 9468 075d  s up or not..h.]
-00003140: 9468 168c 3d54 656c 6c73 2079 6f75 2076  .h..=Tells you v
-00003150: 6961 2054 6572 6d69 6e61 6c20 7765 7468  ia Terminal weth
-00003160: 6572 2079 6f75 7220 7374 7275 6374 7572  er your structur
-00003170: 6520 6c69 6e65 7320 7570 206f 7220 6e6f  e lines up or no
-00003180: 742e 9485 9481 947d 9428 681b 6acf 0400  t......}.(h.j...
-00003190: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
-000031a0: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-000031b0: 275d 9468 295d 9475 682b 682d 681b 6acc  '].h)].uh+h-h.j.
-000031c0: 0400 0075 6261 681f 7d94 2868 215d 9468  ...ubah.}.(h!].h
-000031d0: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
-000031e0: 682b 6a7d 0100 0068 1b6a bb04 0000 7562  h+j}...h.j....ub
-000031f0: 6568 1f7d 9428 6821 5d94 6823 5d94 6825  eh.}.(h!].h#].h%
-00003200: 5d94 6827 5d94 6829 5d94 7568 2b6a 6801  ].h'].h)].uh+jh.
-00003210: 0000 681b 6ae4 0300 0075 626a 6901 0000  ..h.j....ubji...
-00003220: 2981 947d 9428 6805 6806 6807 5d94 286a  )..}.(h.h.h.].(j
-00003230: 6e01 0000 2981 947d 9428 6805 8c0b 5265  n...)..}.(h...Re
-00003240: 7475 726e 2074 7970 6594 6807 5d94 6816  turn type.h.].h.
-00003250: 8c0b 5265 7475 726e 2074 7970 6594 8594  ..Return type...
-00003260: 8194 7d94 2868 1b6a ec04 0000 681c 6803  ..}.(h.j....h.h.
-00003270: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
-00003280: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-00003290: 5d94 7568 2b6a 6d01 0000 681b 6ae9 0400  ].uh+jm...h.j...
-000032a0: 0068 1d68 2c68 1e4b 0075 626a 7e01 0000  .h.h,h.K.ubj~...
-000032b0: 2981 947d 9428 6805 6806 6807 5d94 682e  )..}.(h.h.h.].h.
-000032c0: 2981 947d 9428 6805 8c03 7374 7294 6807  )..}.(h...str.h.
-000032d0: 5d94 6aa1 0100 0029 8194 7d94 2868 0568  ].j....)..}.(h.h
-000032e0: 0668 075d 9468 168c 0373 7472 9485 9481  .h.].h...str....
-000032f0: 947d 9428 681b 6a01 0500 0068 1c68 0368  .}.(h.j....h.h.h
-00003300: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
-00003310: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-00003320: 948c 0972 6566 646f 6d61 696e 946a 2f04  ...refdomain.j/.
-00003330: 0000 8c0b 7265 6665 7870 6c69 6369 7494  ....refexplicit.
-00003340: 898c 0772 6566 7479 7065 946a bf01 0000  ...reftype.j....
-00003350: 8c09 7265 6674 6172 6765 7494 8c03 7374  ..reftarget...st
-00003360: 7294 6ac1 0100 0088 6ac2 0100 004e 6ac3  r.j.....j....Nj.
-00003370: 0100 004e 7568 2b6a a001 0000 681b 6afd  ...Nuh+j....h.j.
-00003380: 0400 0075 6261 681f 7d94 2868 215d 9468  ...ubah.}.(h!].h
-00003390: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
-000033a0: 682b 682d 681b 6afa 0400 0075 6261 681f  h+h-h.j....ubah.
-000033b0: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-000033c0: 275d 9468 295d 9475 682b 6a7d 0100 0068  '].h)].uh+j}...h
-000033d0: 1b6a e904 0000 7562 6568 1f7d 9428 6821  .j....ubeh.}.(h!
-000033e0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-000033f0: 5d94 7568 2b6a 6801 0000 681b 6ae4 0300  ].uh+jh...h.j...
-00003400: 0075 6265 681f 7d94 2868 215d 9468 235d  .ubeh.}.(h!].h#]
-00003410: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
-00003420: 6a63 0100 0068 1b6a c103 0000 681c 6803  jc...h.j....h.h.
-00003430: 681d 4e68 1e4e 7562 6568 1f7d 9428 6821  h.Nh.Nubeh.}.(h!
-00003440: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-00003450: 5d94 7568 2b6a 5001 0000 681b 6aa7 0300  ].uh+jP...h.j...
-00003460: 0068 1c68 0368 1d68 2c68 1e4b 2d75 6265  .h.h.h.h,h.K-ube
-00003470: 681f 7d94 2868 215d 9468 235d 9428 6a2f  h.}.(h!].h#].(j/
-00003480: 0400 008c 0866 756e 6374 696f 6e94 6568  .....function.eh
-00003490: 255d 9468 275d 9468 295d 946a 7d03 0000  %].h'].h)].j}...
-000034a0: 6a2f 0400 006a 7e03 0000 6a34 0500 006a  j/...j~...j4...j
-000034b0: 7f03 0000 6a34 0500 006a 8003 0000 896a  ....j4...j.....j
-000034c0: 8103 0000 896a 8203 0000 8975 682b 6a28  .....j.....uh+j(
-000034d0: 0100 0068 1c68 0368 1b6a 8b03 0000 681d  ...h.h.h.j....h.
-000034e0: 4e68 1e4e 7562 6568 1f7d 9428 6821 5d94  Nh.Nubeh.}.(h!].
-000034f0: 8c0f 6e65 7374 6572 2d76 616c 6964 6174  ..nester-validat
-00003500: 6594 6168 235d 9468 255d 948c 0f6e 6573  e.ah#].h%]...nes
-00003510: 7465 7220 7661 6c69 6461 7465 9461 6827  ter validate.ah'
-00003520: 5d94 6829 5d94 7568 2b68 0a68 1b68 4b68  ].h)].uh+h.h.hKh
-00003530: 1c68 0368 1d68 2c68 1e4b 2b75 6268 0b29  .h.h.h,h.K+ubh.)
-00003540: 8194 7d94 2868 0568 0668 075d 9428 6810  ..}.(h.h.h.].(h.
-00003550: 2981 947d 9428 6805 8c0b 4e65 7374 6572  )..}.(h...Nester
-00003560: 206c 6973 7494 6807 5d94 6816 8c0b 4e65   list.h.].h...Ne
-00003570: 7374 6572 206c 6973 7494 8594 8194 7d94  ster list.....}.
-00003580: 2868 1b6a 4305 0000 681c 6803 681d 4e68  (h.jC...h.h.h.Nh
-00003590: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
-000035a0: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
-000035b0: 2b68 0f68 1b6a 4005 0000 681c 6803 681d  +h.h.j@...h.h.h.
-000035c0: 682c 681e 4b3a 7562 6a1c 0100 0029 8194  h,h.K:ubj....)..
-000035d0: 7d94 2868 0568 0668 075d 9468 1f7d 9428  }.(h.h.h.].h.}.(
-000035e0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-000035f0: 6829 5d94 8c07 656e 7472 6965 7394 5d94  h)]...entries.].
-00003600: 7568 2b6a 1b01 0000 681b 6a40 0500 0068  uh+j....h.j@...h
-00003610: 1c68 0368 1d4e 681e 4e75 626a 2901 0000  .h.h.Nh.Nubj)...
-00003620: 2981 947d 9428 6805 6806 6807 5d94 286a  )..}.(h.h.h.].(j
-00003630: 2e01 0000 2981 947d 9428 6805 8c0d 6e65  ....)..}.(h...ne
-00003640: 7374 6572 206c 6973 7428 2994 6807 5d94  ster list().h.].
-00003650: 6a34 0100 0029 8194 7d94 2868 056a 6105  j4...)..}.(h.ja.
-00003660: 0000 6807 5d94 6816 8c0d 6e65 7374 6572  ..h.].h...nester
-00003670: 206c 6973 7428 2994 8594 8194 7d94 2868   list().....}.(h
-00003680: 1b6a 6305 0000 681c 6803 681d 4e68 1e4e  .jc...h.h.h.Nh.N
-00003690: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
-000036a0: 286a 3f01 0000 6a40 0100 0065 6825 5d94  (j?...j@...eh%].
-000036b0: 6827 5d94 6829 5d94 6a44 0100 006a 4501  h'].h)].jD...jE.
-000036c0: 0000 7568 2b6a 3301 0000 681b 6a5f 0500  ..uh+j3...h.j_..
-000036d0: 0068 1c68 0368 1d68 2c68 1e4b 3c75 6261  .h.h.h.h,h.K<uba
-000036e0: 681f 7d94 2868 215d 9468 235d 9428 6a49  h.}.(h!].h#].(jI
-000036f0: 0100 006a 4a01 0000 6568 255d 9468 275d  ...jJ...eh%].h']
-00003700: 9468 295d 946a 4e01 0000 296a 4f01 0000  .h)].jN...)jO...
-00003710: 6806 7568 2b6a 2d01 0000 681d 682c 681e  h.uh+j-...h.h,h.
-00003720: 4b3c 681b 6a5c 0500 0068 1c68 0375 626a  K<h.j\...h.h.ubj
-00003730: 2e01 0000 2981 947d 9428 6805 8c4d 4c69  ....)..}.(h..MLi
-00003740: 7374 7320 616c 6c20 7072 6576 696f 7573  sts all previous
-00003750: 6c79 2063 7265 6174 6564 2070 726f 6a65  ly created proje
-00003760: 6374 732c 2077 6869 6368 2068 6164 206c  cts, which had l
-00003770: 6f67 6769 6e67 2065 6e61 626c 6564 2c20  ogging enabled, 
-00003780: 696e 2061 2074 6162 6c65 2e94 6807 5d94  in a table..h.].
-00003790: 6a34 0100 0029 8194 7d94 2868 056a 7805  j4...)..}.(h.jx.
-000037a0: 0000 6807 5d94 6816 8c4d 4c69 7374 7320  ..h.].h..MLists 
-000037b0: 616c 6c20 7072 6576 696f 7573 6c79 2063  all previously c
-000037c0: 7265 6174 6564 2070 726f 6a65 6374 732c  reated projects,
-000037d0: 2077 6869 6368 2068 6164 206c 6f67 6769   which had loggi
-000037e0: 6e67 2065 6e61 626c 6564 2c20 696e 2061  ng enabled, in a
-000037f0: 2074 6162 6c65 2e94 8594 8194 7d94 2868   table......}.(h
-00003800: 1b6a 7a05 0000 681c 6803 681d 4e68 1e4e  .jz...h.h.h.Nh.N
-00003810: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
-00003820: 286a 3f01 0000 6a40 0100 0065 6825 5d94  (j?...j@...eh%].
-00003830: 6827 5d94 6829 5d94 6a44 0100 006a 4501  h'].h)].jD...jE.
-00003840: 0000 7568 2b6a 3301 0000 681b 6a76 0500  ..uh+j3...h.jv..
-00003850: 0068 1c68 0368 1d68 2c68 1e4b 3c75 6261  .h.h.h.h,h.K<uba
-00003860: 681f 7d94 2868 215d 9468 235d 9428 6a49  h.}.(h!].h#].(jI
-00003870: 0100 006a 4a01 0000 6568 255d 9468 275d  ...jJ...eh%].h']
-00003880: 9468 295d 946a 4e01 0000 296a 4f01 0000  .h)].jN...)jO...
-00003890: 6806 7568 2b6a 2d01 0000 681d 682c 681e  h.uh+j-...h.h,h.
-000038a0: 4b3c 681b 6a5c 0500 0068 1c68 0375 626a  K<h.j\...h.h.ubj
-000038b0: 5101 0000 2981 947d 9428 6805 6806 6807  Q...)..}.(h.h.h.
-000038c0: 5d94 6a64 0100 0029 8194 7d94 2868 0568  ].jd...)..}.(h.h
-000038d0: 0668 075d 9428 6a69 0100 0029 8194 7d94  .h.].(ji...)..}.
-000038e0: 2868 0568 0668 075d 9428 6a6e 0100 0029  (h.h.h.].(jn...)
-000038f0: 8194 7d94 2868 058c 0a50 6172 616d 6574  ..}.(h...Paramet
-00003900: 6572 7394 6807 5d94 6816 8c0a 5061 7261  ers.h.].h...Para
-00003910: 6d65 7465 7273 9485 9481 947d 9428 681b  meters.....}.(h.
-00003920: 6a96 0500 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
-00003930: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-00003940: 255d 9468 275d 9468 295d 9475 682b 6a6d  %].h'].h)].uh+jm
-00003950: 0100 0068 1b6a 9305 0000 681d 682c 681e  ...h.j....h.h,h.
-00003960: 4b00 7562 6a7e 0100 0029 8194 7d94 2868  K.ubj~...)..}.(h
-00003970: 0568 0668 075d 9468 2e29 8194 7d94 2868  .h.h.].h.)..}.(h
-00003980: 058c 442d 2d63 6c65 616e 2028 666c 6167  ..D--clean (flag
-00003990: 2920 2d2d 2041 6e20 6f70 7469 6f6e 616c  ) -- An optional
-000039a0: 2066 6c61 6720 746f 2063 6c65 616e 2075   flag to clean u
-000039b0: 7020 6f72 7068 616e 6564 206c 6f67 2065  p orphaned log e
-000039c0: 6e74 7269 6573 2e94 6807 5d94 286a 8d01  ntries..h.].(j..
-000039d0: 0000 2981 947d 9428 6805 8c07 2d2d 636c  ..)..}.(h...--cl
-000039e0: 6561 6e94 6807 5d94 6816 8c07 2d2d 636c  ean.h.].h...--cl
-000039f0: 6561 6e94 8594 8194 7d94 2868 1b6a ab05  ean.....}.(h.j..
-00003a00: 0000 681c 6803 681d 4e68 1e4e 7562 6168  ..h.h.h.Nh.Nubah
-00003a10: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
-00003a20: 6827 5d94 6829 5d94 7568 2b6a 8c01 0000  h'].h)].uh+j....
-00003a30: 681b 6aa7 0500 0075 6268 168c 0220 2894  h.j....ubh... (.
-00003a40: 8594 8194 7d94 2868 1b6a a705 0000 681c  ....}.(h.j....h.
-00003a50: 6803 681d 4e68 1e4e 7562 6aa1 0100 0029  h.h.Nh.Nubj....)
-00003a60: 8194 7d94 2868 0568 0668 075d 946a a601  ..}.(h.h.h.].j..
-00003a70: 0000 2981 947d 9428 6805 8c04 666c 6167  ..)..}.(h...flag
-00003a80: 9468 075d 9468 168c 0466 6c61 6794 8594  .h.].h...flag...
-00003a90: 8194 7d94 2868 1b6a c005 0000 681c 6803  ..}.(h.j....h.h.
-00003aa0: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
-00003ab0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-00003ac0: 5d94 7568 2b6a a501 0000 681b 6abd 0500  ].uh+j....h.j...
-00003ad0: 0075 6261 681f 7d94 2868 215d 9468 235d  .ubah.}.(h!].h#]
-00003ae0: 9468 255d 9468 275d 9468 295d 948c 0972  .h%].h'].h)]...r
-00003af0: 6566 646f 6d61 696e 948c 0270 7994 8c0b  efdomain...py...
-00003b00: 7265 6665 7870 6c69 6369 7494 898c 0772  refexplicit....r
-00003b10: 6566 7479 7065 946a bf01 0000 8c09 7265  eftype.j......re
-00003b20: 6674 6172 6765 7494 6ac2 0500 006a c101  ftarget.j....j..
-00003b30: 0000 886a c201 0000 4e6a c301 0000 4e75  ...j....Nj....Nu
-00003b40: 682b 6aa0 0100 0068 1b6a a705 0000 7562  h+j....h.j....ub
-00003b50: 6816 8c01 2994 8594 8194 7d94 2868 1b6a  h...).....}.(h.j
-00003b60: a705 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
-00003b70: 6816 8c05 20e2 8093 2094 8594 8194 7d94  h... ... .....}.
-00003b80: 2868 1b6a a705 0000 681c 6803 681d 4e68  (h.j....h.h.h.Nh
-00003b90: 1e4e 7562 6816 8c32 416e 206f 7074 696f  .Nubh..2An optio
-00003ba0: 6e61 6c20 666c 6167 2074 6f20 636c 6561  nal flag to clea
-00003bb0: 6e20 7570 206f 7270 6861 6e65 6420 6c6f  n up orphaned lo
-00003bc0: 6720 656e 7472 6965 732e 9485 9481 947d  g entries......}
-00003bd0: 9428 681b 6aa7 0500 0068 1c68 0368 1d4e  .(h.j....h.h.h.N
-00003be0: 681e 4e75 6265 681f 7d94 2868 215d 9468  h.Nubeh.}.(h!].h
-00003bf0: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
-00003c00: 682b 682d 681b 6aa4 0500 0075 6261 681f  h+h-h.j....ubah.
-00003c10: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-00003c20: 275d 9468 295d 9475 682b 6a7d 0100 0068  '].h)].uh+j}...h
-00003c30: 1b6a 9305 0000 7562 6568 1f7d 9428 6821  .j....ubeh.}.(h!
-00003c40: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-00003c50: 5d94 7568 2b6a 6801 0000 681b 6a90 0500  ].uh+jh...h.j...
-00003c60: 0075 626a 6901 0000 2981 947d 9428 6805  .ubji...)..}.(h.
-00003c70: 6806 6807 5d94 286a 6e01 0000 2981 947d  h.h.].(jn...)..}
-00003c80: 9428 6805 8c07 5265 7475 726e 7394 6807  .(h...Returns.h.
-00003c90: 5d94 6816 8c07 5265 7475 726e 7394 8594  ].h...Returns...
-00003ca0: 8194 7d94 2868 1b6a fa05 0000 681c 6803  ..}.(h.j....h.h.
-00003cb0: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
-00003cc0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-00003cd0: 5d94 7568 2b6a 6d01 0000 681b 6af7 0500  ].uh+jm...h.j...
-00003ce0: 0068 1d68 2c68 1e4b 0075 626a 7e01 0000  .h.h,h.K.ubj~...
-00003cf0: 2981 947d 9428 6805 6806 6807 5d94 682e  )..}.(h.h.h.].h.
-00003d00: 2981 947d 9428 6805 8c04 4e6f 6e65 9468  )..}.(h...None.h
-00003d10: 075d 9468 168c 044e 6f6e 6594 8594 8194  .].h...None.....
-00003d20: 7d94 2868 1b6a 0b06 0000 681c 6803 681d  }.(h.j....h.h.h.
-00003d30: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
-00003d40: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-00003d50: 7568 2b68 2d68 1b6a 0806 0000 7562 6168  uh+h-h.j....ubah
-00003d60: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
-00003d70: 6827 5d94 6829 5d94 7568 2b6a 7d01 0000  h'].h)].uh+j}...
-00003d80: 681b 6af7 0500 0075 6265 681f 7d94 2868  h.j....ubeh.}.(h
-00003d90: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-00003da0: 295d 9475 682b 6a68 0100 0068 1b6a 9005  )].uh+jh...h.j..
-00003db0: 0000 7562 6a69 0100 0029 8194 7d94 2868  ..ubji...)..}.(h
-00003dc0: 0568 0668 075d 9428 6a6e 0100 0029 8194  .h.h.].(jn...)..
-00003dd0: 7d94 2868 058c 0b52 6574 7572 6e20 7479  }.(h...Return ty
-00003de0: 7065 9468 075d 9468 168c 0b52 6574 7572  pe.h.].h...Retur
-00003df0: 6e20 7479 7065 9485 9481 947d 9428 681b  n type.....}.(h.
-00003e00: 6a28 0600 0068 1c68 0368 1d4e 681e 4e75  j(...h.h.h.Nh.Nu
-00003e10: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-00003e20: 255d 9468 275d 9468 295d 9475 682b 6a6d  %].h'].h)].uh+jm
-00003e30: 0100 0068 1b6a 2506 0000 681d 682c 681e  ...h.j%...h.h,h.
-00003e40: 4b00 7562 6a7e 0100 0029 8194 7d94 2868  K.ubj~...)..}.(h
-00003e50: 0568 0668 075d 9468 2e29 8194 7d94 2868  .h.h.].h.)..}.(h
-00003e60: 058c 044e 6f6e 6594 6807 5d94 6aa1 0100  ...None.h.].j...
-00003e70: 0029 8194 7d94 2868 0568 0668 075d 9468  .)..}.(h.h.h.].h
-00003e80: 168c 044e 6f6e 6594 8594 8194 7d94 2868  ...None.....}.(h
-00003e90: 1b6a 3d06 0000 681c 6803 681d 4e68 1e4e  .j=...h.h.h.Nh.N
-00003ea0: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
-00003eb0: 6825 5d94 6827 5d94 6829 5d94 8c09 7265  h%].h'].h)]...re
-00003ec0: 6664 6f6d 6169 6e94 6ad5 0500 008c 0b72  fdomain.j......r
-00003ed0: 6566 6578 706c 6963 6974 9489 8c07 7265  efexplicit....re
-00003ee0: 6674 7970 6594 6abf 0100 008c 0972 6566  ftype.j......ref
-00003ef0: 7461 7267 6574 948c 044e 6f6e 6594 6ac1  target...None.j.
-00003f00: 0100 0088 6ac2 0100 004e 6ac3 0100 004e  ....j....Nj....N
-00003f10: 7568 2b6a a001 0000 681b 6a39 0600 0075  uh+j....h.j9...u
-00003f20: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-00003f30: 255d 9468 275d 9468 295d 9475 682b 682d  %].h'].h)].uh+h-
-00003f40: 681b 6a36 0600 0075 6261 681f 7d94 2868  h.j6...ubah.}.(h
-00003f50: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-00003f60: 295d 9475 682b 6a7d 0100 0068 1b6a 2506  )].uh+j}...h.j%.
-00003f70: 0000 7562 6568 1f7d 9428 6821 5d94 6823  ..ubeh.}.(h!].h#
-00003f80: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
-00003f90: 2b6a 6801 0000 681b 6a90 0500 0075 6265  +jh...h.j....ube
-00003fa0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-00003fb0: 9468 275d 9468 295d 9475 682b 6a63 0100  .h'].h)].uh+jc..
-00003fc0: 0068 1b6a 8d05 0000 681c 6803 681d 4e68  .h.j....h.h.h.Nh
-00003fd0: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
-00003fe0: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
-00003ff0: 2b6a 5001 0000 681b 6a5c 0500 0068 1c68  +jP...h.j\...h.h
-00004000: 0368 1d68 2c68 1e4b 3c75 6265 681f 7d94  .h.h,h.K<ubeh.}.
-00004010: 2868 215d 9468 235d 9428 6ad5 0500 008c  (h!].h#].(j.....
-00004020: 0866 756e 6374 696f 6e94 6568 255d 9468  .function.eh%].h
-00004030: 275d 9468 295d 946a 7d03 0000 6ad5 0500  '].h)].j}...j...
-00004040: 006a 7e03 0000 6a70 0600 006a 7f03 0000  .j~...jp...j....
-00004050: 6a70 0600 006a 8003 0000 896a 8103 0000  jp...j.....j....
-00004060: 896a 8203 0000 8975 682b 6a28 0100 0068  .j.....uh+j(...h
-00004070: 1c68 0368 1b6a 4005 0000 681d 4e68 1e4e  .h.h.j@...h.Nh.N
-00004080: 7562 6568 1f7d 9428 6821 5d94 8c0b 6e65  ubeh.}.(h!]...ne
-00004090: 7374 6572 2d6c 6973 7494 6168 235d 9468  ster-list.ah#].h
-000040a0: 255d 948c 0b6e 6573 7465 7220 6c69 7374  %]...nester list
-000040b0: 9461 6827 5d94 6829 5d94 7568 2b68 0a68  .ah'].h)].uh+h.h
-000040c0: 1b68 4b68 1c68 0368 1d68 2c68 1e4b 3a75  .hKh.h.h.h,h.K:u
-000040d0: 6268 0b29 8194 7d94 2868 0568 0668 075d  bh.)..}.(h.h.h.]
-000040e0: 9428 6810 2981 947d 9428 6805 8c0c 4e65  .(h.)..}.(h...Ne
-000040f0: 7374 6572 2063 6c65 616e 9468 075d 9468  ster clean.h.].h
-00004100: 168c 0c4e 6573 7465 7220 636c 6561 6e94  ...Nester clean.
-00004110: 8594 8194 7d94 2868 1b6a 7f06 0000 681c  ....}.(h.j....h.
-00004120: 6803 681d 4e68 1e4e 7562 6168 1f7d 9428  h.h.Nh.Nubah.}.(
-00004130: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-00004140: 6829 5d94 7568 2b68 0f68 1b6a 7c06 0000  h)].uh+h.h.j|...
-00004150: 681c 6803 681d 682c 681e 4b45 7562 6a1c  h.h.h.h,h.KEubj.
-00004160: 0100 0029 8194 7d94 2868 0568 0668 075d  ...)..}.(h.h.h.]
-00004170: 9468 1f7d 9428 6821 5d94 6823 5d94 6825  .h.}.(h!].h#].h%
-00004180: 5d94 6827 5d94 6829 5d94 8c07 656e 7472  ].h'].h)]...entr
-00004190: 6965 7394 5d94 7568 2b6a 1b01 0000 681b  ies.].uh+j....h.
-000041a0: 6a7c 0600 0068 1c68 0368 1d4e 681e 4e75  j|...h.h.h.Nh.Nu
-000041b0: 626a 2901 0000 2981 947d 9428 6805 6806  bj)...)..}.(h.h.
-000041c0: 6807 5d94 286a 2e01 0000 2981 947d 9428  h.].(j....)..}.(
-000041d0: 6805 8c25 6e65 7374 6572 2063 6c65 616e  h..%nester clean
-000041e0: 2870 726f 6a65 6374 6e61 6d65 2c20 5b2d  (projectname, [-
-000041f0: 797c 2d2d 7965 735d 2994 6807 5d94 6a34  y|--yes]).h.].j4
-00004200: 0100 0029 8194 7d94 2868 056a 9d06 0000  ...)..}.(h.j....
-00004210: 6807 5d94 6816 8c25 6e65 7374 6572 2063  h.].h..%nester c
-00004220: 6c65 616e 2870 726f 6a65 6374 6e61 6d65  lean(projectname
-00004230: 2c20 5b2d 797c 2d2d 7965 735d 2994 8594  , [-y|--yes])...
-00004240: 8194 7d94 2868 1b6a 9f06 0000 681c 6803  ..}.(h.j....h.h.
-00004250: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
-00004260: 5d94 6823 5d94 286a 3f01 0000 6a40 0100  ].h#].(j?...j@..
-00004270: 0065 6825 5d94 6827 5d94 6829 5d94 6a44  .eh%].h'].h)].jD
-00004280: 0100 006a 4501 0000 7568 2b6a 3301 0000  ...jE...uh+j3...
-00004290: 681b 6a9b 0600 0068 1c68 0368 1d68 2c68  h.j....h.h.h.h,h
-000042a0: 1e4b 4775 6261 681f 7d94 2868 215d 9468  .KGubah.}.(h!].h
-000042b0: 235d 9428 6a49 0100 006a 4a01 0000 6568  #].(jI...jJ...eh
-000042c0: 255d 9468 275d 9468 295d 946a 4e01 0000  %].h'].h)].jN...
-000042d0: 296a 4f01 0000 6806 7568 2b6a 2d01 0000  )jO...h.uh+j-...
-000042e0: 681d 682c 681e 4b47 681b 6a98 0600 0068  h.h,h.KGh.j....h
-000042f0: 1c68 0375 626a 5101 0000 2981 947d 9428  .h.ubjQ...)..}.(
-00004300: 6805 6806 6807 5d94 2868 2e29 8194 7d94  h.h.h.].(h.)..}.
-00004310: 2868 058c 3c44 656c 6574 6573 2074 6865  (h..<Deletes the
-00004320: 202a 656e 7469 7265 2a20 636f 6e74 656e   *entire* conten
-00004330: 7420 6f66 2074 6865 2067 6976 656e 2070  t of the given p
-00004340: 726f 6a65 6374 2064 6972 6563 746f 7279  roject directory
-00004350: 2e94 6807 5d94 2868 168c 0c44 656c 6574  ..h.].(h...Delet
-00004360: 6573 2074 6865 2094 8594 8194 7d94 2868  es the .....}.(h
-00004370: 1b6a b506 0000 681c 6803 681d 4e68 1e4e  .j....h.h.h.Nh.N
-00004380: 7562 6809 8c08 656d 7068 6173 6973 9493  ubh...emphasis..
-00004390: 9429 8194 7d94 2868 058c 082a 656e 7469  .)..}.(h...*enti
-000043a0: 7265 2a94 6807 5d94 6816 8c06 656e 7469  re*.h.].h...enti
-000043b0: 7265 9485 9481 947d 9428 681b 6abf 0600  re.....}.(h.j...
-000043c0: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
-000043d0: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-000043e0: 275d 9468 295d 9475 682b 6abd 0600 0068  '].h)].uh+j....h
-000043f0: 1b6a b506 0000 7562 6816 8c28 2063 6f6e  .j....ubh..( con
-00004400: 7465 6e74 206f 6620 7468 6520 6769 7665  tent of the give
-00004410: 6e20 7072 6f6a 6563 7420 6469 7265 6374  n project direct
-00004420: 6f72 792e 9485 9481 947d 9428 681b 6ab5  ory......}.(h.j.
-00004430: 0600 0068 1c68 0368 1d4e 681e 4e75 6265  ...h.h.h.Nh.Nube
-00004440: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-00004450: 9468 275d 9468 295d 9475 682b 682d 681d  .h'].h)].uh+h-h.
-00004460: 682c 681e 4b49 681b 6ab2 0600 0068 1c68  h,h.KIh.j....h.h
-00004470: 0375 6268 2e29 8194 7d94 2868 058c 2154  .ubh.)..}.(h..!T
-00004480: 6869 7320 6163 7469 6f6e 202a 2a63 616e  his action **can
-00004490: 6e6f 742a 2a20 6265 2075 6e64 6f6e 652e  not** be undone.
-000044a0: 9468 075d 9428 6816 8c0c 5468 6973 2061  .h.].(h...This a
-000044b0: 6374 696f 6e20 9485 9481 947d 9428 681b  ction .....}.(h.
-000044c0: 6ad7 0600 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
-000044d0: 6268 098c 0673 7472 6f6e 6794 9394 2981  bh...strong...).
-000044e0: 947d 9428 6805 8c0a 2a2a 6361 6e6e 6f74  .}.(h...**cannot
-000044f0: 2a2a 9468 075d 9468 168c 0663 616e 6e6f  **.h.].h...canno
-00004500: 7494 8594 8194 7d94 2868 1b6a e106 0000  t.....}.(h.j....
-00004510: 681c 6803 681d 4e68 1e4e 7562 6168 1f7d  h.h.h.Nh.Nubah.}
-00004520: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-00004530: 5d94 6829 5d94 7568 2b6a df06 0000 681b  ].h)].uh+j....h.
-00004540: 6ad7 0600 0075 6268 168c 0b20 6265 2075  j....ubh... be u
-00004550: 6e64 6f6e 652e 9485 9481 947d 9428 681b  ndone......}.(h.
-00004560: 6ad7 0600 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
-00004570: 6265 681f 7d94 2868 215d 9468 235d 9468  beh.}.(h!].h#].h
-00004580: 255d 9468 275d 9468 295d 9475 682b 682d  %].h'].h)].uh+h-
-00004590: 681d 682c 681e 4b4b 681b 6ab2 0600 0068  h.h,h.KKh.j....h
-000045a0: 1c68 0375 626a 6401 0000 2981 947d 9428  .h.ubjd...)..}.(
-000045b0: 6805 6806 6807 5d94 286a 6901 0000 2981  h.h.h.].(ji...).
-000045c0: 947d 9428 6805 6806 6807 5d94 286a 6e01  .}.(h.h.h.].(jn.
-000045d0: 0000 2981 947d 9428 6805 8c0a 5061 7261  ..)..}.(h...Para
-000045e0: 6d65 7465 7273 9468 075d 9468 168c 0a50  meters.h.].h...P
-000045f0: 6172 616d 6574 6572 7394 8594 8194 7d94  arameters.....}.
-00004600: 2868 1b6a ff06 0000 681c 6803 681d 4e68  (h.j....h.h.h.Nh
-00004610: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
-00004620: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
-00004630: 2b6a 6d01 0000 681b 6afc 0600 0068 1d68  +jm...h.j....h.h
-00004640: 2c68 1e4b 0075 626a 7e01 0000 2981 947d  ,h.K.ubj~...)..}
-00004650: 9428 6805 6806 6807 5d94 686b 2981 947d  .(h.h.h.].hk)..}
-00004660: 9428 6805 6806 6807 5d94 2868 7029 8194  .(h.h.h.].(hp)..
-00004670: 7d94 2868 0568 0668 075d 9468 2e29 8194  }.(h.h.h.].h.)..
-00004680: 7d94 2868 058c 4070 726f 6a65 6374 6e61  }.(h..@projectna
-00004690: 6d65 2028 7374 7229 202d 2d20 5468 6520  me (str) -- The 
-000046a0: 6e61 6d65 206f 6620 7468 6520 7072 6f6a  name of the proj
-000046b0: 6563 7420 796f 7520 7761 6e74 2074 6f20  ect you want to 
-000046c0: 6465 6c65 7465 2e94 6807 5d94 286a 8d01  delete..h.].(j..
-000046d0: 0000 2981 947d 9428 6805 8c0b 7072 6f6a  ..)..}.(h...proj
-000046e0: 6563 746e 616d 6594 6807 5d94 6816 8c0b  ectname.h.].h...
-000046f0: 7072 6f6a 6563 746e 616d 6594 8594 8194  projectname.....
-00004700: 7d94 2868 1b6a 1a07 0000 681c 6803 681d  }.(h.j....h.h.h.
-00004710: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
-00004720: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-00004730: 7568 2b6a 8c01 0000 681b 6a16 0700 0075  uh+j....h.j....u
-00004740: 6268 168c 0220 2894 8594 8194 7d94 2868  bh... (.....}.(h
-00004750: 1b6a 1607 0000 681c 6803 681d 4e68 1e4e  .j....h.h.h.Nh.N
-00004760: 7562 6aa1 0100 0029 8194 7d94 2868 0568  ubj....)..}.(h.h
-00004770: 0668 075d 946a a601 0000 2981 947d 9428  .h.].j....)..}.(
-00004780: 6805 8c03 7374 7294 6807 5d94 6816 8c03  h...str.h.].h...
-00004790: 7374 7294 8594 8194 7d94 2868 1b6a 2f07  str.....}.(h.j/.
-000047a0: 0000 681c 6803 681d 4e68 1e4e 7562 6168  ..h.h.h.Nh.Nubah
-000047b0: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
-000047c0: 6827 5d94 6829 5d94 7568 2b6a a501 0000  h'].h)].uh+j....
-000047d0: 681b 6a2c 0700 0075 6261 681f 7d94 2868  h.j,...ubah.}.(h
-000047e0: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-000047f0: 295d 948c 0972 6566 646f 6d61 696e 948c  )]...refdomain..
-00004800: 0270 7994 8c0b 7265 6665 7870 6c69 6369  .py...refexplici
-00004810: 7494 898c 0772 6566 7479 7065 946a bf01  t....reftype.j..
-00004820: 0000 8c09 7265 6674 6172 6765 7494 6a31  ....reftarget.j1
-00004830: 0700 006a c101 0000 886a c201 0000 4e6a  ...j.....j....Nj
-00004840: c301 0000 4e75 682b 6aa0 0100 0068 1b6a  ....Nuh+j....h.j
-00004850: 1607 0000 7562 6816 8c01 2994 8594 8194  ....ubh...).....
-00004860: 7d94 2868 1b6a 1607 0000 681c 6803 681d  }.(h.j....h.h.h.
-00004870: 4e68 1e4e 7562 6816 8c05 20e2 8093 2094  Nh.Nubh... ... .
-00004880: 8594 8194 7d94 2868 1b6a 1607 0000 681c  ....}.(h.j....h.
-00004890: 6803 681d 4e68 1e4e 7562 6816 8c2b 5468  h.h.Nh.Nubh..+Th
-000048a0: 6520 6e61 6d65 206f 6620 7468 6520 7072  e name of the pr
-000048b0: 6f6a 6563 7420 796f 7520 7761 6e74 2074  oject you want t
-000048c0: 6f20 6465 6c65 7465 2e94 8594 8194 7d94  o delete......}.
-000048d0: 2868 1b6a 1607 0000 681c 6803 681d 4e68  (h.j....h.h.h.Nh
-000048e0: 1e4e 7562 6568 1f7d 9428 6821 5d94 6823  .Nubeh.}.(h!].h#
-000048f0: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
-00004900: 2b68 2d68 1b6a 1307 0000 7562 6168 1f7d  +h-h.j....ubah.}
-00004910: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-00004920: 5d94 6829 5d94 7568 2b68 6f68 1b6a 1007  ].h)].uh+hoh.j..
-00004930: 0000 7562 6870 2981 947d 9428 6805 6806  ..ubhp)..}.(h.h.
-00004940: 6807 5d94 682e 2981 947d 9428 6805 8c68  h.].h.)..}.(h..h
-00004950: 2d79 7c2d 2d79 6573 2028 666c 6167 2920  -y|--yes (flag) 
-00004960: 2d2d 2041 6e20 6f70 7469 6f6e 616c 2066  -- An optional f
-00004970: 6c61 6720 746f 2061 7574 6f2d 636f 6e66  lag to auto-conf
-00004980: 6972 6d20 796f 7572 2064 6563 6973 696f  irm your decisio
-00004990: 6e20 616e 6420 736b 6970 2074 6865 2022  n and skip the "
-000049a0: 4172 6520 796f 7520 7375 7265 3f22 2064  Are you sure?" d
-000049b0: 6961 6c6f 6775 652e 9468 075d 9428 6a8d  ialogue..h.].(j.
-000049c0: 0100 0029 8194 7d94 2868 058c 022d 7994  ...)..}.(h...-y.
-000049d0: 6807 5d94 6816 8c02 2d79 9485 9481 947d  h.].h...-y.....}
-000049e0: 9428 681b 6a67 0700 0068 1c68 0368 1d4e  .(h.jg...h.h.h.N
-000049f0: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
-00004a00: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
-00004a10: 682b 6a8c 0100 0068 1b6a 6307 0000 7562  h+j....h.jc...ub
-00004a20: 6a8d 0100 0029 8194 7d94 2868 056a 5102  j....)..}.(h.jQ.
-00004a30: 0000 6807 5d94 6816 8c01 7c94 8594 8194  ..h.].h...|.....
-00004a40: 7d94 2868 1b6a 7507 0000 681c 6803 681d  }.(h.ju...h.h.h.
-00004a50: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
-00004a60: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-00004a70: 7568 2b6a 8c01 0000 681b 6a63 0700 0075  uh+j....h.jc...u
-00004a80: 626a 8d01 0000 2981 947d 9428 6805 8c05  bj....)..}.(h...
-00004a90: 2d2d 7965 7394 6807 5d94 6816 8c05 2d2d  --yes.h.].h...--
-00004aa0: 7965 7394 8594 8194 7d94 2868 1b6a 8207  yes.....}.(h.j..
-00004ab0: 0000 681c 6803 681d 4e68 1e4e 7562 6168  ..h.h.h.Nh.Nubah
-00004ac0: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
-00004ad0: 6827 5d94 6829 5d94 7568 2b6a 8c01 0000  h'].h)].uh+j....
-00004ae0: 681b 6a63 0700 0075 6268 168c 0220 2894  h.jc...ubh... (.
-00004af0: 8594 8194 7d94 2868 1b6a 6307 0000 681c  ....}.(h.jc...h.
-00004b00: 6803 681d 4e68 1e4e 7562 6aa1 0100 0029  h.h.Nh.Nubj....)
-00004b10: 8194 7d94 2868 0568 0668 075d 946a a601  ..}.(h.h.h.].j..
-00004b20: 0000 2981 947d 9428 6805 8c04 666c 6167  ..)..}.(h...flag
-00004b30: 9468 075d 9468 168c 0466 6c61 6794 8594  .h.].h...flag...
-00004b40: 8194 7d94 2868 1b6a 9707 0000 681c 6803  ..}.(h.j....h.h.
-00004b50: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
-00004b60: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-00004b70: 5d94 7568 2b6a a501 0000 681b 6a94 0700  ].uh+j....h.j...
-00004b80: 0075 6261 681f 7d94 2868 215d 9468 235d  .ubah.}.(h!].h#]
-00004b90: 9468 255d 9468 275d 9468 295d 948c 0972  .h%].h'].h)]...r
-00004ba0: 6566 646f 6d61 696e 946a 4407 0000 8c0b  efdomain.jD.....
-00004bb0: 7265 6665 7870 6c69 6369 7494 898c 0772  refexplicit....r
-00004bc0: 6566 7479 7065 946a bf01 0000 8c09 7265  eftype.j......re
-00004bd0: 6674 6172 6765 7494 6a99 0700 006a c101  ftarget.j....j..
-00004be0: 0000 886a c201 0000 4e6a c301 0000 4e75  ...j....Nj....Nu
-00004bf0: 682b 6aa0 0100 0068 1b6a 6307 0000 7562  h+j....h.jc...ub
-00004c00: 6816 8c01 2994 8594 8194 7d94 2868 1b6a  h...).....}.(h.j
-00004c10: 6307 0000 681c 6803 681d 4e68 1e4e 7562  c...h.h.h.Nh.Nub
-00004c20: 6816 8c05 20e2 8093 2094 8594 8194 7d94  h... ... .....}.
-00004c30: 2868 1b6a 6307 0000 681c 6803 681d 4e68  (h.jc...h.h.h.Nh
-00004c40: 1e4e 7562 6816 8c59 416e 206f 7074 696f  .Nubh..YAn optio
-00004c50: 6e61 6c20 666c 6167 2074 6f20 6175 746f  nal flag to auto
-00004c60: 2d63 6f6e 6669 726d 2079 6f75 7220 6465  -confirm your de
-00004c70: 6369 7369 6f6e 2061 6e64 2073 6b69 7020  cision and skip 
-00004c80: 7468 6520 e280 9c41 7265 2079 6f75 2073  the ...Are you s
-00004c90: 7572 653f e280 9d20 6469 616c 6f67 7565  ure?... dialogue
-00004ca0: 2e94 8594 8194 7d94 2868 1b6a 6307 0000  ......}.(h.jc...
-00004cb0: 681c 6803 681d 4e68 1e4e 7562 6568 1f7d  h.h.h.Nh.Nubeh.}
-00004cc0: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-00004cd0: 5d94 6829 5d94 7568 2b68 2d68 1b6a 6007  ].h)].uh+h-h.j`.
-00004ce0: 0000 7562 6168 1f7d 9428 6821 5d94 6823  ..ubah.}.(h!].h#
-00004cf0: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
-00004d00: 2b68 6f68 1b6a 1007 0000 7562 6568 1f7d  +hoh.j....ubeh.}
-00004d10: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-00004d20: 5d94 6829 5d94 7568 2b68 6a68 1b6a 0d07  ].h)].uh+hjh.j..
-00004d30: 0000 7562 6168 1f7d 9428 6821 5d94 6823  ..ubah.}.(h!].h#
-00004d40: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
-00004d50: 2b6a 7d01 0000 681b 6afc 0600 0075 6265  +j}...h.j....ube
-00004d60: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-00004d70: 9468 275d 9468 295d 9475 682b 6a68 0100  .h'].h)].uh+jh..
-00004d80: 0068 1b6a f906 0000 7562 6a69 0100 0029  .h.j....ubji...)
-00004d90: 8194 7d94 2868 0568 0668 075d 9428 6a6e  ..}.(h.h.h.].(jn
-00004da0: 0100 0029 8194 7d94 2868 058c 0752 6574  ...)..}.(h...Ret
-00004db0: 7572 6e73 9468 075d 9468 168c 0752 6574  urns.h.].h...Ret
-00004dc0: 7572 6e73 9485 9481 947d 9428 681b 6adc  urns.....}.(h.j.
-00004dd0: 0700 0068 1c68 0368 1d4e 681e 4e75 6261  ...h.h.h.Nh.Nuba
-00004de0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-00004df0: 9468 275d 9468 295d 9475 682b 6a6d 0100  .h'].h)].uh+jm..
-00004e00: 0068 1b6a d907 0000 681d 682c 681e 4b00  .h.j....h.h,h.K.
-00004e10: 7562 6a7e 0100 0029 8194 7d94 2868 0568  ubj~...)..}.(h.h
-00004e20: 0668 075d 9468 2e29 8194 7d94 2868 058c  .h.].h.)..}.(h..
-00004e30: 044e 6f6e 6594 6807 5d94 6816 8c04 4e6f  .None.h.].h...No
-00004e40: 6e65 9485 9481 947d 9428 681b 6aed 0700  ne.....}.(h.j...
-00004e50: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
-00004e60: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-00004e70: 275d 9468 295d 9475 682b 682d 681b 6aea  '].h)].uh+h-h.j.
-00004e80: 0700 0075 6261 681f 7d94 2868 215d 9468  ...ubah.}.(h!].h
-00004e90: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
-00004ea0: 682b 6a7d 0100 0068 1b6a d907 0000 7562  h+j}...h.j....ub
-00004eb0: 6568 1f7d 9428 6821 5d94 6823 5d94 6825  eh.}.(h!].h#].h%
-00004ec0: 5d94 6827 5d94 6829 5d94 7568 2b6a 6801  ].h'].h)].uh+jh.
-00004ed0: 0000 681b 6af9 0600 0075 626a 6901 0000  ..h.j....ubji...
-00004ee0: 2981 947d 9428 6805 6806 6807 5d94 286a  )..}.(h.h.h.].(j
-00004ef0: 6e01 0000 2981 947d 9428 6805 8c0b 5265  n...)..}.(h...Re
-00004f00: 7475 726e 2074 7970 6594 6807 5d94 6816  turn type.h.].h.
-00004f10: 8c0b 5265 7475 726e 2074 7970 6594 8594  ..Return type...
-00004f20: 8194 7d94 2868 1b6a 0a08 0000 681c 6803  ..}.(h.j....h.h.
-00004f30: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
-00004f40: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-00004f50: 5d94 7568 2b6a 6d01 0000 681b 6a07 0800  ].uh+jm...h.j...
-00004f60: 0068 1d68 2c68 1e4b 0075 626a 7e01 0000  .h.h,h.K.ubj~...
-00004f70: 2981 947d 9428 6805 6806 6807 5d94 682e  )..}.(h.h.h.].h.
-00004f80: 2981 947d 9428 6805 8c04 4e6f 6e65 9468  )..}.(h...None.h
-00004f90: 075d 946a a101 0000 2981 947d 9428 6805  .].j....)..}.(h.
-00004fa0: 6806 6807 5d94 6816 8c04 4e6f 6e65 9485  h.h.].h...None..
-00004fb0: 9481 947d 9428 681b 6a1f 0800 0068 1c68  ...}.(h.j....h.h
-00004fc0: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
-00004fd0: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-00004fe0: 295d 948c 0972 6566 646f 6d61 696e 946a  )]...refdomain.j
-00004ff0: 4407 0000 8c0b 7265 6665 7870 6c69 6369  D.....refexplici
-00005000: 7494 898c 0772 6566 7479 7065 946a bf01  t....reftype.j..
-00005010: 0000 8c09 7265 6674 6172 6765 7494 8c04  ....reftarget...
-00005020: 4e6f 6e65 946a c101 0000 886a c201 0000  None.j.....j....
-00005030: 4e6a c301 0000 4e75 682b 6aa0 0100 0068  Nj....Nuh+j....h
-00005040: 1b6a 1b08 0000 7562 6168 1f7d 9428 6821  .j....ubah.}.(h!
-00005050: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-00005060: 5d94 7568 2b68 2d68 1b6a 1808 0000 7562  ].uh+h-h.j....ub
-00005070: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
-00005080: 5d94 6827 5d94 6829 5d94 7568 2b6a 7d01  ].h'].h)].uh+j}.
-00005090: 0000 681b 6a07 0800 0075 6265 681f 7d94  ..h.j....ubeh.}.
-000050a0: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
-000050b0: 9468 295d 9475 682b 6a68 0100 0068 1b6a  .h)].uh+jh...h.j
-000050c0: f906 0000 7562 6568 1f7d 9428 6821 5d94  ....ubeh.}.(h!].
-000050d0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-000050e0: 7568 2b6a 6301 0000 681b 6ab2 0600 0068  uh+jc...h.j....h
-000050f0: 1c68 0368 1d4e 681e 4e75 6265 681f 7d94  .h.h.Nh.Nubeh.}.
-00005100: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
-00005110: 9468 295d 9475 682b 6a50 0100 0068 1b6a  .h)].uh+jP...h.j
-00005120: 9806 0000 681c 6803 681d 682c 681e 4b47  ....h.h.h.h,h.KG
-00005130: 7562 6568 1f7d 9428 6821 5d94 6823 5d94  ubeh.}.(h!].h#].
-00005140: 286a 4407 0000 8c08 6675 6e63 7469 6f6e  (jD.....function
-00005150: 9465 6825 5d94 6827 5d94 6829 5d94 6a7d  .eh%].h'].h)].j}
-00005160: 0300 006a 4407 0000 6a7e 0300 006a 5208  ...jD...j~...jR.
-00005170: 0000 6a7f 0300 006a 5208 0000 6a80 0300  ..j....jR...j...
-00005180: 0089 6a81 0300 0089 6a82 0300 0089 7568  ..j.....j.....uh
-00005190: 2b6a 2801 0000 681c 6803 681b 6a7c 0600  +j(...h.h.h.j|..
-000051a0: 0068 1d4e 681e 4e75 6265 681f 7d94 2868  .h.Nh.Nubeh.}.(h
-000051b0: 215d 948c 0c6e 6573 7465 722d 636c 6561  !]...nester-clea
-000051c0: 6e94 6168 235d 9468 255d 948c 0c6e 6573  n.ah#].h%]...nes
-000051d0: 7465 7220 636c 6561 6e94 6168 275d 9468  ter clean.ah'].h
-000051e0: 295d 9475 682b 680a 681b 684b 681c 6803  )].uh+h.h.hKh.h.
-000051f0: 681d 682c 681e 4b45 7562 6568 1f7d 9428  h.h,h.KEubeh.}.(
-00005200: 6821 5d94 8c08 636c 692d 6d6f 6465 9461  h!]...cli-mode.a
-00005210: 6823 5d94 6825 5d94 8c08 636c 692d 6d6f  h#].h%]...cli-mo
-00005220: 6465 9461 6827 5d94 6829 5d94 7568 2b68  de.ah'].h)].uh+h
-00005230: 0a68 1b68 0c68 1c68 0368 1d68 2c68 1e4b  .h.h.h.h.h.h,h.K
-00005240: 0a75 6265 681f 7d94 2868 215d 948c 0575  .ubeh.}.(h!]...u
-00005250: 7361 6765 9461 6823 5d94 6825 5d94 8c05  sage.ah#].h%]...
-00005260: 7573 6167 6594 6168 275d 9468 295d 9475  usage.ah'].h)].u
-00005270: 682b 680a 681b 6803 681c 6803 681d 682c  h+h.h.h.h.h.h.h,
-00005280: 681e 4b02 7562 6168 1f7d 9428 6821 5d94  h.K.ubah.}.(h!].
-00005290: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-000052a0: 8c06 736f 7572 6365 9468 2c75 682b 6801  ..source.h,uh+h.
-000052b0: 8c0e 6375 7272 656e 745f 736f 7572 6365  ..current_source
-000052c0: 944e 8c0c 6375 7272 656e 745f 6c69 6e65  .N..current_line
-000052d0: 944e 8c08 7365 7474 696e 6773 948c 1164  .N..settings...d
-000052e0: 6f63 7574 696c 732e 6672 6f6e 7465 6e64  ocutils.frontend
-000052f0: 948c 0656 616c 7565 7394 9394 2981 947d  ...Values...)..}
-00005300: 9428 680f 4e8c 0967 656e 6572 6174 6f72  .(h.N..generator
-00005310: 944e 8c09 6461 7465 7374 616d 7094 4e8c  .N..datestamp.N.
-00005320: 0b73 6f75 7263 655f 6c69 6e6b 944e 8c0a  .source_link.N..
-00005330: 736f 7572 6365 5f75 726c 944e 8c0d 746f  source_url.N..to
-00005340: 635f 6261 636b 6c69 6e6b 7394 8c05 656e  c_backlinks...en
-00005350: 7472 7994 8c12 666f 6f74 6e6f 7465 5f62  try...footnote_b
-00005360: 6163 6b6c 696e 6b73 944b 018c 0d73 6563  acklinks.K...sec
-00005370: 746e 756d 5f78 666f 726d 944b 018c 0e73  tnum_xform.K...s
-00005380: 7472 6970 5f63 6f6d 6d65 6e74 7394 4e8c  trip_comments.N.
-00005390: 1b73 7472 6970 5f65 6c65 6d65 6e74 735f  .strip_elements_
-000053a0: 7769 7468 5f63 6c61 7373 6573 944e 8c0d  with_classes.N..
-000053b0: 7374 7269 705f 636c 6173 7365 7394 4e8c  strip_classes.N.
-000053c0: 0c72 6570 6f72 745f 6c65 7665 6c94 4b02  .report_level.K.
-000053d0: 8c0a 6861 6c74 5f6c 6576 656c 944b 058c  ..halt_level.K..
-000053e0: 1165 7869 745f 7374 6174 7573 5f6c 6576  .exit_status_lev
-000053f0: 656c 944b 058c 0564 6562 7567 944e 8c0e  el.K...debug.N..
-00005400: 7761 726e 696e 675f 7374 7265 616d 944e  warning_stream.N
-00005410: 8c09 7472 6163 6562 6163 6b94 888c 0e69  ..traceback....i
-00005420: 6e70 7574 5f65 6e63 6f64 696e 6794 8c09  nput_encoding...
-00005430: 7574 662d 382d 7369 6794 8c1c 696e 7075  utf-8-sig...inpu
-00005440: 745f 656e 636f 6469 6e67 5f65 7272 6f72  t_encoding_error
-00005450: 5f68 616e 646c 6572 948c 0673 7472 6963  _handler...stric
-00005460: 7494 8c0f 6f75 7470 7574 5f65 6e63 6f64  t...output_encod
-00005470: 696e 6794 8c05 7574 662d 3894 8c1d 6f75  ing...utf-8...ou
-00005480: 7470 7574 5f65 6e63 6f64 696e 675f 6572  tput_encoding_er
-00005490: 726f 725f 6861 6e64 6c65 7294 6a91 0800  ror_handler.j...
-000054a0: 008c 0e65 7272 6f72 5f65 6e63 6f64 696e  ...error_encodin
-000054b0: 6794 8c05 7574 662d 3894 8c1c 6572 726f  g...utf-8...erro
-000054c0: 725f 656e 636f 6469 6e67 5f65 7272 6f72  r_encoding_error
-000054d0: 5f68 616e 646c 6572 948c 1062 6163 6b73  _handler...backs
-000054e0: 6c61 7368 7265 706c 6163 6594 8c0d 6c61  lashreplace...la
-000054f0: 6e67 7561 6765 5f63 6f64 6594 8c02 656e  nguage_code...en
-00005500: 948c 1372 6563 6f72 645f 6465 7065 6e64  ...record_depend
-00005510: 656e 6369 6573 944e 8c06 636f 6e66 6967  encies.N..config
-00005520: 944e 8c09 6964 5f70 7265 6669 7894 6806  .N..id_prefix.h.
-00005530: 8c0e 6175 746f 5f69 645f 7072 6566 6978  ..auto_id_prefix
-00005540: 948c 0269 6494 8c0d 6475 6d70 5f73 6574  ...id...dump_set
-00005550: 7469 6e67 7394 4e8c 0e64 756d 705f 696e  tings.N..dump_in
-00005560: 7465 726e 616c 7394 4e8c 0f64 756d 705f  ternals.N..dump_
-00005570: 7472 616e 7366 6f72 6d73 944e 8c0f 6475  transforms.N..du
-00005580: 6d70 5f70 7365 7564 6f5f 786d 6c94 4e8c  mp_pseudo_xml.N.
-00005590: 1065 7870 6f73 655f 696e 7465 726e 616c  .expose_internal
-000055a0: 7394 4e8c 0e73 7472 6963 745f 7669 7369  s.N..strict_visi
-000055b0: 746f 7294 4e8c 0f5f 6469 7361 626c 655f  tor.N.._disable_
-000055c0: 636f 6e66 6967 944e 8c07 5f73 6f75 7263  config.N.._sourc
-000055d0: 6594 682c 8c0c 5f64 6573 7469 6e61 7469  e.h,.._destinati
-000055e0: 6f6e 944e 8c0d 5f63 6f6e 6669 675f 6669  on.N.._config_fi
-000055f0: 6c65 7394 5d94 8c16 6669 6c65 5f69 6e73  les.]...file_ins
-00005600: 6572 7469 6f6e 5f65 6e61 626c 6564 9488  ertion_enabled..
-00005610: 8c0b 7261 775f 656e 6162 6c65 6494 4b01  ..raw_enabled.K.
-00005620: 8c11 6c69 6e65 5f6c 656e 6774 685f 6c69  ..line_length_li
-00005630: 6d69 7494 4d10 278c 0e70 6570 5f72 6566  mit.M.'..pep_ref
-00005640: 6572 656e 6365 7394 4e8c 0c70 6570 5f62  erences.N..pep_b
-00005650: 6173 655f 7572 6c94 8c18 6874 7470 733a  ase_url...https:
-00005660: 2f2f 7065 7073 2e70 7974 686f 6e2e 6f72  //peps.python.or
-00005670: 672f 948c 1570 6570 5f66 696c 655f 7572  g/...pep_file_ur
-00005680: 6c5f 7465 6d70 6c61 7465 948c 0870 6570  l_template...pep
-00005690: 2d25 3034 6494 8c0e 7266 635f 7265 6665  -%04d...rfc_refe
-000056a0: 7265 6e63 6573 944e 8c0c 7266 635f 6261  rences.N..rfc_ba
-000056b0: 7365 5f75 726c 948c 2668 7474 7073 3a2f  se_url..&https:/
-000056c0: 2f64 6174 6174 7261 636b 6572 2e69 6574  /datatracker.iet
-000056d0: 662e 6f72 672f 646f 632f 6874 6d6c 2f94  f.org/doc/html/.
-000056e0: 8c09 7461 625f 7769 6474 6894 4b08 8c1d  ..tab_width.K...
-000056f0: 7472 696d 5f66 6f6f 746e 6f74 655f 7265  trim_footnote_re
-00005700: 6665 7265 6e63 655f 7370 6163 6594 898c  ference_space...
-00005710: 1073 796e 7461 785f 6869 6768 6c69 6768  .syntax_highligh
-00005720: 7494 8c04 6c6f 6e67 948c 0c73 6d61 7274  t...long...smart
-00005730: 5f71 756f 7465 7394 888c 1373 6d61 7274  _quotes....smart
-00005740: 7175 6f74 6573 5f6c 6f63 616c 6573 945d  quotes_locales.]
-00005750: 948c 1d63 6861 7261 6374 6572 5f6c 6576  ...character_lev
-00005760: 656c 5f69 6e6c 696e 655f 6d61 726b 7570  el_inline_markup
-00005770: 9489 8c0e 646f 6374 6974 6c65 5f78 666f  ....doctitle_xfo
-00005780: 726d 9489 8c0d 646f 6369 6e66 6f5f 7866  rm....docinfo_xf
-00005790: 6f72 6d94 4b01 8c12 7365 6374 7375 6274  orm.K...sectsubt
-000057a0: 6974 6c65 5f78 666f 726d 9489 8c0d 696d  itle_xform....im
-000057b0: 6167 655f 6c6f 6164 696e 6794 8c04 6c69  age_loading...li
-000057c0: 6e6b 948c 1065 6d62 6564 5f73 7479 6c65  nk...embed_style
-000057d0: 7368 6565 7494 898c 1563 6c6f 616b 5f65  sheet....cloak_e
-000057e0: 6d61 696c 5f61 6464 7265 7373 6573 9488  mail_addresses..
-000057f0: 8c11 7365 6374 696f 6e5f 7365 6c66 5f6c  ..section_self_l
-00005800: 696e 6b94 898c 0365 6e76 944e 7562 8c08  ink....env.Nub..
-00005810: 7265 706f 7274 6572 944e 8c10 696e 6469  reporter.N..indi
-00005820: 7265 6374 5f74 6172 6765 7473 945d 948c  rect_targets.]..
-00005830: 1173 7562 7374 6974 7574 696f 6e5f 6465  .substitution_de
-00005840: 6673 947d 948c 1273 7562 7374 6974 7574  fs.}...substitut
-00005850: 696f 6e5f 6e61 6d65 7394 7d94 8c08 7265  ion_names.}...re
-00005860: 666e 616d 6573 947d 948c 0672 6566 6964  fnames.}...refid
-00005870: 7394 7d94 8c07 6e61 6d65 6964 7394 7d94  s.}...nameids.}.
-00005880: 286a 6b08 0000 6a68 0800 006a 6308 0000  (jk...jh...jc...
-00005890: 6a60 0800 006a 8803 0000 6a85 0300 006a  j`...j....j....j
-000058a0: 3d05 0000 6a3a 0500 006a 7906 0000 6a76  =...j:...jy...jv
-000058b0: 0600 006a 5b08 0000 6a58 0800 0075 8c09  ...j[...jX...u..
-000058c0: 6e61 6d65 7479 7065 7394 7d94 286a 6b08  nametypes.}.(jk.
-000058d0: 0000 896a 6308 0000 896a 8803 0000 896a  ...jc....j.....j
-000058e0: 3d05 0000 896a 7906 0000 896a 5b08 0000  =....jy....j[...
-000058f0: 8975 6821 7d94 286a 6808 0000 680c 6a60  .uh!}.(jh...h.j`
-00005900: 0800 0068 4b6a 8503 0000 6a0a 0100 006a  ...hKj....j....j
-00005910: 3a05 0000 6a8b 0300 006a 7606 0000 6a40  :...j....jv...j@
-00005920: 0500 006a 5808 0000 6a7c 0600 0075 8c0d  ...jX...j|...u..
-00005930: 666f 6f74 6e6f 7465 5f72 6566 7394 7d94  footnote_refs.}.
-00005940: 8c0d 6369 7461 7469 6f6e 5f72 6566 7394  ..citation_refs.
-00005950: 7d94 8c0d 6175 746f 666f 6f74 6e6f 7465  }...autofootnote
-00005960: 7394 5d94 8c11 6175 746f 666f 6f74 6e6f  s.]...autofootno
-00005970: 7465 5f72 6566 7394 5d94 8c10 7379 6d62  te_refs.]...symb
-00005980: 6f6c 5f66 6f6f 746e 6f74 6573 945d 948c  ol_footnotes.]..
-00005990: 1473 796d 626f 6c5f 666f 6f74 6e6f 7465  .symbol_footnote
-000059a0: 5f72 6566 7394 5d94 8c09 666f 6f74 6e6f  _refs.]...footno
-000059b0: 7465 7394 5d94 8c09 6369 7461 7469 6f6e  tes.]...citation
-000059c0: 7394 5d94 8c12 6175 746f 666f 6f74 6e6f  s.]...autofootno
-000059d0: 7465 5f73 7461 7274 944b 018c 1573 796d  te_start.K...sym
-000059e0: 626f 6c5f 666f 6f74 6e6f 7465 5f73 7461  bol_footnote_sta
-000059f0: 7274 944b 008c 0a69 645f 636f 756e 7465  rt.K...id_counte
-00005a00: 7294 8c0b 636f 6c6c 6563 7469 6f6e 7394  r...collections.
-00005a10: 8c07 436f 756e 7465 7294 9394 7d94 8594  ..Counter...}...
-00005a20: 5294 8c0e 7061 7273 655f 6d65 7373 6167  R...parse_messag
-00005a30: 6573 945d 948c 1274 7261 6e73 666f 726d  es.]...transform
-00005a40: 5f6d 6573 7361 6765 7394 5d94 8c0b 7472  _messages.]...tr
-00005a50: 616e 7366 6f72 6d65 7294 4e8c 0b69 6e63  ansformer.N..inc
-00005a60: 6c75 6465 5f6c 6f67 945d 948c 0a64 6563  lude_log.]...dec
-00005a70: 6f72 6174 696f 6e94 4e68 1c68 0375 622e  oration.Nh.h.ub.
+000008c0: 9428 6805 8c3c 4c65 7420 7573 206c 6f6f  .(h..<Let us loo
+000008d0: 6b20 696e 746f 2065 6163 6820 6f66 2074  k into each of t
+000008e0: 6865 2066 6f75 7220 636f 6d6d 616e 6473  he four commands
+000008f0: 2069 6e20 6d6f 7265 2064 6574 6169 6c2e   in more detail.
+00000900: 2e2e 9468 075d 9468 168c 3c4c 6574 2075  ...h.].h..<Let u
+00000910: 7320 6c6f 6f6b 2069 6e74 6f20 6561 6368  s look into each
+00000920: 206f 6620 7468 6520 666f 7572 2063 6f6d   of the four com
+00000930: 6d61 6e64 7320 696e 206d 6f72 6520 6465  mands in more de
+00000940: 7461 696c e280 a694 8594 8194 7d94 2868  tail........}.(h
+00000950: 1b68 fc68 1c68 0368 1d4e 681e 4e75 6261  .h.h.h.h.Nh.Nuba
+00000960: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+00000970: 9468 275d 9468 295d 9475 682b 682d 681d  .h'].h)].uh+h-h.
+00000980: 682c 681e 4b14 681b 684b 681c 6803 7562  h,h.K.h.hKh.h.ub
+00000990: 680b 2981 947d 9428 6805 6806 6807 5d94  h.)..}.(h.h.h.].
+000009a0: 2868 1029 8194 7d94 2868 058c 0d4e 6573  (h.)..}.(h...Nes
+000009b0: 7465 7220 6372 6561 7465 9468 075d 9468  ter create.h.].h
+000009c0: 168c 0d4e 6573 7465 7220 6372 6561 7465  ...Nester create
+000009d0: 9485 9481 947d 9428 681b 6a0d 0100 0068  .....}.(h.j....h
+000009e0: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
+000009f0: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+00000a00: 9468 295d 9475 682b 680f 681b 6a0a 0100  .h)].uh+h.h.j...
+00000a10: 0068 1c68 0368 1d68 2c68 1e4b 1775 6268  .h.h.h.h,h.K.ubh
+00000a20: 008c 0569 6e64 6578 9493 9429 8194 7d94  ...index...)..}.
+00000a30: 2868 0568 0668 075d 9468 1f7d 9428 6821  (h.h.h.].h.}.(h!
+00000a40: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+00000a50: 5d94 8c07 656e 7472 6965 7394 5d94 7568  ]...entries.].uh
+00000a60: 2b6a 1b01 0000 681b 6a0a 0100 0068 1c68  +j....h.j....h.h
+00000a70: 0368 1d4e 681e 4e75 6268 008c 0464 6573  .h.Nh.Nubh...des
+00000a80: 6394 9394 2981 947d 9428 6805 6806 6807  c...)..}.(h.h.h.
+00000a90: 5d94 2868 008c 0e64 6573 635f 7369 676e  ].(h...desc_sign
+00000aa0: 6174 7572 6594 9394 2981 947d 9428 6805  ature...)..}.(h.
+00000ab0: 8c30 6e65 7374 6572 2063 7265 6174 6528  .0nester create(
+00000ac0: 6c61 6e67 7561 6765 2c20 7072 6f6a 6563  language, projec
+00000ad0: 746e 616d 652c 205b 2d67 7c2d 2d67 6974  tname, [-g|--git
+00000ae0: 5d29 9468 075d 9468 008c 0964 6573 635f  ]).h.].h...desc_
+00000af0: 6e61 6d65 9493 9429 8194 7d94 2868 056a  name...)..}.(h.j
+00000b00: 3101 0000 6807 5d94 6816 8c30 6e65 7374  1...h.].h..0nest
+00000b10: 6572 2063 7265 6174 6528 6c61 6e67 7561  er create(langua
+00000b20: 6765 2c20 7072 6f6a 6563 746e 616d 652c  ge, projectname,
+00000b30: 205b 2d67 7c2d 2d67 6974 5d29 9485 9481   [-g|--git])....
+00000b40: 947d 9428 681b 6a35 0100 0068 1c68 0368  .}.(h.j5...h.h.h
+00000b50: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
+00000b60: 9468 235d 9428 8c08 7369 672d 6e61 6d65  .h#].(..sig-name
+00000b70: 948c 0864 6573 636e 616d 6594 6568 255d  ...descname.eh%]
+00000b80: 9468 275d 9468 295d 948c 0978 6d6c 3a73  .h'].h)]...xml:s
+00000b90: 7061 6365 948c 0870 7265 7365 7276 6594  pace...preserve.
+00000ba0: 7568 2b6a 3301 0000 681b 6a2f 0100 0068  uh+j3...h.j/...h
+00000bb0: 1c68 0368 1d68 2c68 1e4b 1975 6261 681f  .h.h.h,h.K.ubah.
+00000bc0: 7d94 2868 215d 9468 235d 9428 8c03 7369  }.(h!].h#].(..si
+00000bd0: 6794 8c0a 7369 672d 6f62 6a65 6374 9465  g...sig-object.e
+00000be0: 6825 5d94 6827 5d94 6829 5d94 8c0a 5f74  h%].h'].h)]..._t
+00000bf0: 6f63 5f70 6172 7473 9429 8c09 5f74 6f63  oc_parts.).._toc
+00000c00: 5f6e 616d 6594 6806 7568 2b6a 2d01 0000  _name.h.uh+j-...
+00000c10: 681d 682c 681e 4b19 681b 6a2a 0100 0068  h.h,h.K.h.j*...h
+00000c20: 1c68 0375 6268 008c 0c64 6573 635f 636f  .h.ubh...desc_co
+00000c30: 6e74 656e 7494 9394 2981 947d 9428 6805  ntent...)..}.(h.
+00000c40: 6806 6807 5d94 2868 2e29 8194 7d94 2868  h.h.].(h.)..}.(h
+00000c50: 0558 0501 0000 4372 6561 7465 7320 7468  .X....Creates th
+00000c60: 6520 7072 6f6a 6563 7420 7374 7275 6374  e project struct
+00000c70: 7572 6520 666f 7220 7468 6520 6769 7665  ure for the give
+00000c80: 6e20 7072 6f6a 6563 742e 0a49 6620 796f  n project..If yo
+00000c90: 7520 6172 6520 616c 7265 6164 7920 696e  u are already in
+00000ca0: 2061 2064 6972 6563 746f 7279 2077 6869   a directory whi
+00000cb0: 6368 206d 6174 6368 6573 2074 6865 206e  ch matches the n
+00000cc0: 616d 6520 6f66 2074 6865 2067 6976 656e  ame of the given
+00000cd0: 2070 726f 6a65 6374 2c20 7468 6520 736f   project, the so
+00000ce0: 7572 6365 2066 696c 6573 2077 696c 6c20  urce files will 
+00000cf0: 6265 2063 7265 6174 6564 2069 6e20 796f  be created in yo
+00000d00: 7572 2063 7572 7265 6e74 2064 6972 6563  ur current direc
+00000d10: 746f 7279 2e0a 4966 206e 6f74 204e 6573  tory..If not Nes
+00000d20: 7465 7220 7769 6c6c 2061 7574 6f6d 6174  ter will automat
+00000d30: 6963 616c 6c79 2063 7265 6174 6520 6120  ically create a 
+00000d40: 6469 7265 6374 6f72 7920 666f 7220 796f  directory for yo
+00000d50: 7572 2070 726f 6a65 6374 2e94 6807 5d94  ur project..h.].
+00000d60: 6816 5805 0100 0043 7265 6174 6573 2074  h.X....Creates t
+00000d70: 6865 2070 726f 6a65 6374 2073 7472 7563  he project struc
+00000d80: 7475 7265 2066 6f72 2074 6865 2067 6976  ture for the giv
+00000d90: 656e 2070 726f 6a65 6374 2e0a 4966 2079  en project..If y
+00000da0: 6f75 2061 7265 2061 6c72 6561 6479 2069  ou are already i
+00000db0: 6e20 6120 6469 7265 6374 6f72 7920 7768  n a directory wh
+00000dc0: 6963 6820 6d61 7463 6865 7320 7468 6520  ich matches the 
+00000dd0: 6e61 6d65 206f 6620 7468 6520 6769 7665  name of the give
+00000de0: 6e20 7072 6f6a 6563 742c 2074 6865 2073  n project, the s
+00000df0: 6f75 7263 6520 6669 6c65 7320 7769 6c6c  ource files will
+00000e00: 2062 6520 6372 6561 7465 6420 696e 2079   be created in y
+00000e10: 6f75 7220 6375 7272 656e 7420 6469 7265  our current dire
+00000e20: 6374 6f72 792e 0a49 6620 6e6f 7420 4e65  ctory..If not Ne
+00000e30: 7374 6572 2077 696c 6c20 6175 746f 6d61  ster will automa
+00000e40: 7469 6361 6c6c 7920 6372 6561 7465 2061  tically create a
+00000e50: 2064 6972 6563 746f 7279 2066 6f72 2079   directory for y
+00000e60: 6f75 7220 7072 6f6a 6563 742e 9485 9481  our project.....
+00000e70: 947d 9428 681b 6a55 0100 0068 1c68 0368  .}.(h.jU...h.h.h
+00000e80: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
+00000e90: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+00000ea0: 9475 682b 682d 681d 682c 681e 4b1b 681b  .uh+h-h.h,h.K.h.
+00000eb0: 6a52 0100 0068 1c68 0375 6268 098c 0a66  jR...h.h.ubh...f
+00000ec0: 6965 6c64 5f6c 6973 7494 9394 2981 947d  ield_list...)..}
+00000ed0: 9428 6805 6806 6807 5d94 2868 098c 0566  .(h.h.h.].(h...f
+00000ee0: 6965 6c64 9493 9429 8194 7d94 2868 0568  ield...)..}.(h.h
+00000ef0: 0668 075d 9428 6809 8c0a 6669 656c 645f  .h.].(h...field_
+00000f00: 6e61 6d65 9493 9429 8194 7d94 2868 058c  name...)..}.(h..
+00000f10: 0a50 6172 616d 6574 6572 7394 6807 5d94  .Parameters.h.].
+00000f20: 6816 8c0a 5061 7261 6d65 7465 7273 9485  h...Parameters..
+00000f30: 9481 947d 9428 681b 6a6f 0100 0068 1c68  ...}.(h.jo...h.h
+00000f40: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
+00000f50: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+00000f60: 295d 9475 682b 6a6d 0100 0068 1b6a 6a01  )].uh+jm...h.jj.
+00000f70: 0000 681d 682c 681e 4b00 7562 6809 8c0a  ..h.h,h.K.ubh...
+00000f80: 6669 656c 645f 626f 6479 9493 9429 8194  field_body...)..
+00000f90: 7d94 2868 0568 0668 075d 9468 6b29 8194  }.(h.h.h.].hk)..
+00000fa0: 7d94 2868 0568 0668 075d 9428 6870 2981  }.(h.h.h.].(hp).
+00000fb0: 947d 9428 6805 6806 6807 5d94 682e 2981  .}.(h.h.h.].h.).
+00000fc0: 947d 9428 6805 8c8a 6c61 6e67 7561 6765  .}.(h...language
+00000fd0: 2028 7374 7229 202d 2d20 5468 6520 7368   (str) -- The sh
+00000fe0: 6f72 7466 6f72 6d20 6f66 2061 2073 7570  ortform of a sup
+00000ff0: 706f 7274 6564 2070 726f 6772 616d 6d69  ported programmi
+00001000: 6e67 206c 616e 6775 6167 652e 2052 6566  ng language. Ref
+00001010: 6572 2074 6f20 7468 6520 3a64 6f63 3a20  er to the :doc: 
+00001020: 6c69 7374 206f 6620 7375 7070 6f72 7465  list of supporte
+00001030: 6420 6c61 6e67 7561 6765 7320 3c73 7570  d languages <sup
+00001040: 706f 7274 6564 5f6c 616e 6775 6167 6573  ported_languages
+00001050: 3e2e 9468 075d 9428 6800 8c0e 6c69 7465  >..h.].(h...lite
+00001060: 7261 6c5f 7374 726f 6e67 9493 9429 8194  ral_strong...)..
+00001070: 7d94 2868 058c 086c 616e 6775 6167 6594  }.(h...language.
+00001080: 6807 5d94 6816 8c08 6c61 6e67 7561 6765  h.].h...language
+00001090: 9485 9481 947d 9428 681b 6a8e 0100 0068  .....}.(h.j....h
+000010a0: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
+000010b0: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+000010c0: 9468 295d 9475 682b 6a8c 0100 0068 1b6a  .h)].uh+j....h.j
+000010d0: 8801 0000 7562 6816 8c02 2028 9485 9481  ....ubh... (....
+000010e0: 947d 9428 681b 6a88 0100 0068 1c68 0368  .}.(h.j....h.h.h
+000010f0: 1d4e 681e 4e75 6268 008c 0c70 656e 6469  .Nh.Nubh...pendi
+00001100: 6e67 5f78 7265 6694 9394 2981 947d 9428  ng_xref...)..}.(
+00001110: 6805 6806 6807 5d94 6800 8c10 6c69 7465  h.h.h.].h...lite
+00001120: 7261 6c5f 656d 7068 6173 6973 9493 9429  ral_emphasis...)
+00001130: 8194 7d94 2868 058c 0373 7472 9468 075d  ..}.(h...str.h.]
+00001140: 9468 168c 0373 7472 9485 9481 947d 9428  .h...str.....}.(
+00001150: 681b 6aa7 0100 0068 1c68 0368 1d4e 681e  h.j....h.h.h.Nh.
+00001160: 4e75 6261 681f 7d94 2868 215d 9468 235d  Nubah.}.(h!].h#]
+00001170: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
+00001180: 6aa5 0100 0068 1b6a a201 0000 7562 6168  j....h.j....ubah
+00001190: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+000011a0: 6827 5d94 6829 5d94 8c09 7265 6664 6f6d  h'].h)]...refdom
+000011b0: 6169 6e94 8c02 7079 948c 0b72 6566 6578  ain...py...refex
+000011c0: 706c 6963 6974 9489 8c07 7265 6674 7970  plicit....reftyp
+000011d0: 6594 8c05 636c 6173 7394 8c09 7265 6674  e...class...reft
+000011e0: 6172 6765 7494 6aa9 0100 008c 0b72 6566  arget.j......ref
+000011f0: 7370 6563 6966 6963 9488 8c09 7079 3a6d  specific....py:m
+00001200: 6f64 756c 6594 4e8c 0870 793a 636c 6173  odule.N..py:clas
+00001210: 7394 4e75 682b 6aa0 0100 0068 1b6a 8801  s.Nuh+j....h.j..
+00001220: 0000 7562 6816 8c01 2994 8594 8194 7d94  ..ubh...).....}.
+00001230: 2868 1b6a 8801 0000 681c 6803 681d 4e68  (h.j....h.h.h.Nh
+00001240: 1e4e 7562 6816 8c05 20e2 8093 2094 8594  .Nubh... ... ...
+00001250: 8194 7d94 2868 1b6a 8801 0000 681c 6803  ..}.(h.j....h.h.
+00001260: 681d 4e68 1e4e 7562 6816 8c46 5468 6520  h.Nh.Nubh..FThe 
+00001270: 7368 6f72 7466 6f72 6d20 6f66 2061 2073  shortform of a s
+00001280: 7570 706f 7274 6564 2070 726f 6772 616d  upported program
+00001290: 6d69 6e67 206c 616e 6775 6167 652e 2052  ming language. R
+000012a0: 6566 6572 2074 6f20 7468 6520 3a64 6f63  efer to the :doc
+000012b0: 3a20 9485 9481 947d 9428 681b 6a88 0100  : .....}.(h.j...
+000012c0: 0068 1c68 0368 1d4e 681e 4e75 6268 7929  .h.h.h.Nh.Nubhy)
+000012d0: 8194 7d94 2868 058c 3360 6c69 7374 206f  ..}.(h..3`list o
+000012e0: 6620 7375 7070 6f72 7465 6420 6c61 6e67  f supported lang
+000012f0: 7561 6765 7320 3c73 7570 706f 7274 6564  uages <supported
+00001300: 5f6c 616e 6775 6167 6573 3e60 9468 075d  _languages>`.h.]
+00001310: 9468 168c 316c 6973 7420 6f66 2073 7570  .h..1list of sup
+00001320: 706f 7274 6564 206c 616e 6775 6167 6573  ported languages
+00001330: 203c 7375 7070 6f72 7465 645f 6c61 6e67   <supported_lang
+00001340: 7561 6765 733e 9485 9481 947d 9428 681b  uages>.....}.(h.
+00001350: 6ad0 0100 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
+00001360: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
+00001370: 255d 9468 275d 9468 295d 9475 682b 6878  %].h'].h)].uh+hx
+00001380: 681b 6a88 0100 0068 1c68 0368 1d4e 681e  h.j....h.h.h.Nh.
+00001390: 4e75 6268 168c 012e 9485 9481 947d 9428  Nubh.........}.(
+000013a0: 681b 6a88 0100 0068 1c68 0368 1d4e 681e  h.j....h.h.h.Nh.
+000013b0: 4e75 6265 681f 7d94 2868 215d 9468 235d  Nubeh.}.(h!].h#]
+000013c0: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
+000013d0: 682d 681b 6a85 0100 0075 6261 681f 7d94  h-h.j....ubah.}.
+000013e0: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+000013f0: 9468 295d 9475 682b 686f 681b 6a82 0100  .h)].uh+hoh.j...
+00001400: 0075 6268 7029 8194 7d94 2868 0568 0668  .ubhp)..}.(h.h.h
+00001410: 075d 9468 2e29 8194 7d94 2868 058c 4a70  .].h.)..}.(h..Jp
+00001420: 726f 6a65 6374 6e61 6d65 2028 7374 7229  rojectname (str)
+00001430: 202d 2d20 5468 6520 6e61 6d65 206f 6620   -- The name of 
+00001440: 7468 6520 7072 6f6a 6563 7420 7061 636b  the project pack
+00001450: 6167 6520 7468 6174 2077 696c 6c20 6265  age that will be
+00001460: 2063 7265 6174 6564 2e94 6807 5d94 286a   created..h.].(j
+00001470: 8d01 0000 2981 947d 9428 6805 8c0b 7072  ....)..}.(h...pr
+00001480: 6f6a 6563 746e 616d 6594 6807 5d94 6816  ojectname.h.].h.
+00001490: 8c0b 7072 6f6a 6563 746e 616d 6594 8594  ..projectname...
+000014a0: 8194 7d94 2868 1b6a f501 0000 681c 6803  ..}.(h.j....h.h.
+000014b0: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
+000014c0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+000014d0: 5d94 7568 2b6a 8c01 0000 681b 6af1 0100  ].uh+j....h.j...
+000014e0: 0075 6268 168c 0220 2894 8594 8194 7d94  .ubh... (.....}.
+000014f0: 2868 1b6a f101 0000 681c 6803 681d 4e68  (h.j....h.h.h.Nh
+00001500: 1e4e 7562 6aa1 0100 0029 8194 7d94 2868  .Nubj....)..}.(h
+00001510: 0568 0668 075d 946a a601 0000 2981 947d  .h.h.].j....)..}
+00001520: 9428 6805 8c03 7374 7294 6807 5d94 6816  .(h...str.h.].h.
+00001530: 8c03 7374 7294 8594 8194 7d94 2868 1b6a  ..str.....}.(h.j
+00001540: 0a02 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
+00001550: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+00001560: 5d94 6827 5d94 6829 5d94 7568 2b6a a501  ].h'].h)].uh+j..
+00001570: 0000 681b 6a07 0200 0075 6261 681f 7d94  ..h.j....ubah.}.
+00001580: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+00001590: 9468 295d 948c 0972 6566 646f 6d61 696e  .h)]...refdomain
+000015a0: 946a bc01 0000 8c0b 7265 6665 7870 6c69  .j......refexpli
+000015b0: 6369 7494 898c 0772 6566 7479 7065 946a  cit....reftype.j
+000015c0: bf01 0000 8c09 7265 6674 6172 6765 7494  ......reftarget.
+000015d0: 6a0c 0200 006a c101 0000 886a c201 0000  j....j.....j....
+000015e0: 4e6a c301 0000 4e75 682b 6aa0 0100 0068  Nj....Nuh+j....h
+000015f0: 1b6a f101 0000 7562 6816 8c01 2994 8594  .j....ubh...)...
+00001600: 8194 7d94 2868 1b6a f101 0000 681c 6803  ..}.(h.j....h.h.
+00001610: 681d 4e68 1e4e 7562 6816 8c05 20e2 8093  h.Nh.Nubh... ...
+00001620: 2094 8594 8194 7d94 2868 1b6a f101 0000   .....}.(h.j....
+00001630: 681c 6803 681d 4e68 1e4e 7562 6816 8c35  h.h.h.Nh.Nubh..5
+00001640: 5468 6520 6e61 6d65 206f 6620 7468 6520  The name of the 
+00001650: 7072 6f6a 6563 7420 7061 636b 6167 6520  project package 
+00001660: 7468 6174 2077 696c 6c20 6265 2063 7265  that will be cre
+00001670: 6174 6564 2e94 8594 8194 7d94 2868 1b6a  ated......}.(h.j
+00001680: f101 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
+00001690: 6568 1f7d 9428 6821 5d94 6823 5d94 6825  eh.}.(h!].h#].h%
+000016a0: 5d94 6827 5d94 6829 5d94 7568 2b68 2d68  ].h'].h)].uh+h-h
+000016b0: 1b6a ee01 0000 7562 6168 1f7d 9428 6821  .j....ubah.}.(h!
+000016c0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+000016d0: 5d94 7568 2b68 6f68 1b6a 8201 0000 7562  ].uh+hoh.j....ub
+000016e0: 6870 2981 947d 9428 6805 6806 6807 5d94  hp)..}.(h.h.h.].
+000016f0: 682e 2981 947d 9428 6805 8cb6 2d67 7c2d  h.)..}.(h...-g|-
+00001700: 2d67 6974 2028 666c 6167 2920 2d2d 2041  -git (flag) -- A
+00001710: 6e20 6f70 7469 6f6e 616c 2066 6c61 6720  n optional flag 
+00001720: 746f 2069 6e69 7469 616c 697a 6520 6120  to initialize a 
+00001730: 4769 7420 7265 706f 7369 746f 7279 2069  Git repository i
+00001740: 6e20 7468 6520 7072 6f6a 6563 7420 6469  n the project di
+00001750: 7265 6374 6f72 792e 2049 6620 7370 6563  rectory. If spec
+00001760: 6966 6965 642c 2061 2047 6974 2072 6570  ified, a Git rep
+00001770: 6f73 6974 6f72 7920 7769 6c6c 2062 6520  ository will be 
+00001780: 6372 6561 7465 6420 7369 6d75 6c74 616e  created simultan
+00001790: 656f 7573 6c79 2077 6974 6820 7468 6520  eously with the 
+000017a0: 7072 6f6a 6563 7420 7374 7275 6374 7572  project structur
+000017b0: 652e 9468 075d 9428 6a8d 0100 0029 8194  e..h.].(j....)..
+000017c0: 7d94 2868 058c 022d 6794 6807 5d94 6816  }.(h...-g.h.].h.
+000017d0: 8c02 2d67 9485 9481 947d 9428 681b 6a41  ..-g.....}.(h.jA
+000017e0: 0200 0068 1c68 0368 1d4e 681e 4e75 6261  ...h.h.h.Nh.Nuba
+000017f0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+00001800: 9468 275d 9468 295d 9475 682b 6a8c 0100  .h'].h)].uh+j...
+00001810: 0068 1b6a 3d02 0000 7562 6a8d 0100 0029  .h.j=...ubj....)
+00001820: 8194 7d94 2868 058c 017c 9468 075d 9468  ..}.(h...|.h.].h
+00001830: 168c 017c 9485 9481 947d 9428 681b 6a4f  ...|.....}.(h.jO
+00001840: 0200 0068 1c68 0368 1d4e 681e 4e75 6261  ...h.h.h.Nh.Nuba
+00001850: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+00001860: 9468 275d 9468 295d 9475 682b 6a8c 0100  .h'].h)].uh+j...
+00001870: 0068 1b6a 3d02 0000 7562 6a8d 0100 0029  .h.j=...ubj....)
+00001880: 8194 7d94 2868 058c 052d 2d67 6974 9468  ..}.(h...--git.h
+00001890: 075d 9468 168c 052d 2d67 6974 9485 9481  .].h...--git....
+000018a0: 947d 9428 681b 6a5d 0200 0068 1c68 0368  .}.(h.j]...h.h.h
+000018b0: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
+000018c0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+000018d0: 9475 682b 6a8c 0100 0068 1b6a 3d02 0000  .uh+j....h.j=...
+000018e0: 7562 6816 8c02 2028 9485 9481 947d 9428  ubh... (.....}.(
+000018f0: 681b 6a3d 0200 0068 1c68 0368 1d4e 681e  h.j=...h.h.h.Nh.
+00001900: 4e75 626a a101 0000 2981 947d 9428 6805  Nubj....)..}.(h.
+00001910: 6806 6807 5d94 6aa6 0100 0029 8194 7d94  h.h.].j....)..}.
+00001920: 2868 058c 0466 6c61 6794 6807 5d94 6816  (h...flag.h.].h.
+00001930: 8c04 666c 6167 9485 9481 947d 9428 681b  ..flag.....}.(h.
+00001940: 6a72 0200 0068 1c68 0368 1d4e 681e 4e75  jr...h.h.h.Nh.Nu
+00001950: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
+00001960: 255d 9468 275d 9468 295d 9475 682b 6aa5  %].h'].h)].uh+j.
+00001970: 0100 0068 1b6a 6f02 0000 7562 6168 1f7d  ...h.jo...ubah.}
+00001980: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
+00001990: 5d94 6829 5d94 8c09 7265 6664 6f6d 6169  ].h)]...refdomai
+000019a0: 6e94 6abc 0100 008c 0b72 6566 6578 706c  n.j......refexpl
+000019b0: 6963 6974 9489 8c07 7265 6674 7970 6594  icit....reftype.
+000019c0: 6abf 0100 008c 0972 6566 7461 7267 6574  j......reftarget
+000019d0: 946a 7402 0000 6ac1 0100 0088 6ac2 0100  .jt...j.....j...
+000019e0: 004e 6ac3 0100 004e 7568 2b6a a001 0000  .Nj....Nuh+j....
+000019f0: 681b 6a3d 0200 0075 6268 168c 0129 9485  h.j=...ubh...)..
+00001a00: 9481 947d 9428 681b 6a3d 0200 0068 1c68  ...}.(h.j=...h.h
+00001a10: 0368 1d4e 681e 4e75 6268 168c 0520 e280  .h.Nh.Nubh... ..
+00001a20: 9320 9485 9481 947d 9428 681b 6a3d 0200  . .....}.(h.j=..
+00001a30: 0068 1c68 0368 1d4e 681e 4e75 6268 168c  .h.h.h.Nh.Nubh..
+00001a40: a341 6e20 6f70 7469 6f6e 616c 2066 6c61  .An optional fla
+00001a50: 6720 746f 2069 6e69 7469 616c 697a 6520  g to initialize 
+00001a60: 6120 4769 7420 7265 706f 7369 746f 7279  a Git repository
+00001a70: 2069 6e20 7468 6520 7072 6f6a 6563 7420   in the project 
+00001a80: 6469 7265 6374 6f72 792e 2049 6620 7370  directory. If sp
+00001a90: 6563 6966 6965 642c 2061 2047 6974 2072  ecified, a Git r
+00001aa0: 6570 6f73 6974 6f72 7920 7769 6c6c 2062  epository will b
+00001ab0: 6520 6372 6561 7465 6420 7369 6d75 6c74  e created simult
+00001ac0: 616e 656f 7573 6c79 2077 6974 6820 7468  aneously with th
+00001ad0: 6520 7072 6f6a 6563 7420 7374 7275 6374  e project struct
+00001ae0: 7572 652e 9485 9481 947d 9428 681b 6a3d  ure......}.(h.j=
+00001af0: 0200 0068 1c68 0368 1d4e 681e 4e75 6265  ...h.h.h.Nh.Nube
+00001b00: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+00001b10: 9468 275d 9468 295d 9475 682b 682d 681b  .h'].h)].uh+h-h.
+00001b20: 6a3a 0200 0075 6261 681f 7d94 2868 215d  j:...ubah.}.(h!]
+00001b30: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+00001b40: 9475 682b 686f 681b 6a82 0100 0075 6268  .uh+hoh.j....ubh
+00001b50: 7029 8194 7d94 2868 0568 0668 075d 9468  p)..}.(h.h.h.].h
+00001b60: 2e29 8194 7d94 2868 058c 572d 2d6e 6f2d  .)..}.(h..W--no-
+00001b70: 6c6f 6720 2866 6c61 6729 202d 2d20 416e  log (flag) -- An
+00001b80: 206f 7074 696f 6e61 6c20 666c 6167 2074   optional flag t
+00001b90: 6f20 6469 7361 626c 6520 7072 6f6a 6563  o disable projec
+00001ba0: 7420 6c6f 6767 696e 6720 666f 7220 7468  t logging for th
+00001bb0: 6520 6375 7272 656e 7420 7072 6f6a 6563  e current projec
+00001bc0: 742e 9468 075d 9428 6a8d 0100 0029 8194  t..h.].(j....)..
+00001bd0: 7d94 2868 058c 082d 2d6e 6f2d 6c6f 6794  }.(h...--no-log.
+00001be0: 6807 5d94 6816 8c08 2d2d 6e6f 2d6c 6f67  h.].h...--no-log
+00001bf0: 9485 9481 947d 9428 681b 6aa9 0200 0068  .....}.(h.j....h
+00001c00: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
+00001c10: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+00001c20: 9468 295d 9475 682b 6a8c 0100 0068 1b6a  .h)].uh+j....h.j
+00001c30: a502 0000 7562 6816 8c02 2028 9485 9481  ....ubh... (....
+00001c40: 947d 9428 681b 6aa5 0200 0068 1c68 0368  .}.(h.j....h.h.h
+00001c50: 1d4e 681e 4e75 626a a101 0000 2981 947d  .Nh.Nubj....)..}
+00001c60: 9428 6805 6806 6807 5d94 6aa6 0100 0029  .(h.h.h.].j....)
+00001c70: 8194 7d94 2868 058c 0466 6c61 6794 6807  ..}.(h...flag.h.
+00001c80: 5d94 6816 8c04 666c 6167 9485 9481 947d  ].h...flag.....}
+00001c90: 9428 681b 6abe 0200 0068 1c68 0368 1d4e  .(h.j....h.h.h.N
+00001ca0: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
+00001cb0: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
+00001cc0: 682b 6aa5 0100 0068 1b6a bb02 0000 7562  h+j....h.j....ub
+00001cd0: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+00001ce0: 5d94 6827 5d94 6829 5d94 8c09 7265 6664  ].h'].h)]...refd
+00001cf0: 6f6d 6169 6e94 6abc 0100 008c 0b72 6566  omain.j......ref
+00001d00: 6578 706c 6963 6974 9489 8c07 7265 6674  explicit....reft
+00001d10: 7970 6594 6abf 0100 008c 0972 6566 7461  ype.j......refta
+00001d20: 7267 6574 946a c002 0000 6ac1 0100 0088  rget.j....j.....
+00001d30: 6ac2 0100 004e 6ac3 0100 004e 7568 2b6a  j....Nj....Nuh+j
+00001d40: a001 0000 681b 6aa5 0200 0075 6268 168c  ....h.j....ubh..
+00001d50: 0129 9485 9481 947d 9428 681b 6aa5 0200  .).....}.(h.j...
+00001d60: 0068 1c68 0368 1d4e 681e 4e75 6268 168c  .h.h.h.Nh.Nubh..
+00001d70: 0520 e280 9320 9485 9481 947d 9428 681b  . ... .....}.(h.
+00001d80: 6aa5 0200 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
+00001d90: 6268 168c 4441 6e20 6f70 7469 6f6e 616c  bh..DAn optional
+00001da0: 2066 6c61 6720 746f 2064 6973 6162 6c65   flag to disable
+00001db0: 2070 726f 6a65 6374 206c 6f67 6769 6e67   project logging
+00001dc0: 2066 6f72 2074 6865 2063 7572 7265 6e74   for the current
+00001dd0: 2070 726f 6a65 6374 2e94 8594 8194 7d94   project......}.
+00001de0: 2868 1b6a a502 0000 681c 6803 681d 4e68  (h.j....h.h.h.Nh
+00001df0: 1e4e 7562 6568 1f7d 9428 6821 5d94 6823  .Nubeh.}.(h!].h#
+00001e00: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
+00001e10: 2b68 2d68 1b6a a202 0000 7562 6168 1f7d  +h-h.j....ubah.}
+00001e20: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
+00001e30: 5d94 6829 5d94 7568 2b68 6f68 1b6a 8201  ].h)].uh+hoh.j..
+00001e40: 0000 7562 6568 1f7d 9428 6821 5d94 6823  ..ubeh.}.(h!].h#
+00001e50: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
+00001e60: 2b68 6a68 1b6a 7f01 0000 7562 6168 1f7d  +hjh.j....ubah.}
+00001e70: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
+00001e80: 5d94 6829 5d94 7568 2b6a 7d01 0000 681b  ].h)].uh+j}...h.
+00001e90: 6a6a 0100 0075 6265 681f 7d94 2868 215d  jj...ubeh.}.(h!]
+00001ea0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+00001eb0: 9475 682b 6a68 0100 0068 1b6a 6501 0000  .uh+jh...h.je...
+00001ec0: 7562 6a69 0100 0029 8194 7d94 2868 0568  ubji...)..}.(h.h
+00001ed0: 0668 075d 9428 6a6e 0100 0029 8194 7d94  .h.].(jn...)..}.
+00001ee0: 2868 058c 0752 6574 7572 6e73 9468 075d  (h...Returns.h.]
+00001ef0: 9468 168c 0752 6574 7572 6e73 9485 9481  .h...Returns....
+00001f00: 947d 9428 681b 6a03 0300 0068 1c68 0368  .}.(h.j....h.h.h
+00001f10: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
+00001f20: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+00001f30: 9475 682b 6a6d 0100 0068 1b6a 0003 0000  .uh+jm...h.j....
+00001f40: 681d 682c 681e 4b00 7562 6a7e 0100 0029  h.h,h.K.ubj~...)
+00001f50: 8194 7d94 2868 0568 0668 075d 9468 2e29  ..}.(h.h.h.].h.)
+00001f60: 8194 7d94 2868 058c 044e 6f6e 6594 6807  ..}.(h...None.h.
+00001f70: 5d94 6816 8c04 4e6f 6e65 9485 9481 947d  ].h...None.....}
+00001f80: 9428 681b 6a14 0300 0068 1c68 0368 1d4e  .(h.j....h.h.h.N
+00001f90: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
+00001fa0: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
+00001fb0: 682b 682d 681b 6a11 0300 0075 6261 681f  h+h-h.j....ubah.
+00001fc0: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+00001fd0: 275d 9468 295d 9475 682b 6a7d 0100 0068  '].h)].uh+j}...h
+00001fe0: 1b6a 0003 0000 7562 6568 1f7d 9428 6821  .j....ubeh.}.(h!
+00001ff0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+00002000: 5d94 7568 2b6a 6801 0000 681b 6a65 0100  ].uh+jh...h.je..
+00002010: 0075 626a 6901 0000 2981 947d 9428 6805  .ubji...)..}.(h.
+00002020: 6806 6807 5d94 286a 6e01 0000 2981 947d  h.h.].(jn...)..}
+00002030: 9428 6805 8c0b 5265 7475 726e 2074 7970  .(h...Return typ
+00002040: 6594 6807 5d94 6816 8c0b 5265 7475 726e  e.h.].h...Return
+00002050: 2074 7970 6594 8594 8194 7d94 2868 1b6a   type.....}.(h.j
+00002060: 3103 0000 681c 6803 681d 4e68 1e4e 7562  1...h.h.h.Nh.Nub
+00002070: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+00002080: 5d94 6827 5d94 6829 5d94 7568 2b6a 6d01  ].h'].h)].uh+jm.
+00002090: 0000 681b 6a2e 0300 0068 1d68 2c68 1e4b  ..h.j....h.h,h.K
+000020a0: 0075 626a 7e01 0000 2981 947d 9428 6805  .ubj~...)..}.(h.
+000020b0: 6806 6807 5d94 682e 2981 947d 9428 6805  h.h.].h.)..}.(h.
+000020c0: 8c04 4e6f 6e65 9468 075d 946a a101 0000  ..None.h.].j....
+000020d0: 2981 947d 9428 6805 6806 6807 5d94 6816  )..}.(h.h.h.].h.
+000020e0: 8c04 4e6f 6e65 9485 9481 947d 9428 681b  ..None.....}.(h.
+000020f0: 6a46 0300 0068 1c68 0368 1d4e 681e 4e75  jF...h.h.h.Nh.Nu
+00002100: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
+00002110: 255d 9468 275d 9468 295d 948c 0972 6566  %].h'].h)]...ref
+00002120: 646f 6d61 696e 946a bc01 0000 8c0b 7265  domain.j......re
+00002130: 6665 7870 6c69 6369 7494 898c 0772 6566  fexplicit....ref
+00002140: 7479 7065 946a bf01 0000 8c09 7265 6674  type.j......reft
+00002150: 6172 6765 7494 8c04 4e6f 6e65 946a c101  arget...None.j..
+00002160: 0000 886a c201 0000 4e6a c301 0000 4e75  ...j....Nj....Nu
+00002170: 682b 6aa0 0100 0068 1b6a 4203 0000 7562  h+j....h.jB...ub
+00002180: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+00002190: 5d94 6827 5d94 6829 5d94 7568 2b68 2d68  ].h'].h)].uh+h-h
+000021a0: 1b6a 3f03 0000 7562 6168 1f7d 9428 6821  .j?...ubah.}.(h!
+000021b0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+000021c0: 5d94 7568 2b6a 7d01 0000 681b 6a2e 0300  ].uh+j}...h.j...
+000021d0: 0075 6265 681f 7d94 2868 215d 9468 235d  .ubeh.}.(h!].h#]
+000021e0: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
+000021f0: 6a68 0100 0068 1b6a 6501 0000 7562 6568  jh...h.je...ubeh
+00002200: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+00002210: 6827 5d94 6829 5d94 7568 2b6a 6301 0000  h'].h)].uh+jc...
+00002220: 681b 6a52 0100 0068 1c68 0368 1d4e 681e  h.jR...h.h.h.Nh.
+00002230: 4e75 6265 681f 7d94 2868 215d 9468 235d  Nubeh.}.(h!].h#]
+00002240: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
+00002250: 6a50 0100 0068 1b6a 2a01 0000 681c 6803  jP...h.j*...h.h.
+00002260: 681d 682c 681e 4b19 7562 6568 1f7d 9428  h.h,h.K.ubeh.}.(
+00002270: 6821 5d94 6823 5d94 286a bc01 0000 8c08  h!].h#].(j......
+00002280: 6675 6e63 7469 6f6e 9465 6825 5d94 6827  function.eh%].h'
+00002290: 5d94 6829 5d94 8c06 646f 6d61 696e 946a  ].h)]...domain.j
+000022a0: bc01 0000 8c07 6f62 6a74 7970 6594 6a79  ......objtype.jy
+000022b0: 0300 008c 0864 6573 6374 7970 6594 6a79  .....desctype.jy
+000022c0: 0300 008c 076e 6f69 6e64 6578 9489 8c0c  .....noindex....
+000022d0: 6e6f 696e 6465 7865 6e74 7279 9489 8c0f  noindexentry....
+000022e0: 6e6f 636f 6e74 656e 7473 656e 7472 7994  nocontentsentry.
+000022f0: 8975 682b 6a28 0100 0068 1c68 0368 1b6a  .uh+j(...h.h.h.j
+00002300: 0a01 0000 681d 4e68 1e4e 7562 6568 1f7d  ....h.Nh.Nubeh.}
+00002310: 9428 6821 5d94 8c0d 6e65 7374 6572 2d63  .(h!]...nester-c
+00002320: 7265 6174 6594 6168 235d 9468 255d 948c  reate.ah#].h%]..
+00002330: 0d6e 6573 7465 7220 6372 6561 7465 9461  .nester create.a
+00002340: 6827 5d94 6829 5d94 7568 2b68 0a68 1b68  h'].h)].uh+h.h.h
+00002350: 4b68 1c68 0368 1d68 2c68 1e4b 1775 6268  Kh.h.h.h,h.K.ubh
+00002360: 0b29 8194 7d94 2868 0568 0668 075d 9428  .)..}.(h.h.h.].(
+00002370: 6810 2981 947d 9428 6805 8c0f 4e65 7374  h.)..}.(h...Nest
+00002380: 6572 2076 616c 6964 6174 6594 6807 5d94  er validate.h.].
+00002390: 6816 8c0f 4e65 7374 6572 2076 616c 6964  h...Nester valid
+000023a0: 6174 6594 8594 8194 7d94 2868 1b6a 8e03  ate.....}.(h.j..
+000023b0: 0000 681c 6803 681d 4e68 1e4e 7562 6168  ..h.h.h.Nh.Nubah
+000023c0: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+000023d0: 6827 5d94 6829 5d94 7568 2b68 0f68 1b6a  h'].h)].uh+h.h.j
+000023e0: 8b03 0000 681c 6803 681d 682c 681e 4b2b  ....h.h.h.h,h.K+
+000023f0: 7562 6a1c 0100 0029 8194 7d94 2868 0568  ubj....)..}.(h.h
+00002400: 0668 075d 9468 1f7d 9428 6821 5d94 6823  .h.].h.}.(h!].h#
+00002410: 5d94 6825 5d94 6827 5d94 6829 5d94 8c07  ].h%].h'].h)]...
+00002420: 656e 7472 6965 7394 5d94 7568 2b6a 1b01  entries.].uh+j..
+00002430: 0000 681b 6a8b 0300 0068 1c68 0368 1d4e  ..h.j....h.h.h.N
+00002440: 681e 4e75 626a 2901 0000 2981 947d 9428  h.Nubj)...)..}.(
+00002450: 6805 6806 6807 5d94 286a 2e01 0000 2981  h.h.h.].(j....).
+00002460: 947d 9428 6805 8c26 6e65 7374 6572 2076  .}.(h..&nester v
+00002470: 616c 6964 6174 6528 6c61 6e67 7561 6765  alidate(language
+00002480: 2c20 7072 6f6a 6563 746e 616d 6529 9468  , projectname).h
+00002490: 075d 946a 3401 0000 2981 947d 9428 6805  .].j4...)..}.(h.
+000024a0: 6aac 0300 0068 075d 9468 168c 266e 6573  j....h.].h..&nes
+000024b0: 7465 7220 7661 6c69 6461 7465 286c 616e  ter validate(lan
+000024c0: 6775 6167 652c 2070 726f 6a65 6374 6e61  guage, projectna
+000024d0: 6d65 2994 8594 8194 7d94 2868 1b6a ae03  me).....}.(h.j..
+000024e0: 0000 681c 6803 681d 4e68 1e4e 7562 6168  ..h.h.h.Nh.Nubah
+000024f0: 1f7d 9428 6821 5d94 6823 5d94 286a 3f01  .}.(h!].h#].(j?.
+00002500: 0000 6a40 0100 0065 6825 5d94 6827 5d94  ..j@...eh%].h'].
+00002510: 6829 5d94 6a44 0100 006a 4501 0000 7568  h)].jD...jE...uh
+00002520: 2b6a 3301 0000 681b 6aaa 0300 0068 1c68  +j3...h.j....h.h
+00002530: 0368 1d68 2c68 1e4b 2d75 6261 681f 7d94  .h.h,h.K-ubah.}.
+00002540: 2868 215d 9468 235d 9428 6a49 0100 006a  (h!].h#].(jI...j
+00002550: 4a01 0000 6568 255d 9468 275d 9468 295d  J...eh%].h'].h)]
+00002560: 946a 4e01 0000 296a 4f01 0000 6806 7568  .jN...)jO...h.uh
+00002570: 2b6a 2d01 0000 681d 682c 681e 4b2d 681b  +j-...h.h,h.K-h.
+00002580: 6aa7 0300 0068 1c68 0375 626a 5101 0000  j....h.h.ubjQ...
+00002590: 2981 947d 9428 6805 6806 6807 5d94 2868  )..}.(h.h.h.].(h
+000025a0: 2e29 8194 7d94 2868 058c e056 616c 6964  .)..}.(h...Valid
+000025b0: 6174 6573 2074 6865 2066 696c 6520 7374  ates the file st
+000025c0: 7275 6374 7572 6520 6f66 2074 6865 2067  ructure of the g
+000025d0: 6976 656e 2070 726f 6a65 6374 2061 6761  iven project aga
+000025e0: 696e 7374 206f 7572 204a 534f 4e20 7363  inst our JSON sc
+000025f0: 686d 656d 6173 2e0a 4669 6c65 7320 796f  hmemas..Files yo
+00002600: 7520 6372 6561 7465 642c 2077 6869 6368  u created, which
+00002610: 2061 7265 2074 6865 7265 666f 7265 206e   are therefore n
+00002620: 6f74 2070 6172 7420 6f66 206f 7572 2073  ot part of our s
+00002630: 6368 656d 612c 206f 7220 7375 6368 2077  chema, or such w
+00002640: 6869 6368 2068 6176 6520 6265 656e 2063  hich have been c
+00002650: 7265 6174 6564 2062 7920 6f74 6865 7220  reated by other 
+00002660: 7574 696c 6974 6573 2028 652e 672e 2060  utilites (e.g. `
+00002670: 6769 7420 696e 6974 6029 2077 696c 6c20  git init`) will 
+00002680: 6265 2069 676e 6f72 6564 2e94 6807 5d94  be ignored..h.].
+00002690: 2868 168c c456 616c 6964 6174 6573 2074  (h...Validates t
+000026a0: 6865 2066 696c 6520 7374 7275 6374 7572  he file structur
+000026b0: 6520 6f66 2074 6865 2067 6976 656e 2070  e of the given p
+000026c0: 726f 6a65 6374 2061 6761 696e 7374 206f  roject against o
+000026d0: 7572 204a 534f 4e20 7363 686d 656d 6173  ur JSON schmemas
+000026e0: 2e0a 4669 6c65 7320 796f 7520 6372 6561  ..Files you crea
+000026f0: 7465 642c 2077 6869 6368 2061 7265 2074  ted, which are t
+00002700: 6865 7265 666f 7265 206e 6f74 2070 6172  herefore not par
+00002710: 7420 6f66 206f 7572 2073 6368 656d 612c  t of our schema,
+00002720: 206f 7220 7375 6368 2077 6869 6368 2068   or such which h
+00002730: 6176 6520 6265 656e 2063 7265 6174 6564  ave been created
+00002740: 2062 7920 6f74 6865 7220 7574 696c 6974   by other utilit
+00002750: 6573 2028 652e 672e 2094 8594 8194 7d94  es (e.g. .....}.
+00002760: 2868 1b6a c403 0000 681c 6803 681d 4e68  (h.j....h.h.h.Nh
+00002770: 1e4e 7562 6879 2981 947d 9428 6805 8c0a  .Nubhy)..}.(h...
+00002780: 6067 6974 2069 6e69 7460 9468 075d 9468  `git init`.h.].h
+00002790: 168c 0867 6974 2069 6e69 7494 8594 8194  ...git init.....
+000027a0: 7d94 2868 1b6a cc03 0000 681c 6803 681d  }.(h.j....h.h.h.
+000027b0: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
+000027c0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+000027d0: 7568 2b68 7868 1b6a c403 0000 7562 6816  uh+hxh.j....ubh.
+000027e0: 8c12 2920 7769 6c6c 2062 6520 6967 6e6f  ..) will be igno
+000027f0: 7265 642e 9485 9481 947d 9428 681b 6ac4  red......}.(h.j.
+00002800: 0300 0068 1c68 0368 1d4e 681e 4e75 6265  ...h.h.h.Nh.Nube
+00002810: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+00002820: 9468 275d 9468 295d 9475 682b 682d 681d  .h'].h)].uh+h-h.
+00002830: 682c 681e 4b2f 681b 6ac1 0300 0068 1c68  h,h.K/h.j....h.h
+00002840: 0375 626a 6401 0000 2981 947d 9428 6805  .ubjd...)..}.(h.
+00002850: 6806 6807 5d94 286a 6901 0000 2981 947d  h.h.].(ji...)..}
+00002860: 9428 6805 6806 6807 5d94 286a 6e01 0000  .(h.h.h.].(jn...
+00002870: 2981 947d 9428 6805 8c0a 5061 7261 6d65  )..}.(h...Parame
+00002880: 7465 7273 9468 075d 9468 168c 0a50 6172  ters.h.].h...Par
+00002890: 616d 6574 6572 7394 8594 8194 7d94 2868  ameters.....}.(h
+000028a0: 1b6a ea03 0000 681c 6803 681d 4e68 1e4e  .j....h.h.h.Nh.N
+000028b0: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+000028c0: 6825 5d94 6827 5d94 6829 5d94 7568 2b6a  h%].h'].h)].uh+j
+000028d0: 6d01 0000 681b 6ae7 0300 0068 1d68 2c68  m...h.j....h.h,h
+000028e0: 1e4b 0075 626a 7e01 0000 2981 947d 9428  .K.ubj~...)..}.(
+000028f0: 6805 6806 6807 5d94 686b 2981 947d 9428  h.h.h.].hk)..}.(
+00002900: 6805 6806 6807 5d94 2868 7029 8194 7d94  h.h.h.].(hp)..}.
+00002910: 2868 0568 0668 075d 9468 2e29 8194 7d94  (h.h.h.].h.)..}.
+00002920: 2868 058c 8a6c 616e 6775 6167 6520 2873  (h...language (s
+00002930: 7472 2920 2d2d 2054 6865 2073 686f 7274  tr) -- The short
+00002940: 666f 726d 206f 6620 6120 7375 7070 6f72  form of a suppor
+00002950: 7465 6420 7072 6f67 7261 6d6d 696e 6720  ted programming 
+00002960: 6c61 6e67 7561 6765 2e20 5265 6665 7220  language. Refer 
+00002970: 746f 2074 6865 203a 646f 633a 206c 6973  to the :doc: lis
+00002980: 7420 6f66 2073 7570 706f 7274 6564 206c  t of supported l
+00002990: 616e 6775 6167 6573 203c 7375 7070 6f72  anguages <suppor
+000029a0: 7465 645f 6c61 6e67 7561 6765 733e 2e94  ted_languages>..
+000029b0: 6807 5d94 286a 8d01 0000 2981 947d 9428  h.].(j....)..}.(
+000029c0: 6805 8c08 6c61 6e67 7561 6765 9468 075d  h...language.h.]
+000029d0: 9468 168c 086c 616e 6775 6167 6594 8594  .h...language...
+000029e0: 8194 7d94 2868 1b6a 0504 0000 681c 6803  ..}.(h.j....h.h.
+000029f0: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
+00002a00: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+00002a10: 5d94 7568 2b6a 8c01 0000 681b 6a01 0400  ].uh+j....h.j...
+00002a20: 0075 6268 168c 0220 2894 8594 8194 7d94  .ubh... (.....}.
+00002a30: 2868 1b6a 0104 0000 681c 6803 681d 4e68  (h.j....h.h.h.Nh
+00002a40: 1e4e 7562 6aa1 0100 0029 8194 7d94 2868  .Nubj....)..}.(h
+00002a50: 0568 0668 075d 946a a601 0000 2981 947d  .h.h.].j....)..}
+00002a60: 9428 6805 8c03 7374 7294 6807 5d94 6816  .(h...str.h.].h.
+00002a70: 8c03 7374 7294 8594 8194 7d94 2868 1b6a  ..str.....}.(h.j
+00002a80: 1a04 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
+00002a90: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+00002aa0: 5d94 6827 5d94 6829 5d94 7568 2b6a a501  ].h'].h)].uh+j..
+00002ab0: 0000 681b 6a17 0400 0075 6261 681f 7d94  ..h.j....ubah.}.
+00002ac0: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+00002ad0: 9468 295d 948c 0972 6566 646f 6d61 696e  .h)]...refdomain
+00002ae0: 948c 0270 7994 8c0b 7265 6665 7870 6c69  ...py...refexpli
+00002af0: 6369 7494 898c 0772 6566 7479 7065 946a  cit....reftype.j
+00002b00: bf01 0000 8c09 7265 6674 6172 6765 7494  ......reftarget.
+00002b10: 6a1c 0400 006a c101 0000 886a c201 0000  j....j.....j....
+00002b20: 4e6a c301 0000 4e75 682b 6aa0 0100 0068  Nj....Nuh+j....h
+00002b30: 1b6a 0104 0000 7562 6816 8c01 2994 8594  .j....ubh...)...
+00002b40: 8194 7d94 2868 1b6a 0104 0000 681c 6803  ..}.(h.j....h.h.
+00002b50: 681d 4e68 1e4e 7562 6816 8c05 20e2 8093  h.Nh.Nubh... ...
+00002b60: 2094 8594 8194 7d94 2868 1b6a 0104 0000   .....}.(h.j....
+00002b70: 681c 6803 681d 4e68 1e4e 7562 6816 8c46  h.h.h.Nh.Nubh..F
+00002b80: 5468 6520 7368 6f72 7466 6f72 6d20 6f66  The shortform of
+00002b90: 2061 2073 7570 706f 7274 6564 2070 726f   a supported pro
+00002ba0: 6772 616d 6d69 6e67 206c 616e 6775 6167  gramming languag
+00002bb0: 652e 2052 6566 6572 2074 6f20 7468 6520  e. Refer to the 
+00002bc0: 3a64 6f63 3a20 9485 9481 947d 9428 681b  :doc: .....}.(h.
+00002bd0: 6a01 0400 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
+00002be0: 6268 7929 8194 7d94 2868 058c 3360 6c69  bhy)..}.(h..3`li
+00002bf0: 7374 206f 6620 7375 7070 6f72 7465 6420  st of supported 
+00002c00: 6c61 6e67 7561 6765 7320 3c73 7570 706f  languages <suppo
+00002c10: 7274 6564 5f6c 616e 6775 6167 6573 3e60  rted_languages>`
+00002c20: 9468 075d 9468 168c 316c 6973 7420 6f66  .h.].h..1list of
+00002c30: 2073 7570 706f 7274 6564 206c 616e 6775   supported langu
+00002c40: 6167 6573 203c 7375 7070 6f72 7465 645f  ages <supported_
+00002c50: 6c61 6e67 7561 6765 733e 9485 9481 947d  languages>.....}
+00002c60: 9428 681b 6a3f 0400 0068 1c68 0368 1d4e  .(h.j?...h.h.h.N
+00002c70: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
+00002c80: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
+00002c90: 682b 6878 681b 6a01 0400 0068 1c68 0368  h+hxh.j....h.h.h
+00002ca0: 1d4e 681e 4e75 6268 168c 012e 9485 9481  .Nh.Nubh........
+00002cb0: 947d 9428 681b 6a01 0400 0068 1c68 0368  .}.(h.j....h.h.h
+00002cc0: 1d4e 681e 4e75 6265 681f 7d94 2868 215d  .Nh.Nubeh.}.(h!]
+00002cd0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+00002ce0: 9475 682b 682d 681b 6afe 0300 0075 6261  .uh+h-h.j....uba
+00002cf0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+00002d00: 9468 275d 9468 295d 9475 682b 686f 681b  .h'].h)].uh+hoh.
+00002d10: 6afb 0300 0075 6268 7029 8194 7d94 2868  j....ubhp)..}.(h
+00002d20: 0568 0668 075d 9468 2e29 8194 7d94 2868  .h.h.].h.)..}.(h
+00002d30: 058c 4c70 726f 6a65 6374 6e61 6d65 2028  ..Lprojectname (
+00002d40: 7374 7229 202d 2d20 5468 6520 6e61 6d65  str) -- The name
+00002d50: 206f 6620 7468 6520 7072 6f6a 6563 7420   of the project 
+00002d60: 6f72 2070 6163 6b61 6765 2079 6f75 2077  or package you w
+00002d70: 616e 7420 746f 2076 616c 6964 6174 6594  ant to validate.
+00002d80: 6807 5d94 286a 8d01 0000 2981 947d 9428  h.].(j....)..}.(
+00002d90: 6805 8c0b 7072 6f6a 6563 746e 616d 6594  h...projectname.
+00002da0: 6807 5d94 6816 8c0b 7072 6f6a 6563 746e  h.].h...projectn
+00002db0: 616d 6594 8594 8194 7d94 2868 1b6a 6404  ame.....}.(h.jd.
+00002dc0: 0000 681c 6803 681d 4e68 1e4e 7562 6168  ..h.h.h.Nh.Nubah
+00002dd0: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+00002de0: 6827 5d94 6829 5d94 7568 2b6a 8c01 0000  h'].h)].uh+j....
+00002df0: 681b 6a60 0400 0075 6268 168c 0220 2894  h.j`...ubh... (.
+00002e00: 8594 8194 7d94 2868 1b6a 6004 0000 681c  ....}.(h.j`...h.
+00002e10: 6803 681d 4e68 1e4e 7562 6aa1 0100 0029  h.h.Nh.Nubj....)
+00002e20: 8194 7d94 2868 0568 0668 075d 946a a601  ..}.(h.h.h.].j..
+00002e30: 0000 2981 947d 9428 6805 8c03 7374 7294  ..)..}.(h...str.
+00002e40: 6807 5d94 6816 8c03 7374 7294 8594 8194  h.].h...str.....
+00002e50: 7d94 2868 1b6a 7904 0000 681c 6803 681d  }.(h.jy...h.h.h.
+00002e60: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
+00002e70: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+00002e80: 7568 2b6a a501 0000 681b 6a76 0400 0075  uh+j....h.jv...u
+00002e90: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
+00002ea0: 255d 9468 275d 9468 295d 948c 0972 6566  %].h'].h)]...ref
+00002eb0: 646f 6d61 696e 946a 2f04 0000 8c0b 7265  domain.j/.....re
+00002ec0: 6665 7870 6c69 6369 7494 898c 0772 6566  fexplicit....ref
+00002ed0: 7479 7065 946a bf01 0000 8c09 7265 6674  type.j......reft
+00002ee0: 6172 6765 7494 6a7b 0400 006a c101 0000  arget.j{...j....
+00002ef0: 886a c201 0000 4e6a c301 0000 4e75 682b  .j....Nj....Nuh+
+00002f00: 6aa0 0100 0068 1b6a 6004 0000 7562 6816  j....h.j`...ubh.
+00002f10: 8c01 2994 8594 8194 7d94 2868 1b6a 6004  ..).....}.(h.j`.
+00002f20: 0000 681c 6803 681d 4e68 1e4e 7562 6816  ..h.h.h.Nh.Nubh.
+00002f30: 8c05 20e2 8093 2094 8594 8194 7d94 2868  .. ... .....}.(h
+00002f40: 1b6a 6004 0000 681c 6803 681d 4e68 1e4e  .j`...h.h.h.Nh.N
+00002f50: 7562 6816 8c37 5468 6520 6e61 6d65 206f  ubh..7The name o
+00002f60: 6620 7468 6520 7072 6f6a 6563 7420 6f72  f the project or
+00002f70: 2070 6163 6b61 6765 2079 6f75 2077 616e   package you wan
+00002f80: 7420 746f 2076 616c 6964 6174 6594 8594  t to validate...
+00002f90: 8194 7d94 2868 1b6a 6004 0000 681c 6803  ..}.(h.j`...h.h.
+00002fa0: 681d 4e68 1e4e 7562 6568 1f7d 9428 6821  h.Nh.Nubeh.}.(h!
+00002fb0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+00002fc0: 5d94 7568 2b68 2d68 1b6a 5d04 0000 7562  ].uh+h-h.j]...ub
+00002fd0: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+00002fe0: 5d94 6827 5d94 6829 5d94 7568 2b68 6f68  ].h'].h)].uh+hoh
+00002ff0: 1b6a fb03 0000 7562 6568 1f7d 9428 6821  .j....ubeh.}.(h!
+00003000: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+00003010: 5d94 7568 2b68 6a68 1b6a f803 0000 7562  ].uh+hjh.j....ub
+00003020: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+00003030: 5d94 6827 5d94 6829 5d94 7568 2b6a 7d01  ].h'].h)].uh+j}.
+00003040: 0000 681b 6ae7 0300 0075 6265 681f 7d94  ..h.j....ubeh.}.
+00003050: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+00003060: 9468 295d 9475 682b 6a68 0100 0068 1b6a  .h)].uh+jh...h.j
+00003070: e403 0000 7562 6a69 0100 0029 8194 7d94  ....ubji...)..}.
+00003080: 2868 0568 0668 075d 9428 6a6e 0100 0029  (h.h.h.].(jn...)
+00003090: 8194 7d94 2868 058c 0752 6574 7572 6e73  ..}.(h...Returns
+000030a0: 9468 075d 9468 168c 0752 6574 7572 6e73  .h.].h...Returns
+000030b0: 9485 9481 947d 9428 681b 6abe 0400 0068  .....}.(h.j....h
+000030c0: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
+000030d0: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+000030e0: 9468 295d 9475 682b 6a6d 0100 0068 1b6a  .h)].uh+jm...h.j
+000030f0: bb04 0000 681d 682c 681e 4b00 7562 6a7e  ....h.h,h.K.ubj~
+00003100: 0100 0029 8194 7d94 2868 0568 0668 075d  ...)..}.(h.h.h.]
+00003110: 9468 2e29 8194 7d94 2868 058c 3d54 656c  .h.)..}.(h..=Tel
+00003120: 6c73 2079 6f75 2076 6961 2054 6572 6d69  ls you via Termi
+00003130: 6e61 6c20 7765 7468 6572 2079 6f75 7220  nal wether your 
+00003140: 7374 7275 6374 7572 6520 6c69 6e65 7320  structure lines 
+00003150: 7570 206f 7220 6e6f 742e 9468 075d 9468  up or not..h.].h
+00003160: 168c 3d54 656c 6c73 2079 6f75 2076 6961  ..=Tells you via
+00003170: 2054 6572 6d69 6e61 6c20 7765 7468 6572   Terminal wether
+00003180: 2079 6f75 7220 7374 7275 6374 7572 6520   your structure 
+00003190: 6c69 6e65 7320 7570 206f 7220 6e6f 742e  lines up or not.
+000031a0: 9485 9481 947d 9428 681b 6acf 0400 0068  .....}.(h.j....h
+000031b0: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
+000031c0: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+000031d0: 9468 295d 9475 682b 682d 681b 6acc 0400  .h)].uh+h-h.j...
+000031e0: 0075 6261 681f 7d94 2868 215d 9468 235d  .ubah.}.(h!].h#]
+000031f0: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
+00003200: 6a7d 0100 0068 1b6a bb04 0000 7562 6568  j}...h.j....ubeh
+00003210: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+00003220: 6827 5d94 6829 5d94 7568 2b6a 6801 0000  h'].h)].uh+jh...
+00003230: 681b 6ae4 0300 0075 626a 6901 0000 2981  h.j....ubji...).
+00003240: 947d 9428 6805 6806 6807 5d94 286a 6e01  .}.(h.h.h.].(jn.
+00003250: 0000 2981 947d 9428 6805 8c0b 5265 7475  ..)..}.(h...Retu
+00003260: 726e 2074 7970 6594 6807 5d94 6816 8c0b  rn type.h.].h...
+00003270: 5265 7475 726e 2074 7970 6594 8594 8194  Return type.....
+00003280: 7d94 2868 1b6a ec04 0000 681c 6803 681d  }.(h.j....h.h.h.
+00003290: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
+000032a0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+000032b0: 7568 2b6a 6d01 0000 681b 6ae9 0400 0068  uh+jm...h.j....h
+000032c0: 1d68 2c68 1e4b 0075 626a 7e01 0000 2981  .h,h.K.ubj~...).
+000032d0: 947d 9428 6805 6806 6807 5d94 682e 2981  .}.(h.h.h.].h.).
+000032e0: 947d 9428 6805 8c03 7374 7294 6807 5d94  .}.(h...str.h.].
+000032f0: 6aa1 0100 0029 8194 7d94 2868 0568 0668  j....)..}.(h.h.h
+00003300: 075d 9468 168c 0373 7472 9485 9481 947d  .].h...str.....}
+00003310: 9428 681b 6a01 0500 0068 1c68 0368 1d4e  .(h.j....h.h.h.N
+00003320: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
+00003330: 235d 9468 255d 9468 275d 9468 295d 948c  #].h%].h'].h)]..
+00003340: 0972 6566 646f 6d61 696e 946a 2f04 0000  .refdomain.j/...
+00003350: 8c0b 7265 6665 7870 6c69 6369 7494 898c  ..refexplicit...
+00003360: 0772 6566 7479 7065 946a bf01 0000 8c09  .reftype.j......
+00003370: 7265 6674 6172 6765 7494 8c03 7374 7294  reftarget...str.
+00003380: 6ac1 0100 0088 6ac2 0100 004e 6ac3 0100  j.....j....Nj...
+00003390: 004e 7568 2b6a a001 0000 681b 6afd 0400  .Nuh+j....h.j...
+000033a0: 0075 6261 681f 7d94 2868 215d 9468 235d  .ubah.}.(h!].h#]
+000033b0: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
+000033c0: 682d 681b 6afa 0400 0075 6261 681f 7d94  h-h.j....ubah.}.
+000033d0: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+000033e0: 9468 295d 9475 682b 6a7d 0100 0068 1b6a  .h)].uh+j}...h.j
+000033f0: e904 0000 7562 6568 1f7d 9428 6821 5d94  ....ubeh.}.(h!].
+00003400: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+00003410: 7568 2b6a 6801 0000 681b 6ae4 0300 0075  uh+jh...h.j....u
+00003420: 6265 681f 7d94 2868 215d 9468 235d 9468  beh.}.(h!].h#].h
+00003430: 255d 9468 275d 9468 295d 9475 682b 6a63  %].h'].h)].uh+jc
+00003440: 0100 0068 1b6a c103 0000 681c 6803 681d  ...h.j....h.h.h.
+00003450: 4e68 1e4e 7562 6568 1f7d 9428 6821 5d94  Nh.Nubeh.}.(h!].
+00003460: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+00003470: 7568 2b6a 5001 0000 681b 6aa7 0300 0068  uh+jP...h.j....h
+00003480: 1c68 0368 1d68 2c68 1e4b 2d75 6265 681f  .h.h.h,h.K-ubeh.
+00003490: 7d94 2868 215d 9468 235d 9428 6a2f 0400  }.(h!].h#].(j/..
+000034a0: 008c 0866 756e 6374 696f 6e94 6568 255d  ...function.eh%]
+000034b0: 9468 275d 9468 295d 946a 7d03 0000 6a2f  .h'].h)].j}...j/
+000034c0: 0400 006a 7e03 0000 6a34 0500 006a 7f03  ...j~...j4...j..
+000034d0: 0000 6a34 0500 006a 8003 0000 896a 8103  ..j4...j.....j..
+000034e0: 0000 896a 8203 0000 8975 682b 6a28 0100  ...j.....uh+j(..
+000034f0: 0068 1c68 0368 1b6a 8b03 0000 681d 4e68  .h.h.h.j....h.Nh
+00003500: 1e4e 7562 6568 1f7d 9428 6821 5d94 8c0f  .Nubeh.}.(h!]...
+00003510: 6e65 7374 6572 2d76 616c 6964 6174 6594  nester-validate.
+00003520: 6168 235d 9468 255d 948c 0f6e 6573 7465  ah#].h%]...neste
+00003530: 7220 7661 6c69 6461 7465 9461 6827 5d94  r validate.ah'].
+00003540: 6829 5d94 7568 2b68 0a68 1b68 4b68 1c68  h)].uh+h.h.hKh.h
+00003550: 0368 1d68 2c68 1e4b 2b75 6268 0b29 8194  .h.h,h.K+ubh.)..
+00003560: 7d94 2868 0568 0668 075d 9428 6810 2981  }.(h.h.h.].(h.).
+00003570: 947d 9428 6805 8c0a 4e65 7374 6572 206c  .}.(h...Nester l
+00003580: 6f67 9468 075d 9468 168c 0a4e 6573 7465  og.h.].h...Neste
+00003590: 7220 6c6f 6794 8594 8194 7d94 2868 1b6a  r log.....}.(h.j
+000035a0: 4305 0000 681c 6803 681d 4e68 1e4e 7562  C...h.h.h.Nh.Nub
+000035b0: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+000035c0: 5d94 6827 5d94 6829 5d94 7568 2b68 0f68  ].h'].h)].uh+h.h
+000035d0: 1b6a 4005 0000 681c 6803 681d 682c 681e  .j@...h.h.h.h,h.
+000035e0: 4b3a 7562 6a1c 0100 0029 8194 7d94 2868  K:ubj....)..}.(h
+000035f0: 0568 0668 075d 9468 1f7d 9428 6821 5d94  .h.h.].h.}.(h!].
+00003600: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+00003610: 8c07 656e 7472 6965 7394 5d94 7568 2b6a  ..entries.].uh+j
+00003620: 1b01 0000 681b 6a40 0500 0068 1c68 0368  ....h.j@...h.h.h
+00003630: 1d4e 681e 4e75 626a 2901 0000 2981 947d  .Nh.Nubj)...)..}
+00003640: 9428 6805 6806 6807 5d94 286a 2e01 0000  .(h.h.h.].(j....
+00003650: 2981 947d 9428 6805 8c0c 6e65 7374 6572  )..}.(h...nester
+00003660: 206c 6f67 2829 9468 075d 946a 3401 0000   log().h.].j4...
+00003670: 2981 947d 9428 6805 6a61 0500 0068 075d  )..}.(h.ja...h.]
+00003680: 9468 168c 0c6e 6573 7465 7220 6c6f 6728  .h...nester log(
+00003690: 2994 8594 8194 7d94 2868 1b6a 6305 0000  ).....}.(h.jc...
+000036a0: 681c 6803 681d 4e68 1e4e 7562 6168 1f7d  h.h.h.Nh.Nubah.}
+000036b0: 9428 6821 5d94 6823 5d94 286a 3f01 0000  .(h!].h#].(j?...
+000036c0: 6a40 0100 0065 6825 5d94 6827 5d94 6829  j@...eh%].h'].h)
+000036d0: 5d94 6a44 0100 006a 4501 0000 7568 2b6a  ].jD...jE...uh+j
+000036e0: 3301 0000 681b 6a5f 0500 0068 1c68 0368  3...h.j_...h.h.h
+000036f0: 1d68 2c68 1e4b 3c75 6261 681f 7d94 2868  .h,h.K<ubah.}.(h
+00003700: 215d 9468 235d 9428 6a49 0100 006a 4a01  !].h#].(jI...jJ.
+00003710: 0000 6568 255d 9468 275d 9468 295d 946a  ..eh%].h'].h)].j
+00003720: 4e01 0000 296a 4f01 0000 6806 7568 2b6a  N...)jO...h.uh+j
+00003730: 2d01 0000 681d 682c 681e 4b3c 681b 6a5c  -...h.h,h.K<h.j\
+00003740: 0500 0068 1c68 0375 626a 5101 0000 2981  ...h.h.ubjQ...).
+00003750: 947d 9428 6805 6806 6807 5d94 2868 2e29  .}.(h.h.h.].(h.)
+00003760: 8194 7d94 2868 058c 4d4c 6973 7473 2061  ..}.(h..MLists a
+00003770: 6c6c 2070 7265 7669 6f75 736c 7920 6372  ll previously cr
+00003780: 6561 7465 6420 7072 6f6a 6563 7473 2c20  eated projects, 
+00003790: 7768 6963 6820 6861 6420 6c6f 6767 696e  which had loggin
+000037a0: 6720 656e 6162 6c65 642c 2069 6e20 6120  g enabled, in a 
+000037b0: 7461 626c 652e 9468 075d 9468 168c 4d4c  table..h.].h..ML
+000037c0: 6973 7473 2061 6c6c 2070 7265 7669 6f75  ists all previou
+000037d0: 736c 7920 6372 6561 7465 6420 7072 6f6a  sly created proj
+000037e0: 6563 7473 2c20 7768 6963 6820 6861 6420  ects, which had 
+000037f0: 6c6f 6767 696e 6720 656e 6162 6c65 642c  logging enabled,
+00003800: 2069 6e20 6120 7461 626c 652e 9485 9481   in a table.....
+00003810: 947d 9428 681b 6a79 0500 0068 1c68 0368  .}.(h.jy...h.h.h
+00003820: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
+00003830: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+00003840: 9475 682b 682d 681d 682c 681e 4b3e 681b  .uh+h-h.h,h.K>h.
+00003850: 6a76 0500 0068 1c68 0375 626a 6401 0000  jv...h.h.ubjd...
+00003860: 2981 947d 9428 6805 6806 6807 5d94 286a  )..}.(h.h.h.].(j
+00003870: 6901 0000 2981 947d 9428 6805 6806 6807  i...)..}.(h.h.h.
+00003880: 5d94 286a 6e01 0000 2981 947d 9428 6805  ].(jn...)..}.(h.
+00003890: 8c0a 5061 7261 6d65 7465 7273 9468 075d  ..Parameters.h.]
+000038a0: 9468 168c 0a50 6172 616d 6574 6572 7394  .h...Parameters.
+000038b0: 8594 8194 7d94 2868 1b6a 8d05 0000 681c  ....}.(h.j....h.
+000038c0: 6803 681d 4e68 1e4e 7562 6168 1f7d 9428  h.h.Nh.Nubah.}.(
+000038d0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+000038e0: 6829 5d94 7568 2b6a 6d01 0000 681b 6a8a  h)].uh+jm...h.j.
+000038f0: 0500 0068 1d68 2c68 1e4b 0075 626a 7e01  ...h.h,h.K.ubj~.
+00003900: 0000 2981 947d 9428 6805 6806 6807 5d94  ..)..}.(h.h.h.].
+00003910: 682e 2981 947d 9428 6805 8c44 2d2d 636c  h.)..}.(h..D--cl
+00003920: 6561 6e20 2866 6c61 6729 202d 2d20 416e  ean (flag) -- An
+00003930: 206f 7074 696f 6e61 6c20 666c 6167 2074   optional flag t
+00003940: 6f20 636c 6561 6e20 7570 206f 7270 6861  o clean up orpha
+00003950: 6e65 6420 6c6f 6720 656e 7472 6965 732e  ned log entries.
+00003960: 9468 075d 9428 6a8d 0100 0029 8194 7d94  .h.].(j....)..}.
+00003970: 2868 058c 072d 2d63 6c65 616e 9468 075d  (h...--clean.h.]
+00003980: 9468 168c 072d 2d63 6c65 616e 9485 9481  .h...--clean....
+00003990: 947d 9428 681b 6aa2 0500 0068 1c68 0368  .}.(h.j....h.h.h
+000039a0: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
+000039b0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+000039c0: 9475 682b 6a8c 0100 0068 1b6a 9e05 0000  .uh+j....h.j....
+000039d0: 7562 6816 8c02 2028 9485 9481 947d 9428  ubh... (.....}.(
+000039e0: 681b 6a9e 0500 0068 1c68 0368 1d4e 681e  h.j....h.h.h.Nh.
+000039f0: 4e75 626a a101 0000 2981 947d 9428 6805  Nubj....)..}.(h.
+00003a00: 6806 6807 5d94 6aa6 0100 0029 8194 7d94  h.h.].j....)..}.
+00003a10: 2868 058c 0466 6c61 6794 6807 5d94 6816  (h...flag.h.].h.
+00003a20: 8c04 666c 6167 9485 9481 947d 9428 681b  ..flag.....}.(h.
+00003a30: 6ab7 0500 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
+00003a40: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
+00003a50: 255d 9468 275d 9468 295d 9475 682b 6aa5  %].h'].h)].uh+j.
+00003a60: 0100 0068 1b6a b405 0000 7562 6168 1f7d  ...h.j....ubah.}
+00003a70: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
+00003a80: 5d94 6829 5d94 8c09 7265 6664 6f6d 6169  ].h)]...refdomai
+00003a90: 6e94 8c02 7079 948c 0b72 6566 6578 706c  n...py...refexpl
+00003aa0: 6963 6974 9489 8c07 7265 6674 7970 6594  icit....reftype.
+00003ab0: 6abf 0100 008c 0972 6566 7461 7267 6574  j......reftarget
+00003ac0: 946a b905 0000 6ac1 0100 0088 6ac2 0100  .j....j.....j...
+00003ad0: 004e 6ac3 0100 004e 7568 2b6a a001 0000  .Nj....Nuh+j....
+00003ae0: 681b 6a9e 0500 0075 6268 168c 0129 9485  h.j....ubh...)..
+00003af0: 9481 947d 9428 681b 6a9e 0500 0068 1c68  ...}.(h.j....h.h
+00003b00: 0368 1d4e 681e 4e75 6268 168c 0520 e280  .h.Nh.Nubh... ..
+00003b10: 9320 9485 9481 947d 9428 681b 6a9e 0500  . .....}.(h.j...
+00003b20: 0068 1c68 0368 1d4e 681e 4e75 6268 168c  .h.h.h.Nh.Nubh..
+00003b30: 3241 6e20 6f70 7469 6f6e 616c 2066 6c61  2An optional fla
+00003b40: 6720 746f 2063 6c65 616e 2075 7020 6f72  g to clean up or
+00003b50: 7068 616e 6564 206c 6f67 2065 6e74 7269  phaned log entri
+00003b60: 6573 2e94 8594 8194 7d94 2868 1b6a 9e05  es......}.(h.j..
+00003b70: 0000 681c 6803 681d 4e68 1e4e 7562 6568  ..h.h.h.Nh.Nubeh
+00003b80: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+00003b90: 6827 5d94 6829 5d94 7568 2b68 2d68 1b6a  h'].h)].uh+h-h.j
+00003ba0: 9b05 0000 7562 6168 1f7d 9428 6821 5d94  ....ubah.}.(h!].
+00003bb0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+00003bc0: 7568 2b6a 7d01 0000 681b 6a8a 0500 0075  uh+j}...h.j....u
+00003bd0: 6265 681f 7d94 2868 215d 9468 235d 9468  beh.}.(h!].h#].h
+00003be0: 255d 9468 275d 9468 295d 9475 682b 6a68  %].h'].h)].uh+jh
+00003bf0: 0100 0068 1b6a 8705 0000 7562 6a69 0100  ...h.j....ubji..
+00003c00: 0029 8194 7d94 2868 0568 0668 075d 9428  .)..}.(h.h.h.].(
+00003c10: 6a6e 0100 0029 8194 7d94 2868 058c 0752  jn...)..}.(h...R
+00003c20: 6574 7572 6e73 9468 075d 9468 168c 0752  eturns.h.].h...R
+00003c30: 6574 7572 6e73 9485 9481 947d 9428 681b  eturns.....}.(h.
+00003c40: 6af1 0500 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
+00003c50: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
+00003c60: 255d 9468 275d 9468 295d 9475 682b 6a6d  %].h'].h)].uh+jm
+00003c70: 0100 0068 1b6a ee05 0000 681d 682c 681e  ...h.j....h.h,h.
+00003c80: 4b00 7562 6a7e 0100 0029 8194 7d94 2868  K.ubj~...)..}.(h
+00003c90: 0568 0668 075d 9468 2e29 8194 7d94 2868  .h.h.].h.)..}.(h
+00003ca0: 058c 044e 6f6e 6594 6807 5d94 6816 8c04  ...None.h.].h...
+00003cb0: 4e6f 6e65 9485 9481 947d 9428 681b 6a02  None.....}.(h.j.
+00003cc0: 0600 0068 1c68 0368 1d4e 681e 4e75 6261  ...h.h.h.Nh.Nuba
+00003cd0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+00003ce0: 9468 275d 9468 295d 9475 682b 682d 681b  .h'].h)].uh+h-h.
+00003cf0: 6aff 0500 0075 6261 681f 7d94 2868 215d  j....ubah.}.(h!]
+00003d00: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+00003d10: 9475 682b 6a7d 0100 0068 1b6a ee05 0000  .uh+j}...h.j....
+00003d20: 7562 6568 1f7d 9428 6821 5d94 6823 5d94  ubeh.}.(h!].h#].
+00003d30: 6825 5d94 6827 5d94 6829 5d94 7568 2b6a  h%].h'].h)].uh+j
+00003d40: 6801 0000 681b 6a87 0500 0075 626a 6901  h...h.j....ubji.
+00003d50: 0000 2981 947d 9428 6805 6806 6807 5d94  ..)..}.(h.h.h.].
+00003d60: 286a 6e01 0000 2981 947d 9428 6805 8c0b  (jn...)..}.(h...
+00003d70: 5265 7475 726e 2074 7970 6594 6807 5d94  Return type.h.].
+00003d80: 6816 8c0b 5265 7475 726e 2074 7970 6594  h...Return type.
+00003d90: 8594 8194 7d94 2868 1b6a 1f06 0000 681c  ....}.(h.j....h.
+00003da0: 6803 681d 4e68 1e4e 7562 6168 1f7d 9428  h.h.Nh.Nubah.}.(
+00003db0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+00003dc0: 6829 5d94 7568 2b6a 6d01 0000 681b 6a1c  h)].uh+jm...h.j.
+00003dd0: 0600 0068 1d68 2c68 1e4b 0075 626a 7e01  ...h.h,h.K.ubj~.
+00003de0: 0000 2981 947d 9428 6805 6806 6807 5d94  ..)..}.(h.h.h.].
+00003df0: 682e 2981 947d 9428 6805 8c04 4e6f 6e65  h.)..}.(h...None
+00003e00: 9468 075d 946a a101 0000 2981 947d 9428  .h.].j....)..}.(
+00003e10: 6805 6806 6807 5d94 6816 8c04 4e6f 6e65  h.h.h.].h...None
+00003e20: 9485 9481 947d 9428 681b 6a34 0600 0068  .....}.(h.j4...h
+00003e30: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
+00003e40: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+00003e50: 9468 295d 948c 0972 6566 646f 6d61 696e  .h)]...refdomain
+00003e60: 946a cc05 0000 8c0b 7265 6665 7870 6c69  .j......refexpli
+00003e70: 6369 7494 898c 0772 6566 7479 7065 946a  cit....reftype.j
+00003e80: bf01 0000 8c09 7265 6674 6172 6765 7494  ......reftarget.
+00003e90: 8c04 4e6f 6e65 946a c101 0000 886a c201  ..None.j.....j..
+00003ea0: 0000 4e6a c301 0000 4e75 682b 6aa0 0100  ..Nj....Nuh+j...
+00003eb0: 0068 1b6a 3006 0000 7562 6168 1f7d 9428  .h.j0...ubah.}.(
+00003ec0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+00003ed0: 6829 5d94 7568 2b68 2d68 1b6a 2d06 0000  h)].uh+h-h.j-...
+00003ee0: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+00003ef0: 6825 5d94 6827 5d94 6829 5d94 7568 2b6a  h%].h'].h)].uh+j
+00003f00: 7d01 0000 681b 6a1c 0600 0075 6265 681f  }...h.j....ubeh.
+00003f10: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+00003f20: 275d 9468 295d 9475 682b 6a68 0100 0068  '].h)].uh+jh...h
+00003f30: 1b6a 8705 0000 7562 6568 1f7d 9428 6821  .j....ubeh.}.(h!
+00003f40: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+00003f50: 5d94 7568 2b6a 6301 0000 681b 6a76 0500  ].uh+jc...h.jv..
+00003f60: 0068 1c68 0368 1d4e 681e 4e75 6265 681f  .h.h.h.Nh.Nubeh.
+00003f70: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+00003f80: 275d 9468 295d 9475 682b 6a50 0100 0068  '].h)].uh+jP...h
+00003f90: 1b6a 5c05 0000 681c 6803 681d 682c 681e  .j\...h.h.h.h,h.
+00003fa0: 4b3c 7562 6568 1f7d 9428 6821 5d94 6823  K<ubeh.}.(h!].h#
+00003fb0: 5d94 286a cc05 0000 8c08 6675 6e63 7469  ].(j......functi
+00003fc0: 6f6e 9465 6825 5d94 6827 5d94 6829 5d94  on.eh%].h'].h)].
+00003fd0: 6a7d 0300 006a cc05 0000 6a7e 0300 006a  j}...j....j~...j
+00003fe0: 6706 0000 6a7f 0300 006a 6706 0000 6a80  g...j....jg...j.
+00003ff0: 0300 0089 6a81 0300 0089 6a82 0300 0089  ....j.....j.....
+00004000: 7568 2b6a 2801 0000 681c 6803 681b 6a40  uh+j(...h.h.h.j@
+00004010: 0500 0068 1d4e 681e 4e75 6265 681f 7d94  ...h.Nh.Nubeh.}.
+00004020: 2868 215d 948c 0a6e 6573 7465 722d 6c6f  (h!]...nester-lo
+00004030: 6794 6168 235d 9468 255d 948c 0a6e 6573  g.ah#].h%]...nes
+00004040: 7465 7220 6c6f 6794 6168 275d 9468 295d  ter log.ah'].h)]
+00004050: 9475 682b 680a 681b 684b 681c 6803 681d  .uh+h.h.hKh.h.h.
+00004060: 682c 681e 4b3a 7562 680b 2981 947d 9428  h,h.K:ubh.)..}.(
+00004070: 6805 6806 6807 5d94 2868 1029 8194 7d94  h.h.h.].(h.)..}.
+00004080: 2868 058c 0c4e 6573 7465 7220 636c 6561  (h...Nester clea
+00004090: 6e94 6807 5d94 6816 8c0c 4e65 7374 6572  n.h.].h...Nester
+000040a0: 2063 6c65 616e 9485 9481 947d 9428 681b   clean.....}.(h.
+000040b0: 6a76 0600 0068 1c68 0368 1d4e 681e 4e75  jv...h.h.h.Nh.Nu
+000040c0: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
+000040d0: 255d 9468 275d 9468 295d 9475 682b 680f  %].h'].h)].uh+h.
+000040e0: 681b 6a73 0600 0068 1c68 0368 1d68 2c68  h.js...h.h.h.h,h
+000040f0: 1e4b 4675 626a 1c01 0000 2981 947d 9428  .KFubj....)..}.(
+00004100: 6805 6806 6807 5d94 681f 7d94 2868 215d  h.h.h.].h.}.(h!]
+00004110: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+00004120: 948c 0765 6e74 7269 6573 945d 9475 682b  ...entries.].uh+
+00004130: 6a1b 0100 0068 1b6a 7306 0000 681c 6803  j....h.js...h.h.
+00004140: 681d 4e68 1e4e 7562 6a29 0100 0029 8194  h.Nh.Nubj)...)..
+00004150: 7d94 2868 0568 0668 075d 9428 6a2e 0100  }.(h.h.h.].(j...
+00004160: 0029 8194 7d94 2868 058c 256e 6573 7465  .)..}.(h..%neste
+00004170: 7220 636c 6561 6e28 7072 6f6a 6563 746e  r clean(projectn
+00004180: 616d 652c 205b 2d79 7c2d 2d79 6573 5d29  ame, [-y|--yes])
+00004190: 9468 075d 946a 3401 0000 2981 947d 9428  .h.].j4...)..}.(
+000041a0: 6805 6a94 0600 0068 075d 9468 168c 256e  h.j....h.].h..%n
+000041b0: 6573 7465 7220 636c 6561 6e28 7072 6f6a  ester clean(proj
+000041c0: 6563 746e 616d 652c 205b 2d79 7c2d 2d79  ectname, [-y|--y
+000041d0: 6573 5d29 9485 9481 947d 9428 681b 6a96  es]).....}.(h.j.
+000041e0: 0600 0068 1c68 0368 1d4e 681e 4e75 6261  ...h.h.h.Nh.Nuba
+000041f0: 681f 7d94 2868 215d 9468 235d 9428 6a3f  h.}.(h!].h#].(j?
+00004200: 0100 006a 4001 0000 6568 255d 9468 275d  ...j@...eh%].h']
+00004210: 9468 295d 946a 4401 0000 6a45 0100 0075  .h)].jD...jE...u
+00004220: 682b 6a33 0100 0068 1b6a 9206 0000 681c  h+j3...h.j....h.
+00004230: 6803 681d 682c 681e 4b48 7562 6168 1f7d  h.h.h,h.KHubah.}
+00004240: 9428 6821 5d94 6823 5d94 286a 4901 0000  .(h!].h#].(jI...
+00004250: 6a4a 0100 0065 6825 5d94 6827 5d94 6829  jJ...eh%].h'].h)
+00004260: 5d94 6a4e 0100 0029 6a4f 0100 0068 0675  ].jN...)jO...h.u
+00004270: 682b 6a2d 0100 0068 1d68 2c68 1e4b 4868  h+j-...h.h,h.KHh
+00004280: 1b6a 8f06 0000 681c 6803 7562 6a51 0100  .j....h.h.ubjQ..
+00004290: 0029 8194 7d94 2868 0568 0668 075d 9428  .)..}.(h.h.h.].(
+000042a0: 682e 2981 947d 9428 6805 8c3c 4465 6c65  h.)..}.(h..<Dele
+000042b0: 7465 7320 7468 6520 2a65 6e74 6972 652a  tes the *entire*
+000042c0: 2063 6f6e 7465 6e74 206f 6620 7468 6520   content of the 
+000042d0: 6769 7665 6e20 7072 6f6a 6563 7420 6469  given project di
+000042e0: 7265 6374 6f72 792e 9468 075d 9428 6816  rectory..h.].(h.
+000042f0: 8c0c 4465 6c65 7465 7320 7468 6520 9485  ..Deletes the ..
+00004300: 9481 947d 9428 681b 6aac 0600 0068 1c68  ...}.(h.j....h.h
+00004310: 0368 1d4e 681e 4e75 6268 098c 0865 6d70  .h.Nh.Nubh...emp
+00004320: 6861 7369 7394 9394 2981 947d 9428 6805  hasis...)..}.(h.
+00004330: 8c08 2a65 6e74 6972 652a 9468 075d 9468  ..*entire*.h.].h
+00004340: 168c 0665 6e74 6972 6594 8594 8194 7d94  ...entire.....}.
+00004350: 2868 1b6a b606 0000 681c 6803 681d 4e68  (h.j....h.h.h.Nh
+00004360: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
+00004370: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
+00004380: 2b6a b406 0000 681b 6aac 0600 0075 6268  +j....h.j....ubh
+00004390: 168c 2820 636f 6e74 656e 7420 6f66 2074  ..( content of t
+000043a0: 6865 2067 6976 656e 2070 726f 6a65 6374  he given project
+000043b0: 2064 6972 6563 746f 7279 2e94 8594 8194   directory......
+000043c0: 7d94 2868 1b6a ac06 0000 681c 6803 681d  }.(h.j....h.h.h.
+000043d0: 4e68 1e4e 7562 6568 1f7d 9428 6821 5d94  Nh.Nubeh.}.(h!].
+000043e0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+000043f0: 7568 2b68 2d68 1d68 2c68 1e4b 4a68 1b6a  uh+h-h.h,h.KJh.j
+00004400: a906 0000 681c 6803 7562 682e 2981 947d  ....h.h.ubh.)..}
+00004410: 9428 6805 8c21 5468 6973 2061 6374 696f  .(h..!This actio
+00004420: 6e20 2a2a 6361 6e6e 6f74 2a2a 2062 6520  n **cannot** be 
+00004430: 756e 646f 6e65 2e94 6807 5d94 2868 168c  undone..h.].(h..
+00004440: 0c54 6869 7320 6163 7469 6f6e 2094 8594  .This action ...
+00004450: 8194 7d94 2868 1b6a ce06 0000 681c 6803  ..}.(h.j....h.h.
+00004460: 681d 4e68 1e4e 7562 6809 8c06 7374 726f  h.Nh.Nubh...stro
+00004470: 6e67 9493 9429 8194 7d94 2868 058c 0a2a  ng...)..}.(h...*
+00004480: 2a63 616e 6e6f 742a 2a94 6807 5d94 6816  *cannot**.h.].h.
+00004490: 8c06 6361 6e6e 6f74 9485 9481 947d 9428  ..cannot.....}.(
+000044a0: 681b 6ad8 0600 0068 1c68 0368 1d4e 681e  h.j....h.h.h.Nh.
+000044b0: 4e75 6261 681f 7d94 2868 215d 9468 235d  Nubah.}.(h!].h#]
+000044c0: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
+000044d0: 6ad6 0600 0068 1b6a ce06 0000 7562 6816  j....h.j....ubh.
+000044e0: 8c0b 2062 6520 756e 646f 6e65 2e94 8594  .. be undone....
+000044f0: 8194 7d94 2868 1b6a ce06 0000 681c 6803  ..}.(h.j....h.h.
+00004500: 681d 4e68 1e4e 7562 6568 1f7d 9428 6821  h.Nh.Nubeh.}.(h!
+00004510: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+00004520: 5d94 7568 2b68 2d68 1d68 2c68 1e4b 4c68  ].uh+h-h.h,h.KLh
+00004530: 1b6a a906 0000 681c 6803 7562 6a64 0100  .j....h.h.ubjd..
+00004540: 0029 8194 7d94 2868 0568 0668 075d 9428  .)..}.(h.h.h.].(
+00004550: 6a69 0100 0029 8194 7d94 2868 0568 0668  ji...)..}.(h.h.h
+00004560: 075d 9428 6a6e 0100 0029 8194 7d94 2868  .].(jn...)..}.(h
+00004570: 058c 0a50 6172 616d 6574 6572 7394 6807  ...Parameters.h.
+00004580: 5d94 6816 8c0a 5061 7261 6d65 7465 7273  ].h...Parameters
+00004590: 9485 9481 947d 9428 681b 6af6 0600 0068  .....}.(h.j....h
+000045a0: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
+000045b0: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+000045c0: 9468 295d 9475 682b 6a6d 0100 0068 1b6a  .h)].uh+jm...h.j
+000045d0: f306 0000 681d 682c 681e 4b00 7562 6a7e  ....h.h,h.K.ubj~
+000045e0: 0100 0029 8194 7d94 2868 0568 0668 075d  ...)..}.(h.h.h.]
+000045f0: 9468 6b29 8194 7d94 2868 0568 0668 075d  .hk)..}.(h.h.h.]
+00004600: 9428 6870 2981 947d 9428 6805 6806 6807  .(hp)..}.(h.h.h.
+00004610: 5d94 682e 2981 947d 9428 6805 8c40 7072  ].h.)..}.(h..@pr
+00004620: 6f6a 6563 746e 616d 6520 2873 7472 2920  ojectname (str) 
+00004630: 2d2d 2054 6865 206e 616d 6520 6f66 2074  -- The name of t
+00004640: 6865 2070 726f 6a65 6374 2079 6f75 2077  he project you w
+00004650: 616e 7420 746f 2064 656c 6574 652e 9468  ant to delete..h
+00004660: 075d 9428 6a8d 0100 0029 8194 7d94 2868  .].(j....)..}.(h
+00004670: 058c 0b70 726f 6a65 6374 6e61 6d65 9468  ...projectname.h
+00004680: 075d 9468 168c 0b70 726f 6a65 6374 6e61  .].h...projectna
+00004690: 6d65 9485 9481 947d 9428 681b 6a11 0700  me.....}.(h.j...
+000046a0: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
+000046b0: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+000046c0: 275d 9468 295d 9475 682b 6a8c 0100 0068  '].h)].uh+j....h
+000046d0: 1b6a 0d07 0000 7562 6816 8c02 2028 9485  .j....ubh... (..
+000046e0: 9481 947d 9428 681b 6a0d 0700 0068 1c68  ...}.(h.j....h.h
+000046f0: 0368 1d4e 681e 4e75 626a a101 0000 2981  .h.Nh.Nubj....).
+00004700: 947d 9428 6805 6806 6807 5d94 6aa6 0100  .}.(h.h.h.].j...
+00004710: 0029 8194 7d94 2868 058c 0373 7472 9468  .)..}.(h...str.h
+00004720: 075d 9468 168c 0373 7472 9485 9481 947d  .].h...str.....}
+00004730: 9428 681b 6a26 0700 0068 1c68 0368 1d4e  .(h.j&...h.h.h.N
+00004740: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
+00004750: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
+00004760: 682b 6aa5 0100 0068 1b6a 2307 0000 7562  h+j....h.j#...ub
+00004770: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+00004780: 5d94 6827 5d94 6829 5d94 8c09 7265 6664  ].h'].h)]...refd
+00004790: 6f6d 6169 6e94 8c02 7079 948c 0b72 6566  omain...py...ref
+000047a0: 6578 706c 6963 6974 9489 8c07 7265 6674  explicit....reft
+000047b0: 7970 6594 6abf 0100 008c 0972 6566 7461  ype.j......refta
+000047c0: 7267 6574 946a 2807 0000 6ac1 0100 0088  rget.j(...j.....
+000047d0: 6ac2 0100 004e 6ac3 0100 004e 7568 2b6a  j....Nj....Nuh+j
+000047e0: a001 0000 681b 6a0d 0700 0075 6268 168c  ....h.j....ubh..
+000047f0: 0129 9485 9481 947d 9428 681b 6a0d 0700  .).....}.(h.j...
+00004800: 0068 1c68 0368 1d4e 681e 4e75 6268 168c  .h.h.h.Nh.Nubh..
+00004810: 0520 e280 9320 9485 9481 947d 9428 681b  . ... .....}.(h.
+00004820: 6a0d 0700 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
+00004830: 6268 168c 2b54 6865 206e 616d 6520 6f66  bh..+The name of
+00004840: 2074 6865 2070 726f 6a65 6374 2079 6f75   the project you
+00004850: 2077 616e 7420 746f 2064 656c 6574 652e   want to delete.
+00004860: 9485 9481 947d 9428 681b 6a0d 0700 0068  .....}.(h.j....h
+00004870: 1c68 0368 1d4e 681e 4e75 6265 681f 7d94  .h.h.Nh.Nubeh.}.
+00004880: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+00004890: 9468 295d 9475 682b 682d 681b 6a0a 0700  .h)].uh+h-h.j...
+000048a0: 0075 6261 681f 7d94 2868 215d 9468 235d  .ubah.}.(h!].h#]
+000048b0: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
+000048c0: 686f 681b 6a07 0700 0075 6268 7029 8194  hoh.j....ubhp)..
+000048d0: 7d94 2868 0568 0668 075d 9468 2e29 8194  }.(h.h.h.].h.)..
+000048e0: 7d94 2868 058c 682d 797c 2d2d 7965 7320  }.(h..h-y|--yes 
+000048f0: 2866 6c61 6729 202d 2d20 416e 206f 7074  (flag) -- An opt
+00004900: 696f 6e61 6c20 666c 6167 2074 6f20 6175  ional flag to au
+00004910: 746f 2d63 6f6e 6669 726d 2079 6f75 7220  to-confirm your 
+00004920: 6465 6369 7369 6f6e 2061 6e64 2073 6b69  decision and ski
+00004930: 7020 7468 6520 2241 7265 2079 6f75 2073  p the "Are you s
+00004940: 7572 653f 2220 6469 616c 6f67 7565 2e94  ure?" dialogue..
+00004950: 6807 5d94 286a 8d01 0000 2981 947d 9428  h.].(j....)..}.(
+00004960: 6805 8c02 2d79 9468 075d 9468 168c 022d  h...-y.h.].h...-
+00004970: 7994 8594 8194 7d94 2868 1b6a 5e07 0000  y.....}.(h.j^...
+00004980: 681c 6803 681d 4e68 1e4e 7562 6168 1f7d  h.h.h.Nh.Nubah.}
+00004990: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
+000049a0: 5d94 6829 5d94 7568 2b6a 8c01 0000 681b  ].h)].uh+j....h.
+000049b0: 6a5a 0700 0075 626a 8d01 0000 2981 947d  jZ...ubj....)..}
+000049c0: 9428 6805 6a51 0200 0068 075d 9468 168c  .(h.jQ...h.].h..
+000049d0: 017c 9485 9481 947d 9428 681b 6a6c 0700  .|.....}.(h.jl..
+000049e0: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
+000049f0: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+00004a00: 275d 9468 295d 9475 682b 6a8c 0100 0068  '].h)].uh+j....h
+00004a10: 1b6a 5a07 0000 7562 6a8d 0100 0029 8194  .jZ...ubj....)..
+00004a20: 7d94 2868 058c 052d 2d79 6573 9468 075d  }.(h...--yes.h.]
+00004a30: 9468 168c 052d 2d79 6573 9485 9481 947d  .h...--yes.....}
+00004a40: 9428 681b 6a79 0700 0068 1c68 0368 1d4e  .(h.jy...h.h.h.N
+00004a50: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
+00004a60: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
+00004a70: 682b 6a8c 0100 0068 1b6a 5a07 0000 7562  h+j....h.jZ...ub
+00004a80: 6816 8c02 2028 9485 9481 947d 9428 681b  h... (.....}.(h.
+00004a90: 6a5a 0700 0068 1c68 0368 1d4e 681e 4e75  jZ...h.h.h.Nh.Nu
+00004aa0: 626a a101 0000 2981 947d 9428 6805 6806  bj....)..}.(h.h.
+00004ab0: 6807 5d94 6aa6 0100 0029 8194 7d94 2868  h.].j....)..}.(h
+00004ac0: 058c 0466 6c61 6794 6807 5d94 6816 8c04  ...flag.h.].h...
+00004ad0: 666c 6167 9485 9481 947d 9428 681b 6a8e  flag.....}.(h.j.
+00004ae0: 0700 0068 1c68 0368 1d4e 681e 4e75 6261  ...h.h.h.Nh.Nuba
+00004af0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+00004b00: 9468 275d 9468 295d 9475 682b 6aa5 0100  .h'].h)].uh+j...
+00004b10: 0068 1b6a 8b07 0000 7562 6168 1f7d 9428  .h.j....ubah.}.(
+00004b20: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+00004b30: 6829 5d94 8c09 7265 6664 6f6d 6169 6e94  h)]...refdomain.
+00004b40: 6a3b 0700 008c 0b72 6566 6578 706c 6963  j;.....refexplic
+00004b50: 6974 9489 8c07 7265 6674 7970 6594 6abf  it....reftype.j.
+00004b60: 0100 008c 0972 6566 7461 7267 6574 946a  .....reftarget.j
+00004b70: 9007 0000 6ac1 0100 0088 6ac2 0100 004e  ....j.....j....N
+00004b80: 6ac3 0100 004e 7568 2b6a a001 0000 681b  j....Nuh+j....h.
+00004b90: 6a5a 0700 0075 6268 168c 0129 9485 9481  jZ...ubh...)....
+00004ba0: 947d 9428 681b 6a5a 0700 0068 1c68 0368  .}.(h.jZ...h.h.h
+00004bb0: 1d4e 681e 4e75 6268 168c 0520 e280 9320  .Nh.Nubh... ... 
+00004bc0: 9485 9481 947d 9428 681b 6a5a 0700 0068  .....}.(h.jZ...h
+00004bd0: 1c68 0368 1d4e 681e 4e75 6268 168c 5941  .h.h.Nh.Nubh..YA
+00004be0: 6e20 6f70 7469 6f6e 616c 2066 6c61 6720  n optional flag 
+00004bf0: 746f 2061 7574 6f2d 636f 6e66 6972 6d20  to auto-confirm 
+00004c00: 796f 7572 2064 6563 6973 696f 6e20 616e  your decision an
+00004c10: 6420 736b 6970 2074 6865 20e2 809c 4172  d skip the ...Ar
+00004c20: 6520 796f 7520 7375 7265 3fe2 809d 2064  e you sure?... d
+00004c30: 6961 6c6f 6775 652e 9485 9481 947d 9428  ialogue......}.(
+00004c40: 681b 6a5a 0700 0068 1c68 0368 1d4e 681e  h.jZ...h.h.h.Nh.
+00004c50: 4e75 6265 681f 7d94 2868 215d 9468 235d  Nubeh.}.(h!].h#]
+00004c60: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
+00004c70: 682d 681b 6a57 0700 0075 6261 681f 7d94  h-h.jW...ubah.}.
+00004c80: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+00004c90: 9468 295d 9475 682b 686f 681b 6a07 0700  .h)].uh+hoh.j...
+00004ca0: 0075 6265 681f 7d94 2868 215d 9468 235d  .ubeh.}.(h!].h#]
+00004cb0: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
+00004cc0: 686a 681b 6a04 0700 0075 6261 681f 7d94  hjh.j....ubah.}.
+00004cd0: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+00004ce0: 9468 295d 9475 682b 6a7d 0100 0068 1b6a  .h)].uh+j}...h.j
+00004cf0: f306 0000 7562 6568 1f7d 9428 6821 5d94  ....ubeh.}.(h!].
+00004d00: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+00004d10: 7568 2b6a 6801 0000 681b 6af0 0600 0075  uh+jh...h.j....u
+00004d20: 626a 6901 0000 2981 947d 9428 6805 6806  bji...)..}.(h.h.
+00004d30: 6807 5d94 286a 6e01 0000 2981 947d 9428  h.].(jn...)..}.(
+00004d40: 6805 8c07 5265 7475 726e 7394 6807 5d94  h...Returns.h.].
+00004d50: 6816 8c07 5265 7475 726e 7394 8594 8194  h...Returns.....
+00004d60: 7d94 2868 1b6a d307 0000 681c 6803 681d  }.(h.j....h.h.h.
+00004d70: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
+00004d80: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+00004d90: 7568 2b6a 6d01 0000 681b 6ad0 0700 0068  uh+jm...h.j....h
+00004da0: 1d68 2c68 1e4b 0075 626a 7e01 0000 2981  .h,h.K.ubj~...).
+00004db0: 947d 9428 6805 6806 6807 5d94 682e 2981  .}.(h.h.h.].h.).
+00004dc0: 947d 9428 6805 8c04 4e6f 6e65 9468 075d  .}.(h...None.h.]
+00004dd0: 9468 168c 044e 6f6e 6594 8594 8194 7d94  .h...None.....}.
+00004de0: 2868 1b6a e407 0000 681c 6803 681d 4e68  (h.j....h.h.h.Nh
+00004df0: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
+00004e00: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
+00004e10: 2b68 2d68 1b6a e107 0000 7562 6168 1f7d  +h-h.j....ubah.}
+00004e20: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
+00004e30: 5d94 6829 5d94 7568 2b6a 7d01 0000 681b  ].h)].uh+j}...h.
+00004e40: 6ad0 0700 0075 6265 681f 7d94 2868 215d  j....ubeh.}.(h!]
+00004e50: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+00004e60: 9475 682b 6a68 0100 0068 1b6a f006 0000  .uh+jh...h.j....
+00004e70: 7562 6a69 0100 0029 8194 7d94 2868 0568  ubji...)..}.(h.h
+00004e80: 0668 075d 9428 6a6e 0100 0029 8194 7d94  .h.].(jn...)..}.
+00004e90: 2868 058c 0b52 6574 7572 6e20 7479 7065  (h...Return type
+00004ea0: 9468 075d 9468 168c 0b52 6574 7572 6e20  .h.].h...Return 
+00004eb0: 7479 7065 9485 9481 947d 9428 681b 6a01  type.....}.(h.j.
+00004ec0: 0800 0068 1c68 0368 1d4e 681e 4e75 6261  ...h.h.h.Nh.Nuba
+00004ed0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+00004ee0: 9468 275d 9468 295d 9475 682b 6a6d 0100  .h'].h)].uh+jm..
+00004ef0: 0068 1b6a fe07 0000 681d 682c 681e 4b00  .h.j....h.h,h.K.
+00004f00: 7562 6a7e 0100 0029 8194 7d94 2868 0568  ubj~...)..}.(h.h
+00004f10: 0668 075d 9468 2e29 8194 7d94 2868 058c  .h.].h.)..}.(h..
+00004f20: 044e 6f6e 6594 6807 5d94 6aa1 0100 0029  .None.h.].j....)
+00004f30: 8194 7d94 2868 0568 0668 075d 9468 168c  ..}.(h.h.h.].h..
+00004f40: 044e 6f6e 6594 8594 8194 7d94 2868 1b6a  .None.....}.(h.j
+00004f50: 1608 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
+00004f60: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+00004f70: 5d94 6827 5d94 6829 5d94 8c09 7265 6664  ].h'].h)]...refd
+00004f80: 6f6d 6169 6e94 6a3b 0700 008c 0b72 6566  omain.j;.....ref
+00004f90: 6578 706c 6963 6974 9489 8c07 7265 6674  explicit....reft
+00004fa0: 7970 6594 6abf 0100 008c 0972 6566 7461  ype.j......refta
+00004fb0: 7267 6574 948c 044e 6f6e 6594 6ac1 0100  rget...None.j...
+00004fc0: 0088 6ac2 0100 004e 6ac3 0100 004e 7568  ..j....Nj....Nuh
+00004fd0: 2b6a a001 0000 681b 6a12 0800 0075 6261  +j....h.j....uba
+00004fe0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+00004ff0: 9468 275d 9468 295d 9475 682b 682d 681b  .h'].h)].uh+h-h.
+00005000: 6a0f 0800 0075 6261 681f 7d94 2868 215d  j....ubah.}.(h!]
+00005010: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+00005020: 9475 682b 6a7d 0100 0068 1b6a fe07 0000  .uh+j}...h.j....
+00005030: 7562 6568 1f7d 9428 6821 5d94 6823 5d94  ubeh.}.(h!].h#].
+00005040: 6825 5d94 6827 5d94 6829 5d94 7568 2b6a  h%].h'].h)].uh+j
+00005050: 6801 0000 681b 6af0 0600 0075 6265 681f  h...h.j....ubeh.
+00005060: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+00005070: 275d 9468 295d 9475 682b 6a63 0100 0068  '].h)].uh+jc...h
+00005080: 1b6a a906 0000 681c 6803 681d 4e68 1e4e  .j....h.h.h.Nh.N
+00005090: 7562 6568 1f7d 9428 6821 5d94 6823 5d94  ubeh.}.(h!].h#].
+000050a0: 6825 5d94 6827 5d94 6829 5d94 7568 2b6a  h%].h'].h)].uh+j
+000050b0: 5001 0000 681b 6a8f 0600 0068 1c68 0368  P...h.j....h.h.h
+000050c0: 1d68 2c68 1e4b 4875 6265 681f 7d94 2868  .h,h.KHubeh.}.(h
+000050d0: 215d 9468 235d 9428 6a3b 0700 008c 0866  !].h#].(j;.....f
+000050e0: 756e 6374 696f 6e94 6568 255d 9468 275d  unction.eh%].h']
+000050f0: 9468 295d 946a 7d03 0000 6a3b 0700 006a  .h)].j}...j;...j
+00005100: 7e03 0000 6a49 0800 006a 7f03 0000 6a49  ~...jI...j....jI
+00005110: 0800 006a 8003 0000 896a 8103 0000 896a  ...j.....j.....j
+00005120: 8203 0000 8975 682b 6a28 0100 0068 1c68  .....uh+j(...h.h
+00005130: 0368 1b6a 7306 0000 681d 4e68 1e4e 7562  .h.js...h.Nh.Nub
+00005140: 6568 1f7d 9428 6821 5d94 8c0c 6e65 7374  eh.}.(h!]...nest
+00005150: 6572 2d63 6c65 616e 9461 6823 5d94 6825  er-clean.ah#].h%
+00005160: 5d94 8c0c 6e65 7374 6572 2063 6c65 616e  ]...nester clean
+00005170: 9461 6827 5d94 6829 5d94 7568 2b68 0a68  .ah'].h)].uh+h.h
+00005180: 1b68 4b68 1c68 0368 1d68 2c68 1e4b 4675  .hKh.h.h.h,h.KFu
+00005190: 6265 681f 7d94 2868 215d 948c 0863 6c69  beh.}.(h!]...cli
+000051a0: 2d6d 6f64 6594 6168 235d 9468 255d 948c  -mode.ah#].h%]..
+000051b0: 0863 6c69 2d6d 6f64 6594 6168 275d 9468  .cli-mode.ah'].h
+000051c0: 295d 9475 682b 680a 681b 680c 681c 6803  )].uh+h.h.h.h.h.
+000051d0: 681d 682c 681e 4b0a 7562 6568 1f7d 9428  h.h,h.K.ubeh.}.(
+000051e0: 6821 5d94 8c05 7573 6167 6594 6168 235d  h!]...usage.ah#]
+000051f0: 9468 255d 948c 0575 7361 6765 9461 6827  .h%]...usage.ah'
+00005200: 5d94 6829 5d94 7568 2b68 0a68 1b68 0368  ].h)].uh+h.h.h.h
+00005210: 1c68 0368 1d68 2c68 1e4b 0275 6261 681f  .h.h.h,h.K.ubah.
+00005220: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+00005230: 275d 9468 295d 948c 0673 6f75 7263 6594  '].h)]...source.
+00005240: 682c 7568 2b68 018c 0e63 7572 7265 6e74  h,uh+h...current
+00005250: 5f73 6f75 7263 6594 4e8c 0c63 7572 7265  _source.N..curre
+00005260: 6e74 5f6c 696e 6594 4e8c 0873 6574 7469  nt_line.N..setti
+00005270: 6e67 7394 8c11 646f 6375 7469 6c73 2e66  ngs...docutils.f
+00005280: 726f 6e74 656e 6494 8c06 5661 6c75 6573  rontend...Values
+00005290: 9493 9429 8194 7d94 2868 0f4e 8c09 6765  ...)..}.(h.N..ge
+000052a0: 6e65 7261 746f 7294 4e8c 0964 6174 6573  nerator.N..dates
+000052b0: 7461 6d70 944e 8c0b 736f 7572 6365 5f6c  tamp.N..source_l
+000052c0: 696e 6b94 4e8c 0a73 6f75 7263 655f 7572  ink.N..source_ur
+000052d0: 6c94 4e8c 0d74 6f63 5f62 6163 6b6c 696e  l.N..toc_backlin
+000052e0: 6b73 948c 0565 6e74 7279 948c 1266 6f6f  ks...entry...foo
+000052f0: 746e 6f74 655f 6261 636b 6c69 6e6b 7394  tnote_backlinks.
+00005300: 4b01 8c0d 7365 6374 6e75 6d5f 7866 6f72  K...sectnum_xfor
+00005310: 6d94 4b01 8c0e 7374 7269 705f 636f 6d6d  m.K...strip_comm
+00005320: 656e 7473 944e 8c1b 7374 7269 705f 656c  ents.N..strip_el
+00005330: 656d 656e 7473 5f77 6974 685f 636c 6173  ements_with_clas
+00005340: 7365 7394 4e8c 0d73 7472 6970 5f63 6c61  ses.N..strip_cla
+00005350: 7373 6573 944e 8c0c 7265 706f 7274 5f6c  sses.N..report_l
+00005360: 6576 656c 944b 028c 0a68 616c 745f 6c65  evel.K...halt_le
+00005370: 7665 6c94 4b05 8c11 6578 6974 5f73 7461  vel.K...exit_sta
+00005380: 7475 735f 6c65 7665 6c94 4b05 8c05 6465  tus_level.K...de
+00005390: 6275 6794 4e8c 0e77 6172 6e69 6e67 5f73  bug.N..warning_s
+000053a0: 7472 6561 6d94 4e8c 0974 7261 6365 6261  tream.N..traceba
+000053b0: 636b 9488 8c0e 696e 7075 745f 656e 636f  ck....input_enco
+000053c0: 6469 6e67 948c 0975 7466 2d38 2d73 6967  ding...utf-8-sig
+000053d0: 948c 1c69 6e70 7574 5f65 6e63 6f64 696e  ...input_encodin
+000053e0: 675f 6572 726f 725f 6861 6e64 6c65 7294  g_error_handler.
+000053f0: 8c06 7374 7269 6374 948c 0f6f 7574 7075  ..strict...outpu
+00005400: 745f 656e 636f 6469 6e67 948c 0575 7466  t_encoding...utf
+00005410: 2d38 948c 1d6f 7574 7075 745f 656e 636f  -8...output_enco
+00005420: 6469 6e67 5f65 7272 6f72 5f68 616e 646c  ding_error_handl
+00005430: 6572 946a 8808 0000 8c0e 6572 726f 725f  er.j......error_
+00005440: 656e 636f 6469 6e67 948c 0575 7466 2d38  encoding...utf-8
+00005450: 948c 1c65 7272 6f72 5f65 6e63 6f64 696e  ...error_encodin
+00005460: 675f 6572 726f 725f 6861 6e64 6c65 7294  g_error_handler.
+00005470: 8c10 6261 636b 736c 6173 6872 6570 6c61  ..backslashrepla
+00005480: 6365 948c 0d6c 616e 6775 6167 655f 636f  ce...language_co
+00005490: 6465 948c 0265 6e94 8c13 7265 636f 7264  de...en...record
+000054a0: 5f64 6570 656e 6465 6e63 6965 7394 4e8c  _dependencies.N.
+000054b0: 0663 6f6e 6669 6794 4e8c 0969 645f 7072  .config.N..id_pr
+000054c0: 6566 6978 9468 068c 0e61 7574 6f5f 6964  efix.h...auto_id
+000054d0: 5f70 7265 6669 7894 8c02 6964 948c 0d64  _prefix...id...d
+000054e0: 756d 705f 7365 7474 696e 6773 944e 8c0e  ump_settings.N..
+000054f0: 6475 6d70 5f69 6e74 6572 6e61 6c73 944e  dump_internals.N
+00005500: 8c0f 6475 6d70 5f74 7261 6e73 666f 726d  ..dump_transform
+00005510: 7394 4e8c 0f64 756d 705f 7073 6575 646f  s.N..dump_pseudo
+00005520: 5f78 6d6c 944e 8c10 6578 706f 7365 5f69  _xml.N..expose_i
+00005530: 6e74 6572 6e61 6c73 944e 8c0e 7374 7269  nternals.N..stri
+00005540: 6374 5f76 6973 6974 6f72 944e 8c0f 5f64  ct_visitor.N.._d
+00005550: 6973 6162 6c65 5f63 6f6e 6669 6794 4e8c  isable_config.N.
+00005560: 075f 736f 7572 6365 9468 2c8c 0c5f 6465  ._source.h,.._de
+00005570: 7374 696e 6174 696f 6e94 4e8c 0d5f 636f  stination.N.._co
+00005580: 6e66 6967 5f66 696c 6573 945d 948c 1666  nfig_files.]...f
+00005590: 696c 655f 696e 7365 7274 696f 6e5f 656e  ile_insertion_en
+000055a0: 6162 6c65 6494 888c 0b72 6177 5f65 6e61  abled....raw_ena
+000055b0: 626c 6564 944b 018c 116c 696e 655f 6c65  bled.K...line_le
+000055c0: 6e67 7468 5f6c 696d 6974 944d 1027 8c0e  ngth_limit.M.'..
+000055d0: 7065 705f 7265 6665 7265 6e63 6573 944e  pep_references.N
+000055e0: 8c0c 7065 705f 6261 7365 5f75 726c 948c  ..pep_base_url..
+000055f0: 1868 7474 7073 3a2f 2f70 6570 732e 7079  .https://peps.py
+00005600: 7468 6f6e 2e6f 7267 2f94 8c15 7065 705f  thon.org/...pep_
+00005610: 6669 6c65 5f75 726c 5f74 656d 706c 6174  file_url_templat
+00005620: 6594 8c08 7065 702d 2530 3464 948c 0e72  e...pep-%04d...r
+00005630: 6663 5f72 6566 6572 656e 6365 7394 4e8c  fc_references.N.
+00005640: 0c72 6663 5f62 6173 655f 7572 6c94 8c26  .rfc_base_url..&
+00005650: 6874 7470 733a 2f2f 6461 7461 7472 6163  https://datatrac
+00005660: 6b65 722e 6965 7466 2e6f 7267 2f64 6f63  ker.ietf.org/doc
+00005670: 2f68 746d 6c2f 948c 0974 6162 5f77 6964  /html/...tab_wid
+00005680: 7468 944b 088c 1d74 7269 6d5f 666f 6f74  th.K...trim_foot
+00005690: 6e6f 7465 5f72 6566 6572 656e 6365 5f73  note_reference_s
+000056a0: 7061 6365 9489 8c10 7379 6e74 6178 5f68  pace....syntax_h
+000056b0: 6967 686c 6967 6874 948c 046c 6f6e 6794  ighlight...long.
+000056c0: 8c0c 736d 6172 745f 7175 6f74 6573 9488  ..smart_quotes..
+000056d0: 8c13 736d 6172 7471 756f 7465 735f 6c6f  ..smartquotes_lo
+000056e0: 6361 6c65 7394 5d94 8c1d 6368 6172 6163  cales.]...charac
+000056f0: 7465 725f 6c65 7665 6c5f 696e 6c69 6e65  ter_level_inline
+00005700: 5f6d 6172 6b75 7094 898c 0e64 6f63 7469  _markup....docti
+00005710: 746c 655f 7866 6f72 6d94 898c 0d64 6f63  tle_xform....doc
+00005720: 696e 666f 5f78 666f 726d 944b 018c 1273  info_xform.K...s
+00005730: 6563 7473 7562 7469 746c 655f 7866 6f72  ectsubtitle_xfor
+00005740: 6d94 898c 0d69 6d61 6765 5f6c 6f61 6469  m....image_loadi
+00005750: 6e67 948c 046c 696e 6b94 8c10 656d 6265  ng...link...embe
+00005760: 645f 7374 796c 6573 6865 6574 9489 8c15  d_stylesheet....
+00005770: 636c 6f61 6b5f 656d 6169 6c5f 6164 6472  cloak_email_addr
+00005780: 6573 7365 7394 888c 1173 6563 7469 6f6e  esses....section
+00005790: 5f73 656c 665f 6c69 6e6b 9489 8c03 656e  _self_link....en
+000057a0: 7694 4e75 628c 0872 6570 6f72 7465 7294  v.Nub..reporter.
+000057b0: 4e8c 1069 6e64 6972 6563 745f 7461 7267  N..indirect_targ
+000057c0: 6574 7394 5d94 8c11 7375 6273 7469 7475  ets.]...substitu
+000057d0: 7469 6f6e 5f64 6566 7394 7d94 8c12 7375  tion_defs.}...su
+000057e0: 6273 7469 7475 7469 6f6e 5f6e 616d 6573  bstitution_names
+000057f0: 947d 948c 0872 6566 6e61 6d65 7394 7d94  .}...refnames.}.
+00005800: 8c06 7265 6669 6473 947d 948c 076e 616d  ..refids.}...nam
+00005810: 6569 6473 947d 9428 6a62 0800 006a 5f08  eids.}.(jb...j_.
+00005820: 0000 6a5a 0800 006a 5708 0000 6a88 0300  ..jZ...jW...j...
+00005830: 006a 8503 0000 6a3d 0500 006a 3a05 0000  .j....j=...j:...
+00005840: 6a70 0600 006a 6d06 0000 6a52 0800 006a  jp...jm...jR...j
+00005850: 4f08 0000 758c 096e 616d 6574 7970 6573  O...u..nametypes
+00005860: 947d 9428 6a62 0800 0089 6a5a 0800 0089  .}.(jb....jZ....
+00005870: 6a88 0300 0089 6a3d 0500 0089 6a70 0600  j.....j=....jp..
+00005880: 0089 6a52 0800 0089 7568 217d 9428 6a5f  ..jR....uh!}.(j_
+00005890: 0800 0068 0c6a 5708 0000 684b 6a85 0300  ...h.jW...hKj...
+000058a0: 006a 0a01 0000 6a3a 0500 006a 8b03 0000  .j....j:...j....
+000058b0: 6a6d 0600 006a 4005 0000 6a4f 0800 006a  jm...j@...jO...j
+000058c0: 7306 0000 758c 0d66 6f6f 746e 6f74 655f  s...u..footnote_
+000058d0: 7265 6673 947d 948c 0d63 6974 6174 696f  refs.}...citatio
+000058e0: 6e5f 7265 6673 947d 948c 0d61 7574 6f66  n_refs.}...autof
+000058f0: 6f6f 746e 6f74 6573 945d 948c 1161 7574  ootnotes.]...aut
+00005900: 6f66 6f6f 746e 6f74 655f 7265 6673 945d  ofootnote_refs.]
+00005910: 948c 1073 796d 626f 6c5f 666f 6f74 6e6f  ...symbol_footno
+00005920: 7465 7394 5d94 8c14 7379 6d62 6f6c 5f66  tes.]...symbol_f
+00005930: 6f6f 746e 6f74 655f 7265 6673 945d 948c  ootnote_refs.]..
+00005940: 0966 6f6f 746e 6f74 6573 945d 948c 0963  .footnotes.]...c
+00005950: 6974 6174 696f 6e73 945d 948c 1261 7574  itations.]...aut
+00005960: 6f66 6f6f 746e 6f74 655f 7374 6172 7494  ofootnote_start.
+00005970: 4b01 8c15 7379 6d62 6f6c 5f66 6f6f 746e  K...symbol_footn
+00005980: 6f74 655f 7374 6172 7494 4b00 8c0a 6964  ote_start.K...id
+00005990: 5f63 6f75 6e74 6572 948c 0b63 6f6c 6c65  _counter...colle
+000059a0: 6374 696f 6e73 948c 0743 6f75 6e74 6572  ctions...Counter
+000059b0: 9493 947d 9485 9452 948c 0e70 6172 7365  ...}...R...parse
+000059c0: 5f6d 6573 7361 6765 7394 5d94 8c12 7472  _messages.]...tr
+000059d0: 616e 7366 6f72 6d5f 6d65 7373 6167 6573  ansform_messages
+000059e0: 945d 948c 0b74 7261 6e73 666f 726d 6572  .]...transformer
+000059f0: 944e 8c0b 696e 636c 7564 655f 6c6f 6794  .N..include_log.
+00005a00: 5d94 8c0a 6465 636f 7261 7469 6f6e 944e  ]...decoration.N
+00005a10: 681c 6803 7562 2e                        h.h.ub.
```

### Comparing `nester-struct-0.5.1/docs/_build/html/_sources/index.rst.txt` & `nester-struct-0.5.2/docs/_build/html/_sources/index.rst.txt`

 * *Files 24% similar despite different names*

```diff
@@ -12,14 +12,15 @@
    :maxdepth: 2
    :caption: Contents:
 
    Installation <installation_guide>
    Usage <usage_guide>
    Developer Docs <dev_docs>
       The `utils` module <source/utils>
+      The `nester_log` module <source/logging>
    Supported Languages <supported_languages>
 
 
 
 Indices and tables
 ==================
```

### Comparing `nester-struct-0.5.1/docs/_build/html/_sources/supported_languages.rst.txt` & `nester-struct-0.5.2/docs/_build/html/_sources/supported_languages.rst.txt`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/docs/_build/html/_sources/usage_guide.rst.txt` & `nester-struct-0.5.2/docs/_build/html/_sources/usage_guide.rst.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Nester has four main functions it can perform:
 
 - `create`
 - `validate`
 - `list`
 - `clean`
 
-Let us look into each three in more detail...
+Let us look into each of the four commands in more detail...
 
 Nester create
 ~~~~~~~~~~~~~~~
 
 .. function:: nester create(language, projectname, [-g|--git])
 
    Creates the project structure for the given project.
@@ -50,18 +50,19 @@
   :param language: The shortform of a supported programming language. Refer to the :doc: `list of supported languages <supported_languages>`.
   :type language: str
   :param projectname: The name of the project or package you want to validate
   :type projectname: str
   :return: Tells you via Terminal wether your structure lines up or not.
   :rtype: str
 
-Nester list
+Nester log
 ~~~~~~~~~~~
 
-.. function:: nester list()
+.. function:: nester log()
+
   Lists all previously created projects, which had logging enabled, in a table.
 
   :param --clean: An optional flag to clean up orphaned log entries.
   :type --clean: flag
   :return: None
   :rtype: None
```

### Comparing `nester-struct-0.5.1/docs/_build/html/_static/basic.css` & `nester-struct-0.5.2/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/docs/_build/html/_static/css/badge_only.css` & `nester-struct-0.5.2/docs/_build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/docs/_build/html/_static/css/custom.css` & `nester-struct-0.5.2/docs/_build/html/_static/css/custom.css`

 * *Files 0% similar despite different names*

```diff
@@ -67,11 +67,11 @@
 html.writer-html5 body.wy-body-for-nav div.wy-grid-for-nav nav.wy-nav-side div.wy-side-scroll div.wy-menu.wy-menu-vertical ul.current li.toctree-l1.current ul li.toctree-l2 a.reference.internal,
 html.writer-html5 body.wy-body-for-nav div.wy-grid-for-nav nav.wy-nav-side div.wy-side-scroll div.wy-menu.wy-menu-vertical ul.current li.toctree-l1.current a.current.reference.internal {
   background-color: #111;
 }
 
 /*Change background color of rendered code in toc on index.rst*/
 html.writer-html5 body.wy-body-for-nav div.wy-grid-for-nav section.wy-nav-content-wrap div.wy-nav-content div.rst-content div.document div section#welcome-to-nester-s-documentation div.toctree-wrapper.compound ul li.toctree-l1 ul li.toctree-l2 a.reference.internal code.docutils.literal.notranslate {
-  background-color: #222;
+  background-color: #ffff;
   color: #ff5100;
   border-style: hidden;
 }
```

### Comparing `nester-struct-0.5.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `nester-struct-0.5.2/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `nester-struct-0.5.2/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `nester-struct-0.5.2/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `nester-struct-0.5.2/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot` & `nester-struct-0.5.2/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg` & `nester-struct-0.5.2/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf` & `nester-struct-0.5.2/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff` & `nester-struct-0.5.2/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2` & `nester-struct-0.5.2/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/docs/_build/html/_static/css/fonts/lato-bold-italic.woff` & `nester-struct-0.5.2/docs/_build/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2` & `nester-struct-0.5.2/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/docs/_build/html/_static/css/fonts/lato-bold.woff` & `nester-struct-0.5.2/docs/_build/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/docs/_build/html/_static/css/fonts/lato-bold.woff2` & `nester-struct-0.5.2/docs/_build/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/docs/_build/html/_static/css/fonts/lato-normal-italic.woff` & `nester-struct-0.5.2/docs/_build/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2` & `nester-struct-0.5.2/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/docs/_build/html/_static/css/fonts/lato-normal.woff` & `nester-struct-0.5.2/docs/_build/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/docs/_build/html/_static/css/fonts/lato-normal.woff2` & `nester-struct-0.5.2/docs/_build/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/docs/_build/html/_static/css/theme.css` & `nester-struct-0.5.2/docs/_build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/docs/_build/html/_static/doctools.js` & `nester-struct-0.5.2/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/docs/_build/html/_static/index_logo.png` & `nester-struct-0.5.2/docs/_build/html/_static/index_logo.png`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/docs/_build/html/_static/js/badge_only.js` & `nester-struct-0.5.2/docs/_build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/docs/_build/html/_static/js/html5shiv-printshiv.min.js` & `nester-struct-0.5.2/docs/_build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/docs/_build/html/_static/js/html5shiv.min.js` & `nester-struct-0.5.2/docs/_build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/docs/_build/html/_static/js/theme.js` & `nester-struct-0.5.2/docs/_build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/docs/_build/html/_static/language_data.js` & `nester-struct-0.5.2/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/docs/_build/html/_static/pygments.css` & `nester-struct-0.5.2/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/docs/_build/html/_static/searchtools.js` & `nester-struct-0.5.2/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/docs/_build/html/_static/sphinx_highlight.js` & `nester-struct-0.5.2/docs/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/docs/_build/html/dev_docs.html` & `nester-struct-0.5.2/docs/_build/html/search.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
-  <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
-
+  <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Developer Docs &mdash; Nester  documentation</title>
+  <title>Search &mdash; Nester  documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/custom.css" type="text/css" />
+    
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/doctools.js"></script>
         <script src="_static/sphinx_highlight.js"></script>
     <script src="_static/js/theme.js"></script>
+    <script src="_static/searchtools.js"></script>
+    <script src="_static/language_data.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
-    <link rel="search" title="Search" href="search.html" />
-    <link rel="next" title="The Utils module" href="source/utils.html" />
-    <link rel="prev" title="Usage" href="usage_guide.html" /> 
+    <link rel="search" title="Search" href="#" /> 
 </head>
 
 <body class="wy-body-for-nav"> 
   <div class="wy-grid-for-nav">
     <nav data-toggle="wy-nav-shift" class="wy-nav-side">
       <div class="wy-side-scroll">
         <div class="wy-side-nav-search" >
@@ -31,27 +31,28 @@
           
           
           <a href="index.html">
             
               <img src="_static/index_logo.png" class="logo" alt="Logo"/>
           </a>
 <div role="search">
-  <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
+  <form id="rtd-search-form" class="wy-form" action="#" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
 </div>
         </div><div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
               <p class="caption" role="heading"><span class="caption-text">Contents:</span></p>
-<ul class="current">
+<ul>
 <li class="toctree-l1"><a class="reference internal" href="installation_guide.html">Installation</a></li>
 <li class="toctree-l1"><a class="reference internal" href="usage_guide.html">Usage</a></li>
-<li class="toctree-l1 current"><a class="current reference internal" href="#">Developer Docs</a></li>
+<li class="toctree-l1"><a class="reference internal" href="dev_docs.html">Developer Docs</a></li>
 <li class="toctree-l1"><a class="reference internal" href="source/utils.html">   The `utils` module</a></li>
+<li class="toctree-l1"><a class="reference internal" href="source/logging.html">   The `nester_log` module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="supported_languages.html">Supported Languages</a></li>
 </ul>
 
         </div>
       </div>
     </nav>
 
@@ -61,35 +62,39 @@
       </nav>
 
       <div class="wy-nav-content">
         <div class="rst-content">
           <div role="navigation" aria-label="Page navigation">
   <ul class="wy-breadcrumbs">
       <li><a href="index.html" class="icon icon-home" aria-label="Home"></a></li>
-      <li class="breadcrumb-item active">Developer Docs</li>
+      <li class="breadcrumb-item active">Search</li>
       <li class="wy-breadcrumbs-aside">
-            <a href="_sources/dev_docs.rst.txt" rel="nofollow"> View page source</a>
       </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
              
-  <section id="developer-docs">
-<h1>Developer Docs<a class="headerlink" href="#developer-docs" title="Permalink to this heading"></a></h1>
-</section>
+  <noscript>
+  <div id="fallback" class="admonition warning">
+    <p class="last">
+      Please activate JavaScript to enable the search functionality.
+    </p>
+  </div>
+  </noscript>
 
+  
+  <div id="search-results">
+  
+  </div>
 
            </div>
           </div>
-          <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
-        <a href="usage_guide.html" class="btn btn-neutral float-left" title="Usage" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
-        <a href="source/utils.html" class="btn btn-neutral float-right" title="The Utils module" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
-    </div>
+          <footer>
 
   <hr/>
 
   <div role="contentinfo">
     <p>&#169; Copyright 2023, Christopher Hock aka ByteOtter.</p>
   </div>
 
@@ -103,11 +108,18 @@
       </div>
     </section>
   </div>
   <script>
       jQuery(function () {
           SphinxRtdTheme.Navigation.enable(true);
       });
-  </script> 
+  </script>
+  <script>
+    jQuery(function() { Search.loadIndex("searchindex.js"); });
+  </script>
+  
+  <script id="searchindexloader"></script>
+   
+
 
 </body>
 </html>
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,25 +1,23 @@
 
 
 
 
 
 
-
-
 [Logo]
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Developer_Docs
     * The_`utils`_module
+    * The_`nester_log`_module
     * Supported_Languages
    Nester
-    * Developer Docs
-    * View_page_source
+    * Search
 ===============================================================================
-****** Developer Docsï ******
-Previous Next
+Please activate JavaScript to enable the search functionality.
+
 ===============================================================================
 © Copyright 2023, Christopher Hock aka ByteOtter.
 Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `nester-struct-0.5.1/docs/_build/html/genindex.html` & `nester-struct-0.5.2/docs/_build/html/genindex.html`

 * *Files 26% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         </div><div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
               <p class="caption" role="heading"><span class="caption-text">Contents:</span></p>
 <ul>
 <li class="toctree-l1"><a class="reference internal" href="installation_guide.html">Installation</a></li>
 <li class="toctree-l1"><a class="reference internal" href="usage_guide.html">Usage</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dev_docs.html">Developer Docs</a></li>
 <li class="toctree-l1"><a class="reference internal" href="source/utils.html">   The `utils` module</a></li>
+<li class="toctree-l1"><a class="reference internal" href="source/logging.html">   The `nester_log` module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="supported_languages.html">Supported Languages</a></li>
 </ul>
 
         </div>
       </div>
     </nav>
 
@@ -73,41 +74,58 @@
              
 
 <h1 id="index">Index</h1>
 
 <div class="genindex-jumpbox">
  <a href="#C"><strong>C</strong></a>
  | <a href="#D"><strong>D</strong></a>
+ | <a href="#F"><strong>F</strong></a>
  | <a href="#G"><strong>G</strong></a>
  | <a href="#L"><strong>L</strong></a>
  | <a href="#M"><strong>M</strong></a>
  | <a href="#N"><strong>N</strong></a>
+ | <a href="#P"><strong>P</strong></a>
+ | <a href="#R"><strong>R</strong></a>
  | <a href="#V"><strong>V</strong></a>
  
 </div>
 <h2 id="C">C</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
+      <li><a href="source/logging.html#nester.nester_log.check_log_for_duplicate">check_log_for_duplicate() (in module nester.nester_log)</a>
+</li>
       <li><a href="source/utils.html#nester.utils.clean">clean() (in module nester.utils)</a>
 </li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
+      <li><a href="source/logging.html#nester.nester_log.clean_orphaned_entries">clean_orphaned_entries() (in module nester.nester_log)</a>
+</li>
+      <li><a href="source/logging.html#nester.nester_log.create_log_file_if_none">create_log_file_if_none() (in module nester.nester_log)</a>
+</li>
       <li><a href="source/utils.html#nester.utils.create_structure">create_structure() (in module nester.utils)</a>
 </li>
   </ul></td>
 </tr></table>
 
 <h2 id="D">D</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="source/utils.html#nester.utils.detect_languages">detect_languages() (in module nester.utils)</a>
 </li>
   </ul></td>
 </tr></table>
 
+<h2 id="F">F</h2>
+<table style="width: 100%" class="indextable genindextable"><tr>
+  <td style="width: 33%; vertical-align: top;"><ul>
+      <li><a href="source/logging.html#nester.nester_log.ProjectLogFormatter.format">format() (nester.nester_log.ProjectLogFormatter method)</a>
+</li>
+  </ul></td>
+</tr></table>
+
 <h2 id="G">G</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="source/utils.html#nester.utils.get_project_dir">get_project_dir() (in module nester.utils)</a>
 </li>
   </ul></td>
 </tr></table>
@@ -123,33 +141,66 @@
 <h2 id="M">M</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li>
     module
 
       <ul>
+        <li><a href="source/logging.html#module-nester.nester_log">nester.nester_log</a>
+</li>
         <li><a href="source/utils.html#module-nester.utils">nester.utils</a>
 </li>
       </ul></li>
   </ul></td>
 </tr></table>
 
 <h2 id="N">N</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li>
+    nester.nester_log
+
+      <ul>
+        <li><a href="source/logging.html#module-nester.nester_log">module</a>
+</li>
+      </ul></li>
+  </ul></td>
+  <td style="width: 33%; vertical-align: top;"><ul>
+      <li>
     nester.utils
 
       <ul>
         <li><a href="source/utils.html#module-nester.utils">module</a>
 </li>
       </ul></li>
   </ul></td>
 </tr></table>
 
+<h2 id="P">P</h2>
+<table style="width: 100%" class="indextable genindextable"><tr>
+  <td style="width: 33%; vertical-align: top;"><ul>
+      <li><a href="source/logging.html#nester.nester_log.print_log_to_table">print_log_to_table() (in module nester.nester_log)</a>
+</li>
+  </ul></td>
+  <td style="width: 33%; vertical-align: top;"><ul>
+      <li><a href="source/logging.html#nester.nester_log.ProjectLogFormatter.process">process() (nester.nester_log.ProjectLogFormatter method)</a>
+</li>
+      <li><a href="source/logging.html#nester.nester_log.ProjectLogFormatter">ProjectLogFormatter (class in nester.nester_log)</a>
+</li>
+  </ul></td>
+</tr></table>
+
+<h2 id="R">R</h2>
+<table style="width: 100%" class="indextable genindextable"><tr>
+  <td style="width: 33%; vertical-align: top;"><ul>
+      <li><a href="source/logging.html#nester.nester_log.remove_log_entry">remove_log_entry() (in module nester.nester_log)</a>
+</li>
+  </ul></td>
+</tr></table>
+
 <h2 id="V">V</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="source/utils.html#nester.utils.validate_structure">validate_structure() (in module nester.utils)</a>
 </li>
   </ul></td>
 </tr></table>
```

#### html2text {}

```diff
@@ -7,34 +7,50 @@
 [Logo]
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Developer_Docs
     * The_`utils`_module
+    * The_`nester_log`_module
     * Supported_Languages
    Nester
     * Index
 ===============================================================================
 ****** Index ******
-C | D | G | L | M | N | V
+C | D | F | G | L | M | N | P | R | V
 ***** C *****
-    * clean()_(in_module_nester.utils)     * create_structure()_(in_module
+                                           * clean_orphaned_entries()_(in
+    * check_log_for_duplicate()_(in          module_nester.nester_log)
+      module_nester.nester_log)            * create_log_file_if_none()_(in
+    * clean()_(in_module_nester.utils)       module_nester.nester_log)
+                                           * create_structure()_(in_module
                                              nester.utils)
 ***** D *****
     * detect_languages()_(in_module_nester.utils)
+***** F *****
+    * format()_(nester.nester_log.ProjectLogFormatter_method)
 ***** G *****
     * get_project_dir()_(in_module_nester.utils)
 ***** L *****
     * load_json()_(in_module_nester.utils)
 ***** M *****
     * module
+          o nester.nester_log
           o nester.utils
 ***** N *****
-    * nester.utils
-          o module
+    * nester.nester_log     * nester.utils
+          o module                o module
+***** P *****
+                                    * process()_
+    * print_log_to_table()_(in        (nester.nester_log.ProjectLogFormatter
+      module_nester.nester_log)       method)
+                                    * ProjectLogFormatter_(class_in
+                                      nester.nester_log)
+***** R *****
+    * remove_log_entry()_(in_module_nester.nester_log)
 ***** V *****
     * validate_structure()_(in_module_nester.utils)
 
 ===============================================================================
 © Copyright 2023, Christopher Hock aka ByteOtter.
 Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `nester-struct-0.5.1/docs/_build/html/index.html` & `nester-struct-0.5.2/docs/_build/html/supported_languages.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,127 +1,120 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Welcome to Nester’s documentation! &mdash; Nester  documentation</title>
+  <title>Supported languages &mdash; Nester  documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/custom.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/doctools.js"></script>
         <script src="_static/sphinx_highlight.js"></script>
     <script src="_static/js/theme.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
-    <link rel="next" title="Installing Nester" href="installation_guide.html" /> 
+    <link rel="prev" title="The Utils module" href="source/utils.html" /> 
 </head>
 
 <body class="wy-body-for-nav"> 
   <div class="wy-grid-for-nav">
     <nav data-toggle="wy-nav-shift" class="wy-nav-side">
       <div class="wy-side-scroll">
         <div class="wy-side-nav-search" >
 
           
           
-          <a href="#">
+          <a href="index.html">
             
               <img src="_static/index_logo.png" class="logo" alt="Logo"/>
           </a>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
 </div>
         </div><div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
               <p class="caption" role="heading"><span class="caption-text">Contents:</span></p>
-<ul>
+<ul class="current">
 <li class="toctree-l1"><a class="reference internal" href="installation_guide.html">Installation</a></li>
 <li class="toctree-l1"><a class="reference internal" href="usage_guide.html">Usage</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dev_docs.html">Developer Docs</a></li>
 <li class="toctree-l1"><a class="reference internal" href="source/utils.html">   The `utils` module</a></li>
-<li class="toctree-l1"><a class="reference internal" href="supported_languages.html">Supported Languages</a></li>
+<li class="toctree-l1 current"><a class="current reference internal" href="#">Supported Languages</a></li>
 </ul>
 
         </div>
       </div>
     </nav>
 
     <section data-toggle="wy-nav-shift" class="wy-nav-content-wrap"><nav class="wy-nav-top" aria-label="Mobile navigation menu" >
           <i data-toggle="wy-nav-top" class="fa fa-bars"></i>
-          <a href="#">Nester</a>
+          <a href="index.html">Nester</a>
       </nav>
 
       <div class="wy-nav-content">
         <div class="rst-content">
           <div role="navigation" aria-label="Page navigation">
   <ul class="wy-breadcrumbs">
-      <li><a href="#" class="icon icon-home" aria-label="Home"></a></li>
-      <li class="breadcrumb-item active">Welcome to Nester’s documentation!</li>
+      <li><a href="index.html" class="icon icon-home" aria-label="Home"></a></li>
+      <li class="breadcrumb-item active">Supported languages</li>
       <li class="wy-breadcrumbs-aside">
-            <a href="_sources/index.rst.txt" rel="nofollow"> View page source</a>
+            <a href="_sources/supported_languages.rst.txt" rel="nofollow"> View page source</a>
       </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
              
-  <section id="welcome-to-nester-s-documentation">
-<h1>Welcome to Nester’s documentation!<a class="headerlink" href="#welcome-to-nester-s-documentation" title="Permalink to this heading"></a></h1>
-<p>Nester is your convenient CLI companion which lays the foundation for your programming projects.</p>
-<div class="toctree-wrapper compound">
-<p class="caption" role="heading"><span class="caption-text">Contents:</span></p>
-<ul>
-<li class="toctree-l1"><a class="reference internal" href="installation_guide.html">Installation</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="installation_guide.html#installation-via-pip">Installation via <cite>pip</cite></a></li>
-<li class="toctree-l2"><a class="reference internal" href="installation_guide.html#installation-as-rpm-package">Installation as <cite>rpm</cite> package</a></li>
-<li class="toctree-l2"><a class="reference internal" href="installation_guide.html#building-from-source">Building from source</a></li>
-</ul>
-</li>
-<li class="toctree-l1"><a class="reference internal" href="usage_guide.html">Usage</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="usage_guide.html#cli-mode">CLI-Mode</a></li>
-</ul>
-</li>
-<li class="toctree-l1"><a class="reference internal" href="dev_docs.html">Developer Docs</a></li>
-<li class="toctree-l1"><a class="reference internal" href="source/utils.html">   The `utils` module</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="source/utils.html#nester.utils.clean"><code class="docutils literal notranslate"><span class="pre">clean()</span></code></a></li>
-<li class="toctree-l2"><a class="reference internal" href="source/utils.html#nester.utils.create_structure"><code class="docutils literal notranslate"><span class="pre">create_structure()</span></code></a></li>
-<li class="toctree-l2"><a class="reference internal" href="source/utils.html#nester.utils.detect_languages"><code class="docutils literal notranslate"><span class="pre">detect_languages()</span></code></a></li>
-<li class="toctree-l2"><a class="reference internal" href="source/utils.html#nester.utils.get_project_dir"><code class="docutils literal notranslate"><span class="pre">get_project_dir()</span></code></a></li>
-<li class="toctree-l2"><a class="reference internal" href="source/utils.html#nester.utils.load_json"><code class="docutils literal notranslate"><span class="pre">load_json()</span></code></a></li>
-<li class="toctree-l2"><a class="reference internal" href="source/utils.html#nester.utils.validate_structure"><code class="docutils literal notranslate"><span class="pre">validate_structure()</span></code></a></li>
-</ul>
-</li>
-<li class="toctree-l1"><a class="reference internal" href="supported_languages.html">Supported Languages</a></li>
-</ul>
-</div>
-</section>
-<section id="indices-and-tables">
-<h1>Indices and tables<a class="headerlink" href="#indices-and-tables" title="Permalink to this heading"></a></h1>
-<ul class="simple">
-<li><p><a class="reference internal" href="genindex.html"><span class="std std-ref">Index</span></a></p></li>
-<li><p><a class="reference internal" href="py-modindex.html"><span class="std std-ref">Module Index</span></a></p></li>
-<li><p><a class="reference internal" href="search.html"><span class="std std-ref">Search Page</span></a></p></li>
-</ul>
+  <section id="supported-languages">
+<h1>Supported languages<a class="headerlink" href="#supported-languages" title="Permalink to this heading"></a></h1>
+<table class="docutils align-default" id="id1">
+<caption><span class="caption-text">Supported Language Shortforms</span><a class="headerlink" href="#id1" title="Permalink to this table"></a></caption>
+<thead>
+<tr class="row-odd"><th class="head"><p>Shortform</p></th>
+<th class="head"><p>Language</p></th>
+</tr>
+</thead>
+<tbody>
+<tr class="row-even"><td><p><code class="docutils literal notranslate"><span class="pre">py</span></code></p></td>
+<td><p>Python</p></td>
+</tr>
+<tr class="row-odd"><td><p><code class="docutils literal notranslate"><span class="pre">java</span></code></p></td>
+<td><p>Java</p></td>
+</tr>
+<tr class="row-even"><td><p><code class="docutils literal notranslate"><span class="pre">cs</span></code></p></td>
+<td><p>C#</p></td>
+</tr>
+<tr class="row-odd"><td><p><code class="docutils literal notranslate"><span class="pre">cpp</span></code></p></td>
+<td><p>C++</p></td>
+</tr>
+<tr class="row-even"><td><p><code class="docutils literal notranslate"><span class="pre">c</span></code></p></td>
+<td><p>C</p></td>
+</tr>
+<tr class="row-odd"><td><p><code class="docutils literal notranslate"><span class="pre">rb</span></code></p></td>
+<td><p>Ruby</p></td>
+</tr>
+</tbody>
+</table>
 </section>
 
 
            </div>
           </div>
           <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
-        <a href="installation_guide.html" class="btn btn-neutral float-right" title="Installing Nester" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
+        <a href="source/utils.html" class="btn btn-neutral float-left" title="The Utils module" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
     </div>
 
   <hr/>
 
   <div role="contentinfo">
     <p>&#169; Copyright 2023, Christopher Hock aka ByteOtter.</p>
   </div>
```

#### html2text {}

```diff
@@ -10,38 +10,24 @@
 Contents:
     * Installation
     * Usage
     * Developer_Docs
     * The_`utils`_module
     * Supported_Languages
    Nester
-    * Welcome to Nesterâs documentation!
+    * Supported languages
     * View_page_source
 ===============================================================================
-****** Welcome to Nesterâs documentation!ï ******
-Nester is your convenient CLI companion which lays the foundation for your
-programming projects.
-Contents:
-    * Installation
-          o Installation_viapip
-          o Installation_asrpmpackage
-          o Building_from_source
-    * Usage
-          o CLI-Mode
-    * Developer_Docs
-    * The_`utils`_module
-          o clean()
-          o create_structure()
-          o detect_languages()
-          o get_project_dir()
-          o load_json()
-          o validate_structure()
-    * Supported_Languages
-
-****** Indices and tablesï ******
-    * Index
-    * Module_Index
-    * Search_Page
-Next
+****** Supported languagesï ******
+Supported Language
+  Shortformsï
+Shortform Language
+py        Python
+java      Java
+cs        C#
+cpp       C++
+c         C
+rb        Ruby
+Previous
 ===============================================================================
 © Copyright 2023, Christopher Hock aka ByteOtter.
 Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `nester-struct-0.5.1/docs/_build/html/installation_guide.html` & `nester-struct-0.5.2/docs/_build/html/installation_guide.html`

 * *Files 9% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 <li class="toctree-l2"><a class="reference internal" href="#installation-as-rpm-package">Installation as <cite>rpm</cite> package</a></li>
 <li class="toctree-l2"><a class="reference internal" href="#building-from-source">Building from source</a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="usage_guide.html">Usage</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dev_docs.html">Developer Docs</a></li>
 <li class="toctree-l1"><a class="reference internal" href="source/utils.html">   The `utils` module</a></li>
+<li class="toctree-l1"><a class="reference internal" href="source/logging.html">   The `nester_log` module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="supported_languages.html">Supported Languages</a></li>
 </ul>
 
         </div>
       </div>
     </nav>
 
@@ -99,20 +100,36 @@
 </section>
 <section id="installation-as-rpm-package">
 <h2>Installation as <cite>rpm</cite> package<a class="headerlink" href="#installation-as-rpm-package" title="Permalink to this heading"></a></h2>
 <p>–COMING SOON–</p>
 <p>Some systems may not initially ship with <cite>python3</cite> or <cite>pip</cite> or you may simply do not want to use <cite>pip</cite>.
 For this reason we are planning to offer Nester in a varietly of different Linux packages.</p>
 <p>As we are most familiar with the <cite>rpm</cite> format for openSUSE this is what we will offer first.</p>
-<p>Note: This is a feature we will offer at some point. No dates are planned yet!</p>
-<p>To install it run</p>
-<div class="highlight-shell notranslate"><div class="highlight"><pre><span></span>sudo<span class="w"> </span>zypper<span class="w"> </span><span class="k">in</span><span class="w"> </span>nester
+<p>We can now offer a <cite>.rpm</cite> package!</p>
+<p>To do so follow these steps (on openSUSE):</p>
+<ol class="arabic simple">
+<li><p>Add the repository</p></li>
+</ol>
+<div class="highlight-shell notranslate"><div class="highlight"><pre><span></span>sudo<span class="w"> </span>zypper<span class="w"> </span>addrepo<span class="w"> </span><span class="sb">`</span>https://download.opensuse.org/repositories/home:kodymo/openSUSE_Tumbleweed/home:kodymo.repo<span class="sb">`</span>_
 </pre></div>
 </div>
-<p>This should install the package.</p>
+<ol class="arabic simple" id="https-download-opensuse-org-repositories-home-kodymo-opensuse-tumbleweed-home-kodymo-repo" start="2">
+<li><p>Refresh your repositories</p></li>
+</ol>
+<div class="highlight-shell notranslate"><div class="highlight"><pre><span></span>sudo<span class="w"> </span>zypper<span class="w"> </span>ref
+</pre></div>
+</div>
+<ol class="arabic simple" start="3">
+<li><p>Install Nester</p></li>
+</ol>
+<div class="highlight-shell notranslate"><div class="highlight"><pre><span></span>sudo<span class="w"> </span>zypper<span class="w"> </span>install<span class="w"> </span>python3-nester
+</pre></div>
+</div>
+<p>Note: The repository contains three builds for nester for Python 3.9, 3.10 and 3.11. <cite>zypper</cite> will automatically decide which version to use when running the command above.</p>
+<p>You can visit the repository on the [package maintainer’s OBS account](<a class="reference external" href="https://build.opensuse.org/package/show/home:kodymo/python-nester">https://build.opensuse.org/package/show/home:kodymo/python-nester</a>).</p>
 </section>
 <section id="building-from-source">
 <h2>Building from source<a class="headerlink" href="#building-from-source" title="Permalink to this heading"></a></h2>
 <p>Sometimes installing from shady sources may not be your thing. Fear nought!
 You can also build it from source.</p>
 <p>To do that simply clone or download <a class="reference external" href="https://github.com/ByteOtter/nester">Nester’s GitHub repository</a> enter the <cite>nester/</cite> directory and run <cite>pip install .</cite> to install Nester.</p>
 <p>Done!</p>
```

#### html2text {}

```diff
@@ -12,14 +12,15 @@
     * Installation
           o Installation_viapip
           o Installation_asrpmpackage
           o Building_from_source
     * Usage
     * Developer_Docs
     * The_`utils`_module
+    * The_`nester_log`_module
     * Supported_Languages
    Nester
     * Installing Nester
     * View_page_source
 ===============================================================================
 ****** Installing Nesterï ******
 Nester will initially be offered in three ways:
@@ -36,18 +37,28 @@
 ***** Installation asrpmpackageï *****
 âCOMING SOONâ
 Some systems may not initially ship withpython3orpipor you may simply do not
 want to usepip. For this reason we are planning to offer Nester in a varietly
 of different Linux packages.
 As we are most familiar with therpmformat for openSUSE this is what we will
 offer first.
-Note: This is a feature we will offer at some point. No dates are planned yet!
-To install it run
-sudo zypper in nester
-This should install the package.
+We can now offer a.rpmpackage!
+To do so follow these steps (on openSUSE):
+   1. Add the repository
+sudo zypper addrepo `https://download.opensuse.org/repositories/home:kodymo/
+openSUSE_Tumbleweed/home:kodymo.repo`_
+   1. Refresh your repositories
+sudo zypper ref
+   1. Install Nester
+sudo zypper install python3-nester
+Note: The repository contains three builds for nester for Python 3.9, 3.10 and
+3.11.zypperwill automatically decide which version to use when running the
+command above.
+You can visit the repository on the [package maintainerâs OBS account](https:
+//build.opensuse.org/package/show/home:kodymo/python-nester).
 
 ***** Building from sourceï *****
 Sometimes installing from shady sources may not be your thing. Fear nought! You
 can also build it from source.
 To do that simply clone or download Nesterâs_GitHub_repository enter
 thenester/directory and runpip install .to install Nester.
 Done!
```

### Comparing `nester-struct-0.5.1/docs/_build/html/py-modindex.html` & `nester-struct-0.5.2/docs/_build/html/py-modindex.html`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,15 @@
         </div><div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
               <p class="caption" role="heading"><span class="caption-text">Contents:</span></p>
 <ul>
 <li class="toctree-l1"><a class="reference internal" href="installation_guide.html">Installation</a></li>
 <li class="toctree-l1"><a class="reference internal" href="usage_guide.html">Usage</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dev_docs.html">Developer Docs</a></li>
 <li class="toctree-l1"><a class="reference internal" href="source/utils.html">   The `utils` module</a></li>
+<li class="toctree-l1"><a class="reference internal" href="source/logging.html">   The `nester_log` module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="supported_languages.html">Supported Languages</a></li>
 </ul>
 
         </div>
       </div>
     </nav>
 
@@ -90,14 +91,19 @@
               id="toggle-1" style="display: none" alt="-" /></td>
        <td>
        <code class="xref">nester</code></td><td>
        <em></em></td></tr>
      <tr class="cg-1">
        <td></td>
        <td>&#160;&#160;&#160;
+       <a href="source/logging.html#module-nester.nester_log"><code class="xref">nester.nester_log</code></a></td><td>
+       <em></em></td></tr>
+     <tr class="cg-1">
+       <td></td>
+       <td>&#160;&#160;&#160;
        <a href="source/utils.html#module-nester.utils"><code class="xref">nester.utils</code></a></td><td>
        <em></em></td></tr>
    </table>
 
 
            </div>
           </div>
```

#### html2text {}

```diff
@@ -7,21 +7,23 @@
 [Logo]
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Developer_Docs
     * The_`utils`_module
+    * The_`nester_log`_module
     * Supported_Languages
    Nester
     * Python Module Index
 ===============================================================================
 ****** Python Module Index ******
 n
      
     n
 [-] nester
+        nester.nester_log
         nester.utils
 
 ===============================================================================
 © Copyright 2023, Christopher Hock aka ByteOtter.
 Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `nester-struct-0.5.1/docs/_build/html/source/utils.html` & `nester-struct-0.5.2/docs/_build/html/source/utils.html`

 * *Files 3% similar despite different names*

```diff
@@ -14,16 +14,16 @@
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
         <script src="../_static/doctools.js"></script>
         <script src="../_static/sphinx_highlight.js"></script>
     <script src="../_static/js/theme.js"></script>
     <link rel="index" title="Index" href="../genindex.html" />
     <link rel="search" title="Search" href="../search.html" />
-    <link rel="next" title="Supported languages" href="../supported_languages.html" />
-    <link rel="prev" title="Developer Docs" href="../dev_docs.html" /> 
+    <link rel="next" title="The Nester Log module" href="logging.html" />
+    <link rel="prev" title="Contributing to Nester" href="../contributing.html" /> 
 </head>
 
 <body class="wy-body-for-nav"> 
   <div class="wy-grid-for-nav">
     <nav data-toggle="wy-nav-shift" class="wy-nav-side">
       <div class="wy-side-scroll">
         <div class="wy-side-nav-search" >
@@ -52,14 +52,15 @@
 <li class="toctree-l2"><a class="reference internal" href="#nester.utils.create_structure"><code class="docutils literal notranslate"><span class="pre">create_structure()</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="#nester.utils.detect_languages"><code class="docutils literal notranslate"><span class="pre">detect_languages()</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="#nester.utils.get_project_dir"><code class="docutils literal notranslate"><span class="pre">get_project_dir()</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="#nester.utils.load_json"><code class="docutils literal notranslate"><span class="pre">load_json()</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="#nester.utils.validate_structure"><code class="docutils literal notranslate"><span class="pre">validate_structure()</span></code></a></li>
 </ul>
 </li>
+<li class="toctree-l1"><a class="reference internal" href="logging.html">   The `nester_log` module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="../supported_languages.html">Supported Languages</a></li>
 </ul>
 
         </div>
       </div>
     </nav>
 
@@ -69,14 +70,15 @@
       </nav>
 
       <div class="wy-nav-content">
         <div class="rst-content">
           <div role="navigation" aria-label="Page navigation">
   <ul class="wy-breadcrumbs">
       <li><a href="../index.html" class="icon icon-home" aria-label="Home"></a></li>
+          <li class="breadcrumb-item"><a href="../dev_docs.html">Developer Docs</a></li>
       <li class="breadcrumb-item active">The Utils module</li>
       <li class="wy-breadcrumbs-aside">
             <a href="../_sources/source/utils.rst.txt" rel="nofollow"> View page source</a>
       </li>
   </ul>
   <hr/>
 </div>
@@ -200,16 +202,16 @@
 
 </section>
 
 
            </div>
           </div>
           <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
-        <a href="../dev_docs.html" class="btn btn-neutral float-left" title="Developer Docs" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
-        <a href="../supported_languages.html" class="btn btn-neutral float-right" title="Supported languages" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
+        <a href="../contributing.html" class="btn btn-neutral float-left" title="Contributing to Nester" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
+        <a href="logging.html" class="btn btn-neutral float-right" title="The Nester Log module" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
     </div>
 
   <hr/>
 
   <div role="contentinfo">
     <p>&#169; Copyright 2023, Christopher Hock aka ByteOtter.</p>
   </div>
```

#### html2text {}

```diff
@@ -15,16 +15,18 @@
     * The_`utils`_module
           o clean()
           o create_structure()
           o detect_languages()
           o get_project_dir()
           o load_json()
           o validate_structure()
+    * The_`nester_log`_module
     * Supported_Languages
    Nester
+    * Developer_Docs
     * The Utils module
     * View_page_source
 ===============================================================================
 ****** The Utils moduleï ******
 The utils module is the summary of all functionality needed by Nester.
 We are planning to modularize and clean it up in the future.
 This module provides all functions necessary for Nesterâs three main
```

### Comparing `nester-struct-0.5.1/docs/_build/html/usage_guide.html` & `nester-struct-0.5.2/docs/_build/html/usage_guide.html`

 * *Files 10% similar despite different names*

```diff
@@ -45,22 +45,23 @@
               <p class="caption" role="heading"><span class="caption-text">Contents:</span></p>
 <ul class="current">
 <li class="toctree-l1"><a class="reference internal" href="installation_guide.html">Installation</a></li>
 <li class="toctree-l1 current"><a class="current reference internal" href="#">Usage</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="#cli-mode">CLI-Mode</a><ul>
 <li class="toctree-l3"><a class="reference internal" href="#nester-create">Nester create</a></li>
 <li class="toctree-l3"><a class="reference internal" href="#nester-validate">Nester validate</a></li>
-<li class="toctree-l3"><a class="reference internal" href="#nester-list">Nester list</a></li>
+<li class="toctree-l3"><a class="reference internal" href="#nester-log">Nester log</a></li>
 <li class="toctree-l3"><a class="reference internal" href="#nester-clean">Nester clean</a></li>
 </ul>
 </li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="dev_docs.html">Developer Docs</a></li>
 <li class="toctree-l1"><a class="reference internal" href="source/utils.html">   The `utils` module</a></li>
+<li class="toctree-l1"><a class="reference internal" href="source/logging.html">   The `nester_log` module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="supported_languages.html">Supported Languages</a></li>
 </ul>
 
         </div>
       </div>
     </nav>
 
@@ -94,15 +95,15 @@
 Nester has four main functions it can perform:</p>
 <ul class="simple">
 <li><p><cite>create</cite></p></li>
 <li><p><cite>validate</cite></p></li>
 <li><p><cite>list</cite></p></li>
 <li><p><cite>clean</cite></p></li>
 </ul>
-<p>Let us look into each three in more detail…</p>
+<p>Let us look into each of the four commands in more detail…</p>
 <section id="nester-create">
 <h3>Nester create<a class="headerlink" href="#nester-create" title="Permalink to this heading"></a></h3>
 <dl class="py function">
 <dt class="sig sig-object py">
 <span class="sig-name descname"><span class="pre">nester</span> <span class="pre">create(language,</span> <span class="pre">projectname,</span> <span class="pre">[-g|--git])</span></span></dt>
 <dd><p>Creates the project structure for the given project.
 If you are already in a directory which matches the name of the given project, the source files will be created in your current directory.
@@ -146,22 +147,21 @@
 <dt class="field-odd">Return type<span class="colon">:</span></dt>
 <dd class="field-odd"><p>str</p>
 </dd>
 </dl>
 </dd></dl>
 
 </section>
-<section id="nester-list">
-<h3>Nester list<a class="headerlink" href="#nester-list" title="Permalink to this heading"></a></h3>
+<section id="nester-log">
+<h3>Nester log<a class="headerlink" href="#nester-log" title="Permalink to this heading"></a></h3>
 <dl class="py function">
 <dt class="sig sig-object py">
-<span class="sig-name descname"><span class="pre">nester</span> <span class="pre">list()</span></span></dt>
-<dt class="sig sig-object py">
-<span class="sig-name descname"><span class="pre">Lists</span> <span class="pre">all</span> <span class="pre">previously</span> <span class="pre">created</span> <span class="pre">projects,</span> <span class="pre">which</span> <span class="pre">had</span> <span class="pre">logging</span> <span class="pre">enabled,</span> <span class="pre">in</span> <span class="pre">a</span> <span class="pre">table.</span></span></dt>
-<dd><dl class="field-list simple">
+<span class="sig-name descname"><span class="pre">nester</span> <span class="pre">log()</span></span></dt>
+<dd><p>Lists all previously created projects, which had logging enabled, in a table.</p>
+<dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><strong>--clean</strong> (<em>flag</em>) – An optional flag to clean up orphaned log entries.</p>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>None</p>
 </dd>
 <dt class="field-odd">Return type<span class="colon">:</span></dt>
```

#### html2text {}

```diff
@@ -10,18 +10,19 @@
 [q                   ]
 Contents:
     * Installation
     * Usage
           o CLI-Mode
                 # Nester_create
                 # Nester_validate
-                # Nester_list
+                # Nester_log
                 # Nester_clean
     * Developer_Docs
     * The_`utils`_module
+    * The_`nester_log`_module
     * Supported_Languages
    Nester
     * Usage
     * View_page_source
 ===============================================================================
 ****** Usageï ******
 Nester strives to be as easy to use as possible.
@@ -29,15 +30,15 @@
 ***** CLI-Modeï *****
 This is how Nester was intended to be used: As a small CLI-tool. Nester has
 four main functions it can perform:
     * create
     * validate
     * list
     * clean
-Let us look into each three in more detailâ¦
+Let us look into each of the four commands in more detailâ¦
 **** Nester createï ****
   nester create(language, projectname, [-g|--git])
       Creates the project structure for the given project. If you are already
       in a directory which matches the name of the given project, the source
       files will be created in your current directory. If not Nester will
       automatically create a directory for your project.
         Parameters:
@@ -70,17 +71,18 @@
                 * projectname (str) â The name of the project or package you
                   want to validate
         Returns:
             Tells you via Terminal wether your structure lines up or not.
         Return type:
             str
 
-**** Nester listï ****
-  nester list()
-  Lists all previously created projects, which had logging enabled, in a table.
+**** Nester logï ****
+  nester log()
+      Lists all previously created projects, which had logging enabled, in a
+      table.
         Parameters:
             --clean (flag) â An optional flag to clean up orphaned log
             entries.
         Returns:
             None
         Return type:
             None
```

### Comparing `nester-struct-0.5.1/docs/_static/css/custom.css` & `nester-struct-0.5.2/docs/_static/css/custom.css`

 * *Files 0% similar despite different names*

```diff
@@ -67,11 +67,11 @@
 html.writer-html5 body.wy-body-for-nav div.wy-grid-for-nav nav.wy-nav-side div.wy-side-scroll div.wy-menu.wy-menu-vertical ul.current li.toctree-l1.current ul li.toctree-l2 a.reference.internal,
 html.writer-html5 body.wy-body-for-nav div.wy-grid-for-nav nav.wy-nav-side div.wy-side-scroll div.wy-menu.wy-menu-vertical ul.current li.toctree-l1.current a.current.reference.internal {
   background-color: #111;
 }
 
 /*Change background color of rendered code in toc on index.rst*/
 html.writer-html5 body.wy-body-for-nav div.wy-grid-for-nav section.wy-nav-content-wrap div.wy-nav-content div.rst-content div.document div section#welcome-to-nester-s-documentation div.toctree-wrapper.compound ul li.toctree-l1 ul li.toctree-l2 a.reference.internal code.docutils.literal.notranslate {
-  background-color: #222;
+  background-color: #ffff;
   color: #ff5100;
   border-style: hidden;
 }
```

### Comparing `nester-struct-0.5.1/docs/_static/index_logo.png` & `nester-struct-0.5.2/docs/_static/index_logo.png`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/docs/conf.py` & `nester-struct-0.5.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/docs/index.rst` & `nester-struct-0.5.2/docs/index.rst`

 * *Files 24% similar despite different names*

```diff
@@ -12,14 +12,15 @@
    :maxdepth: 2
    :caption: Contents:
 
    Installation <installation_guide>
    Usage <usage_guide>
    Developer Docs <dev_docs>
       The `utils` module <source/utils>
+      The `nester_log` module <source/logging>
    Supported Languages <supported_languages>
 
 
 
 Indices and tables
 ==================
```

### Comparing `nester-struct-0.5.1/docs/supported_languages.rst` & `nester-struct-0.5.2/docs/supported_languages.rst`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/docs/usage_guide.rst` & `nester-struct-0.5.2/docs/usage_guide.rst`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/img/logo_social_preview.png` & `nester-struct-0.5.2/img/logo_social_preview.png`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/img/logo_thumbnail.png` & `nester-struct-0.5.2/img/logo_thumbnail.png`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/index_logo.png` & `nester-struct-0.5.2/index_logo.png`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/pyproject.toml` & `nester-struct-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/setup.cfg` & `nester-struct-0.5.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/src/nester/nester_commands.py` & `nester-struct-0.5.2/src/nester/nester_commands.py`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/src/nester/nester_log.py` & `nester-struct-0.5.2/src/nester/nester_log.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-This module handles Nester's logging functionality. Nester logs all projects created with it unless the --no-log flag ist set when calling nester create
+This module handles Nester's logging functionality. Nester logs all projects created with it unless the --no-log flag ist set when calling nester create.
 """
 
 import logging
 import re
 from pathlib import Path
 
 
@@ -33,14 +33,17 @@
 LOGGER = logging.getLogger("nester")
 LOGGER.setLevel(logging.INFO)
 
 
 def create_log_file_if_none():
     """
     Create '.nester.log' file if it does not exist already.
+
+    :param: None
+    :return: None
     """
     formatter = ProjectLogFormatter(
         "%(asctime)s - %(name)s - %(levelname)s - Project: %(projectname)s - Language: %(programming_language)s - Location: %(location)s"
     )
     file_handler = logging.FileHandler(_LOG_FILE_PATH)
     file_handler.setFormatter(formatter)
     LOGGER.addHandler(file_handler)
@@ -49,15 +52,15 @@
 def check_log_for_duplicate(projectname):
     """
     Check the nester.log file in the home directory, whether a given projectname has been taken already.
     If no log file exists: Continue with the program.
 
     :param projectname: Name of the project to be checked
     :return: True/False depending on whether an entry has been found.
-    :rtype: Bool
+    :rtype: bool
     """
     try:
         with _LOG_FILE_PATH.open("r", encoding="utf-8") as log_file:
             log = log_file.readlines()
     except FileNotFoundError:
         print(f"\033[34mLog file not found. Moving on ...\033[0m")
         return False
@@ -70,14 +73,17 @@
 
 
 def remove_log_entry(projectname, verbose=True):
     """
     Check if the given project appears in the log. If it does, remove the entry from the log.
 
     :param projectname: The name of the project to be removed.
+    :type projectname: str
+    :param verbose: Flag whether or not to suppress print statements. Needed for clean function.
+    :type verbose: bool
     :return: None
     """
     try:
         with _LOG_FILE_PATH.open("r", encoding="utf-8") as log_file:
             log = log_file.readlines()
     except FileNotFoundError:
         print("\033[34mNo log file found! Moving on ...\033[0m")
@@ -111,14 +117,17 @@
         print(f"\033[34mNo log entry found for '{projectname}'\033[0m")
 
 
 def clean_orphaned_entries():
     """
     Check all projects listed in the log and see whether their paths are still valid.
     If not remove the entry.
+
+    :param: None
+    :return: None
     """
     items_removed = 0
 
     try:
         with open(_LOG_FILE_PATH, "r", encoding="utf-8") as log_file:
             for line in log_file:
                 project_name = re.search(r"[-\s]+Project:\s+(.*?)\s+-", line).group(1)
@@ -140,14 +149,17 @@
             "\033[31mError: No log file found. Run 'nester create' to get started!\033[0m"
         )
 
 
 def print_log_to_table():
     """
     Read the log file and print its contents into a table.
+
+    :param: None
+    :return: None
     """
     try:
         # Check if logfile exists
         if not _LOG_FILE_PATH.exists():
             print(
                 "\033[031mError: Log file could not be found.\033[0m\nThis could happen because you have not created a single project yet. Try `nester create` to get started!"
             )
```

### Comparing `nester-struct-0.5.1/src/nester/templates/c/c_layout.json` & `nester-struct-0.5.2/src/nester/templates/c/c_layout.json`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/src/nester/templates/cpp/cpp_layout.json` & `nester-struct-0.5.2/src/nester/templates/cpp/cpp_layout.json`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/src/nester/templates/java/java_layout.json` & `nester-struct-0.5.2/src/nester/templates/java/java_layout.json`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/src/nester/utils.py` & `nester-struct-0.5.2/src/nester/utils.py`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/src/nester_struct.egg-info/PKG-INFO` & `nester-struct-0.5.2/src/nester_struct.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nester-struct
-Version: 0.5.1
+Version: 0.5.2
 Summary: Automated creation of project structure
 Home-page: https://github.com/ByteOtter/nester
 Author: Christopher Hock
 Author-email: christopher-hock@protonmail.com
 License: GPLv3.0
 Keywords: automation,project_structure,python
 Classifier: Natural Language :: English
@@ -43,15 +43,15 @@
 A small command line tool to set up the basic structure for your Python, C#, C++, Java or Ruby project.
 
 **Index**
 - [Introduction](#introduction)
 - [Our Goal](#our-goal)
 - [Installation](#installation)
   - [Get it on PyPi!](#get-it-on-pypi)
-  - [Get it as an `.rpm` package](#get-it-as-an-rpm-package)
+  - [Get it as an `.rpm` package (wip)](#get-it-as-an-rpm-package-wip)
   - [Build it from source](#build-it-from-source)
 - [Usage](#usage)
   - [CLI Mode](#cli-mode)
   - [Interactive / GUI - Mode (coming soon)](#interactive--gui---mode-coming-soon)
   - [Supported Languages](#supported-languages)
 - [Documentation](#documentation)
     - [Read the Docs (wip)](#read-the-docs-wip)
@@ -76,28 +76,44 @@
 
 Nester, by default, also logs all projects you create with it which allows you to easily view and clean up your projects and avoid creating duplicate projects. Never loose your overview over your projects again!
 
 ## Installation
 
 ### Get it on PyPi!
 
-`Nester` is finally released on [PyPi](https://pypi.org)!<br>
+`Nester` is released on [PyPi](https://pypi.org)!<br>
 To do so, make sure you have at least `Python 3.10` and `pip` installed.<br>
 To get `Nester` simply run:
 
 ```bash
 pip install nester-struct
 ```
 Your done! Have fun with `Nester`!
 
-### Get it as an `.rpm` package
+### Get it as an `.rpm` package (wip)
 
-We plan to release Nester to pypi first and as an `.rpm` package in the future.
+We can now offer a `.rpm` package!
 
-TBA
+To do so follow these steps (on openSUSE):
+
+1. Add the repository
+```bash
+sudo zypper addrepo https://download.opensuse.org/repositories/home:kodymo/openSUSE_Tumbleweed/home:kodymo.repo
+```
+2. Refresh your repositories
+```bash
+sudo zypper ref
+```
+3. Install Nester
+```bash
+sudo zypper install python3-nester
+```
+Note: The repository contains three builds for nester for Python 3.9, 3.10 and 3.11. `zypper` will automatically decide which version to use when running the command above.
+
+You can visit the repository on the [package maintainer's OBS account](https://build.opensuse.org/package/show/home:kodymo/python-nester).
 
 ### Build it from source
 
 If you want to contribute to `Nester` or just prefer building it yoursef, refer to the [Contributing Guide](docs/CONTRIBUTING.md) to find out how.
 
 
 ## Usage
@@ -113,15 +129,15 @@
 nester <OPERATION> <OPTIONAL -git FLAG> <LANGUAGE> <PROJECT_NAME>
 ```
 The following operations will be available:
 |`Operation`|Flags|Argument|Argument|Effect|
 |-|-|-|-|-|
 |`create`|`-g/--git`, `--no-log`|`Language`|`Projectname`|Creates the project structure for the selected lanugage in *the current directory*. IF `-git` is set it will also call `git init` in this directory. `--no-log` Will prevent Nester from creating a log entry for this project. You can find the log in your home directory at `~/nester.log`|
 |`validate`|n/A|`Language`|`Projectname`|Checks the current directory and its sub-directories if it corresponds to the schema provided for the language|
-|`log`|n/A|n/A|n/A|Prints out all *logged* projects that have been created previously|
+|`log`|`--clean`|n/A|n/A|Prints out all *logged* projects that have been created previously<br>If the `--clean` flag is set, orphaned log entries (projects which had their directory deleted) will be purged from the log|
 |`clean`|`-y/--yes`|`Projectname`|n/A|Deletes the content of the specified project|
 
 ### Interactive / GUI - Mode (coming soon)
 
 This is considered to be the fallback mode. If **Nester** is called without any arguments you will be asked to enter all parameters manually.
 
 The parameters themselves will stay the same though.
@@ -149,15 +165,15 @@
 
 ## Documentation
 
 Good documentation is very important to us, even with such a small project like Nester. To this end we have two methods in place to build documentation for us:
 
 #### Read the Docs (wip)
 
-On our [Read the Docs](https://nester.readthedocs.io/en/latest/index.html#) we build the general documentation for the project. You can find the installation and usage guides there, aswell as an overview over the languages we support or want to support.
+On our [Read the Docs](https://nester.readthedocs.io/en/latest/index.html#) we build the documentation for the project. You can find the installation and usage guides there, aswell as an overview over the languages we support or want to support.
 
 Also there is the automatically build documentation of functions and modules that make Nester go.
 
 #### Towncrier (wip)
 
 Towncrier is used to build changelogs for us. It is required that Pull Requests, which change Nesters behaviour, include a changelog file.
```

### Comparing `nester-struct-0.5.1/src/nester_struct.egg-info/SOURCES.txt` & `nester-struct-0.5.2/src/nester_struct.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -27,43 +27,49 @@
 .github/workflows/towncrier.yml
 changelog/.gitkeep
 changelog.d/30.added
 changelog.d/34.added
 changelog.d/changelog_template.jinja
 docs/Makefile
 docs/conf.py
+docs/contributing.rst
 docs/dev_docs.rst
 docs/index.rst
 docs/installation_guide.rst
 docs/requirements.txt
 docs/supported_languages.rst
 docs/usage_guide.rst
 docs/_build/html/.buildinfo
+docs/_build/html/contributing.html
 docs/_build/html/dev_docs.html
 docs/_build/html/genindex.html
 docs/_build/html/index.html
 docs/_build/html/installation_guide.html
 docs/_build/html/objects.inv
 docs/_build/html/py-modindex.html
 docs/_build/html/search.html
 docs/_build/html/searchindex.js
 docs/_build/html/supported_languages.html
 docs/_build/html/usage_guide.html
+docs/_build/html/.doctrees/contributing.doctree
 docs/_build/html/.doctrees/dev_docs.doctree
 docs/_build/html/.doctrees/environment.pickle
 docs/_build/html/.doctrees/index.doctree
 docs/_build/html/.doctrees/installation_guide.doctree
 docs/_build/html/.doctrees/supported_languages.doctree
 docs/_build/html/.doctrees/usage_guide.doctree
+docs/_build/html/.doctrees/source/logging.doctree
 docs/_build/html/.doctrees/source/utils.doctree
+docs/_build/html/_sources/contributing.rst.txt
 docs/_build/html/_sources/dev_docs.rst.txt
 docs/_build/html/_sources/index.rst.txt
 docs/_build/html/_sources/installation_guide.rst.txt
 docs/_build/html/_sources/supported_languages.rst.txt
 docs/_build/html/_sources/usage_guide.rst.txt
+docs/_build/html/_sources/source/logging.rst.txt
 docs/_build/html/_sources/source/utils.rst.txt
 docs/_build/html/_static/basic.css
 docs/_build/html/_static/doctools.js
 docs/_build/html/_static/documentation_options.js
 docs/_build/html/_static/file.png
 docs/_build/html/_static/index_logo.png
 docs/_build/html/_static/language_data.js
@@ -92,17 +98,19 @@
 docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
 docs/_build/html/_static/css/fonts/lato-normal.woff
 docs/_build/html/_static/css/fonts/lato-normal.woff2
 docs/_build/html/_static/js/badge_only.js
 docs/_build/html/_static/js/html5shiv-printshiv.min.js
 docs/_build/html/_static/js/html5shiv.min.js
 docs/_build/html/_static/js/theme.js
+docs/_build/html/source/logging.html
 docs/_build/html/source/utils.html
 docs/_static/index_logo.png
 docs/_static/css/custom.css
+docs/source/logging.rst
 docs/source/utils.rst
 img/logo_social_preview.png
 img/logo_thumbnail.png
 src/nester/__init__.py
 src/nester/nester_commands.py
 src/nester/nester_log.py
 src/nester/utils.py
```

### Comparing `nester-struct-0.5.1/tests/interation_tests/test_util_integration.py` & `nester-struct-0.5.2/tests/interation_tests/test_util_integration.py`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/tests/unit_tests/test_logging.py` & `nester-struct-0.5.2/tests/unit_tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.1/tests/unit_tests/test_utils.py` & `nester-struct-0.5.2/tests/unit_tests/test_utils.py`

 * *Files identical despite different names*

