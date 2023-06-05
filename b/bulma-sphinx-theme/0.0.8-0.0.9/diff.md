# Comparing `tmp/bulma_sphinx_theme-0.0.8.tar.gz` & `tmp/bulma_sphinx_theme-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bulma_sphinx_theme-0.0.8.tar", last modified: Fri Jun  2 03:42:54 2023, max compression
+gzip compressed data, was "bulma_sphinx_theme-0.0.9.tar", last modified: Mon Jun  5 15:13:36 2023, max compression
```

## Comparing `bulma_sphinx_theme-0.0.8.tar` & `bulma_sphinx_theme-0.0.9.tar`

### file list

```diff
@@ -1,200 +1,203 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:54.791115 bulma_sphinx_theme-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-02 03:42:37.599041 bulma_sphinx_theme-0.0.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-02 03:42:37.599041 bulma_sphinx_theme-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-02 03:42:37.599041 bulma_sphinx_theme-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-02 03:42:37.599041 bulma_sphinx_theme-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.599041 bulma_sphinx_theme-0.0.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-06-02 03:42:37.599041 bulma_sphinx_theme-0.0.8/docs/_static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-02 03:42:37.599041 bulma_sphinx_theme-0.0.8/docs/_static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-06-02 03:42:37.599041 bulma_sphinx_theme-0.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-02 03:42:37.599041 bulma_sphinx_theme-0.0.8/docs/develop.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-02 03:42:37.599041 bulma_sphinx_theme-0.0.8/docs/examples/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-02 03:42:37.599041 bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/admonitions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-02 03:42:37.599041 bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-06-02 03:42:37.599041 bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/blocks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-06-02 03:42:37.599041 bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/generic.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/images.rst
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/lists.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/really-long.md
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/sphinx-design.md
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/tables.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/typography.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/mult_headers.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/reference/admonitions.md
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/reference/api.md
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/reference/code-blocks.md
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/reference/hyperlinks.md
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/reference/images.md
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/reference/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/reference/lists.md
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/reference/tables.md
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/reference/tabs.md
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/reference/text-formatting.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/subpages/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/subpages/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/subpages/subpage1.rst
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/subpages/subpage2.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/subpages/subsubpages/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/subpages/subsubpages/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/subpages/subsubpages/subsubpage1.rst
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/subpages/subsubpages/subsubpage2.rst
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/subpages/subsubpages/subsubpage3.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/subpages/subsubpages/subsubsubpages/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/examples/subpages/subsubpages/subsubsubpages/subsubsubpage1.rst
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/user_guide/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/user_guide/navbar.md
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/user_guide/sidenav.md
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/user_guide/source-buttons.md
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/docs/web-components.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)   130410 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/package.json
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/postcss.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/
--rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js
--rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/abstracts/
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/abstracts/_mixins.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/base/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/base/_icons.scss
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/base/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/base/_typography.scss
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/bulma-sphinx-theme.sass
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_article-bottom.scss
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_article-top.scss
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_brand-logo.scss
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_breadcrumbs.scss
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_edit-page.scss
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_info-panel.scss
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_last-updated.scss
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_search-button.scss
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_search-field.sass
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_search-icon.scss
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_search-results.scss
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_search-wrapper.scss
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_search.sass
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_sidenav-brand.scss
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_switcher-theme.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/
--rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_admonitions.scss
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_api.scss
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_blocks.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_code.scss
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_footnotes.sass
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_gui-labels.scss
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_images.sass
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_indexes.sass
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_lists.scss
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_math.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_misc.sass
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_rubrics.sass
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_sidebar.sass
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_tables.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_target.sass
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/extensions/_ablog.scss
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/extensions/_bulma.scss
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/extensions/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/extensions/_leaflet.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/extensions/_notebooks.scss
--rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/extensions/_sphinx-design.scss
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/extensions/_togglebutton.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/sections/_bulma-content.scss
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/sections/_bulma-main.scss
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/sections/_bulma-sidenav.scss
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/sections/_footer.scss
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/sections/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/sections/_navbar.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/variables/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/variables/_admonitions.scss
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/variables/_color.scss
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/variables/_definition.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/variables/_fonts.scss
--rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/variables/_icons.scss
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/variables/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-02 03:42:37.603041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/variables/_layout.scss
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/variables/_spacing.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/translations/
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/translations/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/translations/jsons/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/translations/jsons/Back to top.json
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/translations/jsons/last update.json
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/translations/jsons/with.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/demo/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/demo/sphinxext.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/pygment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/back-to-top.html
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/brand-logo.html
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/copyright.html
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/header-icons.html
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/info-panel.html
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/last-updated.html
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/navbar-nav.html
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-button.html
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-field.html
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-icon.html
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-wrapper.html
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/searchbox.html
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sidenav-nav.html
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sourcelink.html
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sphinx-version.html
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/theme-swither.html
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/globaltoc.html
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/localtoc.html
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/page.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_css_variables_define.html
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html
--rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/icons.html
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/headnav.html
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/sidenav.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/theme.conf
--rw-r--r--   0 runner    (1001) docker     (123)    17845 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/toctree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/translations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-02 03:42:37.607041 bulma_sphinx_theme-0.0.8/webpack.config.js
--rw-r--r--   0        0        0     4297 1970-01-01 00:00:00.000000 bulma_sphinx_theme-0.0.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:36.541664 bulma_sphinx_theme-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/_static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/_static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/admonitions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/blocks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/generic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/images.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/lists.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/really-long.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/sphinx-design.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/tables.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/typography.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/mult_headers.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/reference/admonitions.md
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/reference/api.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/reference/code-blocks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/reference/hyperlinks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/reference/images.md
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/reference/lists.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/reference/tables.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/reference/tabs.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/reference/text-formatting.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/subpages/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/subpages/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/subpages/subpage1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/subpages/subpage2.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/subpages/subsubpages/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/subpages/subsubpages/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/subpages/subsubpages/subsubpage1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/subpages/subsubpages/subsubpage2.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/subpages/subsubpages/subsubpage3.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/subpages/subsubpages/subsubsubpages/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/subpages/subsubpages/subsubsubpages/subsubsubpage1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/user_guide/develop.md
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/user_guide/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/user_guide/navbar.md
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/user_guide/search.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/user_guide/sidenav.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/user_guide/source.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/user_guide/theme-elements.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/user_guide/web-components.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130410 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/postcss.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.633455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    11169 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/abstracts/_mixins.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/base/_icons.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/base/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/base/_typography.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/bulma-sphinx-theme.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_article-bottom.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_article-top.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_brand-logo.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_breadcrumbs.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_edit-page.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_info-panel.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_last-updated.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_search-button.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_search-field.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_search-icon.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_search-results.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_search-wrapper.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_search.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_sidenav-brand.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_switcher-theme.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/
+-rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_admonitions.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_api.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_blocks.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_code.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_footnotes.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_gui-labels.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_images.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_indexes.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_lists.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_math.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_misc.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_rubrics.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_sidebar.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_tables.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_target.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/extensions/_ablog.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/extensions/_bulma.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/extensions/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/extensions/_leaflet.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/extensions/_notebooks.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/extensions/_sphinx-design.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/extensions/_togglebutton.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/sections/_bulma-content.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/sections/_bulma-main.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/sections/_bulma-sidenav.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/sections/_footer.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/sections/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/sections/_navbar.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/variables/_admonitions.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/variables/_color.scss
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/variables/_definition.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/variables/_fonts.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/variables/_icons.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/variables/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/variables/_layout.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/variables/_spacing.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/translations/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/translations/jsons/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/translations/jsons/Back to top.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/translations/jsons/last update.json
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/translations/jsons/with.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/demo/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/demo/sphinxext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/pygment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.633455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/back-to-top.html
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/brand-logo.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/copyright.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/icon-links.html
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/info-panel.html
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/last-updated.html
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/navbar-nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-button.html
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-field.html
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-icon.html
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-wrapper.html
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/searchbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sidenav-nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sourcelink.html
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sphinx-version.html
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/theme-swither.html
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/toggle-sidenav.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/globaltoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/localtoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/page.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_css_variables_define.html
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-06-05 15:13:19.633455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/icons.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-05 15:13:19.633455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.633455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-05 15:13:19.633455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-05 15:13:19.633455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-05 15:13:19.633455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-05 15:13:19.633455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/headnav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-05 15:13:19.633455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/sidenav.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.633455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-05 15:13:19.633455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-05 15:13:19.633455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (123)    17845 2023-06-05 15:13:19.633455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/toctree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-06-05 15:13:19.633455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-06-05 15:13:19.633455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/translations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-05 15:13:19.633455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-05 15:13:19.633455 bulma_sphinx_theme-0.0.9/webpack.config.js
+-rw-r--r--   0        0        0     4450 1970-01-01 00:00:00.000000 bulma_sphinx_theme-0.0.9/PKG-INFO
```

### Comparing `bulma_sphinx_theme-0.0.8/LICENSE` & `bulma_sphinx_theme-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/README.md` & `bulma_sphinx_theme-0.0.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -35,10 +35,16 @@
 html_theme = "bulma_sphinx_theme"
 ```
 
 Your Sphinx documentation's HTML pages will now be generated with this theme! 🎉
 
 <!-- end quickstart -->
 
+## Examples
+
+An examples without fixed navbar: <https://zclab.github.io/bst-demo/>
+
+An examples without navbar: <https://zclab.github.io/bst-nonavbar/>
+
 ## Documentation
 
 See [the bulma sphinx theme](https://bulma-sphinx-theme.readthedocs.io/en/latest/) for more information. Your can also refer to [Bulma Documentation](https://bulma.io/) for more sophisticated change.
```

#### html2text {}

```diff
@@ -13,11 +13,14 @@
 /github.com/zclab/bulma-sphinx-theme/blob/main/LICENSE) [![Github Stars](https:
 //img.shields.io/github/stars/zclab/bulma-sphinx-theme?style=flat-
 square&logo=github)](https://github.com/zclab/bulma-sphinx-theme)  ## Get
 started  To use this theme in your documentation build environment, first
 install the `bulma-sphinx-theme` with `pip`: ``` pip install bulma-sphinx-theme
 ``` then, configure the Sphinx docs to use the theme by editing `conf.py`
 ```python html_theme = "bulma_sphinx_theme" ``` Your Sphinx documentation's
-HTML pages will now be generated with this theme! ð  ## Documentation See
-[the bulma sphinx theme](https://bulma-sphinx-theme.readthedocs.io/en/latest/
-) for more information. Your can also refer to [Bulma Documentation](https://
-bulma.io/) for more sophisticated change.
+HTML pages will now be generated with this theme! ð  ## Examples An examples
+without fixed navbar:
+zclab.github.io/bst-demo/> An examples without navbar:
+zclab.github.io/bst-nonavbar/> ## Documentation See [the bulma sphinx theme]
+(https://bulma-sphinx-theme.readthedocs.io/en/latest/) for more information.
+Your can also refer to [Bulma Documentation](https://bulma.io/) for more
+sophisticated change.
```

### Comparing `bulma_sphinx_theme-0.0.8/docs/_static/favicon.png` & `bulma_sphinx_theme-0.0.9/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/docs/_static/logo.svg` & `bulma_sphinx_theme-0.0.9/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/docs/conf.py` & `bulma_sphinx_theme-0.0.9/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,32 +60,32 @@
 # https://github.com/hung1001/font-awesome-pro-v6
 # html_css_files = [
 #     "https://cdn.jsdelivr.net/gh/duyplus/fontawesome-pro/css/all.min.css",
 # ]
 # fontawesome_included = True
 
 html_theme_options = {
-    "header_links_before_dropdown": 5,
+    "header_links_before_dropdown": 3,
     "navbar_color_style": "is-white",  # see styles: https://bulma.io/documentation/components/navbar/#colors
     "logo": {"text": "Bulma Sphinx Theme", "logo": "_static/logo.svg"},
-    "header_icons": [
+    "icon_links": [
         {
             "name": "Github",
             "url": "https://github.com/zclab/bulma-sphinx-theme",
             "svg": "github",
         },
         {
             "name": "Pypi",
             "url": "https://pypi.org/project/bulma-sphinx-theme/",
             "svg": "package",
         },
         {
             "name": "Bulma",
             "url": "https://bulma.io/",
-            "svg": "bulma",
+            "image": "https://bulma.io/assets/Bulma%20Icon.svg",
         },
     ],
     "external_links": [
         {
             "name": "Pydata",
             "url": "https://pydata-sphinx-theme.readthedocs.io/en/latest/",
         },
@@ -104,21 +104,15 @@
         },
     ],
     "source_repository": "https://github.com/zclab/bulma-sphinx-theme",
     "source_branch": "main",
     "source_directory": "docs/",
     "use_edit_page_button": True,
     "fix_navbar": True,
-    "information_panel": [],
-    "navbar_start": [],
-    "navbar_end": ["navbar-nav.html", "theme-swither.html", "header-icons.html"],
     "have_top_navbar": True,
-    "light_colors": {
-        "bst-color-background-sidenav": "rgb(240, 248, 255)",
-    },
 }
 
 html_context = {"default_mode": "auto"}
 
 # blog_path = "blog"
 # blog_post_pattern = "posts/*/*"
 # blog_authors = {
```

### Comparing `bulma_sphinx_theme-0.0.8/docs/develop.md` & `bulma_sphinx_theme-0.0.9/docs/user_guide/develop.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/docs/examples/index.md` & `bulma_sphinx_theme-0.0.9/docs/examples/index.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/admonitions.rst` & `bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/admonitions.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/api.rst` & `bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/api.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/blocks.rst` & `bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/blocks.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/generic.rst` & `bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/generic.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/images.rst` & `bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/images.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/index.md` & `bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/index.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/lists.rst` & `bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/lists.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/really-long.md` & `bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/really-long.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/sphinx-design.md` & `bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/sphinx-design.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/structure.rst` & `bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/structure.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/tables.rst` & `bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/tables.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/docs/examples/kitchen-sink/typography.rst` & `bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/typography.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/docs/examples/mult_headers.rst` & `bulma_sphinx_theme-0.0.9/docs/examples/mult_headers.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/docs/examples/reference/admonitions.md` & `bulma_sphinx_theme-0.0.9/docs/examples/reference/admonitions.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/docs/examples/reference/api.md` & `bulma_sphinx_theme-0.0.9/docs/examples/reference/api.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/docs/examples/reference/code-blocks.md` & `bulma_sphinx_theme-0.0.9/docs/examples/reference/code-blocks.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/docs/examples/reference/hyperlinks.md` & `bulma_sphinx_theme-0.0.9/docs/examples/reference/hyperlinks.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/docs/examples/reference/images.md` & `bulma_sphinx_theme-0.0.9/docs/examples/reference/images.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/docs/examples/reference/index.md` & `bulma_sphinx_theme-0.0.9/docs/examples/reference/index.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/docs/examples/reference/lists.md` & `bulma_sphinx_theme-0.0.9/docs/examples/reference/lists.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/docs/examples/reference/tables.md` & `bulma_sphinx_theme-0.0.9/docs/examples/reference/tables.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/docs/examples/reference/tabs.md` & `bulma_sphinx_theme-0.0.9/docs/examples/reference/tabs.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/docs/examples/reference/text-formatting.md` & `bulma_sphinx_theme-0.0.9/docs/examples/reference/text-formatting.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/docs/examples/subpages/subpage1.rst` & `bulma_sphinx_theme-0.0.9/docs/examples/subpages/subpage1.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/docs/examples/subpages/subpage2.rst` & `bulma_sphinx_theme-0.0.9/docs/examples/subpages/subpage2.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/docs/examples/subpages/subsubpages/subsubpage1.rst` & `bulma_sphinx_theme-0.0.9/docs/examples/subpages/subsubpages/subsubpage1.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/docs/examples/subpages/subsubpages/subsubpage2.rst` & `bulma_sphinx_theme-0.0.9/docs/examples/subpages/subsubpages/subsubpage2.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/docs/examples/subpages/subsubpages/subsubpage3.rst` & `bulma_sphinx_theme-0.0.9/docs/examples/subpages/subsubpages/subsubpage3.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/docs/user_guide/navbar.md` & `bulma_sphinx_theme-0.0.9/docs/user_guide/navbar.md`

 * *Files 4% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 ```{note}
 When you disable navbar, fix navbar will not work even you set `fix_navbar` to `True`.
 ```
 
 ## Changing header icons
 
-Bulma sphinx theme allows customising the icons that are presented in the header. These icons can be used to link to relevant resources for your project and documentation. To add custom header icons, you need to provide the `header_icons` configuration value as follows,
+Bulma sphinx theme allows customising the icons that are presented in the header. These icons can be used to link to relevant resources for your project and documentation. To add custom header icons, you need to provide the `icon_links` configuration value as follows,
 
 ```python
 html_theme_options = {
-    "header_icons": [
+    "icon_links": [
         {"name":"Gitlab", "url": "http://gitlabcom/zclab/bulma-sphinx-theme", "fontawesome":"fa-brands fa-lg fa-gitlab"},
     ],
 }
 ```
 
 ````{note}
 If you wish to use Font Awesome icons, Using `html_css_files` to add the CSS file(s) for Font Awesome.
```

### Comparing `bulma_sphinx_theme-0.0.8/docs/user_guide/source-buttons.md` & `bulma_sphinx_theme-0.0.9/docs/user_guide/source.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/docs/web-components.rst` & `bulma_sphinx_theme-0.0.9/docs/user_guide/web-components.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/noxfile.py` & `bulma_sphinx_theme-0.0.9/noxfile.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/package-lock.json` & `bulma_sphinx_theme-0.0.9/package-lock.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/package.json` & `bulma_sphinx_theme-0.0.9/package.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/pyproject.toml` & `bulma_sphinx_theme-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/__init__.py` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from functools import lru_cache
 from pathlib import Path
 from typing import Any, Dict, List
 from sphinx.builders.html import StandaloneHTMLBuilder
 from sphinx.locale import get_translation
 from . import pygment, toctree, transforms, utils
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 logger = logging.getLogger(__name__)
 MESSAGE_CATALOG_NAME = "bulmasphinxtheme"
 
 
 def _get_html_theme_path():
     """Return list of HTML theme paths."""
     parent = Path(__file__).parent.resolve()
@@ -68,14 +68,26 @@
 def _builder_inited(app: sphinx.application.Sphinx) -> None:
     theme_options = utils.get_theme_options(app)
 
     have_navbar = theme_options.get("have_top_navbar", True)
     if not (have_navbar):
         theme_options["fix_navbar"] = False
 
+    info_include_directly = theme_options.get(
+        "information_panel_include_directly", None
+    )
+    if info_include_directly and isinstance(info_include_directly, list):
+        theme_options["information_panel_include_directly"].extend(
+            info_include_directly
+        )
+
+    navbar_include_directly = theme_options.get("navbar_include_directly", None)
+    if navbar_include_directly and isinstance(navbar_include_directly, list):
+        theme_options["navbar_include_directly"].extend(navbar_include_directly)
+
     # Add an analytics ID to the site if provided
     analytics = theme_options.get("analytics", {})
     if analytics:
         # Google Analytics
         gid = analytics.get("google_analytics_id")
 
         if gid:
@@ -107,14 +119,15 @@
         "theme_article_top_right",
         "theme_article_bottom_left",
         "theme_article_bottom_right",
         "theme_navbar_start",
         "theme_navbar_end",
         "theme_navbar_include_directly",
         "theme_information_panel",
+        "theme_information_panel_include_directly",
         "sidebars",
     ]
 
     for section in template_sections:
         if context.get(section):
             # Break apart `,` separated strings so we can use , in the defaults
             if isinstance(context.get(section), str):
```

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -180,15 +180,15 @@
         recursive: true,
         navClass: "scroll-current",
         nested: true,
         nestedClass: "scroll-current", //
         events: true,
         offset: () => {
             let rem = parseFloat(getComputedStyle(document.documentElement).fontSize);
-            return header.getBoundingClientRect().height + 1.0 * rem + 1;
+            return header.getBoundingClientRect().height + 4.5 * rem + 1;
         },
     });
 }
 
 function setup() {
     setupScrollHandler();
     addTOCInteractivity();
@@ -371,13 +371,13 @@
 ////////////////////////////////////////////////////////////////////////////////
 function main() {
     document.body.parentNode.classList.remove("no-js");
     addModeListener();
     setupSearchButtons();
     setupDropdwon();
     navbarBurger();
-    header = document.querySelector(".navbar");
+    header = document.querySelector("header");
     tocScroll = document.querySelector(".toc-scroll");
     setup();
 }
 
 document.addEventListener("DOMContentLoaded", main);
```

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/abstracts/_mixins.scss` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/abstracts/_mixins.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/base/_typography.scss` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/base/_typography.scss`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 optgroup,
 select,
 textarea {
   font-family: var(--font-stack);
 }
 
 code,
-pre {
+pre,
+kbd,
+samp {
   font-family: var(--font-stack--monospace);
 }
 
 pre {
   background-color: unset;
   color: var(--bst-color-text-base);
 }
```

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_search-wrapper.scss` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_search-wrapper.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/components/_switcher-theme.scss` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_switcher-theme.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_admonitions.scss` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_admonitions.scss`

 * *Files 1% similar despite different names*

```diff
@@ -247,15 +247,15 @@
     max-width: 40%;
     float: right;
     clear: both;
     margin-left: 0.5rem;
     margin-top: 0;
 
     // Undo the .sidebar directive border
-    border-width: 0 0 0 0.2rem;
+    // border-width: 0 0 0 0.2rem;
 
     // TODO: these semantic-color-names border-color rules might no longer be
     //       needed when we drop support for Sphinx 4 / docutils 0.17
     &.attention,
     &.important {
       border-color: var(--bst-color-attention);
     }
```

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_api.scss` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_api.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_code.scss` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_code.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_footnotes.sass` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_footnotes.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_images.sass` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_images.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_lists.scss` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_lists.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_misc.sass` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_misc.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_sidebar.sass` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_sidebar.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_tables.sass` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_tables.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/content/_target.sass` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_target.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/extensions/_ablog.scss` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/extensions/_ablog.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/extensions/_notebooks.scss` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/extensions/_notebooks.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/extensions/_sphinx-design.scss` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/extensions/_sphinx-design.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/sections/_bulma-sidenav.scss` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/sections/_bulma-sidenav.scss`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,37 @@
 .bulma-sidenav {
-  display: block;
+  display: none;
+
+  @include desktop {
+    display: block;
+  }
+
+  &.is-active {
+    @include touch {
+      display: block;
+      transform: translateX(100%);
+      width: 300px;
+      margin-left: -300px;
+      z-index: 2;
+    }
+  }
+
   clip-path: inset(0);
   background-color: var(--bst-color-background-sidenav);
   width: var(--sidenav-width);
-  border-right: 1px solid var(--bst-color-border);
   margin-top: calc(
     var(--navbar-height) * var(--sidenav-sticky-top-factor) * -1
   );
 
   .sidenav-viewport {
     height: 100%;
     max-height: 100vh;
     position: sticky;
     top: 0;
+    border-right: 1px solid var(--bst-color-border);
 
     .sidenav-drawer {
       display: flex;
       flex-direction: column;
       height: 100%;
 
       nav.menu {
```

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/sections/_navbar.scss` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/sections/_navbar.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/variables/_admonitions.scss` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/variables/_admonitions.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/variables/_color.scss` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/variables/_color.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/variables/_fonts.scss` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/variables/_fonts.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/styles/variables/_icons.scss` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/variables/_icons.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/translations/README.md` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/translations/README.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/demo/module.py` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/demo/module.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/demo/sphinxext.py` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/demo/sphinxext.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/pygment.py` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/pygment.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-field.html` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-field.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/theme-swither.html` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/theme-swither.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html`

 * *Files 3% similar despite different names*

```diff
@@ -10,40 +10,44 @@
 titles_only=True)
 -%}
 
 {% block htmlbody -%}
 {% include "partials/icons.html" %}
 
 {% block docs_headnav %}
-{% if theme_have_top_navbar %}
-<nav class="navbar has-shadow {% if theme_fix_navbar %} is-fixed-top {% endif %} {% if theme_navbar_color_style %} {{ theme_navbar_color_style }} {% endif %}"
-    role="navigation" aria-label="main navigation">
-    {% include "sections/headnav.html" %}
-</nav>
-{% endif %}
+<header>
+    {% if theme_have_top_navbar %}
+    <nav class="navbar has-shadow {% if theme_fix_navbar %} is-fixed-top {% endif %} {% if theme_navbar_color_style %} {{ theme_navbar_color_style }} {% endif %}"
+        role="navigation" aria-label="main navigation">
+        {% include "sections/headnav.html" %}
+    </nav>
+    {% endif %}
+</header>
 {% endblock docs_headnav %}
 
 {%- block mainbody -%}
 <div class="bulma-main">
     <div class="main-wrapper">
         {% if theme_show_back_to_top %}
         {%- include "components/back-to-top.html" -%}
         {% endif %}
 
         {%- include "search-wrapper.html" -%}
 
-        <div class="bulma-sidenav is-hidden-mobile">
+        <div class="bulma-sidenav" id="sidenavMenu">
             <div class="sidenav-viewport">
                 {% block left_sidebar %}
                 {%- include "sections/sidenav.html" -%}
                 {% endblock left_sidebar %}
             </div>
         </div>
 
         <main class="bulma-content">
+            {%- include "components/toggle-sidenav.html" -%}
+
             <div class="columns">
                 <article role="main" class="column is-three-quarters article-container">
                     {% include "sections/article-top.html" %}
                     {% include "components/searchbox.html" %}
 
                     {% block body %}{{ body }}{% endblock body %}
```

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_css_variables_define.html` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_css_variables_define.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/icons.html` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/icons.html`

 * *Files 8% similar despite different names*

```diff
@@ -27,20 +27,14 @@
             <path d="M20 18v-5.5c0 -.667 -.167 -1.333 -.5 -2" />
             <path
                 d="M12 7.5l0 -.297l.01 -.269l.027 -.298l.013 -.105l.033 -.215c.014 -.073 .029 -.146 .046 -.22l.06 -.223c.336 -1.118 1.262 -2.237 3.808 -1.873c2.838 .405 3.703 1.797 3.93 2.842l.036 .204c0 .033 .01 .066 .013 .098l.016 .185l0 .171l0 .49l-.015 .394l-.02 .271c-.122 1.366 -.655 2.845 -2.962 2.845c-3.256 0 -4.524 -1.656 -4.883 -3.081l-.053 -.242a3.865 3.865 0 0 1 -.036 -.235l-.021 -.227a3.518 3.518 0 0 1 -.007 -.215z" />
             <path d="M10 15v2" />
             <path d="M14 15v2" />
         </svg>
     </symbol>
-    <symbol id="svg-bulma" viewBox="0 0 42 64">
-        <svg width="42" height="64" viewBox="0 0 42 64" fill="none" xmlns="http://www.w3.org/2000/svg">
-            <path fill-rule="evenodd" clip-rule="evenodd"
-                d="M0 44L3.81818 16L19.0909 0L38.1818 20L26.7273 32L42 48L19.0909 64L0 44Z" fill="#00D1B2" />
-        </svg>
-    </symbol>
     <symbol id="svg-pencil" viewBox="0 0 16 16">
         <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16">
             <path
                 d="M11.013 1.427a1.75 1.75 0 0 1 2.474 0l1.086 1.086a1.75 1.75 0 0 1 0 2.474l-8.61 8.61c-.21.21-.47.364-.756.445l-3.251.93a.75.75 0 0 1-.927-.928l.929-3.25c.081-.286.235-.547.445-.758l8.61-8.61Zm.176 4.823L9.75 4.81l-6.286 6.287a.253.253 0 0 0-.064.108l-.558 1.953 1.953-.558a.253.253 0 0 0 .108-.064Zm1.238-3.763a.25.25 0 0 0-.354 0L10.811 3.75l1.439 1.44 1.263-1.263a.25.25 0 0 0 0-.354Z">
             </path>
         </svg>
     </symbol>
```

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 {% if (theme_article_top_left or theme_article_top_right) and (title and pagename != root_doc) %}
-<div class="level bulma-article-top">
-    <div class="level-left">
-        {% if theme_article_top_left %}
+<div class="bulma-article-top">
+
+    {% if theme_article_top_left %}
+    <div class="article-top-left">
         {%- for top_left in theme_article_top_left %}
         {%- include top_left %}
         {%- endfor %}
-        {% endif %}
     </div>
+    {% endif %}
 
-    <div class="level-right">
-        {% if theme_article_top_right %}
+    {% if theme_article_top_right %}
+    <div class="article-top-right">
         {%- for top_right in theme_article_top_right %}
         {%- include top_right %}
         {%- endfor %}
-        {% endif %}
     </div>
+    {% endif %}
 </div>
 {% endif %}
```

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/headnav.html` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/headnav.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+{%- set icon_class = "navbar-item" -%}
+
 <div class="navbar-brand">
     {% include "components/brand-logo.html" %}
 
-    <a role="button" class="navbar-burger" aria-label="menu" aria-expanded="false" data-target="navMenu">
+    <a role="button" class="navbar-burger" aria-label="menu" aria-expanded="false" data-target="navbarMenu">
         <span aria-hidden="true"></span>
         <span aria-hidden="true"></span>
         <span aria-hidden="true"></span>
     </a>
 </div>
 
-<div class="navbar-menu" id="navMenu">
+<div class="navbar-menu" id="navbarMenu">
     <div class="navbar-start">
         {% if theme_navbar_start %}
         {%- for ns_section in theme_navbar_start %}
         {% if ns_section in theme_navbar_include_directly %}
         {%- include ns_section %}
         {% else %}
         <div class="navbar-item">
```

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/theme.conf` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/theme.conf`

 * *Files 12% similar despite different names*

```diff
@@ -9,42 +9,43 @@
 [options]
 have_top_navbar = True
 navigation_depth = 4
 show_nav_level = 1
 show_toc_level = 1
 header_links_before_dropdown = 4
 external_links =
-header_icons =
+icon_links =
 logo =
 fix_navbar =
 # see https://pygments.org/styles/ for more styles
 pygment_light_style = manni
 pygment_dark_style = material
 
 # see https://bulma.io/documentation/components/navbar/#colors for more navbar color styles
 navbar_color_style = is-white
 navbar_start = navbar-nav.html
-navbar_end = header-icons.html
-navbar_include_directly = navbar-nav.html, header-icons.html
+navbar_end = theme-swither.html, icon-links.html
+navbar_include_directly = navbar-nav.html, icon-links.html
 analytics =
 footer = copyright.html, sphinx-version.html
 toc_title = On this page
 dropdown_label_name = More
 dropdown_label_target_url =
 navigation_with_keys = True
 search_bar_text = Search the docs ...
 show_back_to_top = True
 article_top_left = breadcrumbs.html
-article_top_right = edit-this-page.html
+article_top_right =
 article_bottom_left = last-updated.html
-article_bottom_right = sourcelink.html
+article_bottom_right = sourcelink.html, edit-this-page.html
 use_edit_page_button =
 source_repository =
 source_branch =
 source_directory =
 source_edit_link =
 show_prev_next = True
-information_panel = theme-swither.html
+information_panel = search-button.html
+information_panel_include_directly = search-button.html, theme-swither.html
 # define css variables
 light_colors =
 dark_colors =
 css_variables =
```

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/toctree.py` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/toctree.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/transforms.py` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,12 +116,12 @@
         )
         for node in list(get_nodes(nodes.table)):
             new_node = nodes.container(classes=["table-wrapper"])
             new_node.update_all_atts(node)
             node.parent.replace(node, new_node)
             new_node.append(node)
 
-        for node in list(get_nodes(nodes.math_block)):
-            new_node = nodes.container(classes=["math-wrapper"])
-            new_node.update_all_atts(node)
-            node.parent.replace(node, new_node)
-            new_node.append(node)
+        # for node in list(get_nodes(nodes.math_block)):
+        #     new_node = nodes.container(classes=["math-wrapper"])
+        #     new_node.update_all_atts(node)
+        #     node.parent.replace(node, new_node)
+        #     new_node.append(node)
```

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/translations.py` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/translations.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/src/bulma_sphinx_theme/utils.py` & `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/utils.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/webpack.config.js` & `bulma_sphinx_theme-0.0.9/webpack.config.js`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.8/PKG-INFO` & `bulma_sphinx_theme-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bulma-sphinx-theme
-Version: 0.0.8
+Version: 0.0.9
 Summary: A sphinx theme based on bulma.
 Author-Email: zclab <syfhub@hotmail.com>
 License: MIT License
         
         Copyright (c) 2023 zc
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -86,10 +86,16 @@
 html_theme = "bulma_sphinx_theme"
 ```
 
 Your Sphinx documentation's HTML pages will now be generated with this theme! 🎉
 
 <!-- end quickstart -->
 
+## Examples
+
+An examples without fixed navbar: <https://zclab.github.io/bst-demo/>
+
+An examples without navbar: <https://zclab.github.io/bst-nonavbar/>
+
 ## Documentation
 
 See [the bulma sphinx theme](https://bulma-sphinx-theme.readthedocs.io/en/latest/) for more information. Your can also refer to [Bulma Documentation](https://bulma.io/) for more sophisticated change.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bulma-sphinx-theme Version: 0.0.8 Summary: A sphinx
+Metadata-Version: 2.1 Name: bulma-sphinx-theme Version: 0.0.9 Summary: A sphinx
 theme based on bulma. Author-Email: zclab
 hotmail.com> License: MIT License Copyright (c) 2023 zc Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
@@ -44,11 +44,14 @@
 /github.com/zclab/bulma-sphinx-theme/blob/main/LICENSE) [![Github Stars](https:
 //img.shields.io/github/stars/zclab/bulma-sphinx-theme?style=flat-
 square&logo=github)](https://github.com/zclab/bulma-sphinx-theme)  ## Get
 started  To use this theme in your documentation build environment, first
 install the `bulma-sphinx-theme` with `pip`: ``` pip install bulma-sphinx-theme
 ``` then, configure the Sphinx docs to use the theme by editing `conf.py`
 ```python html_theme = "bulma_sphinx_theme" ``` Your Sphinx documentation's
-HTML pages will now be generated with this theme! ð  ## Documentation See
-[the bulma sphinx theme](https://bulma-sphinx-theme.readthedocs.io/en/latest/
-) for more information. Your can also refer to [Bulma Documentation](https://
-bulma.io/) for more sophisticated change.
+HTML pages will now be generated with this theme! ð  ## Examples An examples
+without fixed navbar:
+zclab.github.io/bst-demo/> An examples without navbar:
+zclab.github.io/bst-nonavbar/> ## Documentation See [the bulma sphinx theme]
+(https://bulma-sphinx-theme.readthedocs.io/en/latest/) for more information.
+Your can also refer to [Bulma Documentation](https://bulma.io/) for more
+sophisticated change.
```

